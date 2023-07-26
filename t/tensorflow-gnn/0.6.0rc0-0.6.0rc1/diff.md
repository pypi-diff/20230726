# Comparing `tmp/tensorflow-gnn-0.6.0rc0.tar.gz` & `tmp/tensorflow-gnn-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow-gnn-0.6.0rc0.tar", last modified: Thu Jul 20 17:59:41 2023, max compression
+gzip compressed data, was "tensorflow-gnn-0.6.0rc1.tar", last modified: Wed Jul 26 13:37:16 2023, max compression
```

## Comparing `tensorflow-gnn-0.6.0rc0.tar` & `tensorflow-gnn-0.6.0rc1.tar`

### file list

```diff
@@ -1,318 +1,318 @@
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      304 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/AUTHORS
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1481 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11357 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/LICENSE
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      177 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/MANIFEST.in
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)     5322 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/PKG-INFO
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4019 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/README.md
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1392 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/WORKSPACE
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/package/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      477 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/package/BUILD
--rwxr-xr-x   0 mparadkar (603057) primarygroup (89939)     1633 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/package/move_generated_files.sh
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      953 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/package/tfdep.bzl
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)       38 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/setup.cfg
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7305 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/setup.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2072 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9298 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/__init__.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/__init__.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/ogb/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/ogb/__init__.py
--rwxr-xr-x   0 mparadkar (603057) primarygroup (89939)    17657 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1386 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/ogb/convert_ogb_to_npz.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3645 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/ogb/ogb_lib.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3291 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/triples.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1567 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/triples_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1141 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    41983 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/unigraph.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    31879 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/unigraph_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1475 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/__init__.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    45889 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/datasets.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2874 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/datasets_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    38944 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    18108 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13960 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/models.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4786 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/networkx_data.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2589 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/networkx_data_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3138 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/reader_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11411 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/unigraph_data.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11598 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/unigraph_data_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      840 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2230 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/__init__.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.455089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5537 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7559 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/accessors.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9061 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/accessors_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15545 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/edge_samplers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12823 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/edge_samplers_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    24769 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/executor_lib.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8426 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/executor_lib_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9854 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/sampler.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4272 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/sampler_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4018 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/unigraph_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27898 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/unigraph_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5391 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5926 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    56324 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/core.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    46060 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/core_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7585 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/custom_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5659 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/eval_dag.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    28756 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/eval_dag.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    30581 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/eval_dag_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6359 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/ext_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3590 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/ext_ops_parallel.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11443 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/ext_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6255 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/ext_ops_vectorized.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8061 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/interfaces.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    18838 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/link_samplers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14953 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/link_samplers_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11911 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/subgraph_pipeline.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13508 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/subgraph_pipeline_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.455089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14334 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    20785 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/adjacency.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13080 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/adjacency_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    39354 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/batching_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    32323 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/batching_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11447 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/broadcast_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14107 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/broadcast_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1289 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/dict_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1348 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/dict_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3920 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_constants.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    40849 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_piece.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    28881 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_piece_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    63673 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6176 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_encode.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5885 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_encode_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    20523 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_io.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27804 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_io_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    45886 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    67747 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2735 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_pprint.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1587 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_pprint_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10963 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_random.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5892 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_random_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    62064 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2635 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_test_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6722 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/normalization_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10486 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/normalization_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27049 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/padding_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    26711 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/padding_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    34642 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/pool_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    22200 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/pool_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7818 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/preprocessing_common.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9088 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/preprocessing_common_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    28826 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/readout.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    20098 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/readout_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12726 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10402 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    17764 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_validation.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16543 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_validation_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5192 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tag_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4878 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tag_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19429 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tensor_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12925 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tensor_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2984 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tf_internal.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.455089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2982 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1307 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10481 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/builders.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15288 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/builders_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2888 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/initializers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2005 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/initializers_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14805 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/keras_e2e_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5740 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/keras_tensors.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13602 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/keras_tensors_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.459089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6490 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2016 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19666 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolution_base.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15800 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolution_base_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6681 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolutions.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5907 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolutions_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    38598 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/graph_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    54518 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/graph_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    25526 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/graph_update.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10300 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/graph_update_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2904 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/item_dropout.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3874 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/item_dropout_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19343 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/map_features.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    26710 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/map_features_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11360 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/next_state.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6587 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/next_state_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2478 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/padding_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6795 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/padding_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2149 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/parse_example.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6313 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/parse_example_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.447089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.459089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2880 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1356 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6852 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/distribute_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11577 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15368 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/layers_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6262 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/losses.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5509 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/losses_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6836 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/metrics.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5301 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/metrics_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8940 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/tasks.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10842 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/tasks_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.459089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2367 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1467 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2390 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/config_dict.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3051 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/config_dict_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2867 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/hparams_vizier.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1585 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/hparams_vizier_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    28134 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    31034 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/layers_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.459089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      983 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1030 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14098 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/gcn_conv.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    31982 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/gcn_conv_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.459089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      999 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1285 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    33753 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27737 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/layers_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.459089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2219 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1207 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2354 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/config_dict.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3483 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/config_dict_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2678 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/hparams_vizier.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1498 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/hparams_vizier_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16008 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    32549 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/layers_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.459089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2467 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1437 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2784 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/config_dict.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2966 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/config_dict_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3615 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/hparams_vizier.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2318 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/hparams_vizier_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19186 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    17202 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/layers_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2395 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1566 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2433 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/config_dict.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3134 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/config_dict_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2906 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1599 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    37373 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    54358 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/layers_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2399 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1446 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2263 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2990 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2157 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1296 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5260 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7798 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/layers_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1013 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1023 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/examples.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12144 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/graph_schema.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2895 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/graph_schema.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2932 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4908 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8291 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/distribute_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.447089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.447089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1576 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    17093 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/train.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2697 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3158 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/utils_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/input/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      801 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/input/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19958 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/input/datasets.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9151 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/input/datasets_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9286 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/interfaces.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    24069 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/orchestration.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11036 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/orchestration_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2114 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11452 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/classification.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12562 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/classification_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8859 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/link_prediction.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6188 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/link_prediction_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11453 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/regression.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    18994 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/regression_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/trainers/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      499 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/trainers/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13322 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/trainers/keras_fit.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2974 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14492 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/attribution.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10359 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/attribution_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2438 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/label_fns.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1324 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/model_dir.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7788 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/model_export.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9780 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/model_export_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4245 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/padding.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2576 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/parsing.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4907 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/parsing_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1873 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/strategies.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1885 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      424 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19089 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/graph_sampler.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    22306 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/graph_sampler_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    22774 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_lib.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    32206 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_lib_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6762 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_spec.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    18498 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_spec_builder.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10322 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_spec_builder_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4931 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5281 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2123 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/subgraph.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13461 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/subgraph.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16517 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/subgraph_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2769 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tensorflow_gnn.bzl
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      455 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3368 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/generate_training_data.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1375 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/generate_training_data_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3926 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/print_training_data.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2080 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/print_training_data_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2700 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/sampled_stats.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7984 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/sampled_stats.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1975 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/sampled_stats_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1742 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/validate_graph_schema.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/utils/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      343 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/utils/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        1 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/utils/__init__.py
--rwxr-xr-x   0 mparadkar (603057) primarygroup (89939)     2116 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/utils/test_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2131 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/version.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)     5322 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/PKG-INFO
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)    11918 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/SOURCES.txt
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/dependency_links.txt
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)      459 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/entry_points.txt
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/namespace_packages.txt
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/not-zip-safe
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)      244 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/requires.txt
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)       22 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/top_level.txt
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/testdata/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      238 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/testdata/BUILD
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/testdata/heterogeneous/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      420 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/testdata/heterogeneous/BUILD
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/testdata/homogeneous/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      294 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/testdata/homogeneous/BUILD
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/testdata/node_vs_edge/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      366 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/testdata/node_vs_edge/BUILD
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.848797 tensorflow-gnn-0.6.0rc1/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      304 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/AUTHORS
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1481 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11357 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/LICENSE
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      177 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/MANIFEST.in
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)     5322 2023-07-26 13:37:16.848797 tensorflow-gnn-0.6.0rc1/PKG-INFO
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4019 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/README.md
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1392 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/WORKSPACE
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.832797 tensorflow-gnn-0.6.0rc1/package/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      477 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/package/BUILD
+-rwxr-xr-x   0 mparadkar (603057) primarygroup (89939)     1633 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/package/move_generated_files.sh
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      953 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/package/tfdep.bzl
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)       38 2023-07-26 13:37:16.848797 tensorflow-gnn-0.6.0rc1/setup.cfg
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7305 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/setup.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.832797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2072 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9298 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/__init__.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.832797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/converters/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/converters/__init__.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.832797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/converters/ogb/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/converters/ogb/__init__.py
+-rwxr-xr-x   0 mparadkar (603057) primarygroup (89939)    17657 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1386 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/converters/ogb/convert_ogb_to_npz.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3645 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/converters/ogb/ogb_lib.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3291 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/converters/triples.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1567 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/converters/triples_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.832797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/data/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1141 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/data/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/data/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    41983 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/data/unigraph.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    31879 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/data/unigraph_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.832797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1475 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/__init__.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.832797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    45889 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/datasets.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2874 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/datasets_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    38944 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    18108 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13960 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/models.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4786 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/networkx_data.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2589 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/networkx_data_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3138 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/reader_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11411 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/unigraph_data.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11598 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/unigraph_data_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.836797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      840 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2230 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/__init__.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.836797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5537 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7559 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/accessors.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9061 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/accessors_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15545 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/edge_samplers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12823 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/edge_samplers_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    24769 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/executor_lib.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8426 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/executor_lib_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9854 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/sampler.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4272 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/sampler_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4018 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/unigraph_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27898 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/unigraph_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5391 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5926 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    56324 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/core.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    46060 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/core_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7585 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/custom_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5659 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/eval_dag.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    28756 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/eval_dag.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    30581 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/eval_dag_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6359 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/ext_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3590 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/ext_ops_parallel.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11443 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/ext_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6255 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/ext_ops_vectorized.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8061 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/interfaces.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    18838 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/link_samplers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14953 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/link_samplers_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11911 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/subgraph_pipeline.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13508 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/subgraph_pipeline_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.836797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14334 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    20785 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/adjacency.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13080 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/adjacency_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    39354 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/batching_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    32323 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/batching_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11447 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/broadcast_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14107 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/broadcast_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1289 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/dict_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1348 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/dict_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3920 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_constants.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    40849 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_piece.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    28881 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_piece_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    63673 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6176 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_encode.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5885 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_encode_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    20523 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_io.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27804 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_io_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    45886 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    67747 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2735 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_pprint.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1587 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_pprint_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10963 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_random.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5892 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_random_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    62064 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2635 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_test_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6722 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/normalization_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10486 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/normalization_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27049 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/padding_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    26711 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/padding_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    34642 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/pool_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    22200 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/pool_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7818 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/preprocessing_common.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9088 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/preprocessing_common_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    28826 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/readout.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    20098 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/readout_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12726 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/schema_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10402 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/schema_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    17764 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/schema_validation.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16543 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/schema_validation_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5192 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/tag_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4878 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/tag_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19429 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/tensor_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12925 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/tensor_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2984 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/tf_internal.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.840797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2982 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1307 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10481 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/builders.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15288 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/builders_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2888 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/initializers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2005 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/initializers_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14805 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/keras_e2e_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5740 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/keras_tensors.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13602 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/keras_tensors_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.840797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6490 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2016 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19666 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/convolution_base.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15800 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/convolution_base_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6681 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/convolutions.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5907 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/convolutions_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    38598 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/graph_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    54518 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/graph_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    25526 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/graph_update.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10300 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/graph_update_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2904 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/item_dropout.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3874 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/item_dropout_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19343 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/map_features.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    26710 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/map_features_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11360 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/next_state.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6587 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/next_state_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2478 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/padding_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6795 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/padding_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2149 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/parse_example.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6313 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/parse_example_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.828797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.840797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2880 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1356 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6852 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/distribute_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11577 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15368 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/layers_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6262 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/losses.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5509 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/losses_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6836 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/metrics.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5301 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/metrics_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8940 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/tasks.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10842 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/tasks_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.840797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2367 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1467 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2390 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/config_dict.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3051 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/config_dict_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2867 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/hparams_vizier.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1585 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/hparams_vizier_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    28134 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    31034 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.840797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gcn/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      983 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gcn/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1030 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gcn/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14098 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gcn/gcn_conv.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    31982 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gcn/gcn_conv_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.840797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/graph_sage/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      999 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/graph_sage/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1285 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/graph_sage/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    33753 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/graph_sage/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27737 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/graph_sage/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.840797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2219 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1207 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2354 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/config_dict.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3483 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/config_dict_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2678 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/hparams_vizier.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1498 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/hparams_vizier_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16008 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    32549 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.844797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2467 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1437 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2784 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/config_dict.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2966 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/config_dict_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3615 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/hparams_vizier.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2318 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/hparams_vizier_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19186 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    17202 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.844797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2395 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1566 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2433 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/config_dict.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3134 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/config_dict_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2906 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1599 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    37373 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    54358 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.844797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2399 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1446 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2263 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/config_dict.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2990 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2157 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1296 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5260 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7798 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.844797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/proto/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1013 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/proto/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/proto/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1023 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/proto/examples.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12144 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/proto/graph_schema.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2895 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/proto/graph_schema.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.844797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2932 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4908 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8291 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/distribute_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.828797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/examples/
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.828797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/examples/ogbn/
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.844797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/examples/ogbn/mag/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1576 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/examples/ogbn/mag/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    17093 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/examples/ogbn/mag/train.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2697 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/examples/ogbn/mag/utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3158 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/examples/ogbn/mag/utils_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.844797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/input/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      801 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/input/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19958 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/input/datasets.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9151 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/input/datasets_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9286 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/interfaces.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    24069 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/orchestration.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11036 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/orchestration_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.844797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/tasks/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2114 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/tasks/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11452 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/tasks/classification.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12562 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/tasks/classification_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8859 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/tasks/link_prediction.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6188 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/tasks/link_prediction_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11453 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/tasks/regression.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    18994 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/tasks/regression_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.844797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/trainers/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      499 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/trainers/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13322 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/trainers/keras_fit.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.844797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2974 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14492 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/attribution.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10359 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/attribution_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2438 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/label_fns.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1324 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/model_dir.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7788 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/model_export.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9780 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/model_export_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4245 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/padding.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2576 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/parsing.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4907 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/parsing_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1873 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/strategies.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.848797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1885 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      424 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19089 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/graph_sampler.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    22306 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/graph_sampler_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    22774 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/sampling_lib.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    32206 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/sampling_lib_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6762 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/sampling_spec.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    18498 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/sampling_spec_builder.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10322 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/sampling_spec_builder_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4931 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/sampling_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5281 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/sampling_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2123 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/subgraph.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13461 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/subgraph.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16517 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/subgraph_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2769 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tensorflow_gnn.bzl
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.848797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      455 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3368 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/generate_training_data.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1375 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/generate_training_data_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3926 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/print_training_data.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2080 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/print_training_data_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2700 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/sampled_stats.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7984 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/sampled_stats.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1975 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/sampled_stats_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1742 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/validate_graph_schema.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.848797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/utils/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      343 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/utils/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        1 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/utils/__init__.py
+-rwxr-xr-x   0 mparadkar (603057) primarygroup (89939)     2116 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/utils/test_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2131 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn/version.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.832797 tensorflow-gnn-0.6.0rc1/tensorflow_gnn.egg-info/
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)     5322 2023-07-26 13:37:16.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn.egg-info/PKG-INFO
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)    11918 2023-07-26 13:37:16.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn.egg-info/SOURCES.txt
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-07-26 13:37:16.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn.egg-info/dependency_links.txt
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)      459 2023-07-26 13:37:16.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn.egg-info/entry_points.txt
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-07-26 13:37:16.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn.egg-info/namespace_packages.txt
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-07-26 13:37:16.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn.egg-info/not-zip-safe
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)      244 2023-07-26 13:37:16.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn.egg-info/requires.txt
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)       22 2023-07-26 13:37:16.000000 tensorflow-gnn-0.6.0rc1/tensorflow_gnn.egg-info/top_level.txt
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.848797 tensorflow-gnn-0.6.0rc1/testdata/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      238 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/testdata/BUILD
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.848797 tensorflow-gnn-0.6.0rc1/testdata/heterogeneous/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      420 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/testdata/heterogeneous/BUILD
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.848797 tensorflow-gnn-0.6.0rc1/testdata/homogeneous/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      294 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/testdata/homogeneous/BUILD
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-26 13:37:16.848797 tensorflow-gnn-0.6.0rc1/testdata/node_vs_edge/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      366 2023-07-26 13:03:54.000000 tensorflow-gnn-0.6.0rc1/testdata/node_vs_edge/BUILD
```

### Comparing `tensorflow-gnn-0.6.0rc0/BUILD` & `tensorflow-gnn-0.6.0rc1/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/LICENSE` & `tensorflow-gnn-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/PKG-INFO` & `tensorflow-gnn-0.6.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-gnn
-Version: 0.6.0rc0
+Version: 0.6.0rc1
 Summary: A library for building scalable graph neural networks in TensorFlow.
 Home-page: https://github.com/tensorflow/gnn
 Download-URL: https://github.com/tensorflow/gnn.git
 Author: Google LLC
 Author-email: tensorflow-gnn@googlegroups.com
 License: Apache 2.0
 Keywords: tensorflow gnn graph
```

### Comparing `tensorflow-gnn-0.6.0rc0/README.md` & `tensorflow-gnn-0.6.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/WORKSPACE` & `tensorflow-gnn-0.6.0rc1/WORKSPACE`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/package/move_generated_files.sh` & `tensorflow-gnn-0.6.0rc1/package/move_generated_files.sh`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/package/tfdep.bzl` & `tensorflow-gnn-0.6.0rc1/package/tfdep.bzl`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/setup.py` & `tensorflow-gnn-0.6.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/__init__.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/ogb/convert_ogb_to_npz.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/converters/ogb/convert_ogb_to_npz.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/ogb/ogb_lib.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/converters/ogb/ogb_lib.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/triples.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/converters/triples.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/triples_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/converters/triples_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/data/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/unigraph.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/data/unigraph.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/unigraph_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/data/unigraph_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/__init__.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/datasets.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/datasets.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/datasets_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/datasets_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/models.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/models.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/networkx_data.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/networkx_data.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/networkx_data_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/networkx_data_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/reader_utils.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/reader_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/unigraph_data.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/unigraph_data.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/unigraph_data_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/in_memory/unigraph_data_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/__init__.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/accessors.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/accessors.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/accessors_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/accessors_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/edge_samplers.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/edge_samplers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/edge_samplers_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/edge_samplers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/executor_lib.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/executor_lib.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/executor_lib_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/executor_lib_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/sampler.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/sampler.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/sampler_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/sampler_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/unigraph_utils.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/unigraph_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/unigraph_utils_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/unigraph_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/utils.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/utils_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/beam/utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/core.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/core.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/core_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/core_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/custom_ops_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/custom_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/eval_dag.proto` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/eval_dag.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/eval_dag.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/eval_dag.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/eval_dag_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/eval_dag_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/ext_ops.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/ext_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/ext_ops_parallel.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/ext_ops_parallel.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/ext_ops_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/ext_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/ext_ops_vectorized.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/ext_ops_vectorized.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/interfaces.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/link_samplers.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/link_samplers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/link_samplers_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/link_samplers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/subgraph_pipeline.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/subgraph_pipeline.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/subgraph_pipeline_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/experimental/sampler/subgraph_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/adjacency.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/adjacency.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/adjacency_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/adjacency_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/batching_utils.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/batching_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/batching_utils_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/batching_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/broadcast_ops.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/broadcast_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/broadcast_ops_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/broadcast_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/dict_utils.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/dict_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/dict_utils_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/dict_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_constants.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_constants.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_piece.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_piece.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_piece_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_piece_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_encode.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_encode.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_encode_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_encode_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_io.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_io.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_io_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_io_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_ops.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_ops_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_pprint.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_pprint.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_pprint_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_pprint_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_random.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_random.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_random_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_random_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_test_utils.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/graph_tensor_test_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/normalization_ops.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/normalization_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/normalization_ops_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/normalization_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/padding_ops.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/padding_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/padding_ops_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/padding_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/pool_ops.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/pool_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/pool_ops_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/pool_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/preprocessing_common.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/preprocessing_common.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/preprocessing_common_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/preprocessing_common_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/readout.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/readout.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/readout_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/readout_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_utils.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/schema_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_utils_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_validation.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/schema_validation.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_validation_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/schema_validation_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tag_utils.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/tag_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tag_utils_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/tag_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tensor_utils.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tensor_utils_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/tensor_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tf_internal.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/graph/tf_internal.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/__init__.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/builders.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/builders.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/builders_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/builders_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/initializers.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/initializers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/initializers_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/initializers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/keras_e2e_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/keras_e2e_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/keras_tensors.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/keras_tensors.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/keras_tensors_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/keras_tensors_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/__init__.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolution_base.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/convolution_base.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolution_base_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/convolution_base_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolutions.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/convolutions.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolutions_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/convolutions_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/graph_ops.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/graph_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/graph_ops_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/graph_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/graph_update.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/graph_update.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/graph_update_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/graph_update_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/item_dropout.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/item_dropout.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/item_dropout_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/item_dropout_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/map_features.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/map_features.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/map_features_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/map_features_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/next_state.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/next_state.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/next_state_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/next_state_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/padding_ops.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/padding_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/padding_ops_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/padding_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/parse_example.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/parse_example.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/parse_example_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/keras/layers/parse_example_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/__init__.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/distribute_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/distribute_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/layers.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/layers_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/losses.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/losses.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/losses_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/losses_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/metrics.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/metrics.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/metrics_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/metrics_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/tasks.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/tasks.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/tasks_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/contrastive_losses/tasks_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/__init__.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/config_dict.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/config_dict.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/config_dict_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/config_dict_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/hparams_vizier.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/hparams_vizier.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/hparams_vizier_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/hparams_vizier_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/layers.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/layers_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gat_v2/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gcn/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/__init__.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gcn/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/gcn_conv.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gcn/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/gcn_conv_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/gcn/gcn_conv_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/graph_sage/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/__init__.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/graph_sage/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/layers.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/graph_sage/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/layers_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/graph_sage/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/__init__.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/config_dict.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/config_dict.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/config_dict_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/config_dict_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/hparams_vizier.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/hparams_vizier.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/hparams_vizier_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/hparams_vizier_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/layers.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/layers_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/hgt/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/__init__.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/config_dict.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/config_dict.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/config_dict_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/config_dict_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/hparams_vizier.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/hparams_vizier.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/hparams_vizier_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/hparams_vizier_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/layers.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/layers_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/mt_albis/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/__init__.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/config_dict.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/config_dict.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/config_dict_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/config_dict_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/layers.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/layers_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/multi_head_attention/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/__init__.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/config_dict.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/layers.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/layers.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/layers_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/models/vanilla_mpnn/layers_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/proto/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/examples.proto` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/proto/examples.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/graph_schema.proto` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/proto/graph_schema.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/graph_schema.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/proto/graph_schema.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/__init__.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/distribute_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/distribute_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/examples/ogbn/mag/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/train.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/examples/ogbn/mag/train.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/utils.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/examples/ogbn/mag/utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/utils_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/examples/ogbn/mag/utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/input/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/input/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/input/datasets.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/input/datasets.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/input/datasets_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/input/datasets_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/interfaces.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/orchestration.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/orchestration.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/orchestration_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/orchestration_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/tasks/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/classification.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/classification_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/tasks/classification_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/link_prediction.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/tasks/link_prediction.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/link_prediction_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/tasks/link_prediction_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/regression.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/tasks/regression.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/regression_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/tasks/regression_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/trainers/keras_fit.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/trainers/keras_fit.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/attribution.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/attribution.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/attribution_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/attribution_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/label_fns.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/label_fns.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/model_dir.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/model_dir.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/model_export.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/model_export.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/model_export_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/model_export_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/padding.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/padding.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/parsing.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/parsing_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/parsing_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/strategies.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/runner/utils/strategies.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/BUILD` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/graph_sampler.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/graph_sampler.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/graph_sampler_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/graph_sampler_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_lib.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/sampling_lib.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_lib_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/sampling_lib_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_spec.proto` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/sampling_spec.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_spec_builder.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/sampling_spec_builder.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_spec_builder_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/sampling_spec_builder_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_utils.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/sampling_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_utils_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/sampling_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/subgraph.proto` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/subgraph.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/subgraph.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/subgraph.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/subgraph_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/sampler/subgraph_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tensorflow_gnn.bzl` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tensorflow_gnn.bzl`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/generate_training_data.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/generate_training_data.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/generate_training_data_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/generate_training_data_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/print_training_data.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/print_training_data.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/print_training_data_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/print_training_data_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/sampled_stats.proto` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/sampled_stats.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/sampled_stats.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/sampled_stats.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/sampled_stats_test.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/sampled_stats_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/validate_graph_schema.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/tools/validate_graph_schema.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/utils/test_utils.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/version.py` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 #
 # Patch releases X.Y.Z, Z > 0, incl. their release candidates, can be done for
 # patches on branch rX.Y as needed.
 #
 # IMPORANT: Right after branching rX.Y, bump the main branch to X.(Y+1).0.dev1.
 # (Submit a change to the Source of Truth, get it out on the main branch asap.)
 
-__version__ = "0.6.0rc0"
+__version__ = "0.6.0rc1"
```

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/PKG-INFO` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-gnn
-Version: 0.6.0rc0
+Version: 0.6.0rc1
 Summary: A library for building scalable graph neural networks in TensorFlow.
 Home-page: https://github.com/tensorflow/gnn
 Download-URL: https://github.com/tensorflow/gnn.git
 Author: Google LLC
 Author-email: tensorflow-gnn@googlegroups.com
 License: Apache 2.0
 Keywords: tensorflow gnn graph
```

### Comparing `tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/SOURCES.txt` & `tensorflow-gnn-0.6.0rc1/tensorflow_gnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

