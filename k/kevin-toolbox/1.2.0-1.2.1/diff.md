# Comparing `tmp/kevin-toolbox-1.2.0.tar.gz` & `tmp/kevin-toolbox-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kevin-toolbox-1.2.0.tar", last modified: Wed Jul 26 08:49:45 2023, max compression
+gzip compressed data, was "dist/kevin-toolbox-1.2.1.tar", last modified: Wed Jul 26 13:48:37 2023, max compression
```

## Comparing `kevin-toolbox-1.2.0.tar` & `kevin-toolbox-1.2.1.tar`

### file list

```diff
@@ -1,339 +1,344 @@
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1752 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/PKG-INFO
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1165 2023-07-26 08:45:30.000000 kevin-toolbox-1.2.0/README.md
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       23 2023-07-26 08:47:54.000000 kevin-toolbox-1.2.0/kevin_toolbox/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-12-01 13:56:40.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-04 15:12:36.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      142 2023-03-05 16:13:01.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1832 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1914 2023-06-12 05:50:08.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2078 2023-06-12 05:50:08.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2819 2023-03-05 16:40:22.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/for_dict/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       37 2023-06-12 05:50:08.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/for_dict/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      666 2023-06-19 08:36:11.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/for_seq/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-06-12 05:50:08.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/for_seq/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1046 2023-06-12 05:50:08.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      309 2023-06-12 05:50:08.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/for_seq/get_subsets.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/locks/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-04-21 13:18:26.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/locks/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2492 2023-04-24 08:04:07.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/pareto_front/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       57 2023-04-10 08:46:01.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/pareto_front/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2712 2023-04-10 09:09:27.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/registration/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2023-06-12 14:36:27.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/registration/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    13842 2023-07-26 06:36:11.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/registration/registry.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/scheduler/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-06-02 12:00:07.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/scheduler/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    12194 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4470 2023-07-25 12:43:34.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/scheduler/trigger.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/search/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       41 2023-03-20 13:18:25.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/search/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1013 2023-03-04 15:58:55.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/search/binary_search.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/statistician/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      120 2023-06-01 10:31:40.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/statistician/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      904 2023-06-01 10:26:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/statistician/_init_var.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3101 2023-06-01 10:35:42.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5571 2023-06-01 10:29:44.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/utils/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-08 14:31:25.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/utils/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/data_structure/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       31 2023-03-22 06:30:28.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/data_structure/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6206 2023-06-21 01:55:31.000000 kevin-toolbox-1.2.0/kevin_toolbox/computer_science/data_structure/executor.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/dangerous/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       93 2023-03-29 12:29:14.000000 kevin-toolbox-1.2.0/kevin_toolbox/dangerous/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2898 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 12:43:00.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/core/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 09:06:12.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/core/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/core/cache/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       79 2022-02-08 11:12:52.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/core/cache/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16060 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/core/reader/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      146 2022-02-09 09:12:47.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/core/reader/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8827 2022-04-26 13:12:04.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2423 2023-07-25 10:34:14.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/core/reader/unified_reader.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    11929 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/core/reader/unified_reader_base.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-07-25 12:56:33.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       85 2022-07-25 12:54:00.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/converter/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      369 2023-07-22 16:01:59.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/converter/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      559 2022-07-25 12:26:23.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      391 2023-05-22 11:15:00.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/converter/convert_ndarray_to_list.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      809 2023-07-22 15:47:27.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/converter/escape_non_str_dict_key.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      605 2023-07-22 16:02:29.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/converter/escape_tuple.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      377 2023-05-22 11:15:00.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/converter/integrate.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      808 2023-07-22 16:14:24.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/converter/unescape_non_str_dict_key.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      661 2023-07-22 16:14:24.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/converter/unescape_tuple.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1753 2023-07-25 12:37:51.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/read_json.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2355 2023-07-25 12:37:51.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/write_json.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2023-02-08 07:16:46.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3621 2022-11-16 07:31:34.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/converter.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8071 2023-06-21 01:55:22.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16285 2023-06-21 00:22:15.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      447 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/read.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/test/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-08-01 07:19:40.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      324 2022-08-01 07:19:40.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_0.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      249 2022-08-01 07:22:27.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6838 2023-06-21 00:15:01.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      556 2023-06-21 00:11:28.000000 kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/write.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-08 10:14:56.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/decorator/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       66 2022-02-08 10:15:24.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/decorator/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      399 2022-02-08 06:57:21.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/decorator/restore_original_work_path.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       20 2022-04-18 08:15:52.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/producer_consumer/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       28 2022-04-18 08:15:52.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/producer_consumer/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      892 2022-12-12 08:39:00.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3164 2022-04-18 08:15:52.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       50 2022-04-18 11:35:30.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/producer_consumer/getter.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      740 2022-04-18 12:49:09.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2299 2022-04-18 12:23:06.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/producer_consumer/node.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-04-18 08:15:52.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/producer_consumer/producer.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       51 2022-04-18 10:40:32.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/producer_consumer/sender.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/singleton/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-04-18 13:24:36.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/singleton/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3803 2023-06-12 12:14:03.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2089 2022-02-28 06:54:56.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/general_matrix_multiplication.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/numerical_characteristics/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-02 05:01:47.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/numerical_characteristics/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2953 2022-06-02 05:03:41.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/numerical_characteristics/iou.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/temperate/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      630 2022-03-13 18:22:06.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/temperate/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      213 2022-03-10 05:06:13.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/temperate/iterator_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1663 2022-03-13 18:22:06.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/temperate/my_iterator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1214 2022-03-10 05:06:13.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/temperate/my_iterator_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      217 2022-03-10 05:06:13.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/temperate/sequence_map_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      241 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/developing/test.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/env_info/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-30 13:18:27.000000 kevin-toolbox-1.2.0/kevin_toolbox/env_info/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      879 2023-04-10 12:53:17.000000 kevin-toolbox-1.2.0/kevin_toolbox/env_info/check_validity_and_uninstall.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1953 2023-06-21 01:55:26.000000 kevin-toolbox-1.2.0/kevin_toolbox/env_info/check_version_and_update.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/env_info/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-30 12:51:50.000000 kevin-toolbox-1.2.0/kevin_toolbox/env_info/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1728 2023-04-13 07:53:17.000000 kevin-toolbox-1.2.0/kevin_toolbox/env_info/test/test_version.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/env_info/version/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      187 2023-03-30 13:11:22.000000 kevin-toolbox-1.2.0/kevin_toolbox/env_info/version/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2489 2023-04-13 07:51:40.000000 kevin-toolbox-1.2.0/kevin_toolbox/env_info/version/compare_version.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      860 2023-04-13 07:46:23.000000 kevin-toolbox-1.2.0/kevin_toolbox/env_info/version/parse_version.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2458 2023-03-30 13:11:22.000000 kevin-toolbox-1.2.0/kevin_toolbox/env_info/version/sort_version_ls.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-05 07:35:48.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      650 2023-03-24 10:03:29.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/__old_version/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-24 10:03:09.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/__old_version/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2564 2023-03-24 09:28:54.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5701 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      305 2023-03-24 09:34:05.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/cal_area_of_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3079 2023-05-16 14:16:04.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8249 2022-08-01 13:19:11.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      836 2022-08-01 11:47:43.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/detect_collision.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2762 2022-07-06 13:18:05.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8255 2023-05-16 11:51:25.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8634 2023-06-21 01:55:28.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/detect_overlap.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      292 2022-07-05 08:41:47.000000 kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/get_ticks_of_boxes.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-28 06:47:25.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-10 07:21:33.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-14 08:37:13.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/analysis/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2022-09-28 09:26:13.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/analysis/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4714 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/dummy/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       54 2022-02-28 08:44:35.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/dummy/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7137 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2022-09-26 09:52:59.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      896 2022-03-13 18:22:06.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1858 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    17766 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/factory.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      299 2022-03-13 18:22:06.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4480 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3482 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4799 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5480 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      224 2022-03-13 18:22:06.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3114 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3773 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      170 2022-03-10 12:36:00.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/merge.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 04:21:21.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/binary_classification/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      427 2022-02-22 06:22:25.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/binary_classification/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-21 13:29:08.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3247 2022-02-22 06:22:25.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5319 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3355 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      891 2022-04-28 12:02:07.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      442 2022-02-22 05:39:00.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/convert.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3661 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-27 07:16:21.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-03 13:07:44.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/concat_and_split/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      157 2022-08-08 08:06:40.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/concat_and_split/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    23861 2023-06-14 03:08:32.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4997 2022-08-08 08:19:17.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3066 2022-08-08 08:19:17.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      232 2023-03-13 06:47:47.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/convert/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       43 2023-03-13 06:47:47.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/convert/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4972 2023-03-10 14:11:22.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/generate/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      264 2023-03-13 06:47:47.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/generate/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3380 2023-03-13 06:48:36.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5738 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4426 2022-07-29 07:53:01.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1373 2023-03-10 13:56:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/reshape/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      220 2022-07-25 13:28:44.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/reshape/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1946 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1064 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/reshape/merge_blocks.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1236 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/reshape/split_blocks.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1859 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/transpose/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      177 2022-05-31 10:43:01.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/transpose/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      611 2022-08-09 13:17:49.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1472 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/number_theory/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      182 2023-03-05 15:57:35.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/number_theory/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      244 2023-03-05 15:45:13.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/number_theory/cache.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      387 2023-03-05 15:57:35.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/number_theory/get_greatest_common_divisor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      949 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/number_theory/get_primes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      499 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/number_theory/prime_factorization.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/number_theory/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-06 07:12:06.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/number_theory/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      747 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      784 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/number_theory/test/test_get_primes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      551 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/number_theory/test/test_prime_factorization.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/transform/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-10 08:52:28.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/transform/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/transform/dct/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      147 2022-07-22 13:25:44.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/transform/dct/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8296 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/transform/dct/dct_calculator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4305 2022-07-20 12:21:16.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/transform/scaling_and_shift/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       29 2022-07-30 13:19:40.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/transform/scaling_and_shift/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1280 2022-07-30 13:48:26.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/transform/scaling_and_shift/scaling.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/utils/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      289 2023-04-21 12:36:14.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/utils/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1943 2022-08-09 12:09:28.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/utils/convert_dtype.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1620 2022-08-08 08:50:02.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/utils/get_crop_by_box.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1553 2022-08-02 12:15:03.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1775 2022-08-08 08:50:02.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/utils/set_crop_by_box.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      345 2023-05-30 12:44:28.000000 kevin-toolbox-1.2.0/kevin_toolbox/math/utils/spilt_integer_most_evenly.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      241 2023-07-26 06:34:50.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      908 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/copy_.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      614 2023-07-25 12:37:51.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/count_leaf_node_nums.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1286 2023-06-21 01:55:54.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/get_hash.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3457 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/get_nodes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2083 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/get_value.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/name_handler/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      107 2023-06-20 10:05:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/name_handler/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1020 2023-07-26 07:45:46.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/name_handler/build_name.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1163 2023-06-20 09:49:43.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/name_handler/escape_node.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2311 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/name_handler/parse_name.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       48 2023-07-26 08:00:49.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-07-20 06:49:05.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1819 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_json_.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1470 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_bin.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1384 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_npy.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1282 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_pickle_.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      853 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_skip_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      937 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_skip_simple.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1282 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_torch_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1353 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_torch_tensor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1741 2023-07-20 07:15:24.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/backend_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2540 2023-07-26 06:34:50.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/read.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      393 2023-07-26 06:34:50.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/variable.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    14862 2023-07-26 08:31:07.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/write.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2781 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/set_value.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6943 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/traverse.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/value_parser/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      169 2023-06-21 03:27:20.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/value_parser/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3119 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/value_parser/cal_relation_between_references.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2301 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/value_parser/eval_references.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2116 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/value_parser/parse_references.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-29 13:28:32.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_matplotlib/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      127 2023-03-10 08:30:36.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_matplotlib/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1837 2023-03-10 10:16:48.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1696 2023-03-10 09:17:25.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1361 2023-03-10 08:13:57.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_matplotlib/arrow3d.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_numpy/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-24 08:38:24.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_numpy/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_numpy/linalg/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       99 2023-04-24 08:58:58.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_numpy/linalg/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      423 2023-05-17 07:05:16.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_numpy/linalg/cos_similar.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      625 2023-04-24 08:52:01.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_numpy/linalg/normalize.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      253 2023-04-24 08:55:02.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_numpy/linalg/softmax.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_optuna/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2023-05-26 09:14:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_optuna/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4580 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_os/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       77 2023-07-21 09:36:08.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_os/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      656 2023-07-21 09:38:57.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_os/pack.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      658 2023-04-17 12:51:37.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_os/remove.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1047 2023-07-21 09:40:06.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_os/unpack.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-07-29 06:55:38.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3184 2023-06-26 08:43:44.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_test/check_consistency.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 06:56:01.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       75 2023-03-08 07:01:29.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      393 2023-04-12 15:31:18.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/concat.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/linalg/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       44 2023-03-08 08:04:27.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/linalg/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      770 2023-04-12 15:31:18.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      575 2023-04-12 15:31:18.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/nn/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-05-30 11:36:55.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/nn/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5357 2023-04-12 15:31:18.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      845 2023-04-12 15:31:18.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/tile.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-04-12 15:36:21.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/where.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/math/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       68 2022-02-21 09:51:39.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/math/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2047 2022-02-22 06:43:43.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/math/get_y_at_x.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1378 2022-02-21 09:44:44.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/math/my_around.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/nn/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-05-30 11:37:07.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/nn/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      223 2023-05-29 08:32:26.000000 kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/nn/lambda_layer.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox.egg-info/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1752 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    15112 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       92 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox.egg-info/requires.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       14 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/kevin_toolbox.egg-info/top_level.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       59 2023-03-31 06:32:36.000000 kevin-toolbox-1.2.0/pyproject.toml
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      904 2023-07-26 08:49:45.000000 kevin-toolbox-1.2.0/setup.cfg
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-03-31 07:25:47.000000 kevin-toolbox-1.2.0/setup.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1563 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/PKG-INFO
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      972 2023-07-26 13:46:10.000000 kevin-toolbox-1.2.1/README.md
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       23 2023-07-26 13:48:08.000000 kevin-toolbox-1.2.1/kevin_toolbox/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-12-01 13:56:40.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-04 15:12:36.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      142 2023-03-05 16:13:01.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1832 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1914 2023-06-12 05:50:08.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2078 2023-06-12 05:50:08.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2819 2023-03-05 16:40:22.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/for_dict/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       37 2023-06-12 05:50:08.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/for_dict/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      666 2023-06-19 08:36:11.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/for_seq/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-06-12 05:50:08.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/for_seq/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1046 2023-06-12 05:50:08.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      309 2023-06-12 05:50:08.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/for_seq/get_subsets.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/locks/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-04-21 13:18:26.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/locks/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2492 2023-04-24 08:04:07.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/pareto_front/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       57 2023-04-10 08:46:01.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/pareto_front/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2712 2023-04-10 09:09:27.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/registration/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2023-06-12 14:36:27.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/registration/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    13842 2023-07-26 06:36:11.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/registration/registry.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/scheduler/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-06-02 12:00:07.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/scheduler/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    12194 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4470 2023-07-25 12:43:34.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/scheduler/trigger.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/search/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       41 2023-03-20 13:18:25.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/search/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1013 2023-03-04 15:58:55.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/search/binary_search.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/statistician/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      120 2023-06-01 10:31:40.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/statistician/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      904 2023-06-01 10:26:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/statistician/_init_var.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3101 2023-06-01 10:35:42.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5571 2023-06-01 10:29:44.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/utils/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-08 14:31:25.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/utils/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/data_structure/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       31 2023-03-22 06:30:28.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/data_structure/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6206 2023-06-21 01:55:31.000000 kevin-toolbox-1.2.1/kevin_toolbox/computer_science/data_structure/executor.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/dangerous/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       93 2023-03-29 12:29:14.000000 kevin-toolbox-1.2.1/kevin_toolbox/dangerous/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2898 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 12:43:00.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/core/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 09:06:12.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/core/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/core/cache/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       79 2022-02-08 11:12:52.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/core/cache/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16060 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/core/reader/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      146 2022-02-09 09:12:47.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/core/reader/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8827 2022-04-26 13:12:04.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2423 2023-07-25 10:34:14.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/core/reader/unified_reader.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    11929 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/core/reader/unified_reader_base.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-07-25 12:56:33.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       85 2022-07-25 12:54:00.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/converter/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      369 2023-07-22 16:01:59.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/converter/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      559 2022-07-25 12:26:23.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      391 2023-05-22 11:15:00.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/converter/convert_ndarray_to_list.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      809 2023-07-22 15:47:27.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/converter/escape_non_str_dict_key.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      605 2023-07-22 16:02:29.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/converter/escape_tuple.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      377 2023-05-22 11:15:00.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/converter/integrate.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      808 2023-07-22 16:14:24.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/converter/unescape_non_str_dict_key.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      661 2023-07-22 16:14:24.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/converter/unescape_tuple.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1753 2023-07-25 12:37:51.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/read_json.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2355 2023-07-25 12:37:51.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/write_json.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2023-02-08 07:16:46.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3621 2022-11-16 07:31:34.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/converter.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8071 2023-06-21 01:55:22.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16285 2023-06-21 00:22:15.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      447 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/read.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/test/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-08-01 07:19:40.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      324 2022-08-01 07:19:40.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_0.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      249 2022-08-01 07:22:27.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6838 2023-06-21 00:15:01.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      556 2023-06-21 00:11:28.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/write.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/markdown/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      125 2023-07-26 13:43:05.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/markdown/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      304 2023-07-26 13:41:36.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/markdown/generate_link.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1006 2023-07-26 13:41:54.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/markdown/generate_list.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1236 2023-07-26 13:42:14.000000 kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/markdown/generate_table.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-08 10:14:56.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/decorator/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       66 2022-02-08 10:15:24.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/decorator/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      399 2022-02-08 06:57:21.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/decorator/restore_original_work_path.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       20 2022-04-18 08:15:52.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/producer_consumer/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       28 2022-04-18 08:15:52.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/producer_consumer/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      892 2022-12-12 08:39:00.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3164 2022-04-18 08:15:52.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       50 2022-04-18 11:35:30.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/producer_consumer/getter.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      740 2022-04-18 12:49:09.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2299 2022-04-18 12:23:06.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/producer_consumer/node.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-04-18 08:15:52.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/producer_consumer/producer.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       51 2022-04-18 10:40:32.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/producer_consumer/sender.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/singleton/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-04-18 13:24:36.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/singleton/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3803 2023-06-12 12:14:03.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2089 2022-02-28 06:54:56.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/general_matrix_multiplication.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/numerical_characteristics/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-02 05:01:47.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/numerical_characteristics/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2953 2022-06-02 05:03:41.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/numerical_characteristics/iou.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/temperate/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      630 2022-03-13 18:22:06.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/temperate/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      213 2022-03-10 05:06:13.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/temperate/iterator_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1663 2022-03-13 18:22:06.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/temperate/my_iterator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1214 2022-03-10 05:06:13.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/temperate/my_iterator_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      217 2022-03-10 05:06:13.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/temperate/sequence_map_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      241 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/developing/test.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/env_info/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-30 13:18:27.000000 kevin-toolbox-1.2.1/kevin_toolbox/env_info/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      879 2023-04-10 12:53:17.000000 kevin-toolbox-1.2.1/kevin_toolbox/env_info/check_validity_and_uninstall.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1953 2023-06-21 01:55:26.000000 kevin-toolbox-1.2.1/kevin_toolbox/env_info/check_version_and_update.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/env_info/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-30 12:51:50.000000 kevin-toolbox-1.2.1/kevin_toolbox/env_info/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1728 2023-04-13 07:53:17.000000 kevin-toolbox-1.2.1/kevin_toolbox/env_info/test/test_version.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/env_info/version/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      187 2023-03-30 13:11:22.000000 kevin-toolbox-1.2.1/kevin_toolbox/env_info/version/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2489 2023-04-13 07:51:40.000000 kevin-toolbox-1.2.1/kevin_toolbox/env_info/version/compare_version.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      860 2023-04-13 07:46:23.000000 kevin-toolbox-1.2.1/kevin_toolbox/env_info/version/parse_version.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2458 2023-03-30 13:11:22.000000 kevin-toolbox-1.2.1/kevin_toolbox/env_info/version/sort_version_ls.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-05 07:35:48.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      650 2023-03-24 10:03:29.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/__old_version/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-24 10:03:09.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/__old_version/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2564 2023-03-24 09:28:54.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5701 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      305 2023-03-24 09:34:05.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/cal_area_of_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3079 2023-05-16 14:16:04.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8249 2022-08-01 13:19:11.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      836 2022-08-01 11:47:43.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/detect_collision.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2762 2022-07-06 13:18:05.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8255 2023-05-16 11:51:25.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8634 2023-06-21 01:55:28.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/detect_overlap.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      292 2022-07-05 08:41:47.000000 kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/get_ticks_of_boxes.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-28 06:47:25.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-10 07:21:33.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-14 08:37:13.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/analysis/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2022-09-28 09:26:13.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/analysis/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4714 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/dummy/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       54 2022-02-28 08:44:35.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/dummy/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7137 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2022-09-26 09:52:59.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      896 2022-03-13 18:22:06.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1858 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    17766 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/factory.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      299 2022-03-13 18:22:06.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4480 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3482 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4799 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5480 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      224 2022-03-13 18:22:06.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3114 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3773 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      170 2022-03-10 12:36:00.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/merge.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 04:21:21.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/binary_classification/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      427 2022-02-22 06:22:25.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/binary_classification/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-21 13:29:08.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3247 2022-02-22 06:22:25.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5319 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3355 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      891 2022-04-28 12:02:07.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      442 2022-02-22 05:39:00.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/convert.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3661 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-27 07:16:21.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-03 13:07:44.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/concat_and_split/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      157 2022-08-08 08:06:40.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/concat_and_split/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    23861 2023-06-14 03:08:32.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4997 2022-08-08 08:19:17.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3066 2022-08-08 08:19:17.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      232 2023-03-13 06:47:47.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/convert/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       43 2023-03-13 06:47:47.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/convert/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4972 2023-03-10 14:11:22.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/generate/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      264 2023-03-13 06:47:47.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/generate/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3380 2023-03-13 06:48:36.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5738 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4426 2022-07-29 07:53:01.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1373 2023-03-10 13:56:45.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/reshape/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      220 2022-07-25 13:28:44.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/reshape/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1946 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1064 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/reshape/merge_blocks.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1236 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/reshape/split_blocks.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1859 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/transpose/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      177 2022-05-31 10:43:01.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/transpose/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      611 2022-08-09 13:17:49.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1472 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/number_theory/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      182 2023-03-05 15:57:35.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/number_theory/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      244 2023-03-05 15:45:13.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/number_theory/cache.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      387 2023-03-05 15:57:35.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/number_theory/get_greatest_common_divisor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      949 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/number_theory/get_primes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      499 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/number_theory/prime_factorization.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/number_theory/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-06 07:12:06.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/number_theory/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      747 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      784 2023-03-31 07:27:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/number_theory/test/test_get_primes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      551 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/number_theory/test/test_prime_factorization.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/transform/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-10 08:52:28.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/transform/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/transform/dct/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      147 2022-07-22 13:25:44.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/transform/dct/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8296 2023-03-31 07:27:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/transform/dct/dct_calculator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4305 2022-07-20 12:21:16.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/transform/scaling_and_shift/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       29 2022-07-30 13:19:40.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/transform/scaling_and_shift/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1280 2022-07-30 13:48:26.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/transform/scaling_and_shift/scaling.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/utils/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      289 2023-04-21 12:36:14.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/utils/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1943 2022-08-09 12:09:28.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/utils/convert_dtype.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1620 2022-08-08 08:50:02.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/utils/get_crop_by_box.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1553 2022-08-02 12:15:03.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1775 2022-08-08 08:50:02.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/utils/set_crop_by_box.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      345 2023-05-30 12:44:28.000000 kevin-toolbox-1.2.1/kevin_toolbox/math/utils/spilt_integer_most_evenly.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      241 2023-07-26 06:34:50.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      908 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/copy_.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      614 2023-07-25 12:37:51.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/count_leaf_node_nums.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1286 2023-06-21 01:55:54.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/get_hash.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3457 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/get_nodes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2083 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/get_value.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/name_handler/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      107 2023-06-20 10:05:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/name_handler/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1020 2023-07-26 07:45:46.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/name_handler/build_name.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1163 2023-06-20 09:49:43.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/name_handler/escape_node.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2311 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/name_handler/parse_name.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       48 2023-07-26 08:00:49.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-07-20 06:49:05.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1819 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_json_.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1470 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_bin.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1384 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_npy.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1282 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_pickle_.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      853 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_skip_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1355 2023-07-26 13:30:24.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_skip_simple.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1282 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_torch_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1353 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_torch_tensor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1741 2023-07-20 07:15:24.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/backend_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2540 2023-07-26 06:34:50.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/read.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      393 2023-07-26 06:34:50.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/variable.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    15027 2023-07-26 13:36:48.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/write.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2781 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/set_value.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6943 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/traverse.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/value_parser/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      169 2023-06-21 03:27:20.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/value_parser/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3119 2023-07-25 12:39:59.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/value_parser/cal_relation_between_references.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2301 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/value_parser/eval_references.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2116 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/value_parser/parse_references.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-29 13:28:32.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_matplotlib/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      127 2023-03-10 08:30:36.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_matplotlib/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1837 2023-03-10 10:16:48.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1696 2023-03-10 09:17:25.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1361 2023-03-10 08:13:57.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_matplotlib/arrow3d.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_numpy/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-24 08:38:24.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_numpy/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_numpy/linalg/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       99 2023-04-24 08:58:58.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_numpy/linalg/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      423 2023-05-17 07:05:16.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_numpy/linalg/cos_similar.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      625 2023-04-24 08:52:01.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_numpy/linalg/normalize.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      253 2023-04-24 08:55:02.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_numpy/linalg/softmax.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_optuna/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2023-05-26 09:14:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_optuna/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4580 2023-07-26 06:32:19.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_os/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       77 2023-07-21 09:36:08.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_os/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      656 2023-07-21 09:38:57.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_os/pack.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      658 2023-04-17 12:51:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_os/remove.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1047 2023-07-21 09:40:06.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_os/unpack.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-07-29 06:55:38.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3184 2023-06-26 08:43:44.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_test/check_consistency.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 06:56:01.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       75 2023-03-08 07:01:29.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      393 2023-04-12 15:31:18.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/concat.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/linalg/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       44 2023-03-08 08:04:27.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/linalg/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      770 2023-04-12 15:31:18.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      575 2023-04-12 15:31:18.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/nn/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-05-30 11:36:55.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/nn/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5357 2023-04-12 15:31:18.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      845 2023-04-12 15:31:18.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/tile.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-04-12 15:36:21.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/where.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/math/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       68 2022-02-21 09:51:39.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/math/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2047 2022-02-22 06:43:43.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/math/get_y_at_x.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1378 2022-02-21 09:44:44.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/math/my_around.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/nn/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-05-30 11:37:07.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/nn/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      223 2023-05-29 08:32:26.000000 kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/nn/lambda_layer.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox.egg-info/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1563 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    15328 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       92 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox.egg-info/requires.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       14 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/kevin_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       59 2023-03-31 06:32:36.000000 kevin-toolbox-1.2.1/pyproject.toml
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      904 2023-07-26 13:48:37.000000 kevin-toolbox-1.2.1/setup.cfg
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-03-31 07:25:47.000000 kevin-toolbox-1.2.1/setup.py
```

### Comparing `kevin-toolbox-1.2.0/PKG-INFO` & `kevin-toolbox-1.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevin-toolbox
-Version: 1.2.0
+Version: 1.2.1
 Summary: 一个常用的工具代码包集合
 Home-page: https://github.com/cantbeblank96/kevin_toolbox
 Download-URL: https://github.com/username/your-package/archive/refs/tags/v1.0.0.tar.gz
 Author: kevin hsu
 Author-email: xukaiming1996@163.com
 License: MIT
 Keywords: mathematics,pytorch,numpy,machine-learning,algorithm
@@ -41,17 +41,13 @@
 
 [使用指南 User_Guide](./notes/User_Guide.md)
 
 [免责声明 Disclaimer](./notes/Disclaimer.md)
 
 [版本更新记录](./notes/Release_Record.md)：
 
-- v 1.2.0（2023-07-25）【refactor】【new feature】
+- v 1.2.1（2023-07-25）【bug fix】【new feature】
   - nested_dict_list
-    - refactor computer_science.algorithm.for_nested_dict_list to nested_dict_list【refactor】
-    - rename set_value_by_name() to set_value()
-    - rename get_value_by_name() to get_value()
-    - add serializer，添加序列化模块来写入 write() 和读取 read() 嵌套字典列表【new feature】
-      - 其中 write() 支持使用 settings 参数来指定不同部分的序列化方式和匹配方式
-      - 支持在 SERIALIZER_BACKEND 中注册自定义的序列化方式
-  - data_flow.file.json_
-    - modify write()，支持 file_path 参数设置为 None 来直接获取序列化结果而非写入到具体文件中。 
+    - fix bug in backend ":skip:simple" registered in SERIALIZER_BACKEND，修复了没有拒绝具有结构复杂的元素的 tuple 的问题。【bug fix】
+    - fix bug in write()，补充了参数 settings 缺少的默认值。【bug fix】
+  - data_flow.file【new feature】
+    - add new module markdown，包括 generate_link()、generate_list()、generate_table() 等方法，用于创建 markdown 格式的链接、多级列表、表格。
```

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/registration/registry.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/registration/registry.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/scheduler/trigger.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/scheduler/trigger.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/search/binary_search.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/search/binary_search.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/statistician/_init_var.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/statistician/_init_var.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/computer_science/data_structure/executor.py` & `kevin-toolbox-1.2.1/kevin_toolbox/computer_science/data_structure/executor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py` & `kevin-toolbox-1.2.1/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/core/reader/unified_reader.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/core/reader/unified_reader.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/core/reader/unified_reader_base.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/core/reader/unified_reader_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/converter/escape_non_str_dict_key.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/converter/escape_non_str_dict_key.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/converter/escape_tuple.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/converter/escape_tuple.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/converter/unescape_non_str_dict_key.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/converter/unescape_non_str_dict_key.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/converter/unescape_tuple.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/converter/unescape_tuple.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/read_json.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/read_json.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/json_/write_json.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/json_/write_json.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/converter.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/converter.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/data_flow/file/kevin_notation/write.py` & `kevin-toolbox-1.2.1/kevin_toolbox/data_flow/file/kevin_notation/write.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py` & `kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py` & `kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py` & `kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/producer_consumer/node.py` & `kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/producer_consumer/node.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py` & `kevin-toolbox-1.2.1/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/developing/general_matrix_multiplication.py` & `kevin-toolbox-1.2.1/kevin_toolbox/developing/general_matrix_multiplication.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/developing/numerical_characteristics/iou.py` & `kevin-toolbox-1.2.1/kevin_toolbox/developing/numerical_characteristics/iou.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/developing/temperate/__init__.py` & `kevin-toolbox-1.2.1/kevin_toolbox/developing/temperate/__init__.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/developing/temperate/my_iterator.py` & `kevin-toolbox-1.2.1/kevin_toolbox/developing/temperate/my_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/developing/temperate/my_iterator_base.py` & `kevin-toolbox-1.2.1/kevin_toolbox/developing/temperate/my_iterator_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/env_info/check_validity_and_uninstall.py` & `kevin-toolbox-1.2.1/kevin_toolbox/env_info/check_validity_and_uninstall.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/env_info/check_version_and_update.py` & `kevin-toolbox-1.2.1/kevin_toolbox/env_info/check_version_and_update.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/env_info/test/test_version.py` & `kevin-toolbox-1.2.1/kevin_toolbox/env_info/test/test_version.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/env_info/version/compare_version.py` & `kevin-toolbox-1.2.1/kevin_toolbox/env_info/version/compare_version.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/env_info/version/parse_version.py` & `kevin-toolbox-1.2.1/kevin_toolbox/env_info/version/parse_version.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/env_info/version/sort_version_ls.py` & `kevin-toolbox-1.2.1/kevin_toolbox/env_info/version/sort_version_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/__init__.py` & `kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/__init__.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py` & `kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py` & `kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py` & `kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py` & `kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/detect_collision.py` & `kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/detect_collision.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py` & `kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py` & `kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/geometry/for_boxes/detect_overlap.py` & `kevin-toolbox-1.2.1/kevin_toolbox/geometry/for_boxes/detect_overlap.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/factory.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/factory.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py` & `kevin-toolbox-1.2.1/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/reshape/merge_blocks.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/reshape/merge_blocks.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/reshape/split_blocks.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/reshape/split_blocks.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/number_theory/get_primes.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/number_theory/get_primes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/number_theory/test/test_get_primes.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/number_theory/test/test_get_primes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/number_theory/test/test_prime_factorization.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/number_theory/test/test_prime_factorization.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/transform/dct/dct_calculator.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/transform/dct/dct_calculator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/transform/scaling_and_shift/scaling.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/transform/scaling_and_shift/scaling.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/utils/convert_dtype.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/utils/convert_dtype.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/utils/get_crop_by_box.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/utils/get_crop_by_box.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/math/utils/set_crop_by_box.py` & `kevin-toolbox-1.2.1/kevin_toolbox/math/utils/set_crop_by_box.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/copy_.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/copy_.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/count_leaf_node_nums.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/count_leaf_node_nums.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/get_hash.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/get_hash.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/get_nodes.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/get_nodes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/get_value.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/get_value.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/name_handler/build_name.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/name_handler/build_name.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/name_handler/escape_node.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/name_handler/escape_node.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/name_handler/parse_name.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/name_handler/parse_name.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_json_.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_json_.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_bin.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_bin.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_npy.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_numpy_npy.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_pickle_.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_pickle_.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_skip_all.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_skip_all.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_skip_simple.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_skip_simple.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 from kevin_toolbox.nested_dict_list.serializer.backends import Backend_Base
 from kevin_toolbox.nested_dict_list.serializer.variable import SERIALIZER_BACKEND
 
 
 @SERIALIZER_BACKEND.register(name=":skip:simple")
 class Skip_Simple(Backend_Base):
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.w_cache = None
+        self.w_cache_id = None
+
     def write(self, name, var, **kwargs):
-        assert self.writable(var=var)
+        if id(var) != self.w_cache_id:
+            assert self.writable(var=var)
         return var
 
     def read(self, name, **kwargs):
         raise Exception(f'calling skip.read() is prohibited')
 
     def writable(self, var, **kwargs):
         """
             是否可以写
         """
-        return isinstance(var, (int, float, str, tuple))
+        self.w_cache = False
+        if isinstance(var, (int, float, str)):
+            self.w_cache = True
+        elif isinstance(var, (tuple,)):
+            self.w_cache = all(isinstance(i, (int, float, str)) for i in var)
+        self.w_cache_id = id(var)
+        return self.w_cache
 
     def readable(self, name, **kwargs):
         """
             是否可以写
         """
         return False
```

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_torch_all.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_torch_all.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/_torch_tensor.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/_torch_tensor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/backends/backend_base.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/backends/backend_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/read.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/read.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/serializer/write.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/serializer/write.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import kevin_toolbox
 from kevin_toolbox.data_flow.file import json_
 from kevin_toolbox.patches import for_os
 import kevin_toolbox.nested_dict_list as ndl
 from kevin_toolbox.nested_dict_list.serializer.variable import SERIALIZER_BACKEND
 
 
-def write(var, output_dir, settings, traversal_mode="bfs", b_pack_into_tar=True, **kwargs):
+def write(var, output_dir, settings=None, traversal_mode="bfs", b_pack_into_tar=True, **kwargs):
     """
         将输入的嵌套字典列表 var 的结构和节点值保存到文件中
             遍历 var，匹配并使用 settings 中设置的保存方式来对各部分结构/节点进行序列化
             将会生成一个文件夹或者 .tar 文件，其中包含：
                 - var.json：     用于保存结构、简单节点值、复杂节点值/结构的序列化方式
                 - nodes/目录：    其中包含一系列 <name>.<suffix> 文件或者 <name> 文件夹，其中包含复杂节点值/结构的序列化结果
                 - record.json：   其中记录了：
@@ -41,15 +41,15 @@
                                             - ":numpy:npy"      若对象为 np.array，则以 .npy 的形式进行序列化
                                             - ":torch:tensor"   若对象为 torch.tensor，则调用 torch 中的 load 和 save 进行序列化
                                             - ":torch:all"      调用 torch 中的 load() 和 save() 进行序列化
                                             - ":json"           若对象可以被 json 格式保存，则将其按照 json 格式进行序列化
                                             - ":pickle"         调用 pickle 中的 load() 和 save() 进行序列化
                                         比如组合 (":skip:simple", ":numpy:bin", ":torch:tensor", ":pickle") 则表示根据变量的类型，依次尝试这几种方式
                                             直至成功。其含义为：
-                                                - 如果是可以直接写入到 json 中的 int、float、str、tuple 等则选用 ":skip:simple"
+                                                - 如果是可以直接写入到 json 中的 int、float、str、简单的 tuple 等则选用 ":skip:simple"
                                                 - 如果是 np.array 则选用 ":numpy:bin"
                                                 - 如果是 tensor 则选用 ":torch:tensor"
                                                 - 其他无法处理的类型则选用 ":pickle"
                                         <序列化方式>允许进行自定义扩增，若要添加新的<序列化方式>，可以实现一个带有：
                                                 - write(name, var):         序列化
                                                 - read(name):               反序列化
                                                 - writable(var):            是否可以写
@@ -58,26 +58,28 @@
                                             backends._torch_tensor.py 中的实现方式。
                                         <遍历方式>支持以下3种:
                                             - "dfs_pre_order"         深度优先、先序遍历
                                             - "dfs_post_order"        深度优先、后序遍历
                                             - "bfs"                   宽度优先
                                             省略时默认使用参数 traversal_mode 中的设置，更多参考 traverse() 中的介绍。
                                         默认的处理模式是：
-                                            [{"match_cond": "<leaf>", "backend": (":skip:simple", ":numpy:bin", ":torch:tensor", ":pickle")}]
+                                            [{"match_cond": "<level>-1", "backend": (":skip:simple", ":numpy:npy", ":torch:tensor", ":pickle")}]
             traversal_mode:         <str> 遍历方式
                                         默认使用 "bfs"
             output_dir:             <path> 输出文件夹
             b_pack_into_tar:        <boolean> 是否将输出打包成 tar 文件
                                         默认是 True，此时结果将保存到 /<output_dir>.tar 下。
     """
 
     #
     assert traversal_mode in ("dfs_pre_order", "dfs_post_order", "bfs")
     os.makedirs(output_dir, exist_ok=True)
     var = ndl.copy_(var=var, b_deepcopy=True)
+    if settings is None:
+        settings = [{"match_cond": "<level>-1", "backend": (":skip:simple", ":numpy:npy", ":torch:tensor", ":pickle")}]
 
     # 构建 processed_s
     #     为了避免重复处理节点/结构，首先构建与 var 具有相似结构的 processed_s 来记录处理处理进度。
     #     对于 processed_s，其节点值为 True 时表示该节点已经被处理，当节点值为 False 或者 list/dict 类型时表示该节点或者节点下面的结构中仍然
     #       存在未处理的部分。
     #     对于中间节点，只有其下所有叶节点都未处理时才会被匹配。
     processed_s = dict()
@@ -252,22 +254,22 @@
         "b": [torch.randn(5), torch.randn(3)],
         (1, 2, 3): (1, 2, 3),
         "model": dict(name="m", paras=dict(paras=dict(layer_nums=3, input_shape=np.random.rand(2, 5))))
     }
     # var_ = None
 
     _test_hook = dict()
-    settings = [
+    settings_ = [
         {"match_cond": lambda _, idx, value: "paras" == name_handler.parse_name(name=idx)[2][-1],
          "backend": (":pickle",),
          "traversal_mode": "dfs_post_order"},
         {"match_cond": "<level>-1",
          "backend": (":numpy:bin", ":torch:tensor")},
         {"match_cond": lambda _, __, value: not isinstance(value, (list, dict)),
          "backend": (":skip:simple",)},
     ]
     write(var=var_, output_dir=os.path.join(os.path.dirname(__file__), "temp3"), traversal_mode="bfs",
-          b_pack_into_tar=True, settings=settings, _test_hook=_test_hook)
+          b_pack_into_tar=True, settings=settings_, _test_hook=_test_hook)
 
     for bk_name, p in _test_hook["processed"]:
         print(f'backend: {bk_name}')
         print(p)
```

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/set_value.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/set_value.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/traverse.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/traverse.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/value_parser/cal_relation_between_references.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/value_parser/cal_relation_between_references.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/value_parser/eval_references.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/value_parser/eval_references.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/nested_dict_list/value_parser/parse_references.py` & `kevin-toolbox-1.2.1/kevin_toolbox/nested_dict_list/value_parser/parse_references.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_matplotlib/arrow3d.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_matplotlib/arrow3d.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_numpy/linalg/normalize.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_numpy/linalg/normalize.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_os/pack.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_os/pack.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_os/remove.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_os/remove.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_os/unpack.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_os/unpack.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_test/check_consistency.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_test/check_consistency.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/tile.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/tile.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/compatible/where.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/compatible/where.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/math/get_y_at_x.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/math/get_y_at_x.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox/patches/for_torch/math/my_around.py` & `kevin-toolbox-1.2.1/kevin_toolbox/patches/for_torch/math/my_around.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox.egg-info/PKG-INFO` & `kevin-toolbox-1.2.1/kevin_toolbox.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevin-toolbox
-Version: 1.2.0
+Version: 1.2.1
 Summary: 一个常用的工具代码包集合
 Home-page: https://github.com/cantbeblank96/kevin_toolbox
 Download-URL: https://github.com/username/your-package/archive/refs/tags/v1.0.0.tar.gz
 Author: kevin hsu
 Author-email: xukaiming1996@163.com
 License: MIT
 Keywords: mathematics,pytorch,numpy,machine-learning,algorithm
@@ -41,17 +41,13 @@
 
 [使用指南 User_Guide](./notes/User_Guide.md)
 
 [免责声明 Disclaimer](./notes/Disclaimer.md)
 
 [版本更新记录](./notes/Release_Record.md)：
 
-- v 1.2.0（2023-07-25）【refactor】【new feature】
+- v 1.2.1（2023-07-25）【bug fix】【new feature】
   - nested_dict_list
-    - refactor computer_science.algorithm.for_nested_dict_list to nested_dict_list【refactor】
-    - rename set_value_by_name() to set_value()
-    - rename get_value_by_name() to get_value()
-    - add serializer，添加序列化模块来写入 write() 和读取 read() 嵌套字典列表【new feature】
-      - 其中 write() 支持使用 settings 参数来指定不同部分的序列化方式和匹配方式
-      - 支持在 SERIALIZER_BACKEND 中注册自定义的序列化方式
-  - data_flow.file.json_
-    - modify write()，支持 file_path 参数设置为 None 来直接获取序列化结果而非写入到具体文件中。 
+    - fix bug in backend ":skip:simple" registered in SERIALIZER_BACKEND，修复了没有拒绝具有结构复杂的元素的 tuple 的问题。【bug fix】
+    - fix bug in write()，补充了参数 settings 缺少的默认值。【bug fix】
+  - data_flow.file【new feature】
+    - add new module markdown，包括 generate_link()、generate_list()、generate_table() 等方法，用于创建 markdown 格式的链接、多级列表、表格。
```

### Comparing `kevin-toolbox-1.2.0/kevin_toolbox.egg-info/SOURCES.txt` & `kevin-toolbox-1.2.1/kevin_toolbox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,18 @@
 kevin_toolbox/data_flow/file/kevin_notation/read.py
 kevin_toolbox/data_flow/file/kevin_notation/write.py
 kevin_toolbox/data_flow/file/kevin_notation/test/__init__.py
 kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py
 kevin_toolbox/data_flow/file/kevin_notation/test/test_data/__init__.py
 kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_0.py
 kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_all.py
+kevin_toolbox/data_flow/file/markdown/__init__.py
+kevin_toolbox/data_flow/file/markdown/generate_link.py
+kevin_toolbox/data_flow/file/markdown/generate_list.py
+kevin_toolbox/data_flow/file/markdown/generate_table.py
 kevin_toolbox/developing/__init__.py
 kevin_toolbox/developing/general_matrix_multiplication.py
 kevin_toolbox/developing/test.py
 kevin_toolbox/developing/decorator/__init__.py
 kevin_toolbox/developing/decorator/restore_original_work_path.py
 kevin_toolbox/developing/design_pattern/__init__.py
 kevin_toolbox/developing/design_pattern/producer_consumer/__init__.py
```

### Comparing `kevin-toolbox-1.2.0/setup.cfg` & `kevin-toolbox-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.2.0/setup.py` & `kevin-toolbox-1.2.1/setup.py`

 * *Files identical despite different names*

