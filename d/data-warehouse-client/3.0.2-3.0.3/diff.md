# Comparing `tmp/data-warehouse-client-3.0.2.tar.gz` & `tmp/data-warehouse-client-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-warehouse-client-3.0.2.tar", last modified: Sun Apr  9 18:03:51 2023, max compression
+gzip compressed data, was "data-warehouse-client-3.0.3.tar", last modified: Wed Jul 26 20:11:53 2023, max compression
```

## Comparing `data-warehouse-client-3.0.2.tar` & `data-warehouse-client-3.0.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.669648 data-warehouse-client-3.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.661648 data-warehouse-client-3.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.661648 data-warehouse-client-3.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-09 18:03:51.669648 data-warehouse-client-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.665648 data-warehouse-client-3.0.2/data_warehouse_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/auto_generate_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/auto_generate_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/check_bounded_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/check_for_datetime_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/clone_study_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/csv_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    41274 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/data_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/delete_study_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18878 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/import_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    34701 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/import_with_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/load_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    44140 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/load_warehouse_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/multiple_mg_inserts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/print_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/print_metadata_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.669648 data-warehouse-client-3.0.2/data_warehouse_client/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_datetime_measurement_types_without_bounds.sql
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_datetimes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_integer_measurement_types_without_bounds.sql
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_integers.sql
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_real_measurement_types_without_bounds.sql
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_reals.sql
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/core_sql_from_for_measurements.sql
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/core_sql_select_for_measurements.sql
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_all_measurement_groups.sql
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_all_measurement_groups_and_types_in_a_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_all_table_names.sql
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_boundsdatetime_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_boundsint_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_boundsreal_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_categories_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_category_ids.sql
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_measurement_group_info.sql
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_measurement_groups_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_measurement_type_info.sql
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_measurements.sql
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_measurements_by_cohort.sql
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_measurements_with_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/get_units_in_study.sql
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/insert_datetime.sql
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/insert_measurement.sql
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/insert_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/measurements_lacking_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/measurements_with_invalid_category.sql
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/num_types_in_a_measurement_group.sql
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/ordinal_types_not_matching_category.sql
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/types_in_a_measurement_group.sql
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/sql/update_measurement_group_instance_id.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/study_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/study_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/table_reader_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/table_writer_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/transform_result_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/type_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/type_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/data_warehouse_client/warehouse_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.665648 data-warehouse-client-3.0.2/data_warehouse_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-09 18:03:51.000000 data-warehouse-client-3.0.2/data_warehouse_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-09 18:03:51.000000 data-warehouse-client-3.0.2/data_warehouse_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:03:51.000000 data-warehouse-client-3.0.2/data_warehouse_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-09 18:03:51.000000 data-warehouse-client-3.0.2/data_warehouse_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 18:03:51.000000 data-warehouse-client-3.0.2/data_warehouse_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.669648 data-warehouse-client-3.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   574842 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/docs/data_warehouse_guide.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.669648 data-warehouse-client-3.0.2/integration_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/integration_test/clone_study_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/integration_test/delete_study_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 18:03:51.669648 data-warehouse-client-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:51.669648 data-warehouse-client-3.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/test/test_file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-09 18:03:39.000000 data-warehouse-client-3.0.2/test/test_transform_result_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:53.857537 data-warehouse-client-3.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:53.841534 data-warehouse-client-3.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:53.845534 data-warehouse-client-3.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-26 20:11:53.853536 data-warehouse-client-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:53.849534 data-warehouse-client-3.0.3/data_warehouse_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/auto_generate_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/auto_generate_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/check_bounded_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/check_for_datetime_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/clone_study_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/csv_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41274 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/data_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/delete_study_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22213 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/import_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39969 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/import_with_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44140 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/load_warehouse_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/multiple_mg_inserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/print_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/print_metadata_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:53.853536 data-warehouse-client-3.0.3/data_warehouse_client/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/bounded_datetime_measurement_types_without_bounds.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/bounded_datetimes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/bounded_integer_measurement_types_without_bounds.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/bounded_integers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/bounded_real_measurement_types_without_bounds.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/bounded_reals.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/core_sql_from_for_measurements.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/core_sql_select_for_measurements.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/get_all_measurement_groups.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/get_all_measurement_groups_and_types_in_a_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/get_all_table_names.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/get_boundsdatetime_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/get_boundsint_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/get_boundsreal_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/get_categories_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/get_category_ids.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/get_measurement_group_info.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/get_measurement_groups_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/get_measurement_type_info.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/get_measurements.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/get_measurements_by_cohort.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/get_measurements_with_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/get_units_in_study.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/insert_datetime.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/insert_measurement.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/insert_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/measurements_lacking_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/measurements_with_invalid_category.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/num_types_in_a_measurement_group.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/ordinal_types_not_matching_category.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/types_in_a_measurement_group.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/sql/update_measurement_group_instance_id.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/study_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/study_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/table_reader_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/table_writer_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/transform_result_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/type_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/type_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/data_warehouse_client/warehouse_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:53.849534 data-warehouse-client-3.0.3/data_warehouse_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-26 20:11:53.000000 data-warehouse-client-3.0.3/data_warehouse_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-26 20:11:53.000000 data-warehouse-client-3.0.3/data_warehouse_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:11:53.000000 data-warehouse-client-3.0.3/data_warehouse_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-26 20:11:53.000000 data-warehouse-client-3.0.3/data_warehouse_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 20:11:53.000000 data-warehouse-client-3.0.3/data_warehouse_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:53.853536 data-warehouse-client-3.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   574842 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/docs/data_warehouse_guide.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:53.853536 data-warehouse-client-3.0.3/integration_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/integration_test/clone_study_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/integration_test/delete_study_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 20:11:53.857537 data-warehouse-client-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:53.853536 data-warehouse-client-3.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/test/test_file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-26 20:11:38.000000 data-warehouse-client-3.0.3/test/test_transform_result_format.py
```

### Comparing `data-warehouse-client-3.0.2/.github/workflows/build.yml` & `data-warehouse-client-3.0.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/.github/workflows/release.yml` & `data-warehouse-client-3.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/.gitignore` & `data-warehouse-client-3.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/LICENSE` & `data-warehouse-client-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/PKG-INFO` & `data-warehouse-client-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-warehouse-client
-Version: 3.0.2
+Version: 3.0.3
 Summary: This package provides access to the e-Science Central data warehouse that can be used to store, access and analyse data collected in scientific studies, including for healthcare applications
 Home-page: https://github.com/e-science-central/data-warehouse-client
 Author: Paul Watson
 Author-email: paul.watson@ncl.ac.uk
 License: UNKNOWN
 Description: # Data Warehouse Client
```

### Comparing `data-warehouse-client-3.0.2/README.md` & `data-warehouse-client-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/auto_generate_test_cases.py` & `data-warehouse-client-3.0.3/data_warehouse_client/auto_generate_test_cases.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/auto_generate_tests.py` & `data-warehouse-client-3.0.3/data_warehouse_client/auto_generate_tests.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/check_bounded_values.py` & `data-warehouse-client-3.0.3/data_warehouse_client/check_bounded_values.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/check_for_datetime_table.py` & `data-warehouse-client-3.0.3/data_warehouse_client/check_for_datetime_table.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/clone_study_metadata.py` & `data-warehouse-client-3.0.3/data_warehouse_client/clone_study_metadata.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/csv_io.py` & `data-warehouse-client-3.0.3/data_warehouse_client/csv_io.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/data_warehouse.py` & `data-warehouse-client-3.0.3/data_warehouse_client/data_warehouse.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/delete_study_contents.py` & `data-warehouse-client-3.0.3/data_warehouse_client/delete_study_contents.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/file_utils.py` & `data-warehouse-client-3.0.3/data_warehouse_client/file_utils.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/import_tests.py` & `data-warehouse-client-3.0.3/data_warehouse_client/import_tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 import pytest  # see https://realpython.com/pytest-python-testing/
 from typing import Dict, List, Tuple
 from datetime import datetime
 
 from data_warehouse_client.check_bounded_values import get_inverse_category_ids_map
 from data_warehouse_client.data_warehouse import DataWarehouse
 from data_warehouse_client.load_data import load_data
+from data_warehouse_client.load_data import process_measurement_groups as pmg
 from data_warehouse_client.type_checks import check_int
 from data_warehouse_client.type_definitions import DataToLoad, Bounds, LoaderResult, MeasurementGroup, \
     LoadHelperResult, Loader
 from data_warehouse_client import import_with_checks as iwc
+from data_warehouse_client.check_bounded_values import get_bounds
 
 
 @pytest.fixture()
 def walking_test_1() -> DataToLoad:
     data = {
         'visit-date': datetime.now(),
         'visit-code': 'visit3',
@@ -214,14 +216,35 @@
 
 
 @pytest.fixture()
 def test_study():
     return 999
 
 
+@pytest.fixture()
+def bounds_ex1() -> Bounds:
+    return ({419: {'minval': 0, 'maxval': 100}, 435: {'minval': 0, 'maxval': 100}},    # Int Bounds
+            {420: {'minval': 0.0, 'maxval': 100.0}, 436: {'minval': 0, 'maxval': 100}},  # Real Bounds
+            {421: {'minval': datetime(1665, 5, 17, 23, 17, 59),
+                   'maxval': datetime(1668, 5, 17, 23, 17, 59)},
+             437: {'minval': datetime(2400, 5, 17, 23, 17, 59),
+                   'maxval': datetime(2600, 5, 17, 23, 17, 59)}},  # DateTime Bounds
+            {415: [0, 1, 2], 416: [0, 1, 2], 417: [0, 1, 2], 418: [0, 1, 2],
+             431: [0, 1, 2], 432: [0, 1, 2], 433: [0, 1, 2], 434: [0, 1, 2]},  # Category Ids
+            {415: {'First': 0, 'Second': 1, 'Third': 2},
+             416: {'First': 0, 'Second': 1, 'Third': 2},
+             417: {'First': 0, 'Second': 1, 'Third': 2},
+             418: {'First': 0, 'Second': 1, 'Third': 2},
+             431: {'First': 0, 'Second': 1, 'Third': 2},
+             432: {'First': 0, 'Second': 1, 'Third': 2},
+             433: {'First': 0, 'Second': 1, 'Third': 2},
+             434: {'First': 0, 'Second': 1, 'Third': 2}}
+            )  # Category Values to Ids
+
+
 @pytest.mark.parametrize("json_key, json_value, measurement_type, expected_result", [
     ('Int', 4, 410, True),
     ('Real', 5.45, 411, True),
     ('Text', 'Test Data', 412, True),
     ('DateTime', datetime.now(), 413, False),
     ('Bool', 1, 414, True),
     ('NominalfromValue', 'First', 415, True),
@@ -332,14 +355,65 @@
     success, mgis, error_msg = load_data(dw_handle, test_all_example, "test_all", fn_mapper, test_study)
     if success == valid:
         assert True
     else:
         assert False
 
 
+@pytest.mark.parametrize("json_key, json_value, valid", [
+    ('Int', 4.1, False),
+    ('Int', "4", False),
+    ('Real', 5, False),
+    ('Real', "5", False),
+    ('Text', 0, False),
+    ('DateTime', 'Not a Datetime', False),
+    ('DateTime', 32.6, False),
+    ('Bool', 3, False),
+    ('NominalfromValue', 'Fifth', False),
+    ('NominalfromId', 'First', False),
+    ('OrdinalfromValue', 3.142, False),
+    ('OrdinalfromId', 77, False),
+    ('BoundedInt', 9999999, False),
+    ('BoundedReal', 999999.9, False),
+    ('BoundedDateTime', datetime(1666, 5, 17, 23, 17, 59), False),
+    ('External', 5, False),
+    ('SplitEnum', ['First', 'Fifth'], False),
+    ('OptionalInt', '4', False),
+    ('OptionalReal', '3.1', False),
+    ('OptionalText', ['Text List'], False),
+    ('OptionalDateTime', 3, False),
+    ('OptionalBool', 'T', False),
+    ('OptionalNominalfromValue', 'Seventh', False),
+    ('OptionalNominalfromId', 'First', False),
+    ('OptionalOrdinalfromValue', '1', False),
+    ('OptionalOrdinalfromId', '1', False),
+    ('OptionalBoundedInt', 7.89, False),
+    ('OptionalBoundedReal', 4, False),
+    ('OptionalBoundedDateTime', datetime(2500, 5, 17, 23, 17, 59), False),
+    ('OptionalExternal', 5.6, False),
+    ('OptionalSplitEnum', [1, 2], False)
+])
+def test_each_loader(mk_dw_handle, test_study, test_all_example, json_key, measurement_id, json_value, valid):
+    """
+    Check each field in the measurement group instance is handled correctly by the loader
+    """
+    dw_handle = mk_dw_handle
+    bounds = get_bounds(dw_handle, test_study)
+    test_all_example[json_key] = json_value
+    vals_to_load_in_msgs, time_from_data, trial_from_data, participant_from_data, source_from_data = \
+        check_all_loader(test_all_example, bounds)
+    # check for errors in the values
+    successful, all_mgs_and_triples, combined_error_messages = pmg(vals_to_load_in_msgs)
+    if successful == valid:
+        assert True
+    else:
+        print(combined_error_messages)
+        assert False
+
+
 @pytest.mark.parametrize("participant, trial, source, valid", [
     (1, 1, 1, True),
     (2, 1, 1, True),
     (0, 1, 1, False),  # incorrect study
     (1, 0, 1, False),  # incorrect trial
     (1, 1, 3, False)   # incorrect source
 ])
```

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/import_with_checks.py` & `data-warehouse-client-3.0.3/data_warehouse_client/import_with_checks.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 
 from typing import Tuple, List, Optional, Dict, Callable, Any
 from functools import reduce
 from itertools import chain
 
 from data_warehouse_client.type_checks import check_value_type, category_values, check_string
-from data_warehouse_client.type_definitions import MeasurementGroup, ValueTriple, MeasurementType, DataToLoad, ValType, \
-    FieldValue, Bounds, Loader, LoadHelperResult, LoaderResult
+from data_warehouse_client.type_definitions import MeasurementGroup, ValueTriple, MeasurementType, DataToLoad,\
+     ValType, FieldValue, Bounds, Loader, LoadHelperResult, LoaderResult
 
 
 def process_measurement_group(mg_triples):
     """
     takes the result of attempting to load each field in a message group and processes it
     :param mg_triples: [(Success?, [(measurement_type, valtype, value)], Error Message)]
     :return: Success?, [(measurement_type, valtype, value)], [error messages]
@@ -392,14 +392,108 @@
      :param bounds: tuple holding bounds used for checking data
      :return : Error free, [(measurement_type, valtype, value for the jfield in the data)], error_message
      """
     ordinal_type: ValType = 6
     return make_field(measurement_type, ordinal_type, data, jfield, True, bounds)
 
 
+def load_categorical_from_id_in_string(measurement_type: MeasurementType, data: DataToLoad, jfield: str,
+                                       val_type: int, optional: bool, bounds: Bounds) -> \
+        Tuple[bool, List[ValueTriple], str]:
+    """
+     Load a categorical represented by its id encoded in a string
+     :param measurement_type:    measurement type of jfield in the data warehouse
+     :param data:   json that may contain the jfield
+     :param jfield: the name of the field
+     :param val_type: can be nominal or ordinal
+     :param optional: is the field optional?
+     :param bounds: tuple holding bounds used for checking data
+     :return : Error free, [(measurement_type, valtype, value for the jfield in the data)], error_message
+     """
+    exists, val = get_field(data, jfield)  # try to read the field from the data
+    if exists:   # field exists
+        if check_string(val):
+            if val.isnumeric():  # check if the id string encodes an integer
+                num_val: int = int(val)   # turn the string into an integer
+                well_typed, error_message = check_value_type(val_type, num_val, measurement_type, bounds)
+                if well_typed:
+                    return True, [(measurement_type, val_type, num_val)], ""
+                else:
+                    return False, [], wrong_type_error_message(jfield, measurement_type, data, val_type, error_message)
+            else:
+                return False, [], wrong_type_error_message(jfield, measurement_type, data, val_type,
+                                                           f"Category Id {val} is not Integer represented as a String")
+        else:
+            return False, [], wrong_type_error_message(jfield, measurement_type, data, val_type,
+                                                       f"Category Id {val} is not Integer represented as a String")
+    else:
+        if optional:  # optional field
+            return True, [], ""  # Field doesn't exist, which is OK as this is an optional field
+        else:  # compulsary field is missing
+            return False, [], missing_mandatory_type_error_message(jfield, measurement_type, data)
+
+
+def load_nominal_from_id_in_string(measurement_type: MeasurementType, data: DataToLoad, jfield: str,
+                                   bounds: Bounds) -> Tuple[bool, List[ValueTriple], str]:
+    """
+     Load a nominal represented by its id encoded in a string
+     :param measurement_type:    measurement type of jfield in the data warehouse
+     :param data:   json that may contain the jfield
+     :param jfield: the name of the field
+     :param bounds: tuple holding bounds used for checking data
+     :return : Error free, [(measurement_type, valtype, value for the jfield in the data)], error_message
+     """
+    nominal_type: ValType = 5
+    return load_categorical_from_id_in_string(measurement_type, data, jfield, nominal_type, False, bounds)
+
+
+def load_optional_nominal_from_id_in_string(measurement_type: MeasurementType, data: DataToLoad, jfield: str,
+                                            bounds: Bounds) -> Tuple[bool, List[ValueTriple], str]:
+    """
+     Load optional nominal represented by its id encoded in a string
+     :param measurement_type:    measurement type of jfield in the data warehouse
+     :param data:   json that may contain the jfield
+     :param jfield: the name of the field
+     :param bounds: tuple holding bounds used for checking data
+     :return : Error free, [(measurement_type, valtype, value for the jfield in the data)], error_message
+     """
+    nominal_type: ValType = 5
+    return load_categorical_from_id_in_string(measurement_type, data, jfield, nominal_type, True, bounds)
+
+
+def load_ordinal_from_id_in_string(measurement_type: MeasurementType, data: DataToLoad, jfield: str,
+                                   bounds: Bounds) -> \
+        Tuple[bool, List[ValueTriple], str]:
+    """
+     Load ordinal represented by its id encoded in a string
+     :param measurement_type:    measurement type of jfield in the data warehouse
+     :param data:   json that may contain the jfield
+     :param jfield: the name of the field
+     :param bounds: tuple holding bounds used for checking data
+     :return : Error free, [(measurement_type, valtype, value for the jfield in the data)], error_message
+     """
+    ordinal_type: ValType = 6
+    return load_categorical_from_id_in_string(measurement_type, data, jfield, ordinal_type, False, bounds)
+
+
+def load_optional_ordinal_from_id_in_string(measurement_type: MeasurementType, data: DataToLoad, jfield: str,
+                                            bounds: Bounds) -> \
+        Tuple[bool, List[ValueTriple], str]:
+    """
+     Load optional ordinal represented by its id encoded in a string
+     :param measurement_type:    measurement type of jfield in the data warehouse
+     :param data:   json that may contain the jfield
+     :param jfield: the name of the field
+     :param bounds: tuple holding bounds used for checking data
+     :return : Error free, [(measurement_type, valtype, value for the jfield in the data)], error_message
+     """
+    ordinal_type: ValType = 6
+    return load_categorical_from_id_in_string(measurement_type, data, jfield, ordinal_type, True, bounds)
+
+
 def load_categorical_from_value(measurement_type: MeasurementType, data: DataToLoad, jfield: str,
                                 val_type: int, optional: bool, bounds: Bounds) -> \
         Tuple[bool, List[ValueTriple], str]:
     """
      Load a categorical represented by its value in the category table from the dictionary holding the data
      :param measurement_type:    measurement type of jfield in the data warehouse
      :param data:   json that may contain the jfield
```

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/load_data.py` & `data-warehouse-client-3.0.3/data_warehouse_client/load_data.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/load_warehouse_helpers.py` & `data-warehouse-client-3.0.3/data_warehouse_client/load_warehouse_helpers.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/multiple_mg_inserts.py` & `data-warehouse-client-3.0.3/data_warehouse_client/multiple_mg_inserts.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/plot.py` & `data-warehouse-client-3.0.3/data_warehouse_client/plot.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/print_io.py` & `data-warehouse-client-3.0.3/data_warehouse_client/print_io.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/print_metadata_table.py` & `data-warehouse-client-3.0.3/data_warehouse_client/print_metadata_table.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_datetimes.sql` & `data-warehouse-client-3.0.3/data_warehouse_client/sql/bounded_datetimes.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_integers.sql` & `data-warehouse-client-3.0.3/data_warehouse_client/sql/bounded_integers.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/sql/bounded_reals.sql` & `data-warehouse-client-3.0.3/data_warehouse_client/sql/bounded_reals.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/sql/core_sql_from_for_measurements.sql` & `data-warehouse-client-3.0.3/data_warehouse_client/sql/core_sql_from_for_measurements.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/sql/get_measurement_group_info.sql` & `data-warehouse-client-3.0.3/data_warehouse_client/sql/get_measurement_group_info.sql`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/study_profile.py` & `data-warehouse-client-3.0.3/data_warehouse_client/study_profile.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/study_summary.py` & `data-warehouse-client-3.0.3/data_warehouse_client/study_summary.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/table_reader_json.py` & `data-warehouse-client-3.0.3/data_warehouse_client/table_reader_json.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/table_writer_json.py` & `data-warehouse-client-3.0.3/data_warehouse_client/table_writer_json.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/transform_result_format.py` & `data-warehouse-client-3.0.3/data_warehouse_client/transform_result_format.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/type_checks.py` & `data-warehouse-client-3.0.3/data_warehouse_client/type_checks.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/type_definitions.py` & `data-warehouse-client-3.0.3/data_warehouse_client/type_definitions.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client/warehouse_checker.py` & `data-warehouse-client-3.0.3/data_warehouse_client/warehouse_checker.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client.egg-info/PKG-INFO` & `data-warehouse-client-3.0.3/data_warehouse_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-warehouse-client
-Version: 3.0.2
+Version: 3.0.3
 Summary: This package provides access to the e-Science Central data warehouse that can be used to store, access and analyse data collected in scientific studies, including for healthcare applications
 Home-page: https://github.com/e-science-central/data-warehouse-client
 Author: Paul Watson
 Author-email: paul.watson@ncl.ac.uk
 License: UNKNOWN
 Description: # Data Warehouse Client
```

### Comparing `data-warehouse-client-3.0.2/data_warehouse_client.egg-info/SOURCES.txt` & `data-warehouse-client-3.0.3/data_warehouse_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/docs/data_warehouse_guide.pdf` & `data-warehouse-client-3.0.3/docs/data_warehouse_guide.pdf`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/integration_test/clone_study_metadata_test.py` & `data-warehouse-client-3.0.3/integration_test/clone_study_metadata_test.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/integration_test/delete_study_test.py` & `data-warehouse-client-3.0.3/integration_test/delete_study_test.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/setup.py` & `data-warehouse-client-3.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/test/test_file_utils.py` & `data-warehouse-client-3.0.3/test/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `data-warehouse-client-3.0.2/test/test_transform_result_format.py` & `data-warehouse-client-3.0.3/test/test_transform_result_format.py`

 * *Files identical despite different names*

