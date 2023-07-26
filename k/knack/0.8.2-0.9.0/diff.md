# Comparing `tmp/knack-0.8.2.tar.gz` & `tmp/knack-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/vsts/work/1/a/knack-0.8.2.tar", last modified: Sat May  8 06:50:47 2021, max compression
+gzip compressed data, was "knack-0.9.0.tar", last modified: Fri Nov  5 05:18:29 2021, max compression
```

## Comparing `knack-0.8.2.tar` & `knack-0.9.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-08 06:50:47.000000 knack-0.8.2/
--rw-r--r--   0 vsts      (1001) docker     (118)     6244 2021-05-08 06:50:47.000000 knack-0.8.2/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-08 06:50:47.000000 knack-0.8.2/knack.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (118)     6244 2021-05-08 06:50:47.000000 knack-0.8.2/knack.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (118)        6 2021-05-08 06:50:47.000000 knack-0.8.2/knack.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (118)     1307 2021-05-08 06:50:47.000000 knack-0.8.2/knack.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (118)        1 2021-05-08 06:50:47.000000 knack-0.8.2/knack.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (118)       55 2021-05-08 06:50:47.000000 knack-0.8.2/knack.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (118)        1 2021-05-08 06:50:47.000000 knack-0.8.2/knack.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (118)       56 2021-05-08 06:50:44.000000 knack-0.8.2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (118)      551 2021-05-08 06:50:44.000000 knack-0.8.2/CONTRIBUTING.rst
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-08 06:50:47.000000 knack-0.8.2/knack/
--rw-r--r--   0 vsts      (1001) docker     (118)    13424 2021-05-08 06:50:44.000000 knack-0.8.2/knack/parser.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1233 2021-05-08 06:50:44.000000 knack-0.8.2/knack/events.py
--rw-r--r--   0 vsts      (1001) docker     (118)      583 2021-05-08 06:50:44.000000 knack-0.8.2/knack/help_files.py
--rw-r--r--   0 vsts      (1001) docker     (118)    11497 2021-05-08 06:50:44.000000 knack-0.8.2/knack/config.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2677 2021-05-08 06:50:44.000000 knack-0.8.2/knack/query.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4003 2021-05-08 06:50:44.000000 knack-0.8.2/knack/introspection.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9545 2021-05-08 06:50:44.000000 knack-0.8.2/knack/log.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5784 2021-05-08 06:50:44.000000 knack-0.8.2/knack/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2902 2021-05-08 06:50:44.000000 knack-0.8.2/knack/preview.py
--rw-r--r--   0 vsts      (1001) docker     (118)      602 2021-05-08 06:50:44.000000 knack-0.8.2/knack/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)    12357 2021-05-08 06:50:44.000000 knack-0.8.2/knack/cli.py
--rw-r--r--   0 vsts      (1001) docker     (118)      699 2021-05-08 06:50:44.000000 knack-0.8.2/knack/validators.py
--rw-r--r--   0 vsts      (1001) docker     (118)    10143 2021-05-08 06:50:44.000000 knack-0.8.2/knack/invocation.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3022 2021-05-08 06:50:44.000000 knack-0.8.2/knack/experimental.py
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-08 06:50:47.000000 knack-0.8.2/knack/testsdk/
--rw-r--r--   0 vsts      (1001) docker     (118)     3968 2021-05-08 06:50:44.000000 knack-0.8.2/knack/testsdk/recording_processors.py
--rw-r--r--   0 vsts      (1001) docker     (118)      847 2021-05-08 06:50:44.000000 knack-0.8.2/knack/testsdk/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)      798 2021-05-08 06:50:44.000000 knack-0.8.2/knack/testsdk/decorators.py
--rw-r--r--   0 vsts      (1001) docker     (118)      899 2021-05-08 06:50:44.000000 knack-0.8.2/knack/testsdk/patches.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4419 2021-05-08 06:50:44.000000 knack-0.8.2/knack/testsdk/checkers.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1132 2021-05-08 06:50:44.000000 knack-0.8.2/knack/testsdk/util.py
--rw-r--r--   0 vsts      (1001) docker     (118)      463 2021-05-08 06:50:44.000000 knack-0.8.2/knack/testsdk/const.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1157 2021-05-08 06:50:44.000000 knack-0.8.2/knack/testsdk/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (118)     9444 2021-05-08 06:50:44.000000 knack-0.8.2/knack/testsdk/base.py
--rw-r--r--   0 vsts      (1001) docker     (118)    17792 2021-05-08 06:50:44.000000 knack-0.8.2/knack/commands.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2059 2021-05-08 06:50:44.000000 knack-0.8.2/knack/completion.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6075 2021-05-08 06:50:44.000000 knack-0.8.2/knack/util.py
--rw-r--r--   0 vsts      (1001) docker     (118)    22248 2021-05-08 06:50:44.000000 knack-0.8.2/knack/arguments.py
--rw-r--r--   0 vsts      (1001) docker     (118)    10331 2021-05-08 06:50:44.000000 knack-0.8.2/knack/output.py
--rw-r--r--   0 vsts      (1001) docker     (118)     4241 2021-05-08 06:50:44.000000 knack-0.8.2/knack/prompting.py
--rw-r--r--   0 vsts      (1001) docker     (118)    28365 2021-05-08 06:50:44.000000 knack-0.8.2/knack/help.py
--rw-r--r--   0 vsts      (1001) docker     (118)     5625 2021-05-08 06:50:44.000000 knack-0.8.2/HISTORY.rst
-drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2021-05-08 06:50:47.000000 knack-0.8.2/tests/
--rw-r--r--   0 vsts      (1001) docker     (118)     2964 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_command_with_configured_defaults.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16148 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_prompting.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7825 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_experimental.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7605 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_log.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16072 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_help.py
--rw-r--r--   0 vsts      (1001) docker     (118)    16204 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_config.py
--rw-r--r--   0 vsts      (1001) docker     (118)      345 2021-05-08 06:50:44.000000 knack-0.8.2/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (118)    20185 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (118)    11195 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_preview.py
--rw-r--r--   0 vsts      (1001) docker     (118)    19441 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_command_registration.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2826 2021-05-08 06:50:44.000000 knack-0.8.2/tests/util.py
--rw-r--r--   0 vsts      (1001) docker     (118)     7147 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_parser.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3062 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_query.py
--rw-r--r--   0 vsts      (1001) docker     (118)      171 2021-05-08 06:50:44.000000 knack-0.8.2/tests/README.md
--rw-r--r--   0 vsts      (1001) docker     (118)    11281 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_output.py
--rw-r--r--   0 vsts      (1001) docker     (118)     2853 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_introspection.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3133 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_completion.py
--rw-r--r--   0 vsts      (1001) docker     (118)     6236 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_cli_scenarios.py
--rw-r--r--   0 vsts      (1001) docker     (118)     3679 2021-05-08 06:50:44.000000 knack-0.8.2/tests/test_util.py
--rw-r--r--   0 vsts      (1001) docker     (118)     1161 2021-05-08 06:50:44.000000 knack-0.8.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (118)     4310 2021-05-08 06:50:44.000000 knack-0.8.2/README.rst
--rw-r--r--   0 vsts      (1001) docker     (118)     1517 2021-05-08 06:50:44.000000 knack-0.8.2/setup.py
--rw-r--r--   0 vsts      (1001) docker     (118)       74 2021-05-08 06:50:47.000000 knack-0.8.2/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-11-05 05:18:29.853407 knack-0.9.0/
+-rw-r--r--   0 vsts      (1001) docker     (121)      551 2021-11-05 05:18:23.000000 knack-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     5710 2021-11-05 05:18:23.000000 knack-0.9.0/HISTORY.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     1161 2021-11-05 05:18:23.000000 knack-0.9.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)       56 2021-11-05 05:18:23.000000 knack-0.9.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     5106 2021-11-05 05:18:29.853407 knack-0.9.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     4310 2021-11-05 05:18:23.000000 knack-0.9.0/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-11-05 05:18:29.849407 knack-0.9.0/knack/
+-rw-r--r--   0 vsts      (1001) docker     (121)      602 2021-11-05 05:18:23.000000 knack-0.9.0/knack/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    22248 2021-11-05 05:18:23.000000 knack-0.9.0/knack/arguments.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12365 2021-11-05 05:18:23.000000 knack-0.9.0/knack/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    17784 2021-11-05 05:18:23.000000 knack-0.9.0/knack/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2059 2021-11-05 05:18:23.000000 knack-0.9.0/knack/completion.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11591 2021-11-05 05:18:23.000000 knack-0.9.0/knack/config.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5784 2021-11-05 05:18:23.000000 knack-0.9.0/knack/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1233 2021-11-05 05:18:23.000000 knack-0.9.0/knack/events.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3022 2021-11-05 05:18:23.000000 knack-0.9.0/knack/experimental.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    28347 2021-11-05 05:18:23.000000 knack-0.9.0/knack/help.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      583 2021-11-05 05:18:23.000000 knack-0.9.0/knack/help_files.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4003 2021-11-05 05:18:23.000000 knack-0.9.0/knack/introspection.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10143 2021-11-05 05:18:23.000000 knack-0.9.0/knack/invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9545 2021-11-05 05:18:23.000000 knack-0.9.0/knack/log.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10331 2021-11-05 05:18:23.000000 knack-0.9.0/knack/output.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13573 2021-11-05 05:18:23.000000 knack-0.9.0/knack/parser.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2902 2021-11-05 05:18:23.000000 knack-0.9.0/knack/preview.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4241 2021-11-05 05:18:23.000000 knack-0.9.0/knack/prompting.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2677 2021-11-05 05:18:23.000000 knack-0.9.0/knack/query.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-11-05 05:18:29.853407 knack-0.9.0/knack/testsdk/
+-rw-r--r--   0 vsts      (1001) docker     (121)      847 2021-11-05 05:18:23.000000 knack-0.9.0/knack/testsdk/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9444 2021-11-05 05:18:23.000000 knack-0.9.0/knack/testsdk/base.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4419 2021-11-05 05:18:23.000000 knack-0.9.0/knack/testsdk/checkers.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      463 2021-11-05 05:18:23.000000 knack-0.9.0/knack/testsdk/const.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      798 2021-11-05 05:18:23.000000 knack-0.9.0/knack/testsdk/decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1157 2021-11-05 05:18:23.000000 knack-0.9.0/knack/testsdk/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      854 2021-11-05 05:18:23.000000 knack-0.9.0/knack/testsdk/patches.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3968 2021-11-05 05:18:23.000000 knack-0.9.0/knack/testsdk/recording_processors.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1132 2021-11-05 05:18:23.000000 knack-0.9.0/knack/testsdk/util.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6075 2021-11-05 05:18:23.000000 knack-0.9.0/knack/util.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      699 2021-11-05 05:18:23.000000 knack-0.9.0/knack/validators.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-11-05 05:18:29.849407 knack-0.9.0/knack.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5106 2021-11-05 05:18:29.000000 knack-0.9.0/knack.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     1307 2021-11-05 05:18:29.000000 knack-0.9.0/knack.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-11-05 05:18:29.000000 knack-0.9.0/knack.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-11-05 05:18:29.000000 knack-0.9.0/knack.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (121)       46 2021-11-05 05:18:29.000000 knack-0.9.0/knack.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        6 2021-11-05 05:18:29.000000 knack-0.9.0/knack.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       74 2021-11-05 05:18:29.853407 knack-0.9.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)     1627 2021-11-05 05:18:23.000000 knack-0.9.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-11-05 05:18:29.853407 knack-0.9.0/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)      171 2021-11-05 05:18:23.000000 knack-0.9.0/tests/README.md
+-rw-r--r--   0 vsts      (1001) docker     (121)      345 2021-11-05 05:18:23.000000 knack-0.9.0/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6179 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_cli_scenarios.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    19441 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_command_registration.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2919 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_command_with_configured_defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3088 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_completion.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16159 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_config.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    20137 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7779 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_experimental.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16086 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_help.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2853 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_introspection.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7560 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_log.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11295 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_output.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7147 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_parser.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11149 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_preview.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16103 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_prompting.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3076 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_query.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     3679 2021-11-05 05:18:23.000000 knack-0.9.0/tests/test_util.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2781 2021-11-05 05:18:23.000000 knack-0.9.0/tests/util.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `knack-0.8.2/PKG-INFO` & `knack-0.9.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,170 +1,174 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: knack
-Version: 0.8.2
+Version: 0.9.0
 Summary: A Command-Line Interface framework
 Home-page: https://github.com/microsoft/knack
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
-Description: Knack
-        =====
-        
-        .. image:: https://img.shields.io/pypi/v/knack.svg
-            :target: https://pypi.python.org/pypi/knack
-        
-        .. image:: https://img.shields.io/pypi/pyversions/knack.svg
-            :target: https://pypi.python.org/pypi/knack
-        
-        .. image:: https://dev.azure.com/azure-sdk/public/_apis/build/status/cli/microsoft.knack?branchName=dev
-            :target: https://dev.azure.com/azure-sdk/public/_build/latest?definitionId=1643&branchName=dev
-        
-        
-        ------------
-        
-        
-        ::
-        
-            _                     _
-           | | ___ __   __ _  ___| | __
-           | |/ / '_ \ / _` |/ __| |/ /
-           |   <| | | | (_| | (__|   <
-           |_|\_\_| |_|\__,_|\___|_|\_\
-        
-        
-        **A Command-Line Interface framework**
-        
-        Installation is easy via pip:
-        
-        .. code-block:: bash
-        
-            pip install knack
-        
-        Knack can be installed as a non-privileged user to your home directory by adding "--user" as below:
-        
-        .. code-block:: bash
-        
-            pip install knack --user
-        
-        ------------
-        
-        .. note:: The project is in `initial development phase <https://semver.org/#how-should-i-deal-with-revisions-in-the-0yz-initial-development-phase>`__. We recommend pinning to at least a specific minor version when marking **knack** as a dependency in your project.
-        
-        ------------
-        
-        
-        Usage
-        =====
-        
-        
-        .. code-block:: python
-        
-            import sys
-            from collections import OrderedDict
-        
-            from knack import CLI, ArgumentsContext, CLICommandsLoader
-            from knack.commands import CommandGroup
-        
-        
-            def abc_str(length=3):
-                import string
-                return string.ascii_lowercase[:length]
-        
-        
-            class MyCommandsLoader(CLICommandsLoader):
-                def load_command_table(self, args):
-                    with CommandGroup(self, 'abc', '__main__#{}') as g:
-                        g.command('str', 'abc_str')
-                    return OrderedDict(self.command_table)
-        
-                def load_arguments(self, command):
-                    with ArgumentsContext(self, 'abc str') as ac:
-                        ac.argument('length', type=int)
-                    super(MyCommandsLoader, self).load_arguments(command)
-        
-        
-            mycli = CLI(cli_name='mycli', commands_loader_cls=MyCommandsLoader)
-            exit_code = mycli.invoke(sys.argv[1:])
-            sys.exit(exit_code)
-        
-            # $ python mycli.py abc str
-            # "abc"
-        
-            # $ python mycli.py abc str --length 5
-            # "abcde"
-        
-            # $ python mycli.py abc str --length 100
-            # "abcdefghijklmnopqrstuvwxyz"
-        
-        
-        More samples and snippets are available at `examples <https://github.com/Microsoft/knack/tree/dev/examples>`__.
-        
-        
-        Documentation
-        =============
-        
-        Documentation is available at `docs <https://github.com/Microsoft/knack/tree/dev/docs>`__.
-        
-        Developer Setup
-        ===============
-        
-        In a virtual environment, install the `requirements.txt` file.
-        
-        .. code-block:: bash
-        
-            pip install -r requirements.txt
-            pip install -e .
-        
-        Run Automation
-        ==============
-        
-        This project supports running automation using `tox <https://tox.readthedocs.io/en/latest/>`__.
-        
-        .. code-block:: bash
-        
-            pip install tox
-            tox
-        
-        
-        Real-world uses
-        ===============
-        
-        - `Azure CLI <https://github.com/Azure/azure-cli/>`__: The Azure CLI 2.0 is Azure's new command line experience for managing Azure resources.
-        - `VSTS CLI <https://github.com/Microsoft/vsts-cli>`__: A command-line interface for Visual Studio Team Services (VSTS) and Team Foundation Server (TFS). With the VSTS CLI, you can manage and work with resources including pull requests, work items, builds, and more.
-        - `Service Fabric CLI <https://github.com/Azure/service-fabric-cli>`__: A command-line interface for interacting with Azure Service Fabric clusters and their related entities.
-        
-        Do you use knack in your CLI as well? Open a pull request to include it here. We would love to have it in our list.
-        
-        
-        Release History
-        ===============
-        
-        See `GitHub Releases <https://github.com/Microsoft/knack/releases>`__.
-        
-        
-        Contribute Code
-        ===============
-        
-        This project has adopted the `Microsoft Open Source Code of Conduct <https://opensource.microsoft.com/codeofconduct/>`__.
-        
-        For more information see the `Code of Conduct FAQ <https://opensource.microsoft.com/codeofconduct/faq/>`__ or contact `opencode@microsoft.com <mailto:opencode@microsoft.com>`__ with any additional questions or comments.
-        
-        If you would like to become an active contributor to this project, please
-        follow the instructions provided in `Contribution License Agreement <https://cla.microsoft.com/>`__.
-        
-        
-        License
-        =======
-        
-        Knack is licensed under `MIT <LICENSE>`__.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE
+
+Knack
+=====
+
+.. image:: https://img.shields.io/pypi/v/knack.svg
+    :target: https://pypi.python.org/pypi/knack
+
+.. image:: https://img.shields.io/pypi/pyversions/knack.svg
+    :target: https://pypi.python.org/pypi/knack
+
+.. image:: https://dev.azure.com/azure-sdk/public/_apis/build/status/cli/microsoft.knack?branchName=dev
+    :target: https://dev.azure.com/azure-sdk/public/_build/latest?definitionId=1643&branchName=dev
+
+
+------------
+
+
+::
+
+    _                     _
+   | | ___ __   __ _  ___| | __
+   | |/ / '_ \ / _` |/ __| |/ /
+   |   <| | | | (_| | (__|   <
+   |_|\_\_| |_|\__,_|\___|_|\_\
+
+
+**A Command-Line Interface framework**
+
+Installation is easy via pip:
+
+.. code-block:: bash
+
+    pip install knack
+
+Knack can be installed as a non-privileged user to your home directory by adding "--user" as below:
+
+.. code-block:: bash
+
+    pip install knack --user
+
+------------
+
+.. note:: The project is in `initial development phase <https://semver.org/#how-should-i-deal-with-revisions-in-the-0yz-initial-development-phase>`__. We recommend pinning to at least a specific minor version when marking **knack** as a dependency in your project.
+
+------------
+
+
+Usage
+=====
+
+
+.. code-block:: python
+
+    import sys
+    from collections import OrderedDict
+
+    from knack import CLI, ArgumentsContext, CLICommandsLoader
+    from knack.commands import CommandGroup
+
+
+    def abc_str(length=3):
+        import string
+        return string.ascii_lowercase[:length]
+
+
+    class MyCommandsLoader(CLICommandsLoader):
+        def load_command_table(self, args):
+            with CommandGroup(self, 'abc', '__main__#{}') as g:
+                g.command('str', 'abc_str')
+            return OrderedDict(self.command_table)
+
+        def load_arguments(self, command):
+            with ArgumentsContext(self, 'abc str') as ac:
+                ac.argument('length', type=int)
+            super(MyCommandsLoader, self).load_arguments(command)
+
+
+    mycli = CLI(cli_name='mycli', commands_loader_cls=MyCommandsLoader)
+    exit_code = mycli.invoke(sys.argv[1:])
+    sys.exit(exit_code)
+
+    # $ python mycli.py abc str
+    # "abc"
+
+    # $ python mycli.py abc str --length 5
+    # "abcde"
+
+    # $ python mycli.py abc str --length 100
+    # "abcdefghijklmnopqrstuvwxyz"
+
+
+More samples and snippets are available at `examples <https://github.com/Microsoft/knack/tree/dev/examples>`__.
+
+
+Documentation
+=============
+
+Documentation is available at `docs <https://github.com/Microsoft/knack/tree/dev/docs>`__.
+
+Developer Setup
+===============
+
+In a virtual environment, install the `requirements.txt` file.
+
+.. code-block:: bash
+
+    pip install -r requirements.txt
+    pip install -e .
+
+Run Automation
+==============
+
+This project supports running automation using `tox <https://tox.readthedocs.io/en/latest/>`__.
+
+.. code-block:: bash
+
+    pip install tox
+    tox
+
+
+Real-world uses
+===============
+
+- `Azure CLI <https://github.com/Azure/azure-cli/>`__: The Azure CLI 2.0 is Azure's new command line experience for managing Azure resources.
+- `VSTS CLI <https://github.com/Microsoft/vsts-cli>`__: A command-line interface for Visual Studio Team Services (VSTS) and Team Foundation Server (TFS). With the VSTS CLI, you can manage and work with resources including pull requests, work items, builds, and more.
+- `Service Fabric CLI <https://github.com/Azure/service-fabric-cli>`__: A command-line interface for interacting with Azure Service Fabric clusters and their related entities.
+
+Do you use knack in your CLI as well? Open a pull request to include it here. We would love to have it in our list.
+
+
+Release History
+===============
+
+See `GitHub Releases <https://github.com/Microsoft/knack/releases>`__.
+
+
+Contribute Code
+===============
+
+This project has adopted the `Microsoft Open Source Code of Conduct <https://opensource.microsoft.com/codeofconduct/>`__.
+
+For more information see the `Code of Conduct FAQ <https://opensource.microsoft.com/codeofconduct/faq/>`__ or contact `opencode@microsoft.com <mailto:opencode@microsoft.com>`__ with any additional questions or comments.
+
+If you would like to become an active contributor to this project, please
+follow the instructions provided in `Contribution License Agreement <https://cla.microsoft.com/>`__.
+
+
+License
+=======
+
+Knack is licensed under `MIT <LICENSE>`__.
+
+
```

### Comparing `knack-0.8.2/knack.egg-info/PKG-INFO` & `knack-0.9.0/knack.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,170 +1,174 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: knack
-Version: 0.8.2
+Version: 0.9.0
 Summary: A Command-Line Interface framework
 Home-page: https://github.com/microsoft/knack
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
-Description: Knack
-        =====
-        
-        .. image:: https://img.shields.io/pypi/v/knack.svg
-            :target: https://pypi.python.org/pypi/knack
-        
-        .. image:: https://img.shields.io/pypi/pyversions/knack.svg
-            :target: https://pypi.python.org/pypi/knack
-        
-        .. image:: https://dev.azure.com/azure-sdk/public/_apis/build/status/cli/microsoft.knack?branchName=dev
-            :target: https://dev.azure.com/azure-sdk/public/_build/latest?definitionId=1643&branchName=dev
-        
-        
-        ------------
-        
-        
-        ::
-        
-            _                     _
-           | | ___ __   __ _  ___| | __
-           | |/ / '_ \ / _` |/ __| |/ /
-           |   <| | | | (_| | (__|   <
-           |_|\_\_| |_|\__,_|\___|_|\_\
-        
-        
-        **A Command-Line Interface framework**
-        
-        Installation is easy via pip:
-        
-        .. code-block:: bash
-        
-            pip install knack
-        
-        Knack can be installed as a non-privileged user to your home directory by adding "--user" as below:
-        
-        .. code-block:: bash
-        
-            pip install knack --user
-        
-        ------------
-        
-        .. note:: The project is in `initial development phase <https://semver.org/#how-should-i-deal-with-revisions-in-the-0yz-initial-development-phase>`__. We recommend pinning to at least a specific minor version when marking **knack** as a dependency in your project.
-        
-        ------------
-        
-        
-        Usage
-        =====
-        
-        
-        .. code-block:: python
-        
-            import sys
-            from collections import OrderedDict
-        
-            from knack import CLI, ArgumentsContext, CLICommandsLoader
-            from knack.commands import CommandGroup
-        
-        
-            def abc_str(length=3):
-                import string
-                return string.ascii_lowercase[:length]
-        
-        
-            class MyCommandsLoader(CLICommandsLoader):
-                def load_command_table(self, args):
-                    with CommandGroup(self, 'abc', '__main__#{}') as g:
-                        g.command('str', 'abc_str')
-                    return OrderedDict(self.command_table)
-        
-                def load_arguments(self, command):
-                    with ArgumentsContext(self, 'abc str') as ac:
-                        ac.argument('length', type=int)
-                    super(MyCommandsLoader, self).load_arguments(command)
-        
-        
-            mycli = CLI(cli_name='mycli', commands_loader_cls=MyCommandsLoader)
-            exit_code = mycli.invoke(sys.argv[1:])
-            sys.exit(exit_code)
-        
-            # $ python mycli.py abc str
-            # "abc"
-        
-            # $ python mycli.py abc str --length 5
-            # "abcde"
-        
-            # $ python mycli.py abc str --length 100
-            # "abcdefghijklmnopqrstuvwxyz"
-        
-        
-        More samples and snippets are available at `examples <https://github.com/Microsoft/knack/tree/dev/examples>`__.
-        
-        
-        Documentation
-        =============
-        
-        Documentation is available at `docs <https://github.com/Microsoft/knack/tree/dev/docs>`__.
-        
-        Developer Setup
-        ===============
-        
-        In a virtual environment, install the `requirements.txt` file.
-        
-        .. code-block:: bash
-        
-            pip install -r requirements.txt
-            pip install -e .
-        
-        Run Automation
-        ==============
-        
-        This project supports running automation using `tox <https://tox.readthedocs.io/en/latest/>`__.
-        
-        .. code-block:: bash
-        
-            pip install tox
-            tox
-        
-        
-        Real-world uses
-        ===============
-        
-        - `Azure CLI <https://github.com/Azure/azure-cli/>`__: The Azure CLI 2.0 is Azure's new command line experience for managing Azure resources.
-        - `VSTS CLI <https://github.com/Microsoft/vsts-cli>`__: A command-line interface for Visual Studio Team Services (VSTS) and Team Foundation Server (TFS). With the VSTS CLI, you can manage and work with resources including pull requests, work items, builds, and more.
-        - `Service Fabric CLI <https://github.com/Azure/service-fabric-cli>`__: A command-line interface for interacting with Azure Service Fabric clusters and their related entities.
-        
-        Do you use knack in your CLI as well? Open a pull request to include it here. We would love to have it in our list.
-        
-        
-        Release History
-        ===============
-        
-        See `GitHub Releases <https://github.com/Microsoft/knack/releases>`__.
-        
-        
-        Contribute Code
-        ===============
-        
-        This project has adopted the `Microsoft Open Source Code of Conduct <https://opensource.microsoft.com/codeofconduct/>`__.
-        
-        For more information see the `Code of Conduct FAQ <https://opensource.microsoft.com/codeofconduct/faq/>`__ or contact `opencode@microsoft.com <mailto:opencode@microsoft.com>`__ with any additional questions or comments.
-        
-        If you would like to become an active contributor to this project, please
-        follow the instructions provided in `Contribution License Agreement <https://cla.microsoft.com/>`__.
-        
-        
-        License
-        =======
-        
-        Knack is licensed under `MIT <LICENSE>`__.
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
+License-File: LICENSE
+
+Knack
+=====
+
+.. image:: https://img.shields.io/pypi/v/knack.svg
+    :target: https://pypi.python.org/pypi/knack
+
+.. image:: https://img.shields.io/pypi/pyversions/knack.svg
+    :target: https://pypi.python.org/pypi/knack
+
+.. image:: https://dev.azure.com/azure-sdk/public/_apis/build/status/cli/microsoft.knack?branchName=dev
+    :target: https://dev.azure.com/azure-sdk/public/_build/latest?definitionId=1643&branchName=dev
+
+
+------------
+
+
+::
+
+    _                     _
+   | | ___ __   __ _  ___| | __
+   | |/ / '_ \ / _` |/ __| |/ /
+   |   <| | | | (_| | (__|   <
+   |_|\_\_| |_|\__,_|\___|_|\_\
+
+
+**A Command-Line Interface framework**
+
+Installation is easy via pip:
+
+.. code-block:: bash
+
+    pip install knack
+
+Knack can be installed as a non-privileged user to your home directory by adding "--user" as below:
+
+.. code-block:: bash
+
+    pip install knack --user
+
+------------
+
+.. note:: The project is in `initial development phase <https://semver.org/#how-should-i-deal-with-revisions-in-the-0yz-initial-development-phase>`__. We recommend pinning to at least a specific minor version when marking **knack** as a dependency in your project.
+
+------------
+
+
+Usage
+=====
+
+
+.. code-block:: python
+
+    import sys
+    from collections import OrderedDict
+
+    from knack import CLI, ArgumentsContext, CLICommandsLoader
+    from knack.commands import CommandGroup
+
+
+    def abc_str(length=3):
+        import string
+        return string.ascii_lowercase[:length]
+
+
+    class MyCommandsLoader(CLICommandsLoader):
+        def load_command_table(self, args):
+            with CommandGroup(self, 'abc', '__main__#{}') as g:
+                g.command('str', 'abc_str')
+            return OrderedDict(self.command_table)
+
+        def load_arguments(self, command):
+            with ArgumentsContext(self, 'abc str') as ac:
+                ac.argument('length', type=int)
+            super(MyCommandsLoader, self).load_arguments(command)
+
+
+    mycli = CLI(cli_name='mycli', commands_loader_cls=MyCommandsLoader)
+    exit_code = mycli.invoke(sys.argv[1:])
+    sys.exit(exit_code)
+
+    # $ python mycli.py abc str
+    # "abc"
+
+    # $ python mycli.py abc str --length 5
+    # "abcde"
+
+    # $ python mycli.py abc str --length 100
+    # "abcdefghijklmnopqrstuvwxyz"
+
+
+More samples and snippets are available at `examples <https://github.com/Microsoft/knack/tree/dev/examples>`__.
+
+
+Documentation
+=============
+
+Documentation is available at `docs <https://github.com/Microsoft/knack/tree/dev/docs>`__.
+
+Developer Setup
+===============
+
+In a virtual environment, install the `requirements.txt` file.
+
+.. code-block:: bash
+
+    pip install -r requirements.txt
+    pip install -e .
+
+Run Automation
+==============
+
+This project supports running automation using `tox <https://tox.readthedocs.io/en/latest/>`__.
+
+.. code-block:: bash
+
+    pip install tox
+    tox
+
+
+Real-world uses
+===============
+
+- `Azure CLI <https://github.com/Azure/azure-cli/>`__: The Azure CLI 2.0 is Azure's new command line experience for managing Azure resources.
+- `VSTS CLI <https://github.com/Microsoft/vsts-cli>`__: A command-line interface for Visual Studio Team Services (VSTS) and Team Foundation Server (TFS). With the VSTS CLI, you can manage and work with resources including pull requests, work items, builds, and more.
+- `Service Fabric CLI <https://github.com/Azure/service-fabric-cli>`__: A command-line interface for interacting with Azure Service Fabric clusters and their related entities.
+
+Do you use knack in your CLI as well? Open a pull request to include it here. We would love to have it in our list.
+
+
+Release History
+===============
+
+See `GitHub Releases <https://github.com/Microsoft/knack/releases>`__.
+
+
+Contribute Code
+===============
+
+This project has adopted the `Microsoft Open Source Code of Conduct <https://opensource.microsoft.com/codeofconduct/>`__.
+
+For more information see the `Code of Conduct FAQ <https://opensource.microsoft.com/codeofconduct/faq/>`__ or contact `opencode@microsoft.com <mailto:opencode@microsoft.com>`__ with any additional questions or comments.
+
+If you would like to become an active contributor to this project, please
+follow the instructions provided in `Contribution License Agreement <https://cla.microsoft.com/>`__.
+
+
+License
+=======
+
+Knack is licensed under `MIT <LICENSE>`__.
+
+
```

### Comparing `knack-0.8.2/knack.egg-info/SOURCES.txt` & `knack-0.9.0/knack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/CONTRIBUTING.rst` & `knack-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/parser.py` & `knack-0.9.0/knack/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,16 @@
         :param args: Arguments passed from command line
         :type args: list
         """
         for arg, _ in enumerate(args):
             if args[arg].startswith('@'):
                 try:
                     logger.debug('Attempting to read file %s', args[arg][1:])
-                    with open(args[arg][1:], 'r') as f:
+                    # Use the default system encoding: https://docs.python.org/3/library/functions.html#open
+                    with open(args[arg][1:], 'r') as f:  # pylint: disable=unspecified-encoding
                         content = f.read()
                     args[arg] = content
                 except IOError:
                     # Leave arg unmodified
                     logger.debug('File Error: Failed to open %s, assume not a file', args[arg][1:])
         return args
```

### Comparing `knack-0.8.2/knack/events.py` & `knack-0.9.0/knack/events.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/help_files.py` & `knack-0.9.0/knack/help_files.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/config.py` & `knack-0.9.0/knack/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import stat
 import configparser
 
 from .util import ensure_dir
 
 _UNSET = object()
 
+CONFIG_FILE_ENCODING = 'utf-8'
+
 
 def get_config_parser():
     return configparser.ConfigParser()  # keep this for backward compatibility
 
 
 class CLIConfig(object):
     _BOOLEAN_STATES = {'1': True, 'yes': True, 'true': True, 'on': True,
@@ -186,15 +188,15 @@
         see https://docs.python.org/3/library/configparser.html#supported-ini-file-structure
         """
         self.config_dir = config_dir
         self.config_path = config_path
         self.config_comment = config_comment
         self.config_parser = configparser.ConfigParser()
         if os.path.exists(config_path):
-            self.config_parser.read(config_path)
+            self.config_parser.read(config_path, encoding=CONFIG_FILE_ENCODING)
 
     def items(self, section):
         return self.config_parser.items(section) if self.config_parser else []
 
     def sections(self):
         return self.config_parser.sections() if self.config_parser else []
 
@@ -216,15 +218,15 @@
         val = str(self.get(section, option))
         if val.lower() not in _ConfigFile._BOOLEAN_STATES:
             raise ValueError('Not a boolean: {}'.format(val))
         return _ConfigFile._BOOLEAN_STATES[val.lower()]
 
     def set(self, config):
         ensure_dir(self.config_dir)
-        with open(self.config_path, 'w') as configfile:
+        with open(self.config_path, 'w', encoding=CONFIG_FILE_ENCODING) as configfile:
             if self.config_comment:
                 configfile.write(self.config_comment + '\n')
             config.write(configfile)
         os.chmod(self.config_path, stat.S_IRUSR | stat.S_IWUSR)
         self.config_parser.read(self.config_path)
 
     def set_value(self, section, option, value):
```

### Comparing `knack-0.8.2/knack/query.py` & `knack-0.9.0/knack/query.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/introspection.py` & `knack-0.9.0/knack/introspection.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/log.py` & `knack-0.9.0/knack/log.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/deprecation.py` & `knack-0.9.0/knack/deprecation.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/preview.py` & `knack-0.9.0/knack/preview.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/__init__.py` & `knack-0.9.0/knack/__init__.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/cli.py` & `knack-0.9.0/knack/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         # As logging is initialized in `invoke`, call `logger.debug` or `logger.info` here won't work.
         self.init_debug_log = []
         self.init_info_log = []
 
         self.only_show_errors = self.config.getboolean('core', 'only_show_errors', fallback=False)
         self.enable_color = self._should_enable_color()
         # Init colorama only in Windows legacy terminal
-        self._should_init_colorama = self.enable_color and os.name == 'nt' and not is_modern_terminal()
+        self._should_init_colorama = self.enable_color and sys.platform == 'win32' and not is_modern_terminal()
 
     @staticmethod
     def _should_show_version(args):
         return args and (args[0] == '--version' or args[0] == '-v')
 
     def get_cli_version(self):  # pylint: disable=no-self-use
         """ Get the CLI Version. Override this to define how to get the CLI version
```

### Comparing `knack-0.8.2/knack/validators.py` & `knack-0.9.0/knack/validators.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/invocation.py` & `knack-0.9.0/knack/invocation.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/experimental.py` & `knack-0.9.0/knack/experimental.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/testsdk/recording_processors.py` & `knack-0.9.0/knack/testsdk/recording_processors.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/testsdk/__init__.py` & `knack-0.9.0/knack/testsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/testsdk/decorators.py` & `knack-0.9.0/knack/testsdk/decorators.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/testsdk/patches.py` & `knack-0.9.0/knack/testsdk/patches.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 import unittest
-try:
-    import mock
-except ImportError:
-    from unittest import mock
+from unittest import mock
 from .exceptions import CliTestError
 
 
 def patch_time_sleep_api(unit_test):
     def _time_sleep_skip(*_):
         return
     _mock_in_unit_test(unit_test, 'time.sleep', _time_sleep_skip)
```

### Comparing `knack-0.8.2/knack/testsdk/checkers.py` & `knack-0.9.0/knack/testsdk/checkers.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/testsdk/util.py` & `knack-0.9.0/knack/testsdk/util.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/testsdk/exceptions.py` & `knack-0.9.0/knack/testsdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/testsdk/base.py` & `knack-0.9.0/knack/testsdk/base.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/commands.py` & `knack-0.9.0/knack/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,17 +176,17 @@
         if cli_ctx is not None and not isinstance(cli_ctx, CLI):
             raise CtxTypeError(cli_ctx)
         self.cli_ctx = cli_ctx
         self.command_cls = command_cls
         self.skip_applicability = False
         self.excluded_command_handler_args = excluded_command_handler_args
         # A command table is a dictionary of name -> CLICommand instances
-        self.command_table = dict()
+        self.command_table = {}
         # A command group table is a dictionary of names -> CommandGroup instances
-        self.command_group_table = dict()
+        self.command_group_table = {}
         # An argument registry stores all arguments for commands
         self.argument_registry = ArgumentRegistry()
         self.extra_argument_registry = defaultdict(lambda: {})
 
     def _populate_command_group_table_with_subgroups(self, name):
         if not name:
             return
```

### Comparing `knack-0.8.2/knack/completion.py` & `knack-0.9.0/knack/completion.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/util.py` & `knack-0.9.0/knack/util.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/arguments.py` & `knack-0.9.0/knack/arguments.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/output.py` & `knack-0.9.0/knack/output.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/prompting.py` & `knack-0.9.0/knack/prompting.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/knack/help.py` & `knack-0.9.0/knack/help.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,15 +358,15 @@
         self.deprecate_info = deprecate_info
         self.preview_info = preview_info
         self.experimental_info = experimental_info
         self.default_value_source = default_value_source
 
     def update_from_data(self, data):
         if self.name != data.get('name'):
-            raise HelpAuthoringException(u"mismatched name {} vs. {}"
+            raise HelpAuthoringException("mismatched name {} vs. {}"
                                          .format(self.name,
                                                  data.get('name')))
 
         if data.get('type'):
             self.type = data.get('type')
 
         if data.get('short-summary'):
@@ -390,15 +390,15 @@
 
     def _print_header(self, cli_name, help_file):
         indent = 0
         _print_indent('')
         _print_indent('Command' if help_file.type == 'command' else 'Group', indent)
 
         indent += 1
-        LINE_FORMAT = u'{cli}{name}{separator}{summary}'
+        LINE_FORMAT = '{cli}{name}{separator}{summary}'
         line = LINE_FORMAT.format(
             cli=cli_name,
             name=' ' + help_file.command if help_file.command else '',
             separator=FIRST_LINE_PREFIX if help_file.short_summary else '',
             summary=help_file.short_summary if help_file.short_summary else ''
         )
         _print_indent(line, indent, width=self.textwrap_width)
@@ -417,15 +417,15 @@
 
         indent += 1
         long_sum = _build_long_summary(help_file)
         _print_indent(long_sum, indent, width=self.textwrap_width)
 
     def _print_groups(self, help_file):
 
-        LINE_FORMAT = u'{name}{padding}{tags}{separator}{summary}'
+        LINE_FORMAT = '{name}{padding}{tags}{separator}{summary}'
         indent = 1
 
         self.max_line_len = 0
 
         def _build_tags_string(item):
 
             preview_info = getattr(item, 'preview_info', None)
@@ -492,50 +492,50 @@
 
         if commands:
             _print_indent('Commands:')
             _print_items(command_layouts)
 
     @staticmethod
     def _get_choices_defaults_sources_str(p):
-        choice_str = u'  Allowed values: {}.'.format(', '.join(sorted([str(x) for x in p.choices]))) \
+        choice_str = '  Allowed values: {}.'.format(', '.join(sorted([str(x) for x in p.choices]))) \
             if p.choices else ''
-        default_str = u'  Default: {}.'.format(p.default) \
+        default_str = '  Default: {}.'.format(p.default) \
             if p.default and p.default != argparse.SUPPRESS else ''
-        value_sources_str = u'  Values from: {}.'.format(', '.join(p.value_sources)) \
+        value_sources_str = '  Values from: {}.'.format(', '.join(p.value_sources)) \
             if p.value_sources else ''
-        return u'{}{}{}'.format(choice_str, default_str, value_sources_str)
+        return '{}{}{}'.format(choice_str, default_str, value_sources_str)
 
     @staticmethod
     def print_description_list(help_files):
         indent = 1
         max_length = max(len(f.name) for f in help_files) if help_files else 0
         for help_file in sorted(help_files, key=lambda h: h.name):
             column_indent = max_length - len(help_file.name)
-            _print_indent(u'{}{}{}'.format(help_file.name,
-                                           ' ' * column_indent,
-                                           FIRST_LINE_PREFIX + help_file.short_summary
-                                           if help_file.short_summary
-                                           else ''),
+            _print_indent('{}{}{}'.format(help_file.name,
+                                          ' ' * column_indent,
+                                          FIRST_LINE_PREFIX + help_file.short_summary
+                                          if help_file.short_summary
+                                          else ''),
                           indent,
                           _get_hanging_indent(max_length, indent))
 
     @staticmethod
     def _print_examples(help_file):
         indent = 0
         _print_indent('Examples', indent)
         for e in help_file.examples:
             indent = 1
-            _print_indent(u'{0}'.format(e.name), indent)
+            _print_indent('{0}'.format(e.name), indent)
             indent = 2
-            _print_indent(u'{0}'.format(e.text), indent)
+            _print_indent('{0}'.format(e.text), indent)
             print('')
 
     def _print_arguments(self, help_file):  # pylint: disable=too-many-statements
 
-        LINE_FORMAT = u'{name}{padding}{tags}{separator}{short_summary}'
+        LINE_FORMAT = '{name}{padding}{tags}{separator}{short_summary}'
         indent = 1
         self.max_line_len = 0
 
         if not help_file.parameters:
             _print_indent('None', indent)
             _print_indent('')
             return None
@@ -640,17 +640,17 @@
             if experimental_info:
                 lines.append(str(item.experimental_info.message))
             return ' '.join(lines)
 
         group_registry = ArgumentGroupRegistry([p.group_name for p in help_file.parameters if p.group_name])
 
         def _get_parameter_key(parameter):
-            return u'{}{}{}'.format(group_registry.get_group_priority(parameter.group_name),
-                                    str(not parameter.required),
-                                    parameter.name)
+            return '{}{}{}'.format(group_registry.get_group_priority(parameter.group_name),
+                                   str(not parameter.required),
+                                   parameter.name)
 
         parameter_layouts = _layout_items(help_file.parameters)
         _print_items(parameter_layouts)
 
         return indent
 
     def _print_detailed_help(self, cli_name, help_file):
```

### Comparing `knack-0.8.2/HISTORY.rst` & `knack-0.9.0/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. :changelog:
 
 Release History
 ===============
 
+0.9.0
++++++
+
+* Support Python 3.10 (#250)
+* Only install colorama on Windows (#249)
+
 0.8.2
 +++++
 
 * Always use UTF-8 for log file encoding (#247)
 
 0.8.1
 +++++
```

### Comparing `knack-0.8.2/tests/test_command_with_configured_defaults.py` & `knack-0.9.0/tests/test_command_with_configured_defaults.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 import os
 import logging
 import sys
 import unittest
-try:
-    import mock
-except ImportError:
-    from unittest import mock
+from unittest import mock
 
 from knack.arguments import ArgumentsContext
 from knack.commands import CLICommandsLoader, CommandGroup
 from tests.util import DummyCLI, redirect_io
 
 
 # a dummy callback for arg-parse
```

### Comparing `knack-0.8.2/tests/test_prompting.py` & `knack-0.9.0/tests/test_prompting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 import sys
 import unittest
-try:
-    import mock
-except ImportError:
-    from unittest import mock
+from unittest import mock
 from io import StringIO
 
 from knack.prompting import (verify_is_a_tty, NoTTYException, _INVALID_PASSWORD_MSG, prompt,
                              prompt_int, prompt_pass, prompt_y_n, prompt_t_f, prompt_choice_list)
 
 
 @unittest.skipIf(sys.version_info[0] == 2, "Can't modify isatty in Python 2 as it's read-only")
```

### Comparing `knack-0.8.2/tests/test_experimental.py` & `knack-0.9.0/tests/test_experimental.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 import unittest
-try:
-    import mock
-except ImportError:
-    from unittest import mock
+from unittest import mock
 
 import sys
 import argparse
 
 from knack.arguments import ArgumentsContext
 from knack.commands import CLICommandsLoader, CommandGroup
 
@@ -68,15 +65,15 @@
 
     @redirect_io
     def test_experimental_command_group_help(self):
         """ Ensure experimental commands appear correctly in group help view. """
         with self.assertRaises(SystemExit):
             self.cli_ctx.invoke('-h'.split())
         actual = self.io.getvalue()
-        expected = u"""
+        expected = """
 Group
     {}
 
 Subgroups:
     grp1 [Experimental] : A group.
 
 Commands:
```

### Comparing `knack-0.8.2/tests/test_log.py` & `knack-0.9.0/tests/test_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 import unittest
-try:
-    import mock
-except ImportError:
-    from unittest import mock
+from unittest import mock
 import logging
 
 from knack.events import EVENT_PARSER_GLOBAL_CREATE, EVENT_INVOKER_PRE_CMD_TBL_CREATE
 from knack.log import CLILogging, get_logger, CLI_LOGGER_NAME, _CustomStreamHandler
 from knack.util import CLIError
 from tests.util import MockContext
```

### Comparing `knack-0.8.2/tests/test_help.py` & `knack-0.9.0/tests/test_help.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 import sys
 import unittest
+from unittest import mock
 
-import mock
 from knack.arguments import ArgumentsContext
 from knack.commands import CLICommandsLoader, CommandGroup
 from knack.events import EVENT_PARSER_GLOBAL_CREATE
 from knack.help import ArgumentGroupRegistry, HelpObject
 from tests.util import DummyCLI, redirect_io
```

### Comparing `knack-0.8.2/tests/test_config.py` & `knack-0.9.0/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 import os
 import stat
 import unittest
 import shutil
-try:
-    import mock
-except ImportError:
-    from unittest import mock
+from unittest import mock
 import configparser
 
 from knack.config import CLIConfig
 from .util import TEMP_FOLDER_NAME, new_temp_folder
 
 
 def clean_local_temp_folder():
```

### Comparing `knack-0.8.2/tests/test_deprecation.py` & `knack-0.9.0/tests/test_deprecation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 import unittest
-try:
-    import mock
-except ImportError:
-    from unittest import mock
+from unittest import mock
 
 from knack.arguments import ArgumentsContext
 from knack.commands import CLICommandsLoader, CommandGroup
 
 from tests.util import DummyCLI, redirect_io, assert_in_multi_line, disable_color
 
 
@@ -62,15 +59,15 @@
 
     @redirect_io
     def test_deprecate_command_group_help(self):
         """ Ensure deprecated commands appear (or don't appear) correctly in group help view. """
         with self.assertRaises(SystemExit):
             self.cli_ctx.invoke('-h'.split())
         actual = self.io.getvalue()
-        expected = u"""
+        expected = """
 Group
     {}
 
 Subgroups:
     grp1 [Deprecated] : A group.
 
 Commands:
@@ -428,15 +425,15 @@
         self.assertIn(expected, actual)
 
     @redirect_io
     def test_deprecate_options_execute_expired_non_deprecated(self):
         """ Ensure non-expired options can be used without warning. """
         self.cli_ctx.invoke('arg-test --arg1 foo --opt1 bar --opt5 foo'.split())
         actual = self.io.getvalue()
-        self.assertTrue(u'--alt5' not in actual and u'--opt5' not in actual)
+        self.assertTrue('--alt5' not in actual and '--opt5' not in actual)
 
     @redirect_io
     def test_deprecate_options_execute_expiring(self):
         """ Ensure expiring options can be used with warning. """
         self.cli_ctx.invoke('arg-test --arg1 foo --opt1 bar --alt4 bar'.split())
         actual = self.io.getvalue()
         expected = "Option '--alt4' has been deprecated and will be removed in version '1.0.0'. Use '--opt4' instead."
```

### Comparing `knack-0.8.2/tests/test_preview.py` & `knack-0.9.0/tests/test_preview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 import unittest
-try:
-    import mock
-except ImportError:
-    from unittest import mock
+from unittest import mock
 
 import sys
 import argparse
 
 from knack.arguments import ArgumentsContext
 from knack.commands import CLICommandsLoader, CommandGroup
 
@@ -60,15 +57,15 @@
 
     @redirect_io
     def test_preview_command_group_help(self):
         """ Ensure preview commands appear correctly in group help view. """
         with self.assertRaises(SystemExit):
             self.cli_ctx.invoke('-h'.split())
         actual = self.io.getvalue()
-        expected = u"""
+        expected = """
 Group
     {}
 
 Subgroups:
     grp1 [Preview] : A group.
 
 Commands:
```

### Comparing `knack-0.8.2/tests/test_command_registration.py` & `knack-0.9.0/tests/test_command_registration.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/tests/util.py` & `knack-0.9.0/tests/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
-try:
-    import mock
-except ImportError:
-    from unittest import mock
+from unittest import mock
 import logging
 import os
 import re
 import shutil
 import sys
 import tempfile
 from io import StringIO
```

### Comparing `knack-0.8.2/tests/test_parser.py` & `knack-0.9.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/tests/test_query.py` & `knack-0.9.0/tests/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 import unittest
-import mock
+from unittest import mock
 
 from knack.events import EVENT_PARSER_GLOBAL_CREATE
 from knack.query import CLIQuery
 from tests.util import MockContext
 
 
 class TestQueryEventHandling(unittest.TestCase):
```

### Comparing `knack-0.8.2/tests/test_output.py` & `knack-0.9.0/tests/test_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 import unittest
-import mock
+from unittest import mock
 from collections import OrderedDict
 from io import StringIO
 
 from knack.output import OutputProducer, format_json, format_json_color, format_yaml, format_yaml_color, \
     format_table, format_tsv
 from knack.util import CommandResultItem, normalize_newlines
 from tests.util import MockContext
```

### Comparing `knack-0.8.2/tests/test_introspection.py` & `knack-0.9.0/tests/test_introspection.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/tests/test_completion.py` & `knack-0.9.0/tests/test_completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 import os
 import unittest
-try:
-    import mock
-except ImportError:
-    from unittest import mock
+from unittest import mock
 
 from knack.completion import CLICompletion, CaseInsensitiveChoicesCompleter, ARGCOMPLETE_ENV_NAME
 from tests.util import MockContext
 
 
 class TestCompletion(unittest.TestCase):
```

### Comparing `knack-0.8.2/tests/test_cli_scenarios.py` & `knack-0.9.0/tests/test_cli_scenarios.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
 import os
 from collections import OrderedDict
 import unittest
-try:
-    import mock
-except ImportError:
-    from unittest import mock
-import mock
+from unittest import mock
 
 from io import StringIO
 
 from knack import CLI
 from knack.commands import CLICommand, CLICommandsLoader
 from knack.invocation import CommandInvoker
 from tests.util import MockContext, redirect_io
```

### Comparing `knack-0.8.2/tests/test_util.py` & `knack-0.9.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/LICENSE` & `knack-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/README.rst` & `knack-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `knack-0.8.2/setup.py` & `knack-0.9.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 #!/usr/bin/env python
 
 # --------------------------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # --------------------------------------------------------------------------------------------
 
-from codecs import open
-from setuptools import setup, find_packages
+import sys
+from setuptools import setup
 
-VERSION = '0.8.2'
+VERSION = '0.9.0'
 
 DEPENDENCIES = [
     'argcomplete',
-    'colorama',
     'jmespath',
     'pygments',
     'pyyaml',
     'tabulate'
 ]
 
-with open('README.rst', 'r', encoding='utf-8') as f:
+# On Windows, colorama is required for legacy terminals.
+if sys.platform == 'win32':
+    DEPENDENCIES.append('colorama')
+
+with open('README.rst', 'r') as f:
     README = f.read()
 
 setup(
     name='knack',
     version=VERSION,
     description='A Command-Line Interface framework',
     long_description=README,
@@ -38,12 +41,13 @@
         'Intended Audience :: System Administrators',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'License :: OSI Approved :: MIT License',
     ],
     packages=['knack', 'knack.testsdk'],
     install_requires=DEPENDENCIES
 )
```

