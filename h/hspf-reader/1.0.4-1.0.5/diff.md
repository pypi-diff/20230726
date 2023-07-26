# Comparing `tmp/hspf_reader-1.0.4.tar.gz` & `tmp/hspf_reader-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspf_reader-1.0.4.tar", last modified: Fri Jun 16 20:42:06 2023, max compression
+gzip compressed data, was "hspf_reader-1.0.5.tar", last modified: Wed Jul 26 04:04:52 2023, max compression
```

## Comparing `hspf_reader-1.0.4.tar` & `hspf_reader-1.0.5.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.849324 hspf_reader-1.0.4/
--rw-r--r--   0 tim       (1000) tim       (1000)      102 2023-06-16 20:30:10.000000 hspf_reader-1.0.4/.deepsource.toml
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.829324 hspf_reader-1.0.4/.github/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.837324 hspf_reader-1.0.4/.github/workflows/
--rw-r--r--   0 tim       (1000) tim       (1000)      501 2023-06-16 20:30:10.000000 hspf_reader-1.0.4/.github/workflows/clean-workflow-runs.yml
--rw-r--r--   0 tim       (1000) tim       (1000)     2121 2023-06-16 20:30:10.000000 hspf_reader-1.0.4/.github/workflows/python-package.yml
--rw-r--r--   0 tim       (1000) tim       (1000)      335 2023-03-05 18:51:19.000000 hspf_reader-1.0.4/.gitignore
--rw-rw-r--   0 tim       (1000) tim       (1000)     2651 2023-06-16 20:30:10.000000 hspf_reader-1.0.4/.pre-commit-config.yaml
--rw-r--r--   0 tim       (1000) tim       (1000)       50 2022-08-30 21:29:29.000000 hspf_reader-1.0.4/AUTHORS.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1036 2022-09-27 21:47:42.000000 hspf_reader-1.0.4/BADGES.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      885 2023-06-16 20:39:46.000000 hspf_reader-1.0.4/CHANGELOG.md
--rw-r--r--   0 tim       (1000) tim       (1000)     3179 2022-08-30 21:29:29.000000 hspf_reader-1.0.4/CONTRIBUTING.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1488 2022-08-30 21:29:29.000000 hspf_reader-1.0.4/LICENSE.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      339 2022-09-23 07:37:30.000000 hspf_reader-1.0.4/MANIFEST.in
--rw-rw-r--   0 tim       (1000) tim       (1000)     4171 2023-06-16 20:42:06.849324 hspf_reader-1.0.4/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)     2676 2023-06-10 05:29:49.000000 hspf_reader-1.0.4/README.rst
--rw-r--r--   0 tim       (1000) tim       (1000)        6 2023-06-16 20:39:46.000000 hspf_reader-1.0.4/VERSION
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.841324 hspf_reader-1.0.4/docs/
--rw-r--r--   0 tim       (1000) tim       (1000)     5712 2022-08-30 21:28:21.000000 hspf_reader-1.0.4/docs/Makefile
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.841324 hspf_reader-1.0.4/docs/_function_autosummary/
--rw-rw-r--   0 tim       (1000) tim       (1000)      135 2023-06-16 18:22:12.000000 hspf_reader-1.0.4/docs/_function_autosummary/hspf_reader.hspf_reader.about.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      129 2023-06-16 18:22:12.000000 hspf_reader-1.0.4/docs/_function_autosummary/hspf_reader.hspf_reader.hbn.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      141 2023-06-16 18:22:12.000000 hspf_reader-1.0.4/docs/_function_autosummary/hspf_reader.hspf_reader.plotgen.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      129 2023-06-16 18:22:12.000000 hspf_reader-1.0.4/docs/_function_autosummary/hspf_reader.hspf_reader.wdm.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       55 2022-11-05 05:41:26.000000 hspf_reader-1.0.4/docs/authors.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      360 2023-05-13 04:19:29.000000 hspf_reader-1.0.4/docs/command_line.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     9668 2023-01-22 03:38:21.000000 hspf_reader-1.0.4/docs/conf.py
--rw-r--r--   0 tim       (1000) tim       (1000)       60 2022-11-05 05:41:26.000000 hspf_reader-1.0.4/docs/contributing.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      273 2023-05-13 04:10:12.000000 hspf_reader-1.0.4/docs/function_summary.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      466 2022-11-05 05:42:41.000000 hspf_reader-1.0.4/docs/index.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       79 2022-11-05 05:41:26.000000 hspf_reader-1.0.4/docs/license.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     5104 2022-08-30 21:28:21.000000 hspf_reader-1.0.4/docs/make.bat
--rw-r--r--   0 tim       (1000) tim       (1000)       27 2022-11-05 05:41:26.000000 hspf_reader-1.0.4/docs/readme.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     2942 2023-06-16 20:39:46.000000 hspf_reader-1.0.4/pyproject.toml
--rw-r--r--   0 tim       (1000) tim       (1000)      261 2022-10-16 16:07:40.000000 hspf_reader-1.0.4/requirements.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-06-16 20:42:06.849324 hspf_reader-1.0.4/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)      515 2023-03-01 21:50:42.000000 hspf_reader-1.0.4/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.833324 hspf_reader-1.0.4/src/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.841324 hspf_reader-1.0.4/src/hspf_reader/
--rw-r--r--   0 tim       (1000) tim       (1000)       67 2023-01-22 03:38:21.000000 hspf_reader-1.0.4/src/hspf_reader/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    10202 2023-06-16 20:29:41.000000 hspf_reader-1.0.4/src/hspf_reader/hspf_reader.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.845324 hspf_reader-1.0.4/src/hspf_reader.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)     4171 2023-06-16 20:42:06.000000 hspf_reader-1.0.4/src/hspf_reader.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     1280 2023-06-16 20:42:06.000000 hspf_reader-1.0.4/src/hspf_reader.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-06-16 20:42:06.000000 hspf_reader-1.0.4/src/hspf_reader.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       61 2023-06-16 20:42:06.000000 hspf_reader-1.0.4/src/hspf_reader.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      296 2023-06-16 20:42:06.000000 hspf_reader-1.0.4/src/hspf_reader.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       12 2023-06-16 20:42:06.000000 hspf_reader-1.0.4/src/hspf_reader.egg-info/top_level.txt
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-16 20:42:06.849324 hspf_reader-1.0.4/tests/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2023-01-22 03:38:21.000000 hspf_reader-1.0.4/tests/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)      482 2023-01-22 03:38:21.000000 hspf_reader-1.0.4/tests/capture.py
--rw-r--r--   0 tim       (1000) tim       (1000)    81920 2022-08-30 21:28:23.000000 hspf_reader-1.0.4/tests/data.wdm
--rw-r--r--   0 tim       (1000) tim       (1000)   822321 2022-08-30 21:28:23.000000 hspf_reader-1.0.4/tests/data_6b_np1.hbn
--rw-rw-r--   0 tim       (1000) tim       (1000)    62131 2022-08-31 19:57:44.000000 hspf_reader-1.0.4/tests/data_plotgen.plt
--rw-rw-r--   0 tim       (1000) tim       (1000)   172779 2022-09-27 13:00:11.000000 hspf_reader-1.0.4/tests/data_wdm_1.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)   264240 2022-09-27 13:13:16.000000 hspf_reader-1.0.4/tests/data_wdm_2.csv
--rw-r--r--   0 tim       (1000) tim       (1000)   822321 2022-09-21 23:17:47.000000 hspf_reader-1.0.4/tests/data_yearly.hbn
--rw-rw-r--   0 tim       (1000) tim       (1000)        0 2022-08-31 21:31:44.000000 hspf_reader-1.0.4/tests/debug_hspf_reader
--rw-r--r--   0 tim       (1000) tim       (1000)    30250 2022-09-21 23:52:50.000000 hspf_reader-1.0.4/tests/sunspot_area.csv
--rw-r--r--   0 tim       (1000) tim       (1000)    15138 2022-09-21 23:53:58.000000 hspf_reader-1.0.4/tests/sunspot_area_with_missing.csv
--rw-r--r--   0 tim       (1000) tim       (1000)     2486 2023-01-22 03:38:21.000000 hspf_reader-1.0.4/tests/test_hbn.py
--rw-r--r--   0 tim       (1000) tim       (1000)    35491 2023-01-22 03:38:21.000000 hspf_reader-1.0.4/tests/test_plotgen.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1239 2023-02-14 05:41:44.000000 hspf_reader-1.0.4/tests/test_wdm.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:04:52.043013 hspf_reader-1.0.5/
+-rw-r--r--   0 tim       (1000) tim       (1000)      102 2023-06-17 22:11:34.000000 hspf_reader-1.0.5/.deepsource.toml
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:04:52.035013 hspf_reader-1.0.5/.github/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:04:52.039013 hspf_reader-1.0.5/.github/workflows/
+-rw-r--r--   0 tim       (1000) tim       (1000)      501 2023-06-17 22:11:34.000000 hspf_reader-1.0.5/.github/workflows/clean-workflow-runs.yml
+-rw-r--r--   0 tim       (1000) tim       (1000)     2121 2023-06-17 22:11:34.000000 hspf_reader-1.0.5/.github/workflows/python-package.yml
+-rw-r--r--   0 tim       (1000) tim       (1000)      335 2023-03-05 18:51:19.000000 hspf_reader-1.0.5/.gitignore
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2651 2023-07-17 01:12:50.000000 hspf_reader-1.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 tim       (1000) tim       (1000)       50 2022-08-30 21:29:29.000000 hspf_reader-1.0.5/AUTHORS.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1036 2022-09-27 21:47:42.000000 hspf_reader-1.0.5/BADGES.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      909 2023-07-26 03:27:42.000000 hspf_reader-1.0.5/CHANGELOG.md
+-rw-r--r--   0 tim       (1000) tim       (1000)     3179 2022-08-30 21:29:29.000000 hspf_reader-1.0.5/CONTRIBUTING.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1488 2022-08-30 21:29:29.000000 hspf_reader-1.0.5/LICENSE.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      339 2022-09-23 07:37:30.000000 hspf_reader-1.0.5/MANIFEST.in
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4171 2023-07-26 04:04:52.043013 hspf_reader-1.0.5/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)     2676 2023-06-10 05:29:49.000000 hspf_reader-1.0.5/README.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)        6 2023-07-26 03:27:42.000000 hspf_reader-1.0.5/VERSION
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:04:52.039013 hspf_reader-1.0.5/docs/
+-rw-r--r--   0 tim       (1000) tim       (1000)     5712 2022-08-30 21:28:21.000000 hspf_reader-1.0.5/docs/Makefile
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:04:52.039013 hspf_reader-1.0.5/docs/_function_autosummary/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      129 2023-06-19 14:23:37.000000 hspf_reader-1.0.5/docs/_function_autosummary/hspf_reader.hspf_reader.hbn.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      141 2023-06-19 14:23:37.000000 hspf_reader-1.0.5/docs/_function_autosummary/hspf_reader.hspf_reader.plotgen.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      129 2023-06-19 14:23:37.000000 hspf_reader-1.0.5/docs/_function_autosummary/hspf_reader.hspf_reader.wdm.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       55 2022-11-05 05:41:26.000000 hspf_reader-1.0.5/docs/authors.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      360 2023-05-13 04:19:29.000000 hspf_reader-1.0.5/docs/command_line.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     9668 2023-01-22 03:38:21.000000 hspf_reader-1.0.5/docs/conf.py
+-rw-r--r--   0 tim       (1000) tim       (1000)       60 2022-11-05 05:41:26.000000 hspf_reader-1.0.5/docs/contributing.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      239 2023-06-17 04:59:13.000000 hspf_reader-1.0.5/docs/function_summary.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      466 2022-11-05 05:42:41.000000 hspf_reader-1.0.5/docs/index.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       79 2022-11-05 05:41:26.000000 hspf_reader-1.0.5/docs/license.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     5104 2022-08-30 21:28:21.000000 hspf_reader-1.0.5/docs/make.bat
+-rw-r--r--   0 tim       (1000) tim       (1000)       27 2022-11-05 05:41:26.000000 hspf_reader-1.0.5/docs/readme.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2942 2023-07-26 03:27:42.000000 hspf_reader-1.0.5/pyproject.toml
+-rw-r--r--   0 tim       (1000) tim       (1000)      261 2022-10-16 16:07:40.000000 hspf_reader-1.0.5/requirements.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-07-26 04:04:52.043013 hspf_reader-1.0.5/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)      515 2023-03-01 21:50:42.000000 hspf_reader-1.0.5/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:04:52.035013 hspf_reader-1.0.5/src/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:04:52.039013 hspf_reader-1.0.5/src/hspf_reader/
+-rw-r--r--   0 tim       (1000) tim       (1000)       67 2023-01-22 03:38:21.000000 hspf_reader-1.0.5/src/hspf_reader/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    10202 2023-06-16 20:29:41.000000 hspf_reader-1.0.5/src/hspf_reader/hspf_reader.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:04:52.039013 hspf_reader-1.0.5/src/hspf_reader.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4171 2023-07-26 04:04:51.000000 hspf_reader-1.0.5/src/hspf_reader.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1219 2023-07-26 04:04:52.000000 hspf_reader-1.0.5/src/hspf_reader.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-07-26 04:04:51.000000 hspf_reader-1.0.5/src/hspf_reader.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       61 2023-07-26 04:04:51.000000 hspf_reader-1.0.5/src/hspf_reader.egg-info/entry_points.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      296 2023-07-26 04:04:51.000000 hspf_reader-1.0.5/src/hspf_reader.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       12 2023-07-26 04:04:51.000000 hspf_reader-1.0.5/src/hspf_reader.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-07-26 04:04:52.043013 hspf_reader-1.0.5/tests/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2023-01-22 03:38:21.000000 hspf_reader-1.0.5/tests/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)      482 2023-01-22 03:38:21.000000 hspf_reader-1.0.5/tests/capture.py
+-rw-r--r--   0 tim       (1000) tim       (1000)    81920 2022-08-30 21:28:23.000000 hspf_reader-1.0.5/tests/data.wdm
+-rw-r--r--   0 tim       (1000) tim       (1000)   822321 2022-08-30 21:28:23.000000 hspf_reader-1.0.5/tests/data_6b_np1.hbn
+-rw-rw-r--   0 tim       (1000) tim       (1000)    62131 2022-08-31 19:57:44.000000 hspf_reader-1.0.5/tests/data_plotgen.plt
+-rw-rw-r--   0 tim       (1000) tim       (1000)   172779 2022-09-27 13:00:11.000000 hspf_reader-1.0.5/tests/data_wdm_1.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)   264240 2022-09-27 13:13:16.000000 hspf_reader-1.0.5/tests/data_wdm_2.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)   822321 2022-09-21 23:17:47.000000 hspf_reader-1.0.5/tests/data_yearly.hbn
+-rw-rw-r--   0 tim       (1000) tim       (1000)        0 2022-08-31 21:31:44.000000 hspf_reader-1.0.5/tests/debug_hspf_reader
+-rw-r--r--   0 tim       (1000) tim       (1000)    30250 2022-09-21 23:52:50.000000 hspf_reader-1.0.5/tests/sunspot_area.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)    15138 2022-09-21 23:53:58.000000 hspf_reader-1.0.5/tests/sunspot_area_with_missing.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)     2486 2023-01-22 03:38:21.000000 hspf_reader-1.0.5/tests/test_hbn.py
+-rw-r--r--   0 tim       (1000) tim       (1000)    35491 2023-01-22 03:38:21.000000 hspf_reader-1.0.5/tests/test_plotgen.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1239 2023-02-14 05:41:44.000000 hspf_reader-1.0.5/tests/test_wdm.py
```

### Comparing `hspf_reader-1.0.4/.github/workflows/python-package.yml` & `hspf_reader-1.0.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/.pre-commit-config.yaml` & `hspf_reader-1.0.5/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     - repo: https://github.com/lovesegfault/beautysh
       rev: v6.2.1
       hooks:
           - id: beautysh
             args: [--indent-size, '4']
 
     - repo: https://github.com/psf/black
-      rev: 23.3.0
+      rev: 23.7.0
       hooks:
           - id: black
           - id: black-jupyter
 
     - repo: https://github.com/pycqa/isort
       rev: 5.12.0
       hooks:
@@ -69,27 +69,27 @@
             args: [--profile, black, --filter-files]
           - id: isort
             name: isort (pyi)
             types: [pyi]
             args: [--profile, black, --filter-files]
 
     - repo: https://github.com/asottile/blacken-docs
-      rev: 1.13.0
+      rev: 1.15.0
       hooks:
           - id: blacken-docs
 
     - repo: https://github.com/asottile/pyupgrade
-      rev: v3.6.0
+      rev: v3.9.0
       hooks:
           - id: pyupgrade
 
     - repo: https://github.com/commitizen-tools/commitizen
-      rev: 3.2.2
+      rev: 3.5.3
       hooks:
           - id: commitizen
             stages: [commit-msg]
 
     - repo: https://github.com/mwouts/jupytext
-      rev: v1.14.6
+      rev: v1.14.7
       hooks:
           - id: jupytext
             args: [--from, ipynb, --to, auto:percent, --sync]
```

### Comparing `hspf_reader-1.0.4/BADGES.rst` & `hspf_reader-1.0.5/BADGES.rst`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/CHANGELOG.md` & `hspf_reader-1.0.5/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+## v1.0.5 (2023-07-25)
+
 ## v1.0.4 (2023-06-16)
 
 ### Fix
 
 - isolated command line functions so not imported by other packages
 
 ## v1.0.3 (2023-02-14)
```

### Comparing `hspf_reader-1.0.4/CONTRIBUTING.rst` & `hspf_reader-1.0.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/LICENSE.txt` & `hspf_reader-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/PKG-INFO` & `hspf_reader-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspf_reader
-Version: 1.0.4
+Version: 1.0.5
 Summary: Command line script and Python library to read HSPF WDM, binary, and plotgen time series.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/hspf_reader/docs/index.html#hspf_reader-documentation
 Project-URL: github, https://github.com/timcera/hspf_reader
 Project-URL: bitbucket, https://bitbucket.org/timcera/hspf_reader/src/main/
 Keywords: time-series,hspf,simulation,hydrology,hydrologic,python,cli,command line,script,cli-application
```

### Comparing `hspf_reader-1.0.4/README.rst` & `hspf_reader-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/docs/Makefile` & `hspf_reader-1.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/docs/conf.py` & `hspf_reader-1.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/docs/make.bat` & `hspf_reader-1.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/pyproject.toml` & `hspf_reader-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 name = "hspf_reader"
 dynamic = ["version"]
 readme = "README.rst"
 description = "Command line script and Python library to read HSPF WDM, binary, and plotgen time series."
 dependencies = [
     "cltoolbox >= 2.0.0, < 3.0.0",
     "typing-extensions",
-    "toolbox_utils >= 3.0.0, < 4.0.0",
+    "toolbox_utils >= 5.0.0, < 6.0.0",
     "numpy",
     "pandas"
 ]
 authors = [
     {name = "Tim Cera", email = "tim@cerazone.net"}
 ]
 classifiers = [
@@ -99,15 +99,15 @@
     ".ipynb_checkpoints/*"
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "1.0.4"
+version = "1.0.5"
 version_files = ["VERSION"]
 
 [tool.isort]
 profile = "black"
 
 [tool.jupytext]
 formats = "ipynb,py:percent"
```

### Comparing `hspf_reader-1.0.4/setup.py` & `hspf_reader-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/src/hspf_reader/hspf_reader.py` & `hspf_reader-1.0.5/src/hspf_reader/hspf_reader.py`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/src/hspf_reader.egg-info/PKG-INFO` & `hspf_reader-1.0.5/src/hspf_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspf-reader
-Version: 1.0.4
+Version: 1.0.5
 Summary: Command line script and Python library to read HSPF WDM, binary, and plotgen time series.
 Author-email: Tim Cera <tim@cerazone.net>
 License: BSD-3-Clause
 Project-URL: documentation, https://timcera.bitbucket.io/hspf_reader/docs/index.html#hspf_reader-documentation
 Project-URL: github, https://github.com/timcera/hspf_reader
 Project-URL: bitbucket, https://bitbucket.org/timcera/hspf_reader/src/main/
 Keywords: time-series,hspf,simulation,hydrology,hydrologic,python,cli,command line,script,cli-application
```

### Comparing `hspf_reader-1.0.4/src/hspf_reader.egg-info/SOURCES.txt` & `hspf_reader-1.0.5/src/hspf_reader.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 docs/conf.py
 docs/contributing.rst
 docs/function_summary.rst
 docs/index.rst
 docs/license.rst
 docs/make.bat
 docs/readme.rst
-docs/_function_autosummary/hspf_reader.hspf_reader.about.rst
 docs/_function_autosummary/hspf_reader.hspf_reader.hbn.rst
 docs/_function_autosummary/hspf_reader.hspf_reader.plotgen.rst
 docs/_function_autosummary/hspf_reader.hspf_reader.wdm.rst
 src/hspf_reader/__init__.py
 src/hspf_reader/hspf_reader.py
 src/hspf_reader.egg-info/PKG-INFO
 src/hspf_reader.egg-info/SOURCES.txt
```

### Comparing `hspf_reader-1.0.4/tests/data.wdm` & `hspf_reader-1.0.5/tests/data.wdm`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/tests/data_6b_np1.hbn` & `hspf_reader-1.0.5/tests/data_6b_np1.hbn`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/tests/data_plotgen.plt` & `hspf_reader-1.0.5/tests/data_plotgen.plt`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/tests/data_wdm_1.csv` & `hspf_reader-1.0.5/tests/data_wdm_1.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/tests/data_wdm_2.csv` & `hspf_reader-1.0.5/tests/data_wdm_2.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/tests/data_yearly.hbn` & `hspf_reader-1.0.5/tests/data_yearly.hbn`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/tests/sunspot_area.csv` & `hspf_reader-1.0.5/tests/sunspot_area.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/tests/sunspot_area_with_missing.csv` & `hspf_reader-1.0.5/tests/sunspot_area_with_missing.csv`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/tests/test_hbn.py` & `hspf_reader-1.0.5/tests/test_hbn.py`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/tests/test_plotgen.py` & `hspf_reader-1.0.5/tests/test_plotgen.py`

 * *Files identical despite different names*

### Comparing `hspf_reader-1.0.4/tests/test_wdm.py` & `hspf_reader-1.0.5/tests/test_wdm.py`

 * *Files identical despite different names*

