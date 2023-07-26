# Comparing `tmp/difi-1.2rc2.tar.gz` & `tmp/difi-1.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "difi-1.2rc2.tar", last modified: Thu Jul 20 04:38:13 2023, max compression
+gzip compressed data, was "difi-1.2rc3.tar", last modified: Wed Jul 26 15:35:16 2023, max compression
```

## Comparing `difi-1.2rc2.tar` & `difi-1.2rc3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:38:13.862130 difi-1.2rc2/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-20 04:38:02.000000 difi-1.2rc2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 04:38:02.000000 difi-1.2rc2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:38:13.842129 difi-1.2rc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:38:13.846130 difi-1.2rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-20 04:38:02.000000 difi-1.2rc2/.github/workflows/conda-build-lint-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-20 04:38:02.000000 difi-1.2rc2/.github/workflows/conda-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-20 04:38:02.000000 difi-1.2rc2/.github/workflows/docker-build-lint-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-20 04:38:02.000000 difi-1.2rc2/.github/workflows/pip-build-lint-test-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-20 04:38:02.000000 difi-1.2rc2/.github/workflows/pip-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-20 04:38:02.000000 difi-1.2rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 04:38:02.000000 difi-1.2rc2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-20 04:38:02.000000 difi-1.2rc2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-20 04:38:02.000000 difi-1.2rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-07-20 04:38:13.862130 difi-1.2rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-20 04:38:02.000000 difi-1.2rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 04:38:02.000000 difi-1.2rc2/additional_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:38:13.846130 difi-1.2rc2/difi/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/cifi.py
--rw-r--r--   0 runner    (1001) docker     (123)    32648 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/difi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:38:13.846130 difi-1.2rc2/difi/experimental/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9634 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/experimental/miniDifi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2814 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/experimental/rundifi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    51858 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:38:13.850129 difi-1.2rc2/difi/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/tests/linkagesByLine.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/tests/test_cifi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/tests/test_cifi_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)    22584 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/tests/test_difi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/tests/test_difi_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    21723 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/tests/test_metrics_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/tests/test_observations.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-07-20 04:38:02.000000 difi-1.2rc2/difi/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 04:38:13.000000 difi-1.2rc2/difi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:38:13.846130 difi-1.2rc2/difi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-07-20 04:38:13.000000 difi-1.2rc2/difi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-20 04:38:13.000000 difi-1.2rc2/difi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 04:38:13.000000 difi-1.2rc2/difi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 04:38:13.000000 difi-1.2rc2/difi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 04:38:13.000000 difi-1.2rc2/difi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:38:13.842129 difi-1.2rc2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:38:13.854130 difi-1.2rc2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    47096 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/all_linkages.png
--rw-r--r--   0 runner    (1001) docker     (123)    34794 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/cifi_all_truths.png
--rw-r--r--   0 runner    (1001) docker     (123)    71811 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/cifi_findable_observations.png
--rw-r--r--   0 runner    (1001) docker     (123)    36385 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/cifi_min_obs.png
--rw-r--r--   0 runner    (1001) docker     (123)    68507 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/cifi_nightly_linkages.png
--rw-r--r--   0 runner    (1001) docker     (123)    27811 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/cifi_summary_min_obs.png
--rw-r--r--   0 runner    (1001) docker     (123)    27696 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/cifi_summary_nightly_linkages.png
--rw-r--r--   0 runner    (1001) docker     (123)    31033 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/classes.png
--rw-r--r--   0 runner    (1001) docker     (123)   195279 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/classes_dict.png
--rw-r--r--   0 runner    (1001) docker     (123)    31772 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/difi.png
--rw-r--r--   0 runner    (1001) docker     (123)    58566 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/difi_all_truths.png
--rw-r--r--   0 runner    (1001) docker     (123)    41569 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/difi_summary.png
--rw-r--r--   0 runner    (1001) docker     (123)    32022 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/linkage_members.png
--rw-r--r--   0 runner    (1001) docker     (123)    49270 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/mixed_linkages.png
--rw-r--r--   0 runner    (1001) docker     (123)    79135 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/observations_noclasses.png
--rw-r--r--   0 runner    (1001) docker     (123)    92427 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/observations_withclasses.png
--rw-r--r--   0 runner    (1001) docker     (123)    51106 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/partial_linkages.png
--rw-r--r--   0 runner    (1001) docker     (123)    50131 2023-07-20 04:38:02.000000 difi-1.2rc2/docs/images/pure_linkages.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:38:13.862130 difi-1.2rc2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   113966 2023-07-20 04:38:02.000000 difi-1.2rc2/examples/classes.txt
--rw-r--r--   0 runner    (1001) docker     (123)  5051674 2023-07-20 04:38:02.000000 difi-1.2rc2/examples/linkage_members.txt
--rw-r--r--   0 runner    (1001) docker     (123)  6116213 2023-07-20 04:38:02.000000 difi-1.2rc2/examples/observations.txt
--rw-r--r--   0 runner    (1001) docker     (123)   196601 2023-07-20 04:38:02.000000 difi-1.2rc2/examples/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-20 04:38:02.000000 difi-1.2rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-20 04:38:02.000000 difi-1.2rc2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-20 04:38:13.866130 difi-1.2rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:35:16.254513 difi-1.2rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-26 15:35:02.000000 difi-1.2rc3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 15:35:02.000000 difi-1.2rc3/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:35:16.214513 difi-1.2rc3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:35:16.226513 difi-1.2rc3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-26 15:35:02.000000 difi-1.2rc3/.github/workflows/conda-build-lint-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-26 15:35:02.000000 difi-1.2rc3/.github/workflows/conda-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-26 15:35:02.000000 difi-1.2rc3/.github/workflows/docker-build-lint-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-26 15:35:02.000000 difi-1.2rc3/.github/workflows/pip-build-lint-test-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-26 15:35:02.000000 difi-1.2rc3/.github/workflows/pip-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-26 15:35:02.000000 difi-1.2rc3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-26 15:35:02.000000 difi-1.2rc3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-26 15:35:02.000000 difi-1.2rc3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-26 15:35:02.000000 difi-1.2rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-07-26 15:35:16.254513 difi-1.2rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-26 15:35:02.000000 difi-1.2rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 15:35:02.000000 difi-1.2rc3/additional_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:35:16.226513 difi-1.2rc3/difi/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/cifi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32648 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/difi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:35:16.230513 difi-1.2rc3/difi/experimental/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9634 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/experimental/miniDifi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2814 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/experimental/rundifi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53932 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:35:16.234513 difi-1.2rc3/difi/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/tests/linkagesByLine.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/tests/test_cifi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/tests/test_cifi_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22584 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/tests/test_difi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/tests/test_difi_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23412 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/tests/test_metrics_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/tests/test_observations.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-07-26 15:35:02.000000 difi-1.2rc3/difi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 15:35:15.000000 difi-1.2rc3/difi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:35:16.230513 difi-1.2rc3/difi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-07-26 15:35:16.000000 difi-1.2rc3/difi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-26 15:35:16.000000 difi-1.2rc3/difi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:35:16.000000 difi-1.2rc3/difi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 15:35:16.000000 difi-1.2rc3/difi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 15:35:16.000000 difi-1.2rc3/difi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:35:16.218513 difi-1.2rc3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:35:16.238513 difi-1.2rc3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    47096 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/all_linkages.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34794 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/cifi_all_truths.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71811 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/cifi_findable_observations.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36385 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/cifi_min_obs.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68507 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/cifi_nightly_linkages.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27811 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/cifi_summary_min_obs.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27696 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/cifi_summary_nightly_linkages.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31033 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/classes.png
+-rw-r--r--   0 runner    (1001) docker     (123)   195279 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/classes_dict.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31772 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/difi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    58566 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/difi_all_truths.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41569 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/difi_summary.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32022 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/linkage_members.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49270 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/mixed_linkages.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79135 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/observations_noclasses.png
+-rw-r--r--   0 runner    (1001) docker     (123)    92427 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/observations_withclasses.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51106 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/partial_linkages.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50131 2023-07-26 15:35:02.000000 difi-1.2rc3/docs/images/pure_linkages.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:35:16.254513 difi-1.2rc3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   113966 2023-07-26 15:35:02.000000 difi-1.2rc3/examples/classes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  5051674 2023-07-26 15:35:02.000000 difi-1.2rc3/examples/linkage_members.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  6116213 2023-07-26 15:35:02.000000 difi-1.2rc3/examples/observations.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   196601 2023-07-26 15:35:02.000000 difi-1.2rc3/examples/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-26 15:35:02.000000 difi-1.2rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 15:35:02.000000 difi-1.2rc3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-26 15:35:16.254513 difi-1.2rc3/setup.cfg
```

### Comparing `difi-1.2rc2/.github/workflows/conda-build-lint-test.yml` & `difi-1.2rc3/.github/workflows/conda-build-lint-test.yml`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/.github/workflows/conda-publish.yml` & `difi-1.2rc3/.github/workflows/conda-publish.yml`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/.github/workflows/docker-build-lint-test.yml` & `difi-1.2rc3/.github/workflows/docker-build-lint-test.yml`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/.github/workflows/pip-build-lint-test-coverage.yml` & `difi-1.2rc3/.github/workflows/pip-build-lint-test-coverage.yml`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/.github/workflows/pip-publish.yml` & `difi-1.2rc3/.github/workflows/pip-publish.yml`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/.gitignore` & `difi-1.2rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/.pre-commit-config.yaml` & `difi-1.2rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/LICENSE.md` & `difi-1.2rc3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/PKG-INFO` & `difi-1.2rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: difi
-Version: 1.2rc2
+Version: 1.2rc3
 Summary: Did I Find It?
 Author-email: Joachim Moeyens <moeyensj@uw.edu>
 Maintainer-email: Joachim Moeyens <moeyensj@uw.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2018-2023, Joachim Moeyens
         All rights reserved.
```

### Comparing `difi-1.2rc2/README.md` & `difi-1.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi/cifi.py` & `difi-1.2rc3/difi/cifi.py`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi/difi.py` & `difi-1.2rc3/difi/difi.py`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi/experimental/miniDifi.py` & `difi-1.2rc3/difi/experimental/miniDifi.py`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi/experimental/rundifi.py` & `difi-1.2rc3/difi/experimental/rundifi.py`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi/io.py` & `difi-1.2rc3/difi/io.py`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi/metrics.py` & `difi-1.2rc3/difi/metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import hashlib
 import multiprocessing as mp
+import os
 import warnings
 from abc import ABC, abstractmethod
 from itertools import combinations, repeat
 from multiprocessing import shared_memory
 from typing import Any, Dict, List, Optional, Tuple, TypeVar
 
 import numpy as np
@@ -552,31 +553,43 @@
         observations_array = np.empty(
             len(object_ids),
             dtype=dtypes,
         )
         self._num_observations = observations_array.shape[0]
         self._itemsize = observations_array.itemsize
 
-        shared_mem = shared_memory.SharedMemory("DIFI_ARRAY", create=True, size=observations_array.nbytes)
+        self._shared_memory_name = f"DIFI_ARRAY_{os.getpid()}"
+        shared_mem = shared_memory.SharedMemory(
+            self._shared_memory_name, create=True, size=observations_array.nbytes
+        )
         shared_memory_array = np.ndarray(
             observations_array.shape, dtype=observations_array.dtype, buffer=shared_mem.buf
         )
         shared_memory_array["object_id"] = object_ids
         shared_memory_array["obs_id"] = obs_ids
         shared_memory_array["time"] = times
         shared_memory_array["ra"] = ra
         shared_memory_array["dec"] = dec
         shared_memory_array["night"] = nights
         shared_mem.close()
         return
 
-    @staticmethod
-    def _clear_shared_record_array():
-        shared_mem = shared_memory.SharedMemory("DIFI_ARRAY")
+    def _clear_shared_record_array(self):
+        """
+        Clears the shared memory array for this instance of the metric.
+
+        Returns
+        -------
+        None
+        """
+        shared_mem = shared_memory.SharedMemory(self._shared_memory_name)
         shared_mem.unlink()
+        self._shared_memory_name = None
+        self._num_observations = 0
+        self._dtypes = None
 
     def _run_object_worker(
         self,
         object_slice: slice,
         windows: List[Tuple[int, int]],
         discovery_opportunities: bool = False,
         discovery_probability: float = 1.0,
@@ -622,15 +635,15 @@
                     "findable": np.nan,
                     "discovery_opportunities": np.nan,
                     "obs_ids": np.nan,
                 }
             ]
 
         # Load the observations from shared memory
-        existing_shared_mem = shared_memory.SharedMemory(name="DIFI_ARRAY")
+        existing_shared_mem = shared_memory.SharedMemory(name=self._shared_memory_name)
         observations = np.ndarray(
             num_obs,
             dtype=self._dtypes,
             buffer=existing_shared_mem.buf,
             offset=object_slice.start * self._itemsize,
         )
         object_id = observations["object_id"][0]
@@ -685,14 +698,15 @@
         self,
         observations: pd.DataFrame,
         windows: List[Tuple[int, int]],
         discovery_opportunities: bool = False,
         discovery_probability: float = 1.0,
         ignore_after_discovery: bool = False,
         num_jobs: Optional[int] = 1,
+        clear_on_failure: bool = True,
     ) -> List[pd.DataFrame]:
         """
         Run the findability metric on the observations split by objects. For windows where there are many
         observations, this may be faster than running the metric on each window individually
         (with all objects' observations).
 
         Parameters
@@ -714,14 +728,17 @@
             not be discovered.
         ignore_after_discovery : bool, optional
             If True, then ignore all observations after each object's initial discovery. If False,
             then each object's observations will continue to be tested for discovery in each window.
         num_jobs : int, optional
             The number of jobs to run in parallel. If 1, then run in serial. If None, then use the number of
             CPUs on the machine.
+        clear_on_failure : bool, optional
+            If a failure occurs and this is False, then the shared memory array will not be cleared.
+            If True, then the shared memory array will be cleared.
 
         Returns
         -------
         findable : List[`~pandas.DataFrame`]
             Dataframe containing the findable objects and the observations
             that made them findable for each window.
         """
@@ -734,47 +751,53 @@
             observations["dec"].values,
             observations["night"].values,
         )
 
         # Split arrays by object
         split_by_object_slices = self._split_by_object(objects)
 
-        # Store the observations in a global variable so that the worker functions can access them
-        self._store_as_shared_record_array(objects, obs_ids, times, ra, dec, nights)
-
-        findable_lists: List[List[Dict[str, Any]]] = []
-        if num_jobs is None or num_jobs > 1:
-            pool = mp.Pool(num_jobs)
-            findable_lists = pool.starmap(
-                self._run_object_worker,
-                zip(
-                    split_by_object_slices,
-                    repeat(windows),
-                    repeat(discovery_opportunities),
-                    repeat(discovery_probability),
-                    repeat(ignore_after_discovery),
-                ),
-            )
+        try:
+            # Store the observations in a global variable so that the worker functions can access them
+            self._store_as_shared_record_array(objects, obs_ids, times, ra, dec, nights)
+
+            findable_lists: List[List[Dict[str, Any]]] = []
+            if num_jobs is None or num_jobs > 1:
+                pool = mp.Pool(num_jobs)
+                findable_lists = pool.starmap(
+                    self._run_object_worker,
+                    zip(
+                        split_by_object_slices,
+                        repeat(windows),
+                        repeat(discovery_opportunities),
+                        repeat(discovery_probability),
+                        repeat(ignore_after_discovery),
+                    ),
+                )
 
-            pool.close()
-            pool.join()
+                pool.close()
+                pool.join()
 
-        else:
-            for object_indices in split_by_object_slices:
-                findable_lists.append(
-                    self._run_object_worker(
-                        object_indices,
-                        windows,
-                        discovery_opportunities=discovery_opportunities,
-                        discovery_probability=discovery_probability,
-                        ignore_after_discovery=ignore_after_discovery,
+            else:
+                for object_indices in split_by_object_slices:
+                    findable_lists.append(
+                        self._run_object_worker(
+                            object_indices,
+                            windows,
+                            discovery_opportunities=discovery_opportunities,
+                            discovery_probability=discovery_probability,
+                            ignore_after_discovery=ignore_after_discovery,
+                        )
                     )
-                )
 
-        self._clear_shared_record_array()
+            self._clear_shared_record_array()
+
+        except Exception as e:
+            if clear_on_failure:
+                self._clear_shared_record_array()
+            raise e
 
         findable_flattened = [item for sublist in findable_lists for item in sublist]
 
         findable = pd.DataFrame(findable_flattened)
         findable.dropna(subset=["window_id"], inplace=True)
         if len(findable) > 0:
             findable.loc[:, "window_id"] = findable["window_id"].astype(int)
@@ -828,15 +851,15 @@
                     "findable": np.nan,
                     "discovery_opportunities": np.nan,
                     "obs_ids": np.nan,
                 }
             ]
 
         # Read observations from shared memory array
-        existing_shared_mem = shared_memory.SharedMemory(name="DIFI_ARRAY")
+        existing_shared_mem = shared_memory.SharedMemory(name=self._shared_memory_name)
         observations = np.ndarray(
             num_obs,
             dtype=self._dtypes,
             buffer=existing_shared_mem.buf,
             offset=window_slice.start * self._itemsize,
         )
 
@@ -893,14 +916,15 @@
     def run_by_window(
         self,
         observations: pd.DataFrame,
         windows: List[Tuple[int, int]],
         discovery_opportunities: bool = False,
         discovery_probability: float = 1.0,
         num_jobs: Optional[int] = 1,
+        clear_on_failure: bool = True,
     ) -> List[pd.DataFrame]:
         """
         Run the findability metric on the observations split by windows where each window will
         contain all of the observations within a span of detection_window nights.
 
         Parameters
         ----------
@@ -918,14 +942,17 @@
             Each object will have a random seed generated from its object ID, and for each discovery
             opportunity a random number will be drawn between 0 and 1. If the random number is less
             than the discovery probability, then the object will be discovered. If not, then it will
             not be discovered.
         num_jobs : int, optional
             The number of jobs to run in parallel. If 1, then run in serial. If None, then use the number of
             CPUs on the machine.
+        clear_on_failure : bool, optional
+            If a failure occurs and this is False, then the shared memory array will not be cleared.
+            If True, then the shared memory array will be cleared.
 
         Returns
         -------
         findable : List[`~pandas.DataFrame`]
             Dataframe containing the findable objects and the observations
             that made them findable for each window.
         """
@@ -935,47 +962,53 @@
             observations["obs_id"].values.astype(str),
             observations["time"].values,
             observations["ra"].values,
             observations["dec"].values,
             observations["night"].values,
         )
 
-        # Store the observations in a global variable so that the worker functions can access them
-        self._store_as_shared_record_array(objects, obs_ids, times, ra, dec, nights)
-
-        # Find indices that split the observations into windows
-        split_by_window_slices = self._split_by_window(windows, nights)
-
-        findable_lists: List[List[Dict[str, Any]]] = []
-        if num_jobs is None or num_jobs > 1:
-            pool = mp.Pool(num_jobs)
-            findable_lists = pool.starmap(
-                self._run_window_worker,
-                zip(
-                    split_by_window_slices,
-                    range(len(windows)),
-                    repeat(discovery_opportunities),
-                    repeat(discovery_probability),
-                ),
-            )
-            pool.close()
-            pool.join()
+        try:
+            # Store the observations in a global variable so that the worker functions can access them
+            self._store_as_shared_record_array(objects, obs_ids, times, ra, dec, nights)
+
+            # Find indices that split the observations into windows
+            split_by_window_slices = self._split_by_window(windows, nights)
+
+            findable_lists: List[List[Dict[str, Any]]] = []
+            if num_jobs is None or num_jobs > 1:
+                pool = mp.Pool(num_jobs)
+                findable_lists = pool.starmap(
+                    self._run_window_worker,
+                    zip(
+                        split_by_window_slices,
+                        range(len(windows)),
+                        repeat(discovery_opportunities),
+                        repeat(discovery_probability),
+                    ),
+                )
+                pool.close()
+                pool.join()
 
-        else:
-            for i, window_slice in enumerate(split_by_window_slices):
-                findable_lists.append(
-                    self._run_window_worker(
-                        window_slice,
-                        i,
-                        discovery_opportunities=discovery_opportunities,
-                        discovery_probability=discovery_probability,
+            else:
+                for i, window_slice in enumerate(split_by_window_slices):
+                    findable_lists.append(
+                        self._run_window_worker(
+                            window_slice,
+                            i,
+                            discovery_opportunities=discovery_opportunities,
+                            discovery_probability=discovery_probability,
+                        )
                     )
-                )
 
-        self._clear_shared_record_array()
+            self._clear_shared_record_array()
+
+        except Exception as e:
+            if clear_on_failure:
+                self._clear_shared_record_array()
+            raise e
 
         findable_flattened = [item for sublist in findable_lists for item in sublist]
 
         findable = pd.DataFrame(findable_flattened)
         findable.dropna(subset=["window_id"], inplace=True)
         if len(findable) > 0:
             findable.loc[:, "window_id"] = findable["window_id"].astype(int)
@@ -991,15 +1024,17 @@
         detection_window: Optional[int] = None,
         min_window_nights: Optional[int] = None,
         discovery_opportunities: bool = False,
         discovery_probability: float = 1.0,
         by_object: bool = False,
         ignore_after_discovery: bool = False,
         num_jobs: Optional[int] = 1,
-    ) -> Tuple[pd.DataFrame, pd.DataFrame]:
+        return_summary: bool = True,
+        clear_on_failure: bool = True,
+    ) -> Tuple[pd.DataFrame, Optional[pd.DataFrame]]:
         """
         Run the findability metric on the observations.
 
         Parameters
         ----------
         observations : `~pandas.DataFrame`
             Observations dataframe containing at least the following columns:
@@ -1032,14 +1067,20 @@
             (with all objects' observations).
         ignore_after_discovery : bool, optional
             If True, then ignore observations that occur after the object has been discovered. Only applies
             when by_object is True. If False, then the objects will be tested for discovery chances again.
         num_jobs : int, optional
             The number of jobs to run in parallel. If 1, then run in serial. If None, then use the number of
             CPUs on the machine.
+        return_summary : bool, optional
+            If True, then return a summary of the number of observations, number of findable
+            objects and the start and end night of each window.
+        clear_on_failure : bool, optional
+            If a failure occurs and this is False, then the shared memory array will not be cleared.
+            If True, then the shared memory array will be cleared.
 
         Returns
         -------
         findable : `~pandas.DataFrame`
             A dataframe containing the object IDs that are findable and a column
             with a list of the observation IDs that made the object findable.
         window_summary : `~pandas.DataFrame`
@@ -1063,25 +1104,30 @@
             findable = self.run_by_object(
                 observations,
                 windows,
                 discovery_opportunities=discovery_opportunities,
                 discovery_probability=discovery_probability,
                 ignore_after_discovery=ignore_after_discovery,
                 num_jobs=num_jobs,
+                clear_on_failure=clear_on_failure,
             )
         else:
             findable = self.run_by_window(
                 observations,
                 windows,
                 discovery_opportunities=discovery_opportunities,
                 discovery_probability=discovery_probability,
                 num_jobs=num_jobs,
+                clear_on_failure=clear_on_failure,
             )
 
-        window_summary = self._create_window_summary(observations, windows, findable)
+        if return_summary:
+            window_summary = self._create_window_summary(observations, windows, findable)
+        else:
+            window_summary = None
         return findable, window_summary
 
 
 class NightlyLinkagesMetric(FindabilityMetric):
     def __init__(
         self,
         linkage_min_obs: int = 2,
```

### Comparing `difi-1.2rc2/difi/tests/conftest.py` & `difi-1.2rc3/difi/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi/tests/test_cifi.py` & `difi-1.2rc3/difi/tests/test_cifi.py`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi/tests/test_cifi_benchmarks.py` & `difi-1.2rc3/difi/tests/test_cifi_benchmarks.py`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi/tests/test_difi.py` & `difi-1.2rc3/difi/tests/test_difi.py`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi/tests/test_difi_benchmarks.py` & `difi-1.2rc3/difi/tests/test_difi_benchmarks.py`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi/tests/test_io.py` & `difi-1.2rc3/difi/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi/tests/test_metrics.py` & `difi-1.2rc3/difi/tests/test_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+import os
+
 import numpy as np
+import pandas as pd
 import pytest
 
 from ..metrics import (
     FindabilityMetric,
     MinObsMetric,
     NightlyLinkagesMetric,
     find_observations_beyond_angular_separation,
@@ -482,7 +485,52 @@
 
 def test_calcFindableMinObs_assertion(test_observations):
     # Check that an assertion is raised if more than one object's observations
     # are passed to the metric's determine_object_findable method
     with pytest.raises(AssertionError):
         metric = MinObsMetric()
         metric.determine_object_findable(test_observations)
+
+
+def test_FindabilityMetrics_shared_memory(test_observations):
+    # Check that the function stores the observations in shared memory under
+    # the correct name
+    metric = MinObsMetric()
+
+    # Extract the data from the test observations
+    object_ids = test_observations["object_id"].values
+    obs_ids = test_observations["obs_id"].values
+    time = test_observations["time"].values
+    ra = test_observations["ra"].values
+    dec = test_observations["dec"].values
+    night = test_observations["night"].values
+
+    # Store the observations in shared memory
+    metric._store_as_shared_record_array(object_ids, obs_ids, time, ra, dec, night)
+
+    # Check that the shared memory array has the correct name
+    assert metric._shared_memory_name == f"DIFI_ARRAY_{os.getpid()}"
+    assert metric._num_observations == len(test_observations)
+    assert metric._dtypes == [
+        ("object_id", object_ids.dtype),
+        ("obs_id", obs_ids.dtype),
+        ("time", np.float64),
+        ("ra", np.float64),
+        ("dec", np.float64),
+        ("night", np.int64),
+    ]
+
+    metric._clear_shared_record_array()
+    assert metric._shared_memory_name is None
+    assert metric._num_observations == 0
+    assert metric._dtypes is None
+
+
+def test_FindabilityMetrics_run_return_summary(test_observations):
+    # Check that the function returns the summary dataframe when desired
+    metric = MinObsMetric()
+
+    findable, window_summary = metric.run(test_observations, return_summary=True)
+    assert isinstance(window_summary, pd.DataFrame)
+
+    findable, window_summary = metric.run(test_observations, return_summary=False)
+    assert window_summary is None
```

### Comparing `difi-1.2rc2/difi/tests/test_metrics_benchmarks.py` & `difi-1.2rc3/difi/tests/test_metrics_benchmarks.py`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi/tests/test_observations.csv` & `difi-1.2rc3/difi/tests/test_observations.csv`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi/tests/test_utils.py` & `difi-1.2rc3/difi/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi/utils.py` & `difi-1.2rc3/difi/utils.py`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/difi.egg-info/PKG-INFO` & `difi-1.2rc3/difi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: difi
-Version: 1.2rc2
+Version: 1.2rc3
 Summary: Did I Find It?
 Author-email: Joachim Moeyens <moeyensj@uw.edu>
 Maintainer-email: Joachim Moeyens <moeyensj@uw.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2018-2023, Joachim Moeyens
         All rights reserved.
```

### Comparing `difi-1.2rc2/difi.egg-info/SOURCES.txt` & `difi-1.2rc3/difi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/all_linkages.png` & `difi-1.2rc3/docs/images/all_linkages.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/cifi_all_truths.png` & `difi-1.2rc3/docs/images/cifi_all_truths.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/cifi_findable_observations.png` & `difi-1.2rc3/docs/images/cifi_findable_observations.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/cifi_min_obs.png` & `difi-1.2rc3/docs/images/cifi_min_obs.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/cifi_nightly_linkages.png` & `difi-1.2rc3/docs/images/cifi_nightly_linkages.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/cifi_summary_min_obs.png` & `difi-1.2rc3/docs/images/cifi_summary_min_obs.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/cifi_summary_nightly_linkages.png` & `difi-1.2rc3/docs/images/cifi_summary_nightly_linkages.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/classes.png` & `difi-1.2rc3/docs/images/classes.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/classes_dict.png` & `difi-1.2rc3/docs/images/classes_dict.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/difi.png` & `difi-1.2rc3/docs/images/difi.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/difi_all_truths.png` & `difi-1.2rc3/docs/images/difi_all_truths.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/difi_summary.png` & `difi-1.2rc3/docs/images/difi_summary.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/linkage_members.png` & `difi-1.2rc3/docs/images/linkage_members.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/mixed_linkages.png` & `difi-1.2rc3/docs/images/mixed_linkages.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/observations_noclasses.png` & `difi-1.2rc3/docs/images/observations_noclasses.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/observations_withclasses.png` & `difi-1.2rc3/docs/images/observations_withclasses.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/partial_linkages.png` & `difi-1.2rc3/docs/images/partial_linkages.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/docs/images/pure_linkages.png` & `difi-1.2rc3/docs/images/pure_linkages.png`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/examples/classes.txt` & `difi-1.2rc3/examples/classes.txt`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/examples/linkage_members.txt` & `difi-1.2rc3/examples/linkage_members.txt`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/examples/observations.txt` & `difi-1.2rc3/examples/observations.txt`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/examples/tutorial.ipynb` & `difi-1.2rc3/examples/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `difi-1.2rc2/pyproject.toml` & `difi-1.2rc3/pyproject.toml`

 * *Files identical despite different names*

