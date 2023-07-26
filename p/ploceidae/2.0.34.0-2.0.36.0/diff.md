# Comparing `tmp/ploceidae-2.0.34.0.tar.gz` & `tmp/ploceidae-2.0.36.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploceidae-2.0.34.0.tar", last modified: Sun Mar  5 22:20:34 2023, max compression
+gzip compressed data, was "ploceidae-2.0.36.0.tar", last modified: Wed Jul 26 20:17:56 2023, max compression
```

## Comparing `ploceidae-2.0.34.0.tar` & `ploceidae-2.0.36.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:34.023395 ploceidae-2.0.34.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-05 22:20:34.023395 ploceidae-2.0.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:34.019395 ploceidae-2.0.34.0/ploceidae/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:34.019395 ploceidae-2.0.34.0/ploceidae/constants/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/constants/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:34.019395 ploceidae-2.0.34.0/ploceidae/container/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/container/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/container/partial_injection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:34.019395 ploceidae-2.0.34.0/ploceidae/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:34.019395 ploceidae-2.0.34.0/ploceidae/core/configurators/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/core/configurators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/core/configurators/basic_configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:34.019395 ploceidae-2.0.34.0/ploceidae/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency/dependency_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency/dependency_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency/dependency_wrapper_helper_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:34.019395 ploceidae-2.0.34.0/ploceidae/dependency/garbage_collection/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency/garbage_collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency/garbage_collection/garbage_collection_observer.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency/garbage_collection/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:34.019395 ploceidae-2.0.34.0/ploceidae/dependency_lifetime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency_lifetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency_lifetime/dependency_lifetime_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency_lifetime/dependency_lifetime_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:34.019395 ploceidae-2.0.34.0/ploceidae/dependency_management/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency_management/cache_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency_management/dependency_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency_management/dependency_graph_cycle_check_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency_management/dependency_graph_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency_management/dependency_resolution_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/dependency_management/resolved_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:34.023395 ploceidae-2.0.34.0/ploceidae/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/unit_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/unit_tests/test_configurators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17475 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/unit_tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/unit_tests/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/unit_tests/test_dependency_graph_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/unit_tests/test_dependency_grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/unit_tests/test_dependency_lifetime_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/unit_tests/test_dependency_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/unit_tests/test_garbage_collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:34.023395 ploceidae-2.0.34.0/ploceidae/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/utilities/dependency_visibility_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/utilities/logging_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/utilities/module_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/utilities/module_name_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/utilities/reduce_operand.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/ploceidae/utilities/singleton_implementer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:20:34.019395 ploceidae-2.0.34.0/ploceidae.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-05 22:20:33.000000 ploceidae-2.0.34.0/ploceidae.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-03-05 22:20:33.000000 ploceidae-2.0.34.0/ploceidae.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 22:20:33.000000 ploceidae-2.0.34.0/ploceidae.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 22:20:33.000000 ploceidae-2.0.34.0/ploceidae.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-05 22:20:33.000000 ploceidae-2.0.34.0/ploceidae.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-05 22:20:33.000000 ploceidae-2.0.34.0/ploceidae.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-05 22:20:34.023395 ploceidae-2.0.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-05 22:20:25.000000 ploceidae-2.0.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:56.098531 ploceidae-2.0.36.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-26 20:17:56.098531 ploceidae-2.0.36.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:56.086531 ploceidae-2.0.36.0/ploceidae/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:56.090531 ploceidae-2.0.36.0/ploceidae/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/constants/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:56.090531 ploceidae-2.0.36.0/ploceidae/container/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/container/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/container/partial_injection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:56.090531 ploceidae-2.0.36.0/ploceidae/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:56.090531 ploceidae-2.0.36.0/ploceidae/core/configurators/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/core/configurators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/core/configurators/basic_configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:56.090531 ploceidae-2.0.36.0/ploceidae/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency/dependency_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency/dependency_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency/dependency_wrapper_helper_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:56.090531 ploceidae-2.0.36.0/ploceidae/dependency/garbage_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency/garbage_collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency/garbage_collection/garbage_collection_observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency/garbage_collection/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:56.094531 ploceidae-2.0.36.0/ploceidae/dependency_lifetime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency_lifetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency_lifetime/dependency_lifetime_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency_lifetime/dependency_lifetime_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:56.094531 ploceidae-2.0.36.0/ploceidae/dependency_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency_management/cache_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency_management/dependency_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency_management/dependency_graph_cycle_check_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency_management/dependency_graph_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency_management/dependency_resolution_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/dependency_management/resolved_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:56.098531 ploceidae-2.0.36.0/ploceidae/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/unit_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/unit_tests/test_configurators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17475 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/unit_tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/unit_tests/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/unit_tests/test_dependency_graph_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/unit_tests/test_dependency_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/unit_tests/test_dependency_lifetime_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/unit_tests/test_dependency_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/unit_tests/test_garbage_collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:56.098531 ploceidae-2.0.36.0/ploceidae/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/utilities/dependency_visibility_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/utilities/logging_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/utilities/module_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/utilities/module_name_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/utilities/reduce_operand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/ploceidae/utilities/singleton_implementer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:17:56.086531 ploceidae-2.0.36.0/ploceidae.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-26 20:17:56.000000 ploceidae-2.0.36.0/ploceidae.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-26 20:17:56.000000 ploceidae-2.0.36.0/ploceidae.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:17:56.000000 ploceidae-2.0.36.0/ploceidae.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:17:56.000000 ploceidae-2.0.36.0/ploceidae.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 20:17:56.000000 ploceidae-2.0.36.0/ploceidae.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 20:17:56.000000 ploceidae-2.0.36.0/ploceidae.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-26 20:17:56.098531 ploceidae-2.0.36.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-26 20:17:48.000000 ploceidae-2.0.36.0/setup.py
```

### Comparing `ploceidae-2.0.34.0/LICENSE` & `ploceidae-2.0.36.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/PKG-INFO` & `ploceidae-2.0.36.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploceidae
-Version: 2.0.34.0
+Version: 2.0.36.0
 Summary: dependency injection library
 Home-page: https://github.com/MATTHEWFRAZER/ploceidae
 Author: Matthew Frazer
 Author-email: mfrazeriguess@gmail.com
 License: MIT
 Keywords: dependency injection DI
 Platform: UNKNOWN
```

### Comparing `ploceidae-2.0.34.0/README.md` & `ploceidae-2.0.36.0/README.md`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/container/container.py` & `ploceidae-2.0.36.0/ploceidae/container/container.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/container/partial_injection.py` & `ploceidae-2.0.36.0/ploceidae/container/partial_injection.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/core/configurators/basic_configurator.py` & `ploceidae-2.0.36.0/ploceidae/core/configurators/basic_configurator.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/dependency/dependency_locator.py` & `ploceidae-2.0.36.0/ploceidae/dependency/dependency_locator.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/dependency/dependency_wrapper.py` & `ploceidae-2.0.36.0/ploceidae/dependency/dependency_wrapper.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/dependency/dependency_wrapper_helper_methods.py` & `ploceidae-2.0.36.0/ploceidae/dependency/dependency_wrapper_helper_methods.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/dependency/garbage_collection/garbage_collection_observer.py` & `ploceidae-2.0.36.0/ploceidae/dependency/garbage_collection/garbage_collection_observer.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/dependency/garbage_collection/scheduler.py` & `ploceidae-2.0.36.0/ploceidae/dependency/garbage_collection/scheduler.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/dependency_lifetime/dependency_lifetime_key.py` & `ploceidae-2.0.36.0/ploceidae/dependency_lifetime/dependency_lifetime_key.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/dependency_management/cache_item.py` & `ploceidae-2.0.36.0/ploceidae/dependency_management/cache_item.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/dependency_management/dependency_graph.py` & `ploceidae-2.0.36.0/ploceidae/dependency_management/dependency_graph.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/dependency_management/dependency_graph_cycle_check_methods.py` & `ploceidae-2.0.36.0/ploceidae/dependency_management/dependency_graph_cycle_check_methods.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/dependency_management/dependency_graph_manager.py` & `ploceidae-2.0.36.0/ploceidae/dependency_management/dependency_graph_manager.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/dependency_management/dependency_resolution_methods.py` & `ploceidae-2.0.36.0/ploceidae/dependency_management/dependency_resolution_methods.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/unit_tests/conftest.py` & `ploceidae-2.0.36.0/ploceidae/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/unit_tests/test_container.py` & `ploceidae-2.0.36.0/ploceidae/unit_tests/test_container.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/unit_tests/test_dependency.py` & `ploceidae-2.0.36.0/ploceidae/unit_tests/test_dependency.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/unit_tests/test_dependency_graph_manager.py` & `ploceidae-2.0.36.0/ploceidae/unit_tests/test_dependency_graph_manager.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/unit_tests/test_dependency_grouping.py` & `ploceidae-2.0.36.0/ploceidae/unit_tests/test_dependency_grouping.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/unit_tests/test_dependency_lifetime_management.py` & `ploceidae-2.0.36.0/ploceidae/unit_tests/test_dependency_lifetime_management.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/unit_tests/test_dependency_location.py` & `ploceidae-2.0.36.0/ploceidae/unit_tests/test_dependency_location.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/unit_tests/test_garbage_collection.py` & `ploceidae-2.0.36.0/ploceidae/unit_tests/test_garbage_collection.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/utilities/logging_utilities.py` & `ploceidae-2.0.36.0/ploceidae/utilities/logging_utilities.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/utilities/module_caches.py` & `ploceidae-2.0.36.0/ploceidae/utilities/module_caches.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae/utilities/singleton_implementer.py` & `ploceidae-2.0.36.0/ploceidae/utilities/singleton_implementer.py`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/ploceidae.egg-info/PKG-INFO` & `ploceidae-2.0.36.0/ploceidae.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploceidae
-Version: 2.0.34.0
+Version: 2.0.36.0
 Summary: dependency injection library
 Home-page: https://github.com/MATTHEWFRAZER/ploceidae
 Author: Matthew Frazer
 Author-email: mfrazeriguess@gmail.com
 License: MIT
 Keywords: dependency injection DI
 Platform: UNKNOWN
```

### Comparing `ploceidae-2.0.34.0/ploceidae.egg-info/SOURCES.txt` & `ploceidae-2.0.36.0/ploceidae.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ploceidae-2.0.34.0/setup.py` & `ploceidae-2.0.36.0/setup.py`

 * *Files identical despite different names*

