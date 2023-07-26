# Comparing `tmp/kevin-toolbox-1.1.5.tar.gz` & `tmp/kevin-toolbox-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kevin-toolbox-1.1.5.tar", last modified: Mon Jul 24 09:40:11 2023, max compression
+gzip compressed data, was "dist/kevin-toolbox-1.1.6.tar", last modified: Tue Jul 25 12:34:05 2023, max compression
```

## Comparing `kevin-toolbox-1.1.5.tar` & `kevin-toolbox-1.1.6.tar`

### file list

```diff
@@ -1,339 +1,339 @@
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1225 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/PKG-INFO
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      632 2023-07-24 09:39:09.000000 kevin-toolbox-1.1.5/README.md
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       23 2023-07-24 09:37:58.000000 kevin-toolbox-1.1.5/kevin_toolbox/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-12-01 13:56:40.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-04 15:12:36.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      142 2023-03-05 16:13:01.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1832 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1914 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2078 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2819 2023-03-05 16:40:22.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_dict/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       37 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_dict/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      666 2023-06-19 08:36:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      273 2023-06-14 02:14:33.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      939 2023-06-30 08:56:00.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/copy_.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      645 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/count_leaf_node_nums.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1286 2023-06-21 01:55:54.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_hash.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3543 2023-06-20 10:55:20.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_nodes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2122 2023-06-27 09:56:21.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_value_by_name.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      107 2023-06-20 10:05:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1051 2023-06-20 10:25:59.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/build_name.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1163 2023-06-20 09:49:43.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/escape_node.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2350 2023-06-20 23:12:24.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/parse_name.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-04 08:21:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-07-20 06:49:05.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1752 2023-07-22 16:28:34.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_json_.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1514 2023-07-22 14:39:29.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_numpy_bin.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1446 2023-07-22 14:58:58.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_numpy_npy.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1344 2023-07-22 15:01:03.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_pickle_.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      915 2023-07-20 08:55:12.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_skip_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      961 2023-07-20 08:57:14.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_skip_simple.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1344 2023-07-22 15:12:03.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_torch_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1415 2023-07-20 08:24:32.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_torch_tensor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1741 2023-07-20 07:15:24.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/backend_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1878 2023-07-13 09:08:19.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/load.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      424 2023-07-22 14:59:45.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/variable.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    14732 2023-07-22 16:30:54.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/write.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2875 2023-06-27 09:41:07.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/set_value_by_name.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6975 2023-07-20 11:57:24.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/traverse.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      169 2023-06-21 03:27:20.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3181 2023-06-21 03:27:20.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/cal_relation_between_references.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2372 2023-06-30 07:58:07.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/eval_references.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2155 2023-06-21 03:37:47.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/parse_references.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_seq/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_seq/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1046 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      309 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_seq/get_subsets.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/locks/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-04-21 13:18:26.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/locks/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2492 2023-04-24 08:04:07.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/pareto_front/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       57 2023-04-10 08:46:01.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/pareto_front/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2712 2023-04-10 09:09:27.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/registration/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2023-06-12 14:36:27.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/registration/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    13919 2023-07-20 08:22:19.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/registration/registry.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/scheduler/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-06-02 12:00:07.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/scheduler/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    12265 2023-06-29 14:30:59.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4508 2023-06-27 11:00:57.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/scheduler/trigger.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/search/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       41 2023-03-20 13:18:25.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/search/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1013 2023-03-04 15:58:55.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/search/binary_search.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/statistician/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      120 2023-06-01 10:31:40.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/statistician/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      904 2023-06-01 10:26:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/statistician/_init_var.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3101 2023-06-01 10:35:42.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5571 2023-06-01 10:29:44.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/utils/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-08 14:31:25.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/utils/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/data_structure/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       31 2023-03-22 06:30:28.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/data_structure/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6206 2023-06-21 01:55:31.000000 kevin-toolbox-1.1.5/kevin_toolbox/computer_science/data_structure/executor.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/dangerous/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       93 2023-03-29 12:29:14.000000 kevin-toolbox-1.1.5/kevin_toolbox/dangerous/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2898 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 12:43:00.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/core/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 09:06:12.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/core/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/core/cache/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       79 2022-02-08 11:12:52.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/core/cache/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16060 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/core/reader/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      146 2022-02-09 09:12:47.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/core/reader/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8827 2022-04-26 13:12:04.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2507 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/core/reader/unified_reader.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    11929 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/core/reader/unified_reader_base.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-07-25 12:56:33.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       85 2022-07-25 12:54:00.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/converter/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      369 2023-07-22 16:01:59.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/converter/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      559 2022-07-25 12:26:23.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      391 2023-05-22 11:15:00.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/converter/convert_ndarray_to_list.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      809 2023-07-22 15:47:27.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/converter/escape_non_str_dict_key.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      605 2023-07-22 16:02:29.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/converter/escape_tuple.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      377 2023-05-22 11:15:00.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/converter/integrate.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      808 2023-07-22 16:14:24.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/converter/unescape_non_str_dict_key.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      661 2023-07-22 16:14:24.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/converter/unescape_tuple.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1784 2023-07-24 07:20:15.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/read_json.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2003 2023-07-24 09:30:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/write_json.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2023-02-08 07:16:46.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3621 2022-11-16 07:31:34.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/converter.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8071 2023-06-21 01:55:22.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16285 2023-06-21 00:22:15.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      447 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/read.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/test/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-08-01 07:19:40.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      324 2022-08-01 07:19:40.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_0.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      249 2022-08-01 07:22:27.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6838 2023-06-21 00:15:01.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      556 2023-06-21 00:11:28.000000 kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/write.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-08 10:14:56.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/decorator/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       66 2022-02-08 10:15:24.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/decorator/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      399 2022-02-08 06:57:21.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/decorator/restore_original_work_path.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       20 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/producer_consumer/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       28 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/producer_consumer/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      892 2022-12-12 08:39:00.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3164 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       50 2022-04-18 11:35:30.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/producer_consumer/getter.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      740 2022-04-18 12:49:09.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2299 2022-04-18 12:23:06.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/producer_consumer/node.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/producer_consumer/producer.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       51 2022-04-18 10:40:32.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/producer_consumer/sender.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/singleton/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-04-18 13:24:36.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/singleton/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3803 2023-06-12 12:14:03.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2089 2022-02-28 06:54:56.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/general_matrix_multiplication.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/numerical_characteristics/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-02 05:01:47.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/numerical_characteristics/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2953 2022-06-02 05:03:41.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/numerical_characteristics/iou.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/temperate/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      630 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/temperate/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      213 2022-03-10 05:06:13.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/temperate/iterator_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1663 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/temperate/my_iterator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1214 2022-03-10 05:06:13.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/temperate/my_iterator_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      217 2022-03-10 05:06:13.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/temperate/sequence_map_base.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      241 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/developing/test.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/env_info/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-30 13:18:27.000000 kevin-toolbox-1.1.5/kevin_toolbox/env_info/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      879 2023-04-10 12:53:17.000000 kevin-toolbox-1.1.5/kevin_toolbox/env_info/check_validity_and_uninstall.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1953 2023-06-21 01:55:26.000000 kevin-toolbox-1.1.5/kevin_toolbox/env_info/check_version_and_update.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/env_info/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-30 12:51:50.000000 kevin-toolbox-1.1.5/kevin_toolbox/env_info/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1728 2023-04-13 07:53:17.000000 kevin-toolbox-1.1.5/kevin_toolbox/env_info/test/test_version.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/env_info/version/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      187 2023-03-30 13:11:22.000000 kevin-toolbox-1.1.5/kevin_toolbox/env_info/version/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2489 2023-04-13 07:51:40.000000 kevin-toolbox-1.1.5/kevin_toolbox/env_info/version/compare_version.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      860 2023-04-13 07:46:23.000000 kevin-toolbox-1.1.5/kevin_toolbox/env_info/version/parse_version.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2458 2023-03-30 13:11:22.000000 kevin-toolbox-1.1.5/kevin_toolbox/env_info/version/sort_version_ls.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-05 07:35:48.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      650 2023-03-24 10:03:29.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/__old_version/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-24 10:03:09.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/__old_version/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2564 2023-03-24 09:28:54.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5701 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      305 2023-03-24 09:34:05.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/cal_area_of_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3079 2023-05-16 14:16:04.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8249 2022-08-01 13:19:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      836 2022-08-01 11:47:43.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/detect_collision.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2762 2022-07-06 13:18:05.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8255 2023-05-16 11:51:25.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8634 2023-06-21 01:55:28.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/detect_overlap.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      292 2022-07-05 08:41:47.000000 kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/get_ticks_of_boxes.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-28 06:47:25.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-10 07:21:33.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-14 08:37:13.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/analysis/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2022-09-28 09:26:13.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/analysis/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4714 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/dummy/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       54 2022-02-28 08:44:35.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/dummy/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7137 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2022-09-26 09:52:59.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      896 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1858 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    17766 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/factory.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      299 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4480 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3482 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4799 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5480 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      224 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3114 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3773 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      170 2022-03-10 12:36:00.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/merge.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 04:21:21.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/binary_classification/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      427 2022-02-22 06:22:25.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/binary_classification/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-21 13:29:08.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3247 2022-02-22 06:22:25.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5319 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3355 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      891 2022-04-28 12:02:07.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      442 2022-02-22 05:39:00.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/convert.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3661 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-27 07:16:21.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-03 13:07:44.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/concat_and_split/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      157 2022-08-08 08:06:40.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/concat_and_split/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    23861 2023-06-14 03:08:32.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4997 2022-08-08 08:19:17.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3066 2022-08-08 08:19:17.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      232 2023-03-13 06:47:47.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/convert/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       43 2023-03-13 06:47:47.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/convert/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4972 2023-03-10 14:11:22.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/generate/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      264 2023-03-13 06:47:47.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/generate/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3380 2023-03-13 06:48:36.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5738 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4426 2022-07-29 07:53:01.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1373 2023-03-10 13:56:45.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/reshape/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      220 2022-07-25 13:28:44.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/reshape/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1946 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1064 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/reshape/merge_blocks.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1236 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/reshape/split_blocks.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1859 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/transpose/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      177 2022-05-31 10:43:01.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/transpose/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      611 2022-08-09 13:17:49.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1472 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/number_theory/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      182 2023-03-05 15:57:35.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/number_theory/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      244 2023-03-05 15:45:13.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/number_theory/cache.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      387 2023-03-05 15:57:35.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/number_theory/get_greatest_common_divisor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      949 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/number_theory/get_primes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      499 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/number_theory/prime_factorization.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/number_theory/test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-06 07:12:06.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/number_theory/test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      747 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      784 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/number_theory/test/test_get_primes.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      551 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/number_theory/test/test_prime_factorization.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/transform/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-10 08:52:28.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/transform/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/transform/dct/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      147 2022-07-22 13:25:44.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/transform/dct/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8296 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/transform/dct/dct_calculator.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4305 2022-07-20 12:21:16.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/transform/scaling_and_shift/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       29 2022-07-30 13:19:40.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/transform/scaling_and_shift/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1280 2022-07-30 13:48:26.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/transform/scaling_and_shift/scaling.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/utils/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      289 2023-04-21 12:36:14.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/utils/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1943 2022-08-09 12:09:28.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/utils/convert_dtype.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1620 2022-08-08 08:50:02.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/utils/get_crop_by_box.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1553 2022-08-02 12:15:03.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1775 2022-08-08 08:50:02.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/utils/set_crop_by_box.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      345 2023-05-30 12:44:28.000000 kevin-toolbox-1.1.5/kevin_toolbox/math/utils/spilt_integer_most_evenly.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-29 13:28:32.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_matplotlib/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      127 2023-03-10 08:30:36.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_matplotlib/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1837 2023-03-10 10:16:48.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1696 2023-03-10 09:17:25.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1361 2023-03-10 08:13:57.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_matplotlib/arrow3d.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_numpy/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-24 08:38:24.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_numpy/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_numpy/linalg/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       99 2023-04-24 08:58:58.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_numpy/linalg/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      423 2023-05-17 07:05:16.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_numpy/linalg/cos_similar.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      625 2023-04-24 08:52:01.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_numpy/linalg/normalize.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      253 2023-04-24 08:55:02.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_numpy/linalg/softmax.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_optuna/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2023-05-26 09:14:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_optuna/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4588 2023-05-26 09:40:56.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_os/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       77 2023-07-21 09:36:08.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_os/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      656 2023-07-21 09:38:57.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_os/pack.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      658 2023-04-17 12:51:37.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_os/remove.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1047 2023-07-21 09:40:06.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_os/unpack.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_test/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-07-29 06:55:38.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_test/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3184 2023-06-26 08:43:44.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_test/check_consistency.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 06:56:01.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/__init__.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       75 2023-03-08 07:01:29.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      393 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/concat.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/linalg/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       44 2023-03-08 08:04:27.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/linalg/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      770 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      575 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/nn/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-05-30 11:36:55.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/nn/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5357 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      845 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/tile.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-04-12 15:36:21.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/where.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/math/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       68 2022-02-21 09:51:39.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/math/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2047 2022-02-22 06:43:43.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/math/get_y_at_x.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1378 2022-02-21 09:44:44.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/math/my_around.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/nn/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-05-30 11:37:07.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/nn/__init__.py
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      223 2023-05-29 08:32:26.000000 kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/nn/lambda_layer.py
-drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox.egg-info/
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1225 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16058 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       92 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox.egg-info/requires.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       14 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/kevin_toolbox.egg-info/top_level.txt
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       59 2023-03-31 06:32:36.000000 kevin-toolbox-1.1.5/pyproject.toml
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      904 2023-07-24 09:40:11.000000 kevin-toolbox-1.1.5/setup.cfg
--rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-03-31 07:25:47.000000 kevin-toolbox-1.1.5/setup.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1420 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/PKG-INFO
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      828 2023-07-25 12:33:44.000000 kevin-toolbox-1.1.6/README.md
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       23 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-12-01 13:56:40.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-04 15:12:36.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      142 2023-03-05 16:13:01.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1832 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1914 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2078 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2819 2023-03-05 16:40:22.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_dict/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       37 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_dict/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      666 2023-06-19 08:36:11.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      273 2023-06-14 02:14:33.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      939 2023-06-30 08:56:00.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/copy_.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      645 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/count_leaf_node_nums.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1286 2023-06-21 01:55:54.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_hash.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3543 2023-06-20 10:55:20.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_nodes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2122 2023-06-27 09:56:21.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_value_by_name.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      107 2023-06-20 10:05:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1051 2023-06-20 10:25:59.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/build_name.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1163 2023-06-20 09:49:43.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/escape_node.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2350 2023-06-20 23:12:24.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/parse_name.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-04 08:21:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-07-20 06:49:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1881 2023-07-25 10:44:52.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_json_.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1532 2023-07-25 11:14:08.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_numpy_bin.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1446 2023-07-22 14:58:58.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_numpy_npy.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1344 2023-07-22 15:01:03.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_pickle_.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      915 2023-07-20 08:55:12.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_skip_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      999 2023-07-25 11:00:21.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_skip_simple.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1344 2023-07-22 15:12:03.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_torch_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1415 2023-07-20 08:24:32.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_torch_tensor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1741 2023-07-20 07:15:24.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/backend_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2654 2023-07-25 12:05:30.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/read.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      424 2023-07-22 14:59:45.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/variable.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    14568 2023-07-25 11:41:13.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/write.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2875 2023-06-27 09:41:07.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/set_value_by_name.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6974 2023-07-25 12:26:45.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/traverse.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      169 2023-06-21 03:27:20.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3181 2023-06-21 03:27:20.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/cal_relation_between_references.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2372 2023-06-30 07:58:07.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/eval_references.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2155 2023-06-21 03:37:47.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/parse_references.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_seq/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_seq/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1046 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      309 2023-06-12 05:50:08.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_seq/get_subsets.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/locks/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-04-21 13:18:26.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/locks/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2492 2023-04-24 08:04:07.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/pareto_front/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       57 2023-04-10 08:46:01.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/pareto_front/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2712 2023-04-10 09:09:27.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/registration/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2023-06-12 14:36:27.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/registration/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    13919 2023-07-20 08:22:19.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/registration/registry.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/scheduler/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       76 2023-06-02 12:00:07.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/scheduler/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    12265 2023-06-29 14:30:59.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4508 2023-06-27 11:00:57.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/scheduler/trigger.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/search/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       41 2023-03-20 13:18:25.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/search/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1013 2023-03-04 15:58:55.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/search/binary_search.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/statistician/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      120 2023-06-01 10:31:40.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/statistician/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      904 2023-06-01 10:26:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/statistician/_init_var.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3101 2023-06-01 10:35:42.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5571 2023-06-01 10:29:44.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/utils/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-06-08 14:31:25.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/utils/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/data_structure/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       31 2023-03-22 06:30:28.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/data_structure/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6206 2023-06-21 01:55:31.000000 kevin-toolbox-1.1.6/kevin_toolbox/computer_science/data_structure/executor.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/dangerous/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       93 2023-03-29 12:29:14.000000 kevin-toolbox-1.1.6/kevin_toolbox/dangerous/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2898 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 12:43:00.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/core/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-25 09:06:12.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/core/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/core/cache/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       79 2022-02-08 11:12:52.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/core/cache/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16060 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/core/reader/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      146 2022-02-09 09:12:47.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/core/reader/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8827 2022-04-26 13:12:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2423 2023-07-25 10:34:14.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/core/reader/unified_reader.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    11929 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/core/reader/unified_reader_base.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-07-25 12:56:33.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       85 2022-07-25 12:54:00.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/converter/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      369 2023-07-22 16:01:59.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/converter/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      559 2022-07-25 12:26:23.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      391 2023-05-22 11:15:00.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/converter/convert_ndarray_to_list.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      809 2023-07-22 15:47:27.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/converter/escape_non_str_dict_key.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      605 2023-07-22 16:02:29.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/converter/escape_tuple.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      377 2023-05-22 11:15:00.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/converter/integrate.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      808 2023-07-22 16:14:24.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/converter/unescape_non_str_dict_key.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      661 2023-07-22 16:14:24.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/converter/unescape_tuple.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1784 2023-07-24 07:20:15.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/read_json.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2386 2023-07-25 10:44:52.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/write_json.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2023-02-08 07:16:46.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3621 2022-11-16 07:31:34.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/converter.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8071 2023-06-21 01:55:22.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16285 2023-06-21 00:22:15.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      447 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/read.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-30 14:12:33.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/test/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-08-01 07:19:40.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      324 2022-08-01 07:19:40.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_0.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      249 2022-08-01 07:22:27.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/test/test_data/data_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     6838 2023-06-21 00:15:01.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      556 2023-06-21 00:11:28.000000 kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/write.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-08 10:14:56.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/decorator/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       66 2022-02-08 10:15:24.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/decorator/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      399 2022-02-08 06:57:21.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/decorator/restore_original_work_path.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       20 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/producer_consumer/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       28 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/producer_consumer/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      892 2022-12-12 08:39:00.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3164 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       50 2022-04-18 11:35:30.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/producer_consumer/getter.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      740 2022-04-18 12:49:09.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2299 2022-04-18 12:23:06.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/producer_consumer/node.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-04-18 08:15:52.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/producer_consumer/producer.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       51 2022-04-18 10:40:32.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/producer_consumer/sender.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/singleton/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-04-18 13:24:36.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/singleton/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3803 2023-06-12 12:14:03.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2089 2022-02-28 06:54:56.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/general_matrix_multiplication.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/numerical_characteristics/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-02 05:01:47.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/numerical_characteristics/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2953 2022-06-02 05:03:41.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/numerical_characteristics/iou.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/temperate/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      630 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/temperate/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      213 2022-03-10 05:06:13.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/temperate/iterator_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1663 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/temperate/my_iterator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1214 2022-03-10 05:06:13.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/temperate/my_iterator_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      217 2022-03-10 05:06:13.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/temperate/sequence_map_base.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      241 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/developing/test.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/env_info/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-03-30 13:18:27.000000 kevin-toolbox-1.1.6/kevin_toolbox/env_info/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      879 2023-04-10 12:53:17.000000 kevin-toolbox-1.1.6/kevin_toolbox/env_info/check_validity_and_uninstall.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1953 2023-06-21 01:55:26.000000 kevin-toolbox-1.1.6/kevin_toolbox/env_info/check_version_and_update.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/env_info/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-30 12:51:50.000000 kevin-toolbox-1.1.6/kevin_toolbox/env_info/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1728 2023-04-13 07:53:17.000000 kevin-toolbox-1.1.6/kevin_toolbox/env_info/test/test_version.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/env_info/version/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      187 2023-03-30 13:11:22.000000 kevin-toolbox-1.1.6/kevin_toolbox/env_info/version/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2489 2023-04-13 07:51:40.000000 kevin-toolbox-1.1.6/kevin_toolbox/env_info/version/compare_version.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      860 2023-04-13 07:46:23.000000 kevin-toolbox-1.1.6/kevin_toolbox/env_info/version/parse_version.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2458 2023-03-30 13:11:22.000000 kevin-toolbox-1.1.6/kevin_toolbox/env_info/version/sort_version_ls.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-05 07:35:48.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      650 2023-03-24 10:03:29.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/__old_version/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-24 10:03:09.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/__old_version/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2564 2023-03-24 09:28:54.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5701 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      305 2023-03-24 09:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/cal_area_of_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3079 2023-05-16 14:16:04.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8249 2022-08-01 13:19:11.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      836 2022-08-01 11:47:43.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/detect_collision.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2762 2022-07-06 13:18:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8255 2023-05-16 11:51:25.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8634 2023-06-21 01:55:28.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/detect_overlap.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      292 2022-07-05 08:41:47.000000 kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/get_ticks_of_boxes.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-28 06:47:25.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-10 07:21:33.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-14 08:37:13.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/analysis/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2022-09-28 09:26:13.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/analysis/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4714 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/dummy/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       54 2022-02-28 08:44:35.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/dummy/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     7137 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      259 2022-09-26 09:52:59.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      896 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1858 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    17766 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/factory.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      299 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4480 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3482 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4799 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5480 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      224 2022-03-13 18:22:06.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3114 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3773 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      170 2022-03-10 12:36:00.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/merge.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 04:21:21.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/binary_classification/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      427 2022-02-22 06:22:25.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/binary_classification/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2022-02-21 13:29:08.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3247 2022-02-22 06:22:25.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5319 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3355 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      891 2022-04-28 12:02:07.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      442 2022-02-22 05:39:00.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/convert.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3661 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-07-27 07:16:21.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-03 13:07:44.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/concat_and_split/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      157 2022-08-08 08:06:40.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/concat_and_split/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    23861 2023-06-14 03:08:32.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4997 2022-08-08 08:19:17.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3066 2022-08-08 08:19:17.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      232 2023-03-13 06:47:47.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/convert/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       43 2023-03-13 06:47:47.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/convert/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4972 2023-03-10 14:11:22.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/generate/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      264 2023-03-13 06:47:47.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/generate/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3380 2023-03-13 06:48:36.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5738 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4426 2022-07-29 07:53:01.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1373 2023-03-10 13:56:45.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/reshape/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      220 2022-07-25 13:28:44.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/reshape/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1946 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1064 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/reshape/merge_blocks.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1236 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/reshape/split_blocks.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1859 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/transpose/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      177 2022-05-31 10:43:01.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/transpose/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      611 2022-08-09 13:17:49.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1472 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/number_theory/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      182 2023-03-05 15:57:35.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/number_theory/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      244 2023-03-05 15:45:13.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/number_theory/cache.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      387 2023-03-05 15:57:35.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/number_theory/get_greatest_common_divisor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      949 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/number_theory/get_primes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      499 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/number_theory/prime_factorization.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/number_theory/test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-06 07:12:06.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/number_theory/test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      747 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      784 2023-03-31 07:27:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/number_theory/test/test_get_primes.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      551 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/number_theory/test/test_prime_factorization.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/transform/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-06-10 08:52:28.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/transform/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/transform/dct/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      147 2022-07-22 13:25:44.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/transform/dct/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     8296 2023-03-31 07:27:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/transform/dct/dct_calculator.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4305 2022-07-20 12:21:16.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/transform/scaling_and_shift/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       29 2022-07-30 13:19:40.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/transform/scaling_and_shift/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1280 2022-07-30 13:48:26.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/transform/scaling_and_shift/scaling.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/utils/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      289 2023-04-21 12:36:14.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/utils/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1943 2022-08-09 12:09:28.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/utils/convert_dtype.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1620 2022-08-08 08:50:02.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/utils/get_crop_by_box.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1553 2022-08-02 12:15:03.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1775 2022-08-08 08:50:02.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/utils/set_crop_by_box.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      345 2023-05-30 12:44:28.000000 kevin-toolbox-1.1.6/kevin_toolbox/math/utils/spilt_integer_most_evenly.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-03-29 13:28:32.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_matplotlib/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      127 2023-03-10 08:30:36.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_matplotlib/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1837 2023-03-10 10:16:48.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1696 2023-03-10 09:17:25.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1361 2023-03-10 08:13:57.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_matplotlib/arrow3d.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_numpy/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-04-24 08:38:24.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_numpy/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_numpy/linalg/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       99 2023-04-24 08:58:58.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_numpy/linalg/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      423 2023-05-17 07:05:16.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_numpy/linalg/cos_similar.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      625 2023-04-24 08:52:01.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_numpy/linalg/normalize.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      253 2023-04-24 08:55:02.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_numpy/linalg/softmax.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_optuna/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       69 2023-05-26 09:14:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_optuna/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     4588 2023-05-26 09:40:56.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_os/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       77 2023-07-21 09:36:08.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_os/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      656 2023-07-21 09:38:57.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_os/pack.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      658 2023-04-17 12:51:37.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_os/remove.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1047 2023-07-21 09:40:06.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_os/unpack.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_test/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       49 2022-07-29 06:55:38.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_test/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     3184 2023-06-26 08:43:44.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_test/check_consistency.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2022-02-21 06:56:01.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/__init__.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       75 2023-03-08 07:01:29.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      393 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/concat.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/linalg/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       44 2023-03-08 08:04:27.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/linalg/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      770 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      575 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/nn/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       35 2023-05-30 11:36:55.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/nn/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     5357 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      845 2023-04-12 15:31:18.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/tile.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-04-12 15:36:21.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/where.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/math/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       68 2022-02-21 09:51:39.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/math/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     2047 2022-02-22 06:43:43.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/math/get_y_at_x.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1378 2022-02-21 09:44:44.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/math/my_around.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/nn/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       39 2023-05-30 11:37:07.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/nn/__init__.py
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      223 2023-05-29 08:32:26.000000 kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/nn/lambda_layer.py
+drwxr-xr-x   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        0 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox.egg-info/
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)     1420 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)    16058 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)        1 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       92 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox.egg-info/requires.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       14 2023-07-25 12:34:04.000000 kevin-toolbox-1.1.6/kevin_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)       59 2023-03-31 06:32:36.000000 kevin-toolbox-1.1.6/pyproject.toml
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      904 2023-07-25 12:34:05.000000 kevin-toolbox-1.1.6/setup.cfg
+-rw-r--r--   0 SENSETIME\xukaiming (840487534) SENSETIME\domain^users (840434177)      733 2023-03-31 07:25:47.000000 kevin-toolbox-1.1.6/setup.py
```

### Comparing `kevin-toolbox-1.1.5/PKG-INFO` & `kevin-toolbox-1.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevin-toolbox
-Version: 1.1.5
+Version: 1.1.6
 Summary: 一个常用的工具代码包集合
 Home-page: https://github.com/cantbeblank96/kevin_toolbox
 Download-URL: https://github.com/username/your-package/archive/refs/tags/v1.0.0.tar.gz
 Author: kevin hsu
 Author-email: xukaiming1996@163.com
 License: MIT
 Keywords: mathematics,pytorch,numpy,machine-learning,algorithm
@@ -41,11 +41,12 @@
 
 [使用指南 User_Guide](./notes/User_Guide.md)
 
 [免责声明 Disclaimer](./notes/Disclaimer.md)
 
 [版本更新记录](./notes/Release_Record.md)：
 
-- v 1.1.5（2023-07-24）【bug fix】
-  - data_flow.file.json_【bug fix】
-    - fix bug in write()，修复了 b_use_suggested_converter 参数引起的报错
-    - 添加了测试用例
+- v 1.1.6（2023-07-25）【bug fix】
+  - computer_science.algorithm.for_nested_dict_list【bug fix】
+    - fix bug in traverse()，修复了对于 dict 中 int 的键无法正确返回名称的 bug。添加了相应测试用例。
+  - data_flow.file.json_
+    - modify write()，支持 file_path 参数设置为 None 来直接获取序列化结果而非写入到具体文件中。
```

### Comparing `kevin-toolbox-1.1.5/README.md` & `kevin-toolbox-1.1.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -23,11 +23,12 @@
 
 [使用指南 User_Guide](./notes/User_Guide.md)
 
 [免责声明 Disclaimer](./notes/Disclaimer.md)
 
 [版本更新记录](./notes/Release_Record.md)：
 
-- v 1.1.5（2023-07-24）【bug fix】
-  - data_flow.file.json_【bug fix】
-    - fix bug in write()，修复了 b_use_suggested_converter 参数引起的报错
-    - 添加了测试用例
+- v 1.1.6（2023-07-25）【bug fix】
+  - computer_science.algorithm.for_nested_dict_list【bug fix】
+    - fix bug in traverse()，修复了对于 dict 中 int 的键无法正确返回名称的 bug。添加了相应测试用例。
+  - data_flow.file.json_
+    - modify write()，支持 file_path 参数设置为 None 来直接获取序列化结果而非写入到具体文件中。
```

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/get_subset_with_largest_product.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_get_subset_with_largest_product.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/test/test_zero_one_knapsack_problem.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/combinatorial_optimization/zero_one_knapsack_problem.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_dict/deep_update.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/copy_.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/copy_.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/count_leaf_node_nums.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/count_leaf_node_nums.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_hash.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_hash.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_nodes.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_nodes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_value_by_name.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/get_value_by_name.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/build_name.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/build_name.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/escape_node.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/escape_node.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/parse_name.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/parse_name.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_json_.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_numpy_bin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 import os
-import json
-from kevin_toolbox.data_flow.file import json_
-from kevin_toolbox.data_flow.file.json_.converter import escape_non_str_dict_key, unescape_non_str_dict_key, \
-    escape_tuple, unescape_tuple
+import numpy as np
 from kevin_toolbox.computer_science.algorithm.for_nested_dict_list.serializer.backends import Backend_Base
 from kevin_toolbox.computer_science.algorithm.for_nested_dict_list.serializer.variable import SERIALIZER_BACKEND
 
 
 @SERIALIZER_BACKEND.register()
-class Json_(Backend_Base):
-    name = ":json"
+class Numpy_Bin(Backend_Base):
+    name = ":numpy:bin"
 
     def write(self, name, var, **kwargs):
         assert self.writable(var=var)
 
-        json_.write(content=var, file_path=os.path.join(self.paras["folder"], f'{name}.json'),
-                    sort_keys=False, converters=[escape_non_str_dict_key, escape_tuple])
-        return dict(backend=Json_.name, name=name)
+        var.tofile(os.path.join(self.paras["folder"], f'{name}.bin'))
+        details = dict(shape=list(var.shape), dtype=f'{var.dtype}')
+        return dict(backend=Numpy_Bin.name, name=name, details=details)
 
     def read(self, name, **kwargs):
         assert self.readable(name=name)
+        details = kwargs["details"]
 
-        var = json_.read(file_path=os.path.join(self.paras["folder"], f'{name}.json'),
-                         converters=[unescape_non_str_dict_key, unescape_tuple])
+        var = np.fromfile(os.path.join(self.paras["folder"], f'{name}.bin'))
+        var = var.astype(np.dtype(details["dtype"]))
+        var.resize(details["shape"])
         return var
 
     def writable(self, var, **kwargs):
         """
             是否可以写
         """
-        try:
-            _ = json.dumps(var)
-            return True
-        except:
-            return False
+        return type(var) is np.ndarray or isinstance(var, (np.bool_, np.number, np.flexible))
 
     def readable(self, name, **kwargs):
         """
             是否可以写
         """
-        return os.path.isfile(os.path.join(self.paras["folder"], f'{name}.json'))
+        return os.path.isfile(os.path.join(self.paras["folder"], f'{name}.bin'))
 
 
 if __name__ == '__main__':
-    backend = Json_(folder=os.path.join(os.path.dirname(__file__), "temp"))
+    backend = Numpy_Bin(folder=os.path.join(os.path.dirname(__file__), "temp"))
 
-    var_ = [{123: 123, None: None, "<eval>233": 233, "foo": (2, 3, 4)}, 233]
-    print(backend.write(name=":inst", var=var_))
+    a = np.random.randn(100, 2)
+    res = backend.write(name=":a:b", var=a)
+    print(res)
 
-    b = backend.read(name=":inst")
+    b = backend.read(**res)
     print(b)
```

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_numpy_bin.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_numpy_npy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 import os
 import numpy as np
 from kevin_toolbox.computer_science.algorithm.for_nested_dict_list.serializer.backends import Backend_Base
 from kevin_toolbox.computer_science.algorithm.for_nested_dict_list.serializer.variable import SERIALIZER_BACKEND
 
 
 @SERIALIZER_BACKEND.register()
-class Numpy_Bin(Backend_Base):
-    name = ":numpy:bin"
+class Numpy_Npy(Backend_Base):
+    name = ":numpy:npy"
 
     def write(self, name, var, **kwargs):
         assert self.writable(var=var)
 
-        var.tofile(os.path.join(self.paras["folder"], f'{name}.bin'))
+        np.save(os.path.join(self.paras["folder"], f'{name}.npy'), var)
         details = dict(shape=list(var.shape), dtype=f'{var.dtype}')
-        return dict(backend=Numpy_Bin.name, name=name, details=details)
+        return dict(backend=Numpy_Npy.name, name=name, details=details)
 
     def read(self, name, **kwargs):
         assert self.readable(name=name)
-        details = kwargs["details"]
 
-        var = np.fromfile(os.path.join(self.paras["folder"], f'{name}.bin'))
-        var.astype(np.dtype(details["dtype"])).resize(details["shape"])
+        var = np.load(os.path.join(self.paras["folder"], f'{name}.npy'))
         return var
 
     def writable(self, var, **kwargs):
         """
             是否可以写
         """
-        return type(var) is np.ndarray or isinstance(var, (np.bool_, np.number, np.flexible))
+        return isinstance(var, (np.generic, np.ndarray))
 
     def readable(self, name, **kwargs):
         """
             是否可以写
         """
-        return os.path.isfile(os.path.join(self.paras["folder"], f'{name}.bin'))
+        return os.path.isfile(os.path.join(self.paras["folder"], f'{name}.npy'))
 
 
 if __name__ == '__main__':
-    backend = Numpy_Bin(folder=os.path.join(os.path.dirname(__file__), "temp"))
+    print(SERIALIZER_BACKEND.database)
+    backend = Numpy_Npy(folder=os.path.join(os.path.dirname(__file__), "temp"))
 
     a = np.random.randn(100, 2)
     res = backend.write(name=":a:b", var=a)
     print(res)
 
     b = backend.read(**res)
     print(b)
+
+    print(SERIALIZER_BACKEND.database)
```

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_numpy_npy.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_pickle_.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 import os
-import numpy as np
+import pickle
 from kevin_toolbox.computer_science.algorithm.for_nested_dict_list.serializer.backends import Backend_Base
 from kevin_toolbox.computer_science.algorithm.for_nested_dict_list.serializer.variable import SERIALIZER_BACKEND
 
 
 @SERIALIZER_BACKEND.register()
-class Numpy_Npy(Backend_Base):
-    name = ":numpy:npy"
+class Pickle_(Backend_Base):
+    name = ":pickle"
 
     def write(self, name, var, **kwargs):
         assert self.writable(var=var)
 
-        np.save(os.path.join(self.paras["folder"], f'{name}.npy'), var)
-        details = dict(shape=list(var.shape), dtype=f'{var.dtype}')
-        return dict(backend=Numpy_Npy.name, name=name, details=details)
+        with open(os.path.join(self.paras["folder"], f'{name}.pkl'), 'wb') as f:
+            pickle.dump(var, f)
+        return dict(backend=Pickle_.name, name=name)
 
     def read(self, name, **kwargs):
         assert self.readable(name=name)
 
-        var = np.load(os.path.join(self.paras["folder"], f'{name}.npy'))
+        with open(os.path.join(self.paras["folder"], f'{name}.pkl'), 'rb') as f:
+            var = pickle.load(f)
         return var
 
     def writable(self, var, **kwargs):
         """
             是否可以写
         """
-        return isinstance(var, (np.generic, np.ndarray))
+        return True
 
     def readable(self, name, **kwargs):
         """
             是否可以写
         """
-        return os.path.isfile(os.path.join(self.paras["folder"], f'{name}.npy'))
+        return os.path.isfile(os.path.join(self.paras["folder"], f'{name}.pkl'))
 
 
 if __name__ == '__main__':
-    print(SERIALIZER_BACKEND.database)
-    backend = Numpy_Npy(folder=os.path.join(os.path.dirname(__file__), "temp"))
+    import torch
+    backend = Pickle_(folder=os.path.join(os.path.dirname(__file__), "temp"))
 
-    a = np.random.randn(100, 2)
-    res = backend.write(name=":a:b", var=a)
-    print(res)
+    a = torch.randn(100, device=torch.device("cuda"))
+    print(backend.write(name=":a:b", var=a))
 
-    b = backend.read(**res)
+    b = backend.read(name=":a:b")
     print(b)
-
-    print(SERIALIZER_BACKEND.database)
```

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_pickle_.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_skip_all.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-import os
-import pickle
 from kevin_toolbox.computer_science.algorithm.for_nested_dict_list.serializer.backends import Backend_Base
 from kevin_toolbox.computer_science.algorithm.for_nested_dict_list.serializer.variable import SERIALIZER_BACKEND
 
 
-@SERIALIZER_BACKEND.register()
-class Pickle_(Backend_Base):
-    name = ":pickle"
+@SERIALIZER_BACKEND.register(name=":skip:all")
+class Skip_All(Backend_Base):
 
     def write(self, name, var, **kwargs):
-        assert self.writable(var=var)
-
-        with open(os.path.join(self.paras["folder"], f'{name}.pkl'), 'wb') as f:
-            pickle.dump(var, f)
-        return dict(backend=Pickle_.name, name=name)
+        return var
 
     def read(self, name, **kwargs):
-        assert self.readable(name=name)
-
-        with open(os.path.join(self.paras["folder"], f'{name}.pkl'), 'rb') as f:
-            var = pickle.load(f)
-        return var
+        raise Exception(f'calling skip.read() is prohibited')
 
     def writable(self, var, **kwargs):
         """
             是否可以写
         """
         return True
 
     def readable(self, name, **kwargs):
         """
             是否可以写
         """
-        return os.path.isfile(os.path.join(self.paras["folder"], f'{name}.pkl'))
+        return False
 
 
 if __name__ == '__main__':
-    import torch
-    backend = Pickle_(folder=os.path.join(os.path.dirname(__file__), "temp"))
+    import os
+
+    backend = Skip_All(folder=os.path.join(os.path.dirname(__file__), "temp"))
 
-    a = torch.randn(100, device=torch.device("cuda"))
+    a = 100
     print(backend.write(name=":a:b", var=a))
 
     b = backend.read(name=":a:b")
     print(b)
```

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_skip_all.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_skip_simple.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from kevin_toolbox.computer_science.algorithm.for_nested_dict_list.serializer.backends import Backend_Base
 from kevin_toolbox.computer_science.algorithm.for_nested_dict_list.serializer.variable import SERIALIZER_BACKEND
 
 
-@SERIALIZER_BACKEND.register(name=":skip:all")
-class Skip_All(Backend_Base):
+@SERIALIZER_BACKEND.register(name=":skip:simple")
+class Skip_Simple(Backend_Base):
 
     def write(self, name, var, **kwargs):
+        assert self.writable(var=var)
         return var
 
     def read(self, name, **kwargs):
         raise Exception(f'calling skip.read() is prohibited')
 
     def writable(self, var, **kwargs):
         """
             是否可以写
         """
-        return True
+        return isinstance(var, (int, float, str, tuple))
 
     def readable(self, name, **kwargs):
         """
             是否可以写
         """
         return False
 
 
 if __name__ == '__main__':
     import os
 
-    backend = Skip_All(folder=os.path.join(os.path.dirname(__file__), "temp"))
+    backend = Skip_Simple(folder=os.path.join(os.path.dirname(__file__), "temp"))
 
     a = 100
     print(backend.write(name=":a:b", var=a))
 
     b = backend.read(name=":a:b")
     print(b)
```

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_skip_simple.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_torch_tensor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,45 @@
+import os
+import torch
 from kevin_toolbox.computer_science.algorithm.for_nested_dict_list.serializer.backends import Backend_Base
 from kevin_toolbox.computer_science.algorithm.for_nested_dict_list.serializer.variable import SERIALIZER_BACKEND
 
 
-@SERIALIZER_BACKEND.register(name=":skip:simple")
-class Skip_Simple(Backend_Base):
+@SERIALIZER_BACKEND.register()
+class Torch_Tensor(Backend_Base):
+    name = ":torch:tensor"
 
     def write(self, name, var, **kwargs):
-        return var
+        assert self.writable(var=var)
+
+        torch.save(var, os.path.join(self.paras["folder"], f'{name}.pt'))
+        details = dict(shape=list(var.shape), device=var.device.type, dtype=f'{var.dtype}')
+        return dict(backend=Torch_Tensor.name, name=name, details=details)
 
     def read(self, name, **kwargs):
-        raise Exception(f'calling skip.read() is prohibited')
+        assert self.readable(name=name)
+
+        return torch.load(os.path.join(self.paras["folder"], f'{name}.pt'))
 
     def writable(self, var, **kwargs):
         """
             是否可以写
         """
-        return isinstance(var, (int, float, str, tuple))
+        return torch.is_tensor(var)
 
     def readable(self, name, **kwargs):
         """
             是否可以写
         """
-        return False
+        return os.path.isfile(os.path.join(self.paras["folder"], f'{name}.pt'))
 
 
 if __name__ == '__main__':
-    import os
+    backend = Torch_Tensor(folder=os.path.join(os.path.dirname(__file__), "temp"))
 
-    backend = Skip_Simple(folder=os.path.join(os.path.dirname(__file__), "temp"))
-
-    a = 100
+    a = torch.randn(100, device=torch.device("cuda"))
     print(backend.write(name=":a:b", var=a))
 
     b = backend.read(name=":a:b")
     print(b)
+
+    print(SERIALIZER_BACKEND.database)
```

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_torch_all.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_torch_all.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/backend_base.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/backend_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/write.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/write.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import time
 import warnings
 import kevin_toolbox
 from kevin_toolbox.data_flow.file import json_
-from kevin_toolbox.data_flow.file.json_.converter import escape_non_str_dict_key, escape_tuple
 from kevin_toolbox.patches import for_os
-from kevin_toolbox.computer_science.algorithm import for_nested_dict_list as fndl
+from kevin_toolbox.computer_science.algorithm import for_nested_dict_list as ndl
 from kevin_toolbox.computer_science.algorithm.for_nested_dict_list.serializer.variable import SERIALIZER_BACKEND
 
 
 def write(var, output_dir, settings, traversal_mode="bfs", b_pack_into_tar=True, **kwargs):
     """
         将输入的嵌套字典列表 var 的结构和节点值保存到文件中
             遍历 var，匹配并使用 settings 中设置的保存方式来对各部分结构/节点进行序列化
@@ -77,31 +76,31 @@
 
     # 构建 processed_s
     #     为了避免重复处理节点/结构，首先构建与 var 具有相似结构的 processed_s 来记录处理处理进度。
     #     对于 processed_s，其节点值为 True 时表示该节点已经被处理，当节点值为 False 或者 list/dict 类型时表示该节点或者节点下面的结构中仍然
     #       存在未处理的部分。
     #     对于中间节点，只有其下所有叶节点都未处理时才会被匹配。
     processed_s = dict()
-    for n, _ in fndl.get_nodes(var=var, level=-1, b_strict=True):
-        fndl.set_value_by_name(var=processed_s, name=n, value=False, b_force=True)
+    for n, _ in ndl.get_nodes(var=var, level=-1, b_strict=True):
+        ndl.set_value_by_name(var=processed_s, name=n, value=False, b_force=True)
     # processed_s_bak 用于记录 var 的原始结构
-    processed_s_bak = fndl.copy_(var=processed_s, b_deepcopy=True)
+    processed_s_bak = ndl.copy_(var=processed_s, b_deepcopy=True)
 
     # 处理 var
     backend_s = dict()
     for setting in settings:
         # match_cond
         if isinstance(setting["match_cond"], str) and setting["match_cond"].startswith("<eval>"):
             setting["match_cond"] = eval(setting["match_cond"][6:])
         assert callable(setting["match_cond"]) or isinstance(setting["match_cond"], str)
         # backend
         backend_name_ls = setting["backend"] if isinstance(setting["backend"], (list, tuple)) else [setting["backend"]]
         for i in backend_name_ls:
             if i not in backend_s:
-                backend_s[i] = SERIALIZER_BACKEND.get(name=i)(folder=output_dir)
+                backend_s[i] = SERIALIZER_BACKEND.get(name=i)(folder=os.path.join(output_dir, "nodes"))
         # _process and  paras
         if callable(setting["match_cond"]):
             if setting.get("traversal_mode", traversal_mode) in ("dfs_pre_order", "bfs"):
                 _process = _process_from_top_to_down
             else:
                 _process = _process_from_down_to_top
             paras = dict(
@@ -125,73 +124,71 @@
             print(f'backend: {i}')
             _process(backend=backend_s[i], **paras)
 
     print(processed_s)
     print(var)
 
     b_processed_all = True
-    for n, v in fndl.get_nodes(var=processed_s, level=-1):
+    for n, v in ndl.get_nodes(var=processed_s, level=-1):
         if not v:
             warnings.warn(
                 message=f'node {n} failed to write',
                 category=UserWarning
             )
             b_processed_all = False
     assert b_processed_all, \
         f'please check settings to make sure all nodes have been covered and can be deal with backend'
 
     # 保存 var 的结构
-    json_.write(content=var, file_path=os.path.join(output_dir, "var.json"),
-                converters=[escape_non_str_dict_key, escape_tuple])
+    json_.write(content=var, file_path=os.path.join(output_dir, "var.json"), b_use_suggested_converter=True)
     # 保存处理结果（非必要）
     json_.write(content=dict(processed=processed_s, raw_structure=processed_s_bak, timestamp=time.time(),
                              kt_version=kevin_toolbox.__version__),
-                file_path=os.path.join(output_dir, "record.json"),
-                converters=[escape_non_str_dict_key, escape_tuple])
+                file_path=os.path.join(output_dir, "record.json"), b_use_suggested_converter=True)
 
     # 打包成 .tar 文件
     if b_pack_into_tar:
         for_os.pack(source=output_dir)
         for_os.remove(path=output_dir, ignore_errors=True)
 
 
 def _judge_processed_or_not(processed_s, name):
     """
         如 name 所指向的节点已经被处理，或者节点下的部分含有已经处理的子节点，则返回 True
     """
-    b_processed = fndl.get_value_by_name(var=processed_s, name=name, b_pop=False, default=True)
+    b_processed = ndl.get_value_by_name(var=processed_s, name=name, b_pop=False, default=True)
     if not isinstance(b_processed, bool):
         # 需要查清楚下面子节点是否存在未处理的部分
-        for n, v in fndl.get_nodes(var=b_processed, level=-1, b_strict=True):
+        for n, v in ndl.get_nodes(var=b_processed, level=-1, b_strict=True):
             if v:
                 b_processed = True
                 break
         else:
             b_processed = False
     return b_processed
 
 
 def _process_for_level(var, processed_s, processed_s_bak, level, backend):
-    for name, _ in fndl.get_nodes(var=processed_s_bak, level=level, b_strict=True):
+    for name, _ in ndl.get_nodes(var=processed_s_bak, level=level, b_strict=True):
         _process_for_name(var=var, processed_s=processed_s, name=name, backend=backend)
 
 
 def _process_for_name(var, processed_s, name, backend):
     if _judge_processed_or_not(processed_s=processed_s, name=name) is True:
         # has been processed
         return
-    value = fndl.get_value_by_name(var=var, name=name, b_pop=False)
+    value = ndl.get_value_by_name(var=var, name=name, b_pop=False)
     if not backend.writable(var=value):
         # cannot be written by backend
         return
 
     # write by backend
     res = backend.write(name=name, var=value)
-    fndl.set_value_by_name(var=processed_s, name=name, value=True, b_force=False)
-    fndl.set_value_by_name(var=var, name=name, value=res, b_force=False)
+    ndl.set_value_by_name(var=processed_s, name=name, value=True, b_force=False)
+    ndl.set_value_by_name(var=var, name=name, value=res, b_force=False)
 
 
 def _process_from_top_to_down(var, processed_s, match_cond, backend, traversal_mode):
     def match_cond_(parent_type, idx, value):
         nonlocal match_cond, processed_s
 
         b_processed = _judge_processed_or_not(processed_s=processed_s, name=idx)
@@ -202,46 +199,46 @@
         return match_cond(parent_type, idx, value)
 
     def converter(idx, value):
         nonlocal processed_s, backend
 
         # write by backend
         res = backend.write(name=idx, var=value)
-        fndl.set_value_by_name(var=processed_s, name=idx, value=True, b_force=True)
+        ndl.set_value_by_name(var=processed_s, name=idx, value=True, b_force=True)
         return res
 
-    fndl.traverse(var=var, match_cond=match_cond_, action_mode="replace", converter=converter,
-                  b_use_name_as_idx=True, traversal_mode=traversal_mode, b_traverse_matched_element=False)
+    ndl.traverse(var=var, match_cond=match_cond_, action_mode="replace", converter=converter,
+                 b_use_name_as_idx=True, traversal_mode=traversal_mode, b_traverse_matched_element=False)
 
 
 def _process_from_down_to_top(var, processed_s, match_cond, backend, traversal_mode):
-    processed_s_raw, processed_s = processed_s, fndl.copy_(var=processed_s, b_deepcopy=True)
+    processed_s_raw, processed_s = processed_s, ndl.copy_(var=processed_s, b_deepcopy=True)
 
     def match_cond_(parent_type, idx, value):
         nonlocal match_cond, processed_s
 
         b_processed = _judge_processed_or_not(processed_s=processed_s, name=idx)
-        fndl.set_value_by_name(var=processed_s, name=idx, value=b_processed, b_force=False)
+        ndl.set_value_by_name(var=processed_s, name=idx, value=b_processed, b_force=False)
         if b_processed is True or not backend.writable(var=value):
             # has been processed or cannot be written by backend
             return False
 
         return match_cond(parent_type, idx, value)
 
     def converter(idx, value):
         nonlocal processed_s, backend, processed_s_raw
 
         # write by backend
         res = backend.write(name=idx, var=value)
-        fndl.set_value_by_name(var=processed_s, name=idx, value=True, b_force=True)
-        fndl.set_value_by_name(var=processed_s_raw, name=idx, value=True, b_force=True)
+        ndl.set_value_by_name(var=processed_s, name=idx, value=True, b_force=True)
+        ndl.set_value_by_name(var=processed_s_raw, name=idx, value=True, b_force=True)
         return res
 
-    fndl.traverse(var=var, match_cond=match_cond_, action_mode="replace", converter=converter,
-                  b_use_name_as_idx=True, traversal_mode=traversal_mode)
+    ndl.traverse(var=var, match_cond=match_cond_, action_mode="replace", converter=converter,
+                 b_use_name_as_idx=True, traversal_mode=traversal_mode)
 
 
 if __name__ == '__main__':
     import torch
     import numpy as np
     from kevin_toolbox.computer_science.algorithm.for_nested_dict_list import name_handler
```

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/set_value_by_name.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/set_value_by_name.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/traverse.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/traverse.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,13 +137,15 @@
         else:
             pass
     return b_matched, b_popped
 
 
 def _gen_idx(var, keys, b_use_name_as_idx, pre_name):
     if b_use_name_as_idx:
-        # TODO 对于 dict 中 int 的键，应该添加 @。添加相应测试用例
-        method = "@" if isinstance(var, list) else ":"
-        idx_ls = [f'{pre_name}{method}{escape_node(node=k, b_reversed=False, times=1)}' for k in keys]
+        idx_ls = []
+        for k in keys:
+            method = "@" if isinstance(var, list) or not isinstance(k, str) else ":"
+            k = escape_node(node=k, b_reversed=False, times=1)
+            idx_ls.append(f'{pre_name}{method}{k}')
     else:
         idx_ls = keys
     return idx_ls
```

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/cal_relation_between_references.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/cal_relation_between_references.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/eval_references.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/eval_references.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/parse_references.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_nested_dict_list/value_parser/parse_references.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/for_seq/flatten_list.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/locks/mutex_lock.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/pareto_front/get_pareto_points_idx.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/registration/registry.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/registration/registry.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/scheduler/strategy_manager.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/scheduler/trigger.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/scheduler/trigger.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/search/binary_search.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/search/binary_search.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/statistician/_init_var.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/statistician/_init_var.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/statistician/average_accumulator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/algorithm/statistician/exponential_moving_average.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/computer_science/data_structure/executor.py` & `kevin-toolbox-1.1.6/kevin_toolbox/computer_science/data_structure/executor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py` & `kevin-toolbox-1.1.6/kevin_toolbox/dangerous/dump_into_pickle_with_executor_attached.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/core/cache/cache_manager_for_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/core/reader/file_iterative_reader.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/core/reader/unified_reader.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/core/reader/unified_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from kevin_toolbox.data_flow.core.reader import Unified_Reader_Base, File_Iterative_Reader
 
 
 class UReader(Unified_Reader_Base):
-    def __index__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
 
     def get_file_iterative_reader(self, file_path, chunk_size, **kwargs):
         return super().get_file_iterative_reader(file_path, chunk_size, **kwargs)
 
     def get_cache_manager(self, iterator, folder_path):
         return super().get_cache_manager(iterator, folder_path)
```

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/core/reader/unified_reader_base.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/core/reader/unified_reader_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/converter/convert_dict_key_to_number.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/converter/escape_non_str_dict_key.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/converter/escape_non_str_dict_key.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/converter/escape_tuple.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/converter/escape_tuple.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/converter/unescape_non_str_dict_key.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/converter/unescape_non_str_dict_key.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/converter/unescape_tuple.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/converter/unescape_tuple.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/read_json.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/read_json.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/json_/write_json.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/json_/write_json.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,32 +7,40 @@
 
 def write_json(content, file_path, sort_keys=False, converters=None, b_use_suggested_converter=False):
     """
         写入 json file
 
         参数：
             content:                    待写入内容
-            file_path
+            file_path:                  <path or None> 写入路径
+                                            当设置为 None 时，将直接把（经converters处理后的）待写入内容作为结果返回，而不进行实际的写入
             sort_keys
             converters:                 <list of converters> 对写入内容中每个节点的处理方式
                                             转换器 converter 应该是一个形如 def(x): ... ; return x 的函数，具体可以参考
                                             json_.converter 中已实现的转换器
             b_use_suggested_converter:  <boolean> 是否使用建议的转换器
                                             建议使用 unescape/escape_non_str_dict_key 和 unescape/escape_tuple 这两对转换器，
                                             可以避免因 json 的读取/写入而丢失部分信息。
                                             默认为 False。
                     注意：当 converters 非 None，此参数失效，以 converters 中的具体设置为准
     """
-    file_path = os.path.abspath(file_path)
-    os.makedirs(os.path.dirname(file_path), exist_ok=True)
+    assert isinstance(file_path, (str, type(None)))
+
     if converters is None and b_use_suggested_converter:
         converters = [escape_tuple, escape_non_str_dict_key]
 
     if converters is not None:
         converter = integrate(converters)
         content = traverse(var=[copy.deepcopy(content)],
                            match_cond=lambda _, __, ___: True, action_mode="replace",
                            converter=lambda _, x: converter(x),
                            b_traverse_matched_element=True)[0]
 
-    with open(file_path, 'w') as f:
-        json.dump(content, f, indent=4, ensure_ascii=False, sort_keys=sort_keys)
+    content = json.dumps(content, indent=4, ensure_ascii=False, sort_keys=sort_keys)
+
+    if file_path is not None:
+        file_path = os.path.abspath(file_path)
+        os.makedirs(os.path.dirname(file_path), exist_ok=True)
+        with open(file_path, 'w') as f:
+            f.write(content)
+    else:
+        return content
```

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/converter.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/converter.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_reader.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/kevin_notation_writer.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/test/test_kevin_notation.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/data_flow/file/kevin_notation/write.py` & `kevin-toolbox-1.1.6/kevin_toolbox/data_flow/file/kevin_notation/write.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py` & `kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/producer_consumer/consumer.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py` & `kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/producer_consumer/for_cvf.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py` & `kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/producer_consumer/graph.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/producer_consumer/node.py` & `kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/producer_consumer/node.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py` & `kevin-toolbox-1.1.6/kevin_toolbox/developing/design_pattern/singleton/singleton_for_uid.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/developing/general_matrix_multiplication.py` & `kevin-toolbox-1.1.6/kevin_toolbox/developing/general_matrix_multiplication.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/developing/numerical_characteristics/iou.py` & `kevin-toolbox-1.1.6/kevin_toolbox/developing/numerical_characteristics/iou.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/developing/temperate/__init__.py` & `kevin-toolbox-1.1.6/kevin_toolbox/developing/temperate/__init__.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/developing/temperate/my_iterator.py` & `kevin-toolbox-1.1.6/kevin_toolbox/developing/temperate/my_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/developing/temperate/my_iterator_base.py` & `kevin-toolbox-1.1.6/kevin_toolbox/developing/temperate/my_iterator_base.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/env_info/check_validity_and_uninstall.py` & `kevin-toolbox-1.1.6/kevin_toolbox/env_info/check_validity_and_uninstall.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/env_info/check_version_and_update.py` & `kevin-toolbox-1.1.6/kevin_toolbox/env_info/check_version_and_update.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/env_info/test/test_version.py` & `kevin-toolbox-1.1.6/kevin_toolbox/env_info/test/test_version.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/env_info/version/compare_version.py` & `kevin-toolbox-1.1.6/kevin_toolbox/env_info/version/compare_version.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/env_info/version/parse_version.py` & `kevin-toolbox-1.1.6/kevin_toolbox/env_info/version/parse_version.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/env_info/version/sort_version_ls.py` & `kevin-toolbox-1.1.6/kevin_toolbox/env_info/version/sort_version_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/__init__.py` & `kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/__init__.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py` & `kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/__old_version/cal_iou_between_box.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py` & `kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/boolean_algebra_for_boxes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py` & `kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/cal_iou_between_boxes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py` & `kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/convert_boxes_from_coord_to_grid_index.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/detect_collision.py` & `kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/detect_collision.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py` & `kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/detect_collision_among_boxes_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py` & `kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/detect_collision_inside_boxes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/geometry/for_boxes/detect_overlap.py` & `kevin-toolbox-1.1.6/kevin_toolbox/geometry/for_boxes/detect_overlap.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/analysis/get_fail_case_from_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/dummy/dummy_data.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/build_generator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/build_iterator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/factory.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/factory.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_axis.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/along_diagonal.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_all.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/__by_block/of_triangle.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_block.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/dataset/face/verification/get_executor_ls/by_samples.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/accumulator_for_cfm.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_cfm_iteratively_by_chunk.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/cal_tpr_and_fpr.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py` & `kevin-toolbox-1.1.6/kevin_toolbox/machine_learning/statistician/binary_classification/confusion_matrices/merge_cfm_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/concat_and_split/computational_tree.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/concat_and_split/concat_crops_into_whole.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/concat_and_split/split_whole_into_crops.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/convert/convert_format.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/generate/generate_integrated_api.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/generate/generate_shuffled_index_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/generate/generate_z_pattern_indices_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/coordinates/generate/normal_indices_generator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/reshape/flatten_along_pattern.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/reshape/merge_blocks.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/reshape/merge_blocks.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/reshape/split_blocks.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/reshape/split_blocks.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/reshape/unflatten_along_pattern.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/transpose/get_inverse_of_transpose_index_ls.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/dimension/transpose/transpose_inside_axis.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/number_theory/get_primes.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/number_theory/get_primes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/number_theory/test/test_get_greatest_common_divisor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/number_theory/test/test_get_primes.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/number_theory/test/test_get_primes.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/number_theory/test/test_prime_factorization.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/number_theory/test/test_prime_factorization.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/transform/dct/dct_calculator.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/transform/dct/dct_calculator.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/transform/dct/generate_dct_trans_matrix.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/transform/scaling_and_shift/scaling.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/transform/scaling_and_shift/scaling.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/utils/convert_dtype.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/utils/convert_dtype.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/utils/get_crop_by_box.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/utils/get_crop_by_box.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/utils/get_function_table_for_array_and_tensor.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/math/utils/set_crop_by_box.py` & `kevin-toolbox-1.1.6/kevin_toolbox/math/utils/set_crop_by_box.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_matplotlib/add_trajectory_2d.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_matplotlib/add_trajectory_3d.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_matplotlib/arrow3d.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_matplotlib/arrow3d.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_numpy/linalg/normalize.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_numpy/linalg/normalize.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_optuna/sample_from_feasible_domain.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_os/pack.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_os/pack.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_os/remove.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_os/remove.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_os/unpack.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_os/unpack.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_test/check_consistency.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_test/check_consistency.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/linalg/norm.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/linalg/svd.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/nn/sequential.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/tile.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/tile.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/compatible/where.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/compatible/where.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/math/get_y_at_x.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/math/get_y_at_x.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox/patches/for_torch/math/my_around.py` & `kevin-toolbox-1.1.6/kevin_toolbox/patches/for_torch/math/my_around.py`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox.egg-info/PKG-INFO` & `kevin-toolbox-1.1.6/kevin_toolbox.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevin-toolbox
-Version: 1.1.5
+Version: 1.1.6
 Summary: 一个常用的工具代码包集合
 Home-page: https://github.com/cantbeblank96/kevin_toolbox
 Download-URL: https://github.com/username/your-package/archive/refs/tags/v1.0.0.tar.gz
 Author: kevin hsu
 Author-email: xukaiming1996@163.com
 License: MIT
 Keywords: mathematics,pytorch,numpy,machine-learning,algorithm
@@ -41,11 +41,12 @@
 
 [使用指南 User_Guide](./notes/User_Guide.md)
 
 [免责声明 Disclaimer](./notes/Disclaimer.md)
 
 [版本更新记录](./notes/Release_Record.md)：
 
-- v 1.1.5（2023-07-24）【bug fix】
-  - data_flow.file.json_【bug fix】
-    - fix bug in write()，修复了 b_use_suggested_converter 参数引起的报错
-    - 添加了测试用例
+- v 1.1.6（2023-07-25）【bug fix】
+  - computer_science.algorithm.for_nested_dict_list【bug fix】
+    - fix bug in traverse()，修复了对于 dict 中 int 的键无法正确返回名称的 bug。添加了相应测试用例。
+  - data_flow.file.json_
+    - modify write()，支持 file_path 参数设置为 None 来直接获取序列化结果而非写入到具体文件中。
```

### Comparing `kevin-toolbox-1.1.5/kevin_toolbox.egg-info/SOURCES.txt` & `kevin-toolbox-1.1.6/kevin_toolbox.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 kevin_toolbox/computer_science/algorithm/for_nested_dict_list/set_value_by_name.py
 kevin_toolbox/computer_science/algorithm/for_nested_dict_list/traverse.py
 kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/__init__.py
 kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/build_name.py
 kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/escape_node.py
 kevin_toolbox/computer_science/algorithm/for_nested_dict_list/name_handler/parse_name.py
 kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/__init__.py
-kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/load.py
+kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/read.py
 kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/variable.py
 kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/write.py
 kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/__init__.py
 kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_json_.py
 kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_numpy_bin.py
 kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_numpy_npy.py
 kevin_toolbox/computer_science/algorithm/for_nested_dict_list/serializer/backends/_pickle_.py
```

### Comparing `kevin-toolbox-1.1.5/setup.cfg` & `kevin-toolbox-1.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `kevin-toolbox-1.1.5/setup.py` & `kevin-toolbox-1.1.6/setup.py`

 * *Files identical despite different names*

