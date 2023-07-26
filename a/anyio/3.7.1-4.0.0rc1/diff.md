# Comparing `tmp/anyio-3.7.1.tar.gz` & `tmp/anyio-4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyio-3.7.1.tar", last modified: Wed Jul  5 16:44:41 2023, max compression
+gzip compressed data, was "anyio-4.0.0rc1.tar", last modified: Wed Jul 26 20:46:45 2023, max compression
```

## Comparing `anyio-3.7.1.tar` & `anyio-4.0.0rc1.tar`

### file list

```diff
@@ -1,110 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.469102 anyio-3.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.445102 anyio-3.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.445102 anyio-3.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-05 16:44:27.000000 anyio-3.7.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-05 16:44:27.000000 anyio-3.7.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-05 16:44:27.000000 anyio-3.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-05 16:44:27.000000 anyio-3.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-05 16:44:27.000000 anyio-3.7.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-05 16:44:27.000000 anyio-3.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-05 16:44:41.469102 anyio-3.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-05 16:44:27.000000 anyio-3.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.449102 anyio-3.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/cancellation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/fileio.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/networking.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/signals.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/streams.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/subprocesses.rst
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/support.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/synchronization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/tasks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/threads.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/typedattrs.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34390 2023-07-05 16:44:27.000000 anyio-3.7.1/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-05 16:44:27.000000 anyio-3.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 16:44:41.469102 anyio-3.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.445102 anyio-3.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.453102 anyio-3.7.1/src/anyio/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.453102 anyio-3.7.1/src/anyio/_backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67056 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_backends/_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    30035 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_backends/_trio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.457102 anyio-3.7.1/src/anyio/_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18026 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20667 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (123)    16747 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/_core/_typedattr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.461102 anyio-3.7.1/src/anyio/abc/
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/abc/_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/abc/_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/abc/_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/abc/_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/abc/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/abc/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/from_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/lowlevel.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/pytest_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.461102 anyio-3.7.1/src/anyio/streams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/streams/buffered.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/streams/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/streams/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/streams/stapled.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/streams/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/streams/tls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/to_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-05 16:44:27.000000 anyio-3.7.1/src/anyio/to_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.453102 anyio-3.7.1/src/anyio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-05 16:44:41.000000 anyio-3.7.1/src/anyio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-05 16:44:41.000000 anyio-3.7.1/src/anyio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 16:44:41.000000 anyio-3.7.1/src/anyio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 16:44:41.000000 anyio-3.7.1/src/anyio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-05 16:44:41.000000 anyio-3.7.1/src/anyio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 16:44:41.000000 anyio-3.7.1/src/anyio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.465102 anyio-3.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:41.469102 anyio-3.7.1/tests/streams/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/streams/test_buffered.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/streams/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/streams/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/streams/test_stapled.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/streams/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    18830 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/streams/test_tls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_debugging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_from_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_lowlevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    52196 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_subprocesses.py
--rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (123)    34173 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_taskgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_to_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-07-05 16:44:27.000000 anyio-3.7.1/tests/test_to_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:45.928543 anyio-4.0.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:45.916543 anyio-4.0.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:45.916543 anyio-4.0.0rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/.github/ISSUE_TEMPLATE/features_request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:45.920543 anyio-4.0.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/.github/workflows/test-downstream.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-26 20:46:45.928543 anyio-4.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:45.920543 anyio-4.0.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/cancellation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/fileio.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/networking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/subprocesses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/support.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/synchronization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/threads.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/typedattrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    38529 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/docs/versionhistory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 20:46:45.928543 anyio-4.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:45.916543 anyio-4.0.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:45.920543 anyio-4.0.0rc1/src/anyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:45.920543 anyio-4.0.0rc1/src/anyio/_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79073 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_backends/_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34633 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_backends/_trio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:45.924543 anyio-4.0.0rc1/src/anyio/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_core/_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_core/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_core/_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_core/_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_core/_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_core/_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_core/_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_core/_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_core/_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_core/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_core/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/_core/_typedattr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:45.924543 anyio-4.0.0rc1/src/anyio/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/abc/_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/abc/_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/abc/_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/abc/_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/abc/_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/abc/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/abc/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14188 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/from_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/lowlevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/pytest_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:45.924543 anyio-4.0.0rc1/src/anyio/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/streams/buffered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/streams/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9416 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/streams/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/streams/stapled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/streams/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/streams/tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/to_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/src/anyio/to_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:45.920543 anyio-4.0.0rc1/src/anyio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-26 20:46:45.000000 anyio-4.0.0rc1/src/anyio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-26 20:46:45.000000 anyio-4.0.0rc1/src/anyio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:46:45.000000 anyio-4.0.0rc1/src/anyio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-26 20:46:45.000000 anyio-4.0.0rc1/src/anyio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-26 20:46:45.000000 anyio-4.0.0rc1/src/anyio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 20:46:45.000000 anyio-4.0.0rc1/src/anyio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:45.928543 anyio-4.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:45.928543 anyio-4.0.0rc1/tests/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/streams/test_buffered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/streams/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/streams/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/streams/test_stapled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/streams/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/streams/test_tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/test_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/test_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19386 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/test_fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21079 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/test_from_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/test_lowlevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/test_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62963 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/test_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/test_subprocesses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18010 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/test_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37985 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/test_taskgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/test_to_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-07-26 20:46:36.000000 anyio-4.0.0rc1/tests/test_to_thread.py
```

### Comparing `anyio-3.7.1/.github/workflows/publish.yml` & `anyio-4.0.0rc1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `anyio-3.7.1/.github/workflows/test.yml` & `anyio-4.0.0rc1/.github/workflows/test.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 name: test suite
 
 on:
   push:
-    branches: [master, 3.x]
+    branches: [master]
   pull_request:
 
 jobs:
   pyright:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
@@ -24,22 +24,22 @@
       run: pyright --verifytypes anyio
 
   test:
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", pypy-3.9]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12", pypy-3.10]
         include:
         - os: macos-latest
-          python-version: "3.7"
+          python-version: "3.8"
         - os: macos-latest
           python-version: "3.11"
         - os: windows-latest
-          python-version: "3.7"
+          python-version: "3.8"
         - os: windows-latest
           python-version: "3.11"
     runs-on: ${{ matrix.os }}
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
```

### Comparing `anyio-3.7.1/.pre-commit-config.yaml` & `anyio-4.0.0rc1/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -11,22 +11,22 @@
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [ "--fix=lf" ]
       - id: trailing-whitespace
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.277
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.0.280
     hooks:
       - id: ruff
         args: [--fix, --show-fixes]
 
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.4.1
     hooks:
       - id: mypy
```

### Comparing `anyio-3.7.1/LICENSE` & `anyio-4.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `anyio-3.7.1/PKG-INFO` & `anyio-4.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: anyio
-Version: 3.7.1
+Version: 4.0.0rc1
 Summary: High level compatibility layer for multiple asynchronous event loop implementations
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://anyio.readthedocs.io/en/latest/
 Project-URL: Changelog, https://anyio.readthedocs.io/en/stable/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/anyio
 Project-URL: Issue tracker, https://github.com/agronholm/anyio/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: AnyIO
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: trio
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 .. image:: https://github.com/agronholm/anyio/actions/workflows/test.yml/badge.svg
```

### Comparing `anyio-3.7.1/README.rst` & `anyio-4.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.1/docs/api.rst` & `anyio-4.0.0rc1/docs/api.rst`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 .. autoclass:: anyio.TypedAttributeSet
 .. autoclass:: anyio.TypedAttributeProvider
 
 Timeouts and cancellation
 -------------------------
 
-.. autofunction:: anyio.open_cancel_scope
 .. autofunction:: anyio.move_on_after
 .. autofunction:: anyio.fail_after
 .. autofunction:: anyio.current_effective_deadline
 
 .. autoclass:: anyio.CancelScope
 
 Task groups
@@ -58,15 +57,14 @@
 .. autofunction:: anyio.to_process.current_default_process_limiter
 
 Running asynchronous code from other threads
 --------------------------------------------
 
 .. autofunction:: anyio.from_thread.run
 .. autofunction:: anyio.from_thread.run_sync
-.. autofunction:: anyio.from_thread.create_blocking_portal
 .. autofunction:: anyio.from_thread.start_blocking_portal
 
 .. autoclass:: anyio.from_thread.BlockingPortal
 
 Async file I/O
 --------------
 
@@ -156,40 +154,28 @@
 
 .. autoclass:: anyio.LockStatistics
 .. autoclass:: anyio.EventStatistics
 .. autoclass:: anyio.ConditionStatistics
 .. autoclass:: anyio.CapacityLimiterStatistics
 .. autoclass:: anyio.SemaphoreStatistics
 
-.. autofunction:: anyio.create_event
-.. autofunction:: anyio.create_lock
-.. autofunction:: anyio.create_condition
-.. autofunction:: anyio.create_semaphore
-.. autofunction:: anyio.create_capacity_limiter
-
 Operating system signals
 ------------------------
 
 .. autofunction:: anyio.open_signal_receiver
 
 Low level operations
 --------------------
 
 .. autofunction:: anyio.lowlevel.checkpoint
 .. autofunction:: anyio.lowlevel.checkpoint_if_cancelled
 .. autofunction:: anyio.lowlevel.cancel_shielded_checkpoint
 
 .. autoclass:: anyio.lowlevel.RunVar
 
-Compatibility
--------------
-
-.. autofunction:: anyio.maybe_async
-.. autofunction:: anyio.maybe_async_cm
-
 Testing and debugging
 ---------------------
 
 .. autoclass:: anyio.TaskInfo
 .. autofunction:: anyio.get_current_task
 .. autofunction:: anyio.get_running_tasks
 .. autofunction:: anyio.wait_all_tasks_blocked
@@ -198,11 +184,10 @@
 ----------
 
 .. autoexception:: anyio.BrokenResourceError
 .. autoexception:: anyio.BusyResourceError
 .. autoexception:: anyio.ClosedResourceError
 .. autoexception:: anyio.DelimiterNotFound
 .. autoexception:: anyio.EndOfStream
-.. autoexception:: anyio.ExceptionGroup
 .. autoexception:: anyio.IncompleteRead
 .. autoexception:: anyio.TypedAttributeLookupError
 .. autoexception:: anyio.WouldBlock
```

### Comparing `anyio-3.7.1/docs/basics.rst` & `anyio-4.0.0rc1/docs/basics.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 The basics
 ==========
 
 .. py:currentmodule:: anyio
 
-AnyIO requires Python 3.7 or later to run. It is recommended that you set up a virtualenv_ when
-developing or playing around with AnyIO.
+AnyIO requires Python 3.8 or later to run. It is recommended that you set up a
+virtualenv_ when developing or playing around with AnyIO.
 
 Installation
 ------------
 
 To install AnyIO, run:
 
 .. code-block:: bash
@@ -30,62 +30,70 @@
 
 
     async def main():
         print('Hello, world!')
 
     run(main)
 
-This will run the program above on the default backend (asyncio). To run it on another supported
-backend, say trio_, you can use the ``backend`` argument, like so::
+This will run the program above on the default backend (asyncio). To run it on another
+supported backend, say trio_, you can use the ``backend`` argument, like so::
 
     run(main, backend='trio')
 
-But AnyIO code is not required to be run via :func:`run`. You can just as well use the native
-``run()`` function of the backend library::
+But AnyIO code is not required to be run via :func:`run`. You can just as well use the
+native ``run()`` function of the backend library::
 
     import sniffio
     import trio
     from anyio import sleep
 
 
     async def main():
         print('Hello')
         await sleep(1)
         print("I'm running on", sniffio.current_async_library())
 
     trio.run(main)
 
+.. versionchanged:: 4.0.0
+    On the ``asyncio`` backend, ``anyio.run()`` now uses a back-ported version of
+    :class:`asyncio.Runner` on Pythons older than 3.11.
+
 .. _backend options:
 
 Backend specific options
 ------------------------
 
-Asyncio:
-
-* ``debug`` (``bool``, default=False): Enables `debug mode`_ in the event loop
-* ``use_uvloop`` (``bool``, default=False): Use the faster uvloop_ event loop implementation, if
-  available
-* ``policy`` (``AbstractEventLoopPolicy``, default=None): the event loop policy instance to use
-  for creating a new event loop (overrides ``use_uvloop``)
-
-Trio: options covered in the
-`official documentation <https://trio.readthedocs.io/en/stable/reference-core.html#trio.run>`_
+**Asyncio**:
 
-.. note:: The default value of ``use_uvloop`` was ``True`` before v3.2.0.
+* options covered in the documentation of :class:`asyncio.Runner`
+* ``use_uvloop`` (``bool``, default=False): Use the faster uvloop_ event loop
+  implementation, if available (this is a shorthand for passing
+  ``loop_factory=uvloop.new_event_loop``, and is ignored if ``loop_factory`` is passed
+  a value other than ``None``)
+
+**Trio**: options covered in the
+`official documentation
+<https://trio.readthedocs.io/en/stable/reference-core.html#trio.run>`_
+
+.. versionchanged:: 3.2.0
+    The default value of ``use_uvloop`` was changed to ``False``.
+.. versionchanged:: 4.0.0
+    The ``policy`` option was replaced with ``loop_factory``.
 
-.. _debug mode: https://docs.python.org/3/library/asyncio-eventloop.html#enabling-debug-mode
 .. _uvloop: https://pypi.org/project/uvloop/
 
 Using native async libraries
 ----------------------------
 
-AnyIO lets you mix and match code written for AnyIO and code written for the asynchronous framework
-of your choice. There are a few rules to keep in mind however:
+AnyIO lets you mix and match code written for AnyIO and code written for the
+asynchronous framework of your choice. There are a few rules to keep in mind however:
 
-* You can only use "native" libraries for the backend you're running, so you cannot, for example,
-  use a library written for trio together with a library written for asyncio.
-* Tasks spawned by these "native" libraries on backends other than trio_ are not subject to the
-  cancellation rules enforced by AnyIO
-* Threads spawned outside of AnyIO cannot use :func:`.from_thread.run` to call asynchronous code
+* You can only use "native" libraries for the backend you're running, so you cannot, for
+  example, use a library written for trio together with a library written for asyncio.
+* Tasks spawned by these "native" libraries on backends other than trio_ are not subject
+  to the cancellation rules enforced by AnyIO
+* Threads spawned outside of AnyIO cannot use :func:`.from_thread.run` to call
+  asynchronous code
 
 .. _virtualenv: https://docs.python-guide.org/dev/virtualenvs/
 .. _trio: https://github.com/python-trio/trio
```

### Comparing `anyio-3.7.1/docs/cancellation.rst` & `anyio-4.0.0rc1/docs/cancellation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Cancellation and timeouts
 =========================
 
 .. py:currentmodule:: anyio
 
-The ability to cancel tasks is the foremost advantage of the asynchronous programming model.
-Threads, on the other hand, cannot be forcibly killed and shutting them down will require perfect
-cooperation from the code running in them.
-
-Cancellation in AnyIO follows the model established by the trio_ framework. This means that
-cancellation of tasks is done via so called *cancel scopes*. Cancel scopes are used as context
-managers and can be nested. Cancelling a cancel scope cancels all cancel scopes nested within it.
-If a task is waiting on something, it is cancelled immediately. If the task is just starting, it
-will run until it first tries to run an operation requiring waiting, such as :func:`~sleep`.
+The ability to cancel tasks is the foremost advantage of the asynchronous programming
+model. Threads, on the other hand, cannot be forcibly killed and shutting them down will
+require perfect cooperation from the code running in them.
+
+Cancellation in AnyIO follows the model established by the Trio_ framework. This means
+that cancellation of tasks is done via so called *cancel scopes*. Cancel scopes are used
+as context managers and can be nested. Cancelling a cancel scope cancels all cancel
+scopes nested within it. If a task is waiting on something, it is cancelled immediately.
+If the task is just starting, it will run until it first tries to run an operation
+requiring waiting, such as :func:`~sleep`.
 
-A task group contains its own cancel scope. The entire task group can be cancelled by cancelling
-this scope.
+A task group contains its own cancel scope. The entire task group can be cancelled by
+cancelling this scope.
 
-.. _trio: https://trio.readthedocs.io/en/latest/reference-core.html#cancellation-and-timeouts
+.. _Trio: https://trio.readthedocs.io/en/latest/reference-core.html#cancellation-and-timeouts
 
 Timeouts
 --------
 
-Networked operations can often take a long time, and you usually want to set up some kind of a
-timeout to ensure that your application doesn't stall forever. There are two principal ways to do
-this: :func:`~move_on_after` and :func:`~fail_after`. Both are used as synchronous
-context managers. The difference between these two is that the former simply exits the context
-block prematurely on a timeout, while the other raises a :exc:`TimeoutError`.
+Networked operations can often take a long time, and you usually want to set up some
+kind of a timeout to ensure that your application doesn't stall forever. There are two
+principal ways to do this: :func:`~move_on_after` and :func:`~fail_after`. Both are used
+as synchronous context managers. The difference between these two is that the former
+simply exits the context block prematurely on a timeout, while the other raises a
+:exc:`TimeoutError`.
 
 Both methods create a new cancel scope, and you can check the deadline by accessing the
 :attr:`~.CancelScope.deadline` attribute. Note, however, that an outer cancel scope
 may have an earlier deadline than your current cancel scope. To check the actual
 deadline, you can use the :func:`~current_effective_deadline` function.
 
 Here's how you typically use timeouts::
@@ -40,24 +42,29 @@
     async def main():
         async with create_task_group() as tg:
             with move_on_after(1) as scope:
                 print('Starting sleep')
                 await sleep(2)
                 print('This should never be printed')
 
-            # The cancel_called property will be True if timeout was reached
-            print('Exited cancel scope, cancelled =', scope.cancel_called)
+            # The cancelled_caught property will be True if timeout was reached
+            print('Exited cancel scope, cancelled =', scope.cancelled_caught)
 
     run(main)
 
+.. note:: It's recommended not to directly cancel a scope from :func:`~fail_after`, as
+    that may currently result in :exc:`TimeoutError` being erroneously raised if exiting
+    the scope is delayed long enough for the deadline to be exceeded.
+
 Shielding
 ---------
 
-There are cases where you want to shield your task from cancellation, at least temporarily.
-The most important such use case is performing shutdown procedures on asynchronous resources.
+There are cases where you want to shield your task from cancellation, at least
+temporarily. The most important such use case is performing shutdown procedures on
+asynchronous resources.
 
 To accomplish this, open a new cancel scope with the ``shield=True`` argument::
 
     from anyio import CancelScope, create_task_group, sleep, run
 
 
     async def external_task():
@@ -73,125 +80,130 @@
                 tg.cancel_scope.cancel()
                 print('Started sleeping in the host task')
                 await sleep(1)
                 print('Finished sleeping in the host task')
 
     run(main)
 
-The shielded block will be exempt from cancellation except when the shielded block itself is being
-cancelled. Shielding a cancel scope is often best combined with :func:`~move_on_after` or
-:func:`~fail_after`, both of which also accept ``shield=True``.
+The shielded block will be exempt from cancellation except when the shielded block
+itself is being cancelled. Shielding a cancel scope is often best combined with
+:func:`~move_on_after` or :func:`~fail_after`, both of which also accept
+``shield=True``.
 
 Finalization
 ------------
 
-Sometimes you may want to perform cleanup operations in response to the failure of the operation::
+Sometimes you may want to perform cleanup operations in response to the failure of the
+operation::
 
     async def do_something():
         try:
             await run_async_stuff()
         except BaseException:
             # (perform cleanup)
             raise
 
-In some specific cases, you might only want to catch the cancellation exception. This is tricky
-because each async framework has its own exception class for that and AnyIO cannot control which
-exception is raised in the task when it's cancelled. To work around that, AnyIO provides a way to
-retrieve the exception class specific to the currently running async framework, using
-:func:`~get_cancelled_exc_class`::
+In some specific cases, you might only want to catch the cancellation exception. This is
+tricky because each async framework has its own exception class for that and AnyIO
+cannot control which exception is raised in the task when it's cancelled. To work around
+that, AnyIO provides a way to retrieve the exception class specific to the currently
+running async framework, using:func:`~get_cancelled_exc_class`::
 
     from anyio import get_cancelled_exc_class
 
 
     async def do_something():
         try:
             await run_async_stuff()
         except get_cancelled_exc_class():
             # (perform cleanup)
             raise
 
-.. warning:: Always reraise the cancellation exception if you catch it. Failing to do so may cause
-             undefined behavior in your application.
+.. warning:: Always reraise the cancellation exception if you catch it. Failing to do so
+    may cause undefined behavior in your application.
 
-If you need to use ``await`` during finalization, you need to enclose it in a shielded cancel
-scope, or the operation will be cancelled immediately since it's in an already cancelled scope::
+If you need to use ``await`` during finalization, you need to enclose it in a shielded
+cancel scope, or the operation will be cancelled immediately since it's in an already
+cancelled scope::
 
     async def do_something():
         try:
             await run_async_stuff()
         except get_cancelled_exc_class():
             with CancelScope(shield=True):
                 await some_cleanup_function()
 
             raise
 
 Avoiding cancel scope stack corruption
 --------------------------------------
 
-When using cancel scopes, it is important that they are entered and exited in LIFO (last in, first
-out) order within each task. This is usually not an issue since cancel scopes are normally used as
-context managers. However, in certain situations, cancel scope stack corruption might still occur:
-
-* Manually calling ``CancelScope.__enter__()`` and ``CancelScope.__exit__()``, usually from another
-  context manager class, in the wrong order
-* Using cancel scopes with ``[Async]ExitStack`` in a manner that couldn't be achieved by nesting
-  them as context managers
-* Using the low level coroutine protocol to execute parts of the coroutine function in different
-  cancel scopes
+When using cancel scopes, it is important that they are entered and exited in LIFO (last
+in, first out) order within each task. This is usually not an issue since cancel scopes
+are normally used as context managers. However, in certain situations, cancel scope
+stack corruption might still occur:
+
+* Manually calling ``CancelScope.__enter__()`` and ``CancelScope.__exit__()``, usually
+  from another context manager class, in the wrong order
+* Using cancel scopes with ``[Async]ExitStack`` in a manner that couldn't be achieved by
+  nesting them as context managers
+* Using the low level coroutine protocol to execute parts of the coroutine function in
+  different cancel scopes
 * Yielding in an async generator while enclosed in a cancel scope
 
-Remember that task groups contain their own cancel scopes so the same list of risky situations
-applies to them too.
+Remember that task groups contain their own cancel scopes so the same list of risky
+situations applies to them too.
 
 As an example, the following code is highly dubious::
 
     # Bad!
     async def some_generator():
         async with create_task_group() as tg:
             tg.start_soon(foo)
             yield
 
-The problem with this code is that it violates structural concurrency: what happens if the spawned
-task raises an exception? The host task would be cancelled as a result, but the host task might be
-long gone by the time that happens. Even if it weren't, any enclosing ``try...except`` in the
-generator would not be triggered. Unfortunately there is currently no way to automatically detect
-this condition in AnyIO, so in practice you may simply experience some weird behavior in your
-application as a consequence of running code like above.
-
-Depending on how they are used, this pattern is, however, *usually* safe to use in asynchronous
-context managers, so long as you make sure that the same host task keeps running throughout the
-entire enclosed code block::
+The problem with this code is that it violates structural concurrency: what happens if
+the spawned task raises an exception? The host task would be cancelled as a result, but
+the host task might be long gone by the time that happens. Even if it weren't, any
+enclosing ``try...except`` in the generator would not be triggered. Unfortunately there
+is currently no way to automatically detect this condition in AnyIO, so in practice you
+may simply experience some weird behavior in your application as a consequence of
+running code like above.
+
+Depending on how they are used, this pattern is, however, *usually* safe to use in
+asynchronous context managers, so long as you make sure that the same host task keeps
+running throughout the entire enclosed code block::
 
     # Okay in most cases!
     @async_context_manager
     async def some_context_manager():
         async with create_task_group() as tg:
             tg.start_soon(foo)
             yield
 
 Prior to AnyIO 3.6, this usage pattern was also invalid in pytest's asynchronous
 generator fixtures. Starting from 3.6, however, each async generator fixture is run from
 start to end in the same task, making it possible to have task groups or cancel scopes
 safely straddle the ``yield``.
 
-When you're implementing the async context manager protocol manually and your async context manager
-needs to use other context managers, you may find it necessary to call their ``__aenter__()`` and
-``__aexit__()`` directly. In such cases, it is absolutely vital to ensure that their ``__aexit__()``
-methods are called in the exact reverse order of the ``__aenter__()`` calls. To this end, you may
-find the :class:`~contextlib.AsyncExitStack` (available from Python 3.7 up, or as a backport_)
-class very useful::
+When you're implementing the async context manager protocol manually and your async
+context manager needs to use other context managers, you may find it necessary to call
+their ``__aenter__()`` and ``__aexit__()`` directly. In such cases, it is absolutely
+vital to ensure that their ``__aexit__()`` methods are called in the exact reverse order
+of the ``__aenter__()`` calls. To this end, you may find the
+:class:`~contextlib.AsyncExitStack` class very useful::
 
     from contextlib import AsyncExitStack
 
     from anyio import create_task_group
 
 
     class MyAsyncContextManager:
         async def __aenter__(self):
             self._exitstack = AsyncExitStack()
             await self._exitstack.__aenter__()
-            self._task_group = await self._exitstack.enter_async_context(create_task_group())
+            self._task_group = await self._exitstack.enter_async_context(
+                create_task_group()
+            )
 
         async def __aexit__(self, exc_type, exc_val, exc_tb):
             return await self._exitstack.__aexit__(exc_type, exc_val, exc_tb)
-
-.. _backport: https://pypi.org/project/async-exit-stack/
```

### Comparing `anyio-3.7.1/docs/conf.py` & `anyio-4.0.0rc1/docs/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from packaging.version import parse
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx_autodoc_typehints",
-    "sphinxcontrib.jquery",
 ]
 
 templates_path = ["_templates"]
 source_suffix = ".rst"
 master_doc = "index"
 project = "AnyIO"
 author = "Alex Grönholm"
```

### Comparing `anyio-3.7.1/docs/contributing.rst` & `anyio-4.0.0rc1/docs/contributing.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Contributing to AnyIO
 =====================
 
-If you wish to contribute a fix or feature to AnyIO, please follow the following guidelines.
+If you wish to contribute a fix or feature to AnyIO, please follow the following
+guidelines.
 
-When you make a pull request against the main AnyIO codebase, Github runs the AnyIO test suite
-against your modified code. Before making a pull request, you should ensure that the modified code
-passes tests locally. To that end, the use of tox_ is recommended. The default tox run first runs
-code style fixing tools and then the actual test suite. To only run the code style fixers, run
-``tox -e lint``. To run the checks on all environments in parallel, invoke tox with ``tox -p``.
-
-To build the documentation, run ``tox -e docs`` which will generate a directory named ``build``
-in which you may view the formatted HTML documentation.
-
-AnyIO uses pre-commit_ to perform several code style/quality checks. It is recommended to activate
-pre-commit_ on your local clone of the repository (using ``pre-commit install``) to ensure that
-your changes will pass the same checks on GitHub.
+When you make a pull request against the main AnyIO codebase, Github runs the AnyIO test
+suite against your modified code. Before making a pull request, you should ensure that
+the modified code passes tests locally. To that end, the use of tox_ is recommended. The
+default tox run first runs ``pre-commit`` and then the actual test suite. To run the
+checks on all environments in parallel, invoke tox with ``tox -p``.
+
+To build the documentation, run ``tox -e docs`` which will generate a directory named
+``build`` in which you may view the formatted HTML documentation.
+
+AnyIO uses pre-commit_ to perform several code style/quality checks. It is recommended
+to activate pre-commit_ on your local clone of the repository (using
+``pre-commit install``) to ensure that your changes will pass the same checks on GitHub.
 
 .. _tox: https://tox.readthedocs.io/en/latest/install.html
 .. _pre-commit: https://pre-commit.com/#installation
 
 Making a pull request on Github
 -------------------------------
 
@@ -27,19 +28,21 @@
 #. Fork the repository (if you don't have your own fork of it yet) by navigating to the
    `main AnyIO repository`_ and clicking on "Fork" near the top right corner.
 #. Clone the forked repository to your local machine with
    ``git clone git@github.com/yourusername/anyio``.
 #. Create a branch for your pull request, like ``git checkout -b myfixname``
 #. Make the desired changes to the code base.
 #. Commit your changes locally. If your changes close an existing issue, add the text
-   ``Fixes XXX.`` or ``Closes XXX.`` to the commit message (where XXX is the issue number).
+   ``Fixes XXX.`` or ``Closes XXX.`` to the commit message (where XXX is the issue
+   number).
 #. Push the changeset(s) to your forked repository (``git push``)
 #. Navigate to Pull requests page on the original repository (not your fork) and click
    "New pull request"
 #. Click on the text "compare across forks".
 #. Select your own fork as the head repository and then select the correct branch name.
 #. Click on "Create pull request".
 
 If you have trouble, consult the `pull request making guide`_ on opensource.com.
 
 .. _main AnyIO repository: https://github.com/agronholm/anyio
-.. _pull request making guide: https://opensource.com/article/19/7/create-pull-request-github
+.. _pull request making guide:
+    https://opensource.com/article/19/7/create-pull-request-github
```

### Comparing `anyio-3.7.1/docs/faq.rst` & `anyio-4.0.0rc1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.1/docs/fileio.rst` & `anyio-4.0.0rc1/docs/fileio.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.1/docs/migration.rst` & `anyio-4.0.0rc1/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.1/docs/networking.rst` & `anyio-4.0.0rc1/docs/networking.rst`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 offered by each of its supported backends.
 
 Currently AnyIO offers the following networking functionality:
 
 * TCP sockets (client + server)
 * UNIX domain sockets (client + server)
 * UDP sockets
+* UNIX datagram sockets
 
 More exotic forms of networking such as raw sockets and SCTP are currently not supported.
 
 .. warning:: Unlike the standard BSD sockets interface and most other networking libraries, AnyIO
     (from 2.0 onwards) signals the end of any stream by raising the
     :exc:`~EndOfStream` exception instead of returning an empty bytes object.
 
@@ -185,7 +186,45 @@
 
     async def main():
         async with await create_connected_udp_socket(
                 remote_host='hostname', remote_port=1234) as udp:
             await udp.send(b'Hi there!\n')
 
     run(main)
+
+Working with UNIX datagram sockets
+----------------------------------
+
+UNIX datagram sockets are a subset of UNIX domain sockets, with the difference being that while UNIX
+sockets implement reliable communication of a continuous byte stream (similarly to TCP), UNIX
+datagram sockets implement communication of data packets (similarly to UDP).
+
+The API for UNIX datagram sockets is modeled after the one for UDP sockets, except that instead of
+host/port combinations, you use file system paths - here is the UDP "hello" service example written
+with UNIX datagram sockets::
+
+    from anyio import create_unix_datagram_socket, run
+
+
+    async def main():
+        async with await create_unix_datagram_socket(local_path='/tmp/mysock') as unix_dg:
+            async for packet, path in unix_dg:
+                await unix_dg.sendto(b'Hello, ' + packet, path)
+
+    run(main)
+
+
+.. note:: If ``local_path`` is not set, the UNIX datagram socket will be bound on an unnamed address,
+          and will generally not be able to receive datagrams from other UNIX datagram sockets.
+
+Similarly to UDP sockets, if your case involves sending lots of packets to a single destination, you
+can "connect" your UNIX datagram socket to a specific path to avoid having to pass the path every
+time you send data to the peer::
+
+    from anyio import create_connected_unix_datagram_socket, run
+
+
+    async def main():
+        async with await create_connected_unix_datagram_socket(remote_path='/dev/log') as unix_dg:
+            await unix_dg.send(b'Hi there!\n')
+
+    run(main)
```

### Comparing `anyio-3.7.1/docs/signals.rst` & `anyio-4.0.0rc1/docs/signals.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.1/docs/streams.rst` & `anyio-4.0.0rc1/docs/streams.rst`

 * *Files 9% similar despite different names*

```diff
@@ -45,37 +45,44 @@
 
 The receive ends of memory object streams can be iterated using the async iteration protocol.
 The loop exits when all clones of the send stream have been closed.
 
 Example::
 
     from anyio import create_task_group, create_memory_object_stream, run
+    from anyio.streams.memory import MemoryObjectReceiveStream
 
 
-    async def process_items(receive_stream):
+    async def process_items(receive_stream: MemoryObjectReceiveStream[str]) -> None:
         async with receive_stream:
             async for item in receive_stream:
                 print('received', item)
 
 
     async def main():
-        send_stream, receive_stream = create_memory_object_stream()
+        # The [str] specifies the type of the objects being passed through the
+        # memory object stream. This is a bit of trick, as create_memory_object_stream
+        # is actually a class masquerading as a function.
+        send_stream, receive_stream = create_memory_object_stream[str]()
         async with create_task_group() as tg:
             tg.start_soon(process_items, receive_stream)
             async with send_stream:
                 for num in range(10):
                     await send_stream.send(f'number {num}')
 
     run(main)
 
 In contrast to other AnyIO streams (but in line with trio's Channels), memory object streams can be
 closed synchronously, using either the ``close()`` method or by using the stream as a context
 manager::
 
-    def synchronous_callback(send_stream: MemoryObjectSendStream) -> None:
+    from anyio.streams.memory import MemoryObjectSendStream
+
+
+    def synchronous_callback(send_stream: MemoryObjectSendStream[str]) -> None:
         with send_stream:
             send_stream.send_nowait('hello')
 
 Stapled streams
 ---------------
 
 A stapled stream combines any mutually compatible receive and send stream together, forming a
@@ -98,15 +105,15 @@
 Example::
 
     from anyio import run, create_memory_object_stream
     from anyio.streams.buffered import BufferedByteReceiveStream
 
 
     async def main():
-        send, receive = create_memory_object_stream(4)
+        send, receive = create_memory_object_stream[bytes](4)
         buffered = BufferedByteReceiveStream(receive)
         for part in b'hel', b'lo, ', b'wo', b'rld!':
             await send.send(part)
 
         result = await buffered.receive_exactly(8)
         print(repr(result))
 
@@ -128,15 +135,15 @@
 Example::
 
     from anyio import run, create_memory_object_stream
     from anyio.streams.text import TextReceiveStream, TextSendStream
 
 
     async def main():
-        bytes_send, bytes_receive = create_memory_object_stream(1)
+        bytes_send, bytes_receive = create_memory_object_stream[bytes](1)
         text_send = TextSendStream(bytes_send)
         await text_send.send('åäö')
         result = await bytes_receive.receive()
         print(repr(result))
 
         text_receive = TextReceiveStream(bytes_receive)
         await bytes_send.send(result)
```

### Comparing `anyio-3.7.1/docs/subprocesses.rst` & `anyio-4.0.0rc1/docs/subprocesses.rst`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,14 @@
 opening a process handle for you that gives you more control over the subprocess.
 
 You can either give the command as a string, in which case it is passed to your default shell
 (equivalent to ``shell=True`` in :func:`subprocess.run`), or as a sequence of strings
 (``shell=False``) in which case the executable is the first item in the sequence and the rest are
 arguments passed to it.
 
-.. note:: On Windows and Python 3.7 and earlier, asyncio uses :class:`~asyncio.SelectorEventLoop`
-    by default which does not support subprocesses. It is recommended to upgrade to at least Python
-    3.8 to overcome this limitation.
-
 Running one-shot commands
 -------------------------
 
 To run an external command with one call, use :func:`~run_process`::
 
     from anyio import run_process, run
```

### Comparing `anyio-3.7.1/docs/support.rst` & `anyio-4.0.0rc1/docs/support.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.1/docs/synchronization.rst` & `anyio-4.0.0rc1/docs/synchronization.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.1/docs/tasks.rst` & `anyio-4.0.0rc1/docs/tasks.rst`

 * *Files 18% similar despite different names*

```diff
@@ -83,24 +83,78 @@
 Handling multiple errors in a task group
 ----------------------------------------
 
 It is possible for more than one task to raise an exception in a task group. This can happen when
 a task reacts to cancellation by entering either an exception handler block or a ``finally:``
 block and raises an exception there. This raises the question: which exception is propagated from
 the task group context manager? The answer is "both". In practice this means that a special
-exception, :exc:`~ExceptionGroup` is raised which contains both exception objects.
-Unfortunately this complicates any code that wishes to catch a specific exception because it could
-be wrapped in an :exc:`~ExceptionGroup`.
+exception, :exc:`ExceptionGroup` (or :exc:`BaseExceptionGroup`) is raised which contains both
+exception objects.
+
+To catch such exceptions potentially nested in groups, special measures are required.
+On Python 3.11 and later, you can use the ``except*`` syntax to catch multiple exceptions::
+
+    try:
+        async with TaskGroup() as tg:
+            tg.start_soon(some_task)
+            tg.start_soon(another_task)
+    except* ValueError:
+        ...  # handle each ValueError
+    except* KeyError:
+        ...  # handle each KeyError
+
+If compatibility with older Python versions is required, you can use the ``catch()`` function from
+the exceptiongroup_ package::
+
+    from exceptiongroup import catch
+
+    def handle_valueerror(exc: ValueError) -> None:
+        ...  # handle each ValueError
+
+    def handle_keyerror(exc: KeyError) -> None:
+        ...  # handle each KeyError
+
+    with catch({
+        ValueError: handle_valueerror,
+        KeyError: handle_keyerror
+    }):
+        async with TaskGroup() as tg:
+            tg.start_soon(some_task)
+            tg.start_soon(another_task)
+
+If you need to set local variables in the handlers, declare them as ``nonlocal``::
+
+    def handle_valueerror(exc):
+        nonlocal somevariable
+        somevariable = 'whatever'
+
+.. _exceptiongroup: https://pypi.org/project/exceptiongroup/
 
 Context propagation
 -------------------
 
 Whenever a new task is spawned, `context`_ will be copied to the new task. It is important to note
-*which* content will be copied to the newly spawned task. It is not the context of the task group's
+*which* context will be copied to the newly spawned task. It is not the context of the task group's
 host task that will be copied, but the context of the task that calls
 :meth:`TaskGroup.start() <.abc.TaskGroup.start>` or
 :meth:`TaskGroup.start_soon() <.abc.TaskGroup.start_soon>`.
 
-.. note:: Context propagation **does not work** on asyncio when using Python 3.6, as asyncio
-    support for this only landed in v3.7.
-
 .. _context: https://docs.python.org/3/library/contextvars.html
+
+Differences with asyncio.TaskGroup
+----------------------------------
+
+The :class:`asyncio.TaskGroup` class, added in Python 3.11, is very similar in design to
+the AnyIO :class:`~TaskGroup` class. The asyncio counterpart has some important
+differences in its semantics, however:
+
+* Tasks are spawned solely through :meth:`~asyncio.TaskGroup.create_task`; there is no
+  ``start()`` or ``start_soon()`` method
+* The :meth:`~asyncio.TaskGroup.create_task` method returns a task object which can be
+  awaited on (or cancelled)
+* Tasks spawned via :meth:`~asyncio.TaskGroup.create_task` can only be cancelled
+  individually (there is no ``cancel()`` method or similar in the task group)
+* When a task spawned via :meth:`~asyncio.TaskGroup.create_task` is cancelled before its
+  coroutine has started running, it will not get a chance to handle the cancellation
+  exception
+* :class:`asyncio.TaskGroup` does not allow starting new tasks after an exception in
+  one of the tasks has triggered a shutdown of the task group
```

### Comparing `anyio-3.7.1/docs/testing.rst` & `anyio-4.0.0rc1/docs/testing.rst`

 * *Files 24% similar despite different names*

```diff
@@ -141,23 +141,36 @@
 Technical details
 -----------------
 
 The fixtures and tests are run by a "test runner", implemented separately for each backend.
 The test runner keeps an event loop open during the request, making it possible for code in
 fixtures to communicate with the code in the tests (and each other).
 
-The test runner is created when the first matching async test or fixture is about to be run, and
-shut down when that same fixture is being torn down or the test has finished running. As such,
-if no async fixtures are used, a separate test runner is created for each test. Conversely, if
-even one async fixture (scoped higher than ``function``) is shared across all tests, only one test
-runner will be created during the test session.
-
-For async generator based fixtures, the test runner spawns a task that handles both the setup and
-teardown phases to enable context-sensitive code to work properly. A common example of this is
-providing a task group as a fixture.
-
-Since each test and fixture run in their own separate tasks, no changes to any context
-variables will propagate out of them to tests or other fixtures. This is in line with
-``pytest-asyncio``, but in contrast to ``pytest-trio`` where all fixtures and tests
-`share the same context`_.
+The test runner is created when the first matching async test or fixture is about to be
+run, and shut down when that same fixture is being torn down or the test has finished
+running. As such, if no higher-order (scoped ``class`` or higher) async fixtures are
+used, a separate test runner is created for each matching test. Conversely, if even one
+async fixture, scoped higher than ``function``, is shared across all tests, only one
+test runner will be created during the test session.
 
-.. _share the same context: https://pytest-trio.readthedocs.io/en/stable/reference.html#handling-of-contextvars
+Context variable propagation
+++++++++++++++++++++++++++++
+
+The asynchronous test runner runs all async fixtures and tests in the same task, so
+context variables set in async fixtures or tests, within an async test runner, will
+affect other async fixtures and tests within the same runner. However, these context
+variables are **not** carried over to synchronous tests and fixtures, or to other async
+test runners.
+
+Comparison with other async test runners
+++++++++++++++++++++++++++++++++++++++++
+
+The ``pytest-asyncio`` library only works with asyncio code. Like the AnyIO pytest
+plugin, it can be made to support higher order fixtures (by specifying a higher order
+``event_loop`` fixture). However, it runs the setup and teardown phases of each async
+fixture in a new async task per operation, making context variable propagation
+impossible and preventing task groups and cancel scopes from functioning properly.
+
+The ``pytest-trio`` library, made for testing Trio projects, works only with Trio code.
+Additionally, it only supports function scoped async fixtures. Another significant
+difference with the AnyIO pytest plugin is that attempts to run the setup and teardown
+for async fixtures concurrently when their dependency graphs allow that.
```

### Comparing `anyio-3.7.1/docs/threads.rst` & `anyio-4.0.0rc1/docs/threads.rst`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 .. py:currentmodule:: anyio
 
 Practical asynchronous applications occasionally need to run network, file or computationally
 expensive operations. Such operations would normally block the asynchronous event loop, leading to
 performance issues. The solution is to run such code in *worker threads*. Using worker threads lets
 the event loop continue running other tasks while the worker thread runs the blocking call.
 
- .. caution:: Do not spawn too many threads, as the context switching overhead may cause your
-    system to slow down to a crawl. A few dozen threads should be fine, but hundreds are probably
-    bad. Consider using AnyIO's semaphores to limit the maximum number of threads.
-
 Running a function in a worker thread
 -------------------------------------
 
 To run a (synchronous) callable in a worker thread::
 
     import time
```

### Comparing `anyio-3.7.1/docs/typedattrs.rst` & `anyio-4.0.0rc1/docs/typedattrs.rst`

 * *Files identical despite different names*

### Comparing `anyio-3.7.1/docs/versionhistory.rst` & `anyio-4.0.0rc1/docs/versionhistory.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,80 @@
 Version history
 ===============
 
 This library adheres to `Semantic Versioning 2.0 <http://semver.org/>`_.
 
+**4.0.0rc1**
+
+- **BACKWARDS INCOMPATIBLE** Replaced AnyIO's own ``ExceptionGroup`` class with the PEP
+  654 ``BaseExceptionGroup`` and ``ExceptionGroup``
+- **BACKWARDS INCOMPATIBLE** Changes to cancellation semantics:
+
+  - Any exceptions raising out of a task groups are now nested inside an
+    ``ExceptionGroup`` (or ``BaseExceptionGroup`` if one or more ``BaseException`` were
+    included)
+  - Fixed task group not raising a cancellation exception on asyncio at exit if no child
+    tasks were spawned and an outer cancellation scope had been cancelled before
+  - Ensured that exiting a ``TaskGroup`` always hits a yield point, regardless of
+    whether there are running child tasks to be waited on
+  - On asyncio, cancel scopes will defer cancelling tasks that are scheduled to resume
+    with a finished future
+  - On asyncio and Python 3.9 or later, cancel scopes now only suppress cancellation
+    exceptions if the cancel message matches the scope
+  - Task groups on all backends now raise a single cancellation exception when an outer
+    cancel scope is cancelled, and no exceptions other than cancellation exceptions are
+    raised in the group
+- **BACKWARDS INCOMPATIBLE** Changes the pytest plugin to run all tests and fixtures in
+  the same task, allowing fixtures to set context variables for tests and other fixtures
+- **BACKWARDS INCOMPATIBLE** Changed ``anyio.Path.relative_to()`` and
+  ``anyio.Path.is_relative_to()`` to only accept one argument, as passing multiple
+  arguments is deprecated as of Python 3.12
+- **BACKWARDS INCOMPATIBLE** Dropped support for spawning tasks from old-style coroutine
+  functions (``@asyncio.coroutine``)
+- **BACKWARDS INCOMPATIBLE** The ``policy`` option on the ``asyncio`` backend was
+  changed to ``loop_factory`` to accommodate ``asyncio.Runner``
+- Changed ``anyio.run()`` to use ``asyncio.Runner`` (or a back-ported version of it on
+  Pythons older than 3.11) on the ``asyncio`` backend
+- Dropped support for Python 3.7
+- Added support for Python 3.12
+- Bumped minimum version of trio to v0.22
+- Added the ``anyio.Path.is_junction()`` and ``anyio.Path.walk()`` methods
+- Added ``create_unix_datagram_socket`` and ``create_connected_unix_datagram_socket`` to
+  create UNIX datagram sockets (PR by Jean Hominal)
+- Added the ``CancelScope.cancelled_caught`` property which tells users if the cancel
+  scope suppressed a cancellation exception
+- Fixed ``fail_after()`` raising an unwarranted ``TimeoutError`` when the cancel scope
+  was cancelled before reaching its deadline
+- Fixed ``MemoryObjectReceiveStream.receive()`` causing the receiving task on asyncio to
+  remain in a cancelled state if the operation was cancelled after an item was queued to
+  be received by the task (but before the task could actually receive the item)
+- Fixed ``TaskGroup.start()`` on asyncio not responding to cancellation from the outside
+- Fixed tasks started from ``BlockingPortal`` not notifying synchronous listeners
+  (``concurrent.futures.wait()``) when they're cancelled
+- Removed unnecessary extra waiting cycle in ``Event.wait()`` on asyncio in the case
+  where the event was not yet set
+
 **3.7.1**
 
 - Fixed sending large buffers via UNIX stream sockets on asyncio
 - Fixed several minor documentation issues (broken links to classes, missing classes or
   attributes)
 
 **3.7.0**
 
 - Dropped support for Python 3.6
 - Improved type annotations:
 
+  - **BACKWARDS INCOMPATIBLE** ``create_memory_object_stream`` no longer accepts an
+    ``item_type`` argument for static typing. Use
+    ``create_memory_object_stream[T_Item]()`` instead. Type checking should no longer
+    fail when annotating memory object streams with uninstantiable item types (PR by
+    Ganden Schaffner)
+  - Several functions and methods that previously only accepted coroutines as the return
+    type of the callable have been amended to accept any awaitables:
   - Several functions and methods that were previously annotated as accepting
     ``Coroutine[Any, Any, Any]`` as the return type of the callable have been amended to
     accept ``Awaitable[Any]`` instead, to allow a slightly broader set of coroutine-like
     inputs, like ``async_generator_asend`` objects returned from the ``asend()`` method
     of async generators, and to match the ``trio`` annotations:
 
     - ``anyio.run()``
@@ -30,15 +87,14 @@
 
     Note that this change involved only changing the type annotations; run-time
     functionality was not altered.
 
   - The ``TaskStatus`` class is now a generic protocol, and should be parametrized to
     indicate the type of the value passed to ``task_status.started()``
   - The ``Listener`` class is now covariant in its stream type
-  - ``create_memory_object_stream()`` now allows passing only ``item_type``
   - Object receive streams are now covariant and object send streams are correspondingly
     contravariant
 - Changed ``TLSAttribute.shared_ciphers`` to match the documented semantics of
   ``SSLSocket.shared_ciphers`` of always returning ``None`` for client-side streams
 - Fixed ``CapacityLimiter`` on the asyncio backend to order waiting tasks in the FIFO
   order (instead of LIFO) (PR by Conor Stevenson)
 - Fixed ``CancelScope.cancel()`` not working on asyncio if called before entering the
@@ -57,203 +113,223 @@
 - Fixed ``CancelScope`` to properly handle asyncio task uncancellation on Python 3.11
   (PR by Nikolay Bryskin)
 - Fixed ``OSError`` when trying to use ``create_tcp_listener()`` to bind to a link-local
   IPv6 address (and worked around related bugs in ``uvloop``)
 - Worked around a `PyPy bug <https://foss.heptapod.net/pypy/pypy/-/issues/3938>`_
   when using ``anyio.getaddrinfo()`` with for IPv6 link-local addresses containing
   interface names
+- Fixed ``from_thread.run`` and ``from_thread.run_sync`` not setting sniffio on asyncio.
+  As a result:
+
+  - Fixed ``from_thread.run_sync`` failing when used to call sniffio-dependent functions
+    on asyncio
+  - Fixed ``from_thread.run`` failing when used to call sniffio-dependent functions on
+    asyncio from a thread running trio or curio
+  - Fixed deadlock when using ``from_thread.start_blocking_portal(backend="asyncio")``
+    in a thread running trio or curio (PR by Ganden Schaffner)
 
 **3.6.2**
 
 - Pinned Trio to < 0.22 to avoid incompatibility with AnyIO's ``ExceptionGroup`` class
   causing ``AttributeError: 'NonBaseMultiError' object has no attribute '_exceptions'``
 
 **3.6.1**
 
 - Fixed exception handler in the asyncio test runner not properly handling a context
   that does not contain the ``exception`` key
 
 **3.6.0**
 
-- Fixed ``TypeError`` in ``get_current_task()`` on asyncio when using a custom ``Task`` factory
+- Fixed ``TypeError`` in ``get_current_task()`` on asyncio when using a custom ``Task``
+  factory
 - Updated type annotations on ``run_process()`` and ``open_process()``:
 
   * ``command`` now accepts accepts bytes and sequences of bytes
   * ``stdin``, ``stdout`` and ``stderr`` now accept file-like objects
     (PR by John T. Wodder II)
 - Changed the pytest plugin to run both the setup and teardown phases of asynchronous
   generator fixtures within a single task to enable use cases such as cancel scopes and
   task groups where a context manager straddles the ``yield``
 
 **3.5.0**
 
-- Added ``start_new_session`` keyword argument to ``run_process()`` and ``open_process()``
-  (PR by Jordan Speicher)
-- Fixed deadlock in synchronization primitives on asyncio which can happen if a task acquiring a
-  primitive is hit with a native (not AnyIO) cancellation with just the right timing, leaving the
-  next acquiring task waiting forever (`#398 <https://github.com/agronholm/anyio/issues/398>`_)
+- Added ``start_new_session`` keyword argument to ``run_process()`` and
+  ``open_process()`` (PR by Jordan Speicher)
+- Fixed deadlock in synchronization primitives on asyncio which can happen if a task
+  acquiring a primitive is hit with a native (not AnyIO) cancellation with just the
+  right timing, leaving the next acquiring task waiting forever
+  (`#398 <https://github.com/agronholm/anyio/issues/398>`_)
 - Added workaround for bpo-46313_ to enable compatibility with OpenSSL 3.0
 
 .. _bpo-46313: https://bugs.python.org/issue46313
 
 **3.4.0**
 
 - Added context propagation to/from worker threads in ``to_thread.run_sync()``,
   ``from_thread.run()`` and ``from_thread.run_sync()``
-  (`#363 <https://github.com/agronholm/anyio/issues/363>`_; partially based on a PR by Sebastián
-  Ramírez)
+  (`#363 <https://github.com/agronholm/anyio/issues/363>`_; partially based on a PR by
+  Sebastián Ramírez)
 
   **NOTE**: Requires Python 3.7 to work properly on asyncio!
-- Fixed race condition in ``Lock`` and ``Semaphore`` classes when a task waiting on ``acquire()``
-  is cancelled while another task is waiting to acquire the same primitive
+- Fixed race condition in ``Lock`` and ``Semaphore`` classes when a task waiting on
+  ``acquire()`` is cancelled while another task is waiting to acquire the same primitive
   (`#387 <https://github.com/agronholm/anyio/issues/387>`_)
 - Fixed async context manager's ``__aexit__()`` method not being called in
   ``BlockingPortal.wrap_async_context_manager()`` if the host task is cancelled
   (`#381 <https://github.com/agronholm/anyio/issues/381>`_; PR by Jonathan Slenders)
 - Fixed worker threads being marked as being event loop threads in sniffio
 - Fixed task parent ID not getting set to the correct value on asyncio
 - Enabled the test suite to run without IPv6 support, trio or pytest plugin autoloading
 
 **3.3.4**
 
-- Fixed ``BrokenResourceError`` instead of ``EndOfStream`` being raised in ``TLSStream`` when the
-  peer abruptly closes the connection while ``TLSStream`` is receiving data with
-  ``standard_compatible=False`` set
+- Fixed ``BrokenResourceError`` instead of ``EndOfStream`` being raised in ``TLSStream``
+  when the peer abruptly closes the connection while ``TLSStream`` is receiving data
+  with ``standard_compatible=False`` set
 
 **3.3.3**
 
-- Fixed UNIX socket listener not setting accepted sockets to non-blocking mode on asyncio
-- Changed unconnected UDP sockets to be always bound to a local port (on "any" interface) to avoid
-  errors on asyncio + Windows
+- Fixed UNIX socket listener not setting accepted sockets to non-blocking mode on
+  asyncio
+- Changed unconnected UDP sockets to be always bound to a local port (on "any"
+  interface) to avoid errors on asyncio + Windows
 
 **3.3.2**
 
-- Fixed cancellation problem on asyncio where level-triggered cancellation for **all** parent
-  cancel scopes would not resume after exiting a shielded nested scope
+- Fixed cancellation problem on asyncio where level-triggered cancellation for **all**
+  parent cancel scopes would not resume after exiting a shielded nested scope
   (`#370 <https://github.com/agronholm/anyio/issues/370>`_)
 
 **3.3.1**
 
 - Added missing documentation for the ``ExceptionGroup.exceptions`` attribute
 - Changed the asyncio test runner not to use uvloop by default (to match the behavior of
   ``anyio.run()``)
-- Fixed ``RuntimeError`` on asyncio when a ``CancelledError`` is raised from a task spawned through
-  a ``BlockingPortal`` (`#357 <https://github.com/agronholm/anyio/issues/357>`_)
-- Fixed asyncio warning about a ``Future`` with an exception that was never retrieved which
-  happened when a socket was already written to but the peer abruptly closed the connection
+- Fixed ``RuntimeError`` on asyncio when a ``CancelledError`` is raised from a task
+  spawned through a ``BlockingPortal``
+  (`#357 <https://github.com/agronholm/anyio/issues/357>`_)
+- Fixed asyncio warning about a ``Future`` with an exception that was never retrieved
+  which happened when a socket was already written to but the peer abruptly closed the
+  connection
 
 **3.3.0**
 
 - Added asynchronous ``Path`` class
-- Added the ``wrap_file()`` function for wrapping existing files as asynchronous file objects
+- Added the ``wrap_file()`` function for wrapping existing files as asynchronous file
+  objects
 - Relaxed the type of the ``path`` initializer argument to ``FileReadStream`` and
-  ``FileWriteStream`` so they accept any path-like object (including the new asynchronous ``Path``
-  class)
+  ``FileWriteStream`` so they accept any path-like object (including the new
+  asynchronous ``Path`` class)
 - Dropped unnecessary dependency on the ``async_generator`` library
-- Changed the generics in ``AsyncFile`` so that the methods correctly return either ``str`` or
-  ``bytes`` based on the argument to ``open_file()``
-- Fixed an asyncio bug where under certain circumstances, a stopping worker thread would still
-  accept new assignments, leading to a hang
+- Changed the generics in ``AsyncFile`` so that the methods correctly return either
+  ``str`` or ``bytes`` based on the argument to ``open_file()``
+- Fixed an asyncio bug where under certain circumstances, a stopping worker thread would
+  still accept new assignments, leading to a hang
 
 **3.2.1**
 
-- Fixed idle thread pruning on asyncio sometimes causing an expired worker thread to be assigned a
-  task
+- Fixed idle thread pruning on asyncio sometimes causing an expired worker thread to be
+  assigned a task
 
 **3.2.0**
 
 - Added Python 3.10 compatibility
-- Added the ability to close memory object streams synchronously (including support for use as a
-  synchronous context manager)
-- Changed the default value of the ``use_uvloop`` asyncio backend option to ``False`` to prevent
-  unsafe event loop policy changes in different threads
+- Added the ability to close memory object streams synchronously (including support for
+  use as a synchronous context manager)
+- Changed the default value of the ``use_uvloop`` asyncio backend option to ``False`` to
+  prevent unsafe event loop policy changes in different threads
 - Fixed ``to_thread.run_sync()`` hanging on the second call on asyncio when used with
   ``loop.run_until_complete()``
-- Fixed ``to_thread.run_sync()`` prematurely marking a worker thread inactive when a task await on
-  the result is cancelled
-- Fixed ``ResourceWarning`` about an unclosed socket when UNIX socket connect fails on asyncio
-- Fixed the type annotation of ``open_signal_receiver()`` as a synchronous context manager
-- Fixed the type annotation of ``DeprecatedAwaitable(|List|Float).__await__`` to match the
-  ``typing.Awaitable`` protocol
+- Fixed ``to_thread.run_sync()`` prematurely marking a worker thread inactive when a
+  task await on the result is cancelled
+- Fixed ``ResourceWarning`` about an unclosed socket when UNIX socket connect fails on
+  asyncio
+- Fixed the type annotation of ``open_signal_receiver()`` as a synchronous context
+  manager
+- Fixed the type annotation of ``DeprecatedAwaitable(|List|Float).__await__`` to match
+  the ``typing.Awaitable`` protocol
 
 **3.1.0**
 
 - Added ``env`` and ``cwd`` keyword arguments to ``run_process()`` and ``open_process``.
 - Added support for mutation of ``CancelScope.shield`` (PR by John Belmonte)
 - Added the ``sleep_forever()`` and ``sleep_until()`` functions
 - Changed asyncio task groups so that if the host and child tasks have only raised
   ``CancelledErrors``, just one ``CancelledError`` will now be raised instead of an
   ``ExceptionGroup``, allowing asyncio to ignore it when it propagates out of the task
 - Changed task names to be converted to ``str`` early on asyncio (PR by Thomas Grainger)
-- Fixed ``sniffio._impl.AsyncLibraryNotFoundError: unknown async library, or not in async context``
-  on asyncio and Python 3.6 when ``to_thread.run_sync()`` is used from
+- Fixed ``sniffio._impl.AsyncLibraryNotFoundError: unknown async library, or not in
+  async context`` on asyncio and Python 3.6 when ``to_thread.run_sync()`` is used from
   ``loop.run_until_complete()``
-- Fixed odd ``ExceptionGroup: 0 exceptions were raised in the task group`` appearing under certain
-  circumstances on asyncio
-- Fixed ``wait_all_tasks_blocked()`` returning prematurely on asyncio when a previously blocked
-  task is cancelled (PR by Thomas Grainger)
-- Fixed declared return type of ``TaskGroup.start()`` (it was declared as ``None``, but anything
-  can be returned from it)
-- Fixed ``TextStream.extra_attributes`` raising ``AttributeError`` (PR by Thomas Grainger)
+- Fixed odd ``ExceptionGroup: 0 exceptions were raised in the task group`` appearing
+  under certain circumstances on asyncio
+- Fixed ``wait_all_tasks_blocked()`` returning prematurely on asyncio when a previously
+  blocked task is cancelled (PR by Thomas Grainger)
+- Fixed declared return type of ``TaskGroup.start()`` (it was declared as ``None``, but
+  anything can be returned from it)
+- Fixed ``TextStream.extra_attributes`` raising ``AttributeError`` (PR by Thomas
+  Grainger)
 - Fixed ``await maybe_async(current_task())`` returning ``None`` (PR by Thomas Grainger)
-- Fixed: ``pickle.dumps(current_task())`` now correctly raises ``TypeError`` instead of pickling to
-  ``None`` (PR by Thomas Grainger)
-- Fixed return type annotation of ``Event.wait()`` (``bool`` → ``None``) (PR by Thomas Grainger)
-- Fixed return type annotation of ``RunVar.get()`` to return either the type of the default value
-  or the type of the contained value (PR by Thomas Grainger)
-- Fixed a deprecation warning message to refer to ``maybe_async()`` and not ``maybe_awaitable()``
-  (PR by Thomas Grainger)
-- Filled in argument and return types for all functions and methods previously missing them
-  (PR by Thomas Grainger)
+- Fixed: ``pickle.dumps(current_task())`` now correctly raises ``TypeError`` instead of
+  pickling to ``None`` (PR by Thomas Grainger)
+- Fixed return type annotation of ``Event.wait()`` (``bool`` → ``None``) (PR by Thomas
+  Grainger)
+- Fixed return type annotation of ``RunVar.get()`` to return either the type of the
+  default value or the type of the contained value (PR by Thomas Grainger)
+- Fixed a deprecation warning message to refer to ``maybe_async()`` and not
+  ``maybe_awaitable()`` (PR by Thomas Grainger)
+- Filled in argument and return types for all functions and methods previously missing
+  them (PR by Thomas Grainger)
 
 **3.0.1**
 
-- Fixed ``to_thread.run_sync()`` raising ``RuntimeError`` on asyncio when no "root" task could be
-  found for setting up a cleanup callback. This was a problem at least on Tornado and possibly also
-  Twisted in asyncio compatibility mode. The life of worker threads is now bound to the the host
-  task of the topmost cancel scope hierarchy starting from the current one, or if no cancel scope
-  is active, the current task.
+- Fixed ``to_thread.run_sync()`` raising ``RuntimeError`` on asyncio when no "root" task
+  could be found for setting up a cleanup callback. This was a problem at least on
+  Tornado and possibly also Twisted in asyncio compatibility mode. The life of worker
+  threads is now bound to the the host task of the topmost cancel scope hierarchy
+  starting from the current one, or if no cancel scope is active, the current task.
 
 **3.0.0**
 
 - Curio support has been dropped (see the :doc:`FAQ <faq>` as for why)
 - API changes:
 
-  * **BACKWARDS INCOMPATIBLE** Submodules under ``anyio.abc.`` have been made private (use only
-    ``anyio.abc`` from now on).
-  * **BACKWARDS INCOMPATIBLE** The following method was previously a coroutine method and has been
-    converted into a synchronous one:
+  * **BACKWARDS INCOMPATIBLE** Submodules under ``anyio.abc.`` have been made private
+    (use only ``anyio.abc`` from now on).
+  * **BACKWARDS INCOMPATIBLE** The following method was previously a coroutine method
+    and has been converted into a synchronous one:
 
     * ``MemoryObjectReceiveStream.receive_nowait()``
 
-  * The following functions and methods are no longer asynchronous but can still be awaited on
-    (doing so will emit a deprecation warning):
+  * The following functions and methods are no longer asynchronous but can still be
+    awaited on (doing so will emit a deprecation warning):
 
     * ``current_time()``
     * ``current_effective_deadline()``
     * ``get_current_task()``
     * ``get_running_tasks()``
     * ``CancelScope.cancel()``
     * ``CapacityLimiter.acquire_nowait()``
     * ``CapacityLimiter.acquire_on_behalf_of_nowait()``
     * ``Condition.release()``
     * ``Event.set()``
     * ``Lock.release()``
     * ``MemoryObjectSendStream.send_nowait()``
     * ``Semaphore.release()``
-  * The following functions now return synchronous context managers instead of asynchronous
-    context managers (and emit deprecation warnings if used as async context managers):
+  * The following functions now return synchronous context managers instead of
+    asynchronous context managers (and emit deprecation warnings if used as async
+    context managers):
 
     * ``fail_after()``
     * ``move_on_after()``
     * ``open_cancel_scope()`` (now just ``CancelScope()``; see below)
     * ``open_signal_receiver()``
 
-  * The following functions and methods have been renamed/moved (will now emit deprecation
-    warnings when you use them by their old names):
+  * The following functions and methods have been renamed/moved (will now emit
+    deprecation warnings when you use them by their old names):
 
     * ``create_blocking_portal()`` → ``anyio.from_thread.BlockingPortal()``
     * ``create_capacity_limiter()`` → ``anyio.CapacityLimiter()``
     * ``create_event()`` → ``anyio.Event()``
     * ``create_lock()`` → ``anyio.Lock()``
     * ``create_condition()`` → ``anyio.Condition()``
     * ``create_semaphore()`` → ``anyio.Semaphore()``
@@ -263,40 +339,42 @@
     * ``run_sync_in_worker_thread()`` → ``anyio.to_thread.run_sync()``
     * ``run_async_from_thread()`` → ``anyio.from_thread.run()``
     * ``run_sync_from_thread()`` → ``anyio.from_thread.run_sync()``
     * ``BlockingPortal.spawn_task`` → ``BlockingPortal.start_task_soon``
     * ``CapacityLimiter.set_total_tokens()`` → ``limiter.total_tokens = ...``
     * ``TaskGroup.spawn()`` → ``TaskGroup.start_soon()``
 
-  * **BACKWARDS INCOMPATIBLE** ``start_blocking_portal()`` must now be used as a context manager
-    (it no longer returns a BlockingPortal, but a context manager that yields one)
+  * **BACKWARDS INCOMPATIBLE** ``start_blocking_portal()`` must now be used as a context
+    manager (it no longer returns a BlockingPortal, but a context manager that yields
+    one)
   * **BACKWARDS INCOMPATIBLE** The ``BlockingPortal.stop_from_external_thread()`` method
     (use ``portal.call(portal.stop)`` instead now)
-  * **BACKWARDS INCOMPATIBLE** The ``SocketStream`` and ``SocketListener`` classes were made
-    non-generic
+  * **BACKWARDS INCOMPATIBLE** The ``SocketStream`` and ``SocketListener`` classes were
+    made non-generic
   * Made all non-frozen dataclasses hashable with ``eq=False``
   * Removed ``__slots__`` from ``BlockingPortal``
 
-  See the :doc:`migration documentation <migration>` for instructions on how to deal with these
-  changes.
+  See the :doc:`migration documentation <migration>` for instructions on how to deal
+  with these changes.
 - Improvements to running synchronous code:
 
   * Added the ``run_sync_from_thread()`` function
   * Added the ``run_sync_in_process()`` function for running code in worker processes
     (big thanks to Richard Sheridan for his help on this one!)
 - Improvements to sockets and streaming:
 
-  * Added the ``UNIXSocketStream`` class which is capable of sending and receiving file descriptors
+  * Added the ``UNIXSocketStream`` class which is capable of sending and receiving file
+    descriptors
   * Added the ``FileReadStream`` and ``FileWriteStream`` classes
-  * ``create_unix_listener()`` now removes any existing socket at the given path before proceeding
-    (instead of raising ``OSError: Address already in use``)
+  * ``create_unix_listener()`` now removes any existing socket at the given path before
+    proceeding (instead of raising ``OSError: Address already in use``)
 - Improvements to task groups and cancellation:
 
-  * Added the ``TaskGroup.start()`` method and a corresponding ``BlockingPortal.start_task()``
-    method
+  * Added the ``TaskGroup.start()`` method and a corresponding
+    ``BlockingPortal.start_task()`` method
   * Added the ``name`` argument to ``BlockingPortal.start_task_soon()``
     (renamed from ``BlockingPortal.spawn_task()``)
   * Changed ``CancelScope.deadline`` to be writable
   * Added the following functions in the ``anyio.lowlevel`` module:
 
     * ``checkpoint()``
     * ``checkpoint_if_cancelled()``
@@ -304,162 +382,173 @@
 - Improvements and changes to synchronization primitives:
 
   * Added the ``Lock.acquire_nowait()``, ``Condition.acquire_nowait()`` and
     ``Semaphore.acquire_nowait()`` methods
   * Added the ``statistics()`` method to ``Event``, ``Lock``, ``Condition``, ``Semaphore``,
     ``CapacityLimiter``, ``MemoryObjectReceiveStream`` and ``MemoryObjectSendStream``
   * ``Lock`` and ``Condition`` can now only be released by the task that acquired them.
-    This behavior is now consistent on all backends whereas previously only Trio enforced this.
+    This behavior is now consistent on all backends whereas previously only Trio
+    enforced this.
   * The ``CapacityLimiter.total_tokens`` property is now writable and
     ``CapacityLimiter.set_total_tokens()`` has been deprecated
   * Added the ``max_value`` property to ``Semaphore``
-- Asyncio specific improvements (big thanks to Thomas Grainger for his effort on most of these!):
+- Asyncio specific improvements (big thanks to Thomas Grainger for his effort on most of
+  these!):
 
-  * Cancel scopes are now properly enforced with native asyncio coroutine functions (without
-    any explicit AnyIO checkpoints)
-  * Changed the asyncio ``CancelScope`` to raise a ``RuntimeError`` if a cancel scope is being
-    exited before it was even entered
-  * Changed the asyncio test runner to capture unhandled exceptions from asynchronous callbacks and
-    unbound native tasks which are then raised after the test function (or async fixture setup or
-    teardown) completes
-  * Changed the asyncio ``TaskGroup.start_soon()`` (formerly ``spawn()``) method to call the target
-    function immediately before starting the task, for consistency across backends
-  * Changed the asyncio ``TaskGroup.start_soon()`` (formerly ``spawn()``) method to avoid the use
-    of a coroutine wrapper on Python 3.8+ and added a hint for hiding the wrapper in tracebacks on
-    earlier Pythons (supported by Pytest, Sentry etc.)
-  * Changed the default thread limiter on asyncio to use a ``RunVar`` so it is  scoped to the
-    current event loop, thus avoiding potential conflict among multiple running event loops
+  * Cancel scopes are now properly enforced with native asyncio coroutine functions
+    (without any explicit AnyIO checkpoints)
+  * Changed the asyncio ``CancelScope`` to raise a ``RuntimeError`` if a cancel scope is
+    being exited before it was even entered
+  * Changed the asyncio test runner to capture unhandled exceptions from asynchronous
+    callbacks and unbound native tasks which are then raised after the test function (or
+    async fixture setup or teardown) completes
+  * Changed the asyncio ``TaskGroup.start_soon()`` (formerly ``spawn()``) method to call
+    the target function immediately before starting the task, for consistency across
+    backends
+  * Changed the asyncio ``TaskGroup.start_soon()`` (formerly ``spawn()``) method to
+    avoid the use of a coroutine wrapper on Python 3.8+ and added a hint for hiding the
+    wrapper in tracebacks on earlier Pythons (supported by Pytest, Sentry etc.)
+  * Changed the default thread limiter on asyncio to use a ``RunVar`` so it is  scoped
+    to the current event loop, thus avoiding potential conflict among multiple running
+    event loops
   * Thread pooling is now used on asyncio with ``run_sync_in_worker_thread()``
-  * Fixed ``current_effective_deadline()`` raising ``KeyError`` on asyncio when no cancel scope is
-    active
+  * Fixed ``current_effective_deadline()`` raising ``KeyError`` on asyncio when no
+    cancel scope is active
 - Added the ``RunVar`` class for scoping variables to the running event loop
 
 **2.2.0**
 
 - Added the ``maybe_async()`` and ``maybe_async_cm()`` functions to facilitate forward
   compatibility with AnyIO 3
-- Fixed socket stream bug on asyncio where receiving a half-close from the peer would shut down the
-  entire connection
+- Fixed socket stream bug on asyncio where receiving a half-close from the peer would
+  shut down the entire connection
 - Fixed native task names not being set on asyncio on Python 3.8+
 - Fixed ``TLSStream.send_eof()`` raising ``ValueError`` instead of the expected
   ``NotImplementedError``
-- Fixed ``open_signal_receiver()`` on asyncio and curio hanging if the cancel scope was cancelled
-  before the function could run
+- Fixed ``open_signal_receiver()`` on asyncio and curio hanging if the cancel scope was
+  cancelled before the function could run
 - Fixed Trio test runner causing unwarranted test errors on ``BaseException``
   (PR by Matthias Urlichs)
 - Fixed formatted output of ``ExceptionGroup`` containing too many newlines
 
 **2.1.0**
 
-- Added the ``spawn_task()`` and ``wrap_async_context_manager()`` methods to ``BlockingPortal``
+- Added the ``spawn_task()`` and ``wrap_async_context_manager()`` methods to
+  ``BlockingPortal``
 - Added the ``handshake_timeout`` and ``error_handler`` parameters to ``TLSListener``
 - Fixed ``Event`` objects on the trio backend not inheriting from ``anyio.abc.Event``
-- Fixed ``run_sync_in_worker_thread()`` raising ``UnboundLocalError`` on asyncio when cancelled
-- Fixed ``send()`` on socket streams not raising any exception on asyncio, and an unwrapped
-  ``BrokenPipeError`` on trio and curio when the peer has disconnected
-- Fixed ``MemoryObjectSendStream.send()`` raising ``BrokenResourceError`` when the last receiver is
-  closed right after receiving the item
-- Fixed ``ValueError: Invalid file descriptor: -1`` when closing a ``SocketListener`` on asyncio
+- Fixed ``run_sync_in_worker_thread()`` raising ``UnboundLocalError`` on asyncio when
+  cancelled
+- Fixed ``send()`` on socket streams not raising any exception on asyncio, and an
+  unwrapped ``BrokenPipeError`` on trio and curio when the peer has disconnected
+- Fixed ``MemoryObjectSendStream.send()`` raising ``BrokenResourceError`` when the last
+  receiver is closed right after receiving the item
+- Fixed ``ValueError: Invalid file descriptor: -1`` when closing a ``SocketListener`` on
+  asyncio
 
 **2.0.2**
 
 - Fixed one more case of
-  ``AttributeError: 'async_generator_asend' object has no attribute 'cr_await'`` on asyncio
+  ``AttributeError: 'async_generator_asend' object has no attribute 'cr_await'`` on
+  asyncio
 
 **2.0.1**
 
 - Fixed broken ``MultiListener.extra()`` (PR by daa)
-- Fixed ``TLSStream`` returning an empty bytes object instead of raising ``EndOfStream`` when
-  trying to receive from the stream after a closing handshake
-- Fixed ``AttributeError`` when cancelling a task group's scope inside an async test fixture on
-  asyncio
-- Fixed ``wait_all_tasks_blocked()`` raising ``AttributeError`` on asyncio if a native task is
-  waiting on an async generator's ``asend()`` method
+- Fixed ``TLSStream`` returning an empty bytes object instead of raising ``EndOfStream``
+  when trying to receive from the stream after a closing handshake
+- Fixed ``AttributeError`` when cancelling a task group's scope inside an async test
+  fixture on asyncio
+- Fixed ``wait_all_tasks_blocked()`` raising ``AttributeError`` on asyncio if a native
+  task is waiting on an async generator's ``asend()`` method
 
 **2.0.0**
 
 - General new features:
 
   - Added support for subprocesses
-  - Added support for "blocking portals" which allow running functions in the event loop thread
-    from external threads
-  - Added the ``anyio.aclose_forcefully()`` function for closing asynchronous resources as quickly
-    as possible
+  - Added support for "blocking portals" which allow running functions in the event loop
+    thread from external threads
+  - Added the ``anyio.aclose_forcefully()`` function for closing asynchronous resources
+    as quickly as possible
 
 - General changes/fixes:
 
-  - **BACKWARDS INCOMPATIBLE** Some functions have been renamed or removed (see further below for
-    socket/fileio API changes):
+  - **BACKWARDS INCOMPATIBLE** Some functions have been renamed or removed (see further
+    below for socket/fileio API changes):
 
     - ``finalize()`` → (removed; use ``contextlib.aclosing()`` instead)
     - ``receive_signals()`` → ``open_signal_receiver()``
     - ``run_in_thread()`` → ``run_sync_in_worker_thread()``
     - ``current_default_thread_limiter()`` → ``current_default_worker_thread_limiter()``
     - ``ResourceBusyError`` → ``BusyResourceError``
   - **BACKWARDS INCOMPATIBLE** Exception classes were moved to the top level package
   - Dropped support for Python 3.5
   - Bumped minimum versions of trio and curio to v0.16 and v1.4, respectively
   - Changed the ``repr()`` of ``ExceptionGroup`` to match trio's ``MultiError``
 
 - Backend specific changes and fixes:
 
-  - ``asyncio``: Added support for ``ProactorEventLoop``. This allows asyncio applications to use
-    AnyIO on Windows even without using AnyIO as the entry point.
-  - ``asyncio``: The asyncio backend now uses ``asyncio.run()`` behind the scenes which properly
-    shuts down async generators and cancels any leftover native tasks
-  - ``curio``: Worked around the limitation where a task can only be cancelled twice (any
-    cancellations beyond that were ignored)
-  - ``asyncio`` + ``curio``: a cancellation check now calls ``sleep(0)``, allowing the scheduler to
-    switch to a different task
-  - ``asyncio`` + ``curio``: Host name resolution now uses `IDNA 2008`_ (with UTS 46 compatibility
-    mapping, just like trio)
-  - ``asyncio`` + ``curio``: Fixed a bug where a task group would abandon its subtasks if its own
-    cancel scope was cancelled while it was waiting for subtasks to finish
-  - ``asyncio`` + ``curio``: Fixed recursive tracebacks when a single exception from an inner task
-    group is reraised in an outer task group
+  - ``asyncio``: Added support for ``ProactorEventLoop``. This allows asyncio
+    applications to use AnyIO on Windows even without using AnyIO as the entry point.
+  - ``asyncio``: The asyncio backend now uses ``asyncio.run()`` behind the scenes which
+    properly shuts down async generators and cancels any leftover native tasks
+  - ``curio``: Worked around the limitation where a task can only be cancelled twice
+    (any cancellations beyond that were ignored)
+  - ``asyncio`` + ``curio``: a cancellation check now calls ``sleep(0)``, allowing the
+    scheduler to switch to a different task
+  - ``asyncio`` + ``curio``: Host name resolution now uses `IDNA 2008`_ (with UTS 46
+    compatibility mapping, just like trio)
+  - ``asyncio`` + ``curio``: Fixed a bug where a task group would abandon its subtasks
+    if its own cancel scope was cancelled while it was waiting for subtasks to finish
+  - ``asyncio`` + ``curio``: Fixed recursive tracebacks when a single exception from an
+    inner task group is reraised in an outer task group
 
 - Socket/stream changes:
 
-  - **BACKWARDS INCOMPATIBLE** The stream class structure was completely overhauled. There are now
-    separate abstract base classes for receive and send streams, byte streams and reliable and
-    unreliable object streams. Stream wrappers are much better supported by this new ABC structure
-    and a new "typed extra attribute" system that lets you query the wrapper chain for the
-    attributes you want via ``.extra(...)``.
+  - **BACKWARDS INCOMPATIBLE** The stream class structure was completely overhauled.
+    There are now separate abstract base classes for receive and send streams, byte
+    streams and reliable and unreliable object streams. Stream wrappers are much better
+    supported by this new ABC structure and a new "typed extra attribute" system that
+    lets you query the wrapper chain for the attributes you want via ``.extra(...)``.
   - **BACKWARDS INCOMPATIBLE** Socket server functionality has been refactored into a
     network-agnostic listener system
-  - **BACKWARDS INCOMPATIBLE** TLS functionality has been split off from ``SocketStream`` and can
-    now work over any bidirectional bytes-based stream – you can now establish a TLS encrypted
-    communications pathway over UNIX sockets or even memory object streams. The ``TLSRequired``
-    exception has also been removed as it is no longer necessary.
+  - **BACKWARDS INCOMPATIBLE** TLS functionality has been split off from
+    ``SocketStream`` and can now work over any bidirectional bytes-based stream – you
+    can now establish a TLS encrypted communications pathway over UNIX sockets or even
+    memory object streams. The ``TLSRequired`` exception has also been removed as it is
+    no longer necessary.
   - **BACKWARDS INCOMPATIBLE** Buffering functionality (``receive_until()`` and
-    ``receive_exactly()``) was split off from ``SocketStream`` into a stream wrapper class
-    (``anyio.streams.buffered.BufferedByteReceiveStream``)
-  - **BACKWARDS INCOMPATIBLE** IPv6 addresses are now reported as 2-tuples. If original 4-tuple
-    form contains a nonzero scope ID, it is appended to the address with ``%`` as the separator.
-  - **BACKWARDS INCOMPATIBLE** Byte streams (including socket streams) now raise ``EndOfStream``
-    instead of returning an empty bytes object when the stream has been closed from the other end
+    ``receive_exactly()``) was split off from ``SocketStream`` into a stream wrapper
+    class (``anyio.streams.buffered.BufferedByteReceiveStream``)
+  - **BACKWARDS INCOMPATIBLE** IPv6 addresses are now reported as 2-tuples. If original
+    4-tuple form contains a nonzero scope ID, it is appended to the address with ``%``
+    as the separator.
+  - **BACKWARDS INCOMPATIBLE** Byte streams (including socket streams) now raise
+    ``EndOfStream`` instead of returning an empty bytes object when the stream has been
+    closed from the other end
   - **BACKWARDS INCOMPATIBLE** The socket API has changes:
 
     - ``create_tcp_server()`` → ``create_tcp_listener()``
     - ``create_unix_server()`` → ``create_unix_listener()``
     - ``create_udp_socket()`` had some of its parameters changed:
 
       - ``interface`` → ``local_address``
       - ``port`` → ``local_port``
-      - ``reuse_address`` was replaced with ``reuse_port`` (and sets ``SO_REUSEPORT`` instead of
-        ``SO_REUSEADDR``)
+      - ``reuse_address`` was replaced with ``reuse_port`` (and sets ``SO_REUSEPORT``
+        instead of ``SO_REUSEADDR``)
     - ``connect_tcp()`` had some of its parameters changed:
 
       - ``address`` → ``remote_address``
       - ``port`` → ``remote_port``
       - ``bind_host`` → ``local_address``
       - ``bind_port`` → (removed)
       - ``autostart_tls`` → ``tls``
-      - ``tls_hostname`` (new parameter, when you want to match the certificate against against
-        something else than ``remote_address``)
+      - ``tls_hostname`` (new parameter, when you want to match the certificate against
+        against something else than ``remote_address``)
     - ``connect_tcp()`` now returns a ``TLSStream`` if TLS was enabled
     - ``notify_socket_closing()`` was removed, as it is no longer used by AnyIO
     - ``SocketStream`` has changes to its methods and attributes:
 
         - ``address`` → ``.extra(SocketAttribute.local_address)``
         - ``alpn_protocol`` → ``.extra(TLSAttribute.alpn_protocol)``
         - ``close()`` → ``aclose()``
@@ -483,158 +572,171 @@
     - ``UDPSocket`` has changes to its methods and attributes:
 
       - ``address`` → ``.extra(SocketAttribute.local_address)``
       - ``getsockopt()`` → ``.extra(SocketAttribute.raw_socket).getsockopt(...)``
       - ``port`` → ``.extra(SocketAttribute.local_port)``
       - ``receive()`` no longer takes a maximum bytes argument
       - ``receive_packets()`` → (removed; use ``async for`` on the UDP socket instead)
-      - ``send()`` → requires a tuple for destination now (address, port), for compatibility with
-        the new ``UnreliableObjectStream`` interface. The ``sendto()`` method works like the old
-        ``send()`` method.
+      - ``send()`` → requires a tuple for destination now (address, port), for
+        compatibility with the new ``UnreliableObjectStream`` interface. The
+        ``sendto()`` method works like the old ``send()`` method.
       - ``setsockopt()`` → ``.extra(SocketAttribute.raw_socket).setsockopt(...)``
-  - **BACKWARDS INCOMPATIBLE** Renamed the ``max_size`` parameter to ``max_bytes`` wherever it
-    occurred (this was inconsistently named ``max_bytes`` in some subclasses before)
+  - **BACKWARDS INCOMPATIBLE** Renamed the ``max_size`` parameter to ``max_bytes``
+    wherever it occurred (this was inconsistently named ``max_bytes`` in some subclasses
+    before)
   - Added memory object streams as a replacement for queues
   - Added stream wrappers for encoding/decoding unicode strings
-  - Support for the ``SO_REUSEPORT`` option (allows binding more than one socket to the same
-    address/port combination, as long as they all have this option set) has been added to TCP
-    listeners and UDP sockets
+  - Support for the ``SO_REUSEPORT`` option (allows binding more than one socket to the
+    same address/port combination, as long as they all have this option set) has been
+    added to TCP listeners and UDP sockets
   - The ``send_eof()`` method was added to all (bidirectional) streams
 
 - File I/O changes:
 
-  - **BACKWARDS INCOMPATIBLE** Asynchronous file I/O functionality now uses a common code base
-    (``anyio.AsyncFile``) instead of backend-native classes
-  - **BACKWARDS INCOMPATIBLE** The File I/O API has changes to its functions and methods:
+  - **BACKWARDS INCOMPATIBLE** Asynchronous file I/O functionality now uses a common
+    code base (``anyio.AsyncFile``) instead of backend-native classes
+  - **BACKWARDS INCOMPATIBLE** The File I/O API has changes to its functions and
+    methods:
 
     - ``aopen()`` → ``open_file()``
     - ``AsyncFileclose()`` → ``AsyncFileaclose()``
 
 - Task synchronization changes:
 
   - **BACKWARDS INCOMPATIBLE** Queues were replaced by memory object streams
-  - **BACKWARDS INCOMPATIBLE** Added the ``acquire()`` and ``release()`` methods to the ``Lock``,
-    ``Condition`` and ``Semaphore`` classes
-  - **BACKWARDS INCOMPATIBLE** Removed the ``Event.clear()`` method. You must now replace the event
-    object with a new one rather than clear the old one.
+  - **BACKWARDS INCOMPATIBLE** Added the ``acquire()`` and ``release()`` methods to the
+    ``Lock``, ``Condition`` and ``Semaphore`` classes
+  - **BACKWARDS INCOMPATIBLE** Removed the ``Event.clear()`` method. You must now
+    replace the event object with a new one rather than clear the old one.
   - Fixed ``Condition.wait()`` not working on asyncio and curio (PR by Matt Westcott)
 
 - Testing changes:
 
-  - **BACKWARDS INCOMPATIBLE** Removed the ``--anyio-backends`` command line option for the pytest
-    plugin. Use the ``-k`` option to do ad-hoc filtering, and the ``anyio_backend`` fixture to
-    control which backends you wish to run the tests by default.
-  - The pytest plugin was refactored to run the test and all its related async fixtures inside the
-    same event loop, making async fixtures much more useful
-  - Fixed Hypothesis support in the pytest plugin (it was not actually running the Hypothesis
-    tests at all)
+  - **BACKWARDS INCOMPATIBLE** Removed the ``--anyio-backends`` command line option for
+    the pytest plugin. Use the ``-k`` option to do ad-hoc filtering, and the
+    ``anyio_backend`` fixture to control which backends you wish to run the tests by
+    default.
+  - The pytest plugin was refactored to run the test and all its related async fixtures
+    inside the same event loop, making async fixtures much more useful
+  - Fixed Hypothesis support in the pytest plugin (it was not actually running the
+    Hypothesis tests at all)
 
 .. _IDNA 2008: https://tools.ietf.org/html/rfc5895
 
 **1.4.0**
 
-- Added async name resolution functions (``anyio.getaddrinfo()`` and ``anyio.getnameinfo()``)
+- Added async name resolution functions (``anyio.getaddrinfo()`` and
+  ``anyio.getnameinfo()``)
 - Added the ``family`` and ``reuse_address`` parameters to ``anyio.create_udp_socket()``
   (Enables multicast support; test contributed by Matthias Urlichs)
 - Fixed ``fail.after(0)`` not raising a timeout error on asyncio and curio
-- Fixed ``move_on_after()`` and ``fail_after()`` getting stuck on curio in some circumstances
+- Fixed ``move_on_after()`` and ``fail_after()`` getting stuck on curio in some
+  circumstances
 - Fixed socket operations not allowing timeouts to cancel the task
-- Fixed API documentation on ``Stream.receive_until()`` which claimed that the delimiter will be
-  included in the returned data when it really isn't
+- Fixed API documentation on ``Stream.receive_until()`` which claimed that the delimiter
+  will be included in the returned data when it really isn't
 - Harmonized the default task names across all backends
-- ``wait_all_tasks_blocked()`` no longer considers tasks waiting on ``sleep(0)`` to be blocked
-  on asyncio and curio
-- Fixed the type of the ``address`` parameter in ``UDPSocket.send()`` to include ``IPAddress``
-  objects (which were already supported by the backing implementation)
-- Fixed ``UDPSocket.send()`` to resolve host names using ``anyio.getaddrinfo()`` before calling
-  ``socket.sendto()`` to avoid blocking on synchronous name resolution
+- ``wait_all_tasks_blocked()`` no longer considers tasks waiting on ``sleep(0)`` to be
+  blocked on asyncio and curio
+- Fixed the type of the ``address`` parameter in ``UDPSocket.send()`` to include
+  ``IPAddress`` objects (which were already supported by the backing implementation)
+- Fixed ``UDPSocket.send()`` to resolve host names using ``anyio.getaddrinfo()`` before
+  calling ``socket.sendto()`` to avoid blocking on synchronous name resolution
 - Switched to using ``anyio.getaddrinfo()`` for name lookups
 
 **1.3.1**
 
 - Fixed warnings caused by trio 0.15
 - Worked around a compatibility issue between uvloop and Python 3.9 (missing
   ``shutdown_default_executor()`` method)
 
 **1.3.0**
 
 - Fixed compatibility with Curio 1.0
-- Made it possible to assert fine grained control over which AnyIO backends and backend options are
-  being used with each test
-- Added the ``address`` and ``peer_address`` properties to the ``SocketStream`` interface
+- Made it possible to assert fine grained control over which AnyIO backends and backend
+  options are being used with each test
+- Added the ``address`` and ``peer_address`` properties to the ``SocketStream``
+  interface
 
 **1.2.3**
 
 - Repackaged release (v1.2.2 contained extra files from an experimental
   branch which broke imports)
 
 **1.2.2**
 
-- Fixed ``CancelledError`` leaking from a cancel scope on asyncio if the task previously received a
-  cancellation exception
+- Fixed ``CancelledError`` leaking from a cancel scope on asyncio if the task previously
+  received a cancellation exception
 - Fixed ``AttributeError`` when cancelling a generator-based task (asyncio)
 - Fixed ``wait_all_tasks_blocked()`` not working with generator-based tasks (asyncio)
 - Fixed an unnecessary delay in ``connect_tcp()`` if an earlier attempt succeeds
 - Fixed ``AssertionError`` in ``connect_tcp()`` if multiple connection attempts succeed
   simultaneously
 
 **1.2.1**
 
-- Fixed cancellation errors leaking from a task group when they are contained in an exception group
+- Fixed cancellation errors leaking from a task group when they are contained in an
+  exception group
 - Fixed trio v0.13 compatibility on Windows
 - Fixed inconsistent queue capacity across backends when capacity was defined as 0
   (trio = 0, others = infinite)
 - Fixed socket creation failure crashing ``connect_tcp()``
 
 **1.2.0**
 
-- Added the possibility to parametrize regular pytest test functions against the selected list of
-  backends
+- Added the possibility to parametrize regular pytest test functions against the
+  selected list of backends
 - Added the ``set_total_tokens()`` method to ``CapacityLimiter``
 - Added the ``anyio.current_default_thread_limiter()`` function
 - Added the ``cancellable`` parameter to ``anyio.run_in_thread()``
 - Implemented the Happy Eyeballs (:rfc:`6555`) algorithm for ``anyio.connect_tcp()``
-- Fixed ``KeyError`` on asyncio and curio where entering and exiting a cancel scope happens in
-  different tasks
-- Fixed deprecation warnings on Python 3.8 about the ``loop`` argument of ``asyncio.Event()``
-- Forced the use ``WindowsSelectorEventLoopPolicy`` in ``asyncio.run`` when on Windows and asyncio
+- Fixed ``KeyError`` on asyncio and curio where entering and exiting a cancel scope
+  happens in different tasks
+- Fixed deprecation warnings on Python 3.8 about the ``loop`` argument of
+  ``asyncio.Event()``
+- Forced the use ``WindowsSelectorEventLoopPolicy`` in ``asyncio.run`` when on Windows
+  and asyncio
   to keep network functionality working
 - Worker threads are now spawned with ``daemon=True`` on all backends, not just trio
 - Dropped support for trio v0.11
 
 **1.1.0**
 
 - Added the ``lock`` parameter to ``anyio.create_condition()`` (PR by Matthias Urlichs)
 - Added async iteration for queues (PR by Matthias Urlichs)
 - Added capacity limiters
-- Added the possibility of using capacity limiters for limiting the maximum number of threads
+- Added the possibility of using capacity limiters for limiting the maximum number of
+  threads
 - Fixed compatibility with trio v0.12
-- Fixed IPv6 support in ``create_tcp_server()``, ``connect_tcp()`` and ``create_udp_socket()``
-- Fixed mishandling of task cancellation while the task is running a worker thread on asyncio and
-  curio
+- Fixed IPv6 support in ``create_tcp_server()``, ``connect_tcp()`` and
+  ``create_udp_socket()``
+- Fixed mishandling of task cancellation while the task is running a worker thread on
+  asyncio and curio
 
 **1.0.0**
 
 - Fixed pathlib2_ compatibility with ``anyio.aopen()``
-- Fixed timeouts not propagating from nested scopes on asyncio and curio (PR by Matthias Urlichs)
-- Fixed incorrect call order in socket close notifications on asyncio (mostly affecting Windows)
+- Fixed timeouts not propagating from nested scopes on asyncio and curio (PR by Matthias
+  Urlichs)
+- Fixed incorrect call order in socket close notifications on asyncio (mostly affecting
+  Windows)
 - Prefixed backend module names with an underscore to better indicate privateness
 
  .. _pathlib2: https://pypi.org/project/pathlib2/
 
 **1.0.0rc2**
 
-- Fixed some corner cases of cancellation where behavior on asyncio and curio did not match with
-  that of trio. Thanks to Joshua Oreman for help with this.
-- Fixed ``current_effective_deadline()`` not taking shielded cancellation scopes into account on
-  asyncio and curio
-- Fixed task cancellation not happening right away on asyncio and curio when a cancel scope is
-  entered when the deadline has already passed
-- Fixed exception group containing only cancellation exceptions not being swallowed by a timed out
-  cancel scope on asyncio and curio
+- Fixed some corner cases of cancellation where behavior on asyncio and curio did not
+  match with that of trio. Thanks to Joshua Oreman for help with this.
+- Fixed ``current_effective_deadline()`` not taking shielded cancellation scopes into
+  account on asyncio and curio
+- Fixed task cancellation not happening right away on asyncio and curio when a cancel
+  scope is entered when the deadline has already passed
+- Fixed exception group containing only cancellation exceptions not being swallowed by a
+  timed out cancel scope on asyncio and curio
 - Added the ``current_time()`` function
 - Replaced ``CancelledError`` with ``get_cancelled_exc_class()``
 - Added support for Hypothesis_
 - Added support for :pep:`561`
 - Use uvloop for the asyncio backend by default when available (but only on CPython)
 
 .. _Hypothesis: https://hypothesis.works/
@@ -642,15 +744,16 @@
 **1.0.0rc1**
 
 - Fixed ``setsockopt()`` passing options to the underlying method in the wrong manner
 - Fixed cancellation propagation from nested task groups
 - Fixed ``get_running_tasks()`` returning tasks from other event loops
 - Added the ``parent_id`` attribute to ``anyio.TaskInfo``
 - Added the ``get_current_task()`` function
-- Added guards to protect against concurrent read/write from/to sockets by multiple tasks
+- Added guards to protect against concurrent read/write from/to sockets by multiple
+  tasks
 - Added the ``notify_socket_close()`` function
 
 **1.0.0b2**
 
 - Added introspection of running tasks via ``anyio.get_running_tasks()``
 - Added the ``getsockopt()`` and ``setsockopt()`` methods to the ``SocketStream`` API
 - Fixed mishandling of large buffers by ``BaseSocket.sendall()``
```

### Comparing `anyio-3.7.1/pyproject.toml` & `anyio-4.0.0rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,93 +15,88 @@
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Framework :: AnyIO",
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
-requires-python = ">= 3.7"
+requires-python = ">= 3.8"
 dependencies = [
-    "exceptiongroup; python_version < '3.11'",
+    "exceptiongroup >= 1.0.2; python_version < '3.11'",
     "idna >= 2.8",
     "sniffio >= 1.1",
-    "typing_extensions; python_version < '3.8'",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://anyio.readthedocs.io/en/latest/"
 Changelog = "https://anyio.readthedocs.io/en/stable/versionhistory.html"
 "Source code" = "https://github.com/agronholm/anyio"
 "Issue tracker" = "https://github.com/agronholm/anyio/issues"
 
 [project.optional-dependencies]
-trio = ["trio < 0.22"]
+trio = ["trio >= 0.22"]
 test = [
     "anyio[trio]",
-    "mock >= 4; python_version < '3.8'",
     "coverage[toml] >= 4.5",
     "hypothesis >= 4.0",
     "psutil >= 5.9",
     "pytest >= 7.0",
     "pytest-mock >= 3.6.1",
     "trustme",
     "uvloop >= 0.17; python_version < '3.12' and platform_python_implementation == 'CPython' and platform_system != 'Windows'",
 ]
 doc = [
     "packaging",
-    "Sphinx",
-    "sphinx-rtd-theme >= 1.2.2",
+    "Sphinx ~= 6.1.0",
+    "sphinx_rtd_theme",
     "sphinxcontrib-jquery",
     "sphinx-autodoc-typehints >= 1.2.0",
 ]
 
 [project.entry-points]
 pytest11 = {anyio = "anyio.pytest_plugin"}
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
 local_scheme = "dirty-tag"
 
 [tool.ruff]
-line-length = 99
+line-length = 88
 select = [
     "E", "F", "W",  # default flake-8
     "I",            # isort
     "PGH",          # pygrep-hooks
     "UP",           # pyupgrade
 ]
-ignore = [
-    "UP026",  # deprecated-mock-import (needed on py3.7)
-]
-target-version = "py37"
 src = ["src"]
 
 [tool.ruff.isort]
 "required-imports" = ["from __future__ import annotations"]
 
 [tool.mypy]
-python_version = "3.11"
+python_version = "3.12"
 strict = true
 ignore_missing_imports = true
 disallow_any_generics = false
 warn_return_any = false
 disallow_untyped_decorators = false
 disallow_subclassing_any = false
 show_error_codes = true
 
 [tool.pytest.ini_options]
 addopts = "-rsx --tb=short --strict-config --strict-markers -p anyio -p no:asyncio -p no:trio"
 testpaths = ["tests"]
+xfail_strict = true
 # Ignore resource warnings due to a CPython/Windows bug (https://bugs.python.org/issue44428)
 filterwarnings = [
     "error",
     "ignore:unclosed <socket.socket.*:ResourceWarning",
     "ignore:unclosed transport <_ProactorSocketTransport.*:ResourceWarning",
     "ignore:ast.Str is deprecated:DeprecationWarning",
     "ignore:Attribute s is deprecated:DeprecationWarning",
@@ -119,17 +114,17 @@
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = pre-commit, py37, py38, py39, py310, py311, pypy3
+envlist = pre-commit, py38, py39, py310, py311, py312, pypy3
 skip_missing_interpreters = true
-minversion = 4.4.3
+minversion = 4.0.0
 
 [testenv]
 depends = pre-commit
 package = editable
 commands = coverage run -m pytest {posargs}
 extras = test
```

### Comparing `anyio-3.7.1/src/anyio/_backends/_asyncio.py` & `anyio-4.0.0rc1/src/anyio/_backends/_asyncio.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,113 +2,294 @@
 
 import array
 import asyncio
 import concurrent.futures
 import math
 import socket
 import sys
+import threading
+from asyncio import (
+    AbstractEventLoop,
+    CancelledError,
+    all_tasks,
+    create_task,
+    current_task,
+    get_running_loop,
+    sleep,
+)
+from asyncio import run as native_run
 from asyncio.base_events import _run_until_complete_cb  # type: ignore[attr-defined]
 from collections import OrderedDict, deque
+from collections.abc import AsyncIterator, Iterable
 from concurrent.futures import Future
+from contextlib import suppress
 from contextvars import Context, copy_context
 from dataclasses import dataclass
 from functools import partial, wraps
 from inspect import (
     CORO_RUNNING,
     CORO_SUSPENDED,
-    GEN_RUNNING,
-    GEN_SUSPENDED,
     getcoroutinestate,
-    getgeneratorstate,
+    iscoroutine,
 )
 from io import IOBase
 from os import PathLike
 from queue import Queue
+from signal import Signals
 from socket import AddressFamily, SocketKind
 from threading import Thread
 from types import TracebackType
 from typing import (
     IO,
     Any,
     AsyncGenerator,
     Awaitable,
     Callable,
     Collection,
+    ContextManager,
     Coroutine,
-    Generator,
-    Iterable,
     Mapping,
     Optional,
     Sequence,
     Tuple,
     TypeVar,
-    Union,
     cast,
 )
 from weakref import WeakKeyDictionary
 
 import sniffio
 
 from .. import CapacityLimiterStatistics, EventStatistics, TaskInfo, abc
-from .._core._compat import DeprecatedAsyncContextManager, DeprecatedAwaitable
-from .._core._eventloop import claim_worker_thread, threadlocals
+from .._core._eventloop import claim_worker_thread
 from .._core._exceptions import (
     BrokenResourceError,
     BusyResourceError,
     ClosedResourceError,
     EndOfStream,
     WouldBlock,
 )
-from .._core._exceptions import ExceptionGroup as BaseExceptionGroup
-from .._core._sockets import GetAddrInfoReturnType, convert_ipv6_sockaddr
+from .._core._sockets import convert_ipv6_sockaddr
+from .._core._streams import create_memory_object_stream
 from .._core._synchronization import CapacityLimiter as BaseCapacityLimiter
 from .._core._synchronization import Event as BaseEvent
 from .._core._synchronization import ResourceGuard
 from .._core._tasks import CancelScope as BaseCancelScope
-from ..abc import IPSockAddrType, UDPPacketType
+from ..abc import (
+    AsyncBackend,
+    IPSockAddrType,
+    SocketListener,
+    UDPPacketType,
+    UNIXDatagramPacketType,
+)
 from ..lowlevel import RunVar
+from ..streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
+
+if sys.version_info >= (3, 11):
+    from asyncio import Runner
+else:
+    import contextvars
+    import enum
+    import signal
+    from asyncio import coroutines, events, exceptions, tasks
+
+    from exceptiongroup import BaseExceptionGroup
+
+    class _State(enum.Enum):
+        CREATED = "created"
+        INITIALIZED = "initialized"
+        CLOSED = "closed"
+
+    class Runner:
+        # Copied from CPython 3.11
+        def __init__(
+            self,
+            *,
+            debug: bool | None = None,
+            loop_factory: Callable[[], AbstractEventLoop] | None = None,
+        ):
+            self._state = _State.CREATED
+            self._debug = debug
+            self._loop_factory = loop_factory
+            self._loop: AbstractEventLoop | None = None
+            self._context = None
+            self._interrupt_count = 0
+            self._set_event_loop = False
+
+        def __enter__(self) -> Runner:
+            self._lazy_init()
+            return self
+
+        def __exit__(
+            self,
+            exc_type: type[BaseException],
+            exc_val: BaseException,
+            exc_tb: TracebackType,
+        ) -> None:
+            self.close()
+
+        def close(self) -> None:
+            """Shutdown and close event loop."""
+            if self._state is not _State.INITIALIZED:
+                return
+            try:
+                loop = self._loop
+                _cancel_all_tasks(loop)
+                loop.run_until_complete(loop.shutdown_asyncgens())
+                if hasattr(loop, "shutdown_default_executor"):
+                    loop.run_until_complete(loop.shutdown_default_executor())
+                else:
+                    loop.run_until_complete(_shutdown_default_executor(loop))
+            finally:
+                if self._set_event_loop:
+                    events.set_event_loop(None)
+                loop.close()
+                self._loop = None
+                self._state = _State.CLOSED
+
+        def get_loop(self) -> AbstractEventLoop:
+            """Return embedded event loop."""
+            self._lazy_init()
+            return self._loop
+
+        def run(self, coro: Coroutine[T_Retval], *, context=None) -> T_Retval:
+            """Run a coroutine inside the embedded event loop."""
+            if not coroutines.iscoroutine(coro):
+                raise ValueError(f"a coroutine was expected, got {coro!r}")
 
-if sys.version_info >= (3, 8):
+            if events._get_running_loop() is not None:
+                # fail fast with short traceback
+                raise RuntimeError(
+                    "Runner.run() cannot be called from a running event loop"
+                )
 
-    def get_coro(task: asyncio.Task) -> Generator | Awaitable[Any]:
-        return task.get_coro()
+            self._lazy_init()
 
-else:
+            if context is None:
+                context = self._context
+            task = self._loop.create_task(coro, context=context)
 
-    def get_coro(task: asyncio.Task) -> Generator | Awaitable[Any]:
-        return task._coro
+            if (
+                threading.current_thread() is threading.main_thread()
+                and signal.getsignal(signal.SIGINT) is signal.default_int_handler
+            ):
+                sigint_handler = partial(self._on_sigint, main_task=task)
+                try:
+                    signal.signal(signal.SIGINT, sigint_handler)
+                except ValueError:
+                    # `signal.signal` may throw if `threading.main_thread` does
+                    # not support signals (e.g. embedded interpreter with signals
+                    # not registered - see gh-91880)
+                    sigint_handler = None
+            else:
+                sigint_handler = None
 
+            self._interrupt_count = 0
+            try:
+                return self._loop.run_until_complete(task)
+            except exceptions.CancelledError:
+                if self._interrupt_count > 0:
+                    uncancel = getattr(task, "uncancel", None)
+                    if uncancel is not None and uncancel() == 0:
+                        raise KeyboardInterrupt()
+                raise  # CancelledError
+            finally:
+                if (
+                    sigint_handler is not None
+                    and signal.getsignal(signal.SIGINT) is sigint_handler
+                ):
+                    signal.signal(signal.SIGINT, signal.default_int_handler)
 
-from asyncio import all_tasks, create_task, current_task, get_running_loop
-from asyncio import run as native_run
+        def _lazy_init(self) -> None:
+            if self._state is _State.CLOSED:
+                raise RuntimeError("Runner is closed")
+            if self._state is _State.INITIALIZED:
+                return
+            if self._loop_factory is None:
+                self._loop = events.new_event_loop()
+                if not self._set_event_loop:
+                    # Call set_event_loop only once to avoid calling
+                    # attach_loop multiple times on child watchers
+                    events.set_event_loop(self._loop)
+                    self._set_event_loop = True
+            else:
+                self._loop = self._loop_factory()
+            if self._debug is not None:
+                self._loop.set_debug(self._debug)
+            self._context = contextvars.copy_context()
+            self._state = _State.INITIALIZED
+
+        def _on_sigint(self, signum, frame, main_task: asyncio.Task) -> None:
+            self._interrupt_count += 1
+            if self._interrupt_count == 1 and not main_task.done():
+                main_task.cancel()
+                # wakeup loop if it is blocked by select() with long timeout
+                self._loop.call_soon_threadsafe(lambda: None)
+                return
+            raise KeyboardInterrupt()
 
+    def _cancel_all_tasks(loop: AbstractEventLoop) -> None:
+        to_cancel = tasks.all_tasks(loop)
+        if not to_cancel:
+            return
 
-def _get_task_callbacks(task: asyncio.Task) -> Iterable[Callable]:
-    return [cb for cb, context in task._callbacks]
+        for task in to_cancel:
+            task.cancel()
 
+        loop.run_until_complete(tasks.gather(*to_cancel, return_exceptions=True))
 
-T_Retval = TypeVar("T_Retval")
-T_contra = TypeVar("T_contra", contravariant=True)
+        for task in to_cancel:
+            if task.cancelled():
+                continue
+            if task.exception() is not None:
+                loop.call_exception_handler(
+                    {
+                        "message": "unhandled exception during asyncio.run() shutdown",
+                        "exception": task.exception(),
+                        "task": task,
+                    }
+                )
+
+    async def _shutdown_default_executor(loop: AbstractEventLoop) -> None:
+        """Schedule the shutdown of the default executor."""
+
+        def _do_shutdown(future: asyncio.futures.Future) -> None:
+            try:
+                loop._default_executor.shutdown(wait=True)  # type: ignore[attr-defined]
+                loop.call_soon_threadsafe(future.set_result, None)
+            except Exception as ex:
+                loop.call_soon_threadsafe(future.set_exception, ex)
 
-# Check whether there is native support for task names in asyncio (3.8+)
-_native_task_names = hasattr(asyncio.Task, "get_name")
+        loop._executor_shutdown_called = True
+        if loop._default_executor is None:
+            return
+        future = loop.create_future()
+        thread = threading.Thread(target=_do_shutdown, args=(future,))
+        thread.start()
+        try:
+            await future
+        finally:
+            thread.join()
 
 
+T_Retval = TypeVar("T_Retval")
+T_contra = TypeVar("T_contra", contravariant=True)
+
 _root_task: RunVar[asyncio.Task | None] = RunVar("_root_task")
 
 
 def find_root_task() -> asyncio.Task:
     root_task = _root_task.get(None)
     if root_task is not None and not root_task.done():
         return root_task
 
     # Look for a task that has been started via run_until_complete()
     for task in all_tasks():
         if task._callbacks and not task.done():
-            for cb in _get_task_callbacks(task):
+            callbacks = [cb for cb, context in task._callbacks]
+            for cb in callbacks:
                 if (
                     cb is _run_until_complete_cb
                     or getattr(cb, "__module__", None) == "uvloop.loop"
                 ):
                     _root_task.set(task)
                     return task
 
@@ -136,124 +317,60 @@
 # Event loop
 #
 
 _run_vars = (
     WeakKeyDictionary()
 )  # type: WeakKeyDictionary[asyncio.AbstractEventLoop, Any]
 
-current_token = get_running_loop
-
 
 def _task_started(task: asyncio.Task) -> bool:
     """Return ``True`` if the task has been started and has not finished."""
-    coro = cast(Coroutine[Any, Any, Any], get_coro(task))
     try:
-        return getcoroutinestate(coro) in (CORO_RUNNING, CORO_SUSPENDED)
+        return getcoroutinestate(task.get_coro()) in (CORO_RUNNING, CORO_SUSPENDED)
     except AttributeError:
-        try:
-            return getgeneratorstate(cast(Generator, coro)) in (
-                GEN_RUNNING,
-                GEN_SUSPENDED,
-            )
-        except AttributeError:
-            # task coro is async_genenerator_asend https://bugs.python.org/issue37771
-            raise Exception(f"Cannot determine if task {task} has started or not")
-
-
-def _maybe_set_event_loop_policy(
-    policy: asyncio.AbstractEventLoopPolicy | None, use_uvloop: bool
-) -> None:
-    # On CPython, use uvloop when possible if no other policy has been given and if not
-    # explicitly disabled
-    if policy is None and use_uvloop and sys.implementation.name == "cpython":
-        try:
-            import uvloop
-        except ImportError:
-            pass
-        else:
-            # Test for missing shutdown_default_executor() (uvloop 0.14.0 and earlier)
-            if not hasattr(
-                asyncio.AbstractEventLoop, "shutdown_default_executor"
-            ) or hasattr(uvloop.loop.Loop, "shutdown_default_executor"):
-                policy = uvloop.EventLoopPolicy()
-
-    if policy is not None:
-        asyncio.set_event_loop_policy(policy)
-
-
-def run(
-    func: Callable[..., Awaitable[T_Retval]],
-    *args: object,
-    debug: bool = False,
-    use_uvloop: bool = False,
-    policy: asyncio.AbstractEventLoopPolicy | None = None,
-) -> T_Retval:
-    @wraps(func)
-    async def wrapper() -> T_Retval:
-        task = cast(asyncio.Task, current_task())
-        task_state = TaskState(None, get_callable_name(func), None)
-        _task_states[task] = task_state
-        if _native_task_names:
-            task.set_name(task_state.name)
-
-        try:
-            return await func(*args)
-        finally:
-            del _task_states[task]
-
-    _maybe_set_event_loop_policy(policy, use_uvloop)
-    return native_run(wrapper(), debug=debug)
-
-
-#
-# Miscellaneous
-#
-
-sleep = asyncio.sleep
+        # task coro is async_genenerator_asend https://bugs.python.org/issue37771
+        raise Exception(f"Cannot determine if task {task} has started or not") from None
 
 
 #
 # Timeouts and cancellation
 #
 
-CancelledError = asyncio.CancelledError
-
 
 class CancelScope(BaseCancelScope):
     def __new__(
         cls, *, deadline: float = math.inf, shield: bool = False
     ) -> CancelScope:
         return object.__new__(cls)
 
     def __init__(self, deadline: float = math.inf, shield: bool = False):
         self._deadline = deadline
         self._shield = shield
         self._parent_scope: CancelScope | None = None
         self._cancel_called = False
+        self._cancelled_caught = False
         self._active = False
         self._timeout_handle: asyncio.TimerHandle | None = None
         self._cancel_handle: asyncio.Handle | None = None
         self._tasks: set[asyncio.Task] = set()
         self._host_task: asyncio.Task | None = None
-        self._timeout_expired = False
         self._cancel_calls: int = 0
 
     def __enter__(self) -> CancelScope:
         if self._active:
             raise RuntimeError(
                 "Each CancelScope may only be used for a single 'with' block"
             )
 
         self._host_task = host_task = cast(asyncio.Task, current_task())
         self._tasks.add(host_task)
         try:
             task_state = _task_states[host_task]
         except KeyError:
-            task_name = host_task.get_name() if _native_task_names else None
-            task_state = TaskState(None, task_name, self)
+            task_state = TaskState(None, self)
             _task_states[host_task] = task_state
         else:
             self._parent_scope = task_state.cancel_scope
             task_state.cancel_scope = self
 
         self._timeout()
         self._active = True
@@ -291,83 +408,79 @@
             self._timeout_handle.cancel()
             self._timeout_handle = None
 
         self._tasks.remove(self._host_task)
 
         host_task_state.cancel_scope = self._parent_scope
 
-        # Restart the cancellation effort in the farthest directly cancelled parent scope if this
-        # one was shielded
+        # Restart the cancellation effort in the farthest directly cancelled parent
+        # scope if this one was shielded
         if self._shield:
             self._deliver_cancellation_to_parent()
 
-        if exc_val is not None:
-            exceptions = (
-                exc_val.exceptions if isinstance(exc_val, ExceptionGroup) else [exc_val]
-            )
-            if all(isinstance(exc, CancelledError) for exc in exceptions):
-                if self._timeout_expired:
-                    return self._uncancel()
-                elif not self._cancel_called:
-                    # Task was cancelled natively
-                    return None
-                elif not self._parent_cancelled():
-                    # This scope was directly cancelled
-                    return self._uncancel()
+        if isinstance(exc_val, CancelledError) and self._cancel_called:
+            self._cancelled_caught = self._uncancel(exc_val)
+            return self._cancelled_caught
 
         return None
 
-    def _uncancel(self) -> bool:
-        if sys.version_info < (3, 11) or self._host_task is None:
+    def _uncancel(self, cancelled_exc: CancelledError) -> bool:
+        if sys.version_info < (3, 9) or self._host_task is None:
             self._cancel_calls = 0
             return True
 
         # Uncancel all AnyIO cancellations
-        for i in range(self._cancel_calls):
-            self._host_task.uncancel()
+        if sys.version_info >= (3, 11):
+            for i in range(self._cancel_calls):
+                self._host_task.uncancel()
 
         self._cancel_calls = 0
-        return not self._host_task.cancelling()
+        return f"Cancelled by cancel scope {id(self):x}" in cancelled_exc.args
 
     def _timeout(self) -> None:
         if self._deadline != math.inf:
             loop = get_running_loop()
             if loop.time() >= self._deadline:
-                self._timeout_expired = True
                 self.cancel()
             else:
                 self._timeout_handle = loop.call_at(self._deadline, self._timeout)
 
     def _deliver_cancellation(self) -> None:
         """
         Deliver cancellation to directly contained tasks and nested cancel scopes.
 
-        Schedule another run at the end if we still have tasks eligible for cancellation.
+        Schedule another run at the end if we still have tasks eligible for
+        cancellation.
         """
         should_retry = False
         current = current_task()
         for task in self._tasks:
             if task._must_cancel:  # type: ignore[attr-defined]
                 continue
 
-            # The task is eligible for cancellation if it has started and is not in a cancel
-            # scope shielded from this one
+            # The task is eligible for cancellation if it has started and is not in a
+            # cancel scope shielded from this one
             cancel_scope = _task_states[task].cancel_scope
             while cancel_scope is not self:
                 if cancel_scope is None or cancel_scope._shield:
                     break
                 else:
                     cancel_scope = cancel_scope._parent_scope
             else:
                 should_retry = True
                 if task is not current and (
                     task is self._host_task or _task_started(task)
                 ):
-                    self._cancel_calls += 1
-                    task.cancel()
+                    waiter = task._fut_waiter  # type: ignore[attr-defined]
+                    if not isinstance(waiter, asyncio.Future) or not waiter.done():
+                        self._cancel_calls += 1
+                        if sys.version_info >= (3, 9):
+                            task.cancel(f"Cancelled by cancel scope {id(self):x}")
+                        else:
+                            task.cancel()
 
         # Schedule another callback if there are still tasks left
         if should_retry:
             self._cancel_handle = get_running_loop().call_soon(
                 self._deliver_cancellation
             )
         else:
@@ -397,26 +510,24 @@
             if cancel_scope._cancel_called:
                 return True
             else:
                 cancel_scope = cancel_scope._parent_scope
 
         return False
 
-    def cancel(self) -> DeprecatedAwaitable:
+    def cancel(self) -> None:
         if not self._cancel_called:
             if self._timeout_handle:
                 self._timeout_handle.cancel()
                 self._timeout_handle = None
 
             self._cancel_called = True
             if self._host_task is not None:
                 self._deliver_cancellation()
 
-        return DeprecatedAwaitable(self.cancel)
-
     @property
     def deadline(self) -> float:
         return self._deadline
 
     @deadline.setter
     def deadline(self, value: float) -> None:
         self._deadline = float(value)
@@ -428,115 +539,55 @@
             self._timeout()
 
     @property
     def cancel_called(self) -> bool:
         return self._cancel_called
 
     @property
+    def cancelled_caught(self) -> bool:
+        return self._cancelled_caught
+
+    @property
     def shield(self) -> bool:
         return self._shield
 
     @shield.setter
     def shield(self, value: bool) -> None:
         if self._shield != value:
             self._shield = value
             if not value:
                 self._deliver_cancellation_to_parent()
 
 
-async def checkpoint() -> None:
-    await sleep(0)
-
-
-async def checkpoint_if_cancelled() -> None:
-    task = current_task()
-    if task is None:
-        return
-
-    try:
-        cancel_scope = _task_states[task].cancel_scope
-    except KeyError:
-        return
-
-    while cancel_scope:
-        if cancel_scope.cancel_called:
-            await sleep(0)
-        elif cancel_scope.shield:
-            break
-        else:
-            cancel_scope = cancel_scope._parent_scope
-
-
-async def cancel_shielded_checkpoint() -> None:
-    with CancelScope(shield=True):
-        await sleep(0)
-
-
-def current_effective_deadline() -> float:
-    try:
-        cancel_scope = _task_states[current_task()].cancel_scope  # type: ignore[index]
-    except KeyError:
-        return math.inf
-
-    deadline = math.inf
-    while cancel_scope:
-        deadline = min(deadline, cancel_scope.deadline)
-        if cancel_scope._cancel_called:
-            deadline = -math.inf
-            break
-        elif cancel_scope.shield:
-            break
-        else:
-            cancel_scope = cancel_scope._parent_scope
-
-    return deadline
-
-
-def current_time() -> float:
-    return get_running_loop().time()
-
-
 #
 # Task states
 #
 
 
 class TaskState:
     """
-    Encapsulates auxiliary task information that cannot be added to the Task instance itself
-    because there are no guarantees about its implementation.
+    Encapsulates auxiliary task information that cannot be added to the Task instance
+    itself because there are no guarantees about its implementation.
     """
 
-    __slots__ = "parent_id", "name", "cancel_scope"
+    __slots__ = "parent_id", "cancel_scope"
 
-    def __init__(
-        self,
-        parent_id: int | None,
-        name: str | None,
-        cancel_scope: CancelScope | None,
-    ):
+    def __init__(self, parent_id: int | None, cancel_scope: CancelScope | None):
         self.parent_id = parent_id
-        self.name = name
         self.cancel_scope = cancel_scope
 
 
 _task_states = WeakKeyDictionary()  # type: WeakKeyDictionary[asyncio.Task, TaskState]
 
 
 #
 # Task groups
 #
 
 
-class ExceptionGroup(BaseExceptionGroup):
-    def __init__(self, exceptions: list[BaseException]):
-        super().__init__()
-        self.exceptions = exceptions
-
-
 class _AsyncioTaskStatus(abc.TaskStatus):
     def __init__(self, future: asyncio.Future, parent_id: int):
         self._future = future
         self._parent_id = parent_id
 
     def started(self, value: T_contra | None = None) -> None:
         try:
@@ -546,14 +597,32 @@
                 "called 'started' twice on the same task status"
             ) from None
 
         task = cast(asyncio.Task, current_task())
         _task_states[task].parent_id = self._parent_id
 
 
+def collapse_exception_group(excgroup: BaseExceptionGroup) -> BaseException:
+    exceptions = list(excgroup.exceptions)
+    modified = False
+    for i, exc in enumerate(exceptions):
+        if isinstance(exc, BaseExceptionGroup):
+            new_exc = collapse_exception_group(exc)
+            if new_exc is not exc:
+                modified = True
+                exceptions[i] = new_exc
+
+    if len(exceptions) == 1:
+        return exceptions[0]
+    elif modified:
+        return excgroup.derive(exceptions)
+    else:
+        return excgroup
+
+
 class TaskGroup(abc.TaskGroup):
     def __init__(self) -> None:
         self.cancel_scope: CancelScope = CancelScope()
         self._active = False
         self._exceptions: list[BaseException] = []
 
     async def __aenter__(self) -> TaskGroup:
@@ -566,163 +635,112 @@
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> bool | None:
         ignore_exception = self.cancel_scope.__exit__(exc_type, exc_val, exc_tb)
         if exc_val is not None:
             self.cancel_scope.cancel()
-            self._exceptions.append(exc_val)
+            if not isinstance(exc_val, CancelledError):
+                self._exceptions.append(exc_val)
 
+        cancelled_exc_while_waiting_tasks: CancelledError | None = None
+        waited_for_tasks_to_finish = bool(self.cancel_scope._tasks)
         while self.cancel_scope._tasks:
             try:
                 await asyncio.wait(self.cancel_scope._tasks)
-            except asyncio.CancelledError:
+            except CancelledError as exc:
+                # This task was cancelled natively; reraise the CancelledError later
+                # unless this task was already interrupted by another exception
                 self.cancel_scope.cancel()
+                if cancelled_exc_while_waiting_tasks is None:
+                    cancelled_exc_while_waiting_tasks = exc
 
         self._active = False
-        if not self.cancel_scope._parent_cancelled():
-            exceptions = self._filter_cancellation_errors(self._exceptions)
-        else:
-            exceptions = self._exceptions
+        if self._exceptions:
+            raise BaseExceptionGroup(
+                "unhandled errors in a TaskGroup", self._exceptions
+            )
 
-        try:
-            if len(exceptions) > 1:
-                if all(
-                    isinstance(e, CancelledError) and not e.args for e in exceptions
-                ):
-                    # Tasks were cancelled natively, without a cancellation message
-                    raise CancelledError
-                else:
-                    raise ExceptionGroup(exceptions)
-            elif exceptions and exceptions[0] is not exc_val:
-                raise exceptions[0]
-        except BaseException as exc:
-            # Clear the context here, as it can only be done in-flight.
-            # If the context is not cleared, it can result in recursive tracebacks (see #145).
-            exc.__context__ = None
-            raise
+        # Raise the CancelledError received while waiting for child tasks to exit,
+        # unless the context manager itself was previously exited with another
+        # exception, or if any of the  child tasks raised an exception other than
+        # CancelledError
+        if cancelled_exc_while_waiting_tasks:
+            if exc_val is None or ignore_exception:
+                raise cancelled_exc_while_waiting_tasks
+
+        # Yield control to the event loop here to ensure that there is at least one
+        # yield point within __aexit__() (trio does the same)
+        if not waited_for_tasks_to_finish:
+            await AsyncIOBackend.checkpoint()
 
         return ignore_exception
 
-    @staticmethod
-    def _filter_cancellation_errors(
-        exceptions: Sequence[BaseException],
-    ) -> list[BaseException]:
-        filtered_exceptions: list[BaseException] = []
-        for exc in exceptions:
-            if isinstance(exc, ExceptionGroup):
-                new_exceptions = TaskGroup._filter_cancellation_errors(exc.exceptions)
-                if len(new_exceptions) > 1:
-                    filtered_exceptions.append(exc)
-                elif len(new_exceptions) == 1:
-                    filtered_exceptions.append(new_exceptions[0])
-                elif new_exceptions:
-                    new_exc = ExceptionGroup(new_exceptions)
-                    new_exc.__cause__ = exc.__cause__
-                    new_exc.__context__ = exc.__context__
-                    new_exc.__traceback__ = exc.__traceback__
-                    filtered_exceptions.append(new_exc)
-            elif not isinstance(exc, CancelledError) or exc.args:
-                filtered_exceptions.append(exc)
-
-        return filtered_exceptions
-
-    async def _run_wrapped_task(
-        self, coro: Coroutine, task_status_future: asyncio.Future | None
-    ) -> None:
-        # This is the code path for Python 3.7 on which asyncio freaks out if a task
-        # raises a BaseException.
-        __traceback_hide__ = __tracebackhide__ = True  # noqa: F841
-        task = cast(asyncio.Task, current_task())
-        try:
-            await coro
-        except BaseException as exc:
-            if task_status_future is None or task_status_future.done():
-                self._exceptions.append(exc)
-                self.cancel_scope.cancel()
-            else:
-                task_status_future.set_exception(exc)
-        else:
-            if task_status_future is not None and not task_status_future.done():
-                task_status_future.set_exception(
-                    RuntimeError("Child exited without calling task_status.started()")
-                )
-        finally:
-            if task in self.cancel_scope._tasks:
-                self.cancel_scope._tasks.remove(task)
-                del _task_states[task]
-
     def _spawn(
         self,
         func: Callable[..., Awaitable[Any]],
         args: tuple,
         name: object,
         task_status_future: asyncio.Future | None = None,
     ) -> asyncio.Task:
         def task_done(_task: asyncio.Task) -> None:
-            # This is the code path for Python 3.8+
             assert _task in self.cancel_scope._tasks
             self.cancel_scope._tasks.remove(_task)
             del _task_states[_task]
 
             try:
                 exc = _task.exception()
             except CancelledError as e:
                 while isinstance(e.__context__, CancelledError):
                     e = e.__context__
 
                 exc = e
 
             if exc is not None:
                 if task_status_future is None or task_status_future.done():
-                    self._exceptions.append(exc)
+                    if not isinstance(exc, CancelledError):
+                        self._exceptions.append(exc)
+
                     self.cancel_scope.cancel()
                 else:
                     task_status_future.set_exception(exc)
             elif task_status_future is not None and not task_status_future.done():
                 task_status_future.set_exception(
                     RuntimeError("Child exited without calling task_status.started()")
                 )
 
         if not self._active:
             raise RuntimeError(
                 "This task group is not active; no new tasks can be started."
             )
 
-        options: dict[str, Any] = {}
-        name = get_callable_name(func) if name is None else str(name)
-        if _native_task_names:
-            options["name"] = name
-
         kwargs = {}
         if task_status_future:
             parent_id = id(current_task())
             kwargs["task_status"] = _AsyncioTaskStatus(
                 task_status_future, id(self.cancel_scope._host_task)
             )
         else:
             parent_id = id(self.cancel_scope._host_task)
 
         coro = func(*args, **kwargs)
-        if not asyncio.iscoroutine(coro):
+        if not iscoroutine(coro):
+            prefix = f"{func.__module__}." if hasattr(func, "__module__") else ""
             raise TypeError(
-                f"Expected an async function, but {func} appears to be synchronous"
+                f"Expected {prefix}{func.__qualname__}() to return a coroutine, but "
+                f"the return value ({coro!r}) is not a coroutine object"
             )
 
-        foreign_coro = not hasattr(coro, "cr_frame") and not hasattr(coro, "gi_frame")
-        if foreign_coro or sys.version_info < (3, 8):
-            coro = self._run_wrapped_task(coro, task_status_future)
-
-        task = create_task(coro, **options)
-        if not foreign_coro and sys.version_info >= (3, 8):
-            task.add_done_callback(task_done)
+        name = get_callable_name(func) if name is None else str(name)
+        task = create_task(coro, name=name)
+        task.add_done_callback(task_done)
 
         # Make the spawned task inherit the task group's cancel scope
         _task_states[task] = TaskState(
-            parent_id=parent_id, name=name, cancel_scope=self.cancel_scope
+            parent_id=parent_id, cancel_scope=self.cancel_scope
         )
         self.cancel_scope._tasks.add(task)
         return task
 
     def start_soon(
         self, func: Callable[..., Awaitable[Any]], *args: object, name: object = None
     ) -> None:
@@ -730,23 +748,27 @@
 
     async def start(
         self, func: Callable[..., Awaitable[Any]], *args: object, name: object = None
     ) -> None:
         future: asyncio.Future = asyncio.Future()
         task = self._spawn(func, args, name, future)
 
-        # If the task raises an exception after sending a start value without a switch point
-        # between, the task group is cancelled and this method never proceeds to process the
-        # completed future. That's why we have to have a shielded cancel scope here.
-        with CancelScope(shield=True):
-            try:
-                return await future
-            except CancelledError:
-                task.cancel()
-                raise
+        # If the task raises an exception after sending a start value without a switch
+        # point between, the task group is cancelled and this method never proceeds to
+        # process the completed future. That's why we have to have a shielded cancel
+        # scope here.
+        try:
+            return await future
+        except CancelledError:
+            # Cancel the task and wait for it to exit before returning
+            task.cancel()
+            with CancelScope(shield=True), suppress(CancelledError):
+                await task
+
+            raise
 
 
 #
 # Threads
 #
 
 _Retval_Queue_Type = Tuple[Optional[T_Retval], Optional[BaseException]]
@@ -765,21 +787,21 @@
         self.root_task = root_task
         self.workers = workers
         self.idle_workers = idle_workers
         self.loop = root_task._loop
         self.queue: Queue[
             tuple[Context, Callable, tuple, asyncio.Future] | None
         ] = Queue(2)
-        self.idle_since = current_time()
+        self.idle_since = AsyncIOBackend.current_time()
         self.stopping = False
 
     def _report_result(
         self, future: asyncio.Future, result: Any, exc: BaseException | None
     ) -> None:
-        self.idle_since = current_time()
+        self.idle_since = AsyncIOBackend.current_time()
         if not self.stopping:
             self.idle_workers.append(self)
 
         if not future.cancelled():
             if exc is not None:
                 if isinstance(exc, StopIteration):
                     new_exc = RuntimeError("coroutine raised StopIteration")
@@ -787,16 +809,15 @@
                     exc = new_exc
 
                 future.set_exception(exc)
             else:
                 future.set_result(result)
 
     def run(self) -> None:
-        with claim_worker_thread("asyncio"):
-            threadlocals.loop = self.loop
+        with claim_worker_thread(AsyncIOBackend, self.loop):
             while True:
                 item = self.queue.get()
                 if item is None:
                     # Shutdown command received
                     return
 
                 context, func, args, future = item
@@ -827,113 +848,34 @@
 
 _threadpool_idle_workers: RunVar[deque[WorkerThread]] = RunVar(
     "_threadpool_idle_workers"
 )
 _threadpool_workers: RunVar[set[WorkerThread]] = RunVar("_threadpool_workers")
 
 
-async def run_sync_in_worker_thread(
-    func: Callable[..., T_Retval],
-    *args: object,
-    cancellable: bool = False,
-    limiter: CapacityLimiter | None = None,
-) -> T_Retval:
-    await checkpoint()
-
-    # If this is the first run in this event loop thread, set up the necessary variables
-    try:
-        idle_workers = _threadpool_idle_workers.get()
-        workers = _threadpool_workers.get()
-    except LookupError:
-        idle_workers = deque()
-        workers = set()
-        _threadpool_idle_workers.set(idle_workers)
-        _threadpool_workers.set(workers)
-
-    async with (limiter or current_default_thread_limiter()):
-        with CancelScope(shield=not cancellable):
-            future: asyncio.Future = asyncio.Future()
-            root_task = find_root_task()
-            if not idle_workers:
-                worker = WorkerThread(root_task, workers, idle_workers)
-                worker.start()
-                workers.add(worker)
-                root_task.add_done_callback(worker.stop)
-            else:
-                worker = idle_workers.pop()
-
-                # Prune any other workers that have been idle for MAX_IDLE_TIME seconds or longer
-                now = current_time()
-                while idle_workers:
-                    if now - idle_workers[0].idle_since < WorkerThread.MAX_IDLE_TIME:
-                        break
-
-                    expired_worker = idle_workers.popleft()
-                    expired_worker.root_task.remove_done_callback(expired_worker.stop)
-                    expired_worker.stop()
-
-            context = copy_context()
-            context.run(sniffio.current_async_library_cvar.set, None)
-            worker.queue.put_nowait((context, func, args, future))
-            return await future
-
-
-def run_sync_from_thread(
-    func: Callable[..., T_Retval],
-    *args: object,
-    loop: asyncio.AbstractEventLoop | None = None,
-) -> T_Retval:
-    @wraps(func)
-    def wrapper() -> None:
-        try:
-            f.set_result(func(*args))
-        except BaseException as exc:
-            f.set_exception(exc)
-            if not isinstance(exc, Exception):
-                raise
-
-    f: concurrent.futures.Future[T_Retval] = Future()
-    loop = loop or threadlocals.loop
-    loop.call_soon_threadsafe(wrapper)
-    return f.result()
-
-
-def run_async_from_thread(
-    func: Callable[..., Awaitable[T_Retval]], *args: object
-) -> T_Retval:
-    f: concurrent.futures.Future[T_Retval] = asyncio.run_coroutine_threadsafe(
-        func(*args), threadlocals.loop
-    )
-    return f.result()
-
-
 class BlockingPortal(abc.BlockingPortal):
     def __new__(cls) -> BlockingPortal:
         return object.__new__(cls)
 
     def __init__(self) -> None:
         super().__init__()
         self._loop = get_running_loop()
 
     def _spawn_task_from_thread(
         self,
         func: Callable,
-        args: tuple,
+        args: tuple[Any, ...],
         kwargs: dict[str, Any],
         name: object,
         future: Future,
     ) -> None:
-        run_sync_from_thread(
+        AsyncIOBackend.run_sync_from_thread(
             partial(self._task_group.start_soon, name=name),
-            self._call_func,
-            func,
-            args,
-            kwargs,
-            future,
-            loop=self._loop,
+            (self._call_func, func, args, kwargs, future),
+            self._loop,
         )
 
 
 #
 # Subprocesses
 #
 
@@ -1011,106 +953,59 @@
         return self._stdout
 
     @property
     def stderr(self) -> abc.ByteReceiveStream | None:
         return self._stderr
 
 
-async def open_process(
-    command: str | bytes | Sequence[str | bytes],
-    *,
-    shell: bool,
-    stdin: int | IO[Any] | None,
-    stdout: int | IO[Any] | None,
-    stderr: int | IO[Any] | None,
-    cwd: str | bytes | PathLike | None = None,
-    env: Mapping[str, str] | None = None,
-    start_new_session: bool = False,
-) -> Process:
-    await checkpoint()
-    if shell:
-        process = await asyncio.create_subprocess_shell(
-            cast(Union[str, bytes], command),
-            stdin=stdin,
-            stdout=stdout,
-            stderr=stderr,
-            cwd=cwd,
-            env=env,
-            start_new_session=start_new_session,
-        )
-    else:
-        process = await asyncio.create_subprocess_exec(
-            *command,
-            stdin=stdin,
-            stdout=stdout,
-            stderr=stderr,
-            cwd=cwd,
-            env=env,
-            start_new_session=start_new_session,
-        )
-
-    stdin_stream = StreamWriterWrapper(process.stdin) if process.stdin else None
-    stdout_stream = StreamReaderWrapper(process.stdout) if process.stdout else None
-    stderr_stream = StreamReaderWrapper(process.stderr) if process.stderr else None
-    return Process(process, stdin_stream, stdout_stream, stderr_stream)
-
-
 def _forcibly_shutdown_process_pool_on_exit(
     workers: set[Process], _task: object
 ) -> None:
     """
     Forcibly shuts down worker processes belonging to this event loop."""
-    child_watcher: asyncio.AbstractChildWatcher | None
-    try:
-        child_watcher = asyncio.get_event_loop_policy().get_child_watcher()
-    except NotImplementedError:
-        child_watcher = None
+    child_watcher: asyncio.AbstractChildWatcher | None = None
+    if sys.version_info < (3, 12):
+        try:
+            child_watcher = asyncio.get_event_loop_policy().get_child_watcher()
+        except NotImplementedError:
+            pass
 
     # Close as much as possible (w/o async/await) to avoid warnings
     for process in workers:
         if process.returncode is None:
             continue
 
         process._stdin._stream._transport.close()  # type: ignore[union-attr]
         process._stdout._stream._transport.close()  # type: ignore[union-attr]
         process._stderr._stream._transport.close()  # type: ignore[union-attr]
         process.kill()
         if child_watcher:
             child_watcher.remove_child_handler(process.pid)
 
 
-async def _shutdown_process_pool_on_exit(workers: set[Process]) -> None:
+async def _shutdown_process_pool_on_exit(workers: set[abc.Process]) -> None:
     """
     Shuts down worker processes belonging to this event loop.
 
-    NOTE: this only works when the event loop was started using asyncio.run() or anyio.run().
+    NOTE: this only works when the event loop was started using asyncio.run() or
+    anyio.run().
 
     """
-    process: Process
+    process: abc.Process
     try:
         await sleep(math.inf)
     except asyncio.CancelledError:
         for process in workers:
             if process.returncode is None:
                 process.kill()
 
         for process in workers:
             await process.aclose()
 
 
-def setup_process_pool_exit_at_shutdown(workers: set[Process]) -> None:
-    kwargs: dict[str, Any] = (
-        {"name": "AnyIO process pool shutdown task"} if _native_task_names else {}
-    )
-    create_task(_shutdown_process_pool_on_exit(workers), **kwargs)
-    find_root_task().add_done_callback(
-        partial(_forcibly_shutdown_process_pool_on_exit, workers)
-    )
-
-
 #
 # Sockets and networking
 #
 
 
 class StreamProtocol(asyncio.Protocol):
     read_queue: deque[bytes]
@@ -1189,15 +1084,15 @@
 
     @property
     def _raw_socket(self) -> socket.socket:
         return self._transport.get_extra_info("socket")
 
     async def receive(self, max_bytes: int = 65536) -> bytes:
         with self._receive_guard:
-            await checkpoint()
+            await AsyncIOBackend.checkpoint()
 
             if (
                 not self._protocol.read_event.is_set()
                 and not self._transport.is_closing()
             ):
                 self._transport.resume_reading()
                 await self._protocol.read_event.wait()
@@ -1205,33 +1100,33 @@
 
             try:
                 chunk = self._protocol.read_queue.popleft()
             except IndexError:
                 if self._closed:
                     raise ClosedResourceError from None
                 elif self._protocol.exception:
-                    raise self._protocol.exception
+                    raise self._protocol.exception from None
                 else:
                     raise EndOfStream from None
 
             if len(chunk) > max_bytes:
                 # Split the oversized chunk
                 chunk, leftover = chunk[:max_bytes], chunk[max_bytes:]
                 self._protocol.read_queue.appendleft(leftover)
 
-            # If the read queue is empty, clear the flag so that the next call will block until
-            # data is available
+            # If the read queue is empty, clear the flag so that the next call will
+            # block until data is available
             if not self._protocol.read_queue:
                 self._protocol.read_event.clear()
 
         return chunk
 
     async def send(self, item: bytes) -> None:
         with self._send_guard:
-            await checkpoint()
+            await AsyncIOBackend.checkpoint()
 
             if self._closed:
                 raise ClosedResourceError
             elif self._protocol.exception is not None:
                 raise self._protocol.exception
 
             try:
@@ -1259,60 +1154,72 @@
                 pass
 
             self._transport.close()
             await sleep(0)
             self._transport.abort()
 
 
-class UNIXSocketStream(abc.SocketStream):
+class _RawSocketMixin:
     _receive_future: asyncio.Future | None = None
     _send_future: asyncio.Future | None = None
     _closing = False
 
     def __init__(self, raw_socket: socket.socket):
         self.__raw_socket = raw_socket
-        self._loop = get_running_loop()
         self._receive_guard = ResourceGuard("reading from")
         self._send_guard = ResourceGuard("writing to")
 
     @property
     def _raw_socket(self) -> socket.socket:
         return self.__raw_socket
 
     def _wait_until_readable(self, loop: asyncio.AbstractEventLoop) -> asyncio.Future:
         def callback(f: object) -> None:
             del self._receive_future
             loop.remove_reader(self.__raw_socket)
 
         f = self._receive_future = asyncio.Future()
-        self._loop.add_reader(self.__raw_socket, f.set_result, None)
+        loop.add_reader(self.__raw_socket, f.set_result, None)
         f.add_done_callback(callback)
         return f
 
     def _wait_until_writable(self, loop: asyncio.AbstractEventLoop) -> asyncio.Future:
         def callback(f: object) -> None:
             del self._send_future
             loop.remove_writer(self.__raw_socket)
 
         f = self._send_future = asyncio.Future()
-        self._loop.add_writer(self.__raw_socket, f.set_result, None)
+        loop.add_writer(self.__raw_socket, f.set_result, None)
         f.add_done_callback(callback)
         return f
 
+    async def aclose(self) -> None:
+        if not self._closing:
+            self._closing = True
+            if self.__raw_socket.fileno() != -1:
+                self.__raw_socket.close()
+
+            if self._receive_future:
+                self._receive_future.set_result(None)
+            if self._send_future:
+                self._send_future.set_result(None)
+
+
+class UNIXSocketStream(_RawSocketMixin, abc.UNIXSocketStream):
     async def send_eof(self) -> None:
         with self._send_guard:
             self._raw_socket.shutdown(socket.SHUT_WR)
 
     async def receive(self, max_bytes: int = 65536) -> bytes:
         loop = get_running_loop()
-        await checkpoint()
+        await AsyncIOBackend.checkpoint()
         with self._receive_guard:
             while True:
                 try:
-                    data = self.__raw_socket.recv(max_bytes)
+                    data = self._raw_socket.recv(max_bytes)
                 except BlockingIOError:
                     await self._wait_until_readable(loop)
                 except OSError as exc:
                     if self._closing:
                         raise ClosedResourceError from None
                     else:
                         raise BrokenResourceError from exc
@@ -1320,20 +1227,20 @@
                     if not data:
                         raise EndOfStream
 
                     return data
 
     async def send(self, item: bytes) -> None:
         loop = get_running_loop()
-        await checkpoint()
+        await AsyncIOBackend.checkpoint()
         with self._send_guard:
             view = memoryview(item)
             while view:
                 try:
-                    bytes_sent = self.__raw_socket.send(view)
+                    bytes_sent = self._raw_socket.send(view)
                 except BlockingIOError:
                     await self._wait_until_writable(loop)
                 except OSError as exc:
                     if self._closing:
                         raise ClosedResourceError from None
                     else:
                         raise BrokenResourceError from exc
@@ -1344,19 +1251,19 @@
         if not isinstance(msglen, int) or msglen < 0:
             raise ValueError("msglen must be a non-negative integer")
         if not isinstance(maxfds, int) or maxfds < 1:
             raise ValueError("maxfds must be a positive integer")
 
         loop = get_running_loop()
         fds = array.array("i")
-        await checkpoint()
+        await AsyncIOBackend.checkpoint()
         with self._receive_guard:
             while True:
                 try:
-                    message, ancdata, flags, addr = self.__raw_socket.recvmsg(
+                    message, ancdata, flags, addr = self._raw_socket.recvmsg(
                         msglen, socket.CMSG_LEN(maxfds * fds.itemsize)
                     )
                 except BlockingIOError:
                     await self._wait_until_readable(loop)
                 except OSError as exc:
                     if self._closing:
                         raise ClosedResourceError from None
@@ -1390,43 +1297,32 @@
         for fd in fds:
             if isinstance(fd, int):
                 filenos.append(fd)
             elif isinstance(fd, IOBase):
                 filenos.append(fd.fileno())
 
         fdarray = array.array("i", filenos)
-        await checkpoint()
+        await AsyncIOBackend.checkpoint()
         with self._send_guard:
             while True:
                 try:
                     # The ignore can be removed after mypy picks up
                     # https://github.com/python/typeshed/pull/5545
-                    self.__raw_socket.sendmsg(
+                    self._raw_socket.sendmsg(
                         [message], [(socket.SOL_SOCKET, socket.SCM_RIGHTS, fdarray)]
                     )
                     break
                 except BlockingIOError:
                     await self._wait_until_writable(loop)
                 except OSError as exc:
                     if self._closing:
                         raise ClosedResourceError from None
                     else:
                         raise BrokenResourceError from exc
 
-    async def aclose(self) -> None:
-        if not self._closing:
-            self._closing = True
-            if self.__raw_socket.fileno() != -1:
-                self.__raw_socket.close()
-
-            if self._receive_future:
-                self._receive_future.set_result(None)
-            if self._send_future:
-                self._send_future.set_result(None)
-
 
 class TCPSocketListener(abc.SocketListener):
     _accept_scope: CancelScope | None = None
     _closed = False
 
     def __init__(self, raw_socket: socket.socket):
         self.__raw_socket = raw_socket
@@ -1438,15 +1334,15 @@
         return self.__raw_socket
 
     async def accept(self) -> abc.SocketStream:
         if self._closed:
             raise ClosedResourceError
 
         with self._accept_guard:
-            await checkpoint()
+            await AsyncIOBackend.checkpoint()
             with CancelScope() as self._accept_scope:
                 try:
                     client_sock, _addr = await self._loop.sock_accept(self._raw_socket)
                 except asyncio.CancelledError:
                     # Workaround for https://bugs.python.org/issue41317
                     try:
                         self._loop.remove_reader(self._raw_socket)
@@ -1488,15 +1384,15 @@
     def __init__(self, raw_socket: socket.socket):
         self.__raw_socket = raw_socket
         self._loop = get_running_loop()
         self._accept_guard = ResourceGuard("accepting connections from")
         self._closed = False
 
     async def accept(self) -> abc.SocketStream:
-        await checkpoint()
+        await AsyncIOBackend.checkpoint()
         with self._accept_guard:
             while True:
                 try:
                     client_sock, _ = self.__raw_socket.accept()
                     client_sock.setblocking(False)
                     return UNIXSocketStream(client_sock)
                 except BlockingIOError:
@@ -1538,15 +1434,15 @@
     async def aclose(self) -> None:
         if not self._transport.is_closing():
             self._closed = True
             self._transport.close()
 
     async def receive(self) -> tuple[bytes, IPSockAddrType]:
         with self._receive_guard:
-            await checkpoint()
+            await AsyncIOBackend.checkpoint()
 
             # If the buffer is empty, ask for more data
             if not self._protocol.read_queue and not self._transport.is_closing():
                 self._protocol.read_event.clear()
                 await self._protocol.read_event.wait()
 
             try:
@@ -1555,15 +1451,15 @@
                 if self._closed:
                     raise ClosedResourceError from None
                 else:
                     raise BrokenResourceError from None
 
     async def send(self, item: UDPPacketType) -> None:
         with self._send_guard:
-            await checkpoint()
+            await AsyncIOBackend.checkpoint()
             await self._protocol.write_event.wait()
             if self._closed:
                 raise ClosedResourceError
             elif self._transport.is_closing():
                 raise BrokenResourceError
             else:
                 self._transport.sendto(*item)
@@ -1586,15 +1482,15 @@
     async def aclose(self) -> None:
         if not self._transport.is_closing():
             self._closed = True
             self._transport.close()
 
     async def receive(self) -> bytes:
         with self._receive_guard:
-            await checkpoint()
+            await AsyncIOBackend.checkpoint()
 
             # If the buffer is empty, ask for more data
             if not self._protocol.read_queue and not self._transport.is_closing():
                 self._protocol.read_event.clear()
                 await self._protocol.read_event.wait()
 
             try:
@@ -1605,182 +1501,123 @@
                 else:
                     raise BrokenResourceError from None
 
             return packet[0]
 
     async def send(self, item: bytes) -> None:
         with self._send_guard:
-            await checkpoint()
+            await AsyncIOBackend.checkpoint()
             await self._protocol.write_event.wait()
             if self._closed:
                 raise ClosedResourceError
             elif self._transport.is_closing():
                 raise BrokenResourceError
             else:
                 self._transport.sendto(item)
 
 
-async def connect_tcp(
-    host: str, port: int, local_addr: tuple[str, int] | None = None
-) -> SocketStream:
-    transport, protocol = cast(
-        Tuple[asyncio.Transport, StreamProtocol],
-        await get_running_loop().create_connection(
-            StreamProtocol, host, port, local_addr=local_addr
-        ),
-    )
-    transport.pause_reading()
-    return SocketStream(transport, protocol)
-
-
-async def connect_unix(path: str) -> UNIXSocketStream:
-    await checkpoint()
-    loop = get_running_loop()
-    raw_socket = socket.socket(socket.AF_UNIX)
-    raw_socket.setblocking(False)
-    while True:
-        try:
-            raw_socket.connect(path)
-        except BlockingIOError:
-            f: asyncio.Future = asyncio.Future()
-            loop.add_writer(raw_socket, f.set_result, None)
-            f.add_done_callback(lambda _: loop.remove_writer(raw_socket))
-            await f
-        except BaseException:
-            raw_socket.close()
-            raise
-        else:
-            return UNIXSocketStream(raw_socket)
-
-
-async def create_udp_socket(
-    family: socket.AddressFamily,
-    local_address: IPSockAddrType | None,
-    remote_address: IPSockAddrType | None,
-    reuse_port: bool,
-) -> UDPSocket | ConnectedUDPSocket:
-    result = await get_running_loop().create_datagram_endpoint(
-        DatagramProtocol,
-        local_addr=local_address,
-        remote_addr=remote_address,
-        family=family,
-        reuse_port=reuse_port,
-    )
-    transport = result[0]
-    protocol = result[1]
-    if protocol.exception:
-        transport.close()
-        raise protocol.exception
-
-    if not remote_address:
-        return UDPSocket(transport, protocol)
-    else:
-        return ConnectedUDPSocket(transport, protocol)
+class UNIXDatagramSocket(_RawSocketMixin, abc.UNIXDatagramSocket):
+    async def receive(self) -> UNIXDatagramPacketType:
+        loop = get_running_loop()
+        await AsyncIOBackend.checkpoint()
+        with self._receive_guard:
+            while True:
+                try:
+                    data = self._raw_socket.recvfrom(65536)
+                except BlockingIOError:
+                    await self._wait_until_readable(loop)
+                except OSError as exc:
+                    if self._closing:
+                        raise ClosedResourceError from None
+                    else:
+                        raise BrokenResourceError from exc
+                else:
+                    return data
 
+    async def send(self, item: UNIXDatagramPacketType) -> None:
+        loop = get_running_loop()
+        await AsyncIOBackend.checkpoint()
+        with self._send_guard:
+            while True:
+                try:
+                    self._raw_socket.sendto(*item)
+                except BlockingIOError:
+                    await self._wait_until_writable(loop)
+                except OSError as exc:
+                    if self._closing:
+                        raise ClosedResourceError from None
+                    else:
+                        raise BrokenResourceError from exc
+                else:
+                    return
 
-async def getaddrinfo(
-    host: bytes | str,
-    port: str | int | None,
-    *,
-    family: int | AddressFamily = 0,
-    type: int | SocketKind = 0,
-    proto: int = 0,
-    flags: int = 0,
-) -> GetAddrInfoReturnType:
-    # https://github.com/python/typeshed/pull/4304
-    result = await get_running_loop().getaddrinfo(
-        host, port, family=family, type=type, proto=proto, flags=flags
-    )
-    return cast(GetAddrInfoReturnType, result)
 
+class ConnectedUNIXDatagramSocket(_RawSocketMixin, abc.ConnectedUNIXDatagramSocket):
+    async def receive(self) -> bytes:
+        loop = get_running_loop()
+        await AsyncIOBackend.checkpoint()
+        with self._receive_guard:
+            while True:
+                try:
+                    data = self._raw_socket.recv(65536)
+                except BlockingIOError:
+                    await self._wait_until_readable(loop)
+                except OSError as exc:
+                    if self._closing:
+                        raise ClosedResourceError from None
+                    else:
+                        raise BrokenResourceError from exc
+                else:
+                    return data
 
-async def getnameinfo(sockaddr: IPSockAddrType, flags: int = 0) -> tuple[str, str]:
-    return await get_running_loop().getnameinfo(sockaddr, flags)
+    async def send(self, item: bytes) -> None:
+        loop = get_running_loop()
+        await AsyncIOBackend.checkpoint()
+        with self._send_guard:
+            while True:
+                try:
+                    self._raw_socket.send(item)
+                except BlockingIOError:
+                    await self._wait_until_writable(loop)
+                except OSError as exc:
+                    if self._closing:
+                        raise ClosedResourceError from None
+                    else:
+                        raise BrokenResourceError from exc
+                else:
+                    return
 
 
 _read_events: RunVar[dict[Any, asyncio.Event]] = RunVar("read_events")
 _write_events: RunVar[dict[Any, asyncio.Event]] = RunVar("write_events")
 
 
-async def wait_socket_readable(sock: socket.socket) -> None:
-    await checkpoint()
-    try:
-        read_events = _read_events.get()
-    except LookupError:
-        read_events = {}
-        _read_events.set(read_events)
-
-    if read_events.get(sock):
-        raise BusyResourceError("reading from") from None
-
-    loop = get_running_loop()
-    event = read_events[sock] = asyncio.Event()
-    loop.add_reader(sock, event.set)
-    try:
-        await event.wait()
-    finally:
-        if read_events.pop(sock, None) is not None:
-            loop.remove_reader(sock)
-            readable = True
-        else:
-            readable = False
-
-    if not readable:
-        raise ClosedResourceError
-
-
-async def wait_socket_writable(sock: socket.socket) -> None:
-    await checkpoint()
-    try:
-        write_events = _write_events.get()
-    except LookupError:
-        write_events = {}
-        _write_events.set(write_events)
-
-    if write_events.get(sock):
-        raise BusyResourceError("writing to") from None
-
-    loop = get_running_loop()
-    event = write_events[sock] = asyncio.Event()
-    loop.add_writer(sock.fileno(), event.set)
-    try:
-        await event.wait()
-    finally:
-        if write_events.pop(sock, None) is not None:
-            loop.remove_writer(sock)
-            writable = True
-        else:
-            writable = False
-
-    if not writable:
-        raise ClosedResourceError
-
-
 #
 # Synchronization
 #
 
 
 class Event(BaseEvent):
     def __new__(cls) -> Event:
         return object.__new__(cls)
 
     def __init__(self) -> None:
         self._event = asyncio.Event()
 
-    def set(self) -> DeprecatedAwaitable:
+    def set(self) -> None:
         self._event.set()
-        return DeprecatedAwaitable(self.set)
 
     def is_set(self) -> bool:
         return self._event.is_set()
 
     async def wait(self) -> None:
-        if await self._event.wait():
-            await checkpoint()
+        if self.is_set():
+            await AsyncIOBackend.checkpoint()
+        else:
+            await self._event.wait()
 
     def statistics(self) -> EventStatistics:
         return EventStatistics(len(self._event._waiters))  # type: ignore[attr-defined]
 
 
 class CapacityLimiter(BaseCapacityLimiter):
     _total_tokens: float = 0
@@ -1833,51 +1670,49 @@
     def borrowed_tokens(self) -> int:
         return len(self._borrowers)
 
     @property
     def available_tokens(self) -> float:
         return self._total_tokens - len(self._borrowers)
 
-    def acquire_nowait(self) -> DeprecatedAwaitable:
+    def acquire_nowait(self) -> None:
         self.acquire_on_behalf_of_nowait(current_task())
-        return DeprecatedAwaitable(self.acquire_nowait)
 
-    def acquire_on_behalf_of_nowait(self, borrower: object) -> DeprecatedAwaitable:
+    def acquire_on_behalf_of_nowait(self, borrower: object) -> None:
         if borrower in self._borrowers:
             raise RuntimeError(
                 "this borrower is already holding one of this CapacityLimiter's "
                 "tokens"
             )
 
         if self._wait_queue or len(self._borrowers) >= self._total_tokens:
             raise WouldBlock
 
         self._borrowers.add(borrower)
-        return DeprecatedAwaitable(self.acquire_on_behalf_of_nowait)
 
     async def acquire(self) -> None:
         return await self.acquire_on_behalf_of(current_task())
 
     async def acquire_on_behalf_of(self, borrower: object) -> None:
-        await checkpoint_if_cancelled()
+        await AsyncIOBackend.checkpoint_if_cancelled()
         try:
             self.acquire_on_behalf_of_nowait(borrower)
         except WouldBlock:
             event = asyncio.Event()
             self._wait_queue[borrower] = event
             try:
                 await event.wait()
             except BaseException:
                 self._wait_queue.pop(borrower, None)
                 raise
 
             self._borrowers.add(borrower)
         else:
             try:
-                await cancel_shielded_checkpoint()
+                await AsyncIOBackend.cancel_shielded_checkpoint()
             except BaseException:
                 self.release()
                 raise
 
     def release(self) -> None:
         self.release_on_behalf_of(current_task())
 
@@ -1902,37 +1737,28 @@
             len(self._wait_queue),
         )
 
 
 _default_thread_limiter: RunVar[CapacityLimiter] = RunVar("_default_thread_limiter")
 
 
-def current_default_thread_limiter() -> CapacityLimiter:
-    try:
-        return _default_thread_limiter.get()
-    except LookupError:
-        limiter = CapacityLimiter(40)
-        _default_thread_limiter.set(limiter)
-        return limiter
-
-
 #
 # Operating system signals
 #
 
 
-class _SignalReceiver(DeprecatedAsyncContextManager["_SignalReceiver"]):
-    def __init__(self, signals: tuple[int, ...]):
+class _SignalReceiver:
+    def __init__(self, signals: tuple[Signals, ...]):
         self._signals = signals
         self._loop = get_running_loop()
-        self._signal_queue: deque[int] = deque()
+        self._signal_queue: deque[Signals] = deque()
         self._future: asyncio.Future = asyncio.Future()
-        self._handled_signals: set[int] = set()
+        self._handled_signals: set[Signals] = set()
 
-    def _deliver(self, signum: int) -> None:
+    def _deliver(self, signum: Signals) -> None:
         self._signal_queue.append(signum)
         if not self._future.done():
             self._future.set_result(None)
 
     def __enter__(self) -> _SignalReceiver:
         for sig in set(self._signals):
             self._loop.add_signal_handler(sig, self._deliver, sig)
@@ -1949,98 +1775,72 @@
         for sig in self._handled_signals:
             self._loop.remove_signal_handler(sig)
         return None
 
     def __aiter__(self) -> _SignalReceiver:
         return self
 
-    async def __anext__(self) -> int:
-        await checkpoint()
+    async def __anext__(self) -> Signals:
+        await AsyncIOBackend.checkpoint()
         if not self._signal_queue:
             self._future = asyncio.Future()
             await self._future
 
         return self._signal_queue.popleft()
 
 
-def open_signal_receiver(*signals: int) -> _SignalReceiver:
-    return _SignalReceiver(signals)
-
-
 #
 # Testing and debugging
 #
 
 
 def _create_task_info(task: asyncio.Task) -> TaskInfo:
     task_state = _task_states.get(task)
     if task_state is None:
-        name = task.get_name() if _native_task_names else None
         parent_id = None
     else:
-        name = task_state.name
         parent_id = task_state.parent_id
 
-    return TaskInfo(id(task), parent_id, name, get_coro(task))
-
-
-def get_current_task() -> TaskInfo:
-    return _create_task_info(current_task())  # type: ignore[arg-type]
-
-
-def get_running_tasks() -> list[TaskInfo]:
-    return [_create_task_info(task) for task in all_tasks() if not task.done()]
-
-
-async def wait_all_tasks_blocked() -> None:
-    await checkpoint()
-    this_task = current_task()
-    while True:
-        for task in all_tasks():
-            if task is this_task:
-                continue
-
-            if task._fut_waiter is None or task._fut_waiter.done():  # type: ignore[attr-defined]
-                await sleep(0.1)
-                break
-        else:
-            return
+    return TaskInfo(id(task), parent_id, task.get_name(), task.get_coro())
 
 
 class TestRunner(abc.TestRunner):
+    _send_stream: MemoryObjectSendStream[tuple[Awaitable[Any], asyncio.Future[Any]]]
+
     def __init__(
         self,
-        debug: bool = False,
+        *,
+        debug: bool | None = None,
         use_uvloop: bool = False,
-        policy: asyncio.AbstractEventLoopPolicy | None = None,
-    ):
-        self._exceptions: list[BaseException] = []
-        _maybe_set_event_loop_policy(policy, use_uvloop)
-        self._loop = asyncio.new_event_loop()
-        self._loop.set_debug(debug)
-        self._loop.set_exception_handler(self._exception_handler)
-        asyncio.set_event_loop(self._loop)
+        loop_factory: Callable[[], AbstractEventLoop] | None = None,
+    ) -> None:
+        if use_uvloop and loop_factory is None:
+            import uvloop
 
-    def _cancel_all_tasks(self) -> None:
-        to_cancel = all_tasks(self._loop)
-        if not to_cancel:
-            return
+            loop_factory = uvloop.new_event_loop
 
-        for task in to_cancel:
-            task.cancel()
+        self._runner = Runner(debug=debug, loop_factory=loop_factory)
+        self._exceptions: list[BaseException] = []
+        self._runner_task: asyncio.Task | None = None
 
-        self._loop.run_until_complete(
-            asyncio.gather(*to_cancel, return_exceptions=True)
-        )
+    def __enter__(self) -> TestRunner:
+        self._runner.__enter__()
+        self.get_loop().set_exception_handler(self._exception_handler)
+        return self
 
-        for task in to_cancel:
-            if task.cancelled():
-                continue
-            if task.exception() is not None:
-                raise cast(BaseException, task.exception())
+    def __exit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
+        self._runner.__exit__(exc_type, exc_val, exc_tb)
+
+    def get_loop(self) -> AbstractEventLoop:
+        return self._runner.get_loop()
 
     def _exception_handler(
         self, loop: asyncio.AbstractEventLoop, context: dict[str, Any]
     ) -> None:
         if isinstance(context.get("exception"), Exception):
             self._exceptions.append(context["exception"])
         else:
@@ -2049,69 +1849,559 @@
     def _raise_async_exceptions(self) -> None:
         # Re-raise any exceptions raised in asynchronous callbacks
         if self._exceptions:
             exceptions, self._exceptions = self._exceptions, []
             if len(exceptions) == 1:
                 raise exceptions[0]
             elif exceptions:
-                raise ExceptionGroup(exceptions)
+                raise BaseExceptionGroup(
+                    "Multiple exceptions occurred in asynchronous callbacks", exceptions
+                )
 
-    def close(self) -> None:
-        try:
-            self._cancel_all_tasks()
-            self._loop.run_until_complete(self._loop.shutdown_asyncgens())
-        finally:
-            asyncio.set_event_loop(None)
-            self._loop.close()
+    @staticmethod
+    async def _run_tests_and_fixtures(
+        receive_stream: MemoryObjectReceiveStream[
+            tuple[Awaitable[T_Retval], asyncio.Future[T_Retval]]
+        ],
+    ) -> None:
+        with receive_stream:
+            async for coro, future in receive_stream:
+                try:
+                    retval = await coro
+                except BaseException as exc:
+                    if not future.cancelled():
+                        future.set_exception(exc)
+                else:
+                    if not future.cancelled():
+                        future.set_result(retval)
+
+    async def _call_in_runner_task(
+        self, func: Callable[..., Awaitable[T_Retval]], *args: object, **kwargs: object
+    ) -> T_Retval:
+        if not self._runner_task:
+            self._send_stream, receive_stream = create_memory_object_stream[
+                Tuple[Awaitable[Any], asyncio.Future]
+            ](1)
+            self._runner_task = self.get_loop().create_task(
+                self._run_tests_and_fixtures(receive_stream)
+            )
+
+        coro = func(*args, **kwargs)
+        future: asyncio.Future[T_Retval] = self.get_loop().create_future()
+        self._send_stream.send_nowait((coro, future))
+        return await future
 
     def run_asyncgen_fixture(
         self,
         fixture_func: Callable[..., AsyncGenerator[T_Retval, Any]],
         kwargs: dict[str, Any],
     ) -> Iterable[T_Retval]:
-        async def fixture_runner() -> None:
-            agen = fixture_func(**kwargs)
-            try:
-                retval = await agen.asend(None)
-                self._raise_async_exceptions()
-            except BaseException as exc:
-                f.set_exception(exc)
-                return
-            else:
-                f.set_result(retval)
+        asyncgen = fixture_func(**kwargs)
+        fixturevalue: T_Retval = self.get_loop().run_until_complete(
+            self._call_in_runner_task(asyncgen.asend, None)
+        )
+        self._raise_async_exceptions()
 
-            await event.wait()
-            try:
-                await agen.asend(None)
-            except StopAsyncIteration:
-                pass
-            else:
-                await agen.aclose()
-                raise RuntimeError("Async generator fixture did not stop")
+        yield fixturevalue
 
-        f = self._loop.create_future()
-        event = asyncio.Event()
-        fixture_task = self._loop.create_task(fixture_runner())
-        self._loop.run_until_complete(f)
-        yield f.result()
-        event.set()
-        self._loop.run_until_complete(fixture_task)
-        self._raise_async_exceptions()
+        try:
+            self.get_loop().run_until_complete(
+                self._call_in_runner_task(asyncgen.asend, None)
+            )
+        except StopAsyncIteration:
+            self._raise_async_exceptions()
+        else:
+            self.get_loop().run_until_complete(asyncgen.aclose())
+            raise RuntimeError("Async generator fixture did not stop")
 
     def run_fixture(
         self,
         fixture_func: Callable[..., Coroutine[Any, Any, T_Retval]],
         kwargs: dict[str, Any],
     ) -> T_Retval:
-        retval = self._loop.run_until_complete(fixture_func(**kwargs))
+        retval = self.get_loop().run_until_complete(
+            self._call_in_runner_task(fixture_func, **kwargs)
+        )
         self._raise_async_exceptions()
         return retval
 
     def run_test(
         self, test_func: Callable[..., Coroutine[Any, Any, Any]], kwargs: dict[str, Any]
     ) -> None:
         try:
-            self._loop.run_until_complete(test_func(**kwargs))
+            self.get_loop().run_until_complete(
+                self._call_in_runner_task(test_func, **kwargs)
+            )
         except Exception as exc:
             self._exceptions.append(exc)
 
         self._raise_async_exceptions()
+
+
+class AsyncIOBackend(AsyncBackend):
+    @classmethod
+    def run(
+        cls,
+        func: Callable[..., Awaitable[T_Retval]],
+        args: tuple,
+        kwargs: dict[str, Any],
+        options: dict[str, Any],
+    ) -> T_Retval:
+        @wraps(func)
+        async def wrapper() -> T_Retval:
+            task = cast(asyncio.Task, current_task())
+            task.set_name(get_callable_name(func))
+            _task_states[task] = TaskState(None, None)
+
+            try:
+                return await func(*args)
+            finally:
+                del _task_states[task]
+
+        debug = options.get("debug", False)
+        options.get("loop_factory", None)
+        options.get("use_uvloop", False)
+        return native_run(wrapper(), debug=debug)
+
+    @classmethod
+    def current_token(cls) -> object:
+        return get_running_loop()
+
+    @classmethod
+    def current_time(cls) -> float:
+        return get_running_loop().time()
+
+    @classmethod
+    def cancelled_exception_class(cls) -> type[BaseException]:
+        return CancelledError
+
+    @classmethod
+    async def checkpoint(cls) -> None:
+        await sleep(0)
+
+    @classmethod
+    async def checkpoint_if_cancelled(cls) -> None:
+        task = current_task()
+        if task is None:
+            return
+
+        try:
+            cancel_scope = _task_states[task].cancel_scope
+        except KeyError:
+            return
+
+        while cancel_scope:
+            if cancel_scope.cancel_called:
+                await sleep(0)
+            elif cancel_scope.shield:
+                break
+            else:
+                cancel_scope = cancel_scope._parent_scope
+
+    @classmethod
+    async def cancel_shielded_checkpoint(cls) -> None:
+        with CancelScope(shield=True):
+            await sleep(0)
+
+    @classmethod
+    async def sleep(cls, delay: float) -> None:
+        await sleep(delay)
+
+    @classmethod
+    def create_cancel_scope(
+        cls, *, deadline: float = math.inf, shield: bool = False
+    ) -> CancelScope:
+        return CancelScope(deadline=deadline, shield=shield)
+
+    @classmethod
+    def current_effective_deadline(cls) -> float:
+        try:
+            cancel_scope = _task_states[
+                current_task()  # type: ignore[index]
+            ].cancel_scope
+        except KeyError:
+            return math.inf
+
+        deadline = math.inf
+        while cancel_scope:
+            deadline = min(deadline, cancel_scope.deadline)
+            if cancel_scope._cancel_called:
+                deadline = -math.inf
+                break
+            elif cancel_scope.shield:
+                break
+            else:
+                cancel_scope = cancel_scope._parent_scope
+
+        return deadline
+
+    @classmethod
+    def create_task_group(cls) -> abc.TaskGroup:
+        return TaskGroup()
+
+    @classmethod
+    def create_event(cls) -> abc.Event:
+        return Event()
+
+    @classmethod
+    def create_capacity_limiter(cls, total_tokens: float) -> abc.CapacityLimiter:
+        return CapacityLimiter(total_tokens)
+
+    @classmethod
+    async def run_sync_in_worker_thread(
+        cls,
+        func: Callable[..., T_Retval],
+        args: tuple[Any, ...],
+        cancellable: bool = False,
+        limiter: abc.CapacityLimiter | None = None,
+    ) -> T_Retval:
+        await cls.checkpoint()
+
+        # If this is the first run in this event loop thread, set up the necessary
+        # variables
+        try:
+            idle_workers = _threadpool_idle_workers.get()
+            workers = _threadpool_workers.get()
+        except LookupError:
+            idle_workers = deque()
+            workers = set()
+            _threadpool_idle_workers.set(idle_workers)
+            _threadpool_workers.set(workers)
+
+        async with (limiter or cls.current_default_thread_limiter()):
+            with CancelScope(shield=not cancellable):
+                future: asyncio.Future = asyncio.Future()
+                root_task = find_root_task()
+                if not idle_workers:
+                    worker = WorkerThread(root_task, workers, idle_workers)
+                    worker.start()
+                    workers.add(worker)
+                    root_task.add_done_callback(worker.stop)
+                else:
+                    worker = idle_workers.pop()
+
+                    # Prune any other workers that have been idle for MAX_IDLE_TIME
+                    # seconds or longer
+                    now = cls.current_time()
+                    while idle_workers:
+                        if (
+                            now - idle_workers[0].idle_since
+                            < WorkerThread.MAX_IDLE_TIME
+                        ):
+                            break
+
+                        expired_worker = idle_workers.popleft()
+                        expired_worker.root_task.remove_done_callback(
+                            expired_worker.stop
+                        )
+                        expired_worker.stop()
+
+                context = copy_context()
+                context.run(sniffio.current_async_library_cvar.set, None)
+                worker.queue.put_nowait((context, func, args, future))
+                return await future
+
+    @classmethod
+    def run_async_from_thread(
+        cls,
+        func: Callable[..., Awaitable[T_Retval]],
+        args: tuple[Any, ...],
+        token: object,
+    ) -> T_Retval:
+        loop = cast(AbstractEventLoop, token)
+        context = copy_context()
+        context.run(sniffio.current_async_library_cvar.set, "asyncio")
+        f: concurrent.futures.Future[T_Retval] = context.run(
+            asyncio.run_coroutine_threadsafe, func(*args), loop
+        )
+        return f.result()
+
+    @classmethod
+    def run_sync_from_thread(
+        cls, func: Callable[..., T_Retval], args: tuple[Any, ...], token: object
+    ) -> T_Retval:
+        @wraps(func)
+        def wrapper() -> None:
+            try:
+                sniffio.current_async_library_cvar.set("asyncio")
+                f.set_result(func(*args))
+            except BaseException as exc:
+                f.set_exception(exc)
+                if not isinstance(exc, Exception):
+                    raise
+
+        f: concurrent.futures.Future[T_Retval] = Future()
+        loop = cast(AbstractEventLoop, token)
+        loop.call_soon_threadsafe(wrapper)
+        return f.result()
+
+    @classmethod
+    def create_blocking_portal(cls) -> abc.BlockingPortal:
+        return BlockingPortal()
+
+    @classmethod
+    async def open_process(
+        cls,
+        command: str | bytes | Sequence[str | bytes],
+        *,
+        shell: bool,
+        stdin: int | IO[Any] | None,
+        stdout: int | IO[Any] | None,
+        stderr: int | IO[Any] | None,
+        cwd: str | bytes | PathLike | None = None,
+        env: Mapping[str, str] | None = None,
+        start_new_session: bool = False,
+    ) -> Process:
+        await cls.checkpoint()
+        if shell:
+            process = await asyncio.create_subprocess_shell(
+                cast("str | bytes", command),
+                stdin=stdin,
+                stdout=stdout,
+                stderr=stderr,
+                cwd=cwd,
+                env=env,
+                start_new_session=start_new_session,
+            )
+        else:
+            process = await asyncio.create_subprocess_exec(
+                *command,
+                stdin=stdin,
+                stdout=stdout,
+                stderr=stderr,
+                cwd=cwd,
+                env=env,
+                start_new_session=start_new_session,
+            )
+
+        stdin_stream = StreamWriterWrapper(process.stdin) if process.stdin else None
+        stdout_stream = StreamReaderWrapper(process.stdout) if process.stdout else None
+        stderr_stream = StreamReaderWrapper(process.stderr) if process.stderr else None
+        return Process(process, stdin_stream, stdout_stream, stderr_stream)
+
+    @classmethod
+    def setup_process_pool_exit_at_shutdown(cls, workers: set[abc.Process]) -> None:
+        create_task(
+            _shutdown_process_pool_on_exit(workers),
+            name="AnyIO process pool shutdown task",
+        )
+        find_root_task().add_done_callback(
+            partial(_forcibly_shutdown_process_pool_on_exit, workers)
+        )
+
+    @classmethod
+    async def connect_tcp(
+        cls, host: str, port: int, local_address: IPSockAddrType | None = None
+    ) -> abc.SocketStream:
+        transport, protocol = cast(
+            Tuple[asyncio.Transport, StreamProtocol],
+            await get_running_loop().create_connection(
+                StreamProtocol, host, port, local_addr=local_address
+            ),
+        )
+        transport.pause_reading()
+        return SocketStream(transport, protocol)
+
+    @classmethod
+    async def connect_unix(cls, path: str) -> abc.UNIXSocketStream:
+        await cls.checkpoint()
+        loop = get_running_loop()
+        raw_socket = socket.socket(socket.AF_UNIX)
+        raw_socket.setblocking(False)
+        while True:
+            try:
+                raw_socket.connect(path)
+            except BlockingIOError:
+                f: asyncio.Future = asyncio.Future()
+                loop.add_writer(raw_socket, f.set_result, None)
+                f.add_done_callback(lambda _: loop.remove_writer(raw_socket))
+                await f
+            except BaseException:
+                raw_socket.close()
+                raise
+            else:
+                return UNIXSocketStream(raw_socket)
+
+    @classmethod
+    def create_tcp_listener(cls, sock: socket.socket) -> SocketListener:
+        return TCPSocketListener(sock)
+
+    @classmethod
+    def create_unix_listener(cls, sock: socket.socket) -> SocketListener:
+        return UNIXSocketListener(sock)
+
+    @classmethod
+    async def create_udp_socket(
+        cls,
+        family: AddressFamily,
+        local_address: IPSockAddrType | None,
+        remote_address: IPSockAddrType | None,
+        reuse_port: bool,
+    ) -> UDPSocket | ConnectedUDPSocket:
+        transport, protocol = await get_running_loop().create_datagram_endpoint(
+            DatagramProtocol,
+            local_addr=local_address,
+            remote_addr=remote_address,
+            family=family,
+            reuse_port=reuse_port,
+        )
+        if protocol.exception:
+            transport.close()
+            raise protocol.exception
+
+        if not remote_address:
+            return UDPSocket(transport, protocol)
+        else:
+            return ConnectedUDPSocket(transport, protocol)
+
+    @classmethod
+    async def create_unix_datagram_socket(  # type: ignore[override]
+        cls, raw_socket: socket.socket, remote_path: str | None
+    ) -> abc.UNIXDatagramSocket | abc.ConnectedUNIXDatagramSocket:
+        await cls.checkpoint()
+        loop = get_running_loop()
+
+        if remote_path:
+            while True:
+                try:
+                    raw_socket.connect(remote_path)
+                except BlockingIOError:
+                    f: asyncio.Future = asyncio.Future()
+                    loop.add_writer(raw_socket, f.set_result, None)
+                    f.add_done_callback(lambda _: loop.remove_writer(raw_socket))
+                    await f
+                except BaseException:
+                    raw_socket.close()
+                    raise
+                else:
+                    return ConnectedUNIXDatagramSocket(raw_socket)
+        else:
+            return UNIXDatagramSocket(raw_socket)
+
+    @classmethod
+    async def getaddrinfo(
+        cls,
+        host: bytes | str | None,
+        port: str | int | None,
+        *,
+        family: int | AddressFamily = 0,
+        type: int | SocketKind = 0,
+        proto: int = 0,
+        flags: int = 0,
+    ) -> list[
+        tuple[
+            AddressFamily,
+            SocketKind,
+            int,
+            str,
+            tuple[str, int] | tuple[str, int, int, int],
+        ]
+    ]:
+        return await get_running_loop().getaddrinfo(
+            host, port, family=family, type=type, proto=proto, flags=flags
+        )
+
+    @classmethod
+    async def getnameinfo(
+        cls, sockaddr: IPSockAddrType, flags: int = 0
+    ) -> tuple[str, str]:
+        return await get_running_loop().getnameinfo(sockaddr, flags)
+
+    @classmethod
+    async def wait_socket_readable(cls, sock: socket.socket) -> None:
+        await cls.checkpoint()
+        try:
+            read_events = _read_events.get()
+        except LookupError:
+            read_events = {}
+            _read_events.set(read_events)
+
+        if read_events.get(sock):
+            raise BusyResourceError("reading from") from None
+
+        loop = get_running_loop()
+        event = read_events[sock] = asyncio.Event()
+        loop.add_reader(sock, event.set)
+        try:
+            await event.wait()
+        finally:
+            if read_events.pop(sock, None) is not None:
+                loop.remove_reader(sock)
+                readable = True
+            else:
+                readable = False
+
+        if not readable:
+            raise ClosedResourceError
+
+    @classmethod
+    async def wait_socket_writable(cls, sock: socket.socket) -> None:
+        await cls.checkpoint()
+        try:
+            write_events = _write_events.get()
+        except LookupError:
+            write_events = {}
+            _write_events.set(write_events)
+
+        if write_events.get(sock):
+            raise BusyResourceError("writing to") from None
+
+        loop = get_running_loop()
+        event = write_events[sock] = asyncio.Event()
+        loop.add_writer(sock.fileno(), event.set)
+        try:
+            await event.wait()
+        finally:
+            if write_events.pop(sock, None) is not None:
+                loop.remove_writer(sock)
+                writable = True
+            else:
+                writable = False
+
+        if not writable:
+            raise ClosedResourceError
+
+    @classmethod
+    def current_default_thread_limiter(cls) -> CapacityLimiter:
+        try:
+            return _default_thread_limiter.get()
+        except LookupError:
+            limiter = CapacityLimiter(40)
+            _default_thread_limiter.set(limiter)
+            return limiter
+
+    @classmethod
+    def open_signal_receiver(
+        cls, *signals: Signals
+    ) -> ContextManager[AsyncIterator[Signals]]:
+        return _SignalReceiver(signals)
+
+    @classmethod
+    def get_current_task(cls) -> TaskInfo:
+        return _create_task_info(current_task())  # type: ignore[arg-type]
+
+    @classmethod
+    def get_running_tasks(cls) -> list[TaskInfo]:
+        return [_create_task_info(task) for task in all_tasks() if not task.done()]
+
+    @classmethod
+    async def wait_all_tasks_blocked(cls) -> None:
+        await cls.checkpoint()
+        this_task = current_task()
+        while True:
+            for task in all_tasks():
+                if task is this_task:
+                    continue
+
+                waiter = task._fut_waiter  # type: ignore[attr-defined]
+                if waiter is None or waiter.done():
+                    await sleep(0.1)
+                    break
+            else:
+                return
+
+    @classmethod
+    def create_test_runner(cls, options: dict[str, Any]) -> TestRunner:
+        return TestRunner(**options)
+
+
+backend_class = AsyncIOBackend
```

### Comparing `anyio-3.7.1/src/anyio/_backends/_trio.py` & `anyio-4.0.0rc1/src/anyio/_backends/_trio.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,88 @@
 from __future__ import annotations
 
 import array
 import math
 import socket
+import sys
+import types
+from collections.abc import AsyncIterator, Iterable
 from concurrent.futures import Future
-from contextvars import copy_context
 from dataclasses import dataclass
 from functools import partial
 from io import IOBase
 from os import PathLike
 from signal import Signals
+from socket import AddressFamily, SocketKind
 from types import TracebackType
 from typing import (
     IO,
-    TYPE_CHECKING,
     Any,
     AsyncGenerator,
-    AsyncIterator,
     Awaitable,
     Callable,
     Collection,
+    ContextManager,
     Coroutine,
     Generic,
-    Iterable,
     Mapping,
     NoReturn,
     Sequence,
     TypeVar,
     cast,
+    overload,
 )
 
-import sniffio
 import trio.from_thread
+import trio.lowlevel
 from outcome import Error, Outcome, Value
+from trio.lowlevel import (
+    TrioToken,
+    current_root_task,
+    current_task,
+    wait_readable,
+    wait_writable,
+)
 from trio.socket import SocketType as TrioSocketType
 from trio.to_thread import run_sync
 
 from .. import CapacityLimiterStatistics, EventStatistics, TaskInfo, abc
-from .._core._compat import DeprecatedAsyncContextManager, DeprecatedAwaitable
 from .._core._eventloop import claim_worker_thread
 from .._core._exceptions import (
     BrokenResourceError,
     BusyResourceError,
     ClosedResourceError,
     EndOfStream,
 )
-from .._core._exceptions import ExceptionGroup as BaseExceptionGroup
 from .._core._sockets import convert_ipv6_sockaddr
+from .._core._streams import create_memory_object_stream
 from .._core._synchronization import CapacityLimiter as BaseCapacityLimiter
 from .._core._synchronization import Event as BaseEvent
 from .._core._synchronization import ResourceGuard
 from .._core._tasks import CancelScope as BaseCancelScope
-from ..abc import IPSockAddrType, UDPPacketType
-
-if TYPE_CHECKING:
-    from trio_typing import TaskStatus
+from ..abc import IPSockAddrType, UDPPacketType, UNIXDatagramPacketType
+from ..abc._eventloop import AsyncBackend
+from ..streams.memory import MemoryObjectSendStream
 
-try:
-    from trio import lowlevel as trio_lowlevel
-except ImportError:
-    from trio import hazmat as trio_lowlevel  # type: ignore[no-redef]
-    from trio.hazmat import wait_readable, wait_writable
-else:
-    from trio.lowlevel import wait_readable, wait_writable
-
-try:
-    trio_open_process = trio_lowlevel.open_process
-except AttributeError:
-    # isort: off
-    from trio import (  # type: ignore[attr-defined, no-redef]
-        open_process as trio_open_process,
-    )
+if sys.version_info < (3, 11):
+    from exceptiongroup import BaseExceptionGroup
 
+T = TypeVar("T")
 T_Retval = TypeVar("T_Retval")
 T_SockAddr = TypeVar("T_SockAddr", str, IPSockAddrType)
 
 
 #
 # Event loop
 #
 
-run = trio.run
-current_token = trio.lowlevel.current_trio_token
 RunVar = trio.lowlevel.RunVar
 
 
 #
-# Miscellaneous
-#
-
-sleep = trio.sleep
-
-
-#
 # Timeouts and cancellation
 #
 
 
 class CancelScope(BaseCancelScope):
     def __new__(
         cls, original: trio.CancelScope | None = None, **kwargs: object
@@ -117,60 +103,51 @@
         exc_tb: TracebackType | None,
     ) -> bool | None:
         # https://github.com/python-trio/trio-typing/pull/79
         return self.__original.__exit__(  # type: ignore[func-returns-value]
             exc_type, exc_val, exc_tb
         )
 
-    def cancel(self) -> DeprecatedAwaitable:
+    def cancel(self) -> None:
         self.__original.cancel()
-        return DeprecatedAwaitable(self.cancel)
 
     @property
     def deadline(self) -> float:
         return self.__original.deadline
 
     @deadline.setter
     def deadline(self, value: float) -> None:
         self.__original.deadline = value
 
     @property
     def cancel_called(self) -> bool:
         return self.__original.cancel_called
 
     @property
+    def cancelled_caught(self) -> bool:
+        return self.__original.cancelled_caught
+
+    @property
     def shield(self) -> bool:
         return self.__original.shield
 
     @shield.setter
     def shield(self, value: bool) -> None:
         self.__original.shield = value
 
 
-CancelledError = trio.Cancelled
-checkpoint = trio.lowlevel.checkpoint
-checkpoint_if_cancelled = trio.lowlevel.checkpoint_if_cancelled
-cancel_shielded_checkpoint = trio.lowlevel.cancel_shielded_checkpoint
-current_effective_deadline = trio.current_effective_deadline
-current_time = trio.current_time
-
-
 #
 # Task groups
 #
 
 
-class ExceptionGroup(BaseExceptionGroup, trio.MultiError):
-    pass
-
-
 class TaskGroup(abc.TaskGroup):
     def __init__(self) -> None:
         self._active = False
-        self._nursery_manager = trio.open_nursery()
+        self._nursery_manager = trio.open_nursery(strict_exception_groups=True)
         self.cancel_scope = None  # type: ignore[assignment]
 
     async def __aenter__(self) -> TaskGroup:
         self._active = True
         self._nursery = await self._nursery_manager.__aenter__()
         self.cancel_scope = CancelScope(self._nursery.cancel_scope)
         return self
@@ -179,22 +156,25 @@
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> bool | None:
         try:
             return await self._nursery_manager.__aexit__(exc_type, exc_val, exc_tb)
-        except trio.MultiError as exc:
-            raise ExceptionGroup(exc.exceptions) from None
+        except BaseExceptionGroup as exc:
+            _, rest = exc.split(trio.Cancelled)
+            if not rest:
+                cancelled_exc = trio.Cancelled._create()  # type: ignore [attr-defined]
+                raise cancelled_exc from exc
+
+            raise
         finally:
             self._active = False
 
-    def start_soon(
-        self, func: Callable[..., Awaitable[Any]], *args: object, name: object = None
-    ) -> None:
+    def start_soon(self, func: Callable, *args: object, name: object = None) -> None:
         if not self._active:
             raise RuntimeError(
                 "This task group is not active; no new tasks can be started."
             )
 
         self._nursery.start_soon(func, *args, name=name)
 
@@ -210,61 +190,14 @@
 
 
 #
 # Threads
 #
 
 
-async def run_sync_in_worker_thread(
-    func: Callable[..., T_Retval],
-    *args: object,
-    cancellable: bool = False,
-    limiter: trio.CapacityLimiter | None = None,
-) -> T_Retval:
-    def wrapper() -> T_Retval:
-        with claim_worker_thread("trio"):
-            return func(*args)
-
-    # TODO: remove explicit context copying when trio 0.20 is the minimum requirement
-    context = copy_context()
-    context.run(sniffio.current_async_library_cvar.set, None)
-    return await run_sync(
-        context.run, wrapper, cancellable=cancellable, limiter=limiter
-    )
-
-
-# TODO: remove this workaround when trio 0.20 is the minimum requirement
-def run_async_from_thread(
-    fn: Callable[..., Awaitable[T_Retval]], *args: Any
-) -> T_Retval:
-    async def wrapper() -> T_Retval:
-        retval: T_Retval
-
-        async def inner() -> None:
-            nonlocal retval
-            __tracebackhide__ = True
-            retval = await fn(*args)
-
-        async with trio.open_nursery() as n:
-            context.run(n.start_soon, inner)
-
-        __tracebackhide__ = True
-        return retval  # noqa: F821
-
-    context = copy_context()
-    context.run(sniffio.current_async_library_cvar.set, "trio")
-    return trio.from_thread.run(wrapper)
-
-
-def run_sync_from_thread(fn: Callable[..., T_Retval], *args: Any) -> T_Retval:
-    # TODO: remove explicit context copying when trio 0.20 is the minimum requirement
-    retval = trio.from_thread.run_sync(copy_context().run, fn, *args)
-    return cast(T_Retval, retval)
-
-
 class BlockingPortal(abc.BlockingPortal):
     def __new__(cls) -> BlockingPortal:
         return object.__new__(cls)
 
     def __init__(self) -> None:
         super().__init__()
         self._token = trio.lowlevel.current_trio_token()
@@ -273,18 +206,15 @@
         self,
         func: Callable,
         args: tuple,
         kwargs: dict[str, Any],
         name: object,
         future: Future,
     ) -> None:
-        context = copy_context()
-        context.run(sniffio.current_async_library_cvar.set, "trio")
         trio.from_thread.run_sync(
-            context.run,
             partial(self._task_group.start_soon, name=name),
             self._call_func,
             func,
             args,
             kwargs,
             future,
             trio_token=self._token,
@@ -379,69 +309,37 @@
         return self._stdout
 
     @property
     def stderr(self) -> abc.ByteReceiveStream | None:
         return self._stderr
 
 
-async def open_process(
-    command: str | bytes | Sequence[str | bytes],
-    *,
-    shell: bool,
-    stdin: int | IO[Any] | None,
-    stdout: int | IO[Any] | None,
-    stderr: int | IO[Any] | None,
-    cwd: str | bytes | PathLike | None = None,
-    env: Mapping[str, str] | None = None,
-    start_new_session: bool = False,
-) -> Process:
-    process = await trio_open_process(  # type: ignore[misc]
-        command,  # type: ignore[arg-type]
-        stdin=stdin,
-        stdout=stdout,
-        stderr=stderr,
-        shell=shell,
-        cwd=cwd,
-        env=env,
-        start_new_session=start_new_session,
-    )
-    stdin_stream = SendStreamWrapper(process.stdin) if process.stdin else None
-    stdout_stream = ReceiveStreamWrapper(process.stdout) if process.stdout else None
-    stderr_stream = ReceiveStreamWrapper(process.stderr) if process.stderr else None
-    return Process(process, stdin_stream, stdout_stream, stderr_stream)
-
-
 class _ProcessPoolShutdownInstrument(trio.abc.Instrument):
     def after_run(self) -> None:
         super().after_run()
 
 
-current_default_worker_process_limiter: RunVar = RunVar(
+current_default_worker_process_limiter: trio.lowlevel.RunVar = RunVar(
     "current_default_worker_process_limiter"
 )
 
 
-async def _shutdown_process_pool(workers: set[Process]) -> None:
-    process: Process
+async def _shutdown_process_pool(workers: set[abc.Process]) -> None:
     try:
-        await sleep(math.inf)
+        await trio.sleep(math.inf)
     except trio.Cancelled:
         for process in workers:
             if process.returncode is None:
                 process.kill()
 
         with CancelScope(shield=True):
             for process in workers:
                 await process.aclose()
 
 
-def setup_process_pool_exit_at_shutdown(workers: set[Process]) -> None:
-    trio.lowlevel.spawn_system_task(_shutdown_process_pool, workers)
-
-
 #
 # Sockets and networking
 #
 
 
 class _TrioSocketMixin(Generic[T_SockAddr]):
     def __init__(self, trio_socket: TrioSocketType) -> None:
@@ -511,15 +409,15 @@
     async def receive_fds(self, msglen: int, maxfds: int) -> tuple[bytes, list[int]]:
         if not isinstance(msglen, int) or msglen < 0:
             raise ValueError("msglen must be a non-negative integer")
         if not isinstance(maxfds, int) or maxfds < 1:
             raise ValueError("maxfds must be a positive integer")
 
         fds = array.array("i")
-        await checkpoint()
+        await trio.lowlevel.checkpoint()
         with self._receive_guard:
             while True:
                 try:
                     message, ancdata, flags, addr = await self._trio_socket.recvmsg(
                         msglen, socket.CMSG_LEN(maxfds * fds.itemsize)
                     )
                 except BaseException as exc:
@@ -551,15 +449,15 @@
         for fd in fds:
             if isinstance(fd, int):
                 filenos.append(fd)
             elif isinstance(fd, IOBase):
                 filenos.append(fd.fileno())
 
         fdarray = array.array("i", filenos)
-        await checkpoint()
+        await trio.lowlevel.checkpoint()
         with self._send_guard:
             while True:
                 try:
                     await self._trio_socket.sendmsg(
                         [message],
                         [
                             (
@@ -644,84 +542,57 @@
         with self._send_guard:
             try:
                 await self._trio_socket.send(item)
             except BaseException as exc:
                 self._convert_socket_error(exc)
 
 
-async def connect_tcp(
-    host: str, port: int, local_address: IPSockAddrType | None = None
-) -> SocketStream:
-    family = socket.AF_INET6 if ":" in host else socket.AF_INET
-    trio_socket = trio.socket.socket(family)
-    trio_socket.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
-    if local_address:
-        await trio_socket.bind(local_address)
-
-    try:
-        await trio_socket.connect((host, port))
-    except BaseException:
-        trio_socket.close()
-        raise
-
-    return SocketStream(trio_socket)
-
-
-async def connect_unix(path: str) -> UNIXSocketStream:
-    trio_socket = trio.socket.socket(socket.AF_UNIX)
-    try:
-        await trio_socket.connect(path)
-    except BaseException:
-        trio_socket.close()
-        raise
-
-    return UNIXSocketStream(trio_socket)
-
-
-async def create_udp_socket(
-    family: socket.AddressFamily,
-    local_address: IPSockAddrType | None,
-    remote_address: IPSockAddrType | None,
-    reuse_port: bool,
-) -> UDPSocket | ConnectedUDPSocket:
-    trio_socket = trio.socket.socket(family=family, type=socket.SOCK_DGRAM)
-
-    if reuse_port:
-        trio_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
-
-    if local_address:
-        await trio_socket.bind(local_address)
-
-    if remote_address:
-        await trio_socket.connect(remote_address)
-        return ConnectedUDPSocket(trio_socket)
-    else:
-        return UDPSocket(trio_socket)
+class UNIXDatagramSocket(_TrioSocketMixin[str], abc.UNIXDatagramSocket):
+    def __init__(self, trio_socket: TrioSocketType) -> None:
+        super().__init__(trio_socket)
+        self._receive_guard = ResourceGuard("reading from")
+        self._send_guard = ResourceGuard("writing to")
 
+    async def receive(self) -> UNIXDatagramPacketType:
+        with self._receive_guard:
+            try:
+                data, addr = await self._trio_socket.recvfrom(65536)
+                return data, addr
+            except BaseException as exc:
+                self._convert_socket_error(exc)
 
-getaddrinfo = trio.socket.getaddrinfo
-getnameinfo = trio.socket.getnameinfo
+    async def send(self, item: UNIXDatagramPacketType) -> None:
+        with self._send_guard:
+            try:
+                await self._trio_socket.sendto(*item)
+            except BaseException as exc:
+                self._convert_socket_error(exc)
 
 
-async def wait_socket_readable(sock: socket.socket) -> None:
-    try:
-        await wait_readable(sock)
-    except trio.ClosedResourceError as exc:
-        raise ClosedResourceError().with_traceback(exc.__traceback__) from None
-    except trio.BusyResourceError:
-        raise BusyResourceError("reading from") from None
+class ConnectedUNIXDatagramSocket(
+    _TrioSocketMixin[str], abc.ConnectedUNIXDatagramSocket
+):
+    def __init__(self, trio_socket: TrioSocketType) -> None:
+        super().__init__(trio_socket)
+        self._receive_guard = ResourceGuard("reading from")
+        self._send_guard = ResourceGuard("writing to")
 
+    async def receive(self) -> bytes:
+        with self._receive_guard:
+            try:
+                return await self._trio_socket.recv(65536)
+            except BaseException as exc:
+                self._convert_socket_error(exc)
 
-async def wait_socket_writable(sock: socket.socket) -> None:
-    try:
-        await wait_writable(sock)
-    except trio.ClosedResourceError as exc:
-        raise ClosedResourceError().with_traceback(exc.__traceback__) from None
-    except trio.BusyResourceError:
-        raise BusyResourceError("writing to") from None
+    async def send(self, item: bytes) -> None:
+        with self._send_guard:
+            try:
+                await self._trio_socket.send(item)
+            except BaseException as exc:
+                self._convert_socket_error(exc)
 
 
 #
 # Synchronization
 #
 
 
@@ -738,17 +609,16 @@
     async def wait(self) -> None:
         return await self.__original.wait()
 
     def statistics(self) -> EventStatistics:
         orig_statistics = self.__original.statistics()
         return EventStatistics(tasks_waiting=orig_statistics.tasks_waiting)
 
-    def set(self) -> DeprecatedAwaitable:
+    def set(self) -> None:
         self.__original.set()
-        return DeprecatedAwaitable(self.set)
 
 
 class CapacityLimiter(BaseCapacityLimiter):
     def __new__(cls, *args: object, **kwargs: object) -> CapacityLimiter:
         return object.__new__(cls)
 
     def __init__(
@@ -779,21 +649,19 @@
     def borrowed_tokens(self) -> int:
         return self.__original.borrowed_tokens
 
     @property
     def available_tokens(self) -> float:
         return self.__original.available_tokens
 
-    def acquire_nowait(self) -> DeprecatedAwaitable:
+    def acquire_nowait(self) -> None:
         self.__original.acquire_nowait()
-        return DeprecatedAwaitable(self.acquire_nowait)
 
-    def acquire_on_behalf_of_nowait(self, borrower: object) -> DeprecatedAwaitable:
+    def acquire_on_behalf_of_nowait(self, borrower: object) -> None:
         self.__original.acquire_on_behalf_of_nowait(borrower)
-        return DeprecatedAwaitable(self.acquire_on_behalf_of_nowait)
 
     async def acquire(self) -> None:
         await self.__original.acquire()
 
     async def acquire_on_behalf_of(self, borrower: object) -> None:
         await self.__original.acquire_on_behalf_of(borrower)
 
@@ -809,34 +677,23 @@
             borrowed_tokens=orig.borrowed_tokens,
             total_tokens=orig.total_tokens,
             borrowers=orig.borrowers,
             tasks_waiting=orig.tasks_waiting,
         )
 
 
-_capacity_limiter_wrapper: RunVar = RunVar("_capacity_limiter_wrapper")
-
-
-def current_default_thread_limiter() -> CapacityLimiter:
-    try:
-        return _capacity_limiter_wrapper.get()
-    except LookupError:
-        limiter = CapacityLimiter(
-            original=trio.to_thread.current_default_thread_limiter()
-        )
-        _capacity_limiter_wrapper.set(limiter)
-        return limiter
+_capacity_limiter_wrapper: trio.lowlevel.RunVar = RunVar("_capacity_limiter_wrapper")
 
 
 #
 # Signal handling
 #
 
 
-class _SignalReceiver(DeprecatedAsyncContextManager["_SignalReceiver"]):
+class _SignalReceiver:
     _iterator: AsyncIterator[int]
 
     def __init__(self, signals: tuple[Signals, ...]):
         self._signals = signals
 
     def __enter__(self) -> _SignalReceiver:
         self._cm = trio.open_signal_receiver(*self._signals)
@@ -855,142 +712,416 @@
         return self
 
     async def __anext__(self) -> Signals:
         signum = await self._iterator.__anext__()
         return Signals(signum)
 
 
-def open_signal_receiver(*signals: Signals) -> _SignalReceiver:
-    return _SignalReceiver(signals)
-
-
 #
 # Testing and debugging
 #
 
 
-def get_current_task() -> TaskInfo:
-    task = trio_lowlevel.current_task()
-
-    parent_id = None
-    if task.parent_nursery and task.parent_nursery.parent_task:
-        parent_id = id(task.parent_nursery.parent_task)
-
-    return TaskInfo(id(task), parent_id, task.name, task.coro)
-
-
-def get_running_tasks() -> list[TaskInfo]:
-    root_task = trio_lowlevel.current_root_task()
-    task_infos = [TaskInfo(id(root_task), None, root_task.name, root_task.coro)]
-    nurseries = root_task.child_nurseries
-    while nurseries:
-        new_nurseries: list[trio.Nursery] = []
-        for nursery in nurseries:
-            for task in nursery.child_tasks:
-                task_infos.append(
-                    TaskInfo(id(task), id(nursery.parent_task), task.name, task.coro)
-                )
-                new_nurseries.extend(task.child_nurseries)
-
-        nurseries = new_nurseries
-
-    return task_infos
-
-
-def wait_all_tasks_blocked() -> Awaitable[None]:
-    import trio.testing
-
-    return trio.testing.wait_all_tasks_blocked()
-
-
 class TestRunner(abc.TestRunner):
     def __init__(self, **options: Any) -> None:
-        from collections import deque
         from queue import Queue
 
         self._call_queue: Queue[Callable[..., object]] = Queue()
-        self._result_queue: deque[Outcome] = deque()
-        self._stop_event: trio.Event | None = None
-        self._nursery: trio.Nursery | None = None
+        self._send_stream: MemoryObjectSendStream | None = None
         self._options = options
 
-    async def _trio_main(self) -> None:
-        self._stop_event = trio.Event()
-        async with trio.open_nursery() as self._nursery:
-            await self._stop_event.wait()
-
-    async def _call_func(
-        self, func: Callable[..., Awaitable[object]], args: tuple, kwargs: dict
+    def __exit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: types.TracebackType | None,
     ) -> None:
-        try:
-            retval = await func(*args, **kwargs)
-        except BaseException as exc:
-            self._result_queue.append(Error(exc))
-        else:
-            self._result_queue.append(Value(retval))
+        if self._send_stream:
+            self._send_stream.close()
+            while self._send_stream is not None:
+                self._call_queue.get()()
+
+    async def _run_tests_and_fixtures(self) -> None:
+        self._send_stream, receive_stream = create_memory_object_stream(1)
+        with receive_stream:
+            async for coro, outcome_holder in receive_stream:
+                try:
+                    retval = await coro
+                except BaseException as exc:
+                    outcome_holder.append(Error(exc))
+                else:
+                    outcome_holder.append(Value(retval))
 
     def _main_task_finished(self, outcome: object) -> None:
-        self._nursery = None
+        self._send_stream = None
 
-    def _get_nursery(self) -> trio.Nursery:
-        if self._nursery is None:
+    def _call_in_runner_task(
+        self, func: Callable[..., Awaitable[T_Retval]], *args: object, **kwargs: object
+    ) -> T_Retval:
+        if self._send_stream is None:
             trio.lowlevel.start_guest_run(
-                self._trio_main,
+                self._run_tests_and_fixtures,
                 run_sync_soon_threadsafe=self._call_queue.put,
                 done_callback=self._main_task_finished,
                 **self._options,
             )
-            while self._nursery is None:
+            while self._send_stream is None:
                 self._call_queue.get()()
 
-        return self._nursery
-
-    def _call(
-        self, func: Callable[..., Awaitable[T_Retval]], *args: object, **kwargs: object
-    ) -> T_Retval:
-        self._get_nursery().start_soon(self._call_func, func, args, kwargs)
-        while not self._result_queue:
+        outcome_holder: list[Outcome] = []
+        self._send_stream.send_nowait((func(*args, **kwargs), outcome_holder))
+        while not outcome_holder:
             self._call_queue.get()()
 
-        outcome = self._result_queue.pop()
-        return outcome.unwrap()
-
-    def close(self) -> None:
-        if self._stop_event:
-            self._stop_event.set()
-            while self._nursery is not None:
-                self._call_queue.get()()
+        return outcome_holder[0].unwrap()
 
     def run_asyncgen_fixture(
         self,
         fixture_func: Callable[..., AsyncGenerator[T_Retval, Any]],
         kwargs: dict[str, Any],
     ) -> Iterable[T_Retval]:
-        async def fixture_runner(*, task_status: TaskStatus[T_Retval]) -> None:
-            agen = fixture_func(**kwargs)
-            retval = await agen.asend(None)
-            task_status.started(retval)
-            await teardown_event.wait()
-            try:
-                await agen.asend(None)
-            except StopAsyncIteration:
-                pass
-            else:
-                await agen.aclose()
-                raise RuntimeError("Async generator fixture did not stop")
+        asyncgen = fixture_func(**kwargs)
+        fixturevalue: T_Retval = self._call_in_runner_task(asyncgen.asend, None)
+
+        yield fixturevalue
 
-        teardown_event = trio.Event()
-        fixture_value = self._call(lambda: self._get_nursery().start(fixture_runner))
-        yield fixture_value
-        teardown_event.set()
+        try:
+            self._call_in_runner_task(asyncgen.asend, None)
+        except StopAsyncIteration:
+            pass
+        else:
+            self._call_in_runner_task(asyncgen.aclose)
+            raise RuntimeError("Async generator fixture did not stop")
 
     def run_fixture(
         self,
         fixture_func: Callable[..., Coroutine[Any, Any, T_Retval]],
         kwargs: dict[str, Any],
     ) -> T_Retval:
-        return self._call(fixture_func, **kwargs)
+        return self._call_in_runner_task(fixture_func, **kwargs)
 
     def run_test(
         self, test_func: Callable[..., Coroutine[Any, Any, Any]], kwargs: dict[str, Any]
     ) -> None:
-        self._call(test_func, **kwargs)
+        self._call_in_runner_task(test_func, **kwargs)
+
+
+class TrioBackend(AsyncBackend):
+    @classmethod
+    def run(
+        cls,
+        func: Callable[..., Awaitable[T_Retval]],
+        args: tuple,
+        kwargs: dict[str, Any],
+        options: dict[str, Any],
+    ) -> T_Retval:
+        return trio.run(func, *args)
+
+    @classmethod
+    def current_token(cls) -> object:
+        return trio.lowlevel.current_trio_token()
+
+    @classmethod
+    def current_time(cls) -> float:
+        return trio.current_time()
+
+    @classmethod
+    def cancelled_exception_class(cls) -> type[BaseException]:
+        return trio.Cancelled
+
+    @classmethod
+    async def checkpoint(cls) -> None:
+        await trio.lowlevel.checkpoint()
+
+    @classmethod
+    async def checkpoint_if_cancelled(cls) -> None:
+        await trio.lowlevel.checkpoint_if_cancelled()
+
+    @classmethod
+    async def cancel_shielded_checkpoint(cls) -> None:
+        await trio.lowlevel.cancel_shielded_checkpoint()
+
+    @classmethod
+    async def sleep(cls, delay: float) -> None:
+        await trio.sleep(delay)
+
+    @classmethod
+    def create_cancel_scope(
+        cls, *, deadline: float = math.inf, shield: bool = False
+    ) -> abc.CancelScope:
+        return CancelScope(deadline=deadline, shield=shield)
+
+    @classmethod
+    def current_effective_deadline(cls) -> float:
+        return trio.current_effective_deadline()
+
+    @classmethod
+    def create_task_group(cls) -> abc.TaskGroup:
+        return TaskGroup()
+
+    @classmethod
+    def create_event(cls) -> abc.Event:
+        return Event()
+
+    @classmethod
+    def create_capacity_limiter(cls, total_tokens: float) -> CapacityLimiter:
+        return CapacityLimiter(total_tokens)
+
+    @classmethod
+    async def run_sync_in_worker_thread(
+        cls,
+        func: Callable[..., T_Retval],
+        args: tuple[Any, ...],
+        cancellable: bool = False,
+        limiter: abc.CapacityLimiter | None = None,
+    ) -> T_Retval:
+        def wrapper() -> T_Retval:
+            with claim_worker_thread(TrioBackend, token):
+                return func(*args)
+
+        token = TrioBackend.current_token()
+        return await run_sync(
+            wrapper,
+            cancellable=cancellable,
+            limiter=cast(trio.CapacityLimiter, limiter),
+        )
+
+    @classmethod
+    def run_async_from_thread(
+        cls,
+        func: Callable[..., Awaitable[T_Retval]],
+        args: tuple[Any, ...],
+        token: object,
+    ) -> T_Retval:
+        return trio.from_thread.run(func, *args, trio_token=cast(TrioToken, token))
+
+    @classmethod
+    def run_sync_from_thread(
+        cls, func: Callable[..., T_Retval], args: tuple[Any, ...], token: object
+    ) -> T_Retval:
+        return trio.from_thread.run_sync(func, *args, trio_token=cast(TrioToken, token))
+
+    @classmethod
+    def create_blocking_portal(cls) -> abc.BlockingPortal:
+        return BlockingPortal()
+
+    @classmethod
+    async def open_process(
+        cls,
+        command: str | bytes | Sequence[str | bytes],
+        *,
+        shell: bool,
+        stdin: int | IO[Any] | None,
+        stdout: int | IO[Any] | None,
+        stderr: int | IO[Any] | None,
+        cwd: str | bytes | PathLike | None = None,
+        env: Mapping[str, str] | None = None,
+        start_new_session: bool = False,
+    ) -> Process:
+        process = await trio.lowlevel.open_process(  # type: ignore[misc]
+            command,  # type: ignore[arg-type]
+            stdin=stdin,
+            stdout=stdout,
+            stderr=stderr,
+            shell=shell,
+            cwd=cwd,
+            env=env,
+            start_new_session=start_new_session,
+        )
+        stdin_stream = SendStreamWrapper(process.stdin) if process.stdin else None
+        stdout_stream = ReceiveStreamWrapper(process.stdout) if process.stdout else None
+        stderr_stream = ReceiveStreamWrapper(process.stderr) if process.stderr else None
+        return Process(process, stdin_stream, stdout_stream, stderr_stream)
+
+    @classmethod
+    def setup_process_pool_exit_at_shutdown(cls, workers: set[abc.Process]) -> None:
+        trio.lowlevel.spawn_system_task(_shutdown_process_pool, workers)
+
+    @classmethod
+    async def connect_tcp(
+        cls, host: str, port: int, local_address: IPSockAddrType | None = None
+    ) -> SocketStream:
+        family = socket.AF_INET6 if ":" in host else socket.AF_INET
+        trio_socket = trio.socket.socket(family)
+        trio_socket.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
+        if local_address:
+            await trio_socket.bind(local_address)
+
+        try:
+            await trio_socket.connect((host, port))
+        except BaseException:
+            trio_socket.close()
+            raise
+
+        return SocketStream(trio_socket)
+
+    @classmethod
+    async def connect_unix(cls, path: str) -> abc.UNIXSocketStream:
+        trio_socket = trio.socket.socket(socket.AF_UNIX)
+        try:
+            await trio_socket.connect(path)
+        except BaseException:
+            trio_socket.close()
+            raise
+
+        return UNIXSocketStream(trio_socket)
+
+    @classmethod
+    def create_tcp_listener(cls, sock: socket.socket) -> abc.SocketListener:
+        return TCPSocketListener(sock)
+
+    @classmethod
+    def create_unix_listener(cls, sock: socket.socket) -> abc.SocketListener:
+        return UNIXSocketListener(sock)
+
+    @classmethod
+    async def create_udp_socket(
+        cls,
+        family: socket.AddressFamily,
+        local_address: IPSockAddrType | None,
+        remote_address: IPSockAddrType | None,
+        reuse_port: bool,
+    ) -> UDPSocket | ConnectedUDPSocket:
+        trio_socket = trio.socket.socket(family=family, type=socket.SOCK_DGRAM)
+
+        if reuse_port:
+            trio_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
+
+        if local_address:
+            await trio_socket.bind(local_address)
+
+        if remote_address:
+            await trio_socket.connect(remote_address)
+            return ConnectedUDPSocket(trio_socket)
+        else:
+            return UDPSocket(trio_socket)
+
+    @classmethod
+    @overload
+    async def create_unix_datagram_socket(
+        cls, raw_socket: socket.socket, remote_path: None
+    ) -> abc.UNIXDatagramSocket:
+        ...
+
+    @classmethod
+    @overload
+    async def create_unix_datagram_socket(
+        cls, raw_socket: socket.socket, remote_path: str
+    ) -> abc.ConnectedUNIXDatagramSocket:
+        ...
+
+    @classmethod
+    async def create_unix_datagram_socket(
+        cls, raw_socket: socket.socket, remote_path: str | None
+    ) -> abc.UNIXDatagramSocket | abc.ConnectedUNIXDatagramSocket:
+        trio_socket = trio.socket.from_stdlib_socket(raw_socket)
+
+        if remote_path:
+            await trio_socket.connect(remote_path)
+            return ConnectedUNIXDatagramSocket(trio_socket)
+        else:
+            return UNIXDatagramSocket(trio_socket)
+
+    @classmethod
+    async def getaddrinfo(
+        cls,
+        host: bytes | str | None,
+        port: str | int | None,
+        *,
+        family: int | AddressFamily = 0,
+        type: int | SocketKind = 0,
+        proto: int = 0,
+        flags: int = 0,
+    ) -> list[
+        tuple[
+            AddressFamily,
+            SocketKind,
+            int,
+            str,
+            tuple[str, int] | tuple[str, int, int, int],
+        ]
+    ]:
+        return await trio.socket.getaddrinfo(host, port, family, type, proto, flags)
+
+    @classmethod
+    async def getnameinfo(
+        cls, sockaddr: IPSockAddrType, flags: int = 0
+    ) -> tuple[str, str]:
+        return await trio.socket.getnameinfo(sockaddr, flags)
+
+    @classmethod
+    async def wait_socket_readable(cls, sock: socket.socket) -> None:
+        try:
+            await wait_readable(sock)  # type: ignore[arg-type]
+        except trio.ClosedResourceError as exc:
+            raise ClosedResourceError().with_traceback(exc.__traceback__) from None
+        except trio.BusyResourceError:
+            raise BusyResourceError("reading from") from None
+
+    @classmethod
+    async def wait_socket_writable(cls, sock: socket.socket) -> None:
+        try:
+            await wait_writable(sock)  # type: ignore[arg-type]
+        except trio.ClosedResourceError as exc:
+            raise ClosedResourceError().with_traceback(exc.__traceback__) from None
+        except trio.BusyResourceError:
+            raise BusyResourceError("writing to") from None
+
+    @classmethod
+    def current_default_thread_limiter(cls) -> CapacityLimiter:
+        try:
+            return _capacity_limiter_wrapper.get()
+        except LookupError:
+            limiter = CapacityLimiter(
+                original=trio.to_thread.current_default_thread_limiter()
+            )
+            _capacity_limiter_wrapper.set(limiter)
+            return limiter
+
+    @classmethod
+    def open_signal_receiver(
+        cls, *signals: Signals
+    ) -> ContextManager[AsyncIterator[Signals]]:
+        return _SignalReceiver(signals)
+
+    @classmethod
+    def get_current_task(cls) -> TaskInfo:
+        task = current_task()
+
+        parent_id = None
+        if task.parent_nursery and task.parent_nursery.parent_task:
+            parent_id = id(task.parent_nursery.parent_task)
+
+        return TaskInfo(id(task), parent_id, task.name, task.coro)
+
+    @classmethod
+    def get_running_tasks(cls) -> list[TaskInfo]:
+        root_task = current_root_task()
+        task_infos = [TaskInfo(id(root_task), None, root_task.name, root_task.coro)]
+        nurseries = root_task.child_nurseries
+        while nurseries:
+            new_nurseries: list[trio.Nursery] = []
+            for nursery in nurseries:
+                for task in nursery.child_tasks:
+                    task_infos.append(
+                        TaskInfo(
+                            id(task), id(nursery.parent_task), task.name, task.coro
+                        )
+                    )
+                    new_nurseries.extend(task.child_nurseries)
+
+            nurseries = new_nurseries
+
+        return task_infos
+
+    @classmethod
+    async def wait_all_tasks_blocked(cls) -> None:
+        from trio.testing import wait_all_tasks_blocked
+
+        await wait_all_tasks_blocked()
+
+    @classmethod
+    def create_test_runner(cls, options: dict[str, Any]) -> TestRunner:
+        return TestRunner(**options)
+
+
+backend_class = TrioBackend
```

### Comparing `anyio-3.7.1/src/anyio/_core/_eventloop.py` & `anyio-4.0.0rc1/src/anyio/_core/_eventloop.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from __future__ import annotations
 
 import math
 import sys
 import threading
+from collections.abc import Awaitable, Callable, Generator
 from contextlib import contextmanager
 from importlib import import_module
-from typing import (
-    Any,
-    Awaitable,
-    Callable,
-    Generator,
-    TypeVar,
-)
+from typing import TYPE_CHECKING, Any, TypeVar
 
 import sniffio
 
-# This must be updated when new backends are introduced
-from ._compat import DeprecatedAwaitableFloat
+if TYPE_CHECKING:
+    from ..abc import AsyncBackend
 
+# This must be updated when new backends are introduced
 BACKENDS = "asyncio", "trio"
 
 T_Retval = TypeVar("T_Retval")
 threadlocals = threading.local()
 
 
 def run(
@@ -33,56 +29,58 @@
     """
     Run the given coroutine function in an asynchronous event loop.
 
     The current thread must not be already running an event loop.
 
     :param func: a coroutine function
     :param args: positional arguments to ``func``
-    :param backend: name of the asynchronous event loop implementation – currently either
-        ``asyncio`` or ``trio``
-    :param backend_options: keyword arguments to call the backend ``run()`` implementation with
-        (documented :ref:`here <backend options>`)
+    :param backend: name of the asynchronous event loop implementation – currently
+        either ``asyncio`` or ``trio``
+    :param backend_options: keyword arguments to call the backend ``run()``
+        implementation with (documented :ref:`here <backend options>`)
     :return: the return value of the coroutine function
-    :raises RuntimeError: if an asynchronous event loop is already running in this thread
+    :raises RuntimeError: if an asynchronous event loop is already running in this
+        thread
     :raises LookupError: if the named backend is not found
 
     """
     try:
         asynclib_name = sniffio.current_async_library()
     except sniffio.AsyncLibraryNotFoundError:
         pass
     else:
         raise RuntimeError(f"Already running {asynclib_name} in this thread")
 
     try:
-        asynclib = import_module(f"..._backends._{backend}", package=__name__)
+        async_backend = get_async_backend(backend)
     except ImportError as exc:
         raise LookupError(f"No such backend: {backend}") from exc
 
     token = None
     if sniffio.current_async_library_cvar.get(None) is None:
-        # Since we're in control of the event loop, we can cache the name of the async library
+        # Since we're in control of the event loop, we can cache the name of the async
+        # library
         token = sniffio.current_async_library_cvar.set(backend)
 
     try:
         backend_options = backend_options or {}
-        return asynclib.run(func, *args, **backend_options)
+        return async_backend.run(func, args, {}, backend_options)
     finally:
         if token:
             sniffio.current_async_library_cvar.reset(token)
 
 
 async def sleep(delay: float) -> None:
     """
     Pause the current task for the specified duration.
 
     :param delay: the duration, in seconds
 
     """
-    return await get_asynclib().sleep(delay)
+    return await get_async_backend().sleep(delay)
 
 
 async def sleep_forever() -> None:
     """
     Pause the current task until it's cancelled.
 
     This is a shortcut for ``sleep(math.inf)``.
@@ -93,61 +91,66 @@
     await sleep(math.inf)
 
 
 async def sleep_until(deadline: float) -> None:
     """
     Pause the current task until the given time.
 
-    :param deadline: the absolute time to wake up at (according to the internal monotonic clock of
-        the event loop)
+    :param deadline: the absolute time to wake up at (according to the internal
+        monotonic clock of the event loop)
 
     .. versionadded:: 3.1
 
     """
     now = current_time()
     await sleep(max(deadline - now, 0))
 
 
-def current_time() -> DeprecatedAwaitableFloat:
+def current_time() -> float:
     """
     Return the current value of the event loop's internal clock.
 
     :return: the clock value (seconds)
 
     """
-    return DeprecatedAwaitableFloat(get_asynclib().current_time(), current_time)
+    return get_async_backend().current_time()
 
 
 def get_all_backends() -> tuple[str, ...]:
     """Return a tuple of the names of all built-in backends."""
     return BACKENDS
 
 
 def get_cancelled_exc_class() -> type[BaseException]:
     """Return the current async library's cancellation exception class."""
-    return get_asynclib().CancelledError
+    return get_async_backend().cancelled_exception_class()
 
 
 #
 # Private API
 #
 
 
 @contextmanager
-def claim_worker_thread(backend: str) -> Generator[Any, None, None]:
-    module = sys.modules["anyio._backends._" + backend]
-    threadlocals.current_async_module = module
+def claim_worker_thread(
+    backend_class: type[AsyncBackend], token: object
+) -> Generator[Any, None, None]:
+    threadlocals.current_async_backend = backend_class
+    threadlocals.current_token = token
     try:
         yield
     finally:
-        del threadlocals.current_async_module
+        del threadlocals.current_async_backend
+        del threadlocals.current_token
 
 
-def get_asynclib(asynclib_name: str | None = None) -> Any:
+def get_async_backend(asynclib_name: str | None = None) -> AsyncBackend:
     if asynclib_name is None:
         asynclib_name = sniffio.current_async_library()
 
     modulename = "anyio._backends._" + asynclib_name
     try:
-        return sys.modules[modulename]
+        module = sys.modules[modulename]
     except KeyError:
-        return import_module(modulename)
+        module = import_module(modulename)
+
+    return getattr(module, "backend_class")
```

### Comparing `anyio-3.7.1/src/anyio/_core/_exceptions.py` & `anyio-4.0.0rc1/src/anyio/_core/_exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,73 @@
 from __future__ import annotations
 
-from traceback import format_exception
-
 
 class BrokenResourceError(Exception):
     """
-    Raised when trying to use a resource that has been rendered unusable due to external causes
-    (e.g. a send stream whose peer has disconnected).
+    Raised when trying to use a resource that has been rendered unusable due to external
+    causes (e.g. a send stream whose peer has disconnected).
     """
 
 
 class BrokenWorkerProcess(Exception):
     """
-    Raised by :func:`run_sync_in_process` if the worker process terminates abruptly or otherwise
-    misbehaves.
+    Raised by :func:`run_sync_in_process` if the worker process terminates abruptly or
+    otherwise misbehaves.
     """
 
 
 class BusyResourceError(Exception):
-    """Raised when two tasks are trying to read from or write to the same resource concurrently."""
+    """
+    Raised when two tasks are trying to read from or write to the same resource
+    concurrently.
+    """
 
     def __init__(self, action: str):
         super().__init__(f"Another task is already {action} this resource")
 
 
 class ClosedResourceError(Exception):
     """Raised when trying to use a resource that has been closed."""
 
 
 class DelimiterNotFound(Exception):
     """
-    Raised during :meth:`~anyio.streams.buffered.BufferedByteReceiveStream.receive_until` if the
+    Raised during
+    :meth:`~anyio.streams.buffered.BufferedByteReceiveStream.receive_until` if the
     maximum number of bytes has been read without the delimiter being found.
     """
 
     def __init__(self, max_bytes: int) -> None:
         super().__init__(
             f"The delimiter was not found among the first {max_bytes} bytes"
         )
 
 
 class EndOfStream(Exception):
-    """Raised when trying to read from a stream that has been closed from the other end."""
-
-
-class ExceptionGroup(BaseException):
     """
-    Raised when multiple exceptions have been raised in a task group.
-
-    :var ~typing.Sequence[BaseException] exceptions: the sequence of exceptions raised together
+    Raised when trying to read from a stream that has been closed from the other end.
     """
 
-    SEPARATOR = "----------------------------\n"
-
-    exceptions: list[BaseException]
-
-    def __str__(self) -> str:
-        tracebacks = [
-            "".join(format_exception(type(exc), exc, exc.__traceback__))
-            for exc in self.exceptions
-        ]
-        return (
-            f"{len(self.exceptions)} exceptions were raised in the task group:\n"
-            f"{self.SEPARATOR}{self.SEPARATOR.join(tracebacks)}"
-        )
-
-    def __repr__(self) -> str:
-        exception_reprs = ", ".join(repr(exc) for exc in self.exceptions)
-        return f"<{self.__class__.__name__}: {exception_reprs}>"
-
 
 class IncompleteRead(Exception):
     """
-    Raised during :meth:`~anyio.streams.buffered.BufferedByteReceiveStream.receive_exactly` or
+    Raised during
+    :meth:`~anyio.streams.buffered.BufferedByteReceiveStream.receive_exactly` or
     :meth:`~anyio.streams.buffered.BufferedByteReceiveStream.receive_until` if the
     connection is closed before the requested amount of bytes has been read.
     """
 
     def __init__(self) -> None:
         super().__init__(
             "The stream was closed before the read operation could be completed"
         )
 
 
 class TypedAttributeLookupError(LookupError):
     """
-    Raised by :meth:`~anyio.TypedAttributeProvider.extra` when the given typed attribute is not
-    found and no default value has been given.
+    Raised by :meth:`~anyio.TypedAttributeProvider.extra` when the given typed attribute
+    is not found and no default value has been given.
     """
 
 
 class WouldBlock(Exception):
     """Raised by ``X_nowait`` functions if ``X()`` would block."""
```

### Comparing `anyio-3.7.1/src/anyio/_core/_fileio.py` & `anyio-4.0.0rc1/src/anyio/_core/_fileio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,50 +1,43 @@
 from __future__ import annotations
 
 import os
 import pathlib
 import sys
+from collections.abc import Callable, Iterable, Iterator, Sequence
 from dataclasses import dataclass
 from functools import partial
 from os import PathLike
 from typing import (
     IO,
     TYPE_CHECKING,
     Any,
     AnyStr,
     AsyncIterator,
-    Callable,
+    Final,
     Generic,
-    Iterable,
-    Iterator,
-    Sequence,
     cast,
     overload,
 )
 
 from .. import to_thread
 from ..abc import AsyncResource
 
-if sys.version_info >= (3, 8):
-    from typing import Final
-else:
-    from typing_extensions import Final
-
 if TYPE_CHECKING:
     from _typeshed import OpenBinaryMode, OpenTextMode, ReadableBuffer, WriteableBuffer
 else:
     ReadableBuffer = OpenBinaryMode = OpenTextMode = WriteableBuffer = object
 
 
 class AsyncFile(AsyncResource, Generic[AnyStr]):
     """
     An asynchronous file object.
 
-    This class wraps a standard file object and provides async friendly versions of the following
-    blocking methods (where available on the original file object):
+    This class wraps a standard file object and provides async friendly versions of the
+    following blocking methods (where available on the original file object):
 
     * read
     * read1
     * readline
     * readlines
     * readinto
     * readinto1
@@ -53,16 +46,16 @@
     * truncate
     * seek
     * tell
     * flush
 
     All other methods are directly passed through.
 
-    This class supports the asynchronous context manager protocol which closes the underlying file
-    at the end of the context block.
+    This class supports the asynchronous context manager protocol which closes the
+    underlying file at the end of the context block.
 
     This class also supports asynchronous iteration::
 
         async with await open_file(...) as f:
             async for line in f:
                 print(line)
     """
@@ -219,19 +212,20 @@
         return Path(cast("PathLike[str]", nextval))
 
 
 class Path:
     """
     An asynchronous version of :class:`pathlib.Path`.
 
-    This class cannot be substituted for :class:`pathlib.Path` or :class:`pathlib.PurePath`, but
-    it is compatible with the :class:`os.PathLike` interface.
+    This class cannot be substituted for :class:`pathlib.Path` or
+    :class:`pathlib.PurePath`, but it is compatible with the :class:`os.PathLike`
+    interface.
 
-    It implements the Python 3.10 version of :class:`pathlib.Path` interface, except for the
-    deprecated :meth:`~pathlib.Path.link_to` method.
+    It implements the Python 3.10 version of :class:`pathlib.Path` interface, except for
+    the deprecated :meth:`~pathlib.Path.link_to` method.
 
     Any methods that do disk I/O need to be awaited on. These methods are:
 
     * :meth:`~pathlib.Path.absolute`
     * :meth:`~pathlib.Path.chmod`
     * :meth:`~pathlib.Path.cwd`
     * :meth:`~pathlib.Path.exists`
@@ -259,15 +253,16 @@
     * :meth:`~pathlib.Path.samefile`
     * :meth:`~pathlib.Path.stat`
     * :meth:`~pathlib.Path.touch`
     * :meth:`~pathlib.Path.unlink`
     * :meth:`~pathlib.Path.write_bytes`
     * :meth:`~pathlib.Path.write_text`
 
-    Additionally, the following methods return an async iterator yielding :class:`~.Path` objects:
+    Additionally, the following methods return an async iterator yielding
+    :class:`~.Path` objects:
 
     * :meth:`~pathlib.Path.glob`
     * :meth:`~pathlib.Path.iterdir`
     * :meth:`~pathlib.Path.rglob`
     """
 
     __slots__ = "_path", "__weakref__"
@@ -367,21 +362,26 @@
 
     def as_uri(self) -> str:
         return self._path.as_uri()
 
     def match(self, path_pattern: str) -> bool:
         return self._path.match(path_pattern)
 
-    def is_relative_to(self, *other: str | PathLike[str]) -> bool:
+    def is_relative_to(self, other: str | PathLike[str]) -> bool:
         try:
-            self.relative_to(*other)
+            self.relative_to(other)
             return True
         except ValueError:
             return False
 
+    async def is_junction(self) -> bool:
+        return await to_thread.run_sync(
+            self._path.is_junction  # type: ignore [attr-defined]
+        )
+
     async def chmod(self, mode: int, *, follow_symlinks: bool = True) -> None:
         func = partial(os.chmod, follow_symlinks=follow_symlinks)
         return await to_thread.run_sync(func, self._path, mode)
 
     @classmethod
     async def cwd(cls) -> Path:
         path = await to_thread.run_sync(pathlib.Path.cwd)
@@ -567,23 +567,49 @@
     async def unlink(self, missing_ok: bool = False) -> None:
         try:
             await to_thread.run_sync(self._path.unlink)
         except FileNotFoundError:
             if not missing_ok:
                 raise
 
+    if sys.version_info >= (3, 12):
+
+        async def walk(
+            self,
+            top_down: bool = True,
+            on_error: Callable[[OSError], object] | None = None,
+            follow_symlinks: bool = False,
+        ) -> AsyncIterator[tuple[Path, list[str], list[str]]]:
+            def get_next_value() -> tuple[pathlib.Path, list[str], list[str]] | None:
+                try:
+                    return next(gen)
+                except StopIteration:
+                    return None
+
+            gen = self._path.walk(top_down, on_error, follow_symlinks)
+            while True:
+                value = await to_thread.run_sync(get_next_value)
+                if value is None:
+                    return
+
+                root, dirs, paths = value
+                yield Path(root), dirs, paths
+
     def with_name(self, name: str) -> Path:
         return Path(self._path.with_name(name))
 
     def with_stem(self, stem: str) -> Path:
         return Path(self._path.with_name(stem + self._path.suffix))
 
     def with_suffix(self, suffix: str) -> Path:
         return Path(self._path.with_suffix(suffix))
 
+    def with_segments(self, *pathsegments: str) -> Path:
+        return Path(*pathsegments)
+
     async def write_bytes(self, data: bytes) -> int:
         return await to_thread.run_sync(self._path.write_bytes, data)
 
     async def write_text(
         self,
         data: str,
         encoding: str | None = None,
```

### Comparing `anyio-3.7.1/src/anyio/_core/_sockets.py` & `anyio-4.0.0rc1/src/anyio/_core/_sockets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 from __future__ import annotations
 
 import socket
 import ssl
 import sys
+from collections.abc import Awaitable
 from ipaddress import IPv6Address, ip_address
 from os import PathLike, chmod
 from pathlib import Path
 from socket import AddressFamily, SocketKind
-from typing import Awaitable, List, Tuple, cast, overload
+from typing import Literal, Tuple, cast, overload
 
 from .. import to_thread
 from ..abc import (
     ConnectedUDPSocket,
+    ConnectedUNIXDatagramSocket,
     IPAddressType,
     IPSockAddrType,
     SocketListener,
     SocketStream,
     UDPSocket,
+    UNIXDatagramSocket,
     UNIXSocketStream,
 )
 from ..streams.stapled import MultiListener
 from ..streams.tls import TLSStream
-from ._eventloop import get_asynclib
+from ._eventloop import get_async_backend
 from ._resources import aclose_forcefully
 from ._synchronization import Event
 from ._tasks import create_task_group, move_on_after
 
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
+if sys.version_info < (3, 11):
+    from exceptiongroup import ExceptionGroup
 
 IPPROTO_IPV6 = getattr(socket, "IPPROTO_IPV6", 41)  # https://bugs.python.org/issue29515
 
-GetAddrInfoReturnType = List[
-    Tuple[AddressFamily, SocketKind, int, str, Tuple[str, int]]
-]
 AnyIPAddressFamily = Literal[
     AddressFamily.AF_UNSPEC, AddressFamily.AF_INET, AddressFamily.AF_INET6
 ]
 IPAddressFamily = Literal[AddressFamily.AF_INET, AddressFamily.AF_INET6]
 
 
 # tls_hostname given
@@ -138,26 +136,29 @@
     available) is tried first.
 
     When the connection has been established, a TLS handshake will be done if either
     ``ssl_context`` or ``tls_hostname`` is not ``None``, or if ``tls`` is ``True``.
 
     :param remote_host: the IP address or host name to connect to
     :param remote_port: port on the target host to connect to
-    :param local_host: the interface address or name to bind the socket to before connecting
+    :param local_host: the interface address or name to bind the socket to before
+        connecting
     :param tls: ``True`` to do a TLS handshake with the connected stream and return a
         :class:`~anyio.streams.tls.TLSStream` instead
-    :param ssl_context: the SSL context object to use (if omitted, a default context is created)
-    :param tls_standard_compatible: If ``True``, performs the TLS shutdown handshake before closing
-        the stream and requires that the server does this as well. Otherwise,
-        :exc:`~ssl.SSLEOFError` may be raised during reads from the stream.
+    :param ssl_context: the SSL context object to use (if omitted, a default context is
+        created)
+    :param tls_standard_compatible: If ``True``, performs the TLS shutdown handshake
+        before closing the stream and requires that the server does this as well.
+        Otherwise, :exc:`~ssl.SSLEOFError` may be raised during reads from the stream.
         Some protocols, such as HTTP, require this option to be ``False``.
         See :meth:`~ssl.SSLContext.wrap_socket` for details.
-    :param tls_hostname: host name to check the server certificate against (defaults to the value
-        of ``remote_host``)
-    :param happy_eyeballs_delay: delay (in seconds) before starting the next connection attempt
+    :param tls_hostname: host name to check the server certificate against (defaults to
+        the value of ``remote_host``)
+    :param happy_eyeballs_delay: delay (in seconds) before starting the next connection
+        attempt
     :return: a socket stream object if no TLS handshake was done, otherwise a TLS stream
     :raises OSError: if the connection attempt fails
 
     """
     # Placed here due to https://github.com/python/mypy/issues/7057
     connected_stream: SocketStream | None = None
 
@@ -173,15 +174,15 @@
                 connected_stream = stream
                 tg.cancel_scope.cancel()
             else:
                 await stream.aclose()
         finally:
             event.set()
 
-    asynclib = get_asynclib()
+    asynclib = get_async_backend()
     local_address: IPSockAddrType | None = None
     family = socket.AF_UNSPEC
     if local_host:
         gai_res = await getaddrinfo(str(local_host), None)
         family, *_, local_address = gai_res[0]
 
     target_host = str(remote_host)
@@ -189,16 +190,16 @@
         addr_obj = ip_address(remote_host)
     except ValueError:
         # getaddrinfo() will raise an exception if name resolution fails
         gai_res = await getaddrinfo(
             target_host, remote_port, family=family, type=socket.SOCK_STREAM
         )
 
-        # Organize the list so that the first address is an IPv6 address (if available) and the
-        # second one is an IPv4 addresses. The rest can be in whatever order.
+        # Organize the list so that the first address is an IPv6 address (if available)
+        # and the second one is an IPv4 addresses. The rest can be in whatever order.
         v6_found = v4_found = False
         target_addrs: list[tuple[socket.AddressFamily, str]] = []
         for af, *rest, sa in gai_res:
             if af == socket.AF_INET6 and not v6_found:
                 v6_found = True
                 target_addrs.insert(0, (af, sa[0]))
             elif af == socket.AF_INET and not v4_found and v6_found:
@@ -217,15 +218,19 @@
         for i, (af, addr) in enumerate(target_addrs):
             event = Event()
             tg.start_soon(try_connect, addr, event)
             with move_on_after(happy_eyeballs_delay):
                 await event.wait()
 
     if connected_stream is None:
-        cause = oserrors[0] if len(oserrors) == 1 else asynclib.ExceptionGroup(oserrors)
+        cause = (
+            oserrors[0]
+            if len(oserrors) == 1
+            else ExceptionGroup("multiple connection attempts failed", oserrors)
+        )
         raise OSError("All connection attempts failed") from cause
 
     if tls or tls_hostname or ssl_context:
         try:
             return await TLSStream.wrap(
                 connected_stream,
                 server_side=False,
@@ -247,15 +252,15 @@
     Not available on Windows.
 
     :param path: path to the socket
     :return: a socket stream object
 
     """
     path = str(Path(path))
-    return await get_asynclib().connect_unix(path)
+    return await get_async_backend().connect_unix(path)
 
 
 async def create_tcp_listener(
     *,
     local_host: IPAddressType | None = None,
     local_port: int = 0,
     family: AnyIPAddressFamily = socket.AddressFamily.AF_UNSPEC,
@@ -273,19 +278,19 @@
     :param backlog: maximum number of queued incoming connections (up to a maximum of
         2**16, or 65536)
     :param reuse_port: ``True`` to allow multiple sockets to bind to the same
         address/port (not supported on Windows)
     :return: a list of listener objects
 
     """
-    asynclib = get_asynclib()
+    asynclib = get_async_backend()
     backlog = min(backlog, 65536)
     local_host = str(local_host) if local_host is not None else None
     gai_res = await getaddrinfo(
-        local_host,  # type: ignore[arg-type]
+        local_host,
         local_port,
         family=family,
         type=socket.SocketKind.SOCK_STREAM if sys.platform == "win32" else 0,
         flags=socket.AI_PASSIVE | socket.AI_ADDRCONFIG,
     )
     listeners: list[SocketListener] = []
     try:
@@ -298,15 +303,16 @@
             # getaddrinfo(): https://github.com/MagicStack/uvloop/issues/539
             if sys.platform != "win32" and kind is not SocketKind.SOCK_STREAM:
                 continue
 
             raw_socket = socket.socket(fam)
             raw_socket.setblocking(False)
 
-            # For Windows, enable exclusive address use. For others, enable address reuse.
+            # For Windows, enable exclusive address use. For others, enable address
+            # reuse.
             if sys.platform == "win32":
                 raw_socket.setsockopt(socket.SOL_SOCKET, socket.SO_EXCLUSIVEADDRUSE, 1)
             else:
                 raw_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
             if reuse_port:
                 raw_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
@@ -318,61 +324,49 @@
                 # Workaround for #554
                 if "%" in sockaddr[0]:
                     addr, scope_id = sockaddr[0].split("%", 1)
                     sockaddr = (addr, sockaddr[1], 0, int(scope_id))
 
             raw_socket.bind(sockaddr)
             raw_socket.listen(backlog)
-            listener = asynclib.TCPSocketListener(raw_socket)
+            listener = asynclib.create_tcp_listener(raw_socket)
             listeners.append(listener)
     except BaseException:
         for listener in listeners:
             await listener.aclose()
 
         raise
 
     return MultiListener(listeners)
 
 
 async def create_unix_listener(
-    path: str | PathLike[str],
-    *,
-    mode: int | None = None,
-    backlog: int = 65536,
+    path: str | PathLike[str], *, mode: int | None = None, backlog: int = 65536
 ) -> SocketListener:
     """
     Create a UNIX socket listener.
 
     Not available on Windows.
 
     :param path: path of the socket
     :param mode: permissions to set on the socket
-    :param backlog: maximum number of queued incoming connections (up to a maximum of 2**16, or
-        65536)
+    :param backlog: maximum number of queued incoming connections (up to a maximum of
+        2**16, or 65536)
     :return: a listener object
 
     .. versionchanged:: 3.0
-        If a socket already exists on the file system in the given path, it will be removed first.
+        If a socket already exists on the file system in the given path, it will be
+        removed first.
 
     """
-    path_str = str(path)
-    path = Path(path)
-    if path.is_socket():
-        path.unlink()
-
     backlog = min(backlog, 65536)
-    raw_socket = socket.socket(socket.AF_UNIX)
-    raw_socket.setblocking(False)
+    raw_socket = await setup_unix_local_socket(path, mode, socket.SOCK_STREAM)
     try:
-        await to_thread.run_sync(raw_socket.bind, path_str, cancellable=True)
-        if mode is not None:
-            await to_thread.run_sync(chmod, path_str, mode, cancellable=True)
-
         raw_socket.listen(backlog)
-        return get_asynclib().UNIXSocketListener(raw_socket)
+        return get_async_backend().create_unix_listener(raw_socket)
     except BaseException:
         raw_socket.close()
         raise
 
 
 async def create_udp_socket(
     family: AnyIPAddressFamily = AddressFamily.AF_UNSPEC,
@@ -380,23 +374,23 @@
     local_host: IPAddressType | None = None,
     local_port: int = 0,
     reuse_port: bool = False,
 ) -> UDPSocket:
     """
     Create a UDP socket.
 
-    If ``local_port`` has been given, the socket will be bound to this port on the local
+    If ``port`` has been given, the socket will be bound to this port on the local
     machine, making this socket suitable for providing UDP based services.
 
-    :param family: address family (``AF_INET`` or ``AF_INET6``) – automatically determined from
-        ``local_host`` if omitted
+    :param family: address family (``AF_INET`` or ``AF_INET6``) – automatically
+        determined from ``local_host`` if omitted
     :param local_host: IP address or host name of the local interface to bind to
     :param local_port: local port to bind to
-    :param reuse_port: ``True`` to allow multiple sockets to bind to the same address/port
-        (not supported on Windows)
+    :param reuse_port: ``True`` to allow multiple sockets to bind to the same
+        address/port (not supported on Windows)
     :return: a UDP socket
 
     """
     if family is AddressFamily.AF_UNSPEC and not local_host:
         raise ValueError('Either "family" or "local_host" must be given')
 
     if local_host:
@@ -410,42 +404,43 @@
         family = cast(AnyIPAddressFamily, gai_res[0][0])
         local_address = gai_res[0][-1]
     elif family is AddressFamily.AF_INET6:
         local_address = ("::", 0)
     else:
         local_address = ("0.0.0.0", 0)
 
-    return await get_asynclib().create_udp_socket(
+    sock = await get_async_backend().create_udp_socket(
         family, local_address, None, reuse_port
     )
+    return cast(UDPSocket, sock)
 
 
 async def create_connected_udp_socket(
     remote_host: IPAddressType,
     remote_port: int,
     *,
     family: AnyIPAddressFamily = AddressFamily.AF_UNSPEC,
     local_host: IPAddressType | None = None,
     local_port: int = 0,
     reuse_port: bool = False,
 ) -> ConnectedUDPSocket:
     """
     Create a connected UDP socket.
 
-    Connected UDP sockets can only communicate with the specified remote host/port, and any packets
-    sent from other sources are dropped.
+    Connected UDP sockets can only communicate with the specified remote host/port, an
+    any packets sent from other sources are dropped.
 
     :param remote_host: remote host to set as the default target
     :param remote_port: port on the remote host to set as the default target
-    :param family: address family (``AF_INET`` or ``AF_INET6``) – automatically determined from
-        ``local_host`` or ``remote_host`` if omitted
+    :param family: address family (``AF_INET`` or ``AF_INET6``) – automatically
+        determined from ``local_host`` or ``remote_host`` if omitted
     :param local_host: IP address or host name of the local interface to bind to
     :param local_port: local port to bind to
-    :param reuse_port: ``True`` to allow multiple sockets to bind to the same address/port
-        (not supported on Windows)
+    :param reuse_port: ``True`` to allow multiple sockets to bind to the same
+        address/port (not supported on Windows)
     :return: a connected UDP socket
 
     """
     local_address = None
     if local_host:
         gai_res = await getaddrinfo(
             str(local_host),
@@ -459,33 +454,95 @@
 
     gai_res = await getaddrinfo(
         str(remote_host), remote_port, family=family, type=socket.SOCK_DGRAM
     )
     family = cast(AnyIPAddressFamily, gai_res[0][0])
     remote_address = gai_res[0][-1]
 
-    return await get_asynclib().create_udp_socket(
+    sock = await get_async_backend().create_udp_socket(
         family, local_address, remote_address, reuse_port
     )
+    return cast(ConnectedUDPSocket, sock)
+
+
+async def create_unix_datagram_socket(
+    *,
+    local_path: None | str | PathLike[str] = None,
+    local_mode: int | None = None,
+) -> UNIXDatagramSocket:
+    """
+    Create a UNIX datagram socket.
+
+    Not available on Windows.
+
+    If ``local_path`` has been given, the socket will be bound to this path, making this
+    socket suitable for receiving datagrams from other processes. Other processes can
+    send datagrams to this socket only if ``local_path`` is set.
+
+    If a socket already exists on the file system in the ``local_path``, it will be
+    removed first.
+
+    :param local_path: the path on which to bind to
+    :param local_mode: permissions to set on the local socket
+    :return: a UNIX datagram socket
+
+    """
+    raw_socket = await setup_unix_local_socket(
+        local_path, local_mode, socket.SOCK_DGRAM
+    )
+    return await get_async_backend().create_unix_datagram_socket(raw_socket, None)
+
+
+async def create_connected_unix_datagram_socket(
+    remote_path: str | PathLike[str],
+    *,
+    local_path: None | str | PathLike[str] = None,
+    local_mode: int | None = None,
+) -> ConnectedUNIXDatagramSocket:
+    """
+    Create a connected UNIX datagram socket.
+
+    Connected datagram sockets can only communicate with the specified remote path.
+
+    If ``local_path`` has been given, the socket will be bound to this path, making
+    this socket suitable for receiving datagrams from other processes. Other processes
+    can send datagrams to this socket only if ``local_path`` is set.
+
+    If a socket already exists on the file system in the ``local_path``, it will be
+    removed first.
+
+    :param remote_path: the path to set as the default target
+    :param local_path: the path on which to bind to
+    :param local_mode: permissions to set on the local socket
+    :return: a connected UNIX datagram socket
+
+    """
+    remote_path = str(Path(remote_path))
+    raw_socket = await setup_unix_local_socket(
+        local_path, local_mode, socket.SOCK_DGRAM
+    )
+    return await get_async_backend().create_unix_datagram_socket(
+        raw_socket, remote_path
+    )
 
 
 async def getaddrinfo(
-    host: bytearray | bytes | str,
+    host: bytes | str | None,
     port: str | int | None,
     *,
     family: int | AddressFamily = 0,
     type: int | SocketKind = 0,
     proto: int = 0,
     flags: int = 0,
-) -> GetAddrInfoReturnType:
+) -> list[tuple[AddressFamily, SocketKind, int, str, tuple[str, int]]]:
     """
     Look up a numeric IP address given a host name.
 
-    Internationalized domain names are translated according to the (non-transitional) IDNA 2008
-    standard.
+    Internationalized domain names are translated according to the (non-transitional)
+    IDNA 2008 standard.
 
     .. note:: 4-tuple IPv6 socket addresses are automatically converted to 2-tuples of
         (host, port), unlike what :func:`socket.getaddrinfo` does.
 
     :param host: host name
     :param port: port number
     :param family: socket family (`'AF_INET``, ...)
@@ -496,23 +553,23 @@
 
     .. seealso:: :func:`socket.getaddrinfo`
 
     """
     # Handle unicode hostnames
     if isinstance(host, str):
         try:
-            encoded_host = host.encode("ascii")
+            encoded_host: bytes | None = host.encode("ascii")
         except UnicodeEncodeError:
             import idna
 
             encoded_host = idna.encode(host, uts46=True)
     else:
         encoded_host = host
 
-    gai_res = await get_asynclib().getaddrinfo(
+    gai_res = await get_async_backend().getaddrinfo(
         encoded_host, port, family=family, type=type, proto=proto, flags=flags
     )
     return [
         (family, type, proto, canonname, convert_ipv6_sockaddr(sockaddr))
         for family, type, proto, canonname, sockaddr in gai_res
     ]
 
@@ -524,55 +581,55 @@
     :param sockaddr: socket address (e.g. (ipaddress, port) for IPv4)
     :param flags: flags to pass to upstream ``getnameinfo()``
     :return: a tuple of (host name, service name)
 
     .. seealso:: :func:`socket.getnameinfo`
 
     """
-    return get_asynclib().getnameinfo(sockaddr, flags)
+    return get_async_backend().getnameinfo(sockaddr, flags)
 
 
 def wait_socket_readable(sock: socket.socket) -> Awaitable[None]:
     """
     Wait until the given socket has data to be read.
 
-    This does **NOT** work on Windows when using the asyncio backend with a proactor event loop
-    (default on py3.8+).
+    This does **NOT** work on Windows when using the asyncio backend with a proactor
+    event loop (default on py3.8+).
 
-    .. warning:: Only use this on raw sockets that have not been wrapped by any higher level
-        constructs like socket streams!
+    .. warning:: Only use this on raw sockets that have not been wrapped by any higher
+        level constructs like socket streams!
 
     :param sock: a socket object
     :raises ~anyio.ClosedResourceError: if the socket was closed while waiting for the
         socket to become readable
     :raises ~anyio.BusyResourceError: if another task is already waiting for the socket
         to become readable
 
     """
-    return get_asynclib().wait_socket_readable(sock)
+    return get_async_backend().wait_socket_readable(sock)
 
 
 def wait_socket_writable(sock: socket.socket) -> Awaitable[None]:
     """
     Wait until the given socket can be written to.
 
-    This does **NOT** work on Windows when using the asyncio backend with a proactor event loop
-    (default on py3.8+).
+    This does **NOT** work on Windows when using the asyncio backend with a proactor
+    event loop (default on py3.8+).
 
-    .. warning:: Only use this on raw sockets that have not been wrapped by any higher level
-        constructs like socket streams!
+    .. warning:: Only use this on raw sockets that have not been wrapped by any higher
+        level constructs like socket streams!
 
     :param sock: a socket object
     :raises ~anyio.ClosedResourceError: if the socket was closed while waiting for the
         socket to become writable
     :raises ~anyio.BusyResourceError: if another task is already waiting for the socket
         to become writable
 
     """
-    return get_asynclib().wait_socket_writable(sock)
+    return get_async_backend().wait_socket_writable(sock)
 
 
 #
 # Private API
 #
 
 
@@ -601,7 +658,46 @@
 
             # Add scope_id to the address
             return f"{host}%{scope_id}", port
         else:
             return host, port
     else:
         return cast(Tuple[str, int], sockaddr)
+
+
+async def setup_unix_local_socket(
+    path: None | str | PathLike[str],
+    mode: int | None,
+    socktype: int,
+) -> socket.socket:
+    """
+    Create a UNIX local socket object, deleting the socket at the given path if it
+    exists.
+
+    Not available on Windows.
+
+    :param path: path of the socket
+    :param mode: permissions to set on the socket
+    :param socktype: socket.SOCK_STREAM or socket.SOCK_DGRAM
+
+    """
+    if path is not None:
+        path_str = str(path)
+        path = Path(path)
+        if path.is_socket():
+            path.unlink()
+    else:
+        path_str = None
+
+    raw_socket = socket.socket(socket.AF_UNIX, socktype)
+    raw_socket.setblocking(False)
+
+    if path_str is not None:
+        try:
+            await to_thread.run_sync(raw_socket.bind, path_str, cancellable=True)
+            if mode is not None:
+                await to_thread.run_sync(chmod, path_str, mode, cancellable=True)
+        except BaseException:
+            raw_socket.close()
+            raise
+
+    return raw_socket
```

### Comparing `anyio-3.7.1/src/anyio/_core/_subprocesses.py` & `anyio-4.0.0rc1/src/anyio/_core/_subprocesses.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 from __future__ import annotations
 
+from collections.abc import AsyncIterable, Mapping, Sequence
 from io import BytesIO
 from os import PathLike
 from subprocess import DEVNULL, PIPE, CalledProcessError, CompletedProcess
-from typing import (
-    IO,
-    Any,
-    AsyncIterable,
-    Mapping,
-    Sequence,
-    cast,
-)
+from typing import IO, Any, cast
 
 from ..abc import Process
-from ._eventloop import get_asynclib
+from ._eventloop import get_async_backend
 from ._tasks import create_task_group
 
 
 async def run_process(
     command: str | bytes | Sequence[str | bytes],
     *,
     input: bytes | None = None,
@@ -29,30 +23,32 @@
     start_new_session: bool = False,
 ) -> CompletedProcess[bytes]:
     """
     Run an external command in a subprocess and wait until it completes.
 
     .. seealso:: :func:`subprocess.run`
 
-    :param command: either a string to pass to the shell, or an iterable of strings containing the
-        executable name or path and its arguments
+    :param command: either a string to pass to the shell, or an iterable of strings
+        containing the executable name or path and its arguments
     :param input: bytes passed to the standard input of the subprocess
-    :param stdout: either :data:`subprocess.PIPE` or :data:`subprocess.DEVNULL`
-    :param stderr: one of :data:`subprocess.PIPE`, :data:`subprocess.DEVNULL` or
-        :data:`subprocess.STDOUT`
-    :param check: if ``True``, raise :exc:`~subprocess.CalledProcessError` if the process
-        terminates with a return code other than 0
-    :param cwd: If not ``None``, change the working directory to this before running the command
-    :param env: if not ``None``, this mapping replaces the inherited environment variables from the
-        parent process
-    :param start_new_session: if ``true`` the setsid() system call will be made in the child
-        process prior to the execution of the subprocess. (POSIX only)
+    :param stdout: one of :data:`subprocess.PIPE`, :data:`subprocess.DEVNULL`,
+        a file-like object, or `None`
+    :param stderr: one of :data:`subprocess.PIPE`, :data:`subprocess.DEVNULL`,
+        :data:`subprocess.STDOUT`, a file-like object, or `None`
+    :param check: if ``True``, raise :exc:`~subprocess.CalledProcessError` if the
+        process terminates with a return code other than 0
+    :param cwd: If not ``None``, change the working directory to this before running the
+        command
+    :param env: if not ``None``, this mapping replaces the inherited environment
+        variables from the parent process
+    :param start_new_session: if ``true`` the setsid() system call will be made in the
+        child process prior to the execution of the subprocess. (POSIX only)
     :return: an object representing the completed process
-    :raises ~subprocess.CalledProcessError: if ``check`` is ``True`` and the process exits with a
-        nonzero return code
+    :raises ~subprocess.CalledProcessError: if ``check`` is ``True`` and the process
+        exits with a nonzero return code
 
     """
 
     async def drain_stream(stream: AsyncIterable[bytes], index: int) -> None:
         buffer = BytesIO()
         async for chunk in stream:
             buffer.write(chunk)
@@ -102,34 +98,45 @@
     start_new_session: bool = False,
 ) -> Process:
     """
     Start an external command in a subprocess.
 
     .. seealso:: :class:`subprocess.Popen`
 
-    :param command: either a string to pass to the shell, or an iterable of strings containing the
-        executable name or path and its arguments
+    :param command: either a string to pass to the shell, or an iterable of strings
+        containing the executable name or path and its arguments
     :param stdin: one of :data:`subprocess.PIPE`, :data:`subprocess.DEVNULL`, a
         file-like object, or ``None``
     :param stdout: one of :data:`subprocess.PIPE`, :data:`subprocess.DEVNULL`,
         a file-like object, or ``None``
     :param stderr: one of :data:`subprocess.PIPE`, :data:`subprocess.DEVNULL`,
         :data:`subprocess.STDOUT`, a file-like object, or ``None``
     :param cwd: If not ``None``, the working directory is changed before executing
-    :param env: If env is not ``None``, it must be a mapping that defines the environment
-        variables for the new process
-    :param start_new_session: if ``true`` the setsid() system call will be made in the child
-        process prior to the execution of the subprocess. (POSIX only)
+    :param env: If env is not ``None``, it must be a mapping that defines the
+        environment variables for the new process
+    :param start_new_session: if ``true`` the setsid() system call will be made in the
+        child process prior to the execution of the subprocess. (POSIX only)
     :return: an asynchronous process object
 
     """
-    shell = isinstance(command, str)
-    return await get_asynclib().open_process(
-        command,
-        shell=shell,
-        stdin=stdin,
-        stdout=stdout,
-        stderr=stderr,
-        cwd=cwd,
-        env=env,
-        start_new_session=start_new_session,
-    )
+    if isinstance(command, (str, bytes)):
+        return await get_async_backend().open_process(
+            command,
+            shell=True,
+            stdin=stdin,
+            stdout=stdout,
+            stderr=stderr,
+            cwd=cwd,
+            env=env,
+            start_new_session=start_new_session,
+        )
+    else:
+        return await get_async_backend().open_process(
+            command,
+            shell=False,
+            stdin=stdin,
+            stdout=stdout,
+            stderr=stderr,
+            cwd=cwd,
+            env=env,
+            start_new_session=start_new_session,
+        )
```

### Comparing `anyio-3.7.1/src/anyio/_core/_synchronization.py` & `anyio-4.0.0rc1/src/anyio/_core/_synchronization.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from __future__ import annotations
 
 from collections import deque
 from dataclasses import dataclass
 from types import TracebackType
-from warnings import warn
 
 from ..lowlevel import cancel_shielded_checkpoint, checkpoint, checkpoint_if_cancelled
-from ._compat import DeprecatedAwaitable
-from ._eventloop import get_asynclib
+from ._eventloop import get_async_backend
 from ._exceptions import BusyResourceError, WouldBlock
 from ._tasks import CancelScope
 from ._testing import TaskInfo, get_current_task
 
 
 @dataclass(frozen=True)
 class EventStatistics:
@@ -23,45 +21,47 @@
 
 
 @dataclass(frozen=True)
 class CapacityLimiterStatistics:
     """
     :ivar int borrowed_tokens: number of tokens currently borrowed by tasks
     :ivar float total_tokens: total number of available tokens
-    :ivar tuple borrowers: tasks or other objects currently holding tokens borrowed from this
-        limiter
-    :ivar int tasks_waiting: number of tasks waiting on :meth:`~.CapacityLimiter.acquire` or
+    :ivar tuple borrowers: tasks or other objects currently holding tokens borrowed from
+        this limiter
+    :ivar int tasks_waiting: number of tasks waiting on
+        :meth:`~.CapacityLimiter.acquire` or
         :meth:`~.CapacityLimiter.acquire_on_behalf_of`
     """
 
     borrowed_tokens: int
     total_tokens: float
     borrowers: tuple[object, ...]
     tasks_waiting: int
 
 
 @dataclass(frozen=True)
 class LockStatistics:
     """
     :ivar bool locked: flag indicating if this lock is locked or not
-    :ivar ~anyio.TaskInfo owner: task currently holding the lock (or ``None`` if the lock is not
-        held by any task)
+    :ivar ~anyio.TaskInfo owner: task currently holding the lock (or ``None`` if the
+        lock is not held by any task)
     :ivar int tasks_waiting: number of tasks waiting on :meth:`~.Lock.acquire`
     """
 
     locked: bool
     owner: TaskInfo | None
     tasks_waiting: int
 
 
 @dataclass(frozen=True)
 class ConditionStatistics:
     """
     :ivar int tasks_waiting: number of tasks blocked on :meth:`~.Condition.wait`
-    :ivar ~anyio.LockStatistics lock_statistics: statistics of the underlying :class:`~.Lock`
+    :ivar ~anyio.LockStatistics lock_statistics: statistics of the underlying
+        :class:`~.Lock`
     """
 
     tasks_waiting: int
     lock_statistics: LockStatistics
 
 
 @dataclass(frozen=True)
@@ -72,29 +72,30 @@
     """
 
     tasks_waiting: int
 
 
 class Event:
     def __new__(cls) -> Event:
-        return get_asynclib().Event()
+        return get_async_backend().create_event()
 
-    def set(self) -> DeprecatedAwaitable:
+    def set(self) -> None:
         """Set the flag, notifying all listeners."""
         raise NotImplementedError
 
     def is_set(self) -> bool:
         """Return ``True`` if the flag is set, ``False`` if not."""
         raise NotImplementedError
 
     async def wait(self) -> None:
         """
         Wait until the flag has been set.
 
-        If the flag has already been set when this method is called, it returns immediately.
+        If the flag has already been set when this method is called, it returns
+        immediately.
 
         """
         raise NotImplementedError
 
     def statistics(self) -> EventStatistics:
         """Return statistics about the current state of this event."""
         raise NotImplementedError
@@ -157,27 +158,25 @@
             raise RuntimeError("Attempted to acquire an already held Lock")
 
         if self._owner_task is not None:
             raise WouldBlock
 
         self._owner_task = task
 
-    def release(self) -> DeprecatedAwaitable:
+    def release(self) -> None:
         """Release the lock."""
         if self._owner_task != get_current_task():
             raise RuntimeError("The current task is not holding this lock")
 
         if self._waiters:
             self._owner_task, event = self._waiters.popleft()
             event.set()
         else:
             del self._owner_task
 
-        return DeprecatedAwaitable(self.release)
-
     def locked(self) -> bool:
         """Return True if the lock is currently held."""
         return self._owner_task is not None
 
     def statistics(self) -> LockStatistics:
         """
         Return statistics about the current state of this lock.
@@ -220,18 +219,17 @@
 
         :raises ~anyio.WouldBlock: if the operation would block
 
         """
         self._lock.acquire_nowait()
         self._owner_task = get_current_task()
 
-    def release(self) -> DeprecatedAwaitable:
+    def release(self) -> None:
         """Release the underlying lock."""
         self._lock.release()
-        return DeprecatedAwaitable(self.release)
 
     def locked(self) -> bool:
         """Return True if the lock is set."""
         return self._lock.locked()
 
     def notify(self, n: int = 1) -> None:
         """Notify exactly n listeners."""
@@ -340,26 +338,24 @@
 
         """
         if self._value == 0:
             raise WouldBlock
 
         self._value -= 1
 
-    def release(self) -> DeprecatedAwaitable:
+    def release(self) -> None:
         """Increment the semaphore value."""
         if self._max_value is not None and self._value == self._max_value:
             raise ValueError("semaphore released too many times")
 
         if self._waiters:
             self._waiters.popleft().set()
         else:
             self._value += 1
 
-        return DeprecatedAwaitable(self.release)
-
     @property
     def value(self) -> int:
         """The current value of the semaphore."""
         return self._value
 
     @property
     def max_value(self) -> int | None:
@@ -373,15 +369,15 @@
         .. versionadded:: 3.0
         """
         return SemaphoreStatistics(len(self._waiters))
 
 
 class CapacityLimiter:
     def __new__(cls, total_tokens: float) -> CapacityLimiter:
-        return get_asynclib().CapacityLimiter(total_tokens)
+        return get_async_backend().create_capacity_limiter(total_tokens)
 
     async def __aenter__(self) -> None:
         raise NotImplementedError
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
@@ -392,66 +388,61 @@
 
     @property
     def total_tokens(self) -> float:
         """
         The total number of tokens available for borrowing.
 
         This is a read-write property. If the total number of tokens is increased, the
-        proportionate number of tasks waiting on this limiter will be granted their tokens.
+        proportionate number of tasks waiting on this limiter will be granted their
+        tokens.
 
         .. versionchanged:: 3.0
             The property is now writable.
 
         """
         raise NotImplementedError
 
     @total_tokens.setter
     def total_tokens(self, value: float) -> None:
         raise NotImplementedError
 
-    async def set_total_tokens(self, value: float) -> None:
-        warn(
-            "CapacityLimiter.set_total_tokens has been deprecated. Set the value of the"
-            '"total_tokens" attribute directly.',
-            DeprecationWarning,
-        )
-        self.total_tokens = value
-
     @property
     def borrowed_tokens(self) -> int:
         """The number of tokens that have currently been borrowed."""
         raise NotImplementedError
 
     @property
     def available_tokens(self) -> float:
         """The number of tokens currently available to be borrowed"""
         raise NotImplementedError
 
-    def acquire_nowait(self) -> DeprecatedAwaitable:
+    def acquire_nowait(self) -> None:
         """
-        Acquire a token for the current task without waiting for one to become available.
+        Acquire a token for the current task without waiting for one to become
+        available.
 
         :raises ~anyio.WouldBlock: if there are no tokens available for borrowing
 
         """
         raise NotImplementedError
 
-    def acquire_on_behalf_of_nowait(self, borrower: object) -> DeprecatedAwaitable:
+    def acquire_on_behalf_of_nowait(self, borrower: object) -> None:
         """
         Acquire a token without waiting for one to become available.
 
         :param borrower: the entity borrowing a token
         :raises ~anyio.WouldBlock: if there are no tokens available for borrowing
 
         """
         raise NotImplementedError
 
     async def acquire(self) -> None:
         """
-        Acquire a token for the current task, waiting if necessary for one to become available.
+        Acquire a token for the current task, waiting if necessary for one to become
+        available.
 
         """
         raise NotImplementedError
 
     async def acquire_on_behalf_of(self, borrower: object) -> None:
         """
         Acquire a token, waiting if necessary for one to become available.
@@ -460,123 +451,41 @@
 
         """
         raise NotImplementedError
 
     def release(self) -> None:
         """
         Release the token held by the current task.
-        :raises RuntimeError: if the current task has not borrowed a token from this limiter.
+
+        :raises RuntimeError: if the current task has not borrowed a token from this
+            limiter.
 
         """
         raise NotImplementedError
 
     def release_on_behalf_of(self, borrower: object) -> None:
         """
         Release the token held by the given borrower.
 
-        :raises RuntimeError: if the borrower has not borrowed a token from this limiter.
+        :raises RuntimeError: if the borrower has not borrowed a token from this
+            limiter.
 
         """
         raise NotImplementedError
 
     def statistics(self) -> CapacityLimiterStatistics:
         """
         Return statistics about the current state of this limiter.
 
         .. versionadded:: 3.0
 
         """
         raise NotImplementedError
 
 
-def create_lock() -> Lock:
-    """
-    Create an asynchronous lock.
-
-    :return: a lock object
-
-    .. deprecated:: 3.0
-       Use :class:`~Lock` directly.
-
-    """
-    warn("create_lock() is deprecated -- use Lock() directly", DeprecationWarning)
-    return Lock()
-
-
-def create_condition(lock: Lock | None = None) -> Condition:
-    """
-    Create an asynchronous condition.
-
-    :param lock: the lock to base the condition object on
-    :return: a condition object
-
-    .. deprecated:: 3.0
-       Use :class:`~Condition` directly.
-
-    """
-    warn(
-        "create_condition() is deprecated -- use Condition() directly",
-        DeprecationWarning,
-    )
-    return Condition(lock=lock)
-
-
-def create_event() -> Event:
-    """
-    Create an asynchronous event object.
-
-    :return: an event object
-
-    .. deprecated:: 3.0
-       Use :class:`~Event` directly.
-
-    """
-    warn("create_event() is deprecated -- use Event() directly", DeprecationWarning)
-    return get_asynclib().Event()
-
-
-def create_semaphore(value: int, *, max_value: int | None = None) -> Semaphore:
-    """
-    Create an asynchronous semaphore.
-
-    :param value: the semaphore's initial value
-    :param max_value: if set, makes this a "bounded" semaphore that raises :exc:`ValueError` if the
-        semaphore's value would exceed this number
-    :return: a semaphore object
-
-    .. deprecated:: 3.0
-       Use :class:`~Semaphore` directly.
-
-    """
-    warn(
-        "create_semaphore() is deprecated -- use Semaphore() directly",
-        DeprecationWarning,
-    )
-    return Semaphore(value, max_value=max_value)
-
-
-def create_capacity_limiter(total_tokens: float) -> CapacityLimiter:
-    """
-    Create a capacity limiter.
-
-    :param total_tokens: the total number of tokens available for borrowing (can be an integer or
-        :data:`math.inf`)
-    :return: a capacity limiter object
-
-    .. deprecated:: 3.0
-       Use :class:`~CapacityLimiter` directly.
-
-    """
-    warn(
-        "create_capacity_limiter() is deprecated -- use CapacityLimiter() directly",
-        DeprecationWarning,
-    )
-    return get_asynclib().CapacityLimiter(total_tokens)
-
-
 class ResourceGuard:
     __slots__ = "action", "_guarded"
 
     def __init__(self, action: str):
         self.action = action
         self._guarded = False
```

### Comparing `anyio-3.7.1/src/anyio/_core/_tasks.py` & `anyio-4.0.0rc1/src/anyio/_core/_tasks.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 from __future__ import annotations
 
 import math
+from collections.abc import Generator
+from contextlib import contextmanager
 from types import TracebackType
-from warnings import warn
 
 from ..abc._tasks import TaskGroup, TaskStatus
-from ._compat import (
-    DeprecatedAsyncContextManager,
-    DeprecatedAwaitable,
-    DeprecatedAwaitableFloat,
-)
-from ._eventloop import get_asynclib
+from ._eventloop import get_async_backend
 
 
 class _IgnoredTaskStatus(TaskStatus[object]):
     def started(self, value: object = None) -> None:
         pass
 
 
 TASK_STATUS_IGNORED = _IgnoredTaskStatus()
 
 
-class CancelScope(DeprecatedAsyncContextManager["CancelScope"]):
+class CancelScope:
     """
     Wraps a unit of work that can be made separately cancellable.
 
     :param deadline: The time (clock value) when this scope is cancelled automatically
     :param shield: ``True`` to shield the cancel scope from external cancellation
     """
 
     def __new__(
         cls, *, deadline: float = math.inf, shield: bool = False
     ) -> CancelScope:
-        return get_asynclib().CancelScope(shield=shield, deadline=deadline)
+        return get_async_backend().create_cancel_scope(shield=shield, deadline=deadline)
 
-    def cancel(self) -> DeprecatedAwaitable:
+    def cancel(self) -> None:
         """Cancel this scope immediately."""
         raise NotImplementedError
 
     @property
     def deadline(self) -> float:
         """
         The time (clock value) when this scope is cancelled automatically.
@@ -54,14 +50,27 @@
 
     @property
     def cancel_called(self) -> bool:
         """``True`` if :meth:`cancel` has been called."""
         raise NotImplementedError
 
     @property
+    def cancelled_caught(self) -> bool:
+        """
+        ``True`` if this scope suppressed a cancellation exception it itself raised.
+
+        This is typically used to check if any work was interrupted, or to see if the
+        scope was cancelled due to its deadline being reached. The value will, however,
+        only be ``True`` if the cancellation was triggered by the scope itself (and not
+        an outer scope).
+
+        """
+        raise NotImplementedError
+
+    @property
     def shield(self) -> bool:
         """
         ``True`` if this scope is shielded from external cancellation.
 
         While a scope is shielded, it will not receive cancellations from outside.
 
         """
@@ -79,102 +88,71 @@
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> bool | None:
         raise NotImplementedError
 
 
-def open_cancel_scope(*, shield: bool = False) -> CancelScope:
+@contextmanager
+def fail_after(
+    delay: float | None, shield: bool = False
+) -> Generator[CancelScope, None, None]:
     """
-    Open a cancel scope.
+    Create a context manager which raises a :class:`TimeoutError` if does not finish in
+    time.
 
-    :param shield: ``True`` to shield the cancel scope from external cancellation
-    :return: a cancel scope
-
-    .. deprecated:: 3.0
-       Use :class:`~CancelScope` directly.
-
-    """
-    warn(
-        "open_cancel_scope() is deprecated -- use CancelScope() directly",
-        DeprecationWarning,
-    )
-    return get_asynclib().CancelScope(shield=shield)
-
-
-class FailAfterContextManager(DeprecatedAsyncContextManager[CancelScope]):
-    def __init__(self, cancel_scope: CancelScope):
-        self._cancel_scope = cancel_scope
-
-    def __enter__(self) -> CancelScope:
-        return self._cancel_scope.__enter__()
-
-    def __exit__(
-        self,
-        exc_type: type[BaseException] | None,
-        exc_val: BaseException | None,
-        exc_tb: TracebackType | None,
-    ) -> bool | None:
-        retval = self._cancel_scope.__exit__(exc_type, exc_val, exc_tb)
-        if self._cancel_scope.cancel_called:
-            raise TimeoutError
-
-        return retval
-
-
-def fail_after(delay: float | None, shield: bool = False) -> FailAfterContextManager:
-    """
-    Create a context manager which raises a :class:`TimeoutError` if does not finish in time.
-
-    :param delay: maximum allowed time (in seconds) before raising the exception, or ``None`` to
-        disable the timeout
+    :param delay: maximum allowed time (in seconds) before raising the exception, or
+        ``None`` to disable the timeout
     :param shield: ``True`` to shield the cancel scope from external cancellation
     :return: a context manager that yields a cancel scope
     :rtype: :class:`~typing.ContextManager`\\[:class:`~anyio.CancelScope`\\]
 
     """
-    deadline = (
-        (get_asynclib().current_time() + delay) if delay is not None else math.inf
-    )
-    cancel_scope = get_asynclib().CancelScope(deadline=deadline, shield=shield)
-    return FailAfterContextManager(cancel_scope)
+    current_time = get_async_backend().current_time
+    deadline = (current_time() + delay) if delay is not None else math.inf
+    with get_async_backend().create_cancel_scope(
+        deadline=deadline, shield=shield
+    ) as cancel_scope:
+        yield cancel_scope
+
+    if cancel_scope.cancelled_caught and current_time() >= cancel_scope.deadline:
+        raise TimeoutError
 
 
 def move_on_after(delay: float | None, shield: bool = False) -> CancelScope:
     """
     Create a cancel scope with a deadline that expires after the given delay.
 
-    :param delay: maximum allowed time (in seconds) before exiting the context block, or ``None``
-        to disable the timeout
+    :param delay: maximum allowed time (in seconds) before exiting the context block, or
+        ``None`` to disable the timeout
     :param shield: ``True`` to shield the cancel scope from external cancellation
     :return: a cancel scope
 
     """
     deadline = (
-        (get_asynclib().current_time() + delay) if delay is not None else math.inf
+        (get_async_backend().current_time() + delay) if delay is not None else math.inf
     )
-    return get_asynclib().CancelScope(deadline=deadline, shield=shield)
+    return get_async_backend().create_cancel_scope(deadline=deadline, shield=shield)
 
 
-def current_effective_deadline() -> DeprecatedAwaitableFloat:
+def current_effective_deadline() -> float:
     """
-    Return the nearest deadline among all the cancel scopes effective for the current task.
+    Return the nearest deadline among all the cancel scopes effective for the current
+    task.
 
     :return: a clock value from the event loop's internal clock (or ``float('inf')`` if
         there is no deadline in effect, or ``float('-inf')`` if the current scope has
         been cancelled)
     :rtype: float
 
     """
-    return DeprecatedAwaitableFloat(
-        get_asynclib().current_effective_deadline(), current_effective_deadline
-    )
+    return get_async_backend().current_effective_deadline()
 
 
 def create_task_group() -> TaskGroup:
     """
     Create a task group.
 
     :return: a task group
 
     """
-    return get_asynclib().TaskGroup()
+    return get_async_backend().create_task_group()
```

### Comparing `anyio-3.7.1/src/anyio/_core/_testing.py` & `anyio-4.0.0rc1/src/anyio/_core/_testing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
-from typing import Any, Awaitable, Generator
+from collections.abc import Awaitable, Generator
+from typing import Any
 
-from ._compat import DeprecatedAwaitableList, _warn_deprecation
-from ._eventloop import get_asynclib
+from ._eventloop import get_async_backend
 
 
 class TaskInfo:
     """
     Represents an asynchronous task.
 
     :ivar int id: the unique identifier of the task
@@ -41,42 +41,34 @@
 
     def __hash__(self) -> int:
         return hash(self.id)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(id={self.id!r}, name={self.name!r})"
 
-    def __await__(self) -> Generator[None, None, TaskInfo]:
-        _warn_deprecation(self)
-        if False:
-            yield
-
-        return self
-
     def _unwrap(self) -> TaskInfo:
         return self
 
 
 def get_current_task() -> TaskInfo:
     """
     Return the current task.
 
     :return: a representation of the current task
 
     """
-    return get_asynclib().get_current_task()
+    return get_async_backend().get_current_task()
 
 
-def get_running_tasks() -> DeprecatedAwaitableList[TaskInfo]:
+def get_running_tasks() -> list[TaskInfo]:
     """
     Return a list of running tasks in the current event loop.
 
     :return: a list of task info objects
 
     """
-    tasks = get_asynclib().get_running_tasks()
-    return DeprecatedAwaitableList(tasks, func=get_running_tasks)
+    return get_async_backend().get_running_tasks()
 
 
 async def wait_all_tasks_blocked() -> None:
     """Wait until all other tasks are waiting for something."""
-    await get_asynclib().wait_all_tasks_blocked()
+    await get_async_backend().wait_all_tasks_blocked()
```

### Comparing `anyio-3.7.1/src/anyio/_core/_typedattr.py` & `anyio-4.0.0rc1/src/anyio/_core/_typedattr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from __future__ import annotations
 
-import sys
-from typing import Any, Callable, Mapping, TypeVar, overload
+from collections.abc import Callable, Mapping
+from typing import Any, TypeVar, final, overload
 
 from ._exceptions import TypedAttributeLookupError
 
-if sys.version_info >= (3, 8):
-    from typing import final
-else:
-    from typing_extensions import final
-
 T_Attr = TypeVar("T_Attr")
 T_Default = TypeVar("T_Default")
 undefined = object()
 
 
 def typed_attribute() -> Any:
     """Return a unique object, used to mark typed attributes."""
@@ -40,19 +35,20 @@
 
 class TypedAttributeProvider:
     """Base class for classes that wish to provide typed extra attributes."""
 
     @property
     def extra_attributes(self) -> Mapping[T_Attr, Callable[[], T_Attr]]:
         """
-        A mapping of the extra attributes to callables that return the corresponding values.
+        A mapping of the extra attributes to callables that return the corresponding
+        values.
 
-        If the provider wraps another provider, the attributes from that wrapper should also be
-        included in the returned mapping (but the wrapper may override the callables from the
-        wrapped instance).
+        If the provider wraps another provider, the attributes from that wrapper should
+        also be included in the returned mapping (but the wrapper may override the
+        callables from the wrapped instance).
 
         """
         return {}
 
     @overload
     def extra(self, attribute: T_Attr) -> T_Attr:
         ...
@@ -64,18 +60,20 @@
     @final
     def extra(self, attribute: Any, default: object = undefined) -> object:
         """
         extra(attribute, default=undefined)
 
         Return the value of the given typed extra attribute.
 
-        :param attribute: the attribute (member of a :class:`~TypedAttributeSet`) to look for
-        :param default: the value that should be returned if no value is found for the attribute
-        :raises ~anyio.TypedAttributeLookupError: if the search failed and no default value was
-            given
+        :param attribute: the attribute (member of a :class:`~TypedAttributeSet`) to
+            look for
+        :param default: the value that should be returned if no value is found for the
+            attribute
+        :raises ~anyio.TypedAttributeLookupError: if the search failed and no default
+            value was given
 
         """
         try:
             return self.extra_attributes[attribute]()
         except KeyError:
             if default is undefined:
                 raise TypedAttributeLookupError("Attribute not found") from None
```

### Comparing `anyio-3.7.1/src/anyio/abc/_resources.py` & `anyio-4.0.0rc1/src/anyio/abc/_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 T = TypeVar("T")
 
 
 class AsyncResource(metaclass=ABCMeta):
     """
     Abstract base class for all closeable asynchronous resources.
 
-    Works as an asynchronous context manager which returns the instance itself on enter, and calls
-    :meth:`aclose` on exit.
+    Works as an asynchronous context manager which returns the instance itself on enter,
+    and calls :meth:`aclose` on exit.
     """
 
     async def __aenter__(self: T) -> T:
         return self
 
     async def __aexit__(
         self,
```

### Comparing `anyio-3.7.1/src/anyio/abc/_sockets.py` & `anyio-4.0.0rc1/src/anyio/abc/_sockets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 from __future__ import annotations
 
 import socket
 from abc import abstractmethod
+from collections.abc import Callable, Collection, Mapping
 from contextlib import AsyncExitStack
 from io import IOBase
 from ipaddress import IPv4Address, IPv6Address
 from socket import AddressFamily
-from typing import (
-    Any,
-    Callable,
-    Collection,
-    Mapping,
-    Tuple,
-    TypeVar,
-    Union,
-)
+from types import TracebackType
+from typing import Any, Tuple, TypeVar, Union
 
-from .._core._tasks import create_task_group
 from .._core._typedattr import (
     TypedAttributeProvider,
     TypedAttributeSet,
     typed_attribute,
 )
 from ._streams import ByteStream, Listener, UnreliableObjectStream
 from ._tasks import TaskGroup
 
 IPAddressType = Union[str, IPv4Address, IPv6Address]
 IPSockAddrType = Tuple[str, int]
 SockAddrType = Union[IPSockAddrType, str]
 UDPPacketType = Tuple[bytes, IPSockAddrType]
+UNIXDatagramPacketType = Tuple[bytes, str]
 T_Retval = TypeVar("T_Retval")
 
 
+class _NullAsyncContextManager:
+    async def __aenter__(self) -> None:
+        pass
+
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
+        return None
+
+
 class SocketAttribute(TypedAttributeSet):
     #: the address family of the underlying socket
     family: AddressFamily = typed_attribute()
     #: the local socket address of the underlying socket
     local_address: SockAddrType = typed_attribute()
     #: for IP addresses, the local port the underlying socket is bound to
     local_port: int = typed_attribute()
@@ -96,16 +103,16 @@
 class UNIXSocketStream(SocketStream):
     @abstractmethod
     async def send_fds(self, message: bytes, fds: Collection[int | IOBase]) -> None:
         """
         Send file descriptors along with a message to the peer.
 
         :param message: a non-empty bytestring
-        :param fds: a collection of files (either numeric file descriptors or open file or socket
-            objects)
+        :param fds: a collection of files (either numeric file descriptors or open file
+            or socket objects)
         """
 
     @abstractmethod
     async def receive_fds(self, msglen: int, maxfds: int) -> tuple[bytes, list[int]]:
         """
         Receive file descriptors along with a message from the peer.
 
@@ -127,34 +134,61 @@
         """Accept an incoming connection."""
 
     async def serve(
         self,
         handler: Callable[[SocketStream], Any],
         task_group: TaskGroup | None = None,
     ) -> None:
-        async with AsyncExitStack() as exit_stack:
+        from .. import create_task_group
+
+        async with AsyncExitStack() as stack:
             if task_group is None:
-                task_group = await exit_stack.enter_async_context(create_task_group())
+                task_group = await stack.enter_async_context(create_task_group())
 
             while True:
                 stream = await self.accept()
                 task_group.start_soon(handler, stream)
 
 
 class UDPSocket(UnreliableObjectStream[UDPPacketType], _SocketProvider):
     """
     Represents an unconnected UDP socket.
 
     Supports all relevant extra attributes from :class:`~SocketAttribute`.
     """
 
     async def sendto(self, data: bytes, host: str, port: int) -> None:
-        """Alias for :meth:`~.UnreliableObjectSendStream.send` ((data, (host, port)))."""
+        """
+        Alias for :meth:`~.UnreliableObjectSendStream.send` ((data, (host, port))).
+
+        """
         return await self.send((data, (host, port)))
 
 
 class ConnectedUDPSocket(UnreliableObjectStream[bytes], _SocketProvider):
     """
     Represents an connected UDP socket.
 
     Supports all relevant extra attributes from :class:`~SocketAttribute`.
     """
+
+
+class UNIXDatagramSocket(
+    UnreliableObjectStream[UNIXDatagramPacketType], _SocketProvider
+):
+    """
+    Represents an unconnected Unix datagram socket.
+
+    Supports all relevant extra attributes from :class:`~SocketAttribute`.
+    """
+
+    async def sendto(self, data: bytes, path: str) -> None:
+        """Alias for :meth:`~.UnreliableObjectSendStream.send` ((data, path))."""
+        return await self.send((data, path))
+
+
+class ConnectedUNIXDatagramSocket(UnreliableObjectStream[bytes], _SocketProvider):
+    """
+    Represents a connected Unix datagram socket.
+
+    Supports all relevant extra attributes from :class:`~SocketAttribute`.
+    """
```

### Comparing `anyio-3.7.1/src/anyio/abc/_streams.py` & `anyio-4.0.0rc1/src/anyio/abc/_streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from abc import abstractmethod
-from typing import Any, Callable, Generic, TypeVar, Union
+from collections.abc import Callable
+from typing import Any, Generic, TypeVar, Union
 
 from .._core._exceptions import EndOfStream
 from .._core._typedattr import TypedAttributeProvider
 from ._resources import AsyncResource
 from ._tasks import TaskGroup
 
 T_Item = TypeVar("T_Item")
@@ -15,19 +16,19 @@
 
 class UnreliableObjectReceiveStream(
     Generic[T_co], AsyncResource, TypedAttributeProvider
 ):
     """
     An interface for receiving objects.
 
-    This interface makes no guarantees that the received messages arrive in the order in which they
-    were sent, or that no messages are missed.
+    This interface makes no guarantees that the received messages arrive in the order in
+    which they were sent, or that no messages are missed.
 
-    Asynchronously iterating over objects of this type will yield objects matching the given type
-    parameter.
+    Asynchronously iterating over objects of this type will yield objects matching the
+    given type parameter.
     """
 
     def __aiter__(self) -> UnreliableObjectReceiveStream[T_co]:
         return self
 
     async def __anext__(self) -> T_co:
         try:
@@ -50,16 +51,16 @@
 
 class UnreliableObjectSendStream(
     Generic[T_contra], AsyncResource, TypedAttributeProvider
 ):
     """
     An interface for sending objects.
 
-    This interface makes no guarantees that the messages sent will reach the recipient(s) in the
-    same order in which they were sent, or at all.
+    This interface makes no guarantees that the messages sent will reach the
+    recipient(s) in the same order in which they were sent, or at all.
     """
 
     @abstractmethod
     async def send(self, item: T_contra) -> None:
         """
         Send an item to the peer(s).
 
@@ -71,58 +72,59 @@
         """
 
 
 class UnreliableObjectStream(
     UnreliableObjectReceiveStream[T_Item], UnreliableObjectSendStream[T_Item]
 ):
     """
-    A bidirectional message stream which does not guarantee the order or reliability of message
-    delivery.
+    A bidirectional message stream which does not guarantee the order or reliability of
+    message delivery.
     """
 
 
 class ObjectReceiveStream(UnreliableObjectReceiveStream[T_co]):
     """
-    A receive message stream which guarantees that messages are received in the same order in
-    which they were sent, and that no messages are missed.
+    A receive message stream which guarantees that messages are received in the same
+    order in which they were sent, and that no messages are missed.
     """
 
 
 class ObjectSendStream(UnreliableObjectSendStream[T_contra]):
     """
-    A send message stream which guarantees that messages are delivered in the same order in which
-    they were sent, without missing any messages in the middle.
+    A send message stream which guarantees that messages are delivered in the same order
+    in which they were sent, without missing any messages in the middle.
     """
 
 
 class ObjectStream(
     ObjectReceiveStream[T_Item],
     ObjectSendStream[T_Item],
     UnreliableObjectStream[T_Item],
 ):
     """
-    A bidirectional message stream which guarantees the order and reliability of message delivery.
+    A bidirectional message stream which guarantees the order and reliability of message
+    delivery.
     """
 
     @abstractmethod
     async def send_eof(self) -> None:
         """
         Send an end-of-file indication to the peer.
 
-        You should not try to send any further data to this stream after calling this method.
-        This method is idempotent (does nothing on successive calls).
+        You should not try to send any further data to this stream after calling this
+        method. This method is idempotent (does nothing on successive calls).
         """
 
 
 class ByteReceiveStream(AsyncResource, TypedAttributeProvider):
     """
     An interface for receiving bytes from a single peer.
 
-    Iterating this byte stream will yield a byte string of arbitrary length, but no more than
-    65536 bytes.
+    Iterating this byte stream will yield a byte string of arbitrary length, but no more
+    than 65536 bytes.
     """
 
     def __aiter__(self) -> ByteReceiveStream:
         return self
 
     async def __anext__(self) -> bytes:
         try:
@@ -131,16 +133,16 @@
             raise StopAsyncIteration
 
     @abstractmethod
     async def receive(self, max_bytes: int = 65536) -> bytes:
         """
         Receive at most ``max_bytes`` bytes from the peer.
 
-        .. note:: Implementors of this interface should not return an empty :class:`bytes` object,
-            and users should ignore them.
+        .. note:: Implementors of this interface should not return an empty
+            :class:`bytes` object, and users should ignore them.
 
         :param max_bytes: maximum number of bytes to receive
         :return: the received bytes
         :raises ~anyio.EndOfStream: if this stream has been closed from the other end
         """
 
 
@@ -160,16 +162,16 @@
     """A bidirectional byte stream."""
 
     @abstractmethod
     async def send_eof(self) -> None:
         """
         Send an end-of-file indication to the peer.
 
-        You should not try to send any further data to this stream after calling this method.
-        This method is idempotent (does nothing on successive calls).
+        You should not try to send any further data to this stream after calling this
+        method. This method is idempotent (does nothing on successive calls).
         """
 
 
 #: Type alias for all unreliable bytes-oriented receive streams.
 AnyUnreliableByteReceiveStream = Union[
     UnreliableObjectReceiveStream[bytes], ByteReceiveStream
 ]
@@ -186,18 +188,16 @@
 
 
 class Listener(Generic[T_co], AsyncResource, TypedAttributeProvider):
     """An interface for objects that let you accept incoming connections."""
 
     @abstractmethod
     async def serve(
-        self,
-        handler: Callable[[T_co], Any],
-        task_group: TaskGroup | None = None,
+        self, handler: Callable[[T_co], Any], task_group: TaskGroup | None = None
     ) -> None:
         """
         Accept incoming connections as they come in and start tasks to handle them.
 
         :param handler: a callable that will be used to handle each accepted connection
-        :param task_group: the task group that will be used to start tasks for handling each
-            accepted connection (if omitted, an ad-hoc task group will be created)
+        :param task_group: the task group that will be used to start tasks for handling
+            each accepted connection (if omitted, an ad-hoc task group will be created)
         """
```

### Comparing `anyio-3.7.1/src/anyio/abc/_subprocesses.py` & `anyio-4.0.0rc1/src/anyio/abc/_subprocesses.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,16 @@
     def pid(self) -> int:
         """The process ID of the process."""
 
     @property
     @abstractmethod
     def returncode(self) -> int | None:
         """
-        The return code of the process. If the process has not yet terminated, this will be
-        ``None``.
+        The return code of the process. If the process has not yet terminated, this will
+        be ``None``.
         """
 
     @property
     @abstractmethod
     def stdin(self) -> ByteSendStream | None:
         """The stream for the standard input of the process."""
```

### Comparing `anyio-3.7.1/src/anyio/abc/_tasks.py` & `anyio-4.0.0rc1/src/anyio/abc/_tasks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 from __future__ import annotations
 
-import sys
 from abc import ABCMeta, abstractmethod
+from collections.abc import Awaitable, Callable, Coroutine
 from types import TracebackType
-from typing import TYPE_CHECKING, Any, Awaitable, Callable, TypeVar, overload
-from warnings import warn
-
-if sys.version_info >= (3, 8):
-    from typing import Protocol
-else:
-    from typing_extensions import Protocol
+from typing import TYPE_CHECKING, Any, Protocol, TypeVar, overload
 
 if TYPE_CHECKING:
-    from anyio._core._tasks import CancelScope
+    from .._core._tasks import CancelScope
 
 T_Retval = TypeVar("T_Retval")
 T_contra = TypeVar("T_contra", contravariant=True)
 
 
 class TaskStatus(Protocol[T_contra]):
     @overload
@@ -41,42 +35,18 @@
 
     :ivar cancel_scope: the cancel scope inherited by all child tasks
     :vartype cancel_scope: CancelScope
     """
 
     cancel_scope: CancelScope
 
-    async def spawn(
-        self,
-        func: Callable[..., Awaitable[Any]],
-        *args: object,
-        name: object = None,
-    ) -> None:
-        """
-        Start a new task in this task group.
-
-        :param func: a coroutine function
-        :param args: positional arguments to call the function with
-        :param name: name of the task, for the purposes of introspection and debugging
-
-        .. deprecated:: 3.0
-           Use :meth:`start_soon` instead. If your code needs AnyIO 2 compatibility, you
-           can keep using this until AnyIO 4.
-
-        """
-        warn(
-            'spawn() is deprecated -- use start_soon() (without the "await") instead',
-            DeprecationWarning,
-        )
-        self.start_soon(func, *args, name=name)
-
     @abstractmethod
     def start_soon(
         self,
-        func: Callable[..., Awaitable[Any]],
+        func: Callable[..., Coroutine[Any, Any, Any]],
         *args: object,
         name: object = None,
     ) -> None:
         """
         Start a new task in this task group.
 
         :param func: a coroutine function
@@ -96,15 +66,16 @@
         """
         Start a new task and wait until it signals for readiness.
 
         :param func: a coroutine function
         :param args: positional arguments to call the function with
         :param name: name of the task, for the purposes of introspection and debugging
         :return: the value passed to ``task_status.started()``
-        :raises RuntimeError: if the task finishes without calling ``task_status.started()``
+        :raises RuntimeError: if the task finishes without calling
+            ``task_status.started()``
 
         .. versionadded:: 3.0
         """
 
     @abstractmethod
     async def __aenter__(self) -> TaskGroup:
         """Enter the task group context and allow starting new tasks."""
```

### Comparing `anyio-3.7.1/src/anyio/abc/_testing.py` & `anyio-4.0.0rc1/src/anyio/abc/_testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 from __future__ import annotations
 
 import types
 from abc import ABCMeta, abstractmethod
-from collections.abc import AsyncGenerator, Iterable
-from typing import Any, Callable, Coroutine, TypeVar
+from collections.abc import AsyncGenerator, Callable, Coroutine, Iterable
+from typing import Any, TypeVar
 
 _T = TypeVar("_T")
 
 
 class TestRunner(metaclass=ABCMeta):
     """
-    Encapsulates a running event loop. Every call made through this object will use the same event
-    loop.
+    Encapsulates a running event loop. Every call made through this object will use the
+    same event loop.
     """
 
     def __enter__(self) -> TestRunner:
         return self
 
+    @abstractmethod
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: types.TracebackType | None,
     ) -> bool | None:
-        self.close()
-        return None
-
-    @abstractmethod
-    def close(self) -> None:
-        """Close the event loop."""
+        ...
 
     @abstractmethod
     def run_asyncgen_fixture(
         self,
         fixture_func: Callable[..., AsyncGenerator[_T, Any]],
         kwargs: dict[str, Any],
     ) -> Iterable[_T]:
```

### Comparing `anyio-3.7.1/src/anyio/from_thread.py` & `anyio-4.0.0rc1/src/anyio/from_thread.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from __future__ import annotations
 
 import threading
-from asyncio import iscoroutine
+from collections.abc import Awaitable, Callable, Generator
 from concurrent.futures import FIRST_COMPLETED, Future, ThreadPoolExecutor, wait
 from contextlib import AbstractContextManager, contextmanager
+from inspect import isawaitable
 from types import TracebackType
 from typing import (
     Any,
     AsyncContextManager,
-    Awaitable,
-    Callable,
     ContextManager,
-    Generator,
     Generic,
     Iterable,
     TypeVar,
     cast,
     overload,
 )
-from warnings import warn
 
 from ._core import _eventloop
-from ._core._eventloop import get_asynclib, get_cancelled_exc_class, threadlocals
+from ._core._eventloop import get_async_backend, get_cancelled_exc_class, threadlocals
 from ._core._synchronization import Event
 from ._core._tasks import CancelScope, create_task_group
 from .abc._tasks import TaskStatus
 
 T_Retval = TypeVar("T_Retval")
 T_co = TypeVar("T_co")
 
@@ -36,54 +33,38 @@
 
     :param func: a coroutine function
     :param args: positional arguments for the callable
     :return: the return value of the coroutine function
 
     """
     try:
-        asynclib = threadlocals.current_async_module
+        async_backend = threadlocals.current_async_backend
+        token = threadlocals.current_token
     except AttributeError:
         raise RuntimeError("This function can only be run from an AnyIO worker thread")
 
-    return asynclib.run_async_from_thread(func, *args)
-
-
-def run_async_from_thread(
-    func: Callable[..., Awaitable[T_Retval]], *args: object
-) -> T_Retval:
-    warn(
-        "run_async_from_thread() has been deprecated, use anyio.from_thread.run() instead",
-        DeprecationWarning,
-    )
-    return run(func, *args)
+    return async_backend.run_async_from_thread(func, args, token=token)
 
 
 def run_sync(func: Callable[..., T_Retval], *args: object) -> T_Retval:
     """
     Call a function in the event loop thread from a worker thread.
 
     :param func: a callable
     :param args: positional arguments for the callable
     :return: the return value of the callable
 
     """
     try:
-        asynclib = threadlocals.current_async_module
+        async_backend = threadlocals.current_async_backend
+        token = threadlocals.current_token
     except AttributeError:
         raise RuntimeError("This function can only be run from an AnyIO worker thread")
 
-    return asynclib.run_sync_from_thread(func, *args)
-
-
-def run_sync_from_thread(func: Callable[..., T_Retval], *args: object) -> T_Retval:
-    warn(
-        "run_sync_from_thread() has been deprecated, use anyio.from_thread.run_sync() instead",
-        DeprecationWarning,
-    )
-    return run_sync(func, *args)
+    return async_backend.run_sync_from_thread(func, args, token=token)
 
 
 class _BlockingAsyncContextManager(Generic[T_co], AbstractContextManager):
     _enter_future: Future
     _exit_future: Future
     _exit_event: Event
     _exit_exc_info: tuple[
@@ -142,15 +123,15 @@
         self._future.set_result(value)
 
 
 class BlockingPortal:
     """An object that lets external threads run code in an asynchronous event loop."""
 
     def __new__(cls) -> BlockingPortal:
-        return get_asynclib().BlockingPortal()
+        return get_async_backend().create_blocking_portal()
 
     def __init__(self) -> None:
         self._event_loop_thread_id: int | None = threading.get_ident()
         self._stop_event = Event()
         self._task_group = create_task_group()
         self._cancelled_exc_class = get_cancelled_exc_class()
 
@@ -182,16 +163,16 @@
     async def stop(self, cancel_remaining: bool = False) -> None:
         """
         Signal the portal to shut down.
 
         This marks the portal as no longer accepting new calls and exits from
         :meth:`sleep_until_stopped`.
 
-        :param cancel_remaining: ``True`` to cancel all the remaining tasks, ``False`` to let them
-            finish before returning
+        :param cancel_remaining: ``True`` to cancel all the remaining tasks, ``False``
+            to let them finish before returning
 
         """
         self._event_loop_thread_id = None
         self._stop_event.set()
         if cancel_remaining:
             self._task_group.cancel_scope.cancel()
 
@@ -203,24 +184,25 @@
                 None,
                 threading.get_ident(),
             ):
                 self.call(scope.cancel)
 
         try:
             retval = func(*args, **kwargs)
-            if iscoroutine(retval):
+            if isawaitable(retval):
                 with CancelScope() as scope:
                     if future.cancelled():
                         scope.cancel()
                     else:
                         future.add_done_callback(callback)
 
                     retval = await retval
         except self._cancelled_exc_class:
             future.cancel()
+            future.set_running_or_notify_cancel()
         except BaseException as exc:
             if not future.cancelled():
                 future.set_exception(exc)
 
             # Let base exceptions fall through
             if not isinstance(exc, Exception):
                 raise
@@ -229,102 +211,60 @@
                 future.set_result(retval)
         finally:
             scope = None  # type: ignore[assignment]
 
     def _spawn_task_from_thread(
         self,
         func: Callable,
-        args: tuple,
+        args: tuple[Any, ...],
         kwargs: dict[str, Any],
         name: object,
         future: Future,
     ) -> None:
         """
         Spawn a new task using the given callable.
 
         Implementors must ensure that the future is resolved when the task finishes.
 
         :param func: a callable
         :param args: positional arguments to be passed to the callable
         :param kwargs: keyword arguments to be passed to the callable
         :param name: name of the task (will be coerced to a string if not ``None``)
-        :param future: a future that will resolve to the return value of the callable, or the
-            exception raised during its execution
+        :param future: a future that will resolve to the return value of the callable,
+            or the exception raised during its execution
 
         """
         raise NotImplementedError
 
     @overload
     def call(self, func: Callable[..., Awaitable[T_Retval]], *args: object) -> T_Retval:
         ...
 
     @overload
     def call(self, func: Callable[..., T_Retval], *args: object) -> T_Retval:
         ...
 
     def call(
-        self, func: Callable[..., Awaitable[T_Retval] | T_Retval], *args: object
+        self,
+        func: Callable[..., Awaitable[T_Retval] | T_Retval],
+        *args: object,
     ) -> T_Retval:
         """
         Call the given function in the event loop thread.
 
         If the callable returns a coroutine object, it is awaited on.
 
         :param func: any callable
-        :raises RuntimeError: if the portal is not running or if this method is called from within
-            the event loop thread
+        :raises RuntimeError: if the portal is not running or if this method is called
+            from within the event loop thread
 
         """
         return cast(T_Retval, self.start_task_soon(func, *args).result())
 
     @overload
-    def spawn_task(
-        self,
-        func: Callable[..., Awaitable[T_Retval]],
-        *args: object,
-        name: object = None,
-    ) -> Future[T_Retval]:
-        ...
-
-    @overload
-    def spawn_task(
-        self, func: Callable[..., T_Retval], *args: object, name: object = None
-    ) -> Future[T_Retval]:
-        ...
-
-    def spawn_task(
-        self,
-        func: Callable[..., Awaitable[T_Retval] | T_Retval],
-        *args: object,
-        name: object = None,
-    ) -> Future[T_Retval]:
-        """
-        Start a task in the portal's task group.
-
-        :param func: the target coroutine function
-        :param args: positional arguments passed to ``func``
-        :param name: name of the task (will be coerced to a string if not ``None``)
-        :return: a future that resolves with the return value of the callable if the task completes
-            successfully, or with the exception raised in the task
-        :raises RuntimeError: if the portal is not running or if this method is called from within
-            the event loop thread
-
-        .. versionadded:: 2.1
-        .. deprecated:: 3.0
-           Use :meth:`start_task_soon` instead. If your code needs AnyIO 2 compatibility, you
-           can keep using this until AnyIO 4.
-
-        """
-        warn(
-            "spawn_task() is deprecated -- use start_task_soon() instead",
-            DeprecationWarning,
-        )
-        return self.start_task_soon(func, *args, name=name)  # type: ignore[arg-type]
-
-    @overload
     def start_task_soon(
         self,
         func: Callable[..., Awaitable[T_Retval]],
         *args: object,
         name: object = None,
     ) -> Future[T_Retval]:
         ...
@@ -340,16 +280,16 @@
         func: Callable[..., Awaitable[T_Retval] | T_Retval],
         *args: object,
         name: object = None,
     ) -> Future[T_Retval]:
         """
         Start a task in the portal's task group.
 
-        The task will be run inside a cancel scope which can be cancelled by cancelling the
-        returned future.
+        The task will be run inside a cancel scope which can be cancelled by cancelling
+        the returned future.
 
         :param func: the target function
         :param args: positional arguments passed to ``func``
         :param name: name of the task (will be coerced to a string if not ``None``)
         :return: a future that resolves with the return value of the callable if the
             task completes successfully, or with the exception raised in the task
         :raises RuntimeError: if the portal is not running or if this method is called
@@ -361,15 +301,18 @@
         """
         self._check_running()
         f: Future = Future()
         self._spawn_task_from_thread(func, args, {}, name, f)
         return f
 
     def start_task(
-        self, func: Callable[..., Awaitable[Any]], *args: object, name: object = None
+        self,
+        func: Callable[..., Awaitable[Any]],
+        *args: object,
+        name: object = None,
     ) -> tuple[Future[Any], Any]:
         """
         Start a task in the portal's task group and wait until it signals for readiness.
 
         This method works the same way as :meth:`.abc.TaskGroup.start`.
 
         :param func: the target function
@@ -406,45 +349,26 @@
 
     def wrap_async_context_manager(
         self, cm: AsyncContextManager[T_co]
     ) -> ContextManager[T_co]:
         """
         Wrap an async context manager as a synchronous context manager via this portal.
 
-        Spawns a task that will call both ``__aenter__()`` and ``__aexit__()``, stopping in the
-        middle until the synchronous context manager exits.
+        Spawns a task that will call both ``__aenter__()`` and ``__aexit__()``, stopping
+        in the middle until the synchronous context manager exits.
 
         :param cm: an asynchronous context manager
         :return: a synchronous context manager
 
         .. versionadded:: 2.1
 
         """
         return _BlockingAsyncContextManager(cm, self)
 
 
-def create_blocking_portal() -> BlockingPortal:
-    """
-    Create a portal for running functions in the event loop thread from external threads.
-
-    Use this function in asynchronous code when you need to allow external threads access to the
-    event loop where your asynchronous code is currently running.
-
-    .. deprecated:: 3.0
-        Use :class:`.BlockingPortal` directly.
-
-    """
-    warn(
-        "create_blocking_portal() has been deprecated -- use anyio.from_thread.BlockingPortal() "
-        "directly",
-        DeprecationWarning,
-    )
-    return BlockingPortal()
-
-
 @contextmanager
 def start_blocking_portal(
     backend: str = "asyncio", backend_options: dict[str, Any] | None = None
 ) -> Generator[BlockingPortal, Any, None]:
     """
     Start a new event loop in a new thread and run a blocking portal in its main task.
```

### Comparing `anyio-3.7.1/src/anyio/lowlevel.py` & `anyio-4.0.0rc1/src/anyio/lowlevel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 from __future__ import annotations
 
 import enum
-import sys
 from dataclasses import dataclass
-from typing import Any, Generic, TypeVar, overload
+from typing import Any, Generic, Literal, TypeVar, overload
 from weakref import WeakKeyDictionary
 
-from ._core._eventloop import get_asynclib
-
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
+from ._core._eventloop import get_async_backend
 
 T = TypeVar("T")
 D = TypeVar("D")
 
 
 async def checkpoint() -> None:
     """
@@ -26,27 +20,27 @@
         await checkpoint_if_cancelled()
         await cancel_shielded_checkpoint()
 
 
     .. versionadded:: 3.0
 
     """
-    await get_asynclib().checkpoint()
+    await get_async_backend().checkpoint()
 
 
 async def checkpoint_if_cancelled() -> None:
     """
     Enter a checkpoint if the enclosing cancel scope has been cancelled.
 
     This does not allow the scheduler to switch to a different task.
 
     .. versionadded:: 3.0
 
     """
-    await get_asynclib().checkpoint_if_cancelled()
+    await get_async_backend().checkpoint_if_cancelled()
 
 
 async def cancel_shielded_checkpoint() -> None:
     """
     Allow the scheduler to switch to another task but without checking for cancellation.
 
     Equivalent to (but potentially more efficient than)::
@@ -54,20 +48,24 @@
         with CancelScope(shield=True):
             await checkpoint()
 
 
     .. versionadded:: 3.0
 
     """
-    await get_asynclib().cancel_shielded_checkpoint()
+    await get_async_backend().cancel_shielded_checkpoint()
 
 
 def current_token() -> object:
-    """Return a backend specific token object that can be used to get back to the event loop."""
-    return get_asynclib().current_token()
+    """
+    Return a backend specific token object that can be used to get back to the event
+    loop.
+
+    """
+    return get_async_backend().current_token()
 
 
 _run_vars: WeakKeyDictionary[Any, dict[str, Any]] = WeakKeyDictionary()
 _token_wrappers: dict[Any, _TokenWrapper] = {}
 
 
 @dataclass(frozen=True)
@@ -97,36 +95,27 @@
     __slots__ = "_name", "_default"
 
     NO_VALUE_SET: Literal[_NoValueSet.NO_VALUE_SET] = _NoValueSet.NO_VALUE_SET
 
     _token_wrappers: set[_TokenWrapper] = set()
 
     def __init__(
-        self,
-        name: str,
-        default: T | Literal[_NoValueSet.NO_VALUE_SET] = NO_VALUE_SET,
+        self, name: str, default: T | Literal[_NoValueSet.NO_VALUE_SET] = NO_VALUE_SET
     ):
         self._name = name
         self._default = default
 
     @property
     def _current_vars(self) -> dict[str, T]:
         token = current_token()
-        while True:
-            try:
-                return _run_vars[token]
-            except TypeError:
-                # Happens when token isn't weak referable (TrioToken).
-                # This workaround does mean that some memory will leak on Trio until the problem
-                # is fixed on their end.
-                token = _TokenWrapper(token)
-                self._token_wrappers.add(token)
-            except KeyError:
-                run_vars = _run_vars[token] = {}
-                return run_vars
+        try:
+            return _run_vars[token]
+        except KeyError:
+            run_vars = _run_vars[token] = {}
+            return run_vars
 
     @overload
     def get(self, default: D) -> T | D:
         ...
 
     @overload
     def get(self) -> T:
```

### Comparing `anyio-3.7.1/src/anyio/pytest_plugin.py` & `anyio-4.0.0rc1/src/anyio/pytest_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
+from collections.abc import Iterator
 from contextlib import contextmanager
 from inspect import isasyncgenfunction, iscoroutinefunction
-from typing import Any, Dict, Generator, Tuple, cast
+from typing import Any, Dict, Tuple, cast
 
 import pytest
 import sniffio
 
-from ._core._eventloop import get_all_backends, get_asynclib
+from ._core._eventloop import get_all_backends, get_async_backend
 from .abc import TestRunner
 
 _current_runner: TestRunner | None = None
 
 
 def extract_backend_and_options(backend: object) -> tuple[str, dict[str, Any]]:
     if isinstance(backend, str):
@@ -22,29 +23,30 @@
 
     raise TypeError("anyio_backend must be either a string or tuple of (string, dict)")
 
 
 @contextmanager
 def get_runner(
     backend_name: str, backend_options: dict[str, Any]
-) -> Generator[TestRunner, object, None]:
+) -> Iterator[TestRunner]:
     global _current_runner
     if _current_runner:
         yield _current_runner
         return
 
-    asynclib = get_asynclib(backend_name)
+    asynclib = get_async_backend(backend_name)
     token = None
     if sniffio.current_async_library_cvar.get(None) is None:
-        # Since we're in control of the event loop, we can cache the name of the async library
+        # Since we're in control of the event loop, we can cache the name of the async
+        # library
         token = sniffio.current_async_library_cvar.set(backend_name)
 
     try:
         backend_options = backend_options or {}
-        with asynclib.TestRunner(**backend_options) as runner:
+        with asynclib.create_test_runner(backend_options) as runner:
             _current_runner = runner
             yield runner
     finally:
         _current_runner = None
         if token:
             sniffio.current_async_library_cvar.reset(token)
 
@@ -65,16 +67,16 @@
 
         with get_runner(backend_name, backend_options) as runner:
             if isasyncgenfunction(func):
                 yield from runner.run_asyncgen_fixture(func, kwargs)
             else:
                 yield runner.run_fixture(func, kwargs)
 
-    # Only apply this to coroutine functions and async generator functions in requests that involve
-    # the anyio_backend fixture
+    # Only apply this to coroutine functions and async generator functions in requests
+    # that involve the anyio_backend fixture
     func = fixturedef.func
     if isasyncgenfunction(func) or iscoroutinefunction(func):
         if "anyio_backend" in request.fixturenames:
             has_backend_arg = "anyio_backend" in fixturedef.argnames
             fixturedef.func = wrapper
             if not has_backend_arg:
                 fixturedef.argnames += ("anyio_backend",)
@@ -117,15 +119,15 @@
                 runner.run_test(pyfuncitem.obj, testargs)
 
             return True
 
     return None
 
 
-@pytest.fixture(params=get_all_backends())
+@pytest.fixture(scope="module", params=get_all_backends())
 def anyio_backend(request: Any) -> Any:
     return request.param
 
 
 @pytest.fixture
 def anyio_backend_name(anyio_backend: Any) -> str:
     if isinstance(anyio_backend, str):
```

### Comparing `anyio-3.7.1/src/anyio/streams/buffered.py` & `anyio-4.0.0rc1/src/anyio/streams/buffered.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
+from collections.abc import Callable, Mapping
 from dataclasses import dataclass, field
-from typing import Any, Callable, Mapping
+from typing import Any
 
 from .. import ClosedResourceError, DelimiterNotFound, EndOfStream, IncompleteRead
 from ..abc import AnyByteReceiveStream, ByteReceiveStream
 
 
 @dataclass(eq=False)
 class BufferedByteReceiveStream(ByteReceiveStream):
     """
-    Wraps any bytes-based receive stream and uses a buffer to provide sophisticated receiving
-    capabilities in the form of a byte stream.
+    Wraps any bytes-based receive stream and uses a buffer to provide sophisticated
+    receiving capabilities in the form of a byte stream.
     """
 
     receive_stream: AnyByteReceiveStream
     _buffer: bytearray = field(init=False, default_factory=bytearray)
     _closed: bool = field(init=False, default=False)
 
     async def aclose(self) -> None:
@@ -38,16 +39,16 @@
         if self._buffer:
             chunk = bytes(self._buffer[:max_bytes])
             del self._buffer[:max_bytes]
             return chunk
         elif isinstance(self.receive_stream, ByteReceiveStream):
             return await self.receive_stream.receive(max_bytes)
         else:
-            # With a bytes-oriented object stream, we need to handle any surplus bytes we get from
-            # the receive() call
+            # With a bytes-oriented object stream, we need to handle any surplus bytes
+            # we get from the receive() call
             chunk = await self.receive_stream.receive()
             if len(chunk) > max_bytes:
                 # Save the surplus bytes in the buffer
                 self._buffer.extend(chunk[max_bytes:])
                 return chunk[:max_bytes]
             else:
                 return chunk
```

### Comparing `anyio-3.7.1/src/anyio/streams/file.py` & `anyio-4.0.0rc1/src/anyio/streams/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
+from collections.abc import Callable, Mapping
 from io import SEEK_SET, UnsupportedOperation
 from os import PathLike
 from pathlib import Path
-from typing import Any, BinaryIO, Callable, Mapping, cast
+from typing import Any, BinaryIO, cast
 
 from .. import (
     BrokenResourceError,
     ClosedResourceError,
     EndOfStream,
     TypedAttributeSet,
     to_thread,
@@ -126,16 +127,16 @@
     async def from_path(
         cls, path: str | PathLike[str], append: bool = False
     ) -> FileWriteStream:
         """
         Create a file write stream by opening the given file for writing.
 
         :param path: path of the file to write to
-        :param append: if ``True``, open the file for appending; if ``False``, any existing file
-            at the given path will be truncated
+        :param append: if ``True``, open the file for appending; if ``False``, any
+            existing file at the given path will be truncated
 
         """
         mode = "ab" if append else "wb"
         file = await to_thread.run_sync(Path(path).open, mode)
         return cls(cast(BinaryIO, file))
 
     async def send(self, item: bytes) -> None:
```

### Comparing `anyio-3.7.1/src/anyio/streams/memory.py` & `anyio-4.0.0rc1/src/anyio/streams/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,32 +6,31 @@
 from typing import Generic, NamedTuple, TypeVar
 
 from .. import (
     BrokenResourceError,
     ClosedResourceError,
     EndOfStream,
     WouldBlock,
-    get_cancelled_exc_class,
 )
-from .._core._compat import DeprecatedAwaitable
 from ..abc import Event, ObjectReceiveStream, ObjectSendStream
 from ..lowlevel import checkpoint
 
 T_Item = TypeVar("T_Item")
 T_co = TypeVar("T_co", covariant=True)
 T_contra = TypeVar("T_contra", contravariant=True)
 
 
 class MemoryObjectStreamStatistics(NamedTuple):
     current_buffer_used: int  #: number of items stored in the buffer
     #: maximum number of items that can be stored on this stream (or :data:`math.inf`)
     max_buffer_size: float
     open_send_streams: int  #: number of unclosed clones of the send stream
     open_receive_streams: int  #: number of unclosed clones of the receive stream
-    tasks_waiting_send: int  #: number of tasks blocked on :meth:`MemoryObjectSendStream.send`
+    #: number of tasks blocked on :meth:`MemoryObjectSendStream.send`
+    tasks_waiting_send: int
     #: number of tasks blocked on :meth:`MemoryObjectReceiveStream.receive`
     tasks_waiting_receive: int
 
 
 @dataclass(eq=False)
 class MemoryObjectStreamState(Generic[T_Item]):
     max_buffer_size: float = field()
@@ -100,48 +99,43 @@
             # Add ourselves in the queue
             receive_event = Event()
             container: list[T_co] = []
             self._state.waiting_receivers[receive_event] = container
 
             try:
                 await receive_event.wait()
-            except get_cancelled_exc_class():
-                # Ignore the immediate cancellation if we already received an item, so as not to
-                # lose it
-                if not container:
-                    raise
             finally:
                 self._state.waiting_receivers.pop(receive_event, None)
 
             if container:
                 return container[0]
             else:
                 raise EndOfStream
 
     def clone(self) -> MemoryObjectReceiveStream[T_co]:
         """
         Create a clone of this receive stream.
 
-        Each clone can be closed separately. Only when all clones have been closed will the
-        receiving end of the memory stream be considered closed by the sending ends.
+        Each clone can be closed separately. Only when all clones have been closed will
+        the receiving end of the memory stream be considered closed by the sending ends.
 
         :return: the cloned stream
 
         """
         if self._closed:
             raise ClosedResourceError
 
         return MemoryObjectReceiveStream(_state=self._state)
 
     def close(self) -> None:
         """
         Close the stream.
 
-        This works the exact same way as :meth:`aclose`, but is provided as a special case for the
-        benefit of synchronous callbacks.
+        This works the exact same way as :meth:`aclose`, but is provided as a special
+        case for the benefit of synchronous callbacks.
 
         """
         if not self._closed:
             self._closed = True
             self._state.open_receive_channels -= 1
             if self._state.open_receive_channels == 0:
                 send_events = list(self._state.waiting_senders.keys())
@@ -175,15 +169,15 @@
 class MemoryObjectSendStream(Generic[T_contra], ObjectSendStream[T_contra]):
     _state: MemoryObjectStreamState[T_contra]
     _closed: bool = field(init=False, default=False)
 
     def __post_init__(self) -> None:
         self._state.open_send_channels += 1
 
-    def send_nowait(self, item: T_contra) -> DeprecatedAwaitable:
+    def send_nowait(self, item: T_contra) -> None:
         """
         Send an item immediately if it can be done without waiting.
 
         :param item: the item to send
         :raises ~anyio.ClosedResourceError: if this send stream has been closed
         :raises ~anyio.BrokenResourceError: if the stream has been closed from the
             receiving end
@@ -201,54 +195,68 @@
             container.append(item)
             receive_event.set()
         elif len(self._state.buffer) < self._state.max_buffer_size:
             self._state.buffer.append(item)
         else:
             raise WouldBlock
 
-        return DeprecatedAwaitable(self.send_nowait)
-
     async def send(self, item: T_contra) -> None:
+        """
+        Send an item to the stream.
+
+        If the buffer is full, this method blocks until there is again room in the
+        buffer or the item can be sent directly to a receiver.
+
+        :param item: the item to send
+        :raises ~anyio.ClosedResourceError: if this send stream has been closed
+        :raises ~anyio.BrokenResourceError: if the stream has been closed from the
+            receiving end
+
+        """
         await checkpoint()
         try:
             self.send_nowait(item)
         except WouldBlock:
             # Wait until there's someone on the receiving end
             send_event = Event()
             self._state.waiting_senders[send_event] = item
             try:
                 await send_event.wait()
             except BaseException:
-                self._state.waiting_senders.pop(send_event, None)  # type: ignore[arg-type]
+                self._state.waiting_senders.pop(
+                    send_event, None  # type: ignore[arg-type]
+                )
                 raise
 
-            if self._state.waiting_senders.pop(send_event, None):  # type: ignore[arg-type]
-                raise BrokenResourceError
+            if self._state.waiting_senders.pop(
+                send_event, None  # type: ignore[arg-type]
+            ):
+                raise BrokenResourceError from None
 
     def clone(self) -> MemoryObjectSendStream[T_contra]:
         """
         Create a clone of this send stream.
 
-        Each clone can be closed separately. Only when all clones have been closed will the
-        sending end of the memory stream be considered closed by the receiving ends.
+        Each clone can be closed separately. Only when all clones have been closed will
+        the sending end of the memory stream be considered closed by the receiving ends.
 
         :return: the cloned stream
 
         """
         if self._closed:
             raise ClosedResourceError
 
         return MemoryObjectSendStream(_state=self._state)
 
     def close(self) -> None:
         """
         Close the stream.
 
-        This works the exact same way as :meth:`aclose`, but is provided as a special case for the
-        benefit of synchronous callbacks.
+        This works the exact same way as :meth:`aclose`, but is provided as a special
+        case for the benefit of synchronous callbacks.
 
         """
         if not self._closed:
             self._closed = True
             self._state.open_send_channels -= 1
             if self._state.open_send_channels == 0:
                 receive_events = list(self._state.waiting_receivers.keys())
```

### Comparing `anyio-3.7.1/src/anyio/streams/stapled.py` & `anyio-4.0.0rc1/src/anyio/streams/stapled.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
+from collections.abc import Callable, Mapping, Sequence
 from dataclasses import dataclass
-from typing import Any, Callable, Generic, Mapping, Sequence, TypeVar
+from typing import Any, Generic, TypeVar
 
 from ..abc import (
     ByteReceiveStream,
     ByteSendStream,
     ByteStream,
     Listener,
     ObjectReceiveStream,
@@ -19,16 +20,16 @@
 
 
 @dataclass(eq=False)
 class StapledByteStream(ByteStream):
     """
     Combines two byte streams into a single, bidirectional byte stream.
 
-    Extra attributes will be provided from both streams, with the receive stream providing the
-    values in case of a conflict.
+    Extra attributes will be provided from both streams, with the receive stream
+    providing the values in case of a conflict.
 
     :param ByteSendStream send_stream: the sending byte stream
     :param ByteReceiveStream receive_stream: the receiving byte stream
     """
 
     send_stream: ByteSendStream
     receive_stream: ByteReceiveStream
@@ -55,16 +56,16 @@
 
 
 @dataclass(eq=False)
 class StapledObjectStream(Generic[T_Item], ObjectStream[T_Item]):
     """
     Combines two object streams into a single, bidirectional object stream.
 
-    Extra attributes will be provided from both streams, with the receive stream providing the
-    values in case of a conflict.
+    Extra attributes will be provided from both streams, with the receive stream
+    providing the values in case of a conflict.
 
     :param ObjectSendStream send_stream: the sending object stream
     :param ObjectReceiveStream receive_stream: the receiving object stream
     """
 
     send_stream: ObjectSendStream[T_Item]
     receive_stream: ObjectReceiveStream[T_Item]
@@ -91,19 +92,19 @@
 
 
 @dataclass(eq=False)
 class MultiListener(Generic[T_Stream], Listener[T_Stream]):
     """
     Combines multiple listeners into one, serving connections from all of them at once.
 
-    Any MultiListeners in the given collection of listeners will have their listeners moved into
-    this one.
+    Any MultiListeners in the given collection of listeners will have their listeners
+    moved into this one.
 
-    Extra attributes are provided from each listener, with each successive listener overriding any
-    conflicting attributes from the previous one.
+    Extra attributes are provided from each listener, with each successive listener
+    overriding any conflicting attributes from the previous one.
 
     :param listeners: listeners to serve
     :type listeners: Sequence[Listener[T_Stream]]
     """
 
     listeners: Sequence[Listener[T_Stream]]
```

### Comparing `anyio-3.7.1/src/anyio/streams/text.py` & `anyio-4.0.0rc1/src/anyio/streams/text.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import codecs
+from collections.abc import Callable, Mapping
 from dataclasses import InitVar, dataclass, field
-from typing import Any, Callable, Mapping
+from typing import Any
 
 from ..abc import (
     AnyByteReceiveStream,
     AnyByteSendStream,
     AnyByteStream,
     ObjectReceiveStream,
     ObjectSendStream,
@@ -15,24 +16,25 @@
 
 
 @dataclass(eq=False)
 class TextReceiveStream(ObjectReceiveStream[str]):
     """
     Stream wrapper that decodes bytes to strings using the given encoding.
 
-    Decoding is done using :class:`~codecs.IncrementalDecoder` which returns any completely
-    received unicode characters as soon as they come in.
+    Decoding is done using :class:`~codecs.IncrementalDecoder` which returns any
+    completely received unicode characters as soon as they come in.
 
     :param transport_stream: any bytes-based receive stream
-    :param encoding: character encoding to use for decoding bytes to strings (defaults to
-        ``utf-8``)
+    :param encoding: character encoding to use for decoding bytes to strings (defaults
+        to ``utf-8``)
     :param errors: handling scheme for decoding errors (defaults to ``strict``; see the
         `codecs module documentation`_ for a comprehensive list of options)
 
-    .. _codecs module documentation: https://docs.python.org/3/library/codecs.html#codec-objects
+    .. _codecs module documentation:
+        https://docs.python.org/3/library/codecs.html#codec-objects
     """
 
     transport_stream: AnyByteReceiveStream
     encoding: InitVar[str] = "utf-8"
     errors: InitVar[str] = "strict"
     _decoder: codecs.IncrementalDecoder = field(init=False)
 
@@ -58,20 +60,21 @@
 
 @dataclass(eq=False)
 class TextSendStream(ObjectSendStream[str]):
     """
     Sends strings to the wrapped stream as bytes using the given encoding.
 
     :param AnyByteSendStream transport_stream: any bytes-based send stream
-    :param str encoding: character encoding to use for encoding strings to bytes (defaults to
-        ``utf-8``)
-    :param str errors: handling scheme for encoding errors (defaults to ``strict``; see the
-        `codecs module documentation`_ for a comprehensive list of options)
+    :param str encoding: character encoding to use for encoding strings to bytes
+        (defaults to ``utf-8``)
+    :param str errors: handling scheme for encoding errors (defaults to ``strict``; see
+        the `codecs module documentation`_ for a comprehensive list of options)
 
-    .. _codecs module documentation: https://docs.python.org/3/library/codecs.html#codec-objects
+    .. _codecs module documentation:
+        https://docs.python.org/3/library/codecs.html#codec-objects
     """
 
     transport_stream: AnyByteSendStream
     encoding: InitVar[str] = "utf-8"
     errors: str = "strict"
     _encoder: Callable[..., tuple[bytes, int]] = field(init=False)
 
@@ -89,27 +92,28 @@
     def extra_attributes(self) -> Mapping[Any, Callable[[], Any]]:
         return self.transport_stream.extra_attributes
 
 
 @dataclass(eq=False)
 class TextStream(ObjectStream[str]):
     """
-    A bidirectional stream that decodes bytes to strings on receive and encodes strings to bytes on
-    send.
+    A bidirectional stream that decodes bytes to strings on receive and encodes strings
+    to bytes on send.
 
-    Extra attributes will be provided from both streams, with the receive stream providing the
-    values in case of a conflict.
+    Extra attributes will be provided from both streams, with the receive stream
+    providing the values in case of a conflict.
 
     :param AnyByteStream transport_stream: any bytes-based stream
-    :param str encoding: character encoding to use for encoding/decoding strings to/from bytes
-        (defaults to ``utf-8``)
-    :param str errors: handling scheme for encoding errors (defaults to ``strict``; see the
-        `codecs module documentation`_ for a comprehensive list of options)
+    :param str encoding: character encoding to use for encoding/decoding strings to/from
+        bytes (defaults to ``utf-8``)
+    :param str errors: handling scheme for encoding errors (defaults to ``strict``; see
+        the `codecs module documentation`_ for a comprehensive list of options)
 
-    .. _codecs module documentation: https://docs.python.org/3/library/codecs.html#codec-objects
+    .. _codecs module documentation:
+        https://docs.python.org/3/library/codecs.html#codec-objects
     """
 
     transport_stream: AnyByteStream
     encoding: InitVar[str] = "utf-8"
     errors: InitVar[str] = "strict"
     _receive_stream: TextReceiveStream = field(init=False)
     _send_stream: TextSendStream = field(init=False)
```

### Comparing `anyio-3.7.1/src/anyio/streams/tls.py` & `anyio-4.0.0rc1/src/anyio/streams/tls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import logging
 import re
 import ssl
+from collections.abc import Callable, Mapping
 from dataclasses import dataclass
 from functools import wraps
-from typing import Any, Callable, Mapping, Tuple, TypeVar
+from typing import Any, Tuple, TypeVar
 
 from .. import (
     BrokenResourceError,
     EndOfStream,
     aclose_forcefully,
     get_cancelled_exc_class,
 )
@@ -27,16 +28,16 @@
     #: the selected ALPN protocol
     alpn_protocol: str | None = typed_attribute()
     #: the channel binding for type ``tls-unique``
     channel_binding_tls_unique: bytes = typed_attribute()
     #: the selected cipher
     cipher: tuple[str, str, int] = typed_attribute()
     #: the peer certificate in dictionary form (see :meth:`ssl.SSLSocket.getpeercert`
-    #: for more information)
-    peer_certificate: dict[str, str | _PCTRTTT | _PCTRTT] | None = typed_attribute()
+    # for more information)
+    peer_certificate: None | (dict[str, str | _PCTRTTT | _PCTRTT]) = typed_attribute()
     #: the peer certificate in binary form
     peer_certificate_binary: bytes | None = typed_attribute()
     #: ``True`` if this is the server side of the connection
     server_side: bool = typed_attribute()
     #: ciphers shared by the client during the TLS handshake (``None`` if this is the
     #: client side)
     shared_ciphers: list[tuple[str, str, int]] | None = typed_attribute()
@@ -86,16 +87,17 @@
         :param server_side: ``True`` if this is the server side of the connection,
             ``False`` if this is the client side (if omitted, will be set to ``False``
             if ``hostname`` has been provided, ``False`` otherwise). Used only to create
             a default context when an explicit context has not been provided.
         :param hostname: host name of the peer (if host name checking is desired)
         :param ssl_context: the SSLContext object to use (if not provided, a secure
             default will be created)
-        :param standard_compatible: if ``False``, skip the closing handshake when closing the
-            connection, and don't raise an exception if the peer does the same
+        :param standard_compatible: if ``False``, skip the closing handshake when
+            closing the connection, and don't raise an exception if the peer does the
+            same
         :raises ~ssl.SSLError: if the TLS handshake fails
 
         """
         if server_side is None:
             server_side = not hostname
 
         if not ssl_context:
@@ -218,15 +220,17 @@
         )
 
     @property
     def extra_attributes(self) -> Mapping[Any, Callable[[], Any]]:
         return {
             **self.transport_stream.extra_attributes,
             TLSAttribute.alpn_protocol: self._ssl_object.selected_alpn_protocol,
-            TLSAttribute.channel_binding_tls_unique: self._ssl_object.get_channel_binding,
+            TLSAttribute.channel_binding_tls_unique: (
+                self._ssl_object.get_channel_binding
+            ),
             TLSAttribute.cipher: self._ssl_object.cipher,
             TLSAttribute.peer_certificate: lambda: self._ssl_object.getpeercert(False),
             TLSAttribute.peer_certificate_binary: lambda: self._ssl_object.getpeercert(
                 True
             ),
             TLSAttribute.server_side: lambda: self._ssl_object.server_side,
             TLSAttribute.shared_ciphers: lambda: self._ssl_object.shared_ciphers()
@@ -237,19 +241,20 @@
             TLSAttribute.tls_version: self._ssl_object.version,
         }
 
 
 @dataclass(eq=False)
 class TLSListener(Listener[TLSStream]):
     """
-    A convenience listener that wraps another listener and auto-negotiates a TLS session on every
-    accepted connection.
+    A convenience listener that wraps another listener and auto-negotiates a TLS session
+    on every accepted connection.
 
-    If the TLS handshake times out or raises an exception, :meth:`handle_handshake_error` is
-    called to do whatever post-mortem processing is deemed necessary.
+    If the TLS handshake times out or raises an exception,
+    :meth:`handle_handshake_error` is called to do whatever post-mortem processing is
+    deemed necessary.
 
     Supports only the :attr:`~TLSAttribute.standard_compatible` extra attribute.
 
     :param Listener listener: the listener to wrap
     :param ssl_context: the SSL context object
     :param standard_compatible: a flag passed through to :meth:`TLSStream.wrap`
     :param handshake_timeout: time limit for the TLS handshake
```

### Comparing `anyio-3.7.1/src/anyio/to_process.py` & `anyio-4.0.0rc1/src/anyio/to_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import os
 import pickle
 import subprocess
 import sys
 from collections import deque
+from collections.abc import Callable
 from importlib.util import module_from_spec, spec_from_file_location
-from typing import Callable, TypeVar, cast
+from typing import TypeVar, cast
 
-from ._core._eventloop import current_time, get_asynclib, get_cancelled_exc_class
+from ._core._eventloop import current_time, get_async_backend, get_cancelled_exc_class
 from ._core._exceptions import BrokenWorkerProcess
 from ._core._subprocesses import open_process
 from ._core._synchronization import CapacityLimiter
 from ._core._tasks import CancelScope, fail_after
 from .abc import ByteReceiveStream, ByteSendStream, Process
 from .lowlevel import RunVar, checkpoint_if_cancelled
 from .streams.buffered import BufferedByteReceiveStream
@@ -32,23 +33,24 @@
     *args: object,
     cancellable: bool = False,
     limiter: CapacityLimiter | None = None,
 ) -> T_Retval:
     """
     Call the given function with the given arguments in a worker process.
 
-    If the ``cancellable`` option is enabled and the task waiting for its completion is cancelled,
-    the worker process running it will be abruptly terminated using SIGKILL (or
-    ``terminateProcess()`` on Windows).
+    If the ``cancellable`` option is enabled and the task waiting for its completion is
+    cancelled, the worker process running it will be abruptly terminated using SIGKILL
+    (or ``terminateProcess()`` on Windows).
 
     :param func: a callable
     :param args: positional arguments for the callable
-    :param cancellable: ``True`` to allow cancellation of the operation while it's running
-    :param limiter: capacity limiter to use to limit the total amount of processes running
-        (if omitted, the default limiter is used)
+    :param cancellable: ``True`` to allow cancellation of the operation while it's
+        running
+    :param limiter: capacity limiter to use to limit the total amount of processes
+        running (if omitted, the default limiter is used)
     :return: an awaitable that yields the return value of the function.
 
     """
 
     async def send_raw_command(pickled_cmd: bytes) -> object:
         try:
             await stdin.send(pickled_cmd)
@@ -90,30 +92,30 @@
         workers = _process_pool_workers.get()
         idle_workers = _process_pool_idle_workers.get()
     except LookupError:
         workers = set()
         idle_workers = deque()
         _process_pool_workers.set(workers)
         _process_pool_idle_workers.set(idle_workers)
-        get_asynclib().setup_process_pool_exit_at_shutdown(workers)
+        get_async_backend().setup_process_pool_exit_at_shutdown(workers)
 
     async with (limiter or current_default_process_limiter()):
-        # Pop processes from the pool (starting from the most recently used) until we find one that
-        # hasn't exited yet
+        # Pop processes from the pool (starting from the most recently used) until we
+        # find one that hasn't exited yet
         process: Process
         while idle_workers:
             process, idle_since = idle_workers.pop()
             if process.returncode is None:
                 stdin = cast(ByteSendStream, process.stdin)
                 buffered = BufferedByteReceiveStream(
                     cast(ByteReceiveStream, process.stdout)
                 )
 
-                # Prune any other workers that have been idle for WORKER_MAX_IDLE_TIME seconds or
-                # longer
+                # Prune any other workers that have been idle for WORKER_MAX_IDLE_TIME
+                # seconds or longer
                 now = current_time()
                 killed_processes: list[Process] = []
                 while idle_workers:
                     if now - idle_workers[0][1] < WORKER_MAX_IDLE_TIME:
                         break
 
                     process, idle_since = idle_workers.popleft()
@@ -168,15 +170,16 @@
             finally:
                 if process in workers:
                     idle_workers.append((process, current_time()))
 
 
 def current_default_process_limiter() -> CapacityLimiter:
     """
-    Return the capacity limiter that is used by default to limit the number of worker processes.
+    Return the capacity limiter that is used by default to limit the number of worker
+    processes.
 
     :return: a capacity limiter object
 
     """
     try:
         return _default_process_limiter.get()
     except LookupError:
@@ -210,16 +213,16 @@
                 except BaseException as exc:
                     exception = exc
             elif command == "init":
                 main_module_path: str | None
                 sys.path, main_module_path = args
                 del sys.modules["__main__"]
                 if main_module_path:
-                    # Load the parent's main module but as __mp_main__ instead of __main__
-                    # (like multiprocessing does) to avoid infinite recursion
+                    # Load the parent's main module but as __mp_main__ instead of
+                    # __main__ (like multiprocessing does) to avoid infinite recursion
                     try:
                         spec = spec_from_file_location("__mp_main__", main_module_path)
                         if spec and spec.loader:
                             main = module_from_spec(spec)
                             spec.loader.exec_module(main)
                             sys.modules["__main__"] = main
                     except BaseException as exc:
```

### Comparing `anyio-3.7.1/src/anyio.egg-info/PKG-INFO` & `anyio-4.0.0rc1/src/anyio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: anyio
-Version: 3.7.1
+Version: 4.0.0rc1
 Summary: High level compatibility layer for multiple asynchronous event loop implementations
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://anyio.readthedocs.io/en/latest/
 Project-URL: Changelog, https://anyio.readthedocs.io/en/stable/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/anyio
 Project-URL: Issue tracker, https://github.com/agronholm/anyio/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: AnyIO
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: trio
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 .. image:: https://github.com/agronholm/anyio/actions/workflows/test.yml/badge.svg
```

### Comparing `anyio-3.7.1/src/anyio.egg-info/SOURCES.txt` & `anyio-4.0.0rc1/src/anyio.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
 README.rst
 pyproject.toml
+.github/ISSUE_TEMPLATE/bug_report.yaml
+.github/ISSUE_TEMPLATE/config.yml
+.github/ISSUE_TEMPLATE/features_request.yaml
 .github/workflows/publish.yml
+.github/workflows/test-downstream.yml
 .github/workflows/test.yml
 docs/api.rst
 docs/basics.rst
 docs/cancellation.rst
 docs/conf.py
 docs/contributing.rst
 docs/faq.rst
@@ -39,28 +43,28 @@
 src/anyio.egg-info/entry_points.txt
 src/anyio.egg-info/requires.txt
 src/anyio.egg-info/top_level.txt
 src/anyio/_backends/__init__.py
 src/anyio/_backends/_asyncio.py
 src/anyio/_backends/_trio.py
 src/anyio/_core/__init__.py
-src/anyio/_core/_compat.py
 src/anyio/_core/_eventloop.py
 src/anyio/_core/_exceptions.py
 src/anyio/_core/_fileio.py
 src/anyio/_core/_resources.py
 src/anyio/_core/_signals.py
 src/anyio/_core/_sockets.py
 src/anyio/_core/_streams.py
 src/anyio/_core/_subprocesses.py
 src/anyio/_core/_synchronization.py
 src/anyio/_core/_tasks.py
 src/anyio/_core/_testing.py
 src/anyio/_core/_typedattr.py
 src/anyio/abc/__init__.py
+src/anyio/abc/_eventloop.py
 src/anyio/abc/_resources.py
 src/anyio/abc/_sockets.py
 src/anyio/abc/_streams.py
 src/anyio/abc/_subprocesses.py
 src/anyio/abc/_tasks.py
 src/anyio/abc/_testing.py
 src/anyio/streams/__init__.py
@@ -68,15 +72,14 @@
 src/anyio/streams/file.py
 src/anyio/streams/memory.py
 src/anyio/streams/stapled.py
 src/anyio/streams/text.py
 src/anyio/streams/tls.py
 tests/__init__.py
 tests/conftest.py
-tests/test_compat.py
 tests/test_debugging.py
 tests/test_eventloop.py
 tests/test_fileio.py
 tests/test_from_thread.py
 tests/test_lowlevel.py
 tests/test_pytest_plugin.py
 tests/test_signals.py
```

### Comparing `anyio-3.7.1/tests/conftest.py` & `anyio-4.0.0rc1/tests/conftest.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from __future__ import annotations
 
 import asyncio
 import ssl
+from collections.abc import Generator
 from ssl import SSLContext
-from typing import Any, Generator
+from typing import Any
+from unittest.mock import Mock
 
 import pytest
 import trustme
 from _pytest.fixtures import SubRequest
 from trustme import CA
 
 uvloop_marks = []
-uvloop_policy = None
 try:
     import uvloop
 except ImportError:
     uvloop_marks.append(pytest.mark.skip(reason="uvloop not available"))
+    uvloop = Mock()
 else:
     if hasattr(asyncio.AbstractEventLoop, "shutdown_default_executor") and not hasattr(
         uvloop.loop.Loop, "shutdown_default_executor"
     ):
         uvloop_marks.append(
             pytest.mark.skip(reason="uvloop is missing shutdown_default_executor()")
         )
-    else:
-        uvloop_policy = uvloop.EventLoopPolicy()
 
 pytest_plugins = ["pytester", "pytest_mock"]
 
 
 @pytest.fixture(
     params=[
         pytest.param(
-            ("asyncio", {"debug": True, "policy": asyncio.DefaultEventLoopPolicy()}),
+            ("asyncio", {"debug": True, "loop_factory": None}),
             id="asyncio",
         ),
         pytest.param(
-            ("asyncio", {"debug": True, "policy": uvloop_policy}),
+            ("asyncio", {"debug": True, "loop_factory": uvloop.new_event_loop}),
             marks=uvloop_marks,
             id="asyncio+uvloop",
         ),
         pytest.param("trio"),
     ]
 )
 def anyio_backend(request: SubRequest) -> tuple[str, dict[str, Any]]:
```

### Comparing `anyio-3.7.1/tests/streams/test_buffered.py` & `anyio-4.0.0rc1/tests/streams/test_buffered.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,49 +5,49 @@
 from anyio import IncompleteRead, create_memory_object_stream
 from anyio.streams.buffered import BufferedByteReceiveStream
 
 pytestmark = pytest.mark.anyio
 
 
 async def test_receive_exactly() -> None:
-    send_stream, receive_stream = create_memory_object_stream(2)
+    send_stream, receive_stream = create_memory_object_stream[bytes](2)
     buffered_stream = BufferedByteReceiveStream(receive_stream)
     await send_stream.send(b"abcd")
     await send_stream.send(b"efgh")
     result = await buffered_stream.receive_exactly(8)
     assert result == b"abcdefgh"
     assert isinstance(result, bytes)
 
 
 async def test_receive_exactly_incomplete() -> None:
-    send_stream, receive_stream = create_memory_object_stream(1)
+    send_stream, receive_stream = create_memory_object_stream[bytes](1)
     buffered_stream = BufferedByteReceiveStream(receive_stream)
     await send_stream.send(b"abcd")
     await send_stream.aclose()
     with pytest.raises(IncompleteRead):
         await buffered_stream.receive_exactly(8)
 
 
 async def test_receive_until() -> None:
-    send_stream, receive_stream = create_memory_object_stream(2)
+    send_stream, receive_stream = create_memory_object_stream[bytes](2)
     buffered_stream = BufferedByteReceiveStream(receive_stream)
     await send_stream.send(b"abcd")
     await send_stream.send(b"efgh")
 
     result = await buffered_stream.receive_until(b"de", 10)
     assert result == b"abc"
     assert isinstance(result, bytes)
 
     result = await buffered_stream.receive_until(b"h", 10)
     assert result == b"fg"
     assert isinstance(result, bytes)
 
 
 async def test_receive_until_incomplete() -> None:
-    send_stream, receive_stream = create_memory_object_stream(1)
+    send_stream, receive_stream = create_memory_object_stream[bytes](1)
     buffered_stream = BufferedByteReceiveStream(receive_stream)
     await send_stream.send(b"abcd")
     await send_stream.aclose()
     with pytest.raises(IncompleteRead):
         assert await buffered_stream.receive_until(b"de", 10)
 
     assert buffered_stream.buffer == b"abcd"
```

### Comparing `anyio-3.7.1/tests/streams/test_file.py` & `anyio-4.0.0rc1/tests/streams/test_file.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.1/tests/streams/test_memory.py` & `anyio-4.0.0rc1/tests/streams/test_memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from __future__ import annotations
 
+import sys
+from typing import NoReturn
+
 import pytest
 
 from anyio import (
     BrokenResourceError,
     CancelScope,
     ClosedResourceError,
     EndOfStream,
@@ -12,14 +15,17 @@
     create_task_group,
     fail_after,
     wait_all_tasks_blocked,
 )
 from anyio.abc import ObjectReceiveStream, ObjectSendStream
 from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
 
+if sys.version_info < (3, 11):
+    from exceptiongroup import ExceptionGroup
+
 pytestmark = pytest.mark.anyio
 
 
 def test_invalid_max_buffer() -> None:
     pytest.raises(ValueError, create_memory_object_stream, 1.0).match(
         "max_buffer_size must be either an integer or math.inf"
     )
@@ -32,178 +38,184 @@
 
 
 async def test_receive_then_send() -> None:
     async def receiver() -> None:
         received_objects.append(await receive.receive())
         received_objects.append(await receive.receive())
 
-    send, receive = create_memory_object_stream(0)
+    send, receive = create_memory_object_stream[str](0)
     received_objects: list[str] = []
     async with create_task_group() as tg:
         tg.start_soon(receiver)
         await wait_all_tasks_blocked()
         await send.send("hello")
         await send.send("anyio")
 
     assert received_objects == ["hello", "anyio"]
 
 
 async def test_receive_then_send_nowait() -> None:
     async def receiver() -> None:
         received_objects.append(await receive.receive())
 
-    send, receive = create_memory_object_stream(0)
+    send, receive = create_memory_object_stream[str](0)
     received_objects: list[str] = []
     async with create_task_group() as tg:
         tg.start_soon(receiver)
         tg.start_soon(receiver)
         await wait_all_tasks_blocked()
         send.send_nowait("hello")
         send.send_nowait("anyio")
 
     assert sorted(received_objects, reverse=True) == ["hello", "anyio"]
 
 
 async def test_send_then_receive_nowait() -> None:
-    send, receive = create_memory_object_stream(0)
+    send, receive = create_memory_object_stream[str](0)
     async with create_task_group() as tg:
         tg.start_soon(send.send, "hello")
         await wait_all_tasks_blocked()
         assert receive.receive_nowait() == "hello"
 
 
 async def test_send_is_unblocked_after_receive_nowait() -> None:
-    send, receive = create_memory_object_stream(1)
+    send, receive = create_memory_object_stream[str](1)
     send.send_nowait("hello")
 
     with fail_after(1):
         async with create_task_group() as tg:
             tg.start_soon(send.send, "anyio")
             await wait_all_tasks_blocked()
             assert receive.receive_nowait() == "hello"
 
     assert receive.receive_nowait() == "anyio"
 
 
 async def test_send_nowait_then_receive_nowait() -> None:
-    send, receive = create_memory_object_stream(2)
+    send, receive = create_memory_object_stream[str](2)
     send.send_nowait("hello")
     send.send_nowait("anyio")
     assert receive.receive_nowait() == "hello"
     assert receive.receive_nowait() == "anyio"
 
 
 async def test_iterate() -> None:
     async def receiver() -> None:
         async for item in receive:
             received_objects.append(item)
 
-    send, receive = create_memory_object_stream()
+    send, receive = create_memory_object_stream[str]()
     received_objects: list[str] = []
     async with create_task_group() as tg:
         tg.start_soon(receiver)
         await send.send("hello")
         await send.send("anyio")
         await send.aclose()
 
     assert received_objects == ["hello", "anyio"]
 
 
 async def test_receive_send_closed_send_stream() -> None:
-    send, receive = create_memory_object_stream()
+    send, receive = create_memory_object_stream[None]()
     await send.aclose()
     with pytest.raises(EndOfStream):
         receive.receive_nowait()
 
     with pytest.raises(ClosedResourceError):
         await send.send(None)
 
 
 async def test_receive_send_closed_receive_stream() -> None:
-    send, receive = create_memory_object_stream()
+    send, receive = create_memory_object_stream[None]()
     await receive.aclose()
     with pytest.raises(ClosedResourceError):
         receive.receive_nowait()
 
     with pytest.raises(BrokenResourceError):
         await send.send(None)
 
 
 async def test_cancel_receive() -> None:
-    send, receive = create_memory_object_stream()
+    send, receive = create_memory_object_stream[str]()
     async with create_task_group() as tg:
         tg.start_soon(receive.receive)
         await wait_all_tasks_blocked()
         tg.cancel_scope.cancel()
 
     with pytest.raises(WouldBlock):
         send.send_nowait("hello")
 
 
 async def test_cancel_send() -> None:
-    send, receive = create_memory_object_stream()
+    send, receive = create_memory_object_stream[str]()
     async with create_task_group() as tg:
         tg.start_soon(send.send, "hello")
         await wait_all_tasks_blocked()
         tg.cancel_scope.cancel()
 
     with pytest.raises(WouldBlock):
         receive.receive_nowait()
 
 
 async def test_clone() -> None:
-    send1, receive1 = create_memory_object_stream(1)
+    send1, receive1 = create_memory_object_stream[str](1)
     send2 = send1.clone()
     receive2 = receive1.clone()
     await send1.aclose()
     await receive1.aclose()
     send2.send_nowait("hello")
     assert receive2.receive_nowait() == "hello"
 
 
 async def test_clone_closed() -> None:
-    send, receive = create_memory_object_stream(1)
+    send, receive = create_memory_object_stream[NoReturn](1)
     await send.aclose()
     await receive.aclose()
     pytest.raises(ClosedResourceError, send.clone)
     pytest.raises(ClosedResourceError, receive.clone)
 
 
 async def test_close_send_while_receiving() -> None:
-    send, receive = create_memory_object_stream(1)
-    with pytest.raises(EndOfStream):
+    send, receive = create_memory_object_stream[NoReturn](1)
+    with pytest.raises(ExceptionGroup) as exc:
         async with create_task_group() as tg:
             tg.start_soon(receive.receive)
             await wait_all_tasks_blocked()
             await send.aclose()
 
+    assert len(exc.value.exceptions) == 1
+    assert isinstance(exc.value.exceptions[0], EndOfStream)
+
 
 async def test_close_receive_while_sending() -> None:
-    send, receive = create_memory_object_stream(0)
-    with pytest.raises(BrokenResourceError):
+    send, receive = create_memory_object_stream[str](0)
+    with pytest.raises(ExceptionGroup) as exc:
         async with create_task_group() as tg:
             tg.start_soon(send.send, "hello")
             await wait_all_tasks_blocked()
             await receive.aclose()
 
+    assert len(exc.value.exceptions) == 1
+    assert isinstance(exc.value.exceptions[0], BrokenResourceError)
+
 
 async def test_receive_after_send_closed() -> None:
-    send, receive = create_memory_object_stream(1)
+    send, receive = create_memory_object_stream[str](1)
     await send.send("hello")
     await send.aclose()
     assert await receive.receive() == "hello"
 
 
 async def test_receive_when_cancelled() -> None:
     """
-    Test that calling receive() in a cancelled scope prevents it from going through with the
-    operation.
+    Test that calling receive() in a cancelled scope prevents it from going through with
+    the operation.
 
     """
-    send, receive = create_memory_object_stream()
+    send, receive = create_memory_object_stream[str]()
     async with create_task_group() as tg:
         tg.start_soon(send.send, "hello")
         await wait_all_tasks_blocked()
         tg.start_soon(send.send, "world")
         await wait_all_tasks_blocked()
 
         with CancelScope() as scope:
@@ -212,52 +224,52 @@
 
         assert await receive.receive() == "hello"
         assert await receive.receive() == "world"
 
 
 async def test_send_when_cancelled() -> None:
     """
-    Test that calling send() in a cancelled scope prevents it from going through with the
-    operation.
+    Test that calling send() in a cancelled scope prevents it from going through with
+    the operation.
 
     """
 
     async def receiver() -> None:
         received.append(await receive.receive())
 
     received: list[str] = []
-    send, receive = create_memory_object_stream()
+    send, receive = create_memory_object_stream[str]()
     async with create_task_group() as tg:
         tg.start_soon(receiver)
         with CancelScope() as scope:
             scope.cancel()
             await send.send("hello")
 
         await send.send("world")
 
     assert received == ["world"]
 
 
 async def test_cancel_during_receive() -> None:
     """
-    Test that cancelling a pending receive() operation does not cause an item in the stream to be
-    lost.
+    Test that cancelling a pending receive() operation does not cause an item in the
+    stream to be lost.
 
     """
     receiver_scope = None
 
     async def scoped_receiver() -> None:
         nonlocal receiver_scope
         with CancelScope() as receiver_scope:
             received.append(await receive.receive())
 
         assert receiver_scope.cancel_called
 
     received: list[str] = []
-    send, receive = create_memory_object_stream()
+    send, receive = create_memory_object_stream[str]()
     async with create_task_group() as tg:
         tg.start_soon(scoped_receiver)
         await wait_all_tasks_blocked()
         send.send_nowait("hello")
         assert receiver_scope is not None
         receiver_scope.cancel()
 
@@ -269,23 +281,23 @@
         async with send_stream:
             await send_stream.send("test")
 
     async def receive() -> None:
         async with receive_stream:
             assert await receive_stream.receive() == "test"
 
-    send_stream, receive_stream = create_memory_object_stream()
+    send_stream, receive_stream = create_memory_object_stream[str]()
     async with create_task_group() as tg:
         tg.start_soon(send)
         tg.start_soon(receive)
 
 
 async def test_statistics() -> None:
-    send_stream, receive_stream = create_memory_object_stream(1)
-    streams: list[MemoryObjectReceiveStream[int] | MemoryObjectSendStream[int]] = [
+    send_stream, receive_stream = create_memory_object_stream[None](1)
+    streams: list[MemoryObjectReceiveStream[None] | MemoryObjectSendStream[None]] = [
         send_stream,
         receive_stream,
     ]
     for stream in streams:
         statistics = stream.statistics()
         assert statistics.max_buffer_size == 1
         assert statistics.current_buffer_used == 0
@@ -333,15 +345,15 @@
 
         assert stream.statistics().current_buffer_used == 0
         assert stream.statistics().tasks_waiting_send == 0
         assert stream.statistics().tasks_waiting_receive == 0
 
 
 async def test_sync_close() -> None:
-    send_stream, receive_stream = create_memory_object_stream(1)
+    send_stream, receive_stream = create_memory_object_stream[None](1)
     with send_stream, receive_stream:
         pass
 
     with pytest.raises(ClosedResourceError):
         send_stream.send_nowait(None)
 
     with pytest.raises(ClosedResourceError):
@@ -352,12 +364,12 @@
     """
     This test does not do anything at run time, but since the test suite is also checked
     with a static type checker, it ensures that the memory object stream
     co/contravariance works as intended. If it doesn't, one or both of the following
     reassignments will trip the type checker.
 
     """
-    send, receive = create_memory_object_stream(item_type=float)
+    send, receive = create_memory_object_stream[float]()
     receive1: MemoryObjectReceiveStream[complex] = receive  # noqa: F841
     receive2: ObjectReceiveStream[complex] = receive  # noqa: F841
     send1: MemoryObjectSendStream[int] = send  # noqa: F841
     send2: ObjectSendStream[int] = send  # noqa: F841
```

### Comparing `anyio-3.7.1/tests/streams/test_stapled.py` & `anyio-4.0.0rc1/tests/streams/test_stapled.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.1/tests/streams/test_text.py` & `anyio-4.0.0rc1/tests/streams/test_text.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,52 +9,52 @@
 from anyio.streams.stapled import StapledObjectStream
 from anyio.streams.text import TextReceiveStream, TextSendStream, TextStream
 
 pytestmark = pytest.mark.anyio
 
 
 async def test_receive() -> None:
-    send_stream, receive_stream = create_memory_object_stream(1)
+    send_stream, receive_stream = create_memory_object_stream[bytes](1)
     text_stream = TextReceiveStream(receive_stream)
     await send_stream.send(b"\xc3\xa5\xc3\xa4\xc3")  # ends with half of the "ö" letter
     assert await text_stream.receive() == "åä"
 
     # Send the missing byte for "ö"
     await send_stream.send(b"\xb6")
     assert await text_stream.receive() == "ö"
 
 
 async def test_send() -> None:
-    send_stream, receive_stream = create_memory_object_stream(1)
+    send_stream, receive_stream = create_memory_object_stream[bytes](1)
     text_stream = TextSendStream(send_stream)
     await text_stream.send("åäö")
     assert await receive_stream.receive() == b"\xc3\xa5\xc3\xa4\xc3\xb6"
 
 
 @pytest.mark.xfail(
     platform.python_implementation() == "PyPy"
     and sys.pypy_version_info < (7, 3, 2),  # type: ignore[attr-defined]
     reason="PyPy has a bug in its incremental UTF-8 decoder (#3274)",
 )
 async def test_receive_encoding_error() -> None:
-    send_stream, receive_stream = create_memory_object_stream(1)
+    send_stream, receive_stream = create_memory_object_stream[bytes](1)
     text_stream = TextReceiveStream(receive_stream, errors="replace")
     await send_stream.send(b"\xe5\xe4\xf6")  # "åäö" in latin-1
     assert await text_stream.receive() == "���"
 
 
 async def test_send_encoding_error() -> None:
-    send_stream, receive_stream = create_memory_object_stream(1)
+    send_stream, receive_stream = create_memory_object_stream[bytes](1)
     text_stream = TextSendStream(send_stream, encoding="iso-8859-1", errors="replace")
     await text_stream.send("€")
     assert await receive_stream.receive() == b"?"
 
 
 async def test_bidirectional_stream() -> None:
-    send_stream, receive_stream = create_memory_object_stream(1)
+    send_stream, receive_stream = create_memory_object_stream[bytes](1)
     stapled_stream = StapledObjectStream(send_stream, receive_stream)
     text_stream = TextStream(stapled_stream)
 
     await text_stream.send("åäö")
     assert await receive_stream.receive() == b"\xc3\xa5\xc3\xa4\xc3\xb6"
 
     await send_stream.send(b"\xc3\xa6\xc3\xb8")
```

### Comparing `anyio-3.7.1/tests/streams/test_tls.py` & `anyio-4.0.0rc1/tests/streams/test_tls.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
     @pytest.mark.skipif(
         not hasattr(ssl, "OP_IGNORE_UNEXPECTED_EOF"),
         reason="The ssl module does not have the OP_IGNORE_UNEXPECTED_EOF attribute",
     )
     async def test_default_context_ignore_unexpected_eof_flag_off(
         self, mocker: MockerFixture
     ) -> None:
-        send1, receive1 = create_memory_object_stream()
+        send1, receive1 = create_memory_object_stream[bytes]()
         client_stream = StapledObjectStream(send1, receive1)
         mocker.patch.object(TLSStream, "_call_sslobject_method")
         tls_stream = await TLSStream.wrap(client_stream)
         ssl_context = tls_stream.extra(TLSAttribute.ssl_object).context
         assert not ssl_context.options & ssl.OP_IGNORE_UNEXPECTED_EOF
```

### Comparing `anyio-3.7.1/tests/test_debugging.py` & `anyio-4.0.0rc1/tests/test_debugging.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 import sys
-from typing import (
-    Any,
-    AsyncGenerator,
-    Coroutine,
-    Generator,
-    cast,
-)
+from collections.abc import AsyncGenerator, Coroutine, Generator
+from typing import Any, cast
 
 import pytest
 
 import anyio
 from anyio import (
     Event,
     TaskInfo,
@@ -23,20 +18,15 @@
     wait_all_tasks_blocked,
 )
 from anyio.abc import TaskStatus
 
 pytestmark = pytest.mark.anyio
 
 
-if sys.version_info >= (3, 8):
-    get_coro = asyncio.Task.get_coro
-else:
-
-    def get_coro(self: asyncio.Task) -> Any:
-        return self._coro
+get_coro = asyncio.Task.get_coro
 
 
 def test_main_task_name(
     anyio_backend_name: str, anyio_backend_options: dict[str, Any]
 ) -> None:
     task_name = None
 
@@ -121,14 +111,15 @@
 ) -> None:
     async def native_coro_part() -> None:
         await wait_all_tasks_blocked()
         gen = cast(Generator, get_coro(gen_task))
         assert not gen.gi_running
         coro = cast(Coroutine, gen.gi_yieldfrom)
         assert coro.cr_code.co_name == "wait"
+
         event.set()
 
     @asyncio.coroutine  # type: ignore[attr-defined]
     def generator_part() -> Generator[object, BaseException, None]:
         yield from event.wait()  # type: ignore[misc]
 
     event = asyncio.Event()
@@ -141,16 +132,16 @@
     """Test that wait_all_tasks_blocked() does not crash on an `asend()` object."""
 
     async def agen_func() -> AsyncGenerator[None, None]:
         yield
 
     agen = agen_func()
     coro = agen.asend(None)
-    loop = asyncio.get_event_loop()
-    task: asyncio.Task[None] = loop.create_task(coro)  # type: ignore[arg-type]
+    loop = asyncio.get_running_loop()
+    task = loop.create_task(cast("Coroutine[Any, Any, Any]", coro))
     await wait_all_tasks_blocked()
     await task
     await agen.aclose()
 
 
 async def test_wait_all_tasks_blocked_cancelled_task() -> None:
     done = False
```

### Comparing `anyio-3.7.1/tests/test_eventloop.py` & `anyio-4.0.0rc1/tests/test_eventloop.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pytest
 from pytest_mock.plugin import MockerFixture
 
 from anyio import run, sleep_forever, sleep_until
 
 if sys.version_info < (3, 8):
-    from mock import AsyncMock
+    from unittest.mock import AsyncMock
 else:
     from unittest.mock import AsyncMock
 
 pytestmark = pytest.mark.anyio
 fake_current_time = 1620581544.0
```

### Comparing `anyio-3.7.1/tests/test_fileio.py` & `anyio-4.0.0rc1/tests/test_fileio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import os
 import pathlib
 import platform
 import socket
 import stat
+import sys
 
 import pytest
 from _pytest.tmpdir import TempPathFactory
 
 from anyio import AsyncFile, Path, open_file, wrap_file
 
 pytestmark = pytest.mark.anyio
@@ -70,15 +71,19 @@
         subdir = tmp_path / "subdir"
         subdir.mkdir()
         subdir.joinpath("dummyfile1.txt").touch()
         subdir.joinpath("dummyfile2.txt").touch()
         return tmp_path
 
     async def test_properties(self) -> None:
-        """Ensure that all public properties and methods are available on the async Path class."""
+        """
+        Ensure that all public properties and methods are available on the async Path
+        class.
+
+        """
         path = pathlib.Path("/test/path/another/part")
         stdlib_properties = {
             p for p in dir(path) if p.startswith("__") or not p.startswith("_")
         }
         stdlib_properties.discard("link_to")
         stdlib_properties.discard("__class_getitem__")
         stdlib_properties.discard("__enter__")
@@ -244,14 +249,21 @@
 
     async def test_is_file(self, tmp_path: pathlib.Path) -> None:
         path = tmp_path / "somefile"
         assert not await Path(path).is_file()
         path.touch()
         assert await Path(path).is_file()
 
+    @pytest.mark.skipif(
+        sys.version_info < (3, 12),
+        reason="Path.is_junction() is only available on Python 3.12+",
+    )
+    async def test_is_junction(self, tmp_path: pathlib.Path) -> None:
+        assert not await Path(tmp_path).is_junction()
+
     async def test_is_mount(self) -> None:
         assert not await Path("/gfobj4ewiotj").is_mount()
         assert await Path("/").is_mount()
 
     def test_is_reserved(self) -> None:
         expected_result = platform.system() == "Windows"
         assert Path("nul").is_reserved() == expected_result
@@ -273,19 +285,17 @@
     )
     async def test_is_symlink(self, tmp_path: pathlib.Path) -> None:
         path = tmp_path / "testfile"
         assert not await Path(path).is_symlink()
         path.symlink_to("/foo")
         assert await Path(path).is_symlink()
 
-    @pytest.mark.parametrize(
-        "args, result", [(("/xyz", "abc"), True), (("/xyz", "baz"), False)]
-    )
-    def test_is_relative_to(self, args: tuple[str], result: bool) -> None:
-        assert Path("/xyz/abc/foo").is_relative_to(*args) == result
+    @pytest.mark.parametrize("arg, result", [("/xyz/abc", True), ("/xyz/baz", False)])
+    def test_is_relative_to(self, arg: str, result: bool) -> None:
+        assert Path("/xyz/abc/foo").is_relative_to(arg) == result
 
     async def test_glob(self, populated_tmpdir: pathlib.Path) -> None:
         all_paths = []
         async for path in Path(populated_tmpdir).glob("**/*.txt"):
             assert isinstance(path, Path)
             all_paths.append(path.name)
 
@@ -407,14 +417,18 @@
         assert await Path(path).read_bytes() == b"bibbitibobbitiboo"
 
     async def test_read_text(self, tmp_path: pathlib.Path) -> None:
         path = tmp_path / "testfile"
         path.write_text("some text åäö", encoding="utf-8")
         assert await Path(path).read_text(encoding="utf-8") == "some text åäö"
 
+    async def test_relative_to(self, tmp_path: pathlib.Path) -> None:
+        path = tmp_path / "subdir"
+        assert path.relative_to(tmp_path) == Path("subdir")
+
     async def test_rename(self, tmp_path: pathlib.Path) -> None:
         path = tmp_path / "somefile"
         path.touch()
         target = tmp_path / "anotherfile"
         result = await Path(path).rename(Path(target))
         assert isinstance(result, Path)
         assert result == target
@@ -472,14 +486,40 @@
 
     async def test_unlink_missing_file(self, tmp_path: pathlib.Path) -> None:
         path = tmp_path / "testfile"
         await Path(path).unlink(missing_ok=True)
         with pytest.raises(FileNotFoundError):
             await Path(path).unlink(missing_ok=False)
 
+    @pytest.mark.skipif(
+        sys.version_info < (3, 12),
+        reason="Path.walk() is only available on Python 3.12+",
+    )
+    async def test_walk(self, tmp_path: pathlib.Path) -> None:
+        subdir = tmp_path / "subdir"
+        subdir.mkdir()
+        subdir.joinpath("file1").touch()
+        subdir.joinpath("file2").touch()
+
+        path = Path(tmp_path)
+        iterator = Path(tmp_path).walk().__aiter__()
+
+        root, dirs, files = await iterator.__anext__()
+        assert root == path
+        assert dirs == ["subdir"]
+        assert files == []
+
+        root, dirs, files = await iterator.__anext__()
+        assert root == path / "subdir"
+        assert dirs == []
+        assert sorted(files) == ["file1", "file2"]
+
+        with pytest.raises(StopAsyncIteration):
+            await iterator.__anext__()
+
     def test_with_name(self) -> None:
         assert Path("/xyz/foo.txt").with_name("bar").name == "bar"
 
     def test_with_stem(self) -> None:
         assert Path("/xyz/foo.txt").with_stem("bar").name == "bar.txt"
 
     def test_with_suffix(self) -> None:
```

### Comparing `anyio-3.7.1/tests/test_from_thread.py` & `anyio-4.0.0rc1/tests/test_from_thread.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 from __future__ import annotations
 
+import math
 import sys
 import threading
 import time
+from collections.abc import Awaitable, Callable
+from concurrent import futures
 from concurrent.futures import CancelledError
 from contextlib import asynccontextmanager, suppress
 from contextvars import ContextVar
-from typing import (
-    Any,
-    AsyncGenerator,
-    Awaitable,
-    Callable,
-    NoReturn,
-    TypeVar,
-)
+from typing import Any, AsyncGenerator, Literal, NoReturn, TypeVar
 
 import pytest
+import sniffio
 from _pytest.logging import LogCaptureFixture
 
 from anyio import (
     Event,
     create_task_group,
     from_thread,
+    get_all_backends,
     get_cancelled_exc_class,
     get_current_task,
     run,
     sleep,
     to_thread,
     wait_all_tasks_blocked,
 )
 from anyio.abc import TaskStatus
 from anyio.from_thread import BlockingPortal, start_blocking_portal
 from anyio.lowlevel import checkpoint
 
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
+if sys.version_info < (3, 11):
+    from exceptiongroup import BaseExceptionGroup, ExceptionGroup
 
 pytestmark = pytest.mark.anyio
 
 T_Retval = TypeVar("T_Retval")
 
 
 async def async_add(a: int, b: int) -> int:
@@ -132,26 +128,39 @@
         async def foo() -> None:
             pass
 
         exc = pytest.raises(RuntimeError, from_thread.run, foo)
         exc.match("This function can only be run from an AnyIO worker thread")
 
     async def test_contextvar_propagation(self, anyio_backend_name: str) -> None:
+        if anyio_backend_name == "asyncio" and sys.version_info < (3, 7):
+            pytest.skip("Asyncio does not propagate context before Python 3.7")
+
         var = ContextVar("var", default=1)
 
         async def async_func() -> int:
             await checkpoint()
             return var.get()
 
         def worker() -> int:
             var.set(6)
             return from_thread.run(async_func)
 
         assert await to_thread.run_sync(worker) == 6
 
+    async def test_sniffio(self, anyio_backend_name: str) -> None:
+        async def async_func() -> str:
+            return sniffio.current_async_library()
+
+        def worker() -> str:
+            sniffio.current_async_library_cvar.set("something invalid for async_func")
+            return from_thread.run(async_func)
+
+        assert await to_thread.run_sync(worker) == anyio_backend_name
+
 
 class TestRunSyncFromThread:
     def test_run_sync_from_unclaimed_thread(self) -> None:
         def foo() -> None:
             pass
 
         exc = pytest.raises(RuntimeError, from_thread.run_sync, foo)
@@ -162,14 +171,21 @@
 
         def worker() -> int:
             var.set(6)
             return from_thread.run_sync(var.get)
 
         assert await to_thread.run_sync(worker) == 6
 
+    async def test_sniffio(self, anyio_backend_name: str) -> None:
+        def worker() -> str:
+            sniffio.current_async_library_cvar.set("something invalid for async_func")
+            return from_thread.run_sync(sniffio.current_async_library)
+
+        assert await to_thread.run_sync(worker) == anyio_backend_name
+
 
 class TestBlockingPortal:
     class AsyncCM:
         def __init__(self, ignore_error: bool):
             self.ignore_error = ignore_error
 
         async def __aenter__(self) -> Literal["test"]:
@@ -191,15 +207,18 @@
             async with BlockingPortal() as portal:
                 result = await to_thread.run_sync(portal.call, gen.__anext__)
                 assert result == 3
         finally:
             await gen.aclose()
 
     async def test_aexit_with_exception(self) -> None:
-        """Test that when the portal exits with an exception, all tasks are cancelled."""
+        """
+        Test that when the portal exits with an exception, all tasks are cancelled.
+
+        """
 
         def external_thread() -> None:
             try:
                 portal.call(sleep, 3)
             except BaseException as exc:
                 results.append(exc)
             else:
@@ -386,18 +405,21 @@
         @asynccontextmanager
         async def run_in_context() -> AsyncGenerator[None, None]:
             async with create_task_group() as tg:
                 tg.start_soon(failing_func)
                 yield
 
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
-            with pytest.raises(ZeroDivisionError):
+            with pytest.raises(ExceptionGroup) as exc:
                 with portal.wrap_async_context_manager(run_in_context()):
                     pass
 
+            assert len(exc.value.exceptions) == 1
+            assert isinstance(exc.value.exceptions[0], ZeroDivisionError)
+
     def test_start_no_value(
         self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
         def taskfunc(*, task_status: TaskStatus) -> None:
             task_status.started()
 
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
@@ -460,24 +482,30 @@
                 taskfunc, name="testname"  # type: ignore[arg-type]
             )
             assert start_value == "testname"
 
     def test_contextvar_propagation_sync(
         self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
+        if anyio_backend_name == "asyncio" and sys.version_info < (3, 7):
+            pytest.skip("Asyncio does not propagate context before Python 3.7")
+
         var = ContextVar("var", default=1)
         var.set(6)
         with start_blocking_portal(anyio_backend_name, anyio_backend_options) as portal:
             propagated_value = portal.call(var.get)
 
         assert propagated_value == 6
 
     def test_contextvar_propagation_async(
         self, anyio_backend_name: str, anyio_backend_options: dict[str, Any]
     ) -> None:
+        if anyio_backend_name == "asyncio" and sys.version_info < (3, 7):
+            pytest.skip("Asyncio does not propagate context before Python 3.7")
+
         var = ContextVar("var", default=1)
         var.set(6)
 
         async def get_var() -> int:
             await checkpoint()
             return var.get()
 
@@ -506,15 +534,55 @@
         exceptions when trying to close the portal.
 
         """
 
         async def raise_baseexception() -> None:
             raise BaseException("fatal error")
 
-        with pytest.raises(BaseException, match="fatal error"):
+        with pytest.raises(BaseExceptionGroup) as outer_exc:
             with start_blocking_portal(
                 anyio_backend_name, anyio_backend_options
             ) as portal:
                 with pytest.raises(BaseException, match="fatal error") as exc:
                     portal.call(raise_baseexception)
 
                 assert exc.value.__context__ is None
+
+        assert len(outer_exc.value.exceptions) == 1
+        assert str(outer_exc.value.exceptions[0]) == "fatal error"
+
+    @pytest.mark.parametrize("portal_backend_name", get_all_backends())
+    async def test_from_async(
+        self, anyio_backend_name: str, portal_backend_name: str
+    ) -> None:
+        """
+        Test that portals don't deadlock when started/used from async code.
+
+        Note: This test will deadlock if there is a regression. A deadlock should be
+        treated as a failure. See also
+        https://github.com/agronholm/anyio/pull/524#discussion_r1183080886.
+
+        """
+        if anyio_backend_name == "trio" and portal_backend_name == "trio":
+            pytest.xfail("known bug (#525)")
+
+        with start_blocking_portal(portal_backend_name) as portal:
+            portal.call(checkpoint)
+
+    async def test_cancel_portal_future(self) -> None:
+        """Regression test for #575."""
+        event = Event()
+
+        def sync_thread() -> None:
+            fs = [portal.start_task_soon(sleep, math.inf)]
+            from_thread.run_sync(event.set)
+            done, not_done = futures.wait(
+                fs, timeout=1, return_when=futures.FIRST_COMPLETED
+            )
+            assert not not_done
+
+        async with from_thread.BlockingPortal() as portal:
+            async with create_task_group() as tg:
+                tg.start_soon(to_thread.run_sync, sync_thread)
+                # Ensure thread has time to start the task
+                await event.wait()
+                await portal.stop(cancel_remaining=True)
```

### Comparing `anyio-3.7.1/tests/test_lowlevel.py` & `anyio-4.0.0rc1/tests/test_lowlevel.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.1/tests/test_pytest_plugin.py` & `anyio-4.0.0rc1/tests/test_pytest_plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,36 +3,47 @@
 import pytest
 from _pytest.logging import LogCaptureFixture
 from _pytest.pytester import Pytester
 
 from anyio import get_all_backends
 
 pytestmark = pytest.mark.filterwarnings(
-    "ignore:The TerminalReporter.writer attribute is deprecated:pytest.PytestDeprecationWarning:"
+    "ignore:The TerminalReporter.writer attribute is deprecated"
+    ":pytest.PytestDeprecationWarning:"
 )
 
-pytest_args = "-v", "-p", "anyio", "-p", "no:asyncio"
+pytest_args = "-v", "-p", "anyio", "-p", "no:asyncio", "-p", "no:trio"
 
 
 def test_plugin(testdir: Pytester) -> None:
     testdir.makeconftest(
         """
+        from contextvars import ContextVar
         import sniffio
         import pytest
 
         from anyio import sleep
 
+        var = ContextVar("var")
+
 
         @pytest.fixture
         async def async_fixture():
             await sleep(0)
             return sniffio.current_async_library()
 
 
         @pytest.fixture
+        async def context_variable():
+            token = var.set("testvalue")
+            yield var
+            var.reset(token)
+
+
+        @pytest.fixture
         async def some_feature():
             yield None
             await sleep(0)
         """
     )
 
     testdir.makepyfile(
@@ -58,28 +69,34 @@
             # Test that regular functions can use async fixtures too
             assert async_fixture == anyio_backend_name
 
         @pytest.mark.anyio
         async def test_skip_inline(some_feature):
             # Test for github #214
             pytest.skip("Test that skipping works")
+
+        @pytest.mark.anyio
+        async def test_contextvar(context_variable):
+            # Test that a contextvar set in an async fixture is visible to the test
+            assert context_variable.get() == "testvalue"
         """
     )
 
     result = testdir.runpytest(*pytest_args)
     result.assert_outcomes(
-        passed=3 * len(get_all_backends()), skipped=len(get_all_backends())
+        passed=4 * len(get_all_backends()), skipped=len(get_all_backends())
     )
 
 
 def test_asyncio(testdir: Pytester, caplog: LogCaptureFixture) -> None:
     testdir.makeconftest(
         """
         import asyncio
         import pytest
+        import threading
 
 
         @pytest.fixture(scope='class')
         def anyio_backend():
             return 'asyncio'
 
         @pytest.fixture
@@ -95,14 +112,24 @@
         async def teardown_fail_fixture():
             def callback():
                 raise RuntimeError('failing fixture teardown')
 
             yield None
             asyncio.get_running_loop().call_soon(callback)
             await asyncio.sleep(0)
+
+        @pytest.fixture
+        def no_thread_leaks_fixture():
+            # this has to be non-async fixture so that it wraps up
+            # after the event loop gets closed
+            threads_before = threading.enumerate()
+            yield
+            threads_after = threading.enumerate()
+            leaked_threads = set(threads_after) - set(threads_before)
+            assert not leaked_threads
         """
     )
 
     testdir.makepyfile(
         """
         import asyncio
 
@@ -113,15 +140,19 @@
 
         class TestClassFixtures:
             @pytest.fixture(scope='class')
             async def async_class_fixture(self, anyio_backend):
                 await asyncio.sleep(0)
                 return anyio_backend
 
-            def test_class_fixture_in_test_method(self, async_class_fixture, anyio_backend_name):
+            def test_class_fixture_in_test_method(
+                self,
+                async_class_fixture,
+                anyio_backend_name
+            ):
                 assert anyio_backend_name == 'asyncio'
                 assert async_class_fixture == 'asyncio'
 
         async def test_callback_exception_during_test() -> None:
             def callback():
                 nonlocal started
                 started = True
@@ -139,19 +170,23 @@
             pass
 
         async def test_exception_handler_no_exception():
             asyncio.get_event_loop().call_exception_handler(
                 {"message": "bogus error"}
             )
             await asyncio.sleep(0.1)
+
+        async def test_shutdown_default_executor(no_thread_leaks_fixture):
+            # Test for github #503
+            asyncio.get_event_loop().run_in_executor(None, lambda: 1)
         """
     )
 
     result = testdir.runpytest(*pytest_args)
-    result.assert_outcomes(passed=3, failed=1, errors=2)
+    result.assert_outcomes(passed=4, failed=1, errors=2)
     assert len(caplog.messages) == 1
     assert caplog.messages[0] == "bogus error"
 
 
 def test_autouse_async_fixture(testdir: Pytester) -> None:
     testdir.makeconftest(
         """
```

### Comparing `anyio-3.7.1/tests/test_signals.py` & `anyio-4.0.0rc1/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `anyio-3.7.1/tests/test_sockets.py` & `anyio-4.0.0rc1/tests/test_sockets.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,43 +10,37 @@
 import threading
 import time
 from contextlib import suppress
 from pathlib import Path
 from socket import AddressFamily
 from ssl import SSLContext, SSLError
 from threading import Thread
-from typing import (
-    Any,
-    Iterable,
-    Iterator,
-    NoReturn,
-    TypeVar,
-    cast,
-)
+from typing import Any, Iterable, Iterator, NoReturn, TypeVar, cast
 
 import psutil
 import pytest
 from _pytest.fixtures import SubRequest
 from _pytest.logging import LogCaptureFixture
 from _pytest.monkeypatch import MonkeyPatch
 from _pytest.tmpdir import TempPathFactory
 
 from anyio import (
     BrokenResourceError,
     BusyResourceError,
     ClosedResourceError,
     Event,
-    ExceptionGroup,
     TypedAttributeLookupError,
     connect_tcp,
     connect_unix,
     create_connected_udp_socket,
+    create_connected_unix_datagram_socket,
     create_task_group,
     create_tcp_listener,
     create_udp_socket,
+    create_unix_datagram_socket,
     create_unix_listener,
     fail_after,
     getaddrinfo,
     getnameinfo,
     move_on_after,
     sleep,
     wait_all_tasks_blocked,
@@ -56,18 +50,18 @@
     Listener,
     SocketAttribute,
     SocketListener,
     SocketStream,
 )
 from anyio.streams.stapled import MultiListener
 
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
+if sys.version_info < (3, 11):
+    from exceptiongroup import ExceptionGroup
+
+from typing import Literal
 
 AnyIPAddressFamily = Literal[
     AddressFamily.AF_UNSPEC, AddressFamily.AF_INET, AddressFamily.AF_INET6
 ]
 
 pytestmark = pytest.mark.anyio
 
@@ -481,15 +475,16 @@
         assert thread_exception is None
 
     @pytest.mark.parametrize("anyio_backend", ["asyncio"])
     async def test_unretrieved_future_exception_server_crash(
         self, family: AnyIPAddressFamily, caplog: LogCaptureFixture
     ) -> None:
         """
-        Tests that there won't be any leftover Futures that don't get their exceptions retrieved.
+        Test that there won't be any leftover Futures that don't get their exceptions
+        retrieved.
 
         See https://github.com/encode/httpcore/issues/382 for details.
 
         """
 
         def serve() -> None:
             sock, addr = server_sock.accept()
@@ -641,21 +636,27 @@
             SocketAttribute.local_address
         ) == multi2.listeners[0].extra(SocketAttribute.local_address)
         await multi1.aclose()
         await multi2.aclose()
 
     async def test_close_from_other_task(self, family: AnyIPAddressFamily) -> None:
         listener = await create_tcp_listener(local_host="localhost", family=family)
-        with pytest.raises(ClosedResourceError):
+        with pytest.raises(ExceptionGroup) as exc:
             async with create_task_group() as tg:
                 tg.start_soon(listener.serve, lambda stream: None)
                 await wait_all_tasks_blocked()
                 await listener.aclose()
                 tg.cancel_scope.cancel()
 
+        assert len(exc.value.exceptions) == 1
+        assert isinstance(exc.value.exceptions[0], ExceptionGroup)
+        nested_grp = exc.value.exceptions[0]
+        assert len(nested_grp.exceptions) == 1
+        assert isinstance(nested_grp.exceptions[0], ExceptionGroup)
+
     async def test_send_after_eof(self, family: AnyIPAddressFamily) -> None:
         async def handle(stream: SocketStream) -> None:
             async with stream:
                 await stream.send(b"Hello\n")
 
         multi = await create_tcp_listener(family=family, local_host="localhost")
         async with multi, create_task_group() as tg:
@@ -1179,15 +1180,17 @@
         async def serve() -> None:
             async for packet, addr in server:
                 await server.send((packet[::-1], addr))
 
         async with await create_udp_socket(
             family=family, local_host="localhost"
         ) as server:
-            host, port = server.extra(SocketAttribute.local_address)  # type: ignore[misc]
+            host, port = server.extra(  # type: ignore[misc]
+                SocketAttribute.local_address
+            )
             async with await create_udp_socket(
                 family=family, local_host="localhost"
             ) as client:
                 async with create_task_group() as tg:
                     tg.start_soon(serve)
                     await client.sendto(b"FOOBAR", host, port)
                     assert await client.receive() == (b"RABOOF", (host, port))
@@ -1285,15 +1288,17 @@
         async with await create_udp_socket(
             family=family, local_host="localhost"
         ) as udp1:
             host, port = udp1.extra(SocketAttribute.local_address)  # type: ignore[misc]
             async with await create_connected_udp_socket(
                 host, port, local_host="localhost", family=family
             ) as udp2:
-                host, port = udp2.extra(SocketAttribute.local_address)  # type: ignore[misc]
+                host, port = udp2.extra(
+                    SocketAttribute.local_address  # type: ignore[misc]
+                )
                 await udp2.send(b"blah")
                 request = await udp1.receive()
                 assert request == (b"blah", (host, port))
 
                 await udp1.sendto(b"halb", host, port)
                 response = await udp2.receive()
                 assert response == b"halb"
@@ -1304,15 +1309,17 @@
                 await udp2.send(packet[::-1])
 
         async with await create_udp_socket(
             family=family, local_host="localhost"
         ) as udp1:
             host, port = udp1.extra(SocketAttribute.local_address)  # type: ignore[misc]
             async with await create_connected_udp_socket(host, port) as udp2:
-                host, port = udp2.extra(SocketAttribute.local_address)  # type: ignore[misc]
+                host, port = udp2.extra(  # type: ignore[misc]
+                    SocketAttribute.local_address
+                )
                 async with create_task_group() as tg:
                     tg.start_soon(serve)
                     await udp1.sendto(b"FOOBAR", host, port)
                     assert await udp1.receive() == (b"RABOOF", (host, port))
                     await udp1.sendto(b"123456", host, port)
                     assert await udp1.receive() == (b"654321", (host, port))
                     tg.cancel_scope.cancel()
@@ -1377,14 +1384,271 @@
             "localhost", 5000, local_host="localhost", family=family
         )
         await udp.aclose()
         with pytest.raises(ClosedResourceError):
             await udp.send(b"foo")
 
 
+@pytest.mark.skipif(
+    sys.platform == "win32", reason="UNIX sockets are not available on Windows"
+)
+class TestUNIXDatagramSocket:
+    @pytest.fixture
+    def socket_path(self, tmp_path_factory: TempPathFactory) -> Path:
+        return tmp_path_factory.mktemp("unix").joinpath("socket")
+
+    @pytest.fixture(params=[False, True], ids=["str", "path"])
+    def socket_path_or_str(self, request: SubRequest, socket_path: Path) -> Path | str:
+        return socket_path if request.param else str(socket_path)
+
+    @pytest.fixture
+    def peer_socket_path(self, tmp_path_factory: TempPathFactory) -> Path:
+        return tmp_path_factory.mktemp("unix").joinpath("peer_socket")
+
+    async def test_extra_attributes(self, socket_path: Path) -> None:
+        async with await create_unix_datagram_socket(local_path=socket_path) as unix_dg:
+            raw_socket = unix_dg.extra(SocketAttribute.raw_socket)
+            assert raw_socket.gettimeout() == 0
+            assert unix_dg.extra(SocketAttribute.family) == socket.AF_UNIX
+            assert (
+                unix_dg.extra(SocketAttribute.local_address) == raw_socket.getsockname()
+            )
+            pytest.raises(
+                TypedAttributeLookupError, unix_dg.extra, SocketAttribute.local_port
+            )
+            pytest.raises(
+                TypedAttributeLookupError, unix_dg.extra, SocketAttribute.remote_address
+            )
+            pytest.raises(
+                TypedAttributeLookupError, unix_dg.extra, SocketAttribute.remote_port
+            )
+
+    async def test_send_receive(self, socket_path_or_str: Path | str) -> None:
+        async with await create_unix_datagram_socket(
+            local_path=socket_path_or_str,
+        ) as sock:
+            path = str(socket_path_or_str)
+
+            await sock.sendto(b"blah", path)
+            request, addr = await sock.receive()
+            assert request == b"blah"
+            assert addr == path
+
+            await sock.sendto(b"halb", path)
+            response, addr = await sock.receive()
+            assert response == b"halb"
+            assert addr == path
+
+    async def test_iterate(self, peer_socket_path: Path, socket_path: Path) -> None:
+        async def serve() -> None:
+            async for packet, addr in server:
+                await server.send((packet[::-1], addr))
+
+        async with await create_unix_datagram_socket(
+            local_path=peer_socket_path,
+        ) as server:
+            peer_path = str(peer_socket_path)
+            async with await create_unix_datagram_socket(
+                local_path=socket_path
+            ) as client:
+                async with create_task_group() as tg:
+                    tg.start_soon(serve)
+                    await client.sendto(b"FOOBAR", peer_path)
+                    assert await client.receive() == (b"RABOOF", peer_path)
+                    await client.sendto(b"123456", peer_path)
+                    assert await client.receive() == (b"654321", peer_path)
+                    tg.cancel_scope.cancel()
+
+    async def test_concurrent_receive(self) -> None:
+        async with await create_unix_datagram_socket() as unix_dg:
+            async with create_task_group() as tg:
+                tg.start_soon(unix_dg.receive)
+                await wait_all_tasks_blocked()
+                try:
+                    with pytest.raises(BusyResourceError) as exc:
+                        await unix_dg.receive()
+
+                    exc.match("already reading from")
+                finally:
+                    tg.cancel_scope.cancel()
+
+    async def test_close_during_receive(self) -> None:
+        async def close_when_blocked() -> None:
+            await wait_all_tasks_blocked()
+            await unix_dg.aclose()
+
+        async with await create_unix_datagram_socket() as unix_dg:
+            async with create_task_group() as tg:
+                tg.start_soon(close_when_blocked)
+                with pytest.raises(ClosedResourceError):
+                    await unix_dg.receive()
+
+    async def test_receive_after_close(self) -> None:
+        unix_dg = await create_unix_datagram_socket()
+        await unix_dg.aclose()
+        with pytest.raises(ClosedResourceError):
+            await unix_dg.receive()
+
+    async def test_send_after_close(self, socket_path: Path) -> None:
+        unix_dg = await create_unix_datagram_socket(local_path=socket_path)
+        path = str(socket_path)
+        await unix_dg.aclose()
+        with pytest.raises(ClosedResourceError):
+            await unix_dg.sendto(b"foo", path)
+
+
+@pytest.mark.skipif(
+    sys.platform == "win32", reason="UNIX sockets are not available on Windows"
+)
+class TestConnectedUNIXDatagramSocket:
+    @pytest.fixture
+    def socket_path(self, tmp_path_factory: TempPathFactory) -> Path:
+        return tmp_path_factory.mktemp("unix").joinpath("socket")
+
+    @pytest.fixture(params=[False, True], ids=["str", "path"])
+    def socket_path_or_str(self, request: SubRequest, socket_path: Path) -> Path | str:
+        return socket_path if request.param else str(socket_path)
+
+    @pytest.fixture
+    def peer_socket_path(self, tmp_path_factory: TempPathFactory) -> Path:
+        return tmp_path_factory.mktemp("unix").joinpath("peer_socket")
+
+    @pytest.fixture(params=[False, True], ids=["peer_str", "peer_path"])
+    def peer_socket_path_or_str(
+        self, request: SubRequest, peer_socket_path: Path
+    ) -> Path | str:
+        return peer_socket_path if request.param else str(peer_socket_path)
+
+    @pytest.fixture
+    def peer_sock(self, peer_socket_path: Path) -> Iterable[socket.socket]:
+        sock = socket.socket(socket.AF_UNIX, socket.SOCK_DGRAM)
+        sock.settimeout(1)
+        sock.bind(str(peer_socket_path))
+        yield sock
+        sock.close()
+
+    async def test_extra_attributes(
+        self,
+        socket_path: Path,
+        peer_socket_path: Path,
+        peer_sock: socket.socket,
+    ) -> None:
+        async with await create_connected_unix_datagram_socket(
+            remote_path=peer_socket_path,
+            local_path=socket_path,
+        ) as unix_dg:
+            raw_socket = unix_dg.extra(SocketAttribute.raw_socket)
+            assert raw_socket is not None
+            assert unix_dg.extra(SocketAttribute.family) == AddressFamily.AF_UNIX
+            assert unix_dg.extra(SocketAttribute.local_address) == str(socket_path)
+            assert unix_dg.extra(SocketAttribute.remote_address) == str(
+                peer_socket_path
+            )
+            pytest.raises(
+                TypedAttributeLookupError, unix_dg.extra, SocketAttribute.local_port
+            )
+            pytest.raises(
+                TypedAttributeLookupError, unix_dg.extra, SocketAttribute.remote_port
+            )
+
+    async def test_send_receive(
+        self,
+        socket_path_or_str: Path | str,
+        peer_socket_path_or_str: Path | str,
+    ) -> None:
+        async with await create_unix_datagram_socket(
+            local_path=peer_socket_path_or_str,
+        ) as unix_dg1:
+            async with await create_connected_unix_datagram_socket(
+                peer_socket_path_or_str,
+                local_path=socket_path_or_str,
+            ) as unix_dg2:
+                socket_path = str(socket_path_or_str)
+
+                await unix_dg2.send(b"blah")
+                request = await unix_dg1.receive()
+                assert request == (b"blah", socket_path)
+
+                await unix_dg1.sendto(b"halb", socket_path)
+                response = await unix_dg2.receive()
+                assert response == b"halb"
+
+    async def test_iterate(
+        self,
+        socket_path: Path,
+        peer_socket_path: Path,
+    ) -> None:
+        async def serve() -> None:
+            async for packet in unix_dg2:
+                await unix_dg2.send(packet[::-1])
+
+        async with await create_unix_datagram_socket(
+            local_path=peer_socket_path,
+        ) as unix_dg1:
+            async with await create_connected_unix_datagram_socket(
+                peer_socket_path, local_path=socket_path
+            ) as unix_dg2:
+                path = str(socket_path)
+                async with create_task_group() as tg:
+                    tg.start_soon(serve)
+                    await unix_dg1.sendto(b"FOOBAR", path)
+                    assert await unix_dg1.receive() == (b"RABOOF", path)
+                    await unix_dg1.sendto(b"123456", path)
+                    assert await unix_dg1.receive() == (b"654321", path)
+                    tg.cancel_scope.cancel()
+
+    async def test_concurrent_receive(
+        self, peer_socket_path: Path, peer_sock: socket.socket
+    ) -> None:
+        async with await create_connected_unix_datagram_socket(
+            peer_socket_path
+        ) as unix_dg:
+            async with create_task_group() as tg:
+                tg.start_soon(unix_dg.receive)
+                await wait_all_tasks_blocked()
+                try:
+                    with pytest.raises(BusyResourceError) as exc:
+                        await unix_dg.receive()
+
+                    exc.match("already reading from")
+                finally:
+                    tg.cancel_scope.cancel()
+
+    async def test_close_during_receive(
+        self, peer_socket_path_or_str: Path | str, peer_sock: socket.socket
+    ) -> None:
+        async def close_when_blocked() -> None:
+            await wait_all_tasks_blocked()
+            await udp.aclose()
+
+        async with await create_connected_unix_datagram_socket(
+            peer_socket_path_or_str
+        ) as udp:
+            async with create_task_group() as tg:
+                tg.start_soon(close_when_blocked)
+                with pytest.raises(ClosedResourceError):
+                    await udp.receive()
+
+    async def test_receive_after_close(
+        self, peer_socket_path_or_str: Path | str, peer_sock: socket.socket
+    ) -> None:
+        udp = await create_connected_unix_datagram_socket(peer_socket_path_or_str)
+        await udp.aclose()
+        with pytest.raises(ClosedResourceError):
+            await udp.receive()
+
+    async def test_send_after_close(
+        self, peer_socket_path_or_str: Path | str, peer_sock: socket.socket
+    ) -> None:
+        udp = await create_connected_unix_datagram_socket(peer_socket_path_or_str)
+        await udp.aclose()
+        with pytest.raises(ClosedResourceError):
+            await udp.send(b"foo")
+
+
 @pytest.mark.network
 async def test_getaddrinfo() -> None:
     # IDNA 2003 gets this wrong
     correct = await getaddrinfo("faß.de", 0)
     wrong = await getaddrinfo("fass.de", 0)
     assert correct != wrong
```

### Comparing `anyio-3.7.1/tests/test_subprocesses.py` & `anyio-4.0.0rc1/tests/test_subprocesses.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 
 @pytest.fixture(autouse=True)
 def check_compatibility(anyio_backend_name: str) -> None:
     if anyio_backend_name == "asyncio":
         if platform.system() == "Windows" and sys.version_info < (3, 8):
             pytest.skip(
-                "Python < 3.8 uses SelectorEventLoop by default and it does not support "
-                "subprocesses"
+                "Python < 3.8 uses SelectorEventLoop by default and it does not "
+                "support subprocesses"
             )
 
 
 @pytest.mark.parametrize(
     "shell, command",
     [
         pytest.param(
@@ -112,15 +112,18 @@
     assert result.stdout.decode().strip() == env["foo"]
 
 
 @pytest.mark.skipif(
     platform.system() == "Windows", reason="Windows does not have os.getsid()"
 )
 async def test_process_new_session_sid() -> None:
-    """Test that start_new_session is successfully passed to the subprocess implementation"""
+    """
+    Test that start_new_session is successfully passed to the subprocess implementation.
+
+    """
     sid = os.getsid(os.getpid())
     cmd = [sys.executable, "-c", "import os; print(os.getsid(os.getpid()))"]
 
     result = await run_process(cmd)
     assert result.stdout.decode().strip() == str(sid)
 
     result = await run_process(cmd, start_new_session=True)
@@ -136,15 +139,16 @@
         "wb"
     ) as ferr:
         async with await open_process(
             [
                 sys.executable,
                 "-c",
                 "import sys; txt = sys.stdin.read().strip(); "
-                'print("stdin says", repr(txt), "but stderr says NO!", file=sys.stderr); '
+                'print("stdin says", repr(txt), "but stderr says NO!", '
+                "file=sys.stderr); "
                 'print("stdin says", repr(txt), "and stdout says YES!")',
             ],
             stdin=fin,
             stdout=fout,
             stderr=ferr,
         ) as p:
             assert await p.wait() == 0
```

### Comparing `anyio-3.7.1/tests/test_synchronization.py` & `anyio-4.0.0rc1/tests/test_synchronization.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         """Regression test for #398."""
         lock = Lock()
 
         async def acquire() -> None:
             async with lock:
                 await asyncio.sleep(0)
 
-        loop = asyncio.get_event_loop()
+        loop = asyncio.get_running_loop()
         task1 = loop.create_task(acquire())
         task2 = loop.create_task(acquire())
         await asyncio.sleep(0)
         task1.cancel()
         await asyncio.wait_for(task2, 1)
 
 
@@ -168,14 +168,33 @@
             tg.start_soon(task)
             tg.cancel_scope.cancel()
             event.set()
 
         assert task_started
         assert not event_set
 
+    async def test_event_wait_before_set_before_cancel(self) -> None:
+        setter_started = waiter_woke = False
+
+        async def setter() -> None:
+            nonlocal setter_started
+            setter_started = True
+            assert not event.is_set()
+            event.set()
+            tg.cancel_scope.cancel()
+
+        event = Event()
+        async with create_task_group() as tg:
+            tg.start_soon(setter)
+            await event.wait()
+            waiter_woke = True
+
+        assert setter_started
+        assert waiter_woke
+
     async def test_statistics(self) -> None:
         async def waiter() -> None:
             await event.wait()
 
         event = Event()
         async with create_task_group() as tg:
             assert event.statistics().tasks_waiting == 0
@@ -373,16 +392,17 @@
                     await wait_all_tasks_blocked()
                     assert semaphore.statistics().tasks_waiting == i
 
         assert semaphore.statistics().tasks_waiting == 0
 
     async def test_acquire_race(self) -> None:
         """
-        Test against a race condition: when a task waiting on acquire() is rescheduled but another
-        task snatches the last available slot, the task should not raise WouldBlock.
+        Test against a race condition: when a task waiting on acquire() is rescheduled
+        but another task snatches the last available slot, the task should not raise
+        WouldBlock.
 
         """
         semaphore = Semaphore(1)
         async with create_task_group() as tg:
             semaphore.acquire_nowait()
             tg.start_soon(semaphore.acquire)
             await wait_all_tasks_blocked()
@@ -394,15 +414,15 @@
         """Regression test for #398."""
         semaphore = Semaphore(1)
 
         async def acquire() -> None:
             async with semaphore:
                 await asyncio.sleep(0)
 
-        loop = asyncio.get_event_loop()
+        loop = asyncio.get_running_loop()
         task1 = loop.create_task(acquire())
         task2 = loop.create_task(acquire())
         await asyncio.sleep(0)
         task1.cancel()
         await asyncio.wait_for(task2, 1)
 
 
@@ -515,15 +535,15 @@
         """Regression test for #398."""
         limiter = CapacityLimiter(1)
 
         async def acquire() -> None:
             async with limiter:
                 await asyncio.sleep(0)
 
-        loop = asyncio.get_event_loop()
+        loop = asyncio.get_running_loop()
         task1 = loop.create_task(acquire())
         task2 = loop.create_task(acquire())
         await asyncio.sleep(0)
         task1.cancel()
         await asyncio.wait_for(task2, 1)
 
     async def test_ordered_queue(self) -> None:
```

### Comparing `anyio-3.7.1/tests/test_taskgroups.py` & `anyio-4.0.0rc1/tests/test_taskgroups.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 from __future__ import annotations
 
 import asyncio
 import math
-import re
 import sys
 import time
-from typing import (
-    Any,
-    AsyncGenerator,
-    Coroutine,
-    Generator,
-    NoReturn,
-    cast,
-)
+from collections.abc import AsyncGenerator, Coroutine, Generator
+from typing import Any, NoReturn, cast
 
 import pytest
 
 import anyio
 from anyio import (
     TASK_STATUS_IGNORED,
     CancelScope,
-    ExceptionGroup,
     create_task_group,
     current_effective_deadline,
     current_time,
     fail_after,
     get_cancelled_exc_class,
     get_current_task,
     move_on_after,
     sleep,
     wait_all_tasks_blocked,
 )
 from anyio.abc import TaskGroup, TaskStatus
 from anyio.lowlevel import checkpoint
 
+if sys.version_info < (3, 11):
+    from exceptiongroup import BaseExceptionGroup, ExceptionGroup
+
 pytestmark = pytest.mark.anyio
 
 
 async def async_error(text: str, delay: float = 0.1) -> NoReturn:
     try:
         if delay:
             await sleep(delay)
@@ -76,34 +71,29 @@
 )
 def test_run_natively(module: Any) -> None:
     async def testfunc() -> None:
         async with create_task_group() as tg:
             tg.start_soon(sleep, 0)
 
     if module is asyncio:
-        from anyio._backends._asyncio import native_run  # type: ignore[attr-defined]
-
-        try:
-            native_run(testfunc())
-        finally:
-            asyncio.set_event_loop(None)
+        asyncio.run(testfunc())
     else:
         module.run(testfunc)
 
 
 async def test_start_soon_while_running() -> None:
     async def task_func() -> None:
         tg.start_soon(sleep, 0)
 
     async with create_task_group() as tg:
         tg.start_soon(task_func)
 
 
 async def test_start_soon_after_error() -> None:
-    with pytest.raises(ZeroDivisionError):
+    with pytest.raises(ExceptionGroup):
         async with create_task_group() as tg:
             a = 1 / 0  # noqa: F841
 
     with pytest.raises(RuntimeError) as exc:
         tg.start_soon(sleep, 0)
 
     exc.match("This task group is not active; no new tasks can be started")
@@ -153,19 +143,20 @@
 
 
 async def test_start_crash_after_started_call() -> None:
     async def taskfunc(*, task_status: TaskStatus) -> NoReturn:
         task_status.started(2)
         raise Exception("foo")
 
-    with pytest.raises(Exception) as exc:
+    with pytest.raises(ExceptionGroup) as exc:
         async with create_task_group() as tg:
             value = await tg.start(taskfunc)
 
-    exc.match("foo")
+    assert len(exc.value.exceptions) == 1
+    assert str(exc.value.exceptions[0]) == "foo"
     assert value == 2
 
 
 async def test_start_no_started_call() -> None:
     async def taskfunc(*, task_status: TaskStatus) -> None:
         pass
 
@@ -203,15 +194,18 @@
         await sleep(2)
         finished = True
 
     async def start_another() -> None:
         async with create_task_group() as tg:
             await tg.start(taskfunc)
 
-    task = asyncio.get_event_loop().create_task(start_another())
+    if sys.version_info < (3, 9):
+        pytest.xfail("Requires a way to detect cancellation source")
+
+    task = asyncio.get_running_loop().create_task(start_another())
     await wait_all_tasks_blocked()
     task.cancel()
     with pytest.raises(asyncio.CancelledError):
         await task
 
     assert started
     assert not finished
@@ -237,37 +231,81 @@
         await wait_all_tasks_blocked()
         assert task is not None
         task.cancel()
 
     assert not finished
 
 
-async def test_start_exception_delivery() -> None:
-    def task_fn(*, task_status: TaskStatus) -> None:
+@pytest.mark.parametrize("anyio_backend", ["asyncio"])
+async def test_propagate_native_cancellation_from_taskgroup() -> None:
+    async def taskfunc() -> None:
+        async with create_task_group() as tg:
+            tg.start_soon(asyncio.sleep, 2)
+
+    task = asyncio.create_task(taskfunc())
+    await wait_all_tasks_blocked()
+    task.cancel()
+    with pytest.raises(asyncio.CancelledError):
+        await task
+
+
+async def test_start_exception_delivery(anyio_backend_name: str) -> None:
+    def task_fn(*, task_status: TaskStatus = TASK_STATUS_IGNORED) -> None:
         task_status.started("hello")
 
+    if anyio_backend_name == "trio":
+        pattern = "appears to be synchronous"
+    else:
+        pattern = "is not a coroutine object"
+
     async with anyio.create_task_group() as tg:
-        with pytest.raises(TypeError, match="to be synchronous$"):
+        with pytest.raises(TypeError, match=pattern):
             await tg.start(task_fn)  # type: ignore[arg-type]
 
 
+async def test_start_cancel_after_error() -> None:
+    """Regression test for #517."""
+    sleep_completed = False
+
+    async def sleep_and_raise() -> None:
+        await wait_all_tasks_blocked()
+        raise RuntimeError("This should cancel the second start() call")
+
+    async def sleep_only(task_status: TaskStatus[None]) -> None:
+        nonlocal sleep_completed
+        await sleep(1)
+        sleep_completed = True
+        task_status.started()
+
+    with pytest.raises(ExceptionGroup) as exc:
+        async with anyio.create_task_group() as outer_tg:
+            async with anyio.create_task_group() as inner_tg:
+                inner_tg.start_soon(sleep_and_raise)
+                await outer_tg.start(sleep_only)
+
+    assert isinstance(exc.value.exceptions[0], ExceptionGroup)
+    assert isinstance(exc.value.exceptions[0].exceptions[0], RuntimeError)
+    assert not sleep_completed
+
+
 async def test_host_exception() -> None:
     result = None
 
     async def set_result(value: str) -> None:
         nonlocal result
         await sleep(3)
         result = value
 
-    with pytest.raises(Exception) as exc:
+    with pytest.raises(ExceptionGroup) as exc:
         async with create_task_group() as tg:
             tg.start_soon(set_result, "a")
             raise Exception("dummy error")
 
-    exc.match("dummy error")
+    assert len(exc.value.exceptions) == 1
+    assert str(exc.value.exceptions[0]) == "dummy error"
     assert result is None
 
 
 async def test_level_cancellation() -> None:
     marker = None
 
     async def dummy() -> None:
@@ -288,39 +326,41 @@
 
 async def test_failing_child_task_cancels_host() -> None:
     async def child() -> NoReturn:
         await wait_all_tasks_blocked()
         raise Exception("foo")
 
     sleep_completed = False
-    with pytest.raises(Exception) as exc:
+    with pytest.raises(ExceptionGroup) as exc:
         async with create_task_group() as tg:
             tg.start_soon(child)
             await sleep(0.5)
             sleep_completed = True
 
-    exc.match("foo")
+    assert len(exc.value.exceptions) == 1
+    assert str(exc.value.exceptions[0]) == "foo"
     assert not sleep_completed
 
 
 async def test_failing_host_task_cancels_children() -> None:
     sleep_completed = False
 
     async def child() -> None:
         nonlocal sleep_completed
         await sleep(1)
         sleep_completed = True
 
-    with pytest.raises(Exception) as exc:
+    with pytest.raises(ExceptionGroup) as exc:
         async with create_task_group() as tg:
             tg.start_soon(child)
             await wait_all_tasks_blocked()
             raise Exception("foo")
 
-    exc.match("foo")
+    assert len(exc.value.exceptions) == 1
+    assert str(exc.value.exceptions[0]) == "foo"
     assert not sleep_completed
 
 
 async def test_cancel_scope_in_another_task() -> None:
     local_scope = None
     result = False
 
@@ -365,16 +405,16 @@
             tg.start_soon(cancel_group)
             await sleep(1)
             pytest.fail("Execution should not reach this point")
 
 
 async def test_cancel_exiting_task_group() -> None:
     """
-    Test that if a task group is waiting for subtasks to finish and it receives a cancellation, the
-    subtasks are also cancelled and the waiting continues.
+    Test that if a task group is waiting for subtasks to finish and it receives a
+    cancellation, the subtasks are also cancelled and the waiting continues.
 
     """
     cancel_received = False
 
     async def waiter() -> None:
         nonlocal cancel_received
         try:
@@ -403,40 +443,32 @@
     cancel_scope.cancel()
     with cancel_scope:
         await anyio.sleep(1)  # Checkpoint to allow anyio to check for cancellation
         pytest.fail("execution should not reach this point")
 
 
 async def test_exception_group_children() -> None:
-    with pytest.raises(ExceptionGroup) as exc:
+    with pytest.raises(BaseExceptionGroup) as exc:
         async with create_task_group() as tg:
             tg.start_soon(async_error, "task1")
             tg.start_soon(async_error, "task2", 0.15)
 
     assert len(exc.value.exceptions) == 2
     assert sorted(str(e) for e in exc.value.exceptions) == ["task1", "task2"]
-    assert exc.match("^2 exceptions were raised in the task group:\n")
-    assert exc.match(r"Exception: task\d\n----")
-    assert re.fullmatch(
-        r"<ExceptionGroup: Exception\('task[12]',?\), Exception\('task[12]',?\)>",
-        repr(exc.value),
-    )
 
 
 async def test_exception_group_host() -> None:
-    with pytest.raises(ExceptionGroup) as exc:
+    with pytest.raises(BaseExceptionGroup) as exc:
         async with create_task_group() as tg:
             tg.start_soon(async_error, "child", 2)
             await wait_all_tasks_blocked()
             raise Exception("host")
 
     assert len(exc.value.exceptions) == 2
     assert sorted(str(e) for e in exc.value.exceptions) == ["child", "host"]
-    assert exc.match("^2 exceptions were raised in the task group:\n")
-    assert exc.match(r"Exception: host\n----")
 
 
 async def test_escaping_cancelled_exception() -> None:
     async with create_task_group() as tg:
         tg.cancel_scope.cancel()
         await sleep(0)
 
@@ -451,22 +483,24 @@
 @pytest.mark.parametrize("delay", [0, 0.1], ids=["instant", "delayed"])
 async def test_fail_after(delay: float) -> None:
     with pytest.raises(TimeoutError):
         with fail_after(delay) as scope:
             await sleep(1)
 
     assert scope.cancel_called
+    assert scope.cancelled_caught
 
 
 async def test_fail_after_no_timeout() -> None:
     with fail_after(None) as scope:
         assert scope.deadline == float("inf")
         await sleep(0.1)
 
     assert not scope.cancel_called
+    assert not scope.cancelled_caught
 
 
 async def test_fail_after_after_cancellation() -> None:
     event = anyio.Event()
     async with anyio.create_task_group() as tg:
         tg.cancel_scope.cancel()
         await event.wait()
@@ -476,23 +510,46 @@
         with fail_after(0.1):
             await anyio.sleep(0.5)
             block_complete = True
 
     assert not block_complete
 
 
+async def test_fail_after_cancelled_before_deadline() -> None:
+    """
+    Test that fail_after() won't raise TimeoutError if its scope is cancelled before the
+    deadline.
+
+    """
+    with fail_after(1) as scope:
+        scope.cancel()
+        await checkpoint()
+
+
+@pytest.mark.xfail(
+    reason="There is currently no way to tell if cancellation happened due to timeout "
+    "explicitly if the deadline has been exceeded"
+)
+async def test_fail_after_scope_camcelled_before_timeout() -> None:
+    with fail_after(0.1) as scope:
+        scope.cancel()
+        time.sleep(0.11)
+        await sleep(0)
+
+
 @pytest.mark.parametrize("delay", [0, 0.1], ids=["instant", "delayed"])
 async def test_move_on_after(delay: float) -> None:
     result = False
     with move_on_after(delay) as scope:
         await sleep(1)
         result = True
 
     assert not result
     assert scope.cancel_called
+    assert scope.cancelled_caught
 
 
 async def test_move_on_after_no_timeout() -> None:
     result = False
     with move_on_after(None) as scope:
         assert scope.deadline == float("inf")
         await sleep(0.1)
@@ -512,15 +569,17 @@
             sleep_completed = True
 
         inner_scope_completed = True
 
     assert not sleep_completed
     assert not inner_scope_completed
     assert outer_scope.cancel_called
+    assert outer_scope.cancelled_caught
     assert not inner_scope.cancel_called
+    assert not inner_scope.cancelled_caught
 
 
 async def test_shielding() -> None:
     async def cancel_when_ready() -> None:
         await wait_all_tasks_blocked()
         tg.cancel_scope.cancel()
 
@@ -563,14 +622,22 @@
         cancel_scope.cancel()
         assert current_effective_deadline() == -math.inf
 
         with pytest.raises(get_cancelled_exc_class()):
             await sleep(0)
 
 
+async def test_cancelled_not_caught() -> None:
+    with CancelScope() as scope:
+        scope.cancel()
+
+    assert scope.cancel_called
+    assert not scope.cancelled_caught
+
+
 @pytest.mark.parametrize("anyio_backend", ["asyncio"])
 async def test_cancel_host_asyncgen() -> None:
     done = False
 
     async def host_task() -> None:
         nonlocal done
         async with create_task_group() as tg:
@@ -589,15 +656,16 @@
     async def host_agen_fn() -> AsyncGenerator[None, None]:
         await host_task()
         yield
         pytest.fail("host_agen_fn should only be __anext__ed once")
 
     host_agen = host_agen_fn()
     try:
-        await asyncio.get_event_loop().create_task(host_agen.__anext__())  # type: ignore[arg-type]
+        loop = asyncio.get_running_loop()
+        await loop.create_task(host_agen.__anext__())  # type: ignore[arg-type]
     finally:
         await host_agen.aclose()
 
     assert done
 
 
 async def test_shielding_immediate_scope_cancelled() -> None:
@@ -667,21 +735,22 @@
         if fail:
             raise Exception("foo")
         else:
             nonlocal sleep_completed
             await sleep(1)
             sleep_completed = True
 
-    with pytest.raises(Exception) as exc:
+    with pytest.raises(ExceptionGroup) as exc:
         async with create_task_group() as tg:
             tg.start_soon(child, False)
             await wait_all_tasks_blocked()
             tg.start_soon(child, True)
 
-    exc.match("foo")
+    assert len(exc.value.exceptions) == 1
+    assert str(exc.value.exceptions[0]) == "foo"
     assert not sleep_completed
 
 
 async def test_cancel_cascade() -> None:
     async def do_something() -> NoReturn:
         async with create_task_group() as tg2:
             tg2.start_soon(sleep, 1)
@@ -758,22 +827,25 @@
 
 
 async def test_nested_shield() -> None:
     async def killer(scope: CancelScope) -> None:
         await wait_all_tasks_blocked()
         scope.cancel()
 
-    with pytest.raises(TimeoutError):
+    with pytest.raises(ExceptionGroup) as exc:
         async with create_task_group() as tg:
             with CancelScope() as scope:
                 with CancelScope(shield=True):
                     tg.start_soon(killer, scope)
                     with fail_after(0.2):
                         await sleep(2)
 
+    assert len(exc.value.exceptions) == 1
+    assert isinstance(exc.value.exceptions[0], TimeoutError)
+
 
 async def test_triple_nested_shield() -> None:
     """Regression test for #370."""
 
     got_past_checkpoint = False
 
     async def taskfunc() -> None:
@@ -819,29 +891,31 @@
 async def test_exception_group_filtering() -> None:
     """Test that CancelledErrors are filtered out of nested exception groups."""
 
     async def fail(name: str) -> NoReturn:
         try:
             await anyio.sleep(0.1)
         finally:
-            raise Exception("%s task failed" % name)
+            raise Exception(f"{name} task failed")
 
     async def fn() -> None:
         async with anyio.create_task_group() as tg:
             tg.start_soon(fail, "parent")
             async with anyio.create_task_group() as tg2:
                 tg2.start_soon(fail, "child")
                 await anyio.sleep(1)
 
-    with pytest.raises(ExceptionGroup) as exc:
+    with pytest.raises(BaseExceptionGroup) as exc:
         await fn()
 
     assert len(exc.value.exceptions) == 2
     assert str(exc.value.exceptions[0]) == "parent task failed"
-    assert str(exc.value.exceptions[1]) == "child task failed"
+    assert isinstance(exc.value.exceptions[1], ExceptionGroup)
+    assert len(exc.value.exceptions[1].exceptions) == 1
+    assert str(exc.value.exceptions[1].exceptions[0]) == "child task failed"
 
 
 async def test_cancel_propagation_with_inner_spawn() -> None:
     async def g() -> NoReturn:
         async with anyio.create_task_group() as tg2:
             tg2.start_soon(anyio.sleep, 10)
             await anyio.sleep(1)
@@ -851,15 +925,18 @@
     async with anyio.create_task_group() as tg:
         tg.start_soon(g)
         await wait_all_tasks_blocked()
         tg.cancel_scope.cancel()
 
 
 async def test_escaping_cancelled_error_from_cancelled_task() -> None:
-    """Regression test for issue #88. No CancelledError should escape the outer scope."""
+    """
+    Regression test for issue #88. No CancelledError should escape the outer scope.
+
+    """
     with CancelScope() as scope:
         with move_on_after(0.1):
             await sleep(1)
 
         scope.cancel()
 
 
@@ -867,69 +944,83 @@
     sys.version_info >= (3, 11),
     reason="Generator based coroutines have been removed in Python 3.11",
 )
 @pytest.mark.filterwarnings(
     'ignore:"@coroutine" decorator is deprecated:DeprecationWarning'
 )
 def test_cancel_generator_based_task() -> None:
-    from asyncio import coroutine  # type: ignore[attr-defined]
-
     async def native_coro_part() -> None:
         with CancelScope() as scope:
-            scope.cancel()
+            asyncio.get_running_loop().call_soon(scope.cancel)
+            await asyncio.sleep(1)
+            pytest.fail("Execution should not have reached this line")
 
-    @coroutine
+    @asyncio.coroutine  # type: ignore[attr-defined]
     def generator_part() -> Generator[object, BaseException, None]:
         yield from native_coro_part()  # type: ignore[misc]
 
     anyio.run(generator_part, backend="asyncio")
 
 
-async def test_suppress_exception_context() -> None:
+@pytest.mark.skipif(
+    sys.version_info >= (3, 11),
+    reason="Generator based coroutines have been removed in Python 3.11",
+)
+@pytest.mark.filterwarnings(
+    'ignore:"@coroutine" decorator is deprecated:DeprecationWarning'
+)
+@pytest.mark.parametrize("anyio_backend", ["asyncio"])
+async def test_schedule_old_style_coroutine_func() -> None:
     """
-    Test that the __context__ attribute has been cleared when the exception is re-raised in the
-    exception group. This prevents recursive tracebacks.
-
+    Test that we give a sensible error when a user tries to spawn a task from a
+    generator-style coroutine function.
     """
-    with pytest.raises(ValueError) as exc:
-        async with create_task_group() as tg:
-            tg.cancel_scope.cancel()
-            async with create_task_group() as tg2:
-                tg2.start_soon(sleep, 1)
-                raise ValueError
 
-    assert exc.value.__context__ is None
+    @asyncio.coroutine  # type: ignore[attr-defined]
+    def corofunc() -> Generator[Any, Any, None]:
+        yield from asyncio.sleep(1)  # type: ignore[misc]
+
+    async with create_task_group() as tg:
+        funcname = (
+            f"{__name__}.test_schedule_old_style_coroutine_func.<locals>.corofunc"
+        )
+        with pytest.raises(
+            TypeError,
+            match=f"Expected {funcname}\\(\\) to return a coroutine, but the return "
+            f"value \\(<generator .+>\\) is not a coroutine object",
+        ):
+            tg.start_soon(corofunc)
 
 
 @pytest.mark.parametrize("anyio_backend", ["asyncio"])
 async def test_cancel_native_future_tasks() -> None:
     async def wait_native_future() -> None:
-        loop = asyncio.get_event_loop()
+        loop = asyncio.get_running_loop()
         await loop.create_future()
 
     async with anyio.create_task_group() as tg:
         tg.start_soon(wait_native_future)
         tg.cancel_scope.cancel()
 
 
 @pytest.mark.parametrize("anyio_backend", ["asyncio"])
 async def test_cancel_native_future_tasks_cancel_scope() -> None:
     async def wait_native_future() -> None:
         with anyio.CancelScope():
-            loop = asyncio.get_event_loop()
+            loop = asyncio.get_running_loop()
             await loop.create_future()
 
     async with anyio.create_task_group() as tg:
         tg.start_soon(wait_native_future)
         tg.cancel_scope.cancel()
 
 
 @pytest.mark.parametrize("anyio_backend", ["asyncio"])
 async def test_cancel_completed_task() -> None:
-    loop = asyncio.get_event_loop()
+    loop = asyncio.get_running_loop()
     old_exception_handler = loop.get_exception_handler()
     exceptions = []
 
     def exception_handler(*args: object, **kwargs: object) -> None:
         exceptions.append((args, kwargs))
 
     loop.set_exception_handler(exception_handler)
@@ -964,15 +1055,18 @@
         tg.start_soon(task_wrap)
 
     assert inner_task_id is not None
     assert inner_task_id != outer_task_id
 
 
 async def test_shielded_cancel_sleep_time() -> None:
-    """Test that cancelling a shielded tasks spends more time sleeping than cancelling."""
+    """
+    Test that cancelling a shielded tasks spends more time sleeping than cancelling.
+
+    """
     event = anyio.Event()
     hang_time = 0.2
 
     async def set_event() -> None:
         await sleep(hang_time)
         event.set()
 
@@ -990,26 +1084,31 @@
             process_time = time.process_time()
 
         assert (time.process_time() - process_time) < hang_time
 
 
 async def test_cancelscope_wrong_exit_order() -> None:
     """
-    Test that a RuntimeError is raised if the task tries to exit cancel scopes in the wrong order.
+    Test that a RuntimeError is raised if the task tries to exit cancel scopes in the
+    wrong order.
 
     """
     scope1 = CancelScope()
     scope2 = CancelScope()
     scope1.__enter__()
     scope2.__enter__()
     pytest.raises(RuntimeError, scope1.__exit__, None, None, None)
 
 
 async def test_cancelscope_exit_before_enter() -> None:
-    """Test that a RuntimeError is raised if one tries to exit a cancel scope before entering."""
+    """
+    Test that a RuntimeError is raised if one tries to exit a cancel scope before
+    entering.
+
+    """
     scope = CancelScope()
     pytest.raises(RuntimeError, scope.__exit__, None, None, None)
 
 
 @pytest.mark.parametrize(
     "anyio_backend", ["asyncio"]
 )  # trio does not check for this yet
@@ -1020,62 +1119,68 @@
     async def exit_scope(scope: CancelScope) -> None:
         scope.__exit__(None, None, None)
 
     scope = CancelScope()
     async with create_task_group() as tg:
         tg.start_soon(enter_scope, scope)
 
-    with pytest.raises(RuntimeError):
+    with pytest.raises(ExceptionGroup) as exc:
         async with create_task_group() as tg:
             tg.start_soon(exit_scope, scope)
 
+    assert len(exc.value.exceptions) == 1
+    assert str(exc.value.exceptions[0]) == (
+        "Attempted to exit cancel scope in a different task than it was entered in"
+    )
+
 
 def test_unhandled_exception_group(caplog: pytest.LogCaptureFixture) -> None:
     def crash() -> NoReturn:
         raise KeyboardInterrupt
 
     async def nested() -> None:
         async with anyio.create_task_group() as tg:
             tg.start_soon(anyio.sleep, 5)
             await anyio.sleep(5)
 
     async def main() -> NoReturn:
         async with anyio.create_task_group() as tg:
             tg.start_soon(nested)
             await wait_all_tasks_blocked()
-            asyncio.get_event_loop().call_soon(crash)
+            asyncio.get_running_loop().call_soon(crash)
             await anyio.sleep(5)
 
         pytest.fail("Execution should never reach this point")
 
     with pytest.raises(KeyboardInterrupt):
         anyio.run(main, backend="asyncio")
 
     assert not caplog.messages
 
 
-@pytest.mark.skipif(
-    sys.version_info < (3, 9),
-    sys.version_info >= (3, 11),
-    reason="Cancel messages are only supported on Python 3.9 and 3.10",
-)
-@pytest.mark.parametrize("anyio_backend", ["asyncio"])
-async def test_cancellederror_combination_with_message() -> None:
-    async def taskfunc(*, task_status: TaskStatus) -> NoReturn:
-        task_status.started(asyncio.current_task())
-        await sleep(5)
-        pytest.fail("Execution should never reach this point")
+async def test_single_cancellation_exc() -> None:
+    """
+    Test that only a single cancellation exception bubbles out of the task group when
+    case it was cancelled via an outer scope and no actual errors were raised.
 
-    with pytest.raises(asyncio.CancelledError, match="blah"):
-        async with create_task_group() as tg:
-            task = await tg.start(taskfunc)
-            tg.start_soon(sleep, 5)
-            await wait_all_tasks_blocked()
-            assert isinstance(task, asyncio.Task)
-            task.cancel("blah")
+    """
+    with CancelScope() as outer:
+        try:
+            async with create_task_group() as tg:
+                tg.start_soon(sleep, 5)
+                await wait_all_tasks_blocked()
+                outer.cancel()
+                await sleep(5)
+        except BaseException as exc:
+            if isinstance(exc, get_cancelled_exc_class()):
+                raise
+
+            pytest.fail(f"Raised the wrong type of exception: {exc}")
+        else:
+            pytest.fail("Did not raise a cancellation exception")
 
 
 async def test_start_soon_parent_id() -> None:
     root_task_id = get_current_task().id
     parent_id: int | None = None
 
     async def subtask() -> None:
@@ -1146,14 +1251,23 @@
             task.cancel()
             await anyio.sleep(0)
 
         assert task.cancelling() == 1
         task.uncancel()
 
 
+async def test_cancel_before_entering_task_group() -> None:
+    with CancelScope() as scope:
+        scope.cancel()
+        async with create_task_group():
+            pass
+
+        pytest.fail("Execution should never reach this point")
+
+
 class TestTaskStatusTyping:
     """
     These tests do not do anything at run time, but since the test suite is also checked
     with a static type checker, it ensures that the `TaskStatus` typing works as
     intended.
     """
```

### Comparing `anyio-3.7.1/tests/test_to_process.py` & `anyio-4.0.0rc1/tests/test_to_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,23 @@
 
 
 @pytest.fixture(autouse=True)
 def check_compatibility(anyio_backend_name: str) -> None:
     if anyio_backend_name == "asyncio":
         if platform.system() == "Windows" and sys.version_info < (3, 8):
             pytest.skip(
-                "Python < 3.8 uses SelectorEventLoop by default and it does not support "
-                "subprocesses"
+                "Python < 3.8 uses SelectorEventLoop by default and it does not "
+                "support subprocesses"
             )
 
 
 async def test_run_sync_in_process_pool() -> None:
     """
-    Test that the function runs in a different process, and the same process in both calls.
+    Test that the function runs in a different process, and the same process in both
+    calls.
 
     """
     worker_pid = await to_process.run_sync(os.getpid)
     assert worker_pid != os.getpid()
     assert await to_process.run_sync(os.getpid) == worker_pid
 
 
@@ -64,28 +65,29 @@
     await to_process.run_sync(print, "hello")
     await to_process.run_sync(print, "world")
     assert await to_process.run_sync(os.getpid) == worker_pid
 
 
 async def test_cancel_before() -> None:
     """
-    Test that starting to_process.run_sync() in a cancelled scope does not cause a worker
-    process to be reserved.
+    Test that starting to_process.run_sync() in a cancelled scope does not cause a
+    worker process to be reserved.
 
     """
     with CancelScope() as scope:
         scope.cancel()
         await to_process.run_sync(os.getpid)
 
     pytest.raises(LookupError, to_process._process_pool_workers.get)
 
 
 async def test_cancel_during() -> None:
     """
-    Test that cancelling an operation on the worker process causes the process to be killed.
+    Test that cancelling an operation on the worker process causes the process to be
+    killed.
 
     """
     worker_pid = await to_process.run_sync(os.getpid)
     with fail_after(4):
         async with create_task_group() as tg:
             tg.start_soon(partial(to_process.run_sync, cancellable=True), time.sleep, 5)
             await wait_all_tasks_blocked()
```

### Comparing `anyio-3.7.1/tests/test_to_thread.py` & `anyio-4.0.0rc1/tests/test_to_thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,16 @@
     [(False, "task"), (True, "thread")],
     ids=["uncancellable", "cancellable"],
 )
 async def test_cancel_worker_thread(
     cancellable: bool, expected_last_active: str
 ) -> None:
     """
-    Test that when a task running a worker thread is cancelled, the cancellation is not acted on
-    until the thread finishes.
+    Test that when a task running a worker thread is cancelled, the cancellation is not
+    acted on until the thread finishes.
 
     """
     last_active: str | None = None
 
     def thread_worker() -> None:
         nonlocal last_active
         from_thread.run_sync(sleep_event.set)
@@ -167,17 +167,17 @@
         task.cancel()
 
 
 def test_asyncio_no_root_task(asyncio_event_loop: asyncio.AbstractEventLoop) -> None:
     """
     Regression test for #264.
 
-    Ensures that to_thread.run_sync() does not raise an error when there is no root task, but
-    instead tries to find the top most parent task by traversing the cancel scope tree, or failing
-    that, uses the current task to set up a shutdown callback.
+    Ensures that to_thread.run_sync() does not raise an error when there is no root
+    task, but instead tries to find the top most parent task by traversing the cancel
+    scope tree, or failing that, uses the current task to set up a shutdown callback.
 
     """
 
     async def run_in_thread() -> None:
         try:
             await to_thread.run_sync(time.sleep, 0)
         finally:
@@ -253,16 +253,16 @@
         event1.set()
         await event2.wait()
 
     async def taskfunc2() -> None:
         await event1.wait()
         asyncio_event_loop.call_soon(event2.set)
         await anyio.to_thread.run_sync(time.sleep, 0)
-        # At this point, the worker would be stopped but still in the idle workers pool, so the
-        # following would hang prior to the fix
+        # At this point, the worker would be stopped but still in the idle workers pool,
+        # so the following would hang prior to the fix
         await anyio.to_thread.run_sync(time.sleep, 0)
 
     event1 = asyncio.Event()
     event2 = asyncio.Event()
     task1 = asyncio_event_loop.create_task(taskfunc1())
     task2 = asyncio_event_loop.create_task(taskfunc2())
     asyncio_event_loop.run_until_complete(asyncio.gather(task1, task2))
```

