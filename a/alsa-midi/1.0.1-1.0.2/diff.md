# Comparing `tmp/alsa-midi-1.0.1.tar.gz` & `tmp/alsa-midi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-alsa-midi/python-alsa-midi/dist/tmp1xlclfg9/alsa-midi-1.0.1.tar", last modified: Tue May 31 07:56:58 2022, max compression
+gzip compressed data, was "/home/runner/work/python-alsa-midi/python-alsa-midi/dist/.tmp-k1po3rle/alsa-midi-1.0.2.tar", last modified: Wed Jul 26 13:10:39 2023, max compression
```

## Comparing `alsa-midi-1.0.1.tar` & `alsa-midi-1.0.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 07:56:58.000000 alsa-midi-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 07:56:58.000000 alsa-midi-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 07:56:58.000000 alsa-midi-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     6968 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3658 2022-05-31 07:56:58.000000 alsa-midi-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2783 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 07:56:58.000000 alsa-midi-1.0.1/alsa_midi/
--rw-r--r--   0 runner    (1001) docker     (121)     3427 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/alsa_midi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/alsa_midi/_ffi.py
--rw-r--r--   0 runner    (1001) docker     (121)    41689 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/alsa_midi/_ffi_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3005 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/alsa_midi/address.py
--rw-r--r--   0 runner    (1001) docker     (121)    75170 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/alsa_midi/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    40152 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/alsa_midi/event.py
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/alsa_midi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7513 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/alsa_midi/mido_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)    10949 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/alsa_midi/port.py
--rw-r--r--   0 runner    (1001) docker     (121)    15823 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/alsa_midi/queue.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/alsa_midi/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 07:56:58.000000 alsa-midi-1.0.1/alsa_midi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3658 2022-05-31 07:56:57.000000 alsa-midi-1.0.1/alsa_midi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-05-31 07:56:58.000000 alsa-midi-1.0.1/alsa_midi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-31 07:56:57.000000 alsa-midi-1.0.1/alsa_midi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-31 07:56:57.000000 alsa-midi-1.0.1/alsa_midi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-05-31 07:56:57.000000 alsa-midi-1.0.1/alsa_midi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-05-31 07:56:57.000000 alsa-midi-1.0.1/alsa_midi.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     2180 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/build-wheels.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 07:56:58.000000 alsa-midi-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)  1882978 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/docs/alsa.tag
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/docs/api_async_client.rst
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/docs/api_client.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3516 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/docs/api_events.rst
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/docs/api_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/docs/api_misc.rst
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/docs/api_port.rst
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/docs/api_queue.rst
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7161 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 07:56:58.000000 alsa-midi-1.0.1/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1403 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/examples/connect.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2270 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/examples/dump_bytes.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2701 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/examples/dump_events.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      965 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/examples/list_clients.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2786 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/examples/list_ports.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2048 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/examples/list_ports_full.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2046 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/examples/play_the_lick.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2122 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/examples/play_the_lick_bytes.py
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-05-31 07:56:58.000000 alsa-midi-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 07:56:58.000000 alsa-midi-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/Vagrantfile
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16600 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 07:56:58.000000 alsa-midi-1.0.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/data/c_major.mid
--rwxr-xr-x   0 runner    (1001) docker     (121)     1536 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/data/generate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/test_address.py
--rw-r--r--   0 runner    (1001) docker     (121)    21537 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/test_compile_no_compile.py
--rw-r--r--   0 runner    (1001) docker     (121)    82701 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/test_event_async_input.py
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/test_event_async_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     4999 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/test_event_input.py
--rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/test_event_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     9669 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/test_port.py
--rw-r--r--   0 runner    (1001) docker     (121)    18927 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/test_port_query.py
--rw-r--r--   0 runner    (1001) docker     (121)    12766 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/test_realtime.py
--rw-r--r--   0 runner    (1001) docker     (121)     2575 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/test_remove_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     5503 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/test_subs_query.py
--rw-r--r--   0 runner    (1001) docker     (121)     2039 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-05-31 07:56:24.000000 alsa-midi-1.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/alsa_midi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/alsa_midi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/alsa_midi/_ffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41689 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/alsa_midi/_ffi_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/alsa_midi/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75194 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/alsa_midi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40156 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/alsa_midi/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/alsa_midi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/alsa_midi/mido_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/alsa_midi/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15847 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/alsa_midi/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/alsa_midi/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/alsa_midi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/alsa_midi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/alsa_midi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/alsa_midi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/alsa_midi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/alsa_midi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/alsa_midi.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2188 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/build-wheels.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)  1882978 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/docs/alsa.tag
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/docs/api_async_client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/docs/api_client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/docs/api_events.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/docs/api_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/docs/api_misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/docs/api_port.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/docs/api_queue.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1403 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/examples/connect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2270 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/examples/dump_bytes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2701 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/examples/dump_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      965 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/examples/list_clients.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2786 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/examples/list_ports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2048 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/examples/list_ports_full.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2046 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/examples/play_the_lick.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2122 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/examples/play_the_lick_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/Vagrantfile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16600 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:10:39.000000 alsa-midi-1.0.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/data/c_major.mid
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1536 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/data/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21537 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/test_compile_no_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82701 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/test_event_async_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/test_event_async_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/test_event_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/test_event_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/test_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18927 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/test_port_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/test_realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/test_remove_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/test_subs_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-26 13:10:11.000000 alsa-midi-1.0.2/tox.ini
```

### Comparing `alsa-midi-1.0.1/.github/workflows/ci.yml` & `alsa-midi-1.0.2/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 jobs:
   check:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Set up Python 3.9
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.9
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install isort==5.10.1 flake8==3.8.3
@@ -38,42 +38,50 @@
   test:
 
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox
         sudo apt update
         sudo apt install -y libasound2-dev
 
     - name: Run tests
       run: "tox -e py -- -vv"
 
   test-on-alsa-kernel:
-    runs-on: macos-10.15
+    runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
+
+    - name: Install vagrant
+      run: |
+        sudo apt update
+        sudo apt install -y vagrant libvirt-daemon libvirt-daemon-driver-qemu libvirt-clients libvirt-daemon-system
+        sudo systemctl
+        sudo systemctl status libvirtd.service
+        sudo chmod a+rw /var/run/libvirt/libvirt-sock
 
     - name: Cache Vagrant boxes
-      uses: actions/cache@v2
+      uses: actions/cache@v3
       with:
         path: ~/.vagrant.d/boxes
         key: ${{ runner.os }}-vagrant-${{ hashFiles('Vagrantfile') }}
         restore-keys: |
           ${{ runner.os }}-vagrant-
 
     - name: Start vagrant VM
@@ -91,20 +99,20 @@
     needs:
       - test
       - test-on-alsa-kernel
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
     - name: Set up Python 3.7
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.7
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install build twine
@@ -113,15 +121,15 @@
     - name: Build
       run: |
         export PY_ALSA_MIDI_NO_COMPILE=1
         python -m build .
         twine check dist/*
 
     - name: Upload artifacts
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: dist-pure
         path: dist
 
   # separate jobs, as matrix does not work with 'uses: docker://' and 'container:' does not work well with 'actions/checkout'
 
   build-manylinux_2_12_x86_64:
@@ -130,167 +138,140 @@
       - test
       - test-on-alsa-kernel
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Checkout the code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
     - name: Build and test ${{ matrix.manylinux-tag }} wheels
       uses: docker://quay.io/pypa/manylinux2010_x86_64
       with:
         args: ./build-wheels.sh manylinux_2_12_x86_64
 
     - name: Upload artifacts
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: wheelhouse-manylinux_2_12_x86_64
         path: wheelhouse
 
   build-manylinux_2_12_i686:
 
     needs:
       - test
       - test-on-alsa-kernel
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Checkout the code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
     - name: Build and test ${{ matrix.manylinux-tag }} wheels
       uses: docker://quay.io/pypa/manylinux2010_i686
       with:
         args: linux32 ./build-wheels.sh manylinux_2_12_i686
 
     - name: Upload artifacts
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: wheelhouse-manylinux_2_12_i686
         path: wheelhouse
 
   build-manylinux_2_17_x86_64:
 
     needs:
       - test
       - test-on-alsa-kernel
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Checkout the code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
     - name: Build and test ${{ matrix.manylinux-tag }} wheels
       uses: docker://quay.io/pypa/manylinux2014_x86_64
       with:
         args: ./build-wheels.sh manylinux_2_17_x86_64
 
     - name: Upload artifacts
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: wheelhouse-manylinux_2_17_x86_64
         path: wheelhouse
 
   build-manylinux_2_17_i686:
 
     needs:
       - test
       - test-on-alsa-kernel
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Checkout the code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
     - name: Build and test ${{ matrix.manylinux-tag }} wheels
       uses: docker://quay.io/pypa/manylinux2014_i686
       with:
         args: linux32 ./build-wheels.sh manylinux_2_17_i686
 
     - name: Upload artifacts
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: wheelhouse-manylinux_2_17_i686
         path: wheelhouse
 
-  build-manylinux_2_24_x86_64:
-
-    needs:
-      - test
-      - test-on-alsa-kernel
-
-    runs-on: ubuntu-latest
-
-    steps:
-    - name: Checkout the code
-      uses: actions/checkout@v2
-      with:
-        fetch-depth: 0
-
-    - name: Build and test ${{ matrix.manylinux-tag }} wheels
-      uses: docker://quay.io/pypa/manylinux_2_24_x86_64
-      with:
-        args: ./build-wheels.sh manylinux_2_24_x86_64
-
-    - name: Upload artifacts
-      uses: actions/upload-artifact@v2
-      with:
-        name: wheelhouse-manylinux_2_24_x86_64
-        path: wheelhouse
-
-  build-manylinux_2_24_i686:
+  build-manylinux_2_28_x86_64:
 
     needs:
       - test
       - test-on-alsa-kernel
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Checkout the code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
     - name: Build and test ${{ matrix.manylinux-tag }} wheels
-      uses: docker://quay.io/pypa/manylinux_2_24_i686
+      uses: docker://quay.io/pypa/manylinux_2_28_x86_64
       with:
-        args: linux32 ./build-wheels.sh manylinux_2_24_i686
+        args: ./build-wheels.sh manylinux_2_28_x86_64
 
     - name: Upload artifacts
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
-        name: wheelhouse-manylinux_2_24_i686
+        name: wheelhouse-manylinux_2_28_x86_64
         path: wheelhouse
 
-
   publish:
 
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
 
     needs:
       - build-pure
       - build-manylinux_2_12_x86_64
       - build-manylinux_2_12_i686
       - build-manylinux_2_17_x86_64
       - build-manylinux_2_17_i686
-      - build-manylinux_2_24_x86_64
-      - build-manylinux_2_24_i686
+      - build-manylinux_2_28_x86_64
 
     runs-on: ubuntu-latest
 
     steps:
       - name: Download artifacts
         uses: actions/download-artifact@v2
```

### Comparing `alsa-midi-1.0.1/LICENSE` & `alsa-midi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/PKG-INFO` & `alsa-midi-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alsa-midi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python interface for ALSA MIDI sequencer
 License: MIT
 Project-URL: GitHub, https://github.com/Jajcus/python-alsa-midi/
 Project-URL: Documentation, https://python-alsa-midi.readthedocs.io/
 Keywords: ALSA MIDI sequencer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -35,15 +35,15 @@
 
   * Precise timestamping of messages sent and received
   * Port connection management, including connection between ports on different
     clients
   * Access to non-MIDI events, like announcements about new clients, ports and
     connections
 
-* Python 3.7 – 3.10 compatibility
+* Python 3.7 – 3.11 compatibility
 
 * Both synchronous (blocking) and asynchronous (asyncio) I/O
 
 * Only Python code, no need to compile a binary module. Requires `cffi`_, though.
 
 * `MIDO`_ backend provided
```

### Comparing `alsa-midi-1.0.1/README.rst` & `alsa-midi-1.0.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
   * Precise timestamping of messages sent and received
   * Port connection management, including connection between ports on different
     clients
   * Access to non-MIDI events, like announcements about new clients, ports and
     connections
 
-* Python 3.7 – 3.10 compatibility
+* Python 3.7 – 3.11 compatibility
 
 * Both synchronous (blocking) and asynchronous (asyncio) I/O
 
 * Only Python code, no need to compile a binary module. Requires `cffi`_, though.
 
 * `MIDO`_ backend provided
```

### Comparing `alsa-midi-1.0.1/alsa_midi/__init__.py` & `alsa-midi-1.0.2/alsa_midi/__init__.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/alsa_midi/_ffi_defs.py` & `alsa-midi-1.0.2/alsa_midi/_ffi_defs.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/alsa_midi/address.py` & `alsa-midi-1.0.2/alsa_midi/address.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/alsa_midi/client.py` & `alsa-midi-1.0.2/alsa_midi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import asyncio
 import errno
 import select
 import time
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from enum import IntEnum, IntFlag
 from functools import partial
 from typing import (Any, Callable, List, MutableMapping, NewType, Optional, Set, Tuple, Union,
                     overload)
 from weakref import WeakValueDictionary
 
 from ._ffi import alsa, ffi
@@ -333,15 +333,15 @@
 @dataclass
 class RemoveEvents:
     """Events removal condition.
 
     Represents :alsa:`snd_seq_remove_events_t` data."""
     condition: RemoveCondition = RemoveCondition(0)
     queue_id: int = 0
-    time: Union[RealTime, int] = RealTime(0, 0)
+    time: Union[RealTime, int] = field(default_factory=RealTime)
     dest: AddressType = Address(0, 0)
     channel: int = 0
     event_type: EventType = EventType.NONE
     tag: int = 0
 
 
 class SequencerClientBase:
```

### Comparing `alsa-midi-1.0.1/alsa_midi/event.py` & `alsa-midi-1.0.2/alsa_midi/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     :ivar nanoseconds: number of nanoseconds
     """
     __slots__ = ('seconds', 'nanoseconds')
 
     seconds: int
     nanoseconds: int
 
-    def __init__(self, seconds: Union[float, int, str, 'RealTime'], nanoseconds: int = 0):
+    def __init__(self, seconds: Union[float, int, str, 'RealTime'] = 0, nanoseconds: int = 0):
         if isinstance(seconds, RealTime):
             self.seconds = seconds.seconds
             self.nanoseconds = seconds.nanoseconds + nanoseconds
         else:
             if isinstance(seconds, str):
                 if "." in seconds:
                     seconds = float(seconds)
```

### Comparing `alsa-midi-1.0.1/alsa_midi/exceptions.py` & `alsa-midi-1.0.2/alsa_midi/exceptions.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/alsa_midi/mido_backend.py` & `alsa-midi-1.0.2/alsa_midi/mido_backend.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/alsa_midi/port.py` & `alsa-midi-1.0.2/alsa_midi/port.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/alsa_midi/queue.py` & `alsa-midi-1.0.2/alsa_midi/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from enum import IntEnum
 from typing import TYPE_CHECKING, NamedTuple, NewType, Optional, Union
 
 from ._ffi import alsa, ffi
 from .event import EventType, RealTime
 from .exceptions import Error, StateError
 from .util import _check_alsa_error
@@ -82,15 +82,15 @@
     :ivar tick_time: queue time in ticks
     :ivar real_time: queue time in seconds and nanoseconds
     :ivar status: running status bits
     """
     queue_id: int = 0
     events: int = 0
     tick_time: int = 0
-    real_time: RealTime = RealTime(0, 0)
+    real_time: RealTime = field(default_factory=RealTime)
     status: int = 0
 
     @classmethod
     def _from_alsa(cls, info: _snd_seq_queue_status_t):
         """Create a QueueStatus object from ALSA :alsa:`snd_seq_queue_status_t`."""
         real_time = alsa.snd_seq_queue_status_get_real_time(info)
         return cls(
```

### Comparing `alsa-midi-1.0.1/alsa_midi/util.py` & `alsa-midi-1.0.2/alsa_midi/util.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/alsa_midi.egg-info/PKG-INFO` & `alsa-midi-1.0.2/alsa_midi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alsa-midi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python interface for ALSA MIDI sequencer
 License: MIT
 Project-URL: GitHub, https://github.com/Jajcus/python-alsa-midi/
 Project-URL: Documentation, https://python-alsa-midi.readthedocs.io/
 Keywords: ALSA MIDI sequencer
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -35,15 +35,15 @@
 
   * Precise timestamping of messages sent and received
   * Port connection management, including connection between ports on different
     clients
   * Access to non-MIDI events, like announcements about new clients, ports and
     connections
 
-* Python 3.7 – 3.10 compatibility
+* Python 3.7 – 3.11 compatibility
 
 * Both synchronous (blocking) and asynchronous (asyncio) I/O
 
 * Only Python code, no need to compile a binary module. Requires `cffi`_, though.
 
 * `MIDO`_ backend provided
```

### Comparing `alsa-midi-1.0.1/alsa_midi.egg-info/SOURCES.txt` & `alsa-midi-1.0.2/alsa_midi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/build-wheels.sh` & `alsa-midi-1.0.2/build-wheels.sh`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 fi
 
 # stop git from panicing because this is run as root
 # as it breaks setuptools_scm
 git config --global --add safe.directory "$GITHUB_WORKSPACE"
 
 # Compile wheels
-for PYBIN in /opt/python/cp{37,38,39,310}*/bin; do
+for PYBIN in /opt/python/cp{37,38,39,310,311}*/bin; do
     [ -d "$PYBIN" ] || continue
     "${PYBIN}/pip" install --upgrade pip setuptools
     "${PYBIN}/pip" install -r "$GITHUB_WORKSPACE/requirements.txt"
 
     "${PYBIN}/pip" wheel "$GITHUB_WORKSPACE" --no-deps -w wheelhouse/
 done
 
@@ -72,14 +72,14 @@
 done
 
 # remove 'bad' linux_* wheels
 rm wheelhouse/*-linux_*.whl
 
 # Install packages and test
 cd /
-for PYBIN in /opt/python/cp{37,38,39,310}*/bin/; do
+for PYBIN in /opt/python/cp{37,38,39,310,311}*/bin/; do
     [ -d "$PYBIN" ] || continue
 
     "${PYBIN}/pip" install pytest pytest-asyncio
     "${PYBIN}/pip" install alsa-midi --no-index -f "$GITHUB_WORKSPACE/wheelhouse/"
     "${PYBIN}/python" -m pytest -vv "$GITHUB_WORKSPACE/tests"
 done
```

### Comparing `alsa-midi-1.0.1/docs/Makefile` & `alsa-midi-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/docs/alsa.tag` & `alsa-midi-1.0.2/docs/alsa.tag`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/docs/api_events.rst` & `alsa-midi-1.0.2/docs/api_events.rst`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/docs/api_misc.rst` & `alsa-midi-1.0.2/docs/api_misc.rst`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/docs/api_port.rst` & `alsa-midi-1.0.2/docs/api_port.rst`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/docs/conf.py` & `alsa-midi-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/docs/requirements.txt` & `alsa-midi-1.0.2/docs/requirements.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 alabaster==0.7.12
 Babel==2.9.1
-certifi==2021.10.8
+certifi==2023.07.22
 cffi==1.15.0
 charset-normalizer==2.0.9
 docutils==0.17.1
 idna==3.3
 imagesize==1.3.0
 Jinja2==3.0.3
 MarkupSafe==2.0.1
 packaging==21.3
 pycparser==2.21
-Pygments==2.10.0
+Pygments==2.15.0
 pyparsing==3.0.6
 python-dateutil==2.8.2
 pytz==2021.3
-requests==2.26.0
+requests==2.31.0
 six==1.16.0
 snowballstemmer==2.2.0
 Sphinx==4.3.2
 sphinx-rtd-theme==1.0.0
 sphinxcontrib-applehelp==1.0.2
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-doxylink==1.11.1
```

### Comparing `alsa-midi-1.0.1/docs/usage.rst` & `alsa-midi-1.0.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/examples/connect.py` & `alsa-midi-1.0.2/examples/connect.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/examples/dump_bytes.py` & `alsa-midi-1.0.2/examples/dump_bytes.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/examples/dump_events.py` & `alsa-midi-1.0.2/examples/dump_events.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/examples/list_clients.py` & `alsa-midi-1.0.2/examples/list_clients.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/examples/list_ports.py` & `alsa-midi-1.0.2/examples/list_ports.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/examples/list_ports_full.py` & `alsa-midi-1.0.2/examples/list_ports_full.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/examples/play_the_lick.py` & `alsa-midi-1.0.2/examples/play_the_lick.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/examples/play_the_lick_bytes.py` & `alsa-midi-1.0.2/examples/play_the_lick_bytes.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/setup.cfg` & `alsa-midi-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/conftest.py` & `alsa-midi-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/data/generate.py` & `alsa-midi-1.0.2/tests/data/generate.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/test_address.py` & `alsa-midi-1.0.2/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/test_client.py` & `alsa-midi-1.0.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/test_compile_no_compile.py` & `alsa-midi-1.0.2/tests/test_compile_no_compile.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/test_event.py` & `alsa-midi-1.0.2/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/test_event_async_input.py` & `alsa-midi-1.0.2/tests/test_event_async_input.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/test_event_async_output.py` & `alsa-midi-1.0.2/tests/test_event_async_output.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/test_event_input.py` & `alsa-midi-1.0.2/tests/test_event_input.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/test_event_output.py` & `alsa-midi-1.0.2/tests/test_event_output.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/test_port.py` & `alsa-midi-1.0.2/tests/test_port.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/test_port_query.py` & `alsa-midi-1.0.2/tests/test_port_query.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/test_queue.py` & `alsa-midi-1.0.2/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/test_realtime.py` & `alsa-midi-1.0.2/tests/test_realtime.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/test_remove_events.py` & `alsa-midi-1.0.2/tests/test_remove_events.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/test_subs_query.py` & `alsa-midi-1.0.2/tests/test_subs_query.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tests/test_util.py` & `alsa-midi-1.0.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `alsa-midi-1.0.1/tox.ini` & `alsa-midi-1.0.2/tox.ini`

 * *Files identical despite different names*

