# Comparing `tmp/lightning-habana-1.0.0rc1.tar.gz` & `tmp/lightning-habana-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-habana-1.0.0rc1.tar", last modified: Tue Jun  6 02:42:49 2023, max compression
+gzip compressed data, was "lightning-habana-1.0.1.tar", last modified: Wed Jul 26 13:16:28 2023, max compression
```

## Comparing `lightning-habana-1.0.0rc1.tar` & `lightning-habana-1.0.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.695874 lightning-habana-1.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 02:42:49.695874 lightning-habana-1.0.0rc1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4144 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.687873 lightning-habana-1.0.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.687873 lightning-habana-1.0.0rc1/src/lightning_habana/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/accelerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/plugins/io_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/plugins/precision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/fabric/strategies/single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/accelerator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/dataloaders/resnet_media_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/plugins/io_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/plugins/precision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/profiler/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44163 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-06 02:42:33.000000 lightning-habana-1.0.0rc1/src/lightning_habana/utils/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:42:49.691873 lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-06 02:42:49.000000 lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-06 02:42:49.000000 lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 02:42:49.000000 lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 02:42:49.000000 lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-06 02:42:49.000000 lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-06 02:42:49.000000 lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:28.237843 lightning-habana-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-26 13:16:28.237843 lightning-habana-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:16:28.237843 lightning-habana-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4144 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:28.233843 lightning-habana-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:28.233843 lightning-habana-1.0.1/src/lightning_habana/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:28.233843 lightning-habana-1.0.1/src/lightning_habana/fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/fabric/accelerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:28.233843 lightning-habana-1.0.1/src/lightning_habana/fabric/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/fabric/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/fabric/plugins/io_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/fabric/plugins/precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:28.237843 lightning-habana-1.0.1/src/lightning_habana/fabric/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/fabric/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/fabric/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/fabric/strategies/single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:28.237843 lightning-habana-1.0.1/src/lightning_habana/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/accelerator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:28.237843 lightning-habana-1.0.1/src/lightning_habana/pytorch/datamodule/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/datamodule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:28.237843 lightning-habana-1.0.1/src/lightning_habana/pytorch/datamodule/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/datamodule/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/datamodule/dataloaders/resnet_media_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/datamodule/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/datamodule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:28.237843 lightning-habana-1.0.1/src/lightning_habana/pytorch/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/plugins/io_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/plugins/precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:28.237843 lightning-habana-1.0.1/src/lightning_habana/pytorch/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/profiler/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:28.237843 lightning-habana-1.0.1/src/lightning_habana/pytorch/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44776 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/pytorch/strategies/single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:28.237843 lightning-habana-1.0.1/src/lightning_habana/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-26 13:16:17.000000 lightning-habana-1.0.1/src/lightning_habana/utils/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:16:28.233843 lightning-habana-1.0.1/src/lightning_habana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-26 13:16:28.000000 lightning-habana-1.0.1/src/lightning_habana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-26 13:16:28.000000 lightning-habana-1.0.1/src/lightning_habana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:16:28.000000 lightning-habana-1.0.1/src/lightning_habana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:16:28.000000 lightning-habana-1.0.1/src/lightning_habana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-26 13:16:28.000000 lightning-habana-1.0.1/src/lightning_habana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 13:16:28.000000 lightning-habana-1.0.1/src/lightning_habana.egg-info/top_level.txt
```

### Comparing `lightning-habana-1.0.0rc1/CHANGELOG.md` & `lightning-habana-1.0.1/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,78 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [Unreleased] - YYYY-MM-DD
+## [Unreleased] - 2023-MM-DD
+
+
+### Added
+
+-
+
+### Changed
+
+-
+
+### Fixed
+
+-
+
+### Removed
+
+-
+
+### Deprecated
+
+-
+
+
+## [1.0.1] - 2023-07-26
+
+
+### Added
+
+- Added tests for mixed precision training ([#36](https://github.com/Lightning-AI/lightning-Habana/pull/36))
+- Example to include mixed precision training ([#54](https://github.com/Lightning-AI/lightning-Habana/pull/54))
+
+### Changed
+
+- Enabled skipped tests based on registered strategy, accelerator ([#46](https://github.com/Lightning-AI/lightning-Habana/pull/46))
+
+### Fixed
+
+- Fixed Attribute Error ([#43](https://github.com/Lightning-AI/lightning-Habana/pull/43))
+- Fixed wrong imports ([#44](https://github.com/Lightning-AI/lightning-Habana/pull/44))
+- Fixed graph breaks in test/val phases in lazy mode ([#45](https://github.com/Lightning-AI/lightning-Habana/pull/45))
+
+
+## [1.0.0] - 2023-06-14
 
 ### Added
 
 - Added HPU support for fabric ([#11](https://github.com/Lightning-AI/lightning-Habana/pull/11))
 - Added Pytorch HPU profiler support ([#15](https://github.com/Lightning-AI/lightning-Habana/pull/15))
-
 - Added basic HPU infra support for deep speed ([#21](https://github.com/Lightning-AI/lightning-Habana/pull/21))
-
 - Added Pytorch HPU datamodule support ([#16](https://github.com/Lightning-AI/lightning-Habana/pull/16))
 
 ### Changed
 
 - Changed code hierarchy in compliance with base lightning code for pytorch ([#12](https://github.com/Lightning-AI/lightning-Habana/pull/12))
 - Changed default HPU docker image based on HPU release 1.10.0 ([#30](https://github.com/Lightning-AI/lightning-Habana/pull/30))
 -
 ### Fixed
 
 - Fixed mnist example test ([#20](https://github.com/Lightning-AI/lightning-Habana/pull/20))
 - Habana dataloader hang with Lightning 2.0.x ([#29](https://github.com/Lightning-AI/lightning-Habana/pull/29))
+- Make #29 applicable only for gaudi devices ([#39](https://github.com/Lightning-AI/lightning-Habana/pull/39))
+- Fixed environment initialization for hpus and fixed docs ([#40](https://github.com/Lightning-AI/lightning-Habana/pull/40))
+- Fixed docs and added work around to make use hpu media packages without signature issues ([#41](https://github.com/Lightning-AI/lightning-Habana/pull/41))
 
 ### Removed
 
 - Cleaning up env's ID for HPU parallel plugins based on synapse AI release 1.9 ([#28](https://github.com/Lightning-AI/lightning-Habana/pull/28))
+- Remove unnecessary import checks which degrade performance ([#38](https://github.com/Lightning-AI/lightning-Habana/pull/38))
 
 ### Deprecated
```

### Comparing `lightning-habana-1.0.0rc1/LICENSE` & `lightning-habana-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc1/MANIFEST.in` & `lightning-habana-1.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc1/setup.py` & `lightning-habana-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/__init__.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,38 +7,27 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import operator
 
-from lightning_utilities import compare_version
-
-from lightning_habana.__about__ import *  # noqa: F401, F403
 from lightning_habana.pytorch.accelerator import HPUAccelerator
 from lightning_habana.pytorch.datamodule.datamodule import HPUDataModule
 from lightning_habana.pytorch.plugins.io_plugin import HPUCheckpointIO
 from lightning_habana.pytorch.plugins.precision import HPUPrecisionPlugin
 from lightning_habana.pytorch.profiler.profiler import HPUProfiler
 from lightning_habana.pytorch.strategies.deepspeed import HPUDeepSpeedStrategy
 from lightning_habana.pytorch.strategies.parallel import HPUParallelStrategy
 from lightning_habana.pytorch.strategies.single import SingleHPUStrategy
-from lightning_habana.utils.imports import _HPU_AVAILABLE
-
-if compare_version("lightning", operator.lt, "2.0.0") and compare_version("pytorch_lightning", operator.lt, "2.0.0"):
-    raise ImportError(
-        "You are missing `lightning` or `pytorch-lightning` package or neither of them is in version 2.0+"
-    )
 
 __all__ = [
     "HPUAccelerator",
     "HPUDeepSpeedStrategy",
     "HPUParallelStrategy",
     "SingleHPUStrategy",
     "HPUPrecisionPlugin",
     "HPUCheckpointIO",
-    "HPUDataModule",
     "HPUProfiler",
-    "_HPU_AVAILABLE",
+    "HPUDataModule",
 ]
```

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/fabric/__init__.py` & `lightning-habana-1.0.1/src/lightning_habana/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/fabric/accelerator.py` & `lightning-habana-1.0.1/src/lightning_habana/fabric/accelerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     from lightning.pytorch.utilities.rank_zero import rank_zero_debug
 elif module_available("pytorch_lightning"):
     from pytorch_lightning.accelerators.accelerator import Accelerator
     from pytorch_lightning.utilities.rank_zero import rank_zero_debug
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 
-from lightning_habana.utils.imports import _HPU_AVAILABLE
+from lightning_habana import _HPU_AVAILABLE
 
 if _HPU_AVAILABLE:
     import habana_frameworks.torch.hpu as torch_hpu
 
 
 class HPUAccelerator(Accelerator):
     """Accelerator for HPU devices."""
```

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/fabric/plugins/__init__.py` & `lightning-habana-1.0.1/src/lightning_habana/fabric/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/fabric/plugins/io_plugin.py` & `lightning-habana-1.0.1/src/lightning_habana/fabric/plugins/io_plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/fabric/plugins/precision.py` & `lightning-habana-1.0.1/src/lightning_habana/fabric/plugins/precision.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,18 @@
     from lightning.fabric.plugins.precision.precision import Precision
 elif module_available("pytorch_lightning"):
     from lightning_fabric.plugins.precision.precision import Precision
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 
 
-from lightning_habana.utils.imports import _HPU_AVAILABLE
+from lightning_habana import _HPU_AVAILABLE
+from lightning_habana.utils.imports import _HABANA_FRAMEWORK_AVAILABLE
 
-if _HPU_AVAILABLE:
+if _HABANA_FRAMEWORK_AVAILABLE:
     from habana_frameworks.torch.hpex import hmp
 
 _PRECISION_INPUT_INT = Literal[32]
 _PRECISION_INPUT_STR = Literal["32", "bf16", "32-true", "bf16-mixed"]
 _PRECISION_INPUT = Union[_PRECISION_INPUT_INT, _PRECISION_INPUT_STR]
```

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/fabric/strategies/__init__.py` & `lightning-habana-1.0.1/src/lightning_habana/fabric/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/fabric/strategies/parallel.py` & `lightning-habana-1.0.1/src/lightning_habana/fabric/strategies/parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,20 @@
     from lightning_fabric.utilities.types import Optimizable
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 
 from torch import Tensor
 from torch.nn import Module
 
+from lightning_habana import _HPU_AVAILABLE
 from lightning_habana.fabric.accelerator import HPUAccelerator
 from lightning_habana.fabric.plugins.precision import HPUPrecision
-from lightning_habana.utils.imports import _HPU_AVAILABLE, _TORCH_LESSER_EQUAL_1_13_1
+from lightning_habana.utils.imports import _HABANA_FRAMEWORK_AVAILABLE, _TORCH_LESSER_EQUAL_1_13_1
 
-if _HPU_AVAILABLE:
+if _HABANA_FRAMEWORK_AVAILABLE:
     import habana_frameworks.torch.core as htcore
     import habana_frameworks.torch.distributed.hccl  # noqa: F401
 
 log = logging.getLogger(__name__)
 
 
 class HPUParallelStrategy(DDPStrategy):
```

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/fabric/strategies/single.py` & `lightning-habana-1.0.1/src/lightning_habana/fabric/strategies/single.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,21 @@
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 
 from torch import Tensor
 from torch.nn import Module
 
 from lightning_habana.fabric.plugins.precision import HPUPrecision
-from lightning_habana.utils.imports import _HPU_AVAILABLE, _TORCH_LESSER_EQUAL_1_13_1
+from lightning_habana.utils.imports import _HABANA_FRAMEWORK_AVAILABLE, _TORCH_LESSER_EQUAL_1_13_1
 
-if _HPU_AVAILABLE:
+if _HABANA_FRAMEWORK_AVAILABLE:
     import habana_frameworks.torch.core as htcore
 
+from lightning_habana import _HPU_AVAILABLE
+
 
 class SingleHPUStrategy(SingleDeviceStrategy):
     """Strategy for training on single HPU device."""
 
     strategy_name = "single_hpu"
 
     def __init__(
```

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/__init__.py` & `lightning-habana-1.0.1/src/lightning_habana/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,27 +7,46 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import operator
 
+from lightning_utilities import compare_version
+
+from lightning_habana.__about__ import *  # noqa: F401, F403
 from lightning_habana.pytorch.accelerator import HPUAccelerator
 from lightning_habana.pytorch.datamodule.datamodule import HPUDataModule
 from lightning_habana.pytorch.plugins.io_plugin import HPUCheckpointIO
 from lightning_habana.pytorch.plugins.precision import HPUPrecisionPlugin
 from lightning_habana.pytorch.profiler.profiler import HPUProfiler
 from lightning_habana.pytorch.strategies.deepspeed import HPUDeepSpeedStrategy
 from lightning_habana.pytorch.strategies.parallel import HPUParallelStrategy
 from lightning_habana.pytorch.strategies.single import SingleHPUStrategy
+from lightning_habana.utils.imports import _HABANA_FRAMEWORK_AVAILABLE
+
+if compare_version("lightning", operator.lt, "2.0.0") and compare_version("pytorch_lightning", operator.lt, "2.0.0"):
+    raise ImportError(
+        "You are missing `lightning` or `pytorch-lightning` package or neither of them is in version 2.0+"
+    )
+
+if _HABANA_FRAMEWORK_AVAILABLE:
+    from habana_frameworks.torch.utils.library_loader import is_habana_available
+
+    _HPU_AVAILABLE: bool = is_habana_available()
+else:
+    _HPU_AVAILABLE = False
+
 
 __all__ = [
     "HPUAccelerator",
     "HPUDeepSpeedStrategy",
     "HPUParallelStrategy",
     "SingleHPUStrategy",
     "HPUPrecisionPlugin",
     "HPUCheckpointIO",
-    "HPUProfiler",
     "HPUDataModule",
+    "HPUProfiler",
+    "_HPU_AVAILABLE",
 ]
```

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/accelerator.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/accelerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     from lightning_fabric.utilities.types import _DEVICE
     from pytorch_lightning.accelerators.accelerator import Accelerator
     from pytorch_lightning.utilities.exceptions import MisconfigurationException
     from pytorch_lightning.utilities.rank_zero import rank_zero_debug
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 
-from lightning_habana.utils.imports import _HPU_AVAILABLE
+from lightning_habana.utils.imports import _HABANA_FRAMEWORK_AVAILABLE
 
-if _HPU_AVAILABLE:
+if _HABANA_FRAMEWORK_AVAILABLE:
     import habana_frameworks.torch.hpu as torch_hpu
 
 
 class HPUAccelerator(Accelerator):
     """Accelerator for HPU devices."""
 
     def setup_device(self, device: torch.device) -> None:
```

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/__init__.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/datamodule/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/dataloaders/__init__.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/datamodule/dataloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/dataloaders/resnet_media_pipe.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/datamodule/dataloaders/resnet_media_pipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import time
 from typing import Any, Tuple
 
 import numpy as np
 import torch.utils.data
 
 import lightning_habana.pytorch.datamodule.utils as utils
-from lightning_habana.utils.imports import _HPU_AVAILABLE
+from lightning_habana.utils.imports import _HABANA_FRAMEWORK_AVAILABLE
 
 TRAIN_RESIZE_DIM = 224
 EVAL_RESIZE_DIM = 256
 CROP_DIM = 224
 
 DECODER_SCALE_MIN = 0.08
 DECODER_SCALE_MAX = 1.0
@@ -36,15 +36,15 @@
 RGB_MEAN_VALUES = [0.485, 0.456, 0.406]
 RGB_STD_VALUES = [0.229, 0.224, 0.225]
 RGB_MULTIPLIER = 255
 
 EVAL_CROP_X = 0.5
 EVAL_CROP_Y = 0.5
 
-if _HPU_AVAILABLE:
+if _HABANA_FRAMEWORK_AVAILABLE:
     try:
         from habana_frameworks.mediapipe import fn
         from habana_frameworks.mediapipe.media_types import decoderStage, dtype, ftype, imgtype, randomCropType
         from habana_frameworks.mediapipe.mediapipe import MediaPipe
         from habana_frameworks.mediapipe.operators.cpu_nodes.cpu_nodes import media_function
         from habana_frameworks.mediapipe.plugins.iterator_pytorch import HPUResnetPytorchIterator
     except ImportError:
@@ -182,26 +182,25 @@
         Args:
             random_flip_func specific params.
             shape: output shape
             dtype: output data type
             seed: seed to be used
         """
 
-        def __init__(self, params: Any) -> None:
+        def __init__(self, params):  # type: ignore[no-untyped-def]
             self.np_shape = params["shape"][::-1]
             self.np_dtype = params["dtype"]
             self.seed = params["seed"]
             self.rng = np.random.default_rng(self.seed)
 
-        def __call__(self) -> Any:
+        def __call__(self):  # type: ignore[no-untyped-def]
             """:returns : randomly generated binary output per image."""
             probabilities = [1.0 - FLIP_PROBABILITY, FLIP_PROBABILITY]
             random_flips = self.rng.choice([0, 1], p=probabilities, size=self.np_shape)
-            random_flips = np.array(random_flips, dtype=self.np_dtype)
-            return random_flips
+            return np.array(random_flips, dtype=self.np_dtype)
 
     class MediaApiDataLoader(torch.utils.data.DataLoader):
         """Helper to construct resnet media pipe dataloader."""
 
         def __init__(
             self,
             dataset: Any,
```

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/datamodule.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/datamodule/datamodule.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,33 @@
 
 import warnings
 from typing import Any, Optional
 
 from lightning_utilities import module_available
 
 if module_available("lightning"):
-    import lightning.pytorch as pl
+    from lightning.pytorch import LightningDataModule
     from lightning.pytorch.utilities.imports import _TORCHVISION_AVAILABLE
 elif module_available("pytorch_lightning"):
-    import pytorch_lightning as pl
+    from pytorch_lightning import LightningDataModule
     from pytorch_lightning.utilities.imports import _TORCHVISION_AVAILABLE
 
 import torch
 
-from lightning_habana.utils.imports import _HPU_AVAILABLE, _LIGHTNING_GREATER_EQUAL_2_0_0, _TORCH_GREATER_EQUAL_2_0_0
+from lightning_habana.utils.imports import (
+    _HABANA_FRAMEWORK_AVAILABLE,
+    _LIGHTNING_GREATER_EQUAL_2_0_0,
+    _TORCH_GREATER_EQUAL_2_0_0,
+)
 
 if _TORCHVISION_AVAILABLE:
     import torchvision.datasets
     from torchvision import transforms as transform_lib
 
-if _HPU_AVAILABLE:
+if _HABANA_FRAMEWORK_AVAILABLE:
     try:
         import habana_dataloader
     except ImportError:
         raise ModuleNotFoundError("habana_dataloader package is not installed.")
 
     from lightning_habana.pytorch.datamodule.dataloaders.resnet_media_pipe import MediaApiDataLoader
 
@@ -97,15 +101,15 @@
     dataset_train = torchvision.datasets.ImageFolder(traindir, train_transforms)
 
     dataset_val = torchvision.datasets.ImageFolder(valdir, val_transforms)
 
     return dataset_train, dataset_val
 
 
-class HPUDataModule(pl.LightningDataModule):
+class HPUDataModule(LightningDataModule):
     """Datamodule helper class to load the right media pipe."""
 
     name = "hpu-dataset"
 
     def __init__(
         self,
         train_dir: str = _DATASETS_PATH,
@@ -135,15 +139,15 @@
         self.val_transform = val_transforms
         self.pin_memory = pin_memory
         self.shuffle = shuffle
         self.drop_last = drop_last
         self.distributed = distributed
         self.data_loader_type = torch.utils.data.DataLoader
 
-        if _HPU_AVAILABLE:
+        if _HABANA_FRAMEWORK_AVAILABLE:
             if lightning_habana.pytorch.datamodule.utils.is_gaudi2():
                 self.data_loader_type = MediaApiDataLoader  # type: ignore
             else:
                 self.data_loader_type = habana_dataloader.HabanaDataLoader
 
     def setup(self, stage: Optional[str] = None):  # type: ignore[no-untyped-def]
         """Method to sanitize the input params."""
@@ -177,15 +181,15 @@
     def train_dataloader(self):  # type: ignore[no-untyped-def]
         """Train set removes a subset to use for validation."""
         sampler_train = (
             torch.utils.data.distributed.DistributedSampler(self.dataset_train)
             if self.distributed
             else torch.utils.data.RandomSampler(self.dataset_train)
         )
-        if self.drop_last:
+        if self.drop_last and lightning_habana.pytorch.datamodule.utils.is_gaudi():
             self.data_loader_type.__len__ = patch_aeon_length
         return self.data_loader_type(
             dataset=self.dataset_train,
             batch_size=self.batch_size,
             shuffle=self.shuffle,
             num_workers=self.num_workers,
             pin_memory=self.pin_memory,
@@ -196,15 +200,15 @@
     def val_dataloader(self):  # type: ignore[no-untyped-def]
         """Val set uses a subset of the training set for validation."""
         sampler_eval = (
             torch.utils.data.distributed.DistributedSampler(self.dataset_val)
             if self.distributed
             else torch.utils.data.SequentialSampler(self.dataset_val)
         )
-        if self.drop_last:
+        if self.drop_last and lightning_habana.pytorch.datamodule.utils.is_gaudi():
             self.data_loader_type.__len__ = patch_aeon_length
         return self.data_loader_type(
             dataset=self.dataset_val,
             batch_size=self.batch_size,
             shuffle=self.shuffle,
             num_workers=self.num_workers,
             pin_memory=self.pin_memory,
@@ -215,15 +219,15 @@
     def test_dataloader(self):  # type: ignore[no-untyped-def]
         """Test set uses the test split."""
         sampler_eval = (
             torch.utils.data.distributed.DistributedSampler(self.dataset_val)
             if self.distributed
             else torch.utils.data.SequentialSampler(self.dataset_val)
         )
-        if self.drop_last:
+        if self.drop_last and lightning_habana.pytorch.datamodule.utils.is_gaudi():
             self.data_loader_type.__len__ = patch_aeon_length
         return self.data_loader_type(
             dataset=self.dataset_val,
             batch_size=self.batch_size,
             shuffle=self.shuffle,
             num_workers=self.num_workers,
             pin_memory=self.pin_memory,
```

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/datamodule/utils.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/datamodule/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from lightning_habana.utils.imports import _HPU_AVAILABLE
+from lightning_habana.utils.imports import _HABANA_FRAMEWORK_AVAILABLE
 
-if _HPU_AVAILABLE:
+if _HABANA_FRAMEWORK_AVAILABLE:
     import habana_frameworks.torch.hpu as torch_hpu
 
 import torch.distributed as dist
 
 
 def is_dist_avail_and_initialized() -> bool:
     """Check distributed backend is initialized or not."""
```

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/plugins/__init__.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/plugins/io_plugin.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/plugins/io_plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/plugins/precision.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/plugins/precision.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 if module_available("lightning"):
     from lightning.pytorch.plugins.precision.precision_plugin import PrecisionPlugin
 elif module_available("pytorch_lightning"):
     from pytorch_lightning.plugins.precision.precision_plugin import PrecisionPlugin
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 
-from lightning_habana.utils.imports import _HPU_AVAILABLE
+from lightning_habana.utils.imports import _HABANA_FRAMEWORK_AVAILABLE
 
-if _HPU_AVAILABLE:
+if _HABANA_FRAMEWORK_AVAILABLE:
     from habana_frameworks.torch.hpex import hmp
 
 _PRECISION_INPUT = Literal["32", "32-true", "bf16", "bf16-mixed"]
 
 
 class HPUPrecisionPlugin(PrecisionPlugin):
     """Plugin that enables bfloat/half support on HPUs.
```

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/profiler/__init__.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/profiler/profiler.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/__init__.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/deepspeed.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/strategies/deepspeed.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,60 +27,66 @@
 from lightning_utilities.core.apply_func import apply_to_collection
 from lightning_utilities.core.imports import RequirementCache
 from torch import Tensor
 from torch.nn import Module
 from torch.optim import Optimizer
 
 if module_available("lightning"):
-    import lightning.pytorch as pl
     from lightning.fabric.plugins import ClusterEnvironment
+    from lightning.fabric.strategies import _StrategyRegistry
     from lightning.fabric.utilities.optimizer import _optimizers_to_device
     from lightning.fabric.utilities.seed import reset_seed
     from lightning.fabric.utilities.types import _PATH, LRScheduler, ReduceLROnPlateau
+    from lightning.pytorch import LightningModule, Trainer
+    from lightning.pytorch.accelerators import Accelerator
     from lightning.pytorch.core.optimizer import _init_optimizers_and_lr_schedulers
     from lightning.pytorch.overrides.base import _LightningModuleWrapperBase, _LightningPrecisionModuleWrapperBase
     from lightning.pytorch.plugins.precision import PrecisionPlugin
     from lightning.pytorch.strategies.utils import _fp_to_half
     from lightning.pytorch.trainer.states import TrainerFn
     from lightning.pytorch.utilities import GradClipAlgorithmType
     from lightning.pytorch.utilities.exceptions import MisconfigurationException
     from lightning.pytorch.utilities.model_helpers import is_overridden
     from lightning.pytorch.utilities.rank_zero import WarningCache, rank_zero_info, rank_zero_only, rank_zero_warn
     from lightning.pytorch.utilities.types import STEP_OUTPUT, LRSchedulerConfig
 elif module_available("pytorch_lightning"):
-    import pytorch_lightning as pl
     from lightning_fabric.plugins import ClusterEnvironment
+    from lightning_fabric.strategies import _StrategyRegistry
     from lightning_fabric.utilities.optimizer import _optimizers_to_device
     from lightning_fabric.utilities.seed import reset_seed
     from lightning_fabric.utilities.types import _PATH, LRScheduler, ReduceLROnPlateau
     from pytorch_lightning.core.optimizer import _init_optimizers_and_lr_schedulers
+    from pytorch_lightning.accelerators import Accelerator
+    from pytorch_lightning import LightningModule, Trainer
     from pytorch_lightning.overrides.base import _LightningModuleWrapperBase, _LightningPrecisionModuleWrapperBase
     from pytorch_lightning.plugins.precision import PrecisionPlugin
     from pytorch_lightning.strategies.utils import _fp_to_half
     from pytorch_lightning.trainer.states import TrainerFn
     from pytorch_lightning.utilities import GradClipAlgorithmType
     from pytorch_lightning.utilities.exceptions import MisconfigurationException
     from pytorch_lightning.utilities.model_helpers import is_overridden
     from pytorch_lightning.utilities.rank_zero import WarningCache, rank_zero_info, rank_zero_only, rank_zero_warn
     from pytorch_lightning.utilities.types import STEP_OUTPUT, LRSchedulerConfig
 
 from lightning_habana.pytorch.accelerator import HPUAccelerator
 from lightning_habana.pytorch.strategies.parallel import HPUParallelStrategy
-from lightning_habana.utils.imports import _HPU_AVAILABLE
+from lightning_habana.utils.imports import _HABANA_FRAMEWORK_AVAILABLE
 
-if _HPU_AVAILABLE:
+if _HABANA_FRAMEWORK_AVAILABLE:
     import habana_frameworks.torch.core as htcore  # noqa: F401
     import habana_frameworks.torch.distributed.hccl  # noqa: F401
 
 log = logging.getLogger(__name__)
 warning_cache = WarningCache()
 
+# WA : TBD : there is an issue with internal habana pipelines wrt deepspeed package naming in 1.10.0 release
 _HPU_DEEPSPEED_AVAILABLE = (
     # HPU deep speed is supported only through this pip install git+https://github.com/HabanaAI/DeepSpeed.git@1.10.0
     RequirementCache("deepspeed==0.7.7+hpu.synapse.v1.10.0")
+    or RequirementCache("deepspeed==0.7.7+ca649af")
 )
 if TYPE_CHECKING and _HPU_DEEPSPEED_AVAILABLE:
     import deepspeed
 
 
 def remove_module_hooks(model: torch.nn.Module) -> None:
     """Helper to remove all module hooks."""
@@ -188,15 +194,15 @@
     """
 
     strategy_name = "hpu_deepspeed"
     DEEPSPEED_ENV_VAR = "PL_DEEPSPEED_CONFIG_PATH"
 
     def __init__(
         self,
-        accelerator: Optional["pl.accelerators.Accelerator"] = None,
+        accelerator: Optional[Accelerator] = None,
         zero_optimization: bool = True,
         stage: int = 2,
         remote_device: str = "cpu",
         offload_optimizer: bool = False,
         offload_parameters: bool = False,
         offload_params_device: str = "cpu",
         nvme_path: str = "/local_nvme",
@@ -325,15 +331,15 @@
         self.set_world_ranks()
         rank_zero_only.rank = self.global_rank
         self._init_deepspeed_distributed()
         if not self._config_initialized:
             self._format_config()
             self._config_initialized = True
 
-    def setup(self, trainer: "pl.Trainer") -> None:
+    def setup(self, trainer: Trainer) -> None:
         assert self.accelerator is not None
         self.accelerator.setup(trainer)
         # habana deepspeed needs model to be moved to device before initialization
         self.model.to(self.root_device)
         # we set the device so that optimizers can be created with distributed comms.
         assert self.lightning_module is not None
         self.lightning_module._device = self.root_device
@@ -419,15 +425,15 @@
             dist_init_required=False,
         )
         return deepspeed_engine, deepspeed_optimizer
 
     def init_deepspeed(self) -> None:
         assert self.lightning_module is not None
         # deepspeed handles gradient clipping internally
-        if is_overridden("configure_gradient_clipping", self.lightning_module, pl.LightningModule):
+        if is_overridden("configure_gradient_clipping", self.lightning_module, LightningModule):
             rank_zero_warn(
                 "Since DeepSpeed handles gradient clipping internally, the default"
                 " `LightningModule.configure_gradient_clipping` implementation will not actually clip gradients."
                 " The hook will still be called. Consider setting"
                 " `Trainer(gradient_clip_val=..., gradient_clip_algorithm='norm')`"
                 " which will use the internal mechanism."
             )
@@ -436,15 +442,15 @@
             raise MisconfigurationException("DeepSpeed does not support clipping gradients by value.")
 
         if not isinstance(self.accelerator, HPUAccelerator):
             raise MisconfigurationException(
                 f"DeepSpeed strategy is only supported on HPU but `{self.accelerator.__class__.__name__}` is used."
             )
 
-        assert isinstance(self.model, (pl.LightningModule, _LightningPrecisionModuleWrapperBase))
+        assert isinstance(self.model, (LightningModule, _LightningPrecisionModuleWrapperBase))
         model = _LightningModuleWrapperBase(forward_module=self.model)
 
         if self.lightning_module.trainer and self.lightning_module.trainer.training:
             self._initialize_deepspeed_train(model)
         else:
             self._initialize_deepspeed_inference(model)
 
@@ -530,23 +536,26 @@
                 mpu_=None,
                 partition_activations=checkpoint_config.get("partition_activations"),
                 contiguous_checkpointing=checkpoint_config.get("contiguous_memory_optimization"),
                 checkpoint_in_cpu=checkpoint_config.get("cpu_checkpointing"),
                 profile=checkpoint_config.get("profile"),
             )
 
+    # TBD - this is still experimental and not complete
     def _initialize_deepspeed_inference(self, model: Module) -> None:
         import deepspeed
 
         assert isinstance(self.config, dict)
 
         # todo: this is required for DeepSpeed throughput timers
         inference_config = {"train_micro_batch_size_per_gpu": 1}
         if "fp16" in self.config:
             inference_config.update({"fp16": self.config["fp16"]})
+        if "bf16" in self.config:
+            inference_config.update({"bf16": self.config["bf16"]})
         if self.zero_stage_3:
             inference_config.update(
                 {
                     "zero_allow_untested_optimizer": self.config["zero_allow_untested_optimizer"],
                     "zero_optimization": self.config["zero_optimization"],
                 }
             )
@@ -565,15 +574,15 @@
         model = model.to("hpu")
         self.model = model
 
     @property
     def distributed_sampler_kwargs(self) -> Dict[str, int]:
         return {"num_replicas": self.world_size, "rank": self.global_rank}
 
-    def setup_optimizers(self, trainer: "pl.Trainer") -> None:
+    def setup_optimizers(self, trainer: Trainer) -> None:
         """Creates optimizers and schedulers.
 
         Args:
             trainer: the Trainer, these optimizers should be connected to.
         """
         if trainer.state.fn != TrainerFn.FITTING:
             return
@@ -857,15 +866,15 @@
         load(self.lightning_module, prefix="")
 
     def load_optimizer_state_dict(self, checkpoint: Mapping[str, Any]) -> None:
         # override to do nothing, deepspeed engine already loaded the states in `load_checkpoint()`
         pass
 
     @classmethod
-    def register_strategies(cls, strategy_registry: Dict) -> None:
+    def register_strategies(cls, strategy_registry: _StrategyRegistry) -> None:
         strategy_registry.register("hpu_deepspeed", cls, description="Default DeepSpeed Strategy")
         strategy_registry.register(
             "hpu_deepspeed_stage_1", cls, description="DeepSpeed with ZeRO Stage 1 enabled", stage=1
         )
         strategy_registry.register(
             "hpu_deepspeed_stage_2", cls, description="DeepSpeed with ZeRO Stage 2 enabled", stage=2
         )
```

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/parallel.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/strategies/parallel.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,47 +11,45 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import logging
 import os
 from typing import Any, Callable, Dict, List, Optional, Union
 
+import torch
 import torch.distributed
 from lightning_utilities import module_available
 
 if module_available("lightning"):
     from lightning.fabric.plugins import CheckpointIO, ClusterEnvironment
-    from lightning.fabric.utilities.distributed import _distributed_available
     from lightning.fabric.utilities.distributed import group as _group
     from lightning.pytorch import LightningModule
     from lightning.pytorch.accelerators import Accelerator
-    from lightning.pytorch.plugins.io.hpu_plugin import HPUCheckpointIO
     from lightning.pytorch.plugins.io.wrapper import _WrappingCheckpointIO
     from lightning.pytorch.plugins.precision import PrecisionPlugin
     from lightning.pytorch.strategies.ddp import DDPStrategy
 elif module_available("pytorch_lightning"):
     from lightning_fabric.plugins import CheckpointIO, ClusterEnvironment
-    from lightning_fabric.utilities.distributed import _distributed_available
     from lightning_fabric.utilities.distributed import group as _group
     from pytorch_lightning import LightningModule
     from pytorch_lightning.accelerators import Accelerator
-    from pytorch_lightning.plugins.io.hpu_plugin import HPUCheckpointIO
     from pytorch_lightning.plugins.io.wrapper import _WrappingCheckpointIO
     from pytorch_lightning.plugins.precision import PrecisionPlugin
     from pytorch_lightning.strategies.ddp import DDPStrategy
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 from torch.nn import Module
 from torch.optim.optimizer import Optimizer
 
-from lightning_habana.utils.imports import _HPU_AVAILABLE
+from lightning_habana.pytorch.plugins.io_plugin import HPUCheckpointIO
+from lightning_habana.utils.imports import _HABANA_FRAMEWORK_AVAILABLE
 
-if _HPU_AVAILABLE:
+if _HABANA_FRAMEWORK_AVAILABLE:
     import habana_frameworks.torch.core as htcore
-    import habana_frameworks.torch.distributed.hccl  # noqa: F401
+    import habana_frameworks.torch.distributed.hccl as hpu_dist
 
 log = logging.getLogger(__name__)
 
 
 class HPUParallelStrategy(DDPStrategy):
     """Strategy for distributed training on multiple HPU devices."""
 
@@ -92,27 +90,31 @@
         elif isinstance(self._checkpoint_io, _WrappingCheckpointIO):
             self._checkpoint_io.checkpoint_io = HPUCheckpointIO()
 
         return self._checkpoint_io
 
     @checkpoint_io.setter
     def checkpoint_io(self, io: Optional[CheckpointIO]) -> None:
-        self._checkpoint_io = io
+        self._checkpoint_io = io  # type: ignore
 
     def setup_environment(self) -> None:
         if self._process_group_backend == "hccl":
             # this env is used in overrides to check the backend initiated
             os.environ["HCCL_DISTRIBUTED_BACKEND"] = str(1)
+            _ws = self.cluster_environment.world_size()
+            _grank = self.cluster_environment.global_rank()
+            _lrank = self.cluster_environment.local_rank()
+            hpu_dist.initialize_distributed_hpu(world_size=_ws, rank=_grank, local_rank=_lrank)
         super().setup_environment()
 
     def determine_ddp_device_ids(self) -> None:
         return None
 
     def broadcast(self, obj: object, src: int = 0) -> object:
-        if not _distributed_available():
+        if not torch.distributed.is_available():
             return obj
 
         obj = [obj]
         if self.global_rank != src:
             obj = [None]
 
         _hpu_broadcast_object_list(obj, src, group=_group.WORLD)
@@ -130,14 +132,29 @@
         **kwargs: Any,
     ) -> Any:
         optimizer_output = super().optimizer_step(optimizer, closure, model, **kwargs)
         # Break lazy accumulation of graph after optimizer
         htcore.mark_step()
         return optimizer_output
 
+    def validation_step(self, batch: Any, batch_idx: int) -> Any:
+        # Break lazy accumulation of graph after every step
+        htcore.mark_step()
+        return super().validation_step(batch, batch_idx)
+
+    def test_step(self, batch: Any, batch_idx: int) -> Any:
+        # Break lazy accumulation of graph after every step
+        htcore.mark_step()
+        return super().test_step(batch, batch_idx)
+
+    def predict_step(self, batch: Any, batch_idx: int) -> Any:
+        # Break lazy accumulation of graph after every step
+        htcore.mark_step()
+        return super().predict_step(batch, batch_idx)
+
     @classmethod
     def register_strategies(cls, strategy_registry: Dict) -> None:
         strategy_registry.register(
             cls.strategy_name,
             cls,
             description=f"{cls.__class__.__name__}",
         )
```

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/pytorch/strategies/single.py` & `lightning-habana-1.0.1/src/lightning_habana/pytorch/strategies/single.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,36 +17,35 @@
 from lightning_utilities import module_available
 
 if module_available("lightning"):
     from lightning.fabric.plugins import CheckpointIO
     from lightning.fabric.utilities.types import _DEVICE
     from lightning.pytorch import LightningModule, Trainer
     from lightning.pytorch.accelerators import Accelerator
-    from lightning.pytorch.plugins.io.hpu_plugin import HPUCheckpointIO
     from lightning.pytorch.plugins.io.wrapper import _WrappingCheckpointIO
     from lightning.pytorch.plugins.precision import PrecisionPlugin
     from lightning.pytorch.strategies.single_device import SingleDeviceStrategy
 elif module_available("pytorch_lightning"):
     from lightning_fabric.plugins import CheckpointIO
     from lightning_fabric.utilities.types import _DEVICE
     from pytorch_lightning import LightningModule, Trainer
     from pytorch_lightning.accelerators import Accelerator
-    from pytorch_lightning.plugins.io.hpu_plugin import HPUCheckpointIO
     from pytorch_lightning.plugins.io.wrapper import _WrappingCheckpointIO
     from pytorch_lightning.plugins.precision import PrecisionPlugin
     from pytorch_lightning.strategies.single_device import SingleDeviceStrategy
 else:
     raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 
 from torch.nn import Module
 from torch.optim.optimizer import Optimizer
 
-from lightning_habana.utils.imports import _HPU_AVAILABLE
+from lightning_habana.pytorch.plugins.io_plugin import HPUCheckpointIO
+from lightning_habana.utils.imports import _HABANA_FRAMEWORK_AVAILABLE
 
-if _HPU_AVAILABLE:
+if _HABANA_FRAMEWORK_AVAILABLE:
     import habana_frameworks.torch.core as htcore
 
 
 class SingleHPUStrategy(SingleDeviceStrategy):
     """Strategy for training on single HPU device."""
 
     strategy_name = "hpu_single"
@@ -72,15 +71,15 @@
         elif isinstance(self._checkpoint_io, _WrappingCheckpointIO):
             self._checkpoint_io.checkpoint_io = HPUCheckpointIO()
 
         return self._checkpoint_io
 
     @checkpoint_io.setter
     def checkpoint_io(self, io: Optional[CheckpointIO]) -> None:
-        self._checkpoint_io = io
+        self._checkpoint_io = io  # type: ignore
 
     @property
     def is_distributed(self) -> bool:
         return False
 
     def setup(self, trainer: Trainer) -> None:
         self.model_to_device()
@@ -104,14 +103,29 @@
         **kwargs: Any,
     ) -> Any:
         optimizer_output = super().optimizer_step(optimizer, closure, model, **kwargs)
         # Break lazy accumulation of graph after optimizer
         htcore.mark_step()
         return optimizer_output
 
+    def validation_step(self, batch: Any, batch_idx: int) -> Any:
+        # Break lazy accumulation of graph after every step
+        htcore.mark_step()
+        return super().validation_step(batch, batch_idx)
+
+    def test_step(self, batch: Any, batch_idx: int) -> Any:
+        # Break lazy accumulation of graph after every step
+        htcore.mark_step()
+        return super().test_step(batch, batch_idx)
+
+    def predict_step(self, batch: Any, batch_idx: int) -> Any:
+        # Break lazy accumulation of graph after every step
+        htcore.mark_step()
+        return super().predict_step(batch, batch_idx)
+
     @classmethod
     def register_strategies(cls, strategy_registry: Dict) -> None:
         strategy_registry.register(
             cls.strategy_name,
             cls,
             description=f"{cls.__class__.__name__}",
         )
```

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana/utils/imports.py` & `lightning-habana-1.0.1/src/lightning_habana/utils/imports.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,19 +17,13 @@
 
 _PACKAGE_ROOT = os.path.dirname(__file__)
 _PROJECT_ROOT = os.path.dirname(_PACKAGE_ROOT)
 
 from lightning_utilities.core.imports import compare_version, package_available  # noqa: E402
 
 _HABANA_FRAMEWORK_AVAILABLE = package_available("habana_frameworks")
-if _HABANA_FRAMEWORK_AVAILABLE:
-    from habana_frameworks.torch.utils.library_loader import is_habana_available
-
-    _HPU_AVAILABLE: bool = is_habana_available()
-else:
-    _HPU_AVAILABLE = False
 
 _TORCH_LESSER_EQUAL_1_13_1 = compare_version("torch", operator.le, "1.13.1")
 _TORCH_GREATER_EQUAL_2_0_0 = compare_version("torch", operator.ge, "2.0.0")
 _LIGHTNING_GREATER_EQUAL_2_0_0 = compare_version("lightning", operator.ge, "2.0.0") or compare_version(
     "pytorch_lightning", operator.ge, "2.0.0"
 )
```

### Comparing `lightning-habana-1.0.0rc1/src/lightning_habana.egg-info/SOURCES.txt` & `lightning-habana-1.0.1/src/lightning_habana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

