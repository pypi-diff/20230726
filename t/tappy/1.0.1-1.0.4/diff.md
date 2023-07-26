# Comparing `tmp/tappy-1.0.1.tar.gz` & `tmp/tappy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tappy-1.0.1.tar", last modified: Wed Jul 26 04:05:39 2023, max compression
+gzip compressed data, was "tappy-1.0.4.tar", last modified: Wed Jul 26 19:09:37 2023, max compression
```

## Comparing `tappy-1.0.1.tar` & `tappy-1.0.4.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:05:39.643977 tappy-1.0.1/
--rw-rw-r--   0 tim       (1000) tim       (1000)      102 2023-06-17 22:12:09.000000 tappy-1.0.1/.deepsource.toml
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:05:39.631976 tappy-1.0.1/.github/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:05:39.631976 tappy-1.0.1/.github/workflows/
--rw-rw-r--   0 tim       (1000) tim       (1000)      501 2023-06-19 23:00:36.000000 tappy-1.0.1/.github/workflows/clean-workflow-runs.yml
--rw-rw-r--   0 tim       (1000) tim       (1000)     2121 2023-06-17 22:12:09.000000 tappy-1.0.1/.github/workflows/python-package.yml
--rw-r--r--   0 tim       (1000) tim       (1000)      349 2023-03-05 18:49:58.000000 tappy-1.0.1/.gitignore
--rw-rw-r--   0 tim       (1000) tim       (1000)     2651 2023-07-26 04:01:44.000000 tappy-1.0.1/.pre-commit-config.yaml
--rw-rw-r--   0 tim       (1000) tim       (1000)       50 2022-04-05 13:33:48.000000 tappy-1.0.1/AUTHORS.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      960 2022-09-28 02:52:38.000000 tappy-1.0.1/BADGES.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     1042 2023-07-26 04:02:02.000000 tappy-1.0.1/CHANGELOG.md
--rw-rw-r--   0 tim       (1000) tim       (1000)     1191 2023-01-26 23:43:13.000000 tappy-1.0.1/CITATION.cff
--rw-r--r--   0 tim       (1000) tim       (1000)     3123 2022-07-03 23:02:05.000000 tappy-1.0.1/CONTRIBUTING.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1482 2022-07-03 23:02:18.000000 tappy-1.0.1/LICENSE.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)    10085 2023-07-26 04:05:39.643977 tappy-1.0.1/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     8641 2023-06-10 05:29:49.000000 tappy-1.0.1/README.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)        6 2023-07-26 04:02:02.000000 tappy-1.0.1/VERSION
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:05:39.635977 tappy-1.0.1/docs/
--rw-rw-r--   0 tim       (1000) tim       (1000)     2538 2022-06-12 00:06:46.000000 tappy-1.0.1/docs/CompareTidalFilters.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)    14579 2022-04-05 12:03:23.000000 tappy-1.0.1/docs/Comparison_of_subtraction.png
--rw-rw-r--   0 tim       (1000) tim       (1000)    13684 2022-04-05 12:04:00.000000 tappy-1.0.1/docs/Comparison_of_tidal_filters_large.png
--rw-rw-r--   0 tim       (1000) tim       (1000)    12734 2022-04-05 12:04:28.000000 tappy-1.0.1/docs/Comparison_of_tidal_filters_small.png
--rw-rw-r--   0 tim       (1000) tim       (1000)      462 2022-06-02 19:34:03.000000 tappy-1.0.1/docs/FillMissing.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     1074 2022-06-02 19:34:03.000000 tappy-1.0.1/docs/HarmonicAnalysis.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     5712 2022-04-05 13:36:55.000000 tappy-1.0.1/docs/Makefile
--rw-rw-r--   0 tim       (1000) tim       (1000)    11237 2022-04-05 12:05:55.000000 tappy-1.0.1/docs/Missing.png
--rw-rw-r--   0 tim       (1000) tim       (1000)    16493 2022-10-06 12:58:35.000000 tappy-1.0.1/docs/TappyUsersGuide.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     3233 2022-06-12 00:06:46.000000 tappy-1.0.1/docs/TidalScience.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       55 2022-04-05 15:46:46.000000 tappy-1.0.1/docs/authors.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     5207 2023-06-19 22:50:20.000000 tappy-1.0.1/docs/citation.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      232 2023-05-13 04:20:03.000000 tappy-1.0.1/docs/command_line.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     9549 2023-01-22 03:38:20.000000 tappy-1.0.1/docs/conf.py
--rw-r--r--   0 tim       (1000) tim       (1000)       60 2022-04-05 15:46:22.000000 tappy-1.0.1/docs/contributing.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     3385 2023-06-19 23:00:17.000000 tappy-1.0.1/docs/create_citations.sh
--rw-r--r--   0 tim       (1000) tim       (1000)      191 2023-05-13 04:13:00.000000 tappy-1.0.1/docs/function_summary.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      563 2022-11-06 21:06:34.000000 tappy-1.0.1/docs/index.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       79 2022-04-05 15:46:53.000000 tappy-1.0.1/docs/license.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)       27 2022-04-05 15:41:05.000000 tappy-1.0.1/docs/readme.rst
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:05:39.635977 tappy-1.0.1/example/
--rwxrwxr-x   0 tim       (1000) tim       (1000)      847 2022-10-06 12:58:35.000000 tappy-1.0.1/example/example.sh
--rw-rw-r--   0 tim       (1000) tim       (1000)     2065 2022-04-01 22:29:05.000000 tappy-1.0.1/example/mayport_florida_8720220_con_noaa.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      954 2022-04-01 22:29:05.000000 tappy-1.0.1/example/mayport_florida_8720220_con_tappy.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)    33480 2022-10-06 12:58:35.000000 tappy-1.0.1/example/mayport_florida_8720220_data.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      632 2022-10-06 12:58:35.000000 tappy-1.0.1/example/mayport_florida_8720220_data_def.txt
--rwxrwxr-x   0 tim       (1000) tim       (1000)      825 2023-01-22 03:38:20.000000 tappy-1.0.1/example/process_grace.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      633 2022-10-06 12:58:35.000000 tappy-1.0.1/example/sparse.def
--rw-rw-r--   0 tim       (1000) tim       (1000)      660 2022-10-06 12:58:35.000000 tappy-1.0.1/example/tidesandcurrents.def
--rw-rw-r--   0 tim       (1000) tim       (1000)     2066 2022-04-01 22:29:05.000000 tappy-1.0.1/example/tridentpier_florida_8721604_con_noaa.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      953 2022-04-01 22:29:05.000000 tappy-1.0.1/example/tridentpier_florida_8721604_con_tappy.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)    14490 2022-04-01 22:29:05.000000 tappy-1.0.1/example/tridentpier_florida_8721604_data.txt.gz
--rw-rw-r--   0 tim       (1000) tim       (1000)      949 2022-10-06 12:58:35.000000 tappy-1.0.1/example/tridentpier_florida_8721604_datetime.txt.def
--rw-rw-r--   0 tim       (1000) tim       (1000)     2618 2023-07-26 04:02:02.000000 tappy-1.0.1/pyproject.toml
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-07-26 04:05:39.643977 tappy-1.0.1/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)      509 2023-03-01 21:51:24.000000 tappy-1.0.1/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:05:39.631976 tappy-1.0.1/src/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:05:39.635977 tappy-1.0.1/src/tappy/
--rw-rw-r--   0 tim       (1000) tim       (1000)        0 2023-01-22 03:38:20.000000 tappy-1.0.1/src/tappy/__init__.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)    13822 2023-06-18 18:19:37.000000 tappy-1.0.1/src/tappy/analysis.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     3670 2023-06-19 01:07:24.000000 tappy-1.0.1/src/tappy/prediction.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     3935 2023-06-19 02:59:26.000000 tappy-1.0.1/src/tappy/tappy.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:05:39.635977 tappy-1.0.1/src/tappy/tappy_lib/
--rw-rw-r--   0 tim       (1000) tim       (1000)        0 2023-06-19 21:42:08.000000 tappy-1.0.1/src/tappy/tappy_lib/__init__.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     2501 2023-06-19 04:26:22.000000 tappy-1.0.1/src/tappy/tappy_lib/filter.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    40384 2023-01-22 03:38:20.000000 tappy-1.0.1/src/tappy/tappy_lib/parameter_database.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)    15147 2023-06-19 22:50:21.000000 tappy-1.0.1/src/tappy/tappy_lib/sparser.py
--rwxr-xr-x   0 tim       (1000) tim       (1000)    73991 2023-06-19 22:50:21.000000 tappy-1.0.1/src/tappy/utils.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:05:39.635977 tappy-1.0.1/src/tappy.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)    10085 2023-07-26 04:05:39.000000 tappy-1.0.1/src/tappy.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     3680 2023-07-26 04:05:39.000000 tappy-1.0.1/src/tappy.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-07-26 04:05:39.000000 tappy-1.0.1/src/tappy.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       43 2023-07-26 04:05:39.000000 tappy-1.0.1/src/tappy.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      200 2023-07-26 04:05:39.000000 tappy-1.0.1/src/tappy.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        6 2023-07-26 04:05:39.000000 tappy-1.0.1/src/tappy.egg-info/top_level.txt
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:05:39.635977 tappy-1.0.1/tests/
--rw-rw-r--   0 tim       (1000) tim       (1000)   320926 2022-07-16 12:57:52.000000 tappy-1.0.1/tests/8720218.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)   232070 2022-07-16 13:06:15.000000 tappy-1.0.1/tests/8720218_wl.csv
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:05:39.643977 tappy-1.0.1/tests/output_ts/
--rw-rw-r--   0 tim       (1000) tim       (1000)     2413 2022-04-01 22:29:05.000000 tappy-1.0.1/tests/output_ts/constituents.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31114 2022-07-03 20:09:20.000000 tappy-1.0.1/tests/output_ts/outts_2MN6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31139 2022-07-03 20:09:20.000000 tappy-1.0.1/tests/output_ts/outts_2MS6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31089 2022-07-03 20:09:20.000000 tappy-1.0.1/tests/output_ts/outts_2Q1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30606 2022-07-03 20:09:20.000000 tappy-1.0.1/tests/output_ts/outts_2SM2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31149 2022-07-03 20:09:21.000000 tappy-1.0.1/tests/output_ts/outts_2SM6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31560 2022-07-03 20:09:21.000000 tappy-1.0.1/tests/output_ts/outts_J1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30221 2022-07-03 20:09:21.000000 tappy-1.0.1/tests/output_ts/outts_K1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    29590 2022-07-03 20:09:21.000000 tappy-1.0.1/tests/output_ts/outts_M2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30959 2022-07-03 20:09:21.000000 tappy-1.0.1/tests/output_ts/outts_M3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30698 2022-07-03 20:09:22.000000 tappy-1.0.1/tests/output_ts/outts_M4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31021 2022-07-03 20:09:22.000000 tappy-1.0.1/tests/output_ts/outts_M6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31618 2022-07-03 20:09:22.000000 tappy-1.0.1/tests/output_ts/outts_M8.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30841 2022-07-03 20:09:22.000000 tappy-1.0.1/tests/output_ts/outts_MK3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30806 2022-07-03 20:09:22.000000 tappy-1.0.1/tests/output_ts/outts_MN4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31258 2022-07-03 20:09:23.000000 tappy-1.0.1/tests/output_ts/outts_MO3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30884 2022-07-03 20:09:23.000000 tappy-1.0.1/tests/output_ts/outts_MS4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30446 2022-07-03 20:09:23.000000 tappy-1.0.1/tests/output_ts/outts_MSf.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30050 2022-07-03 20:09:23.000000 tappy-1.0.1/tests/output_ts/outts_N2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30958 2022-07-03 20:09:23.000000 tappy-1.0.1/tests/output_ts/outts_NO1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30493 2022-07-03 20:09:24.000000 tappy-1.0.1/tests/output_ts/outts_O1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31009 2022-07-03 20:09:24.000000 tappy-1.0.1/tests/output_ts/outts_OO1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30878 2022-07-03 20:09:24.000000 tappy-1.0.1/tests/output_ts/outts_Q1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30244 2022-07-03 20:09:24.000000 tappy-1.0.1/tests/output_ts/outts_S2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31326 2022-07-03 20:09:24.000000 tappy-1.0.1/tests/output_ts/outts_S4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31482 2022-07-03 20:09:25.000000 tappy-1.0.1/tests/output_ts/outts_S6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31053 2022-07-03 20:09:25.000000 tappy-1.0.1/tests/output_ts/outts_SK3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30580 2022-07-03 20:09:25.000000 tappy-1.0.1/tests/output_ts/outts_eta2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28802 2022-07-03 20:09:20.000000 tappy-1.0.1/tests/output_ts/outts_ff_2MN6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:20.000000 tappy-1.0.1/tests/output_ts/outts_ff_2MS6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:20.000000 tappy-1.0.1/tests/output_ts/outts_ff_2Q1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:20.000000 tappy-1.0.1/tests/output_ts/outts_ff_2SM2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:21.000000 tappy-1.0.1/tests/output_ts/outts_ff_2SM6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28899 2022-07-03 20:09:21.000000 tappy-1.0.1/tests/output_ts/outts_ff_J1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28900 2022-07-03 20:09:21.000000 tappy-1.0.1/tests/output_ts/outts_ff_K1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:21.000000 tappy-1.0.1/tests/output_ts/outts_ff_M2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28799 2022-07-03 20:09:21.000000 tappy-1.0.1/tests/output_ts/outts_ff_M3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:22.000000 tappy-1.0.1/tests/output_ts/outts_ff_M4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28802 2022-07-03 20:09:22.000000 tappy-1.0.1/tests/output_ts/outts_ff_M6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28799 2022-07-03 20:09:22.000000 tappy-1.0.1/tests/output_ts/outts_ff_M8.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28886 2022-07-03 20:09:22.000000 tappy-1.0.1/tests/output_ts/outts_ff_MK3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:22.000000 tappy-1.0.1/tests/output_ts/outts_ff_MN4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28912 2022-07-03 20:09:23.000000 tappy-1.0.1/tests/output_ts/outts_ff_MO3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:23.000000 tappy-1.0.1/tests/output_ts/outts_ff_MS4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:23.000000 tappy-1.0.1/tests/output_ts/outts_ff_MSf.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:23.000000 tappy-1.0.1/tests/output_ts/outts_ff_N2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28911 2022-07-03 20:09:23.000000 tappy-1.0.1/tests/output_ts/outts_ff_NO1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:24.000000 tappy-1.0.1/tests/output_ts/outts_ff_O1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28904 2022-07-03 20:09:24.000000 tappy-1.0.1/tests/output_ts/outts_ff_OO1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:24.000000 tappy-1.0.1/tests/output_ts/outts_ff_Q1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:24.000000 tappy-1.0.1/tests/output_ts/outts_ff_S2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:24.000000 tappy-1.0.1/tests/output_ts/outts_ff_S4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:25.000000 tappy-1.0.1/tests/output_ts/outts_ff_S6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28900 2022-07-03 20:09:25.000000 tappy-1.0.1/tests/output_ts/outts_ff_SK3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28911 2022-07-03 20:09:25.000000 tappy-1.0.1/tests/output_ts/outts_ff_eta2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28904 2022-07-03 20:09:25.000000 tappy-1.0.1/tests/output_ts/outts_ff_ups1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    21576 2022-04-01 22:29:05.000000 tappy-1.0.1/tests/output_ts/outts_filtered_transform.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    19317 2022-07-03 20:09:25.000000 tappy-1.0.1/tests/output_ts/outts_original.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    21918 2022-04-01 22:29:05.000000 tappy-1.0.1/tests/output_ts/outts_total_prediction.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    29591 2022-07-03 20:09:25.000000 tappy-1.0.1/tests/output_ts/outts_total_tidal_components.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31026 2022-07-03 20:09:25.000000 tappy-1.0.1/tests/output_ts/outts_ups1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)      410 2022-10-06 12:58:35.000000 tappy-1.0.1/tests/predict_def.out
--rw-rw-r--   0 tim       (1000) tim       (1000)      586 2022-10-06 12:58:35.000000 tappy-1.0.1/tests/sparse.def
--rwxrwxr-x   0 tim       (1000) tim       (1000)     3332 2023-06-19 22:50:21.000000 tappy-1.0.1/tests/test_tappy.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 19:09:37.195194 tappy-1.0.4/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      102 2023-06-17 22:12:09.000000 tappy-1.0.4/.deepsource.toml
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 19:09:37.183194 tappy-1.0.4/.github/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 19:09:37.183194 tappy-1.0.4/.github/workflows/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      501 2023-06-19 23:00:36.000000 tappy-1.0.4/.github/workflows/clean-workflow-runs.yml
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2121 2023-06-17 22:12:09.000000 tappy-1.0.4/.github/workflows/python-package.yml
+-rw-r--r--   0 tim       (1000) tim       (1000)      349 2023-03-05 18:49:58.000000 tappy-1.0.4/.gitignore
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2656 2023-07-26 18:06:25.000000 tappy-1.0.4/.pre-commit-config.yaml
+-rw-rw-r--   0 tim       (1000) tim       (1000)       50 2022-04-05 13:33:48.000000 tappy-1.0.4/AUTHORS.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      960 2022-09-28 02:52:38.000000 tappy-1.0.4/BADGES.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1111 2023-07-26 19:09:18.000000 tappy-1.0.4/CHANGELOG.md
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1191 2023-01-26 23:43:13.000000 tappy-1.0.4/CITATION.cff
+-rw-r--r--   0 tim       (1000) tim       (1000)     3123 2022-07-03 23:02:05.000000 tappy-1.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1482 2022-07-03 23:02:18.000000 tappy-1.0.4/LICENSE.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)    10085 2023-07-26 19:09:37.195194 tappy-1.0.4/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     8641 2023-06-10 05:29:49.000000 tappy-1.0.4/README.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)        6 2023-07-26 19:09:18.000000 tappy-1.0.4/VERSION
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 19:09:37.187194 tappy-1.0.4/docs/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2538 2022-06-12 00:06:46.000000 tappy-1.0.4/docs/CompareTidalFilters.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)    14579 2022-04-05 12:03:23.000000 tappy-1.0.4/docs/Comparison_of_subtraction.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)    13684 2022-04-05 12:04:00.000000 tappy-1.0.4/docs/Comparison_of_tidal_filters_large.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)    12734 2022-04-05 12:04:28.000000 tappy-1.0.4/docs/Comparison_of_tidal_filters_small.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)      462 2022-06-02 19:34:03.000000 tappy-1.0.4/docs/FillMissing.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1074 2022-06-02 19:34:03.000000 tappy-1.0.4/docs/HarmonicAnalysis.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     5712 2022-04-05 13:36:55.000000 tappy-1.0.4/docs/Makefile
+-rw-rw-r--   0 tim       (1000) tim       (1000)    11237 2022-04-05 12:05:55.000000 tappy-1.0.4/docs/Missing.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)    16493 2022-10-06 12:58:35.000000 tappy-1.0.4/docs/TappyUsersGuide.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3233 2022-06-12 00:06:46.000000 tappy-1.0.4/docs/TidalScience.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       55 2022-04-05 15:46:46.000000 tappy-1.0.4/docs/authors.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5207 2023-06-19 22:50:20.000000 tappy-1.0.4/docs/citation.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      232 2023-05-13 04:20:03.000000 tappy-1.0.4/docs/command_line.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     9549 2023-01-22 03:38:20.000000 tappy-1.0.4/docs/conf.py
+-rw-r--r--   0 tim       (1000) tim       (1000)       60 2022-04-05 15:46:22.000000 tappy-1.0.4/docs/contributing.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3385 2023-06-19 23:00:17.000000 tappy-1.0.4/docs/create_citations.sh
+-rw-r--r--   0 tim       (1000) tim       (1000)      191 2023-05-13 04:13:00.000000 tappy-1.0.4/docs/function_summary.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      563 2022-11-06 21:06:34.000000 tappy-1.0.4/docs/index.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       79 2022-04-05 15:46:53.000000 tappy-1.0.4/docs/license.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)       27 2022-04-05 15:41:05.000000 tappy-1.0.4/docs/readme.rst
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 19:09:37.187194 tappy-1.0.4/example/
+-rwxrwxr-x   0 tim       (1000) tim       (1000)      847 2022-10-06 12:58:35.000000 tappy-1.0.4/example/example.sh
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2065 2022-04-01 22:29:05.000000 tappy-1.0.4/example/mayport_florida_8720220_con_noaa.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      954 2022-04-01 22:29:05.000000 tappy-1.0.4/example/mayport_florida_8720220_con_tappy.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)    33480 2022-10-06 12:58:35.000000 tappy-1.0.4/example/mayport_florida_8720220_data.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      632 2022-10-06 12:58:35.000000 tappy-1.0.4/example/mayport_florida_8720220_data_def.txt
+-rwxrwxr-x   0 tim       (1000) tim       (1000)      825 2023-01-22 03:38:20.000000 tappy-1.0.4/example/process_grace.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      633 2022-10-06 12:58:35.000000 tappy-1.0.4/example/sparse.def
+-rw-rw-r--   0 tim       (1000) tim       (1000)      660 2022-10-06 12:58:35.000000 tappy-1.0.4/example/tidesandcurrents.def
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2066 2022-04-01 22:29:05.000000 tappy-1.0.4/example/tridentpier_florida_8721604_con_noaa.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      953 2022-04-01 22:29:05.000000 tappy-1.0.4/example/tridentpier_florida_8721604_con_tappy.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)    14490 2022-04-01 22:29:05.000000 tappy-1.0.4/example/tridentpier_florida_8721604_data.txt.gz
+-rw-rw-r--   0 tim       (1000) tim       (1000)      949 2022-10-06 12:58:35.000000 tappy-1.0.4/example/tridentpier_florida_8721604_datetime.txt.def
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2648 2023-07-26 19:09:19.000000 tappy-1.0.4/pyproject.toml
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-07-26 19:09:37.195194 tappy-1.0.4/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)      509 2023-03-01 21:51:24.000000 tappy-1.0.4/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 19:09:37.183194 tappy-1.0.4/src/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 19:09:37.187194 tappy-1.0.4/src/tappy/
+-rw-rw-r--   0 tim       (1000) tim       (1000)        0 2023-01-22 03:38:20.000000 tappy-1.0.4/src/tappy/__init__.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)    13822 2023-06-18 18:19:37.000000 tappy-1.0.4/src/tappy/analysis.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     3670 2023-06-19 01:07:24.000000 tappy-1.0.4/src/tappy/prediction.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     3935 2023-06-19 02:59:26.000000 tappy-1.0.4/src/tappy/tappy.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 19:09:37.187194 tappy-1.0.4/src/tappy/tappy_lib/
+-rw-rw-r--   0 tim       (1000) tim       (1000)        0 2023-06-19 21:42:08.000000 tappy-1.0.4/src/tappy/tappy_lib/__init__.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     2501 2023-06-19 04:26:22.000000 tappy-1.0.4/src/tappy/tappy_lib/filter.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    40384 2023-01-22 03:38:20.000000 tappy-1.0.4/src/tappy/tappy_lib/parameter_database.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)    15147 2023-06-19 22:50:21.000000 tappy-1.0.4/src/tappy/tappy_lib/sparser.py
+-rwxr-xr-x   0 tim       (1000) tim       (1000)    73991 2023-06-19 22:50:21.000000 tappy-1.0.4/src/tappy/utils.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 19:09:37.187194 tappy-1.0.4/src/tappy.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)    10085 2023-07-26 19:09:37.000000 tappy-1.0.4/src/tappy.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3680 2023-07-26 19:09:37.000000 tappy-1.0.4/src/tappy.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-07-26 19:09:37.000000 tappy-1.0.4/src/tappy.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       43 2023-07-26 19:09:37.000000 tappy-1.0.4/src/tappy.egg-info/entry_points.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      216 2023-07-26 19:09:37.000000 tappy-1.0.4/src/tappy.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        6 2023-07-26 19:09:37.000000 tappy-1.0.4/src/tappy.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 19:09:37.187194 tappy-1.0.4/tests/
+-rw-rw-r--   0 tim       (1000) tim       (1000)   320926 2022-07-16 12:57:52.000000 tappy-1.0.4/tests/8720218.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)   232070 2022-07-16 13:06:15.000000 tappy-1.0.4/tests/8720218_wl.csv
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 19:09:37.195194 tappy-1.0.4/tests/output_ts/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2413 2022-04-01 22:29:05.000000 tappy-1.0.4/tests/output_ts/constituents.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31114 2022-07-03 20:09:20.000000 tappy-1.0.4/tests/output_ts/outts_2MN6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31139 2022-07-03 20:09:20.000000 tappy-1.0.4/tests/output_ts/outts_2MS6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31089 2022-07-03 20:09:20.000000 tappy-1.0.4/tests/output_ts/outts_2Q1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30606 2022-07-03 20:09:20.000000 tappy-1.0.4/tests/output_ts/outts_2SM2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31149 2022-07-03 20:09:21.000000 tappy-1.0.4/tests/output_ts/outts_2SM6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31560 2022-07-03 20:09:21.000000 tappy-1.0.4/tests/output_ts/outts_J1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30221 2022-07-03 20:09:21.000000 tappy-1.0.4/tests/output_ts/outts_K1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    29590 2022-07-03 20:09:21.000000 tappy-1.0.4/tests/output_ts/outts_M2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30959 2022-07-03 20:09:21.000000 tappy-1.0.4/tests/output_ts/outts_M3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30698 2022-07-03 20:09:22.000000 tappy-1.0.4/tests/output_ts/outts_M4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31021 2022-07-03 20:09:22.000000 tappy-1.0.4/tests/output_ts/outts_M6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31618 2022-07-03 20:09:22.000000 tappy-1.0.4/tests/output_ts/outts_M8.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30841 2022-07-03 20:09:22.000000 tappy-1.0.4/tests/output_ts/outts_MK3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30806 2022-07-03 20:09:22.000000 tappy-1.0.4/tests/output_ts/outts_MN4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31258 2022-07-03 20:09:23.000000 tappy-1.0.4/tests/output_ts/outts_MO3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30884 2022-07-03 20:09:23.000000 tappy-1.0.4/tests/output_ts/outts_MS4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30446 2022-07-03 20:09:23.000000 tappy-1.0.4/tests/output_ts/outts_MSf.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30050 2022-07-03 20:09:23.000000 tappy-1.0.4/tests/output_ts/outts_N2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30958 2022-07-03 20:09:23.000000 tappy-1.0.4/tests/output_ts/outts_NO1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30493 2022-07-03 20:09:24.000000 tappy-1.0.4/tests/output_ts/outts_O1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31009 2022-07-03 20:09:24.000000 tappy-1.0.4/tests/output_ts/outts_OO1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30878 2022-07-03 20:09:24.000000 tappy-1.0.4/tests/output_ts/outts_Q1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30244 2022-07-03 20:09:24.000000 tappy-1.0.4/tests/output_ts/outts_S2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31326 2022-07-03 20:09:24.000000 tappy-1.0.4/tests/output_ts/outts_S4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31482 2022-07-03 20:09:25.000000 tappy-1.0.4/tests/output_ts/outts_S6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31053 2022-07-03 20:09:25.000000 tappy-1.0.4/tests/output_ts/outts_SK3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30580 2022-07-03 20:09:25.000000 tappy-1.0.4/tests/output_ts/outts_eta2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28802 2022-07-03 20:09:20.000000 tappy-1.0.4/tests/output_ts/outts_ff_2MN6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:20.000000 tappy-1.0.4/tests/output_ts/outts_ff_2MS6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:20.000000 tappy-1.0.4/tests/output_ts/outts_ff_2Q1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:20.000000 tappy-1.0.4/tests/output_ts/outts_ff_2SM2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:21.000000 tappy-1.0.4/tests/output_ts/outts_ff_2SM6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28899 2022-07-03 20:09:21.000000 tappy-1.0.4/tests/output_ts/outts_ff_J1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28900 2022-07-03 20:09:21.000000 tappy-1.0.4/tests/output_ts/outts_ff_K1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:21.000000 tappy-1.0.4/tests/output_ts/outts_ff_M2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28799 2022-07-03 20:09:21.000000 tappy-1.0.4/tests/output_ts/outts_ff_M3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:22.000000 tappy-1.0.4/tests/output_ts/outts_ff_M4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28802 2022-07-03 20:09:22.000000 tappy-1.0.4/tests/output_ts/outts_ff_M6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28799 2022-07-03 20:09:22.000000 tappy-1.0.4/tests/output_ts/outts_ff_M8.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28886 2022-07-03 20:09:22.000000 tappy-1.0.4/tests/output_ts/outts_ff_MK3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:22.000000 tappy-1.0.4/tests/output_ts/outts_ff_MN4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28912 2022-07-03 20:09:23.000000 tappy-1.0.4/tests/output_ts/outts_ff_MO3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:23.000000 tappy-1.0.4/tests/output_ts/outts_ff_MS4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:23.000000 tappy-1.0.4/tests/output_ts/outts_ff_MSf.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:23.000000 tappy-1.0.4/tests/output_ts/outts_ff_N2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28911 2022-07-03 20:09:23.000000 tappy-1.0.4/tests/output_ts/outts_ff_NO1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:24.000000 tappy-1.0.4/tests/output_ts/outts_ff_O1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28904 2022-07-03 20:09:24.000000 tappy-1.0.4/tests/output_ts/outts_ff_OO1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:24.000000 tappy-1.0.4/tests/output_ts/outts_ff_Q1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:24.000000 tappy-1.0.4/tests/output_ts/outts_ff_S2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:24.000000 tappy-1.0.4/tests/output_ts/outts_ff_S4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:25.000000 tappy-1.0.4/tests/output_ts/outts_ff_S6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28900 2022-07-03 20:09:25.000000 tappy-1.0.4/tests/output_ts/outts_ff_SK3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28911 2022-07-03 20:09:25.000000 tappy-1.0.4/tests/output_ts/outts_ff_eta2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28904 2022-07-03 20:09:25.000000 tappy-1.0.4/tests/output_ts/outts_ff_ups1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    21576 2022-04-01 22:29:05.000000 tappy-1.0.4/tests/output_ts/outts_filtered_transform.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    19317 2022-07-03 20:09:25.000000 tappy-1.0.4/tests/output_ts/outts_original.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    21918 2022-04-01 22:29:05.000000 tappy-1.0.4/tests/output_ts/outts_total_prediction.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    29591 2022-07-03 20:09:25.000000 tappy-1.0.4/tests/output_ts/outts_total_tidal_components.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31026 2022-07-03 20:09:25.000000 tappy-1.0.4/tests/output_ts/outts_ups1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)      410 2022-10-06 12:58:35.000000 tappy-1.0.4/tests/predict_def.out
+-rw-rw-r--   0 tim       (1000) tim       (1000)      586 2022-10-06 12:58:35.000000 tappy-1.0.4/tests/sparse.def
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     2848 2023-07-26 19:02:59.000000 tappy-1.0.4/tests/test_tappy.py
```

### Comparing `tappy-1.0.1/.github/workflows/python-package.yml` & `tappy-1.0.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/.pre-commit-config.yaml` & `tappy-1.0.4/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -85,11 +85,11 @@
     - repo: https://github.com/commitizen-tools/commitizen
       rev: 3.5.3
       hooks:
           - id: commitizen
             stages: [commit-msg]
 
     - repo: https://github.com/mwouts/jupytext
-      rev: v1.14.7
+      rev: v1.15.0-dev1
       hooks:
           - id: jupytext
             args: [--from, ipynb, --to, auto:percent, --sync]
```

### Comparing `tappy-1.0.1/BADGES.rst` & `tappy-1.0.4/BADGES.rst`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/CHANGELOG.md` & `tappy-1.0.4/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.0.4 (2023-07-26)
+
+## 1.0.3 (2023-07-26)
+
+## 1.0.2 (2023-07-26)
+
 ## 1.0.1 (2023-07-26)
 
 ## 1.0.0 (2023-06-20)
 
 ### Refactor
 
 - complete refactor to match approach with other toolboxes
```

### Comparing `tappy-1.0.1/CITATION.cff` & `tappy-1.0.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/CONTRIBUTING.rst` & `tappy-1.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/LICENSE.txt` & `tappy-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/PKG-INFO` & `tappy-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: tappy
-Version: 1.0.1
+Version: 1.0.4
 Summary: Command line script and Python library perform tidally-based analysis of water level data.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/tappy/docs/index.html#tappy-documentation
 Project-URL: github, https://github.com/timcera/tappy
 Project-URL: bitbucket, https://bitbucket.org/timcera/tappy/src/main/
-Keywords: tidal-analysis,cli-app,tide-analysis,tide-prediction,tide-filter,python
+Keywords: cli-app,python,tidal-analysis,tide-analysis,tide-filter,tide-prediction
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7.1
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 .. image:: https://github.com/timcera/tappy/actions/workflows/python-package.yml/badge.svg
```

### Comparing `tappy-1.0.1/README.rst` & `tappy-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/docs/CompareTidalFilters.rst` & `tappy-1.0.4/docs/CompareTidalFilters.rst`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/docs/Comparison_of_subtraction.png` & `tappy-1.0.4/docs/Comparison_of_subtraction.png`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/docs/Comparison_of_tidal_filters_large.png` & `tappy-1.0.4/docs/Comparison_of_tidal_filters_large.png`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/docs/Comparison_of_tidal_filters_small.png` & `tappy-1.0.4/docs/Comparison_of_tidal_filters_small.png`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/docs/HarmonicAnalysis.rst` & `tappy-1.0.4/docs/HarmonicAnalysis.rst`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/docs/Makefile` & `tappy-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/docs/Missing.png` & `tappy-1.0.4/docs/Missing.png`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/docs/TappyUsersGuide.rst` & `tappy-1.0.4/docs/TappyUsersGuide.rst`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/docs/TidalScience.rst` & `tappy-1.0.4/docs/TidalScience.rst`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/docs/citation.txt` & `tappy-1.0.4/docs/citation.txt`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/docs/conf.py` & `tappy-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/docs/create_citations.sh` & `tappy-1.0.4/docs/create_citations.sh`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/docs/index.rst` & `tappy-1.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/example/example.sh` & `tappy-1.0.4/example/example.sh`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/example/mayport_florida_8720220_con_noaa.txt` & `tappy-1.0.4/example/mayport_florida_8720220_con_noaa.txt`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/example/mayport_florida_8720220_con_tappy.txt` & `tappy-1.0.4/example/mayport_florida_8720220_con_tappy.txt`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/example/mayport_florida_8720220_data.txt` & `tappy-1.0.4/example/mayport_florida_8720220_data.txt`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/example/mayport_florida_8720220_data_def.txt` & `tappy-1.0.4/example/mayport_florida_8720220_data_def.txt`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/example/process_grace.py` & `tappy-1.0.4/example/process_grace.py`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/example/sparse.def` & `tappy-1.0.4/example/sparse.def`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/example/tidesandcurrents.def` & `tappy-1.0.4/example/tidesandcurrents.def`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/example/tridentpier_florida_8721604_con_noaa.txt` & `tappy-1.0.4/example/tridentpier_florida_8721604_con_noaa.txt`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/example/tridentpier_florida_8721604_con_tappy.txt` & `tappy-1.0.4/example/tridentpier_florida_8721604_con_tappy.txt`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/example/tridentpier_florida_8721604_data.txt.gz` & `tappy-1.0.4/example/tridentpier_florida_8721604_data.txt.gz`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/example/tridentpier_florida_8721604_datetime.txt.def` & `tappy-1.0.4/example/tridentpier_florida_8721604_datetime.txt.def`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/pyproject.toml` & `tappy-1.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -9,90 +9,92 @@
 
 [project]
 name = "tappy"
 dynamic = ["version", "readme"]
 description = "Command line script and Python library perform tidally-based analysis of water level data."
 requires-python = ">=3.7.1"
 dependencies = [
-    "toolbox_utils >= 5.0.0, < 6.0.0",
     "astronomia",
     "cltoolbox",
-    "numpy"
+    "numpy",
+    "pyparsing",
+    "scipy",
+    "toolbox_utils >= 5.0.0, < 6.0.0"
 ]
 license = {text = "BSD-3-Clause"}
 authors = [
     {name = "Tim Cera", email = "tim@cerazone.net"}
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Science/Research",
-    "Intended Audience :: End Users/Desktop",
-    "Intended Audience :: Developers",
     "Environment :: Console",
+    "Intended Audience :: Developers",
+    "Intended Audience :: End Users/Desktop",
+    "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Topic :: Scientific/Engineering :: Information Analysis",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering",
+    "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 keywords = [
-    "tidal-analysis",
     "cli-app",
+    "python",
+    "tidal-analysis",
     "tide-analysis",
-    "tide-prediction",
     "tide-filter",
-    "python"
+    "tide-prediction"
 ]
 
 [project.optional-dependencies]
 dev = [
     "black",
+    "blacken-docs",
+    "black-nbconvert",
     "cleanpy",
-    "twine",
-    "pytest",
+    "commitizen",
     "coverage",
     "flake8",
+    "isort",
+    "pre-commit",
+    "pytest",
     "pytest-cov",
     "pytest-mpl",
-    "pre-commit",
-    "black-nbconvert",
-    "blacken-docs",
-    "velin",
-    "isort",
     "pyupgrade",
-    "commitizen"
+    "twine",
+    "velin"
 ]
 
 [project.scripts]
 tappy = "tappy.tappy:main"
 
 [project.urls]
 documentation = "https://timcera.bitbucket.io/tappy/docs/index.html#tappy-documentation"
 github = "https://github.com/timcera/tappy"
 bitbucket = "https://bitbucket.org/timcera/tappy/src/main/"
 
 [tool]
 
 [tool.check-manifest]
 ignore = [
-    "docs/_function_autosummary/*",
     ".coverage",
     ".deepsource.toml",
+    "docs/_function_autosummary/*",
     ".ipynb_checkpoints/*"
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.1"
+version = "1.0.4"
 tag_format = "$version"
 version_files = ["VERSION"]
 update_changelog_on_bump = true
 
 [tool.isort]
 profile = "black"
```

### Comparing `tappy-1.0.1/src/tappy/analysis.py` & `tappy-1.0.4/src/tappy/analysis.py`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/src/tappy/prediction.py` & `tappy-1.0.4/src/tappy/prediction.py`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/src/tappy/tappy.py` & `tappy-1.0.4/src/tappy/tappy.py`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/src/tappy/tappy_lib/filter.py` & `tappy-1.0.4/src/tappy/tappy_lib/filter.py`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/src/tappy/tappy_lib/parameter_database.py` & `tappy-1.0.4/src/tappy/tappy_lib/parameter_database.py`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/src/tappy/tappy_lib/sparser.py` & `tappy-1.0.4/src/tappy/tappy_lib/sparser.py`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/src/tappy/utils.py` & `tappy-1.0.4/src/tappy/utils.py`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/src/tappy.egg-info/PKG-INFO` & `tappy-1.0.4/src/tappy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: tappy
-Version: 1.0.1
+Version: 1.0.4
 Summary: Command line script and Python library perform tidally-based analysis of water level data.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/tappy/docs/index.html#tappy-documentation
 Project-URL: github, https://github.com/timcera/tappy
 Project-URL: bitbucket, https://bitbucket.org/timcera/tappy/src/main/
-Keywords: tidal-analysis,cli-app,tide-analysis,tide-prediction,tide-filter,python
+Keywords: cli-app,python,tidal-analysis,tide-analysis,tide-filter,tide-prediction
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7.1
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 .. image:: https://github.com/timcera/tappy/actions/workflows/python-package.yml/badge.svg
```

### Comparing `tappy-1.0.1/src/tappy.egg-info/SOURCES.txt` & `tappy-1.0.4/src/tappy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/8720218.csv` & `tappy-1.0.4/tests/8720218.csv`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/8720218_wl.csv` & `tappy-1.0.4/tests/8720218_wl.csv`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/constituents.dat` & `tappy-1.0.4/tests/output_ts/constituents.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_2MN6.dat` & `tappy-1.0.4/tests/output_ts/outts_2MN6.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_2MS6.dat` & `tappy-1.0.4/tests/output_ts/outts_2MS6.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_2Q1.dat` & `tappy-1.0.4/tests/output_ts/outts_2Q1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_2SM2.dat` & `tappy-1.0.4/tests/output_ts/outts_2SM2.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_2SM6.dat` & `tappy-1.0.4/tests/output_ts/outts_2SM6.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_J1.dat` & `tappy-1.0.4/tests/output_ts/outts_J1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_K1.dat` & `tappy-1.0.4/tests/output_ts/outts_K1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_M2.dat` & `tappy-1.0.4/tests/output_ts/outts_M2.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_M3.dat` & `tappy-1.0.4/tests/output_ts/outts_M3.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_M4.dat` & `tappy-1.0.4/tests/output_ts/outts_M4.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_M6.dat` & `tappy-1.0.4/tests/output_ts/outts_M6.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_M8.dat` & `tappy-1.0.4/tests/output_ts/outts_M8.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_MK3.dat` & `tappy-1.0.4/tests/output_ts/outts_MK3.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_MN4.dat` & `tappy-1.0.4/tests/output_ts/outts_MN4.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_MO3.dat` & `tappy-1.0.4/tests/output_ts/outts_MO3.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_MS4.dat` & `tappy-1.0.4/tests/output_ts/outts_MS4.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_MSf.dat` & `tappy-1.0.4/tests/output_ts/outts_MSf.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_N2.dat` & `tappy-1.0.4/tests/output_ts/outts_N2.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_NO1.dat` & `tappy-1.0.4/tests/output_ts/outts_NO1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_O1.dat` & `tappy-1.0.4/tests/output_ts/outts_O1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_OO1.dat` & `tappy-1.0.4/tests/output_ts/outts_OO1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_Q1.dat` & `tappy-1.0.4/tests/output_ts/outts_Q1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_S2.dat` & `tappy-1.0.4/tests/output_ts/outts_S2.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_S4.dat` & `tappy-1.0.4/tests/output_ts/outts_S4.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_S6.dat` & `tappy-1.0.4/tests/output_ts/outts_S6.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_SK3.dat` & `tappy-1.0.4/tests/output_ts/outts_SK3.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_eta2.dat` & `tappy-1.0.4/tests/output_ts/outts_eta2.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_2MN6.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_2MN6.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_2MS6.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_2MS6.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_2Q1.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_2Q1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_2SM2.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_2SM2.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_2SM6.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_2SM6.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_J1.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_J1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_K1.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_K1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_M2.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_M2.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_M3.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_M3.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_M4.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_M4.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_M6.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_M6.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_M8.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_M8.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_MK3.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_MK3.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_MN4.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_MN4.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_MO3.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_MO3.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_MS4.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_MS4.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_MSf.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_MSf.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_N2.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_N2.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_NO1.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_NO1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_O1.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_O1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_OO1.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_OO1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_Q1.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_Q1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_S2.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_S2.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_S4.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_S4.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_S6.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_S6.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_SK3.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_SK3.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_eta2.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_eta2.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ff_ups1.dat` & `tappy-1.0.4/tests/output_ts/outts_ff_ups1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_filtered_transform.dat` & `tappy-1.0.4/tests/output_ts/outts_filtered_transform.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_original.dat` & `tappy-1.0.4/tests/output_ts/outts_original.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_total_prediction.dat` & `tappy-1.0.4/tests/output_ts/outts_total_prediction.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_total_tidal_components.dat` & `tappy-1.0.4/tests/output_ts/outts_total_tidal_components.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/output_ts/outts_ups1.dat` & `tappy-1.0.4/tests/output_ts/outts_ups1.dat`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/sparse.def` & `tappy-1.0.4/tests/sparse.def`

 * *Files identical despite different names*

### Comparing `tappy-1.0.1/tests/test_tappy.py` & `tappy-1.0.4/tests/test_tappy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python
 
-import difflib
 import glob
 import os
 import re
 import shlex
 import shutil
 import subprocess
 import tempfile
 from pathlib import Path
 from unittest import TestCase
 
+import pandas as pd
+from pandas.testing import assert_frame_equal
+
 # directory dance to find tappy.py module in directory above
 # test_tappy.py
 file_loc = Path(__file__).resolve()
 cur_path = file_loc.parent
 
 
 class TappyTest(TestCase):
@@ -34,36 +36,25 @@
                 #        '--zero_ts="transform"',
                 "--outputts",
                 '--outputxml="testout.xml"',
                 #        '--filter="transform"',
                 "--include_inferred",
             ]
         )
-        print(ret)
 
     def tearDown(self):
         os.chdir(self.cwd)
         shutil.rmtree(self.tmpdir)
 
     def test_constituents(self):
         os.chdir(self.tmpdir)
         for i in ["M2", "M8"]:
-            alines = open(
-                self.cwd / "tests" / "output_ts" / f"outts_{i}.dat"
-            ).readlines()
-            print(Path.cwd())
-            print(glob.glob("*"))
-            blines = open(Path(f"outts_{i}.dat")).readlines()
-            d = difflib.Differ()
-            result = list(d.compare(alines, blines))
-            result = [i for i in result if i[0] in ["+", "-", "?"]]
-            print(
-                "".join(result),
-            )
-            self.assertEqual(result, [])
+            alines = pd.read_csv(self.cwd / "tests" / "output_ts" / f"outts_{i}.dat")
+            blines = pd.read_csv(Path(f"outts_{i}.dat"))
+            assert_frame_equal(alines, blines, atol=1e-4)
 
     def test_closure(self):
         os.chdir(self.tmpdir)
         inputf = self.cwd / "example" / "mayport_florida_8720220_data.txt"
         _ = subprocess.call(
             shlex.split(
                 f"tappy analysis {inputf} --outputxml testout.xml --include_inferred"
@@ -76,32 +67,27 @@
         )
         def_filename = self.cwd / "tests" / "predict_def.out"
         _ = subprocess.call(
             shlex.split(
                 f"tappy analysis predict.out --def_filename {def_filename} --outputxml testoutclosure.xml --include_inferred"
             )
         )
-        print(os.getcwd())
-        print(glob.glob("*"))
-        alines = open("testout.xml").readlines()
-        blines = open("testoutclosure.xml").readlines()
+
+        alines = open("testout.xml", encoding="ascii").readlines()
+        blines = open("testoutclosure.xml", encoding="ascii").readlines()
+
         nalines = []
         for a in alines:
             match = re.search(r"[0-9\.]+", a)
             if match is not None:
                 nalines.append(str(round(float(match.group()), 2)))
         nblines = []
         for b in blines:
             match = re.search(r"[0-9\.]+", b)
             if match is not None:
                 nblines.append(str(round(float(match.group()), 2)))
-        d = difflib.Differ()
-        result = list(d.compare(nalines, nblines))
-        result = [i for i in result if i[0] in ["+", "-", "?"]]
-        print(
-            "".join(result),
-        )
-        self.assertEqual(result, [])
+
+        self.assertEqual(nalines, nblines)
 
 
 if __name__ == "__main__":
     unittest.main()
```

