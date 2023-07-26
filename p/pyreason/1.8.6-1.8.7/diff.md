# Comparing `tmp/pyreason-1.8.6.tar.gz` & `tmp/pyreason-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.8.6.tar", last modified: Tue Jul 25 16:41:38 2023, max compression
+gzip compressed data, was "pyreason-1.8.7.tar", last modified: Wed Jul 26 05:48:44 2023, max compression
```

## Comparing `pyreason-1.8.6.tar` & `pyreason-1.8.7.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.474181 pyreason-1.8.6/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-07-25 16:41:16.000000 pyreason-1.8.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 16:41:16.000000 pyreason-1.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-25 16:41:38.474181 pyreason-1.8.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-07-25 16:41:16.000000 pyreason-1.8.6/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.466181 pyreason-1.8.6/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.466181 pyreason-1.8.6/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.470181 pyreason-1.8.6/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    31359 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.470181 pyreason-1.8.6/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.470181 pyreason-1.8.6/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.470181 pyreason-1.8.6/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.470181 pyreason-1.8.6/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/facts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/facts/fact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.470181 pyreason-1.8.6/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    76966 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/interpretation/interpretation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.470181 pyreason-1.8.6/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.470181 pyreason-1.8.6/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.470181 pyreason-1.8.6/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10414 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.470181 pyreason-1.8.6/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2404 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.470181 pyreason-1.8.6/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.474181 pyreason-1.8.6/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4551 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/utils/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/utils/rule_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8756 2023-07-25 16:41:16.000000 pyreason-1.8.6/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.466181 pyreason-1.8.6/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-25 16:41:38.000000 pyreason-1.8.6/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-25 16:41:38.000000 pyreason-1.8.6/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:41:38.000000 pyreason-1.8.6/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 16:41:38.000000 pyreason-1.8.6/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 16:41:38.000000 pyreason-1.8.6/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 16:41:38.474181 pyreason-1.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-25 16:41:16.000000 pyreason-1.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:41:38.474181 pyreason-1.8.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-25 16:41:16.000000 pyreason-1.8.6/tests/test_hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.011128 pyreason-1.8.7/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-07-26 05:48:32.000000 pyreason-1.8.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-26 05:48:32.000000 pyreason-1.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-26 05:48:44.011128 pyreason-1.8.7/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-07-26 05:48:32.000000 pyreason-1.8.7/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31359 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/facts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/facts/fact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    77016 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/interpretation/interpretation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.011128 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10414 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.011128 pyreason-1.8.7/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.011128 pyreason-1.8.7/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.011128 pyreason-1.8.7/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4551 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/rule_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8756 2023-07-26 05:48:32.000000 pyreason-1.8.7/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.007128 pyreason-1.8.7/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-26 05:48:43.000000 pyreason-1.8.7/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-26 05:48:44.000000 pyreason-1.8.7/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 05:48:43.000000 pyreason-1.8.7/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 05:48:43.000000 pyreason-1.8.7/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 05:48:43.000000 pyreason-1.8.7/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 05:48:44.011128 pyreason-1.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-26 05:48:32.000000 pyreason-1.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:48:44.011128 pyreason-1.8.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-26 05:48:32.000000 pyreason-1.8.7/tests/test_hello_world.py
```

### Comparing `pyreason-1.8.6/LICENSE.md` & `pyreason-1.8.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/PKG-INFO` & `pyreason-1.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.8.6
+Version: 1.8.7
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.8.6/README.md` & `pyreason-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/__init__.py` & `pyreason-1.8.7/pyreason/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.8.7/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.8.7/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.8.7/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/pyreason.py` & `pyreason-1.8.7/pyreason/pyreason.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.8.7/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/args.py` & `pyreason-1.8.7/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/components/world.py` & `pyreason-1.8.7/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/diffuse.py` & `pyreason-1.8.7/pyreason/scripts/diffuse.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/facts/fact.py` & `pyreason-1.8.7/pyreason/scripts/facts/fact.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.8.7/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/facts/fact_node.py` & `pyreason-1.8.7/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.8.7/pyreason/scripts/interpretation/interpretation.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,19 +167,19 @@
 			convergence_mode = 'delta_interpretation'
 			convergence_delta = convergence_threshold
 		else:
 			convergence_mode = 'delta_bound'
 			convergence_delta = convergence_bound_threshold
 		return convergence_mode, convergence_delta
 
-	def start_fp(self, tmax, facts_node, facts_edge, rules, verbose, convergence_threshold, convergence_bound_threshold):
+	def start_fp(self, tmax, facts_node, facts_edge, rules, verbose, convergence_threshold, convergence_bound_threshold, again=False):
 		self.tmax = tmax
 		self._convergence_mode, self._convergence_delta = self._init_convergence(convergence_bound_threshold, convergence_threshold)
 		max_facts_time = self._init_facts(facts_node, facts_edge, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.atom_trace)
-		self._start_fp(rules, max_facts_time, verbose)
+		self._start_fp(rules, max_facts_time, verbose, again)
 
 	@staticmethod
 	@numba.njit(cache=CACHEING)
 	def _init_facts(facts_node, facts_edge, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, atom_trace):
 		max_time = 0
 		for fact in facts_node:
 			for t in range(fact.get_time_lower(), fact.get_time_upper() + 1):
@@ -195,26 +195,26 @@
 				name = fact.get_name()
 				graph_attribute = True if name=='graph-attribute-fact' else False
 				facts_to_be_applied_edge.append((numba.types.uint16(t), fact.get_component(), fact.get_label(), fact.get_bound(), fact.static, graph_attribute))
 				if atom_trace:
 					facts_to_be_applied_edge_trace.append(fact.get_name())
 		return max_time
 
-	def _start_fp(self, rules, max_facts_time, verbose):
-		fp_cnt, t = self.reason(self.interpretations_node, self.interpretations_edge, self.tmax, self.prev_reasoning_data, rules, self.nodes, self.edges, self.neighbors, self.reverse_neighbors, self.rules_to_be_applied_node, self.rules_to_be_applied_edge, self.edges_to_be_added_node_rule, self.edges_to_be_added_edge_rule, self.rules_to_be_applied_node_trace, self.rules_to_be_applied_edge_trace, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.ipl, self.rule_trace_node, self.rule_trace_edge, self.rule_trace_node_atoms, self.rule_trace_edge_atoms, self.reverse_graph, self.atom_trace, self.save_graph_attributes_to_rule_trace, self.canonical, self.inconsistency_check, self.store_interpretation_changes, max_facts_time, self.annotation_functions, self._convergence_mode, self._convergence_delta, verbose)
+	def _start_fp(self, rules, max_facts_time, verbose, again):
+		fp_cnt, t = self.reason(self.interpretations_node, self.interpretations_edge, self.tmax, self.prev_reasoning_data, rules, self.nodes, self.edges, self.neighbors, self.reverse_neighbors, self.rules_to_be_applied_node, self.rules_to_be_applied_edge, self.edges_to_be_added_node_rule, self.edges_to_be_added_edge_rule, self.rules_to_be_applied_node_trace, self.rules_to_be_applied_edge_trace, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.ipl, self.rule_trace_node, self.rule_trace_edge, self.rule_trace_node_atoms, self.rule_trace_edge_atoms, self.reverse_graph, self.atom_trace, self.save_graph_attributes_to_rule_trace, self.canonical, self.inconsistency_check, self.store_interpretation_changes, max_facts_time, self.annotation_functions, self._convergence_mode, self._convergence_delta, verbose, again)
 		self.time = t - 1
 		# If we need to reason again, store the next timestep to start from
 		self.prev_reasoning_data[0] = t
 		self.prev_reasoning_data[1] = fp_cnt
 		if verbose:
 			print('Fixed Point iterations:', fp_cnt)
 
 	@staticmethod
 	@numba.njit(cache=CACHEING)
-	def reason(interpretations_node, interpretations_edge, tmax, prev_reasoning_data, rules, nodes, edges, neighbors, reverse_neighbors, rules_to_be_applied_node, rules_to_be_applied_edge, edges_to_be_added_node_rule, edges_to_be_added_edge_rule, rules_to_be_applied_node_trace, rules_to_be_applied_edge_trace, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, ipl, rule_trace_node, rule_trace_edge, rule_trace_node_atoms, rule_trace_edge_atoms, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes, max_facts_time, annotation_functions, convergence_mode, convergence_delta, verbose):
+	def reason(interpretations_node, interpretations_edge, tmax, prev_reasoning_data, rules, nodes, edges, neighbors, reverse_neighbors, rules_to_be_applied_node, rules_to_be_applied_edge, edges_to_be_added_node_rule, edges_to_be_added_edge_rule, rules_to_be_applied_node_trace, rules_to_be_applied_edge_trace, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, ipl, rule_trace_node, rule_trace_edge, rule_trace_node_atoms, rule_trace_edge_atoms, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, store_interpretation_changes, max_facts_time, annotation_functions, convergence_mode, convergence_delta, verbose, again):
 		t = prev_reasoning_data[0]
 		fp_cnt = prev_reasoning_data[1]
 		max_rules_time = 0
 		timestep_loop = True
 		facts_to_be_applied_node_new = numba.typed.List.empty_list(facts_to_be_applied_node_type)
 		facts_to_be_applied_edge_new = numba.typed.List.empty_list(facts_to_be_applied_edge_type)
 		rules_to_remove_idx = numba.typed.List.empty_list(numba.types.int64)
@@ -569,15 +569,15 @@
 						rule = rules[i]
 						immediate_rule = rule.is_immediate_rule()
 						immediate_node_rule_fire = False
 						immediate_edge_rule_fire = False
 
 						# Only go through if the rule can be applied within the given timesteps, or we're running until convergence
 						delta_t = rule.get_delta()
-						if t + delta_t <= tmax or tmax == -1:
+						if t + delta_t <= tmax or tmax == -1 or again:
 							applicable_node_rules = _ground_node_rule(rule, interpretations_node, interpretations_edge, nodes, neighbors, reverse_neighbors, atom_trace, reverse_graph, nodes_to_skip[i])
 							applicable_edge_rules = _ground_edge_rule(rule, interpretations_node, interpretations_edge, nodes, edges, neighbors, reverse_neighbors, atom_trace, reverse_graph, edges_to_skip[i])
 
 							# Loop through applicable rules and add them to the rules to be applied for later or next fp operation
 							for applicable_rule in applicable_node_rules:
 								n, annotations, qualified_nodes, qualified_edges, edges_to_add = applicable_rule
 								# If there is an edge to add or the predicate doesn't exist or the interpretation is not static
```

### Comparing `pyreason-1.8.6/pyreason/scripts/interval/interval.py` & `pyreason-1.8.7/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.8.7/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/program/program.py` & `pyreason-1.8.7/pyreason/scripts/program/program.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,11 +40,10 @@
 		self.interp.start_fp(self._tmax, self._facts_node, self._facts_edge, self._rules, verbose, convergence_threshold, convergence_bound_threshold)
 
 		return self.interp
 	
 	def reason_again(self, tmax, convergence_threshold, convergence_bound_threshold, facts_node, facts_edge, verbose=True):
 		assert self.interp is not None, 'Call reason before calling reason again'
 		self._tmax = self.interp.time + tmax
-		self.interp.start_fp(self._tmax, facts_node, facts_edge, self._rules, verbose, convergence_threshold, convergence_bound_threshold)
+		self.interp.start_fp(self._tmax, facts_node, facts_edge, self._rules, verbose, convergence_threshold, convergence_bound_threshold, again=True)
 
 		return self.interp
-
```

### Comparing `pyreason-1.8.6/pyreason/scripts/rules/rule.py` & `pyreason-1.8.7/pyreason/scripts/rules/rule.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/utils/filter.py` & `pyreason-1.8.7/pyreason/scripts/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.8.7/pyreason/scripts/utils/graphml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/utils/output.py` & `pyreason-1.8.7/pyreason/scripts/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/utils/plotter.py` & `pyreason-1.8.7/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/utils/rule_parser.py` & `pyreason-1.8.7/pyreason/scripts/utils/rule_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/utils/visuals.py` & `pyreason-1.8.7/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.8.7/pyreason/scripts/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/pyreason.egg-info/PKG-INFO` & `pyreason-1.8.7/pyreason.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.8.6
+Version: 1.8.7
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.8.6/pyreason.egg-info/SOURCES.txt` & `pyreason-1.8.7/pyreason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.6/setup.py` & `pyreason-1.8.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pyreason',
-    version='1.8.6',
+    version='1.8.7',
     author='Dyuman Aditya',
     author_email='dyuman.aditya@gmail.com',
     description='An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/lab-v2/pyreason',
     license='BSD 3-clause',
```

### Comparing `pyreason-1.8.6/tests/test_hello_world.py` & `pyreason-1.8.7/tests/test_hello_world.py`

 * *Files identical despite different names*

