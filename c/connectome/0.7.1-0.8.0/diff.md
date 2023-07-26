# Comparing `tmp/connectome-0.7.1.tar.gz` & `tmp/connectome-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome-0.7.1.tar", last modified: Wed Jul  5 00:34:50 2023, max compression
+gzip compressed data, was "connectome-0.8.0.tar", last modified: Wed Jul 26 07:50:17 2023, max compression
```

## Comparing `connectome-0.7.1.tar` & `connectome-0.8.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.977531 connectome-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-05 00:34:47.000000 connectome-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-05 00:34:47.000000 connectome-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-07-05 00:34:50.977531 connectome-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-05 00:34:47.000000 connectome-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.973531 connectome-0.7.1/connectome/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.973531 connectome-0.7.1/connectome/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/cache/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/cache/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.973531 connectome-0.7.1/connectome/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/containers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/containers/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/containers/reversible.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.973531 connectome-0.7.1/connectome/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/node_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/engine/vm.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.977531 connectome-0.7.1/connectome/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/complex_edges.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)    17982 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/factory_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/metaclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/split.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/interface/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.977531 connectome-0.7.1/connectome/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/layers/split.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-07-05 00:34:47.000000 connectome-0.7.1/connectome/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:34:50.973531 connectome-0.7.1/connectome.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-07-05 00:34:50.000000 connectome-0.7.1/connectome.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-05 00:34:50.000000 connectome-0.7.1/connectome.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:34:50.000000 connectome-0.7.1/connectome.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 00:34:50.000000 connectome-0.7.1/connectome.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 00:34:50.000000 connectome-0.7.1/connectome.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-05 00:34:47.000000 connectome-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 00:34:47.000000 connectome-0.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 00:34:50.977531 connectome-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-05 00:34:47.000000 connectome-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:50:17.381461 connectome-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-07-26 07:50:07.000000 connectome-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-26 07:50:07.000000 connectome-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-07-26 07:50:17.381461 connectome-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-26 07:50:07.000000 connectome-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:50:17.377461 connectome-0.8.0/connectome/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:50:17.377461 connectome-0.8.0/connectome/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/cache/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/cache/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:50:17.377461 connectome-0.8.0/connectome/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/containers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/containers/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/containers/reversible.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:50:17.377461 connectome-0.8.0/connectome/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/engine/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/engine/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/engine/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/engine/node_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/engine/vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:50:17.381461 connectome-0.8.0/connectome/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/interface/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/interface/complex_edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/interface/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/interface/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17982 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/interface/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/interface/factory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/interface/metaclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/interface/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/interface/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/interface/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:50:17.381461 connectome-0.8.0/connectome/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/layers/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/layers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/layers/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/layers/check_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/layers/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/layers/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/layers/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/layers/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/layers/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/layers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/layers/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/layers/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-07-26 07:50:07.000000 connectome-0.8.0/connectome/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:50:17.377461 connectome-0.8.0/connectome.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-07-26 07:50:17.000000 connectome-0.8.0/connectome.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-26 07:50:17.000000 connectome-0.8.0/connectome.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 07:50:17.000000 connectome-0.8.0/connectome.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-26 07:50:17.000000 connectome-0.8.0/connectome.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 07:50:17.000000 connectome-0.8.0/connectome.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-26 07:50:07.000000 connectome-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-26 07:50:07.000000 connectome-0.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 07:50:17.381461 connectome-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-26 07:50:07.000000 connectome-0.8.0/setup.py
```

### Comparing `connectome-0.7.1/LICENSE` & `connectome-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/PKG-INFO` & `connectome-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: connectome
-Version: 0.7.1
+Version: 0.8.0
 Summary: A library for datasets containing heterogeneous data
 Home-page: https://github.com/neuro-ml/connectome
-Download-URL: https://github.com/neuro-ml/connectome/archive/v0.7.1.tar.gz
+Download-URL: https://github.com/neuro-ml/connectome/archive/v0.8.0.tar.gz
 Author: NeuroML Group
 Author-email: NeuroML Group <max@ira-labs.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `connectome-0.7.1/README.md` & `connectome-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/cache/base.py` & `connectome-0.8.0/connectome/cache/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/cache/disk.py` & `connectome-0.8.0/connectome/cache/disk.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/cache/memory.py` & `connectome-0.8.0/connectome/cache/memory.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/containers/base.py` & `connectome-0.8.0/connectome/containers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 
         self.inputs, self.outputs, self.edges, self.virtual = normalize_bag(
             inputs, outputs, edges, virtual, optional, persistent)
 
         self.persistent: NameSet = persistent
         self.optional: NodeSet = optional
         self.context = context
-        self.backend = None
 
     def freeze(self, parent: Union[Details, None] = None) -> 'EdgesBag':
         """
         Creates a copy of the nodes and edges.
         If `parent` is not None, increases the nesting of the layers hierarchy by assigning
         `parent` to top layers and nodes
         """
@@ -89,15 +88,15 @@
             edges, context,
             virtual=self.virtual, persistent=self.persistent,
             optional=set(update_map(self.optional, node_map, parent, layers_map)),
         )
 
     def compile(self) -> GraphCompiler:
         return GraphCompiler(
-            self.inputs, self.outputs, self.edges, self.virtual, self.optional, self.backend
+            self.inputs, self.outputs, self.edges, self.virtual, self.optional
         )
 
     def loopback(self, func: Callable, inputs: StringsLike, output: StringsLike) -> 'EdgesBag':
         state = connect_bags(self, function_to_bag(func, inputs, output))
         outputs, new_edges, new_optionals = state.context.reverse(state.outputs)
         return EdgesBag(
             state.inputs, outputs, list(state.edges) + list(new_edges), None,
```

### Comparing `connectome-0.7.1/connectome/containers/context.py` & `connectome-0.8.0/connectome/containers/context.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/containers/reversible.py` & `connectome-0.8.0/connectome/containers/reversible.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/engine/base.py` & `connectome-0.8.0/connectome/engine/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     'Edge', 'Node', 'Nodes', 'NodeSet', 'BoundEdge', 'BoundEdges', 'TreeNode', 'TreeNodes', 'Details',
     'EvalGen', 'HashGen',
 )
 
 
 class Command(Enum):
     ParentHash, CurrentHash, ParentValue, Payload, Await, Call = range(6)
-    Send, Store, Item, ComputeHash, Evaluate, AwaitFuture, Tuple, Return = range(-8, 0)
+    Send, Store, Item, ComputeHash, Evaluate, Tuple, Return = range(-7, 0)
 
 
 HashOutput = Tuple[NodeHash, Any]
 Request = Tuple  # [RequestType, Any, ...]
 Response = Union[NodeHash, Any, Tuple[NodeHash, Any]]
 HashGen = Generator[Request, Response, HashOutput]
 EvalGen = Generator[Request, Response, Any]
```

### Comparing `connectome-0.7.1/connectome/engine/compiler.py` & `connectome-0.8.0/connectome/engine/compiler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-from concurrent.futures import Executor
 from typing import Tuple, Union
 
 from ..exceptions import DependencyError, FieldError
 from ..utils import NameSet, check_for_duplicates
 from .base import BoundEdges, Nodes, TreeNode, TreeNodes
 from .edges import ProductEdge
 from .graph import Graph
 
 
 class GraphCompiler:
-    def __init__(self, inputs: Nodes, outputs: Nodes, edges: BoundEdges, virtuals: NameSet, optionals: Nodes,
-                 executor: Executor):
+    def __init__(self, inputs: Nodes, outputs: Nodes, edges: BoundEdges, virtuals: NameSet, optionals: Nodes):
         check_for_duplicates(inputs)
         check_for_duplicates(outputs)
         self._mapping = TreeNode.from_edges(edges)
         # TODO: optimize:
         #  - remove identity edges
 
         self._edges = edges
         self._inputs = {self._mapping[x] for x in inputs}
         # TODO: make sure the inputs are leaves
         self._all_outputs = {x.name: self._mapping[x] for x in outputs}
         # some optional nodes might be unreachable
         self._optionals = {self._mapping[x] for x in optionals if x in self._mapping}
         self._virtuals = virtuals
-        self._executor = executor
 
         self._cache = {}
         self._dependencies = self._outputs = None
 
     def fields(self):
         if self._outputs is None:
             self._validate_optionals()
@@ -67,27 +64,27 @@
 
         if isinstance(item, str):
             node = get_node(item)
             if node is None:
                 # TODO: signature
                 return identity
 
-            return Graph(self._inputs, node, self._executor)
+            return Graph(self._inputs, node)
 
         inputs, outputs = [], []
         for name in item:
             node = get_node(name)
             if node is None:
                 node = TreeNode(name, None, None)
                 inputs.append(node)
 
             outputs.append(node)
 
         product = TreeNode(f'({", ".join(item)})', (ProductEdge(len(item)), outputs), None)
-        return Graph(self._inputs | set(inputs), product, self._executor)
+        return Graph(self._inputs | set(inputs), product)
 
     def __getitem__(self, item):
         # TODO: deprecate
         return self.compile(item)
 
     def _validate_optionals(self):
         self._dependencies = find_dependencies(self._all_outputs.values())
```

### Comparing `connectome-0.7.1/connectome/engine/edges.py` & `connectome-0.8.0/connectome/engine/edges.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/engine/graph.py` & `connectome-0.8.0/connectome/engine/graph.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 import inspect
 from collections import defaultdict
-from concurrent.futures import Executor
 from typing import Any, Sequence
 
 from .base import Command, TreeNode, TreeNodes
-from .executor import DefaultExecutor
 from .node_hash import GraphHash, LeafHash, NodeHash
 from .utils import EvictionCache
 from .vm import execute
 
 
 class Graph:
-    def __init__(self, inputs: TreeNodes, output: TreeNode, executor: Executor = None):
+    def __init__(self, inputs: TreeNodes, output: TreeNode):
         validate_graph(inputs, output)
         # TODO: need a cumulative eviction policy
         counts = count_entries(inputs, output, multiplier=2)
         inputs = sorted([x for x in inputs if counts.get(x, 0)], key=lambda x: x.name)
         signature = inspect.Signature([
             inspect.Parameter(x.name, inspect.Parameter.POSITIONAL_OR_KEYWORD)
             for x in inputs
         ])
         self.inputs = inputs
         self.output = output
         self.counts = counts
-        self.executor = DefaultExecutor if executor is None else executor
         self.__signature__ = signature
         # TODO: deprecate
         self.call = self.__call__
 
     def __call__(*args, **kwargs):
         self, *args = args
         scope = self.__signature__.bind(*args, **kwargs)
         hashes, cache = self._prepare_cache(scope.arguments)
-        return evaluate(self.output, hashes, cache, self.executor)
+        return evaluate(self.output, hashes, cache)
 
     def __str__(self):
         inputs = ', '.join(x.name for x in self.inputs)
         if len(self.inputs) != 1:
             inputs = f'({inputs})'
         return f'Graph({inputs} -> {self.output.name})'
 
@@ -50,30 +47,30 @@
         return hashes, cache
 
     def get_hash(self, *inputs: Any):
         assert len(inputs) == len(self.inputs)
         assert all(not isinstance(v, NodeHash) for v in inputs)
 
         hashes, cache = self._prepare_cache({n.name: v for n, v in zip(self.inputs, inputs)})
-        result, _ = compute_hash(self.output, hashes, cache, self.executor)
+        result, _ = compute_hash(self.output, hashes, cache)
         return result, (hashes, cache)
 
     def get_value(self, hashes, cache) -> Any:
-        return evaluate(self.output, hashes, cache, self.executor)
+        return evaluate(self.output, hashes, cache)
 
     def hash(self) -> GraphHash:
         return GraphHash(hash_graph(self.inputs, self.output))
 
 
-def evaluate(node: TreeNode, hashes: EvictionCache, cache: EvictionCache, executor: Executor):
-    return execute(Command.Evaluate, node, hashes, cache, executor)
+def evaluate(node: TreeNode, hashes: EvictionCache, cache: EvictionCache):
+    return execute(Command.Evaluate, node, hashes, cache)
 
 
-def compute_hash(node: TreeNode, hashes: EvictionCache, cache: EvictionCache, executor: Executor):
-    return execute(Command.ComputeHash, node, hashes, cache, executor)
+def compute_hash(node: TreeNode, hashes: EvictionCache, cache: EvictionCache):
+    return execute(Command.ComputeHash, node, hashes, cache)
 
 
 def validate_graph(inputs: TreeNodes, output: TreeNode):
     def visitor(node):
         # input doesn't need parents
         if node in inputs:
             return
```

### Comparing `connectome-0.7.1/connectome/engine/node_hash.py` & `connectome-0.8.0/connectome/engine/node_hash.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/engine/utils.py` & `connectome-0.8.0/connectome/engine/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/interface/complex_edges.py` & `connectome-0.8.0/connectome/interface/complex_edges.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/interface/edges.py` & `connectome-0.8.0/connectome/interface/edges.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/interface/factory.py` & `connectome-0.8.0/connectome/interface/factory.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/interface/metaclasses.py` & `connectome-0.8.0/connectome/interface/metaclasses.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/interface/nodes.py` & `connectome-0.8.0/connectome/interface/nodes.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/interface/split.py` & `connectome-0.8.0/connectome/interface/split.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/interface/utils.py` & `connectome-0.8.0/connectome/interface/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/layers/apply.py` & `connectome-0.8.0/connectome/layers/apply.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/layers/base.py` & `connectome-0.8.0/connectome/layers/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/layers/cache.py` & `connectome-0.8.0/connectome/layers/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import weakref
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Container as ContainerType, Sequence, Union
 
 import numpy as np
+import yaml
+
 from tarn import DiskDict, HashKeyStorage, PickleKeyStorage
 from tarn.config import StorageConfig, init_storage
 from tarn.interface import MaybeLabels
 
 from ..cache import Cache, DiskCache, MemoryCache
 from ..containers import EdgesBag, IdentityContext
 from ..engine import CacheEdge, Details, ImpureEdge, Node, TreeNode
@@ -154,14 +156,24 @@
         if serializer is None:
             serializer = ChainSerializer(
                 JsonSerializer(),
                 NumpySerializer({np.bool_: 1, np.int_: 1}),
                 PickleSerializer(),
             )
 
+        # TODO: this is a bit of a legacy cleanup
+        for c in index, storage:
+            c = c / 'config.yml'
+            with open(c) as file:
+                config = yaml.safe_load(file)
+            if 'version' in config:
+                config.pop('version')
+                with open(c, 'w') as file:
+                    yaml.safe_dump(config, file)
+
         return cls(index, HashKeyStorage(DiskDict(storage)), serializer, names, labels=labels)
 
 
 def _normalize_disk_arguments(names, serializer):
     return to_seq(names), _resolve_serializer(serializer)
```

### Comparing `connectome-0.7.1/connectome/layers/columns.py` & `connectome-0.8.0/connectome/layers/columns.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/layers/debug.py` & `connectome-0.8.0/connectome/layers/debug.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/layers/filter.py` & `connectome-0.8.0/connectome/layers/filter.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/layers/group.py` & `connectome-0.8.0/connectome/layers/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from collections import defaultdict
 
 from typing import Callable, Union, Sequence, Any
 
-from .chain import connect
-from .dynamic import DynamicConnectLayer
-from .join import to_hash_id
+
+from ..cache import MemoryCache
 from ..containers import EdgesBag
 from ..engine import (
-    Details, Node, FunctionEdge, StaticGraph, StaticHash, Graph, NodeHashes, NodeHash, CustomHash, StaticEdge
+    Details, Node, FunctionEdge, StaticGraph, StaticHash, Graph, NodeHashes, NodeHash, CustomHash, StaticEdge, CacheEdge
 )
 from ..engine import EvalGen, Command
 from ..utils import node_to_dict, extract_signature
+from .chain import connect
+from .dynamic import DynamicConnectLayer
+from .join import to_hash_id
 
 
 class GroupBy(DynamicConnectLayer):
     def __init__(self, by: Union[str, Sequence[str], Callable]):
         self.by = by
 
     def _by_layer(self, details):
@@ -47,19 +49,21 @@
         changed_input = Node(key_name, details)
         mapping_node = Node('$mapping', details)
         output_nodes = node_to_dict(main.outputs)
         assert keys_name in output_nodes
         keys = output_nodes[keys_name]
         outputs.append(changed_input)
 
-        # create a mapping: {new_id: [old_ids]}
+        # create a mapping: {new_id: [old_ids]} and store it in memory
         by_layer = self._by_layer(details)
+        raw_mapping = Node('$mapping', details)
         edges.append(GroupMapping(
             connect(main, by_layer).compile().compile('$by')
-        ).bind([keys], mapping_node))
+        ).bind(keys, raw_mapping))
+        edges.append(CacheEdge(MemoryCache(None)).bind(raw_mapping, mapping_node))
 
         compiler = main.compile()
         # evaluate each output
         for node in main.outputs:
             if node.name in [keys_name, key_name]:
                 continue
```

### Comparing `connectome-0.7.1/connectome/layers/join.py` & `connectome-0.8.0/connectome/layers/join.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/layers/merge.py` & `connectome-0.8.0/connectome/layers/merge.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/layers/split.py` & `connectome-0.8.0/connectome/layers/split.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome/utils.py` & `connectome-0.8.0/connectome/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/connectome.egg-info/PKG-INFO` & `connectome-0.8.0/connectome.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: connectome
-Version: 0.7.1
+Version: 0.8.0
 Summary: A library for datasets containing heterogeneous data
 Home-page: https://github.com/neuro-ml/connectome
-Download-URL: https://github.com/neuro-ml/connectome/archive/v0.7.1.tar.gz
+Download-URL: https://github.com/neuro-ml/connectome/archive/v0.8.0.tar.gz
 Author: NeuroML Group
 Author-email: NeuroML Group <max@ira-labs.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `connectome-0.7.1/connectome.egg-info/SOURCES.txt` & `connectome-0.8.0/connectome.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 connectome/containers/base.py
 connectome/containers/context.py
 connectome/containers/reversible.py
 connectome/engine/__init__.py
 connectome/engine/base.py
 connectome/engine/compiler.py
 connectome/engine/edges.py
-connectome/engine/executor.py
 connectome/engine/graph.py
 connectome/engine/node_hash.py
 connectome/engine/utils.py
 connectome/engine/vm.py
 connectome/interface/__init__.py
 connectome/interface/blocks.py
 connectome/interface/complex_edges.py
@@ -43,14 +42,15 @@
 connectome/interface/split.py
 connectome/interface/utils.py
 connectome/layers/__init__.py
 connectome/layers/apply.py
 connectome/layers/base.py
 connectome/layers/cache.py
 connectome/layers/chain.py
+connectome/layers/check_ids.py
 connectome/layers/columns.py
 connectome/layers/debug.py
 connectome/layers/dynamic.py
 connectome/layers/filter.py
 connectome/layers/group.py
 connectome/layers/join.py
 connectome/layers/merge.py
```

### Comparing `connectome-0.7.1/pyproject.toml` & `connectome-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `connectome-0.7.1/setup.py` & `connectome-0.8.0/setup.py`

 * *Files identical despite different names*

