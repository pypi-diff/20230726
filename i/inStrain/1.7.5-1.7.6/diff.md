# Comparing `tmp/inStrain-1.7.5.tar.gz` & `tmp/inStrain-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inStrain-1.7.5.tar", last modified: Tue May 16 21:16:14 2023, max compression
+gzip compressed data, was "inStrain-1.7.6.tar", last modified: Wed Jul 26 21:40:17 2023, max compression
```

## Comparing `inStrain-1.7.5.tar` & `inStrain-1.7.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 21:16:14.633691 inStrain-1.7.5/
--rw-r--r--   0 mattolm    (501) staff       (20)     1065 2021-03-26 22:19:41.000000 inStrain-1.7.5/LICENSE
--rw-r--r--   0 mattolm    (501) staff       (20)      279 2023-05-16 21:16:14.633562 inStrain-1.7.5/PKG-INFO
--rw-r--r--   0 mattolm    (501) staff       (20)     1416 2023-02-21 01:15:19.000000 inStrain-1.7.5/README.md
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 21:16:14.618438 inStrain-1.7.5/bin/
--rwxr-xr-x   0 mattolm    (501) staff       (20)      962 2021-01-21 18:18:24.000000 inStrain-1.7.5/bin/inStrain
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 21:16:14.619261 inStrain-1.7.5/docker/
--rw-r--r--   0 mattolm    (501) staff       (20)        0 2021-01-21 18:18:24.000000 inStrain-1.7.5/docker/__init__.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     1688 2021-01-21 18:18:24.000000 inStrain-1.7.5/docker/job_utils.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    10928 2022-06-10 19:12:50.000000 inStrain-1.7.5/docker/run_instrain.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     5153 2021-01-21 18:18:24.000000 inStrain-1.7.5/docker/s3_utils.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 21:16:14.623295 inStrain-1.7.5/inStrain/
--rwxr-xr-x   0 mattolm    (501) staff       (20)    31954 2023-02-24 17:32:05.000000 inStrain-1.7.5/inStrain/GeneProfile.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    42757 2023-05-16 19:21:51.000000 inStrain-1.7.5/inStrain/SNVprofile.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)       34 2021-01-21 18:18:24.000000 inStrain-1.7.5/inStrain/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)       22 2023-05-16 21:09:11.000000 inStrain-1.7.5/inStrain/_version.py
--rw-r--r--   0 mattolm    (501) staff       (20)    23220 2023-02-21 01:15:04.000000 inStrain-1.7.5/inStrain/argumentParser.py
--rw-r--r--   0 mattolm    (501) staff       (20)    25579 2022-06-10 19:12:50.000000 inStrain-1.7.5/inStrain/compare_controller.py
--rw-r--r--   0 mattolm    (501) staff       (20)     4897 2021-01-21 18:18:24.000000 inStrain-1.7.5/inStrain/compare_greedy.py
--rw-r--r--   0 mattolm    (501) staff       (20)     8480 2023-02-25 01:32:59.000000 inStrain-1.7.5/inStrain/compare_utils.py
--rw-r--r--   0 mattolm    (501) staff       (20)    17782 2023-02-21 01:15:04.000000 inStrain-1.7.5/inStrain/controller.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 21:16:14.625452 inStrain-1.7.5/inStrain/deprecated/
--rw-r--r--   0 mattolm    (501) staff       (20)     2257 2023-02-24 18:53:38.000000 inStrain-1.7.5/inStrain/deprecated/DEPRECATEDmapping_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)    34343 2021-02-12 01:00:32.000000 inStrain-1.7.5/inStrain/deprecated/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)    22971 2021-01-21 18:18:24.000000 inStrain-1.7.5/inStrain/deprecated/deprecated_filter_reads.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     9651 2021-01-21 18:18:24.000000 inStrain-1.7.5/inStrain/deprecated/deprecated_gene_statistics.py
--rw-r--r--   0 mattolm    (501) staff       (20)    58073 2023-02-25 01:32:59.000000 inStrain-1.7.5/inStrain/deprecated/plottingUtilities.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    35695 2023-02-25 01:48:27.000000 inStrain-1.7.5/inStrain/filter_reads.py
--rw-r--r--   0 mattolm    (501) staff       (20)    34180 2023-02-25 01:41:50.000000 inStrain-1.7.5/inStrain/genomeUtilities.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 21:16:14.628406 inStrain-1.7.5/inStrain/helper_files/
--rw-r--r--   0 mattolm    (501) staff       (20)  1256610 2021-01-21 18:18:24.000000 inStrain-1.7.5/inStrain/helper_files/NullModel.txt
--rw-r--r--   0 mattolm    (501) staff       (20)     8957 2021-02-12 01:00:32.000000 inStrain-1.7.5/inStrain/irep_utilities.py
--rw-r--r--   0 mattolm    (501) staff       (20)    38401 2021-03-26 21:19:02.000000 inStrain-1.7.5/inStrain/logUtils.py
--rw-r--r--   0 mattolm    (501) staff       (20)    15346 2023-05-16 21:08:22.000000 inStrain-1.7.5/inStrain/parse_annotations.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 21:16:14.631704 inStrain-1.7.5/inStrain/plotting/
--rw-r--r--   0 mattolm    (501) staff       (20)     2524 2023-02-24 18:53:38.000000 inStrain-1.7.5/inStrain/plotting/SNV_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)      662 2021-02-12 01:00:32.000000 inStrain-1.7.5/inStrain/plotting/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)     9260 2023-02-25 01:38:35.000000 inStrain-1.7.5/inStrain/plotting/compare_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     2548 2021-02-12 01:00:32.000000 inStrain-1.7.5/inStrain/plotting/gene_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     6638 2023-02-24 18:50:29.000000 inStrain-1.7.5/inStrain/plotting/linkage_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     9075 2023-02-25 00:47:19.000000 inStrain-1.7.5/inStrain/plotting/mapping_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     5332 2023-02-25 00:49:14.000000 inStrain-1.7.5/inStrain/plotting/plotting_controller.py
--rw-r--r--   0 mattolm    (501) staff       (20)    18444 2023-02-24 18:53:38.000000 inStrain-1.7.5/inStrain/plotting/positional_plots.py
--rw-r--r--   0 mattolm    (501) staff       (20)     2831 2021-02-12 01:00:32.000000 inStrain-1.7.5/inStrain/plotting/utilities.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    20710 2023-02-25 01:32:59.000000 inStrain-1.7.5/inStrain/polymorpher.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 21:16:14.633043 inStrain-1.7.5/inStrain/profile/
--rw-r--r--   0 mattolm    (501) staff       (20)      636 2021-01-21 18:18:24.000000 inStrain-1.7.5/inStrain/profile/__init__.py
--rw-r--r--   0 mattolm    (501) staff       (20)     5822 2021-02-12 01:00:32.000000 inStrain-1.7.5/inStrain/profile/fasta.py
--rw-r--r--   0 mattolm    (501) staff       (20)     9115 2021-01-21 18:18:24.000000 inStrain-1.7.5/inStrain/profile/linkage.py
--rw-r--r--   0 mattolm    (501) staff       (20)    15636 2021-01-21 18:18:24.000000 inStrain-1.7.5/inStrain/profile/profile_controller.py
--rw-r--r--   0 mattolm    (501) staff       (20)    32820 2023-02-24 18:17:07.000000 inStrain-1.7.5/inStrain/profile/profile_utilities.py
--rw-r--r--   0 mattolm    (501) staff       (20)     3144 2021-02-17 23:42:47.000000 inStrain-1.7.5/inStrain/profile/samtools_ops.py
--rw-r--r--   0 mattolm    (501) staff       (20)    10361 2021-02-12 01:00:32.000000 inStrain-1.7.5/inStrain/profile/snv_utilities.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)     5332 2021-02-12 01:00:32.000000 inStrain-1.7.5/inStrain/quickProfile.py
--rwxr-xr-x   0 mattolm    (501) staff       (20)    16916 2022-06-10 19:12:50.000000 inStrain-1.7.5/inStrain/readComparer.py
--rw-r--r--   0 mattolm    (501) staff       (20)     2629 2023-02-25 01:49:24.000000 inStrain-1.7.5/inStrain/utils.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 21:16:14.624089 inStrain-1.7.5/inStrain.egg-info/
--rw-r--r--   0 mattolm    (501) staff       (20)      279 2023-05-16 21:16:14.000000 inStrain-1.7.5/inStrain.egg-info/PKG-INFO
--rw-r--r--   0 mattolm    (501) staff       (20)     1563 2023-05-16 21:16:14.000000 inStrain-1.7.5/inStrain.egg-info/SOURCES.txt
--rw-r--r--   0 mattolm    (501) staff       (20)        1 2023-05-16 21:16:14.000000 inStrain-1.7.5/inStrain.egg-info/dependency_links.txt
--rw-r--r--   0 mattolm    (501) staff       (20)        1 2023-02-25 02:21:32.000000 inStrain-1.7.5/inStrain.egg-info/not-zip-safe
--rw-r--r--   0 mattolm    (501) staff       (20)      113 2023-05-16 21:16:14.000000 inStrain-1.7.5/inStrain.egg-info/requires.txt
--rw-r--r--   0 mattolm    (501) staff       (20)       16 2023-05-16 21:16:14.000000 inStrain-1.7.5/inStrain.egg-info/top_level.txt
--rw-r--r--   0 mattolm    (501) staff       (20)       38 2023-05-16 21:16:14.633726 inStrain-1.7.5/setup.cfg
--rw-r--r--   0 mattolm    (501) staff       (20)     1051 2023-02-25 02:18:49.000000 inStrain-1.7.5/setup.py
-drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-05-16 21:16:14.633284 inStrain-1.7.5/test/
--rwxr-xr-x   0 mattolm    (501) staff       (20)     1213 2022-06-10 19:12:50.000000 inStrain-1.7.5/test/test_suite.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-07-26 21:40:17.217949 inStrain-1.7.6/
+-rw-r--r--   0 mattolm    (501) staff       (20)     1065 2021-03-26 22:19:41.000000 inStrain-1.7.6/LICENSE
+-rw-r--r--   0 mattolm    (501) staff       (20)      279 2023-07-26 21:40:17.217815 inStrain-1.7.6/PKG-INFO
+-rw-r--r--   0 mattolm    (501) staff       (20)     1416 2023-02-21 01:15:19.000000 inStrain-1.7.6/README.md
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-07-26 21:40:17.205376 inStrain-1.7.6/bin/
+-rwxr-xr-x   0 mattolm    (501) staff       (20)      962 2021-01-21 18:18:24.000000 inStrain-1.7.6/bin/inStrain
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-07-26 21:40:17.206271 inStrain-1.7.6/docker/
+-rw-r--r--   0 mattolm    (501) staff       (20)        0 2021-01-21 18:18:24.000000 inStrain-1.7.6/docker/__init__.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     1688 2021-01-21 18:18:24.000000 inStrain-1.7.6/docker/job_utils.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    10928 2022-06-10 19:12:50.000000 inStrain-1.7.6/docker/run_instrain.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     5153 2021-01-21 18:18:24.000000 inStrain-1.7.6/docker/s3_utils.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-07-26 21:40:17.210929 inStrain-1.7.6/inStrain/
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    31954 2023-02-24 17:32:05.000000 inStrain-1.7.6/inStrain/GeneProfile.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    42757 2023-05-16 19:21:51.000000 inStrain-1.7.6/inStrain/SNVprofile.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)       34 2021-01-21 18:18:24.000000 inStrain-1.7.6/inStrain/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)       22 2023-07-26 21:13:31.000000 inStrain-1.7.6/inStrain/_version.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    23220 2023-02-21 01:15:04.000000 inStrain-1.7.6/inStrain/argumentParser.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    25579 2023-07-26 21:10:33.000000 inStrain-1.7.6/inStrain/compare_controller.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     4897 2021-01-21 18:18:24.000000 inStrain-1.7.6/inStrain/compare_greedy.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     8480 2023-02-25 01:32:59.000000 inStrain-1.7.6/inStrain/compare_utils.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    17782 2023-02-21 01:15:04.000000 inStrain-1.7.6/inStrain/controller.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-07-26 21:40:17.213148 inStrain-1.7.6/inStrain/deprecated/
+-rw-r--r--   0 mattolm    (501) staff       (20)     2257 2023-02-24 18:53:38.000000 inStrain-1.7.6/inStrain/deprecated/DEPRECATEDmapping_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    34343 2021-02-12 01:00:32.000000 inStrain-1.7.6/inStrain/deprecated/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    22971 2021-01-21 18:18:24.000000 inStrain-1.7.6/inStrain/deprecated/deprecated_filter_reads.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     9651 2021-01-21 18:18:24.000000 inStrain-1.7.6/inStrain/deprecated/deprecated_gene_statistics.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    58073 2023-02-25 01:32:59.000000 inStrain-1.7.6/inStrain/deprecated/plottingUtilities.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    35695 2023-02-25 01:48:27.000000 inStrain-1.7.6/inStrain/filter_reads.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    34180 2023-02-25 01:41:50.000000 inStrain-1.7.6/inStrain/genomeUtilities.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-07-26 21:40:17.213692 inStrain-1.7.6/inStrain/helper_files/
+-rw-r--r--   0 mattolm    (501) staff       (20)  1256610 2021-01-21 18:18:24.000000 inStrain-1.7.6/inStrain/helper_files/NullModel.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)     8957 2021-02-12 01:00:32.000000 inStrain-1.7.6/inStrain/irep_utilities.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    38401 2021-03-26 21:19:02.000000 inStrain-1.7.6/inStrain/logUtils.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    15346 2023-05-16 21:08:22.000000 inStrain-1.7.6/inStrain/parse_annotations.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-07-26 21:40:17.215740 inStrain-1.7.6/inStrain/plotting/
+-rw-r--r--   0 mattolm    (501) staff       (20)     2524 2023-02-24 18:53:38.000000 inStrain-1.7.6/inStrain/plotting/SNV_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)      662 2021-02-12 01:00:32.000000 inStrain-1.7.6/inStrain/plotting/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     9260 2023-02-25 01:38:35.000000 inStrain-1.7.6/inStrain/plotting/compare_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     2548 2021-02-12 01:00:32.000000 inStrain-1.7.6/inStrain/plotting/gene_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     6638 2023-02-24 18:50:29.000000 inStrain-1.7.6/inStrain/plotting/linkage_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     9075 2023-02-25 00:47:19.000000 inStrain-1.7.6/inStrain/plotting/mapping_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     5332 2023-02-25 00:49:14.000000 inStrain-1.7.6/inStrain/plotting/plotting_controller.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    18496 2023-07-26 21:15:53.000000 inStrain-1.7.6/inStrain/plotting/positional_plots.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     2831 2021-02-12 01:00:32.000000 inStrain-1.7.6/inStrain/plotting/utilities.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    20770 2023-07-26 21:10:50.000000 inStrain-1.7.6/inStrain/polymorpher.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-07-26 21:40:17.217284 inStrain-1.7.6/inStrain/profile/
+-rw-r--r--   0 mattolm    (501) staff       (20)      636 2021-01-21 18:18:24.000000 inStrain-1.7.6/inStrain/profile/__init__.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     5822 2021-02-12 01:00:32.000000 inStrain-1.7.6/inStrain/profile/fasta.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     9115 2021-01-21 18:18:24.000000 inStrain-1.7.6/inStrain/profile/linkage.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    15636 2021-01-21 18:18:24.000000 inStrain-1.7.6/inStrain/profile/profile_controller.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    32820 2023-02-24 18:17:07.000000 inStrain-1.7.6/inStrain/profile/profile_utilities.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     3144 2021-02-17 23:42:47.000000 inStrain-1.7.6/inStrain/profile/samtools_ops.py
+-rw-r--r--   0 mattolm    (501) staff       (20)    10361 2021-02-12 01:00:32.000000 inStrain-1.7.6/inStrain/profile/snv_utilities.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     5332 2021-02-12 01:00:32.000000 inStrain-1.7.6/inStrain/quickProfile.py
+-rwxr-xr-x   0 mattolm    (501) staff       (20)    16916 2022-06-10 19:12:50.000000 inStrain-1.7.6/inStrain/readComparer.py
+-rw-r--r--   0 mattolm    (501) staff       (20)     2629 2023-02-25 01:49:24.000000 inStrain-1.7.6/inStrain/utils.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-07-26 21:40:17.211823 inStrain-1.7.6/inStrain.egg-info/
+-rw-r--r--   0 mattolm    (501) staff       (20)      279 2023-07-26 21:40:16.000000 inStrain-1.7.6/inStrain.egg-info/PKG-INFO
+-rw-r--r--   0 mattolm    (501) staff       (20)     1563 2023-07-26 21:40:17.000000 inStrain-1.7.6/inStrain.egg-info/SOURCES.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)        1 2023-07-26 21:40:16.000000 inStrain-1.7.6/inStrain.egg-info/dependency_links.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)        1 2023-02-25 02:21:32.000000 inStrain-1.7.6/inStrain.egg-info/not-zip-safe
+-rw-r--r--   0 mattolm    (501) staff       (20)      113 2023-07-26 21:40:16.000000 inStrain-1.7.6/inStrain.egg-info/requires.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)       16 2023-07-26 21:40:16.000000 inStrain-1.7.6/inStrain.egg-info/top_level.txt
+-rw-r--r--   0 mattolm    (501) staff       (20)       38 2023-07-26 21:40:17.217985 inStrain-1.7.6/setup.cfg
+-rw-r--r--   0 mattolm    (501) staff       (20)     1051 2023-02-25 02:18:49.000000 inStrain-1.7.6/setup.py
+drwxr-xr-x   0 mattolm    (501) staff       (20)        0 2023-07-26 21:40:17.217546 inStrain-1.7.6/test/
+-rwxr-xr-x   0 mattolm    (501) staff       (20)     1213 2022-06-10 19:12:50.000000 inStrain-1.7.6/test/test_suite.py
```

### Comparing `inStrain-1.7.5/LICENSE` & `inStrain-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/README.md` & `inStrain-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/bin/inStrain` & `inStrain-1.7.6/bin/inStrain`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/docker/job_utils.py` & `inStrain-1.7.6/docker/job_utils.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/docker/run_instrain.py` & `inStrain-1.7.6/docker/run_instrain.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/docker/s3_utils.py` & `inStrain-1.7.6/docker/s3_utils.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/GeneProfile.py` & `inStrain-1.7.6/inStrain/GeneProfile.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/SNVprofile.py` & `inStrain-1.7.6/inStrain/SNVprofile.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/argumentParser.py` & `inStrain-1.7.6/inStrain/argumentParser.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/compare_controller.py` & `inStrain-1.7.6/inStrain/compare_controller.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/compare_greedy.py` & `inStrain-1.7.6/inStrain/compare_greedy.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/compare_utils.py` & `inStrain-1.7.6/inStrain/compare_utils.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/controller.py` & `inStrain-1.7.6/inStrain/controller.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/deprecated/DEPRECATEDmapping_plots.py` & `inStrain-1.7.6/inStrain/deprecated/DEPRECATEDmapping_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/deprecated/__init__.py` & `inStrain-1.7.6/inStrain/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/deprecated/deprecated_filter_reads.py` & `inStrain-1.7.6/inStrain/deprecated/deprecated_filter_reads.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/deprecated/deprecated_gene_statistics.py` & `inStrain-1.7.6/inStrain/deprecated/deprecated_gene_statistics.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/deprecated/plottingUtilities.py` & `inStrain-1.7.6/inStrain/deprecated/plottingUtilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/filter_reads.py` & `inStrain-1.7.6/inStrain/filter_reads.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/genomeUtilities.py` & `inStrain-1.7.6/inStrain/genomeUtilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/helper_files/NullModel.txt` & `inStrain-1.7.6/inStrain/helper_files/NullModel.txt`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/irep_utilities.py` & `inStrain-1.7.6/inStrain/irep_utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/logUtils.py` & `inStrain-1.7.6/inStrain/logUtils.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/parse_annotations.py` & `inStrain-1.7.6/inStrain/parse_annotations.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/plotting/SNV_plots.py` & `inStrain-1.7.6/inStrain/plotting/SNV_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/plotting/__init__.py` & `inStrain-1.7.6/inStrain/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/plotting/compare_plots.py` & `inStrain-1.7.6/inStrain/plotting/compare_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/plotting/gene_plots.py` & `inStrain-1.7.6/inStrain/plotting/gene_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/plotting/linkage_plots.py` & `inStrain-1.7.6/inStrain/plotting/linkage_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/plotting/mapping_plots.py` & `inStrain-1.7.6/inStrain/plotting/mapping_plots.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/plotting/plotting_controller.py` & `inStrain-1.7.6/inStrain/plotting/plotting_controller.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/plotting/positional_plots.py` & `inStrain-1.7.6/inStrain/plotting/positional_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,14 +354,16 @@
         Wdb = pd.DataFrame()
     return Wdb#, breaks
 
 def load_windowed_linkage(Ldb, scaffolds, window_len, mms, ANI_levels, s2l, on='r2'):
 
     # Get the linkage table
     #Ldb = IS.get('raw_linkage_table')
+    if len(Ldb) == 0:
+        return pd.DataFrame()
     Ldb = Ldb[Ldb['scaffold'].isin(scaffolds)].sort_values('mm')
     got_scaffolds = set(Ldb['scaffold'].unique())
 
     # Make the windows
     dbs = []
     tally = 0
     breaks = []
```

### Comparing `inStrain-1.7.5/inStrain/plotting/utilities.py` & `inStrain-1.7.6/inStrain/plotting/utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/polymorpher.py` & `inStrain-1.7.6/inStrain/polymorpher.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
                 name2scaffs[name].append(sc.scaffold)
                 if name in name2snpTable:
                     continue
                 db = isp.get('cumulative_snv_table').rename(
                     columns={'conBase': 'con_base', 'refBase': 'ref_base', 'varBase': 'var_base',
                              'baseCoverage': 'position_coverage'})
                 db = db[db['cryptic'] == False]
+                db['scaffold'] = db['scaffold'].astype(str)
                 if 'mm' in list(db.columns):
                     db = db.sort_values('mm').drop_duplicates(subset=['scaffold', 'position'], keep='last').sort_index().drop(columns=['mm'])
                 name2snpTable[name] = db
                 name2isp[name] = isp
 
         self.name2isp = name2isp
         self.name2snpTable = name2snpTable
```

### Comparing `inStrain-1.7.5/inStrain/profile/__init__.py` & `inStrain-1.7.6/inStrain/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/profile/fasta.py` & `inStrain-1.7.6/inStrain/profile/fasta.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/profile/linkage.py` & `inStrain-1.7.6/inStrain/profile/linkage.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/profile/profile_controller.py` & `inStrain-1.7.6/inStrain/profile/profile_controller.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/profile/profile_utilities.py` & `inStrain-1.7.6/inStrain/profile/profile_utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/profile/samtools_ops.py` & `inStrain-1.7.6/inStrain/profile/samtools_ops.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/profile/snv_utilities.py` & `inStrain-1.7.6/inStrain/profile/snv_utilities.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/quickProfile.py` & `inStrain-1.7.6/inStrain/quickProfile.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/readComparer.py` & `inStrain-1.7.6/inStrain/readComparer.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain/utils.py` & `inStrain-1.7.6/inStrain/utils.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/inStrain.egg-info/SOURCES.txt` & `inStrain-1.7.6/inStrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/setup.py` & `inStrain-1.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `inStrain-1.7.5/test/test_suite.py` & `inStrain-1.7.6/test/test_suite.py`

 * *Files identical despite different names*

