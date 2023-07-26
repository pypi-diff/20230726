# Comparing `tmp/trailmet-0.0.1rc2.tar.gz` & `tmp/trailmet-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trailmet-0.0.1rc2.tar", last modified: Mon Jul 10 18:58:37 2023, max compression
+gzip compressed data, was "dist/trailmet-0.0.1rc3.tar", last modified: Wed Jul 26 13:14:06 2023, max compression
```

## Comparing `trailmet-0.0.1rc2.tar` & `trailmet-0.0.1rc3.tar`

### file list

```diff
@@ -1,81 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/algorithms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/algorithms/binarize/
--rw-r--r--   0 runner    (1001) docker     (123)    22386 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/binarize/BNNBN.py
--rw-r--r--   0 runner    (1001) docker     (123)    21686 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/binarize/ReActNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/binarize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/binarize/binarize.py
--rw-r--r--   0 runner    (1001) docker     (123)    17234 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/binarize/birealnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/binarize/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15922 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/attention_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/distill.py
--rw-r--r--   0 runner    (1001) docker     (123)    26230 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/factor_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/response_kd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/distill/rkd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27307 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/chip.py
--rw-r--r--   0 runner    (1001) docker     (123)    37915 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/chipnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17230 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/growth_regularisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/network_slimming.py
--rw-r--r--   0 runner    (1001) docker     (123)    19335 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/pns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/l1_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)    20535 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/meta_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)    32365 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/reg_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/prune/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33476 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/bitsplit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19698 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/brecq.py
--rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/lapq.py
--rw-r--r--   0 runner    (1001) docker     (123)    32027 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    22819 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/qmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/quantize.py
--rw-r--r--   0 runner    (1001) docker     (123)    29083 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/quantize/reconstruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/algorithms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    19597 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/algorithms/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/datasets/classification/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/datasets/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/datasets/classification/chest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/datasets/classification/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/datasets/classification/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/datasets/classification/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/datasets/classification/tcga.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/models/
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/mobilenetv2_bireal.py
--rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    21882 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/resnet_bireal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/resnet_chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/models/wideresnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/utils/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/utils/tp_pruning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-10 18:58:34.000000 trailmet-0.0.1rc2/trailmet/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 18:58:37.000000 trailmet-0.0.1rc2/trailmet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/trailmet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/trailmet/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/algorithms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/trailmet/algorithms/binarize/
+-rw-r--r--   0 runner    (1001) docker     (123)    22386 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/binarize/BNNBN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21686 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/binarize/ReActNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/binarize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/binarize/binarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17234 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/binarize/birealnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/binarize/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/trailmet/algorithms/distill/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/distill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15922 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/distill/attention_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/distill/distill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26230 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/distill/factor_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/distill/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/distill/response_kd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/distill/rkd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/trailmet/algorithms/prune/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/prune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27307 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/prune/chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37915 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/prune/chipnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17230 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/prune/growth_regularisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/prune/network_slimming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19335 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/prune/pns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/prune/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/trailmet/algorithms/prune/pruner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/prune/pruner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/prune/pruner/l1_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20535 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/prune/pruner/meta_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32365 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/prune/pruner/reg_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/prune/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/trailmet/algorithms/quantize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/quantize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33476 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/quantize/bitsplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19698 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/quantize/brecq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/quantize/lapq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32027 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/quantize/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22819 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/quantize/qmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/quantize/quantize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29083 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/quantize/reconstruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/trailmet/algorithms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    19597 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/algorithms/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/trailmet/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/trailmet/datasets/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/datasets/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/datasets/classification/chest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/datasets/classification/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/datasets/classification/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/datasets/classification/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/datasets/classification/tcga.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/trailmet/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/mobilenetv2_bireal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/trailmet/models/models_bnnbn/
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/models_bnnbn/Qa_reactnet_18_bf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/models_bnnbn/Qa_reactnet_18_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/models_bnnbn/Qa_reactnet_18_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/models_bnnbn/Qa_reactnet_A_bf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/models_bnnbn/Qa_reactnet_A_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/models_bnnbn/Qa_reactnet_A_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/models_bnnbn/Qaw_reactnet_18_bf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/models_bnnbn/Qaw_reactnet_18_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/models_bnnbn/Qaw_reactnet_18_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/models_bnnbn/Qaw_reactnet_A_bf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/models_bnnbn/Qaw_reactnet_A_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/models_bnnbn/Qaw_reactnet_A_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/models_bnnbn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/models_bnnbn/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21882 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/resnet_bireal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/resnet_chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/models/wideresnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/trailmet/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/utils/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/utils/tp_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-26 13:13:59.000000 trailmet-0.0.1rc3/trailmet/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/trailmet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-26 13:14:05.000000 trailmet-0.0.1rc3/trailmet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-26 13:14:06.000000 trailmet-0.0.1rc3/trailmet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:14:05.000000 trailmet-0.0.1rc3/trailmet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:14:05.000000 trailmet-0.0.1rc3/trailmet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-26 13:14:05.000000 trailmet-0.0.1rc3/trailmet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 13:14:05.000000 trailmet-0.0.1rc3/trailmet.egg-info/top_level.txt
```

### Comparing `trailmet-0.0.1rc2/PKG-INFO` & `trailmet-0.0.1rc3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: trailmet
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: Transmute AI Model Efficiency Toolkit
 Home-page: https://github.com/transmuteAI/trailmet
 Author: TrAILMET Contributors
 Author-email: transmute.ai@gmail.com
 License: MIT License
 Description: <p align="center">
             <br>
                 <img src="docs/source/imgs/trailmet.png" width="500"/>
             </br>
             <br>
                 <strong> Transmute AI Model Efficiency Toolkit </strong>
             </br>
         </p>
         <p align="center">
+            <a href="https://pypi.org/project/trailmet/">
+            <img src="https://pepy.tech/badge/trailmet" />
+            </a>
+            <a href="https://pypi.org/project/trailmet/">
+            <img src="https://badge.fury.io/py/trailmet.svg" />
+            </a>
             <a href="https://github.com/transmuteAI/trailmet/blob/dev/LICENSE">
                 <img alt="GitHub" src="https://img.shields.io/github/license/transmuteAI/trailmet?color=blue">
             </a>
             <a href="https://transmuteai-trailmet.readthedocs.io/en/latest/">
                 <img alt="Documentation" src="https://img.shields.io/badge/docs-passing-brightgreen">
             </a>
             <a href="https://github.com/transmuteAI/trailmet/actions/workflows/ci.yml">
@@ -52,15 +58,15 @@
         
         ```shell
         git clone https://github.com/transmuteAI/trailmet.git
         cd trailmet
         conda create -n trailmet
         conda activate trailmet
         conda install pytorch=1.13 torchvision=0.14 pytorch-cuda=11.7 -c pytorch -c nvidia
-        pip install -r requirements.txt
+        pip install trailmet
         ```
         
         # Algorithms Implemented
         
         Demo notebooks for each algorithm is added in [experiments](https://github.com/transmuteAI/trailmet/blob/dev/experiments) folder
         
         <details open>
```

#### html2text {}

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1 Name: trailmet Version: 0.0.1rc2 Summary: Transmute AI
+Metadata-Version: 2.1 Name: trailmet Version: 0.0.1rc3 Summary: Transmute AI
 Model Efficiency Toolkit Home-page: https://github.com/transmuteAI/trailmet
 Author: TrAILMET Contributors Author-email: transmute.ai@gmail.com License: MIT
 License Description:
 
                        [docs/source/imgs/trailmet.png]
                     Transmute AI Model Efficiency Toolkit
+  [https://pepy.tech/badge/trailmet] [https://badge.fury.io/py/trailmet.svg]
 [GitHub] [Documentation] [Run_tests_with_pytest] [GitHub_Stars] [GitHub_Forks]
 # Introduction Trailmet is a model efficiency toolkit for compressing deep
 learning models using state of the art compression techniques. Today deep
 learning models are not deployable because of their huge memory footprint,
 TRAILMET is an effort to make deep learning models more efficient in their size
 to performance ratio. It is developed using Pytorch 1.13. ### Major features -
 State of the art compression algorithms implemented. - Demo notebooks for
 training each algorithm. - Modular Design: All alogithms are modular and can
 customized easily for any kind of model and dataset. # Installation Below are
 quick steps for installation: ```shell git clone https://github.com/
 transmuteAI/trailmet.git cd trailmet conda create -n trailmet conda activate
 trailmet conda install pytorch=1.13 torchvision=0.14 pytorch-cuda=11.7 -
-c pytorch -c nvidia pip install -r requirements.txt ``` # Algorithms
-Implemented Demo notebooks for each algorithm is added in [experiments](https:/
-/github.com/transmuteAI/trailmet/blob/dev/experiments) folder   Knowledge
-Distillation - [x] [Response KD](https://arxiv.org/abs/1503.02531) - [x]
-[Factor Transfer](https://arxiv.org/abs/1802.04977) - [x] [Attention Transfer]
-(https://arxiv.org/abs/1612.03928)    Pruning  - [x] [Chipnet](https://
-arxiv.org/abs/2102.07156) - [x] [Network slimming](https://arxiv.org/abs/
-1708.06519) - [x] [Growth Regularization](https://arxiv.org/abs/2012.09243)
-Quantization - [x] [BitSplit](https://dl.acm.org/doi/abs/10.5555/
-3524938.3525851) - [x] [BRECQ](https://arxiv.org/abs/2102.05426) - [x] [LAPQ]
-(https://arxiv.org/abs/1911.07190)    Binarization - [x] [BiRealNet](https://
-arxiv.org/abs/1808.00278) - [x] [ReActNet](https://arxiv.org/abs/2003.03488) -
-[x] [BNN-BN](https://arxiv.org/abs/2104.08215v1)  # Acknowledgement # Citation
-If you find this project useful in your research, please consider cite:
-```BibTeX @misc{, title={}, author={}, howpublished = {}}, year={2023} } ``` #
-License This project is released under the [MIT license](LICENSE). Keywords:
-computer vision,image classification,model efficiency Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-all
+c pytorch -c nvidia pip install trailmet ``` # Algorithms Implemented Demo
+notebooks for each algorithm is added in [experiments](https://github.com/
+transmuteAI/trailmet/blob/dev/experiments) folder   Knowledge Distillation -
+[x] [Response KD](https://arxiv.org/abs/1503.02531) - [x] [Factor Transfer]
+(https://arxiv.org/abs/1802.04977) - [x] [Attention Transfer](https://
+arxiv.org/abs/1612.03928)    Pruning  - [x] [Chipnet](https://arxiv.org/abs/
+2102.07156) - [x] [Network slimming](https://arxiv.org/abs/1708.06519) - [x]
+[Growth Regularization](https://arxiv.org/abs/2012.09243)    Quantization - [x]
+[BitSplit](https://dl.acm.org/doi/abs/10.5555/3524938.3525851) - [x] [BRECQ]
+(https://arxiv.org/abs/2102.05426) - [x] [LAPQ](https://arxiv.org/abs/
+1911.07190)    Binarization - [x] [BiRealNet](https://arxiv.org/abs/1808.00278)
+- [x] [ReActNet](https://arxiv.org/abs/2003.03488) - [x] [BNN-BN](https://
+arxiv.org/abs/2104.08215v1)  # Acknowledgement # Citation If you find this
+project useful in your research, please consider cite: ```BibTeX @misc{, title=
+{}, author={}, howpublished = {}}, year={2023} } ``` # License This project is
+released under the [MIT license](LICENSE). Keywords: computer vision,image
+classification,model efficiency Platform: UNKNOWN Classifier: Development
+Status :: 4 - Beta Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: OS Independent Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: all
```

### Comparing `trailmet-0.0.1rc2/README.md` & `trailmet-0.0.1rc3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,20 @@
         <img src="docs/source/imgs/trailmet.png" width="500"/>
     </br>
     <br>
         <strong> Transmute AI Model Efficiency Toolkit </strong>
     </br>
 </p>
 <p align="center">
+    <a href="https://pypi.org/project/trailmet/">
+    <img src="https://pepy.tech/badge/trailmet" />
+    </a>
+    <a href="https://pypi.org/project/trailmet/">
+    <img src="https://badge.fury.io/py/trailmet.svg" />
+    </a>
     <a href="https://github.com/transmuteAI/trailmet/blob/dev/LICENSE">
         <img alt="GitHub" src="https://img.shields.io/github/license/transmuteAI/trailmet?color=blue">
     </a>
     <a href="https://transmuteai-trailmet.readthedocs.io/en/latest/">
         <img alt="Documentation" src="https://img.shields.io/badge/docs-passing-brightgreen">
     </a>
     <a href="https://github.com/transmuteAI/trailmet/actions/workflows/ci.yml">
@@ -44,15 +50,15 @@
 
 ```shell
 git clone https://github.com/transmuteAI/trailmet.git
 cd trailmet
 conda create -n trailmet
 conda activate trailmet
 conda install pytorch=1.13 torchvision=0.14 pytorch-cuda=11.7 -c pytorch -c nvidia
-pip install -r requirements.txt
+pip install trailmet
 ```
 
 # Algorithms Implemented
 
 Demo notebooks for each algorithm is added in [experiments](https://github.com/transmuteAI/trailmet/blob/dev/experiments) folder
 
 <details open>
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
 
                        [docs/source/imgs/trailmet.png]
                     Transmute AI Model Efficiency Toolkit
+  [https://pepy.tech/badge/trailmet] [https://badge.fury.io/py/trailmet.svg]
 [GitHub] [Documentation] [Run_tests_with_pytest] [GitHub_Stars] [GitHub_Forks]
 # Introduction Trailmet is a model efficiency toolkit for compressing deep
 learning models using state of the art compression techniques. Today deep
 learning models are not deployable because of their huge memory footprint,
 TRAILMET is an effort to make deep learning models more efficient in their size
 to performance ratio. It is developed using Pytorch 1.13. ### Major features -
 State of the art compression algorithms implemented. - Demo notebooks for
 training each algorithm. - Modular Design: All alogithms are modular and can
 customized easily for any kind of model and dataset. # Installation Below are
 quick steps for installation: ```shell git clone https://github.com/
 transmuteAI/trailmet.git cd trailmet conda create -n trailmet conda activate
 trailmet conda install pytorch=1.13 torchvision=0.14 pytorch-cuda=11.7 -
-c pytorch -c nvidia pip install -r requirements.txt ``` # Algorithms
-Implemented Demo notebooks for each algorithm is added in [experiments](https:/
-/github.com/transmuteAI/trailmet/blob/dev/experiments) folder   Knowledge
-Distillation - [x] [Response KD](https://arxiv.org/abs/1503.02531) - [x]
-[Factor Transfer](https://arxiv.org/abs/1802.04977) - [x] [Attention Transfer]
-(https://arxiv.org/abs/1612.03928)    Pruning  - [x] [Chipnet](https://
-arxiv.org/abs/2102.07156) - [x] [Network slimming](https://arxiv.org/abs/
-1708.06519) - [x] [Growth Regularization](https://arxiv.org/abs/2012.09243)
-Quantization - [x] [BitSplit](https://dl.acm.org/doi/abs/10.5555/
-3524938.3525851) - [x] [BRECQ](https://arxiv.org/abs/2102.05426) - [x] [LAPQ]
-(https://arxiv.org/abs/1911.07190)    Binarization - [x] [BiRealNet](https://
-arxiv.org/abs/1808.00278) - [x] [ReActNet](https://arxiv.org/abs/2003.03488) -
-[x] [BNN-BN](https://arxiv.org/abs/2104.08215v1)  # Acknowledgement # Citation
-If you find this project useful in your research, please consider cite:
-```BibTeX @misc{, title={}, author={}, howpublished = {}}, year={2023} } ``` #
-License This project is released under the [MIT license](LICENSE).
+c pytorch -c nvidia pip install trailmet ``` # Algorithms Implemented Demo
+notebooks for each algorithm is added in [experiments](https://github.com/
+transmuteAI/trailmet/blob/dev/experiments) folder   Knowledge Distillation -
+[x] [Response KD](https://arxiv.org/abs/1503.02531) - [x] [Factor Transfer]
+(https://arxiv.org/abs/1802.04977) - [x] [Attention Transfer](https://
+arxiv.org/abs/1612.03928)    Pruning  - [x] [Chipnet](https://arxiv.org/abs/
+2102.07156) - [x] [Network slimming](https://arxiv.org/abs/1708.06519) - [x]
+[Growth Regularization](https://arxiv.org/abs/2012.09243)    Quantization - [x]
+[BitSplit](https://dl.acm.org/doi/abs/10.5555/3524938.3525851) - [x] [BRECQ]
+(https://arxiv.org/abs/2102.05426) - [x] [LAPQ](https://arxiv.org/abs/
+1911.07190)    Binarization - [x] [BiRealNet](https://arxiv.org/abs/1808.00278)
+- [x] [ReActNet](https://arxiv.org/abs/2003.03488) - [x] [BNN-BN](https://
+arxiv.org/abs/2104.08215v1)  # Acknowledgement # Citation If you find this
+project useful in your research, please consider cite: ```BibTeX @misc{, title=
+{}, author={}, howpublished = {}}, year={2023} } ``` # License This project is
+released under the [MIT license](LICENSE).
```

### Comparing `trailmet-0.0.1rc2/setup.py` & `trailmet-0.0.1rc3/setup.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/__init__.py` & `trailmet-0.0.1rc3/trailmet/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/__init__.py` & `trailmet-0.0.1rc3/trailmet/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/algorithms.py` & `trailmet-0.0.1rc3/trailmet/algorithms/algorithms.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/binarize/BNNBN.py` & `trailmet-0.0.1rc3/trailmet/algorithms/binarize/BNNBN.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/binarize/ReActNet.py` & `trailmet-0.0.1rc3/trailmet/algorithms/binarize/ReActNet.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/binarize/__init__.py` & `trailmet-0.0.1rc3/trailmet/algorithms/binarize/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/binarize/binarize.py` & `trailmet-0.0.1rc3/trailmet/algorithms/binarize/binarize.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/binarize/birealnet.py` & `trailmet-0.0.1rc3/trailmet/algorithms/binarize/birealnet.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/binarize/utils.py` & `trailmet-0.0.1rc3/trailmet/algorithms/binarize/utils.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/distill/__init__.py` & `trailmet-0.0.1rc3/trailmet/algorithms/distill/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/distill/attention_transfer.py` & `trailmet-0.0.1rc3/trailmet/algorithms/distill/attention_transfer.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/distill/distill.py` & `trailmet-0.0.1rc3/trailmet/algorithms/distill/distill.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/distill/factor_transfer.py` & `trailmet-0.0.1rc3/trailmet/algorithms/distill/factor_transfer.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/distill/losses.py` & `trailmet-0.0.1rc3/trailmet/algorithms/distill/losses.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/distill/response_kd.py` & `trailmet-0.0.1rc3/trailmet/algorithms/distill/response_kd.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/distill/rkd.py` & `trailmet-0.0.1rc3/trailmet/algorithms/distill/rkd.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/prune/__init__.py` & `trailmet-0.0.1rc3/trailmet/algorithms/prune/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/prune/chip.py` & `trailmet-0.0.1rc3/trailmet/algorithms/prune/chip.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/prune/chipnet.py` & `trailmet-0.0.1rc3/trailmet/algorithms/prune/chipnet.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/prune/growth_regularisation.py` & `trailmet-0.0.1rc3/trailmet/algorithms/prune/growth_regularisation.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/prune/network_slimming.py` & `trailmet-0.0.1rc3/trailmet/algorithms/prune/network_slimming.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/prune/pns.py` & `trailmet-0.0.1rc3/trailmet/algorithms/prune/pns.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/prune/prune.py` & `trailmet-0.0.1rc3/trailmet/algorithms/prune/prune.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/__init__.py` & `trailmet-0.0.1rc3/trailmet/algorithms/prune/pruner/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/l1_pruner.py` & `trailmet-0.0.1rc3/trailmet/algorithms/prune/pruner/l1_pruner.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/meta_pruner.py` & `trailmet-0.0.1rc3/trailmet/algorithms/prune/pruner/meta_pruner.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/prune/pruner/reg_pruner.py` & `trailmet-0.0.1rc3/trailmet/algorithms/prune/pruner/reg_pruner.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/prune/utils.py` & `trailmet-0.0.1rc3/trailmet/algorithms/prune/utils.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/quantize/__init__.py` & `trailmet-0.0.1rc3/trailmet/algorithms/quantize/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/quantize/bitsplit.py` & `trailmet-0.0.1rc3/trailmet/algorithms/quantize/bitsplit.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/quantize/brecq.py` & `trailmet-0.0.1rc3/trailmet/algorithms/quantize/brecq.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/quantize/lapq.py` & `trailmet-0.0.1rc3/trailmet/algorithms/quantize/lapq.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/quantize/methods.py` & `trailmet-0.0.1rc3/trailmet/algorithms/quantize/methods.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/quantize/qmodel.py` & `trailmet-0.0.1rc3/trailmet/algorithms/quantize/qmodel.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/quantize/quantize.py` & `trailmet-0.0.1rc3/trailmet/algorithms/quantize/quantize.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/quantize/reconstruct.py` & `trailmet-0.0.1rc3/trailmet/algorithms/quantize/reconstruct.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/algorithms/utils/__init__.py` & `trailmet-0.0.1rc3/trailmet/algorithms/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/datasets/__init__.py` & `trailmet-0.0.1rc3/trailmet/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/datasets/classification/__init__.py` & `trailmet-0.0.1rc3/trailmet/datasets/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/datasets/classification/chest.py` & `trailmet-0.0.1rc3/trailmet/datasets/classification/chest.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/datasets/classification/cifar.py` & `trailmet-0.0.1rc3/trailmet/datasets/classification/cifar.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/datasets/classification/dataset.py` & `trailmet-0.0.1rc3/trailmet/datasets/classification/dataset.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/datasets/classification/imagenet.py` & `trailmet-0.0.1rc3/trailmet/datasets/classification/imagenet.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/datasets/classification/tcga.py` & `trailmet-0.0.1rc3/trailmet/datasets/classification/tcga.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,31 +119,37 @@
         if self._mode == 'train':
             path = self.Train_List[idx]
             image_path = os.path.join(self.data_path, self.labels_dict[path],
                                       path + '.png')
             img = Image.open(image_path).convert('RGB')
             img = self.transform(img)
             class_name = self.labels_dict[path]
-            return img, torch.tensor([self.class_dict[class_name]])
+            return img, torch.tensor([self.class_dict[class_name]]).item()
         elif self._mode == 'val':
             path = self.Val_List[idx]
             image_path = os.path.join(self.data_path, self.labels_dict[path],
                                       path + '.png')
             img = Image.open(image_path).convert('RGB')
-            img = self.target_transform(img)
+            if self.target_transform == None:
+                img = self.transform(img)
+            else:
+                img = self.target_transform(img)
             class_name = self.labels_dict[path]
-            return img, torch.tensor([self.class_dict[class_name]])
+            return img, torch.tensor([self.class_dict[class_name]]).item()
         else:
             path = self.Test_List[idx]
             image_path = os.path.join(self.data_path, self.labels_dict[path],
                                       path + '.png')
             img = Image.open(image_path).convert('RGB')
-            img = self.target_transform(img)
+            if self.target_transform == None:
+                img = self.transform(img)
+            else:
+                img = self.target_transform(img)
             class_name = self.labels_dict[path]
-            return img, torch.tensor([self.class_dict[class_name]])
+            return img, torch.tensor([self.class_dict[class_name]]).item()
 
 
 class TCGADataset(BaseDataset):
     """
     `TCGA <https://www.cancer.gov/ccg/research/structural-genomics/tcga/studied-cancers/lung-squamous-cell-carcinoma-study>`_ Dataset.
 
     References
```

### Comparing `trailmet-0.0.1rc2/trailmet/models/__init__.py` & `trailmet-0.0.1rc3/trailmet/models/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/models/base_model.py` & `trailmet-0.0.1rc3/trailmet/models/base_model.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/models/mobilenet.py` & `trailmet-0.0.1rc3/trailmet/models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/models/mobilenetv2_bireal.py` & `trailmet-0.0.1rc3/trailmet/models/mobilenetv2_bireal.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/models/resnet.py` & `trailmet-0.0.1rc3/trailmet/models/resnet.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/models/resnet_bireal.py` & `trailmet-0.0.1rc3/trailmet/models/resnet_bireal.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/models/resnet_chip.py` & `trailmet-0.0.1rc3/trailmet/models/resnet_chip.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/models/wideresnet.py` & `trailmet-0.0.1rc3/trailmet/models/wideresnet.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/utils/__init__.py` & `trailmet-0.0.1rc3/trailmet/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/utils/benchmark.py` & `trailmet-0.0.1rc3/trailmet/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/utils/functions.py` & `trailmet-0.0.1rc3/trailmet/utils/functions.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/utils/tp_pruning.py` & `trailmet-0.0.1rc3/trailmet/utils/tp_pruning.py`

 * *Files identical despite different names*

### Comparing `trailmet-0.0.1rc2/trailmet/version.py` & `trailmet-0.0.1rc3/trailmet/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-__version__ = '0.0.1rc2'
+__version__ = '0.0.1rc3'
 
 
 def parse_version_info(version_str):
     """Parse a version string into a tuple.
 
     Args:
         version_str (str): The version string.
```

### Comparing `trailmet-0.0.1rc2/trailmet.egg-info/PKG-INFO` & `trailmet-0.0.1rc3/trailmet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: trailmet
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: Transmute AI Model Efficiency Toolkit
 Home-page: https://github.com/transmuteAI/trailmet
 Author: TrAILMET Contributors
 Author-email: transmute.ai@gmail.com
 License: MIT License
 Description: <p align="center">
             <br>
                 <img src="docs/source/imgs/trailmet.png" width="500"/>
             </br>
             <br>
                 <strong> Transmute AI Model Efficiency Toolkit </strong>
             </br>
         </p>
         <p align="center">
+            <a href="https://pypi.org/project/trailmet/">
+            <img src="https://pepy.tech/badge/trailmet" />
+            </a>
+            <a href="https://pypi.org/project/trailmet/">
+            <img src="https://badge.fury.io/py/trailmet.svg" />
+            </a>
             <a href="https://github.com/transmuteAI/trailmet/blob/dev/LICENSE">
                 <img alt="GitHub" src="https://img.shields.io/github/license/transmuteAI/trailmet?color=blue">
             </a>
             <a href="https://transmuteai-trailmet.readthedocs.io/en/latest/">
                 <img alt="Documentation" src="https://img.shields.io/badge/docs-passing-brightgreen">
             </a>
             <a href="https://github.com/transmuteAI/trailmet/actions/workflows/ci.yml">
@@ -52,15 +58,15 @@
         
         ```shell
         git clone https://github.com/transmuteAI/trailmet.git
         cd trailmet
         conda create -n trailmet
         conda activate trailmet
         conda install pytorch=1.13 torchvision=0.14 pytorch-cuda=11.7 -c pytorch -c nvidia
-        pip install -r requirements.txt
+        pip install trailmet
         ```
         
         # Algorithms Implemented
         
         Demo notebooks for each algorithm is added in [experiments](https://github.com/transmuteAI/trailmet/blob/dev/experiments) folder
         
         <details open>
```

#### html2text {}

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1 Name: trailmet Version: 0.0.1rc2 Summary: Transmute AI
+Metadata-Version: 2.1 Name: trailmet Version: 0.0.1rc3 Summary: Transmute AI
 Model Efficiency Toolkit Home-page: https://github.com/transmuteAI/trailmet
 Author: TrAILMET Contributors Author-email: transmute.ai@gmail.com License: MIT
 License Description:
 
                        [docs/source/imgs/trailmet.png]
                     Transmute AI Model Efficiency Toolkit
+  [https://pepy.tech/badge/trailmet] [https://badge.fury.io/py/trailmet.svg]
 [GitHub] [Documentation] [Run_tests_with_pytest] [GitHub_Stars] [GitHub_Forks]
 # Introduction Trailmet is a model efficiency toolkit for compressing deep
 learning models using state of the art compression techniques. Today deep
 learning models are not deployable because of their huge memory footprint,
 TRAILMET is an effort to make deep learning models more efficient in their size
 to performance ratio. It is developed using Pytorch 1.13. ### Major features -
 State of the art compression algorithms implemented. - Demo notebooks for
 training each algorithm. - Modular Design: All alogithms are modular and can
 customized easily for any kind of model and dataset. # Installation Below are
 quick steps for installation: ```shell git clone https://github.com/
 transmuteAI/trailmet.git cd trailmet conda create -n trailmet conda activate
 trailmet conda install pytorch=1.13 torchvision=0.14 pytorch-cuda=11.7 -
-c pytorch -c nvidia pip install -r requirements.txt ``` # Algorithms
-Implemented Demo notebooks for each algorithm is added in [experiments](https:/
-/github.com/transmuteAI/trailmet/blob/dev/experiments) folder   Knowledge
-Distillation - [x] [Response KD](https://arxiv.org/abs/1503.02531) - [x]
-[Factor Transfer](https://arxiv.org/abs/1802.04977) - [x] [Attention Transfer]
-(https://arxiv.org/abs/1612.03928)    Pruning  - [x] [Chipnet](https://
-arxiv.org/abs/2102.07156) - [x] [Network slimming](https://arxiv.org/abs/
-1708.06519) - [x] [Growth Regularization](https://arxiv.org/abs/2012.09243)
-Quantization - [x] [BitSplit](https://dl.acm.org/doi/abs/10.5555/
-3524938.3525851) - [x] [BRECQ](https://arxiv.org/abs/2102.05426) - [x] [LAPQ]
-(https://arxiv.org/abs/1911.07190)    Binarization - [x] [BiRealNet](https://
-arxiv.org/abs/1808.00278) - [x] [ReActNet](https://arxiv.org/abs/2003.03488) -
-[x] [BNN-BN](https://arxiv.org/abs/2104.08215v1)  # Acknowledgement # Citation
-If you find this project useful in your research, please consider cite:
-```BibTeX @misc{, title={}, author={}, howpublished = {}}, year={2023} } ``` #
-License This project is released under the [MIT license](LICENSE). Keywords:
-computer vision,image classification,model efficiency Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-all
+c pytorch -c nvidia pip install trailmet ``` # Algorithms Implemented Demo
+notebooks for each algorithm is added in [experiments](https://github.com/
+transmuteAI/trailmet/blob/dev/experiments) folder   Knowledge Distillation -
+[x] [Response KD](https://arxiv.org/abs/1503.02531) - [x] [Factor Transfer]
+(https://arxiv.org/abs/1802.04977) - [x] [Attention Transfer](https://
+arxiv.org/abs/1612.03928)    Pruning  - [x] [Chipnet](https://arxiv.org/abs/
+2102.07156) - [x] [Network slimming](https://arxiv.org/abs/1708.06519) - [x]
+[Growth Regularization](https://arxiv.org/abs/2012.09243)    Quantization - [x]
+[BitSplit](https://dl.acm.org/doi/abs/10.5555/3524938.3525851) - [x] [BRECQ]
+(https://arxiv.org/abs/2102.05426) - [x] [LAPQ](https://arxiv.org/abs/
+1911.07190)    Binarization - [x] [BiRealNet](https://arxiv.org/abs/1808.00278)
+- [x] [ReActNet](https://arxiv.org/abs/2003.03488) - [x] [BNN-BN](https://
+arxiv.org/abs/2104.08215v1)  # Acknowledgement # Citation If you find this
+project useful in your research, please consider cite: ```BibTeX @misc{, title=
+{}, author={}, howpublished = {}}, year={2023} } ``` # License This project is
+released under the [MIT license](LICENSE). Keywords: computer vision,image
+classification,model efficiency Platform: UNKNOWN Classifier: Development
+Status :: 4 - Beta Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: OS Independent Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: all
```

