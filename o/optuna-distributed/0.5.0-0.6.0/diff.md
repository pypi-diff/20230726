# Comparing `tmp/optuna-distributed-0.5.0.tar.gz` & `tmp/optuna-distributed-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optuna-distributed-0.5.0.tar", last modified: Mon May  1 11:53:50 2023, max compression
+gzip compressed data, was "optuna-distributed-0.6.0.tar", last modified: Wed Jul 26 11:33:13 2023, max compression
```

## Comparing `optuna-distributed-0.5.0.tar` & `optuna-distributed-0.6.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.484776 optuna-distributed-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.480776 optuna-distributed-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.480776 optuna-distributed-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/.github/ISSUE_TEMPLATE/general-question.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.480776 optuna-distributed-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/.github/workflows/format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-01 11:53:50.484776 optuna-distributed-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.480776 optuna-distributed-0.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/examples/disable_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/examples/quadratic_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/examples/simple_pruning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/examples/simple_storages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.480776 optuna-distributed-0.5.0/optuna_distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/eventloop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.484776 optuna-distributed-0.5.0/optuna_distributed/ipc/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/ipc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/ipc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/ipc/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/ipc/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.484776 optuna-distributed-0.5.0/optuna_distributed/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/managers/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/managers/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.484776 optuna-distributed-0.5.0/optuna_distributed/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/completed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/failed.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/pruned.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/setattr.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/shouldprune.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/messages/suggest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/study.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/optuna_distributed/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.484776 optuna-distributed-0.5.0/optuna_distributed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-01 11:53:50.000000 optuna-distributed-0.5.0/optuna_distributed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-01 11:53:50.000000 optuna-distributed-0.5.0/optuna_distributed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 11:53:50.000000 optuna-distributed-0.5.0/optuna_distributed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-01 11:53:50.000000 optuna-distributed-0.5.0/optuna_distributed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 11:53:50.000000 optuna-distributed-0.5.0/optuna_distributed.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 11:53:50.488776 optuna-distributed-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:50.484776 optuna-distributed-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/tests/test_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/tests/test_ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/tests/test_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/tests/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-05-01 11:53:40.000000 optuna-distributed-0.5.0/tests/test_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.113499 optuna-distributed-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.101499 optuna-distributed-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.105499 optuna-distributed-0.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/.github/ISSUE_TEMPLATE/general-question.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.105499 optuna-distributed-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/.github/workflows/format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-26 11:33:13.117499 optuna-distributed-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.109499 optuna-distributed-0.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/examples/disable_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/examples/quadratic_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/examples/simple_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/examples/simple_storages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/examples/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.109499 optuna-distributed-0.6.0/optuna_distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/eventloop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.109499 optuna-distributed-0.6.0/optuna_distributed/ipc/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/ipc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/ipc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/ipc/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/ipc/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.113499 optuna-distributed-0.6.0/optuna_distributed/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/managers/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/managers/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.113499 optuna-distributed-0.6.0/optuna_distributed/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/completed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/failed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/pruned.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/setattr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/shouldprune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/messages/suggest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14733 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/study.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/optuna_distributed/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.109499 optuna-distributed-0.6.0/optuna_distributed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-26 11:33:13.000000 optuna-distributed-0.6.0/optuna_distributed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-26 11:33:13.000000 optuna-distributed-0.6.0/optuna_distributed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:33:13.000000 optuna-distributed-0.6.0/optuna_distributed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-26 11:33:13.000000 optuna-distributed-0.6.0/optuna_distributed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 11:33:13.000000 optuna-distributed-0.6.0/optuna_distributed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-26 11:33:13.117499 optuna-distributed-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:13.113499 optuna-distributed-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/tests/test_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/tests/test_ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/tests/test_managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/tests/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-26 11:33:01.000000 optuna-distributed-0.6.0/tests/test_trial.py
```

### Comparing `optuna-distributed-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `optuna-distributed-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/.github/workflows/format.yaml` & `optuna-distributed-0.6.0/.github/workflows/format.yaml`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/.github/workflows/release.yaml` & `optuna-distributed-0.6.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/.github/workflows/test.yaml` & `optuna-distributed-0.6.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/.gitignore` & `optuna-distributed-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/LICENSE` & `optuna-distributed-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/PKG-INFO` & `optuna-distributed-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optuna-distributed
-Version: 0.5.0
+Version: 0.6.0
 Summary: Distributed hyperparameter optimization made easy
 Author-email: Adrian Zuber <xadrianzetx@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/xadrianzetx/optuna-distributed
 Project-URL: Bug Tracker, https://github.com/xadrianzetx/optuna-distributed/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -85,7 +85,8 @@
 
 But there's more! All of the core Optuna APIs, including [storages, samplers](https://github.com/xadrianzetx/optuna-distributed/blob/main/examples/simple_storages.py) and [pruners](https://github.com/xadrianzetx/optuna-distributed/blob/main/examples/simple_pruning.py) are supported! If you'd like to know how Optuna-distributed works, then check out [this article on Optuna blog](https://medium.com/optuna/running-distributed-hyperparameter-optimization-with-optuna-distributed-17bb2f7d422d).
 
 ## What's missing?
 * Support for callbacks and Optuna integration modules.
 * Study APIs such as [`study.stop`](https://optuna.readthedocs.io/en/stable/reference/generated/optuna.study.Study.html#optuna.study.Study.stop) can't be called from trial at the moment.
 * Local asynchronous optimization on Windows machines. Distributed mode is still available.
+* Support for [`optuna.terminator`](https://optuna.readthedocs.io/en/stable/reference/terminator.html).
```

### Comparing `optuna-distributed-0.5.0/README.md` & `optuna-distributed-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -53,8 +53,9 @@
 ```
 
 But there's more! All of the core Optuna APIs, including [storages, samplers](https://github.com/xadrianzetx/optuna-distributed/blob/main/examples/simple_storages.py) and [pruners](https://github.com/xadrianzetx/optuna-distributed/blob/main/examples/simple_pruning.py) are supported! If you'd like to know how Optuna-distributed works, then check out [this article on Optuna blog](https://medium.com/optuna/running-distributed-hyperparameter-optimization-with-optuna-distributed-17bb2f7d422d).
 
 ## What's missing?
 * Support for callbacks and Optuna integration modules.
 * Study APIs such as [`study.stop`](https://optuna.readthedocs.io/en/stable/reference/generated/optuna.study.Study.html#optuna.study.Study.stop) can't be called from trial at the moment.
-* Local asynchronous optimization on Windows machines. Distributed mode is still available.
+* Local asynchronous optimization on Windows machines. Distributed mode is still available.
+* Support for [`optuna.terminator`](https://optuna.readthedocs.io/en/stable/reference/terminator.html).
```

### Comparing `optuna-distributed-0.5.0/examples/disable_logging.py` & `optuna-distributed-0.6.0/examples/disable_logging.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/examples/quadratic_simple.py` & `optuna-distributed-0.6.0/examples/quadratic_simple.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/examples/simple_pruning.py` & `optuna-distributed-0.6.0/examples/simple_pruning.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/examples/simple_storages.py` & `optuna-distributed-0.6.0/examples/simple_storages.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/optuna_distributed/config.py` & `optuna-distributed-0.6.0/optuna_distributed/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from __future__ import annotations
+
 import logging
-from typing import Optional
 
 from rich.logging import RichHandler
 
 
-_default_handler: Optional[logging.Handler] = None
+_default_handler: logging.Handler | None = None
 
 
 def _get_library_logger() -> logging.Logger:
     library_name = __name__.split(".")[0]
     return logging.getLogger(library_name)
```

### Comparing `optuna-distributed-0.5.0/optuna_distributed/eventloop.py` & `optuna-distributed-0.6.0/optuna_distributed/eventloop.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
+from __future__ import annotations
+
 from datetime import datetime
-from typing import Optional
-from typing import Tuple
-from typing import Type
 
 from optuna.study import Study
 from optuna.trial import TrialState
 
 from optuna_distributed.managers import ObjectiveFuncType
 from optuna_distributed.managers import OptimizationManager
 from optuna_distributed.terminal import Terminal
@@ -41,16 +40,16 @@
         self.manager = manager
         self.objective = objective
         self._interrupt_patience = interrupt_patience
 
     def run(
         self,
         terminal: Terminal,
-        timeout: Optional[float] = None,
-        catch: Tuple[Type[Exception], ...] = (),
+        timeout: float | None = None,
+        catch: tuple[type[Exception], ...] = (),
     ) -> None:
         """Starts the event loop.
 
         Args:
             terminal:
                 An instance of :obj:`optuna_distributed.terminal.Terminal`.
             timeout:
```

### Comparing `optuna-distributed-0.5.0/optuna_distributed/ipc/base.py` & `optuna-distributed-0.6.0/optuna_distributed/ipc/base.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/optuna_distributed/ipc/pipe.py` & `optuna-distributed-0.6.0/optuna_distributed/ipc/pipe.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/optuna_distributed/ipc/queue.py` & `optuna-distributed-0.6.0/optuna_distributed/ipc/queue.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
+
 import asyncio
 import pickle
-from typing import Optional
 
 from dask.distributed import Queue as DaskQueue
 
 from optuna_distributed.ipc import IPCPrimitive
 from optuna_distributed.messages import Message
 
 
@@ -27,28 +28,28 @@
             Specifies maximum number of attempts to fetch a message.
             After each attempt, timeout is extended exponentially.
     """
 
     def __init__(
         self,
         publishing: str,
-        recieving: Optional[str] = None,
-        timeout: Optional[int] = None,
-        max_retries: Optional[int] = None,
+        recieving: str | None = None,
+        timeout: int | None = None,
+        max_retries: int | None = None,
     ) -> None:
         self._publishing = publishing
         self._recieving = recieving
 
         if max_retries is not None and timeout is not None:
             raise ValueError("Exponentially growing timeout is used when `max_retries` is set.")
 
         self._timeout = timeout
         self._max_retries = max_retries
-        self._publisher: Optional[DaskQueue] = None
-        self._subscriber: Optional[DaskQueue] = None
+        self._publisher: DaskQueue | None = None
+        self._subscriber: DaskQueue | None = None
         self._initialized = False
 
     def _initialize(self) -> None:
         if not self._initialized:
             # Lazy initialization, since we have to make sure
             # channels are opened on target machine.
             self._publisher = DaskQueue(self._publishing)
```

### Comparing `optuna-distributed-0.5.0/optuna_distributed/managers/__init__.py` & `optuna-distributed-0.6.0/optuna_distributed/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/optuna_distributed/managers/base.py` & `optuna-distributed-0.6.0/optuna_distributed/managers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 import abc
 from abc import ABC
+from collections.abc import Generator
 from typing import Callable
-from typing import Generator
 from typing import Sequence
 from typing import TYPE_CHECKING
 from typing import Union
 
 from optuna.study import Study
 
 from optuna_distributed.ipc import IPCPrimitive
```

### Comparing `optuna-distributed-0.5.0/optuna_distributed/managers/distributed.py` & `optuna-distributed-0.6.0/optuna_distributed/managers/distributed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+from __future__ import annotations
+
 import asyncio
+from collections.abc import Generator
 import ctypes
 from dataclasses import dataclass
 from enum import IntEnum
 import sys
 import threading
 from threading import Thread
 import time
 from typing import Callable
-from typing import Dict
-from typing import Generator
-from typing import List
 from typing import TYPE_CHECKING
 import uuid
 
 from dask.distributed import Client
 from dask.distributed import Future
 from dask.distributed import Variable
 from optuna.exceptions import TrialPruned
@@ -55,15 +55,15 @@
     state_id: str
 
 
 class _StateSynchronizer:
     def __init__(self) -> None:
         self._optimization_enabled = Variable()
         self._optimization_enabled.set(True)
-        self._task_states: List[Variable] = []
+        self._task_states: list[Variable] = []
 
     @property
     def stop_flag(self) -> str:
         return self._optimization_enabled.name
 
     def set_initial_state(self) -> str:
         task_state = Variable()
@@ -107,37 +107,37 @@
         # Basically that means we can pump event loop from callbacks running in
         # main process with e.g. HeartbeatMessage.
         self._message_queue = Queue(
             publishing=self._public_channel,
             recieving=self._public_channel,
             timeout=heartbeat_interval,
         )
-        self._private_channels: Dict[int, str] = {}
-        self._futures: List[Future] = []
+        self._private_channels: dict[int, str] = {}
+        self._futures: list[Future] = []
 
     def _ensure_safe_exit(self, future: Future) -> None:
         if future.status in ["error", "cancelled"]:
             # FIXME: I'm not sure if there is a way to get
             # id of a trial that failed this way.
             self.register_trial_exit(-1)
             self._message_queue.put(HeartbeatMessage())
 
     def _assign_private_channel(self, trial_id: int) -> "Queue":
         private_channel = str(uuid.uuid4())
         self._private_channels[trial_id] = private_channel
         return Queue(self._public_channel, private_channel, max_retries=5)
 
-    def _create_trials(self, study: Study) -> List[DistributedTrial]:
+    def _create_trials(self, study: Study) -> list[DistributedTrial]:
         # HACK: It's kinda naughty to access _trial_id, but this is gonna make
         # our lifes much easier in messaging system.
         trial_ids = [study.ask()._trial_id for _ in range(self._n_trials)]
         return [DistributedTrial(tid, self._assign_private_channel(tid)) for tid in trial_ids]
 
-    def _add_task_context(self, trials: List[DistributedTrial]) -> List[_TaskContext]:
-        trials_with_context: List[_TaskContext] = []
+    def _add_task_context(self, trials: list[DistributedTrial]) -> list[_TaskContext]:
+        trials_with_context: list[_TaskContext] = []
         for trial in trials:
             trials_with_context.append(
                 _TaskContext(
                     trial,
                     stop_flag=self._synchronizer.stop_flag,
                     state_id=self._synchronizer.set_initial_state(),
                 )
```

### Comparing `optuna-distributed-0.5.0/optuna_distributed/managers/local.py` & `optuna-distributed-0.6.0/optuna_distributed/managers/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+from __future__ import annotations
+
+from collections.abc import Generator
 import multiprocessing
 from multiprocessing import Pipe as MultiprocessingPipe
 from multiprocessing import Process
 from multiprocessing.connection import Connection
 from multiprocessing.connection import wait
 import sys
-from typing import Dict
-from typing import Generator
-from typing import List
 from typing import TYPE_CHECKING
 
 from optuna import Study
 from optuna.exceptions import TrialPruned
 
 from optuna_distributed.ipc import IPCPrimitive
 from optuna_distributed.ipc import Pipe
@@ -45,31 +45,31 @@
         if n_jobs <= 0 or n_jobs > multiprocessing.cpu_count():
             self._n_jobs = multiprocessing.cpu_count()
         else:
             self._n_jobs = n_jobs
 
         self._workers_to_spawn = min(self._n_jobs, n_trials)
         self._trials_remaining = n_trials - self._workers_to_spawn
-        self._pool: Dict[int, Connection] = {}
-        self._processes: List[Process] = []
+        self._pool: dict[int, Connection] = {}
+        self._processes: list[Process] = []
 
     def create_futures(self, study: Study, objective: ObjectiveFuncType) -> None:
         trial_ids = [study.ask()._trial_id for _ in range(self._workers_to_spawn)]
         for trial_id in trial_ids:
             master, worker = MultiprocessingPipe()
             trial = DistributedTrial(trial_id, Pipe(worker))
             p = Process(target=_trial_runtime, args=(objective, trial), daemon=True)
             p.start()
             self._processes.append(p)
             self._pool[trial_id] = master
             worker.close()
 
     def get_message(self) -> Generator[Message, None, None]:
         while True:
-            messages: List[Message] = []
+            messages: list[Message] = []
             for incoming in wait(self._pool.values(), timeout=10):
                 # FIXME: This assertion is true only for Unix systems.
                 # Some refactoring is needed to support Windows as well.
                 # https://docs.python.org/3/library/multiprocessing.html#multiprocessing.connection.wait
                 assert isinstance(incoming, Connection)
                 try:
                     message = incoming.recv()
```

### Comparing `optuna-distributed-0.5.0/optuna_distributed/messages/__init__.py` & `optuna-distributed-0.6.0/optuna_distributed/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/optuna_distributed/messages/base.py` & `optuna-distributed-0.6.0/optuna_distributed/messages/base.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/optuna_distributed/messages/completed.py` & `optuna-distributed-0.6.0/optuna_distributed/messages/completed.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from __future__ import annotations
+
+from collections.abc import Sequence
 import io
 import logging
-from typing import Sequence
 from typing import TYPE_CHECKING
-from typing import Union
 
 from optuna.study import Study
 from optuna.trial import FrozenTrial
 from optuna.trial import Trial
 from optuna.trial import TrialState
 
 from optuna_distributed.messages import Message
@@ -31,15 +32,15 @@
             Id of a trial to which the message is referring.
         value_or_values:
             Objective value or sequence of objective values.
     """
 
     closing = True
 
-    def __init__(self, trial_id: int, value_or_values: Union[Sequence[float], float]) -> None:
+    def __init__(self, trial_id: int, value_or_values: Sequence[float] | float) -> None:
         self._trial_id = trial_id
         self._value_or_values = value_or_values
 
     def process(self, study: Study, manager: "OptimizationManager") -> None:
         trial = Trial(study, self._trial_id)
         try:
             frozen_trial = study.tell(trial, self._value_or_values, skip_if_finished=True)
```

### Comparing `optuna-distributed-0.5.0/optuna_distributed/messages/failed.py` & `optuna-distributed-0.6.0/optuna_distributed/messages/failed.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/optuna_distributed/messages/heartbeat.py` & `optuna-distributed-0.6.0/optuna_distributed/messages/heartbeat.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/optuna_distributed/messages/property.py` & `optuna-distributed-0.6.0/optuna_distributed/messages/property.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/optuna_distributed/messages/pruned.py` & `optuna-distributed-0.6.0/optuna_distributed/messages/pruned.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/optuna_distributed/messages/report.py` & `optuna-distributed-0.6.0/optuna_distributed/messages/report.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/optuna_distributed/messages/response.py` & `optuna-distributed-0.6.0/optuna_distributed/messages/response.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/optuna_distributed/messages/setattr.py` & `optuna-distributed-0.6.0/optuna_distributed/messages/setattr.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/optuna_distributed/messages/shouldprune.py` & `optuna-distributed-0.6.0/optuna_distributed/messages/shouldprune.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/optuna_distributed/messages/suggest.py` & `optuna-distributed-0.6.0/optuna_distributed/messages/suggest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
+
 from typing import TYPE_CHECKING
-from typing import Union
 
 from optuna.distributions import BaseDistribution
 from optuna.distributions import CategoricalChoiceType
 from optuna.distributions import CategoricalDistribution
 from optuna.distributions import FloatDistribution
 from optuna.distributions import IntDistribution
 from optuna.study import Study
@@ -38,15 +39,15 @@
     def __init__(self, trial_id: int, name: str, distribution: BaseDistribution) -> None:
         self._trial_id = trial_id
         self._name = name
         self._distribution = distribution
 
     def process(self, study: Study, manager: "OptimizationManager") -> None:
         trial = Trial(study, self._trial_id)
-        value: Union[float, int, CategoricalChoiceType]
+        value: float | int | CategoricalChoiceType
         if isinstance(self._distribution, FloatDistribution):
             value = trial.suggest_float(
                 name=self._name,
                 low=self._distribution.low,
                 high=self._distribution.high,
                 step=self._distribution.step,
                 log=self._distribution.log,
```

### Comparing `optuna-distributed-0.5.0/optuna_distributed/study.py` & `optuna-distributed-0.6.0/optuna_distributed/study.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
+from __future__ import annotations
+
+from collections.abc import Callable
+from collections.abc import Container
+from collections.abc import Iterable
+from collections.abc import Sequence
 import sys
 from typing import Any
-from typing import Callable
-from typing import Container
-from typing import Dict
-from typing import Iterable
-from typing import List
-from typing import Optional
-from typing import Sequence
 from typing import TYPE_CHECKING
-from typing import Tuple
-from typing import Type
-from typing import Union
 
 from dask.distributed import Client
 from dask.distributed import LocalCluster
 from optuna.distributions import BaseDistribution
 from optuna.study import Study
 from optuna.study import StudyDirection
 from optuna.trial import FrozenTrial
@@ -60,66 +56,70 @@
         client:
             A Dask client. When specified, all trials will be passed to
             Dask scheduler to distribute across available workers.
             If :obj:`None`, multiprocessing backend is used for
             process based parallelism.
     """
 
-    def __init__(self, study: Study, client: Optional[Client] = None) -> None:
+    def __init__(self, study: Study, client: Client | None = None) -> None:
         self._study = study
         self._client = client
 
     @property
-    def best_params(self) -> Dict[str, Any]:
+    def best_params(self) -> dict[str, Any]:
         """Return parameters of the best trial in the study."""
         return self._study.best_params
 
     @property
     def best_value(self) -> float:
         """Return the best objective value in the study."""
         return self._study.best_value
 
     @property
     def best_trial(self) -> FrozenTrial:
         """Return the best trial in the study."""
         return self._study.best_trial
 
     @property
-    def best_trials(self) -> List[FrozenTrial]:
+    def best_trials(self) -> list[FrozenTrial]:
         """Return trials located at the Pareto front in the study."""
         return self._study.best_trials
 
     @property
     def direction(self) -> StudyDirection:
         """Return the direction of the study."""
         return self._study.direction
 
     @property
-    def directions(self) -> List[StudyDirection]:
+    def directions(self) -> list[StudyDirection]:
         """Return the directions of the study."""
         return self._study.directions
 
     @property
-    def trials(self) -> List[FrozenTrial]:
+    def trials(self) -> list[FrozenTrial]:
         """Return all trials in the study."""
         return self._study.trials
 
     @property
-    def user_attrs(self) -> Dict[str, Any]:
+    def user_attrs(self) -> dict[str, Any]:
         """Return user attributes."""
         return self._study.user_attrs
 
     @property
-    def system_attrs(self) -> Dict[str, Any]:
+    def system_attrs(self) -> dict[str, Any]:
         """Return system attributes."""
         return self._study.system_attrs
 
+    def into_study(self) -> Study:
+        """Returns regular Optuna study."""
+        return self._study
+
     def get_trials(
-        self, deepcopy: bool = True, states: Optional[Container[TrialState]] = None
-    ) -> List[FrozenTrial]:
+        self, deepcopy: bool = True, states: Container[TrialState] | None = None
+    ) -> list[FrozenTrial]:
         """Return all trials in the study.
 
         For complete documentation, please refer to:
         https://optuna.readthedocs.io/en/stable/reference/generated/optuna.study.Study.html#optuna.study.Study.get_trials
 
         Args:
             deepcopy:
@@ -128,19 +128,19 @@
                 Trial states to filter on. If :obj:`None`, include all states.
         """
         return self._study.get_trials(deepcopy, states)
 
     def optimize(
         self,
         func: ObjectiveFuncType,
-        n_trials: Optional[int] = None,
-        timeout: Optional[float] = None,
+        n_trials: int | None = None,
+        timeout: float | None = None,
         n_jobs: int = -1,
-        catch: Union[Iterable[Type[Exception]], Type[Exception]] = (),
-        callbacks: Optional[List[Callable[["Study", FrozenTrial], None]]] = None,
+        catch: Iterable[type[Exception]] | type[Exception] = (),
+        callbacks: list[Callable[["Study", FrozenTrial], None]] | None = None,
         show_progress_bar: bool = False,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         """Optimize an objective function.
 
         Optimization is done by choosing a suitable set of hyperparameter values from a given
@@ -200,31 +200,31 @@
             for trial in trials:
                 self._study._storage.set_trial_state_values(trial._trial_id, TrialState.FAIL)
             raise
 
         finally:
             self._study._storage.remove_session()
 
-    def ask(self, fixed_distributions: Optional[Dict[str, BaseDistribution]] = None) -> Trial:
+    def ask(self, fixed_distributions: dict[str, BaseDistribution] | None = None) -> Trial:
         """Create a new trial from which hyperparameters can be suggested.
 
         For complete documentation, please refer to:
         https://optuna.readthedocs.io/en/stable/reference/generated/optuna.study.Study.html#optuna.study.Study.ask
 
         Args:
             fixed_distributions:
                 A dictionary containing the parameter names and parameter's distributions.
         """
         return self._study.ask(fixed_distributions)
 
     def tell(
         self,
-        trial: Union[Trial, int],
-        values: Optional[Union[float, Sequence[float]]] = None,
-        state: Optional[TrialState] = None,
+        trial: Trial | int,
+        values: float | Sequence[float] | None = None,
+        state: TrialState | None = None,
         skip_if_finished: bool = False,
     ) -> FrozenTrial:
         """Finish a trial created with :func:`~optuna_distributed.study.DistributedStudy.ask`.
 
         For complete documentation, please refer to:
         https://optuna.readthedocs.io/en/stable/reference/generated/optuna.study.Study.html#optuna.study.Study.tell
 
@@ -264,15 +264,15 @@
             key: A key string of the attribute.
             value: A value of the attribute. The value should be JSON serializable
         """
         self._study.set_system_attr(key, value)
 
     def trials_dataframe(
         self,
-        attrs: Tuple[str, ...] = (
+        attrs: tuple[str, ...] = (
             "number",
             "value",
             "datetime_start",
             "datetime_complete",
             "duration",
             "params",
             "user_attrs",
@@ -301,16 +301,16 @@
         This method is effectively a noop, sice there is no way to reach study from the
         objective function at the moment. TODO(xadrianzetx) Implement this.
         """
         self._study.stop()
 
     def enqueue_trial(
         self,
-        params: Dict[str, Any],
-        user_attrs: Optional[Dict[str, Any]] = None,
+        params: dict[str, Any],
+        user_attrs: dict[str, Any] | None = None,
         skip_if_exists: bool = False,
     ) -> None:
         """Enqueue a trial with given parameter values.
 
         For complete documentation, please refer to:
         https://optuna.readthedocs.io/en/stable/reference/generated/optuna.study.Study.html#optuna.study.Study.enqueue_trial
 
@@ -343,15 +343,15 @@
 
         Args:
             trial: Trials to add.
         """
         self._study.add_trials(trials)
 
 
-def from_study(study: Study, client: Optional[Client] = None) -> DistributedStudy:
+def from_study(study: Study, client: Client | None = None) -> DistributedStudy:
     """Takes regular Optuna study and extends it to :class:`~optuna_distributed.DistributedStudy`.
 
     This creates an object which behaves like regular Optuna study, except trials
     will be evaluated in parallel after :func:`optuna_distributed.DistributedStudy.optimize`
     is called. When :obj:`client` is :obj:`None`, work is distributed among available CPU cores
     by using multiprocessing. If Dask client is specified, `optuna_distributed` can use it to
     distribute trials across many physical workers in the cluster.
```

### Comparing `optuna-distributed-0.5.0/optuna_distributed/terminal.py` & `optuna-distributed-0.6.0/optuna_distributed/terminal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from __future__ import annotations
 
 from rich.progress import BarColumn
 from rich.progress import Progress
 from rich.progress import TaskProgressColumn
 from rich.progress import TextColumn
 from rich.progress import TimeElapsedColumn
 from rich.status import Status
@@ -18,15 +18,15 @@
         n_trials:
             The number of trials to run in total.
         timeout:
             Stops study after the given number of second(s).
     """
 
     def __init__(
-        self, show_progress_bar: bool, n_trials: int, timeout: Optional[float] = None
+        self, show_progress_bar: bool, n_trials: int, timeout: float | None = None
     ) -> None:
         self._timeout = timeout
         self._progbar = Progress(
             TextColumn("[progress.description]{task.description}"),
             BarColumn(complete_style=Style(color="light_coral")),
             TaskProgressColumn(),
             TimeElapsedColumn(),
```

### Comparing `optuna-distributed-0.5.0/optuna_distributed/trial.py` & `optuna-distributed-0.6.0/optuna_distributed/trial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+from __future__ import annotations
+
+from collections.abc import Sequence
 import datetime
 from typing import Any
-from typing import Dict
-from typing import Optional
-from typing import Sequence
 from typing import TypeVar
 
 from optuna.distributions import BaseDistribution
 from optuna.distributions import CategoricalChoiceType
 from optuna.distributions import CategoricalDistribution
 from optuna.distributions import FloatDistribution
 from optuna.distributions import IntDistribution
@@ -62,15 +62,15 @@
 
     def suggest_float(
         self,
         name: str,
         low: float,
         high: float,
         *,
-        step: Optional[float] = None,
+        step: float | None = None,
         log: bool = False,
     ) -> float:
         """Suggest a value for the floating point parameter.
 
         For complete documentation, please refer to:
         https://optuna.readthedocs.io/en/stable/reference/generated/optuna.trial.Trial.html#optuna.trial.Trial.suggest_float
 
@@ -234,35 +234,35 @@
             value:
                 A value of the attribute. The value should be able to serialize with pickle.
         """
         message = SetAttributeMessage(self.trial_id, key, value, kind="system")
         self.connection.put(message)
 
     @property
-    def params(self) -> Dict[str, Any]:
+    def params(self) -> dict[str, Any]:
         """Return parameters to be optimized."""
         return self._get_property("params")
 
     @property
-    def distributions(self) -> Dict[str, BaseDistribution]:
+    def distributions(self) -> dict[str, BaseDistribution]:
         """Return distributions of parameters to be optimized."""
         return self._get_property("distributions")
 
     @property
-    def user_attrs(self) -> Dict[str, Any]:
+    def user_attrs(self) -> dict[str, Any]:
         """Return user attributes."""
         return self._get_property("user_attrs")
 
     @property
-    def system_attrs(self) -> Dict[str, Any]:
+    def system_attrs(self) -> dict[str, Any]:
         """Return system attributes."""
         return self._get_property("system_attrs")
 
     @property
-    def datetime_start(self) -> Optional[datetime.datetime]:
+    def datetime_start(self) -> datetime.datetime | None:
         """Return start datetime."""
         return self._get_property("datetime_start")
 
     @property
     def number(self) -> int:
         """Return trial's number which is consecutive and unique in a study."""
         return self._get_property("number")
```

### Comparing `optuna-distributed-0.5.0/optuna_distributed.egg-info/PKG-INFO` & `optuna-distributed-0.6.0/optuna_distributed.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optuna-distributed
-Version: 0.5.0
+Version: 0.6.0
 Summary: Distributed hyperparameter optimization made easy
 Author-email: Adrian Zuber <xadrianzetx@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/xadrianzetx/optuna-distributed
 Project-URL: Bug Tracker, https://github.com/xadrianzetx/optuna-distributed/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -85,7 +85,8 @@
 
 But there's more! All of the core Optuna APIs, including [storages, samplers](https://github.com/xadrianzetx/optuna-distributed/blob/main/examples/simple_storages.py) and [pruners](https://github.com/xadrianzetx/optuna-distributed/blob/main/examples/simple_pruning.py) are supported! If you'd like to know how Optuna-distributed works, then check out [this article on Optuna blog](https://medium.com/optuna/running-distributed-hyperparameter-optimization-with-optuna-distributed-17bb2f7d422d).
 
 ## What's missing?
 * Support for callbacks and Optuna integration modules.
 * Study APIs such as [`study.stop`](https://optuna.readthedocs.io/en/stable/reference/generated/optuna.study.Study.html#optuna.study.Study.stop) can't be called from trial at the moment.
 * Local asynchronous optimization on Windows machines. Distributed mode is still available.
+* Support for [`optuna.terminator`](https://optuna.readthedocs.io/en/stable/reference/terminator.html).
```

### Comparing `optuna-distributed-0.5.0/optuna_distributed.egg-info/SOURCES.txt` & `optuna-distributed-0.6.0/optuna_distributed.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 .github/workflows/format.yaml
 .github/workflows/release.yaml
 .github/workflows/test.yaml
 examples/disable_logging.py
 examples/quadratic_simple.py
 examples/simple_pruning.py
 examples/simple_storages.py
+examples/visualization.py
 optuna_distributed/__init__.py
 optuna_distributed/config.py
 optuna_distributed/eventloop.py
 optuna_distributed/study.py
 optuna_distributed/terminal.py
 optuna_distributed/trial.py
 optuna_distributed.egg-info/PKG-INFO
```

### Comparing `optuna-distributed-0.5.0/pyproject.toml` & `optuna-distributed-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/tests/test_eventloop.py` & `optuna-distributed-0.6.0/tests/test_eventloop.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/tests/test_ipc.py` & `optuna-distributed-0.6.0/tests/test_ipc.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/tests/test_managers.py` & `optuna-distributed-0.6.0/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/tests/test_messages.py` & `optuna-distributed-0.6.0/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `optuna-distributed-0.5.0/tests/test_trial.py` & `optuna-distributed-0.6.0/tests/test_trial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from __future__ import annotations
+
 from collections import deque
-from typing import Deque
-from typing import List
 
 from optuna.distributions import CategoricalDistribution
 from optuna.distributions import FloatDistribution
 from optuna.distributions import IntDistribution
 import pytest
 
 from optuna_distributed.ipc import IPCPrimitive
@@ -16,16 +16,16 @@
 from optuna_distributed.messages import SuggestMessage
 from optuna_distributed.messages import TrialPropertyMessage
 from optuna_distributed.trial import DistributedTrial
 
 
 class MockIPC(IPCPrimitive):
     def __init__(self) -> None:
-        self.captured: List[Message] = []
-        self.responses: Deque[ResponseMessage] = deque()
+        self.captured: list[Message] = []
+        self.responses: deque[ResponseMessage] = deque()
 
     def get(self) -> "Message":
         return self.responses.popleft()
 
     def put(self, message: "Message") -> None:
         self.captured.append(message)
```

