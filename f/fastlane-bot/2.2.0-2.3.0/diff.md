# Comparing `tmp/fastlane_bot-2.2.0.tar.gz` & `tmp/fastlane_bot-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastlane_bot-2.2.0.tar", last modified: Wed Jul 26 13:34:19 2023, max compression
+gzip compressed data, was "fastlane_bot-2.3.0.tar", last modified: Wed Jul 26 14:30:05 2023, max compression
```

## Comparing `fastlane_bot-2.2.0.tar` & `fastlane_bot-2.3.0.tar`

### file list

```diff
@@ -1,102 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:19.577657 fastlane_bot-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-26 13:34:19.577657 fastlane_bot-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:19.565657 fastlane_bot-2.2.0/fastlane_bot/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-26 13:33:48.000000 fastlane_bot-2.2.0/fastlane_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44456 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:19.569657 fastlane_bot-2.2.0/fastlane_bot/config/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/config/cloaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/config/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/config/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/config/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/config/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/config/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/config/selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:19.569657 fastlane_bot-2.2.0/fastlane_bot/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   192059 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/data/abi.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/data/pools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:19.569657 fastlane_bot-2.2.0/fastlane_bot/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:19.569657 fastlane_bot-2.2.0/fastlane_bot/events/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/exchanges/bancor_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/exchanges/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/exchanges/carbon_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/exchanges/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/exchanges/sushiswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/exchanges/uniswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/exchanges/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:19.573657 fastlane_bot-2.2.0/fastlane_bot/events/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/managers/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/managers/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/managers/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/managers/pools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:19.573657 fastlane_bot-2.2.0/fastlane_bot/events/pools/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/pools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/pools/bancor_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/pools/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/pools/carbon_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/pools/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/pools/sushiswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/pools/uniswap_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/pools/uniswap_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:19.573657 fastlane_bot-2.2.0/fastlane_bot/events/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/tests/convert_py_test_to_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/tests/test_exchanges.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/tests/test_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:19.573657 fastlane_bot-2.2.0/fastlane_bot/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/helpers/poolandtokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/helpers/receipthandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/helpers/routehandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/helpers/submithandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/helpers/tradeinstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/helpers/txhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/helpers/univ3calc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:19.577657 fastlane_bot-2.2.0/fastlane_bot/modes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/modes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/modes/base_pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/modes/base_triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/modes/pairwise_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/modes/pairwise_single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:19.577657 fastlane_bot-2.2.0/fastlane_bot/modes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/modes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/modes/tests/test_pairwise_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/modes/triangle_bancor_v3_two_hop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/modes/triangle_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/modes/triangle_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/modes/triangle_single_bancor3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:19.577657 fastlane_bot-2.2.0/fastlane_bot/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/tools/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    75829 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/tools/arbgraphs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85741 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/tools/cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    70412 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/tools/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/tools/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/tools/simplepair.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/tools/tokenscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/tools/univ3calc_DELETE.py
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/fastlane_bot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:34:19.569657 fastlane_bot-2.2.0/fastlane_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-26 13:34:19.000000 fastlane_bot-2.2.0/fastlane_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-26 13:34:19.000000 fastlane_bot-2.2.0/fastlane_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:34:19.000000 fastlane_bot-2.2.0/fastlane_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-26 13:34:19.000000 fastlane_bot-2.2.0/fastlane_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 13:34:19.000000 fastlane_bot-2.2.0/fastlane_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:34:19.577657 fastlane_bot-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-26 13:32:31.000000 fastlane_bot-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.870561 fastlane_bot-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-26 14:30:05.870561 fastlane_bot-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.846561 fastlane_bot-2.3.0/fastlane_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-26 14:29:31.000000 fastlane_bot-2.3.0/fastlane_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44456 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.850561 fastlane_bot-2.3.0/fastlane_bot/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/cloaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/config/selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.850561 fastlane_bot-2.3.0/fastlane_bot/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192059 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/data/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/data/pools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.850561 fastlane_bot-2.3.0/fastlane_bot/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.850561 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/bancor_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/carbon_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/sushiswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/uniswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/exchanges/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.854561 fastlane_bot-2.3.0/fastlane_bot/events/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/managers/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/managers/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/managers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/managers/pools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.854561 fastlane_bot-2.3.0/fastlane_bot/events/pools/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/bancor_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/carbon_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/sushiswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/uniswap_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/pools/uniswap_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.854561 fastlane_bot-2.3.0/fastlane_bot/events/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/tests/convert_py_test_to_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/tests/test_exchanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/tests/test_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.858561 fastlane_bot-2.3.0/fastlane_bot/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/poolandtokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/receipthandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/routehandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/submithandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/tradeinstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/txhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/helpers/univ3calc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.858561 fastlane_bot-2.3.0/fastlane_bot/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/base_pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/base_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/pairwise_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/pairwise_single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.858561 fastlane_bot-2.3.0/fastlane_bot/modes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/tests/test_pairwise_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/triangle_bancor_v3_two_hop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/triangle_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/triangle_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/modes/triangle_single_bancor3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.862561 fastlane_bot-2.3.0/fastlane_bot/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.866561 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_000_Template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70594 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_002_CPCandOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20948 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_003_Serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29819 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_004_GraphCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_005_Uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_007_NoneResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_033_Pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_034_Interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_035_Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_036_Manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_037_Exchanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_038_TestBancorV3Mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17871 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_039_TestMultiMode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_040_TestSingleMode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22316 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_042_TestBancorV3ModeTwoHop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_043_TestEmptyCarbonOrders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_047_Randomizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25275 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_900_OptimizerDetailedSlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_901_TestMultiTriangleModeSlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tests/nbtest/test_902_ValidatorSlow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.866561 fastlane_bot-2.3.0/fastlane_bot/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76162 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/arbgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86957 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/cryptocompare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/noneresult.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.866561 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18750 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/convexoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24480 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/cpcarboptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/dcbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18617 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/margpoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/optimizer/simpleoptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/simplepair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/tokenscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/tools/univ3calc_DELETE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/fastlane_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:30:05.846561 fastlane_bot-2.3.0/fastlane_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-26 14:30:05.000000 fastlane_bot-2.3.0/fastlane_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-26 14:30:05.000000 fastlane_bot-2.3.0/fastlane_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:30:05.000000 fastlane_bot-2.3.0/fastlane_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-26 14:30:05.000000 fastlane_bot-2.3.0/fastlane_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 14:30:05.000000 fastlane_bot-2.3.0/fastlane_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:30:05.870561 fastlane_bot-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-26 14:27:27.000000 fastlane_bot-2.3.0/setup.py
```

### Comparing `fastlane_bot-2.2.0/LICENSE` & `fastlane_bot-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/PKG-INFO` & `fastlane_bot-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlane_bot
-Version: 2.2.0
+Version: 2.3.0
 Summary: Carbon Arbitrage Bot, an open-source arbitrage protocol, allows any user to perform arbitrage between Bancor ecosystem protocols and external exchanges and redirect arbitrage profits back to the protocol.
 Home-page: https://github.com/bancorprotocol/carbon-bot
 Author: Bancor Network
 Author-email: mike@bancor.network
 Requires-Python: >= 3.8, != 3.11.*
 Description-Content-Type: text/markdown
 Provides-Extra: complete
```

### Comparing `fastlane_bot-2.2.0/README.md` & `fastlane_bot-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/bot.py` & `fastlane_bot-2.3.0/fastlane_bot/bot.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/config/base.py` & `fastlane_bot-2.3.0/fastlane_bot/config/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/config/cloaker.py` & `fastlane_bot-2.3.0/fastlane_bot/config/cloaker.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/config/config.py` & `fastlane_bot-2.3.0/fastlane_bot/config/config.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/config/connect.py` & `fastlane_bot-2.3.0/fastlane_bot/config/connect.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/config/db.py` & `fastlane_bot-2.3.0/fastlane_bot/config/db.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/config/logger.py` & `fastlane_bot-2.3.0/fastlane_bot/config/logger.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/config/network.py` & `fastlane_bot-2.3.0/fastlane_bot/config/network.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/config/provider.py` & `fastlane_bot-2.3.0/fastlane_bot/config/provider.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/config/selectors.py` & `fastlane_bot-2.3.0/fastlane_bot/config/selectors.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/data/abi.py` & `fastlane_bot-2.3.0/fastlane_bot/data/abi.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/data/pools.py` & `fastlane_bot-2.3.0/fastlane_bot/data/pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/exchanges/__init__.py` & `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/exchanges/bancor_v3.py` & `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/bancor_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/exchanges/base.py` & `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/exchanges/carbon_v1.py` & `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/carbon_v1.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/exchanges/factory.py` & `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/factory.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/exchanges/sushiswap_v2.py` & `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/sushiswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/exchanges/uniswap_v2.py` & `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/uniswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/exchanges/uniswap_v3.py` & `fastlane_bot-2.3.0/fastlane_bot/events/exchanges/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/interface.py` & `fastlane_bot-2.3.0/fastlane_bot/events/interface.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/managers/base.py` & `fastlane_bot-2.3.0/fastlane_bot/events/managers/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/managers/contracts.py` & `fastlane_bot-2.3.0/fastlane_bot/events/managers/contracts.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/managers/events.py` & `fastlane_bot-2.3.0/fastlane_bot/events/managers/events.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/managers/manager.py` & `fastlane_bot-2.3.0/fastlane_bot/events/managers/manager.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/managers/pools.py` & `fastlane_bot-2.3.0/fastlane_bot/events/managers/pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/pools/__init__.py` & `fastlane_bot-2.3.0/fastlane_bot/events/pools/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/pools/bancor_v3.py` & `fastlane_bot-2.3.0/fastlane_bot/events/pools/bancor_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/pools/base.py` & `fastlane_bot-2.3.0/fastlane_bot/events/pools/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/pools/carbon_v1.py` & `fastlane_bot-2.3.0/fastlane_bot/events/pools/carbon_v1.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/pools/factory.py` & `fastlane_bot-2.3.0/fastlane_bot/events/pools/factory.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/pools/sushiswap_v2.py` & `fastlane_bot-2.3.0/fastlane_bot/events/pools/sushiswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/pools/uniswap_v2.py` & `fastlane_bot-2.3.0/fastlane_bot/events/pools/uniswap_v2.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/pools/uniswap_v3.py` & `fastlane_bot-2.3.0/fastlane_bot/events/pools/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/tests/convert_py_test_to_jupyter.py` & `fastlane_bot-2.3.0/fastlane_bot/events/tests/convert_py_test_to_jupyter.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/tests/test_exchanges.py` & `fastlane_bot-2.3.0/fastlane_bot/events/tests/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/tests/test_interface.py` & `fastlane_bot-2.3.0/fastlane_bot/events/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/tests/test_manager.py` & `fastlane_bot-2.3.0/fastlane_bot/events/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/tests/test_pools.py` & `fastlane_bot-2.3.0/fastlane_bot/events/tests/test_pools.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/tests/test_utils.py` & `fastlane_bot-2.3.0/fastlane_bot/events/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/events/utils.py` & `fastlane_bot-2.3.0/fastlane_bot/events/utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/helpers/poolandtokens.py` & `fastlane_bot-2.3.0/fastlane_bot/helpers/poolandtokens.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/helpers/routehandler.py` & `fastlane_bot-2.3.0/fastlane_bot/helpers/routehandler.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/helpers/submithandler.py` & `fastlane_bot-2.3.0/fastlane_bot/helpers/submithandler.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/helpers/tradeinstruction.py` & `fastlane_bot-2.3.0/fastlane_bot/helpers/tradeinstruction.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/helpers/txhelpers.py` & `fastlane_bot-2.3.0/fastlane_bot/helpers/txhelpers.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/helpers/univ3calc.py` & `fastlane_bot-2.3.0/fastlane_bot/helpers/univ3calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 (c) Copyright Bprotocol foundation 2023. 
 Licensed under MIT
 
 NOTE: this class is not part of the API of the Carbon protocol, and you must expect breaking
 changes even in minor version updates. Use at your own risk.
 """
-__VERSION__ = "1.4" 
-__DATE__ = "07/May/2023"
+__VERSION__ = "1.4.1" 
+__DATE__ = "25/Jul/2023"
 
 from math import sqrt
 from dataclasses import dataclass, InitVar, asdict
 
 
 @dataclass(frozen=True)
 class Univ3Calculator():
@@ -35,20 +35,20 @@
     tick: int
     liquidity: int
     fee_const: int 
 
     tkn0decv: InitVar[int] = None
     tkn1decv: InitVar[int] = None
     addrdec: InitVar[dict] = None
-    ADDRDEC = dict(
+    ADDRDEC = {
         # only for testing
-        USDC = ("0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48", 6),
-        WETH = ("0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2", 18),
-    )
-
+        "USDC-eB48": ("0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48", 6),
+        "WETH-6Cc2": ("0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2", 18),
+    }
+    
     @classmethod
     def from_dict(cls, d, fee_const, *, addrdec=None, tkn0decv=None, tkn1decv=None):
         """
         alternative constructor from a dictionary
         
         :d:             dict with keys: token0 [address], token1 [address], sqrt_price_q96, tick, liquidity
         :fee_const:     fee constant (FEE100, ...)
```

### Comparing `fastlane_bot-2.2.0/fastlane_bot/modes/base.py` & `fastlane_bot-2.3.0/fastlane_bot/modes/base.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/modes/base_pairwise.py` & `fastlane_bot-2.3.0/fastlane_bot/modes/base_pairwise.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/modes/base_triangle.py` & `fastlane_bot-2.3.0/fastlane_bot/modes/base_triangle.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/modes/pairwise_multi.py` & `fastlane_bot-2.3.0/fastlane_bot/modes/pairwise_multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 from typing import List, Any, Tuple, Union, Hashable
 
 import pandas as pd
 
 from fastlane_bot.modes.base_pairwise import ArbitrageFinderPairwiseBase
 from fastlane_bot.tools.cpc import CPCContainer
-from fastlane_bot.tools.optimizer import CPCArbOptimizer
+from fastlane_bot.tools.optimizer import MargPOptimizer
 
 
 class FindArbitrageMultiPairwise(ArbitrageFinderPairwiseBase):
     """
     Multi-pairwise arbitrage finder mode.
     """
 
@@ -158,15 +158,15 @@
     def run_main_flow(
         curves: List[Any], src_token: str, tkn0: str, tkn1: str
     ) -> Tuple[Any, float, Any, pd.DataFrame]:
         """
         Run main flow to find arbitrage.
         """
         CC_cc = CPCContainer(curves)
-        O = CPCArbOptimizer(CC_cc)
+        O = MargPOptimizer(CC_cc)
         pstart = {
             tkn0: CC_cc.bypairs(f"{tkn0}/{tkn1}")[0].p
         }  # this intentionally selects the non_carbon curve
         r = O.margp_optimizer(src_token, params=dict(pstart=pstart))
         profit_src = -r.result
         trade_instructions_df = r.trade_instructions(O.TIF_DFAGGR)
         return O, profit_src, r, trade_instructions_df
```

### Comparing `fastlane_bot-2.2.0/fastlane_bot/modes/pairwise_single.py` & `fastlane_bot-2.3.0/fastlane_bot/modes/pairwise_single.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 from typing import List, Any, Tuple, Union
 
 from tqdm.contrib import itertools
 
 from fastlane_bot.modes.base_pairwise import ArbitrageFinderPairwiseBase
 from fastlane_bot.tools.cpc import CPCContainer
-from fastlane_bot.tools.optimizer import CPCArbOptimizer
+from fastlane_bot.tools.optimizer import MargPOptimizer
 
 
 class FindArbitrageSinglePairwise(ArbitrageFinderPairwiseBase):
     """
     Single pairwise arbitrage finder mode
     """
 
@@ -54,24 +54,25 @@
             )
 
             if not curve_combos:
                 continue
 
             for curve_combo in curve_combos:
                 CC_cc = CPCContainer(curve_combo)
-                O = CPCArbOptimizer(CC_cc)
+                O = MargPOptimizer(CC_cc)
                 src_token = tkn1
                 try:
                     pstart = {tkn0: CC_cc.bypairs(f"{tkn0}/{tkn1}")[0].p}
                     r = O.margp_optimizer(src_token, params=dict(pstart=pstart))
                     profit_src = -r.result
                     trade_instructions_df = r.trade_instructions(O.TIF_DFAGGR)
                     trade_instructions_dic = r.trade_instructions(O.TIF_DICTS)
                     trade_instructions = r.trade_instructions()
                 except Exception as e:
+                    print("[FindArbitrageSinglePairwise] Exception: ", e)
                     continue
 
                 # Get the candidate ids
                 cids = [ti["cid"] for ti in trade_instructions_dic]
 
                 # Calculate the profit
                 profit = self.calculate_profit(src_token, profit_src, self.CCm, cids)
```

### Comparing `fastlane_bot-2.2.0/fastlane_bot/modes/tests/test_pairwise_single.py` & `fastlane_bot-2.3.0/fastlane_bot/modes/tests/test_pairwise_single.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/modes/triangle_bancor_v3_two_hop.py` & `fastlane_bot-2.3.0/fastlane_bot/modes/triangle_bancor_v3_two_hop.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under MIT
 """
 import math
 from typing import Union, List, Tuple, Any, Iterable
 
 from fastlane_bot.modes.base_triangle import ArbitrageFinderTriangleBase
 from fastlane_bot.tools.cpc import CPCContainer, T, ConstantProductCurve
-from fastlane_bot.tools.optimizer import CPCArbOptimizer
+from fastlane_bot.tools.optimizer import MargPOptimizer
 
 
 class ArbitrageFinderTriangleBancor3TwoHop(ArbitrageFinderTriangleBase):
     """
     Bancor V3 triangular arbitrage finder mode
     """
 
@@ -288,15 +288,15 @@
         tuple
             Tuple of profit, trade instructions, trade instructions dataframe and trade instructions dictionary.
 
         """
 
         # Instantiate the container and optimizer objects
         CC_cc = CPCContainer(miniverse)
-        O = CPCArbOptimizer(CC_cc)
+        O = MargPOptimizer(CC_cc)
 
         # Perform the optimization
         r = O.margp_optimizer(src_token)
 
         # Get the profit in the source token
         profit_src = -r.result
```

### Comparing `fastlane_bot-2.2.0/fastlane_bot/modes/triangle_multi.py` & `fastlane_bot-2.3.0/fastlane_bot/modes/triangle_multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 (c) Copyright Bprotocol foundation 2023.
 Licensed under MIT
 """
 from typing import List, Any, Tuple, Union
 
 from fastlane_bot.modes.base_triangle import ArbitrageFinderTriangleBase
 from fastlane_bot.tools.cpc import CPCContainer
-from fastlane_bot.tools.optimizer import CPCArbOptimizer
+from fastlane_bot.tools.optimizer import MargPOptimizer
 
 
 class ArbitrageFinderTriangleMulti(ArbitrageFinderTriangleBase):
     """
     Triangular arbitrage finder mode
     """
 
@@ -34,15 +34,15 @@
             self.flashloan_tokens, self.CCm, arb_mode=self.arb_mode
         )
 
         for src_token, miniverse in combos:
 
             r = None
             CC_cc = CPCContainer(miniverse)
-            O = CPCArbOptimizer(CC_cc)
+            O = MargPOptimizer(CC_cc)
             try:
                 r = O.margp_optimizer(src_token)
                 trade_instructions_df = r.trade_instructions(O.TIF_DFAGGR)
                 trade_instructions_dic = r.trade_instructions(O.TIF_DICTS)
                 trade_instructions = r.trade_instructions()
                 """
                 The following handles an edge case until parallel execution is available:
@@ -76,15 +76,15 @@
                         curve
                         for curve in miniverse
                         if curve.cid not in wrong_direction_cids
                     ]
 
                     # Rerun main flow with the new set of curves
                     CC_cc = CPCContainer(new_curves)
-                    O = CPCArbOptimizer(CC_cc)
+                    O = MargPOptimizer(CC_cc)
                     r = O.margp_optimizer(src_token)
                     profit_src = -r.result
                     trade_instructions_df = r.trade_instructions(O.TIF_DFAGGR)
                     trade_instructions_dic = r.trade_instructions(O.TIF_DICTS)
                     trade_instructions = r.trade_instructions()
             except Exception as e:
                 continue
```

### Comparing `fastlane_bot-2.2.0/fastlane_bot/modes/triangle_single.py` & `fastlane_bot-2.3.0/fastlane_bot/modes/triangle_single.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 (c) Copyright Bprotocol foundation 2023.
 Licensed under MIT
 """
 from typing import Union, List, Tuple, Any
 
 from fastlane_bot.modes.base_triangle import ArbitrageFinderTriangleBase
 from fastlane_bot.tools.cpc import CPCContainer
-from fastlane_bot.tools.optimizer import CPCArbOptimizer
+from fastlane_bot.tools.optimizer import MargPOptimizer
 
 
 class ArbitrageFinderTriangleSingle(ArbitrageFinderTriangleBase):
     """
     Triangle single arbitrage finder mode
     """
 
@@ -34,15 +34,15 @@
 
         # Check each source token and miniverse combination
         for src_token, miniverse in combos:
             r = None
 
             # Instantiate the container and optimizer objects
             CC_cc = CPCContainer(miniverse)
-            O = CPCArbOptimizer(CC_cc)
+            O = MargPOptimizer(CC_cc)
 
             try:
                 # Perform the optimization
                 r = O.margp_optimizer(src_token)
 
                 # Get the profit in the source token
                 profit_src = -r.result
```

### Comparing `fastlane_bot-2.2.0/fastlane_bot/modes/triangle_single_bancor3.py` & `fastlane_bot-2.3.0/fastlane_bot/modes/triangle_single_bancor3.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under MIT
 """
 import math
 from typing import Union, List, Tuple, Any, Iterable
 
 from fastlane_bot.modes.base_triangle import ArbitrageFinderTriangleBase
 from fastlane_bot.tools.cpc import CPCContainer, T, ConstantProductCurve
-from fastlane_bot.tools.optimizer import CPCArbOptimizer
+from fastlane_bot.tools.optimizer import MargPOptimizer
 
 
 class ArbitrageFinderTriangleSingleBancor3(ArbitrageFinderTriangleBase):
     """
     Bancor V3 triangular arbitrage finder mode
     """
 
@@ -291,15 +291,15 @@
         tuple
             Tuple of profit, trade instructions, trade instructions dataframe and trade instructions dictionary.
 
         """
 
         # Instantiate the container and optimizer objects
         CC_cc = CPCContainer(miniverse)
-        O = CPCArbOptimizer(CC_cc)
+        O = MargPOptimizer(CC_cc)
 
         # Perform the optimization
         r = O.margp_optimizer(src_token)
 
         # Get the profit in the source token
         profit_src = -r.result
```

### Comparing `fastlane_bot-2.2.0/fastlane_bot/testing.py` & `fastlane_bot-2.3.0/fastlane_bot/testing.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/tools/arbgraphs.py` & `fastlane_bot-2.3.0/fastlane_bot/tools/arbgraphs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 (c) Copyright Bprotocol foundation 2023. 
 Licensed under MIT
 
 NOTE: this class is not part of the API of the Carbon protocol, and you must expect breaking
 changes even in minor version updates. Use at your own risk.
 """
-__VERSION__ = "2.1"
-__DATE__ = "16/Apr/2023"
+__VERSION__ = "2.2"
+__DATE__ = "09/May/2023"
 
 from dataclasses import dataclass, field, asdict, astuple, InitVar
 from .simplepair import SimplePair as Pair
 import networkx as nx
 import numpy as np
 import matplotlib.pyplot as plt
 import pandas as pd
@@ -1599,25 +1599,31 @@
         return self.degree(inout=self.OUTDEGREE, as_matrix=as_matrix)
 
     PLOT_DEFAULTS = {
         "directed": True,
         "labels": True,
         "edge_labels": False,
         "node_color": "lightblue",
+        "node_size": 200,
         "show": True,
+        "font_size": 12,
+        "font_color": "k",
     }
 
     def plot(self, **params):
         """
         plot the graph
 
         :directed:      if True (default), plot a directed graph, otherwise undirected
         :labels:        if True (default), plot node labels
         :edge_labels:   if True (default), plot edge labels
-        :node_color:    color of the nodes (default: "lightblue")
+        :node_color:    node color (default: "lightblue")
+        :node_size:     node size (default: 200)
+        :font_size:     font size (default: 12)
+        :font_color:    font color (default: "k")
         :show:          if True (default), show the plot
         :rnone:         if True, returns None, otherwise returns self
         """
 
         p = lambda name: params.get(name, self.PLOT_DEFAULTS.get(name))
 
         G = self.as_graph(directed=p("directed"))
@@ -1626,14 +1632,17 @@
         # pos = nx.spring_layout(G) # works only in 2.6.3+
         nx.draw(
             G,
             pos,
             with_labels=p("labels"),
             labels=nx.get_node_attributes(G, "label"),
             node_color=p("node_color"),
+            node_size=p("node_size"),
+            font_size=p("font_size"),
+            font_color=p("font_color"),
         )
 
         if p("edge_labels"):
             edge_labels = nx.get_edge_attributes(G, "label")
             nx.draw_networkx_edge_labels(G, pos, edge_labels=edge_labels)
 
         if p("show"):
```

### Comparing `fastlane_bot-2.2.0/fastlane_bot/tools/cpc.py` & `fastlane_bot-2.3.0/fastlane_bot/tools/cpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,32 @@
 
 (c) Copyright Bprotocol foundation 2023. 
 Licensed under MIT
 
 NOTE: this class is not part of the API of the Carbon protocol, and you must expect breaking
 changes even in minor version updates. Use at your own risk.
 """
-__VERSION__ = "2.10.1"
-__DATE__ = "07/May/2023"
+__VERSION__ = "2.14"
+__DATE__ = "23/May/2023"
 
 from dataclasses import dataclass, field, asdict, InitVar
 from .simplepair import SimplePair as Pair
 from . import tokenscale as ts
 import random
 from math import sqrt
 import numpy as np
 import pandas as pd
 import json
 from matplotlib import pyplot as plt
 from .params import Params
-import itertools
+import itertools as it
+import collections as cl
 from sys import float_info
 from hashlib import md5 as digest
+import time
 
 try:
     dataclass_ = dataclass(frozen=True, kw_only=True)
 except:
     dataclass_ = dataclass(frozen=True)
 
 
@@ -340,173 +342,14 @@
     "vBNT-7f94",
     "wMEMO-af57",
     "wOXEN-bcc5",
     "wPPC-2958",
 }
 
 
-
-# @dataclass
-# class Pair:
-#     """
-#     a pair in notation TKNB/TKNQ; can also be provided as list
-#     """
-
-#     tknb: str = field(init=False)
-#     tknq: str = field(init=False)
-#     pair: InitVar[str] = None
-
-#     def __post_init__(self, pair):
-#         if isinstance(pair, CPCContainer.Pair):
-#             self.tknb = pair.tknb
-#             self.tknq = pair.tknq
-#         elif isinstance(pair, str):
-#             self.tknb, self.tknq = pair.split("/")
-#         elif pair is False:
-#             # used in alternative constructors
-#             pass
-#         else:
-#             try:
-#                 self.tknb, self.tknq = pair
-#             except:
-#                 raise ValueError(f"pair must be a string or list of two strings {pair}")
-
-#     @classmethod
-#     def from_tokens(cls, tknb, tknq):
-#         pair = cls(False)
-#         pair.tknb = tknb
-#         pair.tknq = tknq
-#         return pair
-
-#     def __str__(self):
-#         return f"{self.tknb}/{self.tknq}"
-
-#     @property
-#     def pair(self):
-#         """string representation of the pair"""
-#         return str(self)
-
-#     @property
-#     def pairt(self):
-#         """tuple representation of the pair"""
-#         return (self.tknb, self.tknq)
-
-#     @property
-#     def pairr(self):
-#         """returns the reversed pair"""
-#         return f"{self.tknq}/{self.tknb}"
-
-#     @property
-#     def pairrt(self):
-#         """tuple representation of the reverse pair"""
-#         return (self.tknq, self.tknb)
-
-#     @staticmethod
-#     def prettify_tkn(tkn):
-#         """returns a prettified token name"""
-#         return tkn.split("-")[0]
-
-#     @staticmethod
-#     def prettify_pair(pair):
-#         """returns a prettified pair name"""
-#         return "/".join(Pair.prettify_tkn(tkn) for tkn in pair.split("/"))
-
-#     @property
-#     def tknx(self):
-#         return self.tknb
-
-#     @property
-#     def tkny(self):
-#         return self.tknq
-
-#     @property
-#     def tknbp(self):
-#         return self.prettify_tkn(self.tknb)
-
-#     @property
-#     def tknqp(self):
-#         return self.prettify_tkn(self.tknq)
-
-#     @property
-#     def tknxp(self):
-#         return self.prettify_tkn(self.tknx)
-
-#     @property
-#     def tknyp(self):
-#         return self.prettify_tkn(self.tkny)
-
-#     def other(self, tkn):
-#         assert tkn in self.pairt, f"token not in pair{self.pair} {tkn}"
-#         return self.tknq if tkn == self.tknb else self.tknb
-
-#     def otherp(self, tkn):
-#         return self.prettify_tkn(self.other(tkn))
-
-#     NUMERAIRE_TOKENS = {
-#         tkn: i
-#         for i, tkn in enumerate(
-#             [
-#                 "USDC",
-#                 "USDT",
-#                 "DAI",
-#                 "TUSD",
-#                 "BUSD",
-#                 "PAX",
-#                 "GUSD",
-#                 "USDS",
-#                 "sUSD",
-#                 "mUSD",
-#                 "HUSD",
-#                 "USDN",
-#                 "USDP",
-#                 "USDQ",
-#                 "ETH",
-#                 "WETH",
-#                 "WBTC",
-#                 "BTC",
-#             ]
-#         )
-#     }
-
-#     @property
-#     def isprimary(self):
-#         """whether the representation is primary or secondary"""
-#         tknqix = self.NUMERAIRE_TOKENS.get(self.tknqp, 1e10)
-#         tknbix = self.NUMERAIRE_TOKENS.get(self.tknbp, 1e10)
-#         if tknqix == tknbix:
-#             return self.tknb < self.tknq
-#         return tknqix < tknbix
-
-#     def primary_price(self, p):
-#         """returns the primary price (p if primary, 1/p if secondary)"""
-#         return p if self.isprimary else 1 / p
-
-#     pp = primary_price
-
-#     @property
-#     def primary(self):
-#         """returns the primary pair"""
-#         return self.pair if self.isprimary else self.pairr
-
-#     @property
-#     def secondary(self):
-#         """returns the secondary pair"""
-#         return self.pairr if self.isprimary else self.pair
-
-#     @classmethod
-#     def wrap(cls, pairlist):
-#         """wraps a list of strings into Pairs"""
-#         return tuple(cls(p) for p in pairlist)
-
-#     @classmethod
-#     def unwrap(cls, pairlist):
-#         """unwraps a list of Pairs into strings"""
-#         return tuple(str(p) for p in pairlist)
-
-
 @dataclass_
 class ConstantProductCurve:
     """
     represents a, potentially levered, constant product curve
 
     :k:        pool constant k = xy [x=k/y, y=k/x]
     :x:        (virtual) pool state x (virtual number of base tokens for sale)
@@ -526,24 +369,26 @@
     __DATE__ = __DATE__
 
     k: float
     x: float
     x_act: float = None
     y_act: float = None
     pair: str = None
-    cid: any = None
+    cid: str = None
     fee: float = None
     descr: str = None
     constr: str = field(default=None, repr=True, compare=False, hash=False)
     params: AttrDict = field(default=None, repr=True, compare=False, hash=False)
 
     def __post_init__(self):
 
         if self.constr is None:
             super().__setattr__("constr", "default")
+            
+        super().__setattr__("cid", str(self.cid))   
 
         if self.params is None:
             super().__setattr__("params", AttrDict())
         elif isinstance(self.params, str):
             data = json.loads(self.params.replace("'", '"'))
             super().__setattr__("params", AttrDict(data))
         elif isinstance(self.params, dict):
@@ -586,14 +431,19 @@
         for field in fieldl:
             try:
                 val = val[field]
             except KeyError:
                 return defaultval
         return val
 
+    @property
+    def cid0(self):
+        "short cid [last 8 characters]"
+        return self.cid[-8:]
+    
     TOKENSCALE = ts.TokenScale1Data
     # default token scale object is the trivial scale (everything one)
     # change this to a different scale object be creating a derived class
 
     def set_tokenscale(self, tokenscale):
         """sets the tokenscale object (returns self)"""
         # print("setting tokenscale", self.cid, tokenscale)
@@ -1139,22 +989,27 @@
     tknyp = tknqp
 
     @property
     def pairp(self):
         """prettified pair"""
         return f"{self.tknbp}/{self.tknqp}"
 
-    @property
     def description(self):
         "description of the pool"
-        s1 = f"tknx = {self.x_act} [virtual: {self.x}] {self.tknx}"
-        s2 = f"tkny = {self.y_act} [virtual: {self.y}] {self.tkny}"
-        s3 = f"p    = {self.p} [min={self.p_min}, max={self.p_max}] {self.tknq} per {self.tknb}"
-        s4 = f"fee  = {self.fee}, cid = {self.cid}, descr = {self.descr}"
-        return "\n".join([s1, s2, s3, s4])
+        s = ""
+        s += f"cid      = {self.cid0} [{self.cid}]\n"
+        s += f"primary  = {Pair.n(self.pairo.primary)} [{self.pairo.primary}]\n"
+        s += f"pp       = {self.pp:,.6f} {self.pairo.pp_convention}\n"
+        s += f"pair     = {Pair.n(self.pair)} [{self.pair}]\n"
+        s += f"tknx     = {self.x_act:20,.6f} {self.tknx:10} [virtual: {self.x:20,.3f}]\n"
+        s += f"tkny     = {self.y_act:20,.6f} {self.tkny:10} [virtual: {self.y:20,.3f}]\n"
+        s += f"p        = {self.p} [min={self.p_min}, max={self.p_max}] {self.tknq} per {self.tknb}\n"
+        s += f"fee      = {self.fee}\n"
+        s += f"descr    = {self.descr}\n"
+        return s
 
     @property
     def y(self):
         "(virtual) pool state x (virtual number of base tokens for sale)"
         if self.k == 0:
             return 0
         return self.k / self.x
@@ -1178,14 +1033,22 @@
                 result += f" @ {self.primaryp(withconvention=True)}"
             return result
         if withprice:
             return result, self.primaryp()
         else:
             return result
     
+    def buy(self):
+        """returns 'b' if the curve buys the primary token, '' otherwise"""
+        return self.buysell(verbose=False, withprice=False).replace("s", "")
+    
+    def sell(self):
+        """returns 's' if the curve sells the primary token, '' otherwise"""
+        return self.buysell(verbose=False, withprice=False).replace("b", "")
+        
     ITM_THRESHOLDPC = 0.01
     @classmethod
     def itm0(cls, bsp1, bsp2, *, thresholdpc=None):
         """
         whether or not two positions are in the money against each other
 
         :bsp1:          first position ("bs", price) [from buysell]
@@ -1256,17 +1119,22 @@
 
     def p_convention(self):
         """price convention for p (dy/dx)"""
         return f"{self.tknyp} per {self.tknxp}"
     
     @property
     def primary(self):
-        "alias for self.pairo.primary [pair]"
+        "alias for self.pairo.primary"
         return self.pairo.primary
     
+    @property
+    def isprimary(self):
+        "alias for self.pairo.isprimary"
+        return self.pairo.isprimary
+    
     def primaryp(self, *, withconvention=False):
         "pool price in the native quote of the curve Pair object"
         price = self.pairo.pp(self.p)
         if not withconvention:
             return price
         return f"{price:.2f} {self.pairo.pp_convention}"     
     
@@ -1332,23 +1200,35 @@
     @property
     def p_max(self):
         "maximum pool price (in dy/dx; None if unlimited) = y_max/x_min"
         if not self.x_min is None and self.x_min > 0:
             return self.y_max / self.x_min
         else:
             return None
-
+        
+    def p_max_primary(self, swap=True):
+        "p_max in the native quote of the curve Pair object (swap=True: p_min)"
+        p = self.p_max if not (swap and not self.isprimary) else self.p_min
+        if p is None: return None
+        return p if self.isprimary else 1/p
+    
     @property
     def p_min(self):
         "minimum pool price (in dy/dx; None if unlimited) = y_min/x_max"
         if not self.x_max is None and self.x_max > 0:
             return self.y_min / self.x_max
         else:
             return None
-
+    
+    def p_min_primary(self, swap=True):
+        "p_min in the native quote of the curve Pair object (swap=True: p_max)"
+        p = self.p_min if not (swap and not self.isprimary) else self.p_max
+        if p is None: return None
+        return p if self.isprimary else 1/p
+    
     def format(self, *, heading=False, formatid=None):
         """returns info about the curve as a formatted string"""
         if formatid is None:
             formatid = 0
         assert formatid in [0], "only formatid in [0] is supported"
         c = self
         cid = str(c.cid)[-10:]
@@ -1625,14 +1505,53 @@
         """returns price of tknb in tknq (tknb per tknq)"""
         pairo = Pair.from_tokens(tknb, tknq)
         curves = self.curves_by_primary_pair.get(pairo.primary, None)
         if curves is None:
             return None
         pp = sum(c.pp for c in curves) / len(curves)
         return pp if pairo.isprimary else 1 / pp
+    
+    PR_TUPLE = "tuple"
+    PR_DICT = "dict"
+    PR_DF = "df"
+    def prices(self, result=None, *, inclpair=None, primary=None):
+        """
+        returns tuple or dictionary of the prices of all curves in the container
+
+        :primary:       if True (default), returns the price quoted in the convention of the primary pair
+        :inclpair:      if True, includes the pair in the dictionary
+        :result:        what result to return (PR_TUPLE, PR_DICT, PR_DF)
+        """
+        if primary is None: primary = True
+        if inclpair is None: inclpair = True
+        if result is None: result = self.PR_DICT
+        price_g = ((
+                c.cid,
+                c.primaryp() if primary else c.p, 
+                c.pairo.primary if primary else c.pair
+            ) for c in self.curves
+        )
+        
+        if result == self.PR_TUPLE:
+            if inclpair:
+                return tuple(price_g)
+            else:
+                return tuple(r[1] for r in price_g)
+        
+        if result == self.PR_DICT:
+            if inclpair:
+                return {r[0]: (r[1], r[2]) for r in price_g}
+            else:
+                return {r[0]: r[1] for r in price_g}
+        
+        if result == self.PR_DF:
+            df = pd.DataFrame.from_records(price_g, columns=["cid", "price", "pair"])
+            df = df.set_index("cid")
+            return df
+        raise ValueError(f"unknown result type {result}")
 
     def __iadd__(self, other):
         """alias for  self.add"""
         return self.add(other)
 
     def __iter__(self):
         return iter(self.curves)
@@ -1676,14 +1595,27 @@
 
     tokens = tkns
 
     def tokens_s(self, curves=None):
         """returns set of all tokens used by the curves as a string"""
         return ",".join(sorted(self.tokens(curves)))
 
+    def token_count(self, asdict=False):
+        """
+        counts the number of times each token appears in the curves
+        """
+        tokens_l = (c.pair for c in self)
+        tokens_l = (t.split("/") for t in tokens_l)
+        tokens_l = (t for t in it.chain.from_iterable(tokens_l))
+        tokens_l = list(cl.Counter([t for t in tokens_l]).items())
+        tokens_l = sorted(tokens_l, key=lambda x: x[1], reverse=True)
+        if not asdict:
+            return tokens_l
+        return dict(tokens_l)
+    
     def pairs(self, *, standardize=True):
         """
         returns set of all pairs used by the curves
 
         :standardize:   if False, the pairs are returned as they are in the curves; eg if we have curves
                         for both ETH/USDT and USDT/ETH, both pairs will be returned; if True, only the
                         canonical pair will be returned
@@ -2049,38 +1981,48 @@
     def curveix(self, curve):
         """returns index of curve in container"""
         return self.curveix_by_curve.get(curve, None)
 
     def bycid(self, cid):
         """returns curve by cid"""
         return self.curves_by_cid.get(cid, None)
-
-    def bycids(self, include=None, *, exclude=None, asgenerator=None, ascc=None):
+    
+    def bycids(self, include=None, *, endswith=None, exclude=None, asgenerator=None, ascc=None):
         """
         returns curves by cids (as tuple, generator or CC object)
 
         :include:   list of cids to include, if None all cids are included
+        :endswith:  alternative to include, include all cids that end with this string
         :exclude:   list of cids to exclude, if None no cids are excluded
                     exclude beats include
         :returns:   tuple, generator or container object (default)
         """
+        if not include is None and not endswith is None:
+            raise ValueError(f"include and endswith cannot be used together")
         if exclude is None:
             exclude = set()
-        if include is None:
+        if include is None and endswith is None:
             result = (c for c in self if not c.cid in exclude)
         else:
-            result = (self.curves_by_cid[cid] for cid in include if not cid in exclude)
+            if not include is None:
+                result = (self.curves_by_cid[cid] for cid in include if not cid in exclude)
+            else:
+                result = (c for c in self if c.cid.endswith(endswith) and not c.cid in exclude)
         return self._convert(result, asgenerator=asgenerator, ascc=ascc)
 
+    def bycid0(self, cid0, **kwargs):
+        """alias for bycids(endswith=cid0)"""
+        return self.bycids(endswith=cid0, **kwargs)
+    
     def bypair(self, pair, *, directed=False, asgenerator=None, ascc=None):
         """returns all curves by (possibly directed) pair (as tuple, genator or CC object)"""
         result = (c for c in self if c.pair == pair)
         if not directed:
             pairr = "/".join(pair.split("/")[::-1])
-            result = itertools.chain(result, (c for c in self if c.pair == pairr))
+            result = it.chain(result, (c for c in self if c.pair == pairr))
         return self._convert(result, asgenerator=asgenerator, ascc=ascc)
 
     def bp(self, pair, *, directed=False, asgenerator=None, ascc=None):
         """alias for bypair by with directed=False for interactive use"""
         return self.bypair(pair, directed=directed, asgenerator=asgenerator, ascc=ascc)
 
     def bypairs(self, pairs=None, *, directed=False, asgenerator=None, ascc=None):
@@ -2101,30 +2043,34 @@
             if not directed:
                 rpairs = set(f"{q}/{b}" for b, q in (p.split("/") for p in pairs))
                 # print("[CC] bypairs: adding reverse pairs", rpairs)
                 pairs = pairs.union(rpairs)
             result = (c for c in self if c.pair in pairs)
         return self._convert(result, asgenerator=asgenerator, ascc=ascc)
 
-    def byparams(self, *, _asgenerator=None, _ascc=None, **params):
+    def byparams(self, *, _asgenerator=None, _ascc=None, _inv=False, **params):
         """
         returns all curves by params (as tuple, generator or CC object)
 
+        :_inv:      if True, returns all curves that do NOT match the params
         :params:    keyword arguments in the form param=value
         :returns:   tuple, generator or container object (default)
         """
         if not params:
             raise ValueError(f"no params given {params}")
         
         params_t = tuple(params.items())
         if len(params_t) > 1:
             raise NotImplementedError(f"currently only one param allowed {params}")
         
         pname, pvalue = params_t[0]
-        result = (c for c in self if c.P(pname) == pvalue)
+        if _inv:
+            result = (c for c in self if c.P(pname) != pvalue)
+        else:
+            result = (c for c in self if c.P(pname) == pvalue)
         return self._convert(result, asgenerator=_asgenerator, ascc=_ascc)
 
     def copy(self):
         """returns a copy of the container"""
         return self.bypairs(ascc=True)
 
     def bytknx(self, tknx, *, asgenerator=None, ascc=None):
@@ -2234,78 +2180,82 @@
             c for c in self if not c.at_boundary and c.tknq == tknq and c.tknb == tknb
         )
         rcrvs = (
             c for c in self if not c.at_boundary and c.tknb == tknq and c.tknq == tknb
         )
         crvs = ((c, c.p, c.k) for c in crvs)
         rcrvs = ((c, 1 / c.p, c.k) for c in rcrvs)
-        acurves = itertools.chain(crvs, rcrvs)
+        acurves = it.chain(crvs, rcrvs)
         if result == self.PE_CURVES:
             # return dict(curves=tuple(crvs), rcurves=tuple(rcrvs))
             return tuple(acurves)
         data = tuple((r[1], sqrt(r[2])) for r in acurves)
         if not len(data) > 0:
             if raiseonerror:
                 raise ValueError(f"no curves found for {tknq}/{tknb}")
             return None
         prices, weights = zip(*data)
         prices, weights = np.array(prices), np.array(weights)
         if result == self.PE_DATA:
             return prices, weights
         return float(np.average(prices, weights=weights))
 
-    TRIANGTOKENS = f"{T.USDC}, {T.USDT}, {T.DAI}, {T.WBTC}, {T.ETH}"
+    TRIANGTOKENS = f"{T.USDT}, {T.USDC}, {T.DAI}, {T.BNT}, {T.ETH}, {T.WBTC}"
 
     def price_estimates(
         self,
         *,
         tknqs=None,
         tknbs=None,
         triangulate=True,
         unwrapsingle=True,
         pairs=False,
+        stopatfirst=True,
         raiseonerror=True,
         verbose=False,
     ):
         """
         calculates prices estimates in the reference token as base token
 
         :tknqs:         list of quote tokens to calculate prices for
         :tknbs:         list of base tokens to calculate prices for
         :triangulate:   tokens used as intermediate token for triangulation; if True, a standard 
                         token list is used; if None or False, no triangulation
         :unwrapsingle:  if there is only one quote token, a 1-d array is returned
         :pairs:         if True, returns the slashpairs instead of the prices
         :raiseonerror:  if True, raise exception if no price can be calculated
+        :stopatfirst:   it True, stop at first triangulation match
         :verbose:       if True, print some progress
         :return:        np.array of prices (quote outer, base inner; quote per base)
         """
+        # NOTE: this code is relatively slow to compute, on the order of a few seconds
+        # for go through the entire token list; the likely reason is that it keeps reestablishing
+        # the CPCContainer objects whenever price_estimate is called; there may be a way to
+        # speed this up by smartly computing the container objects once and storing them 
+        # in a dictionary the is then passed to price_estimate.
+        start_time = time.time()
         assert not tknqs is None, "tknqs must be set"
         assert not tknbs is None, "tknbs must be set"
         if isinstance(tknqs, str):
             tknqs = [t.strip() for t in tknqs.split(",")]
         if isinstance(tknbs, str):
             tknbs = [t.strip() for t in tknbs.split(",")]
         # print(f"[price_estimates] tknqs [{len(tknqs)}], tknbs [{len(tknbs)}]")
         # print(f"[price_estimates] tknqs [{len(tknqs)}] = {tknqs} , tknbs [{len(tknbs)}]] = {tknbs} ")
+        resulttp = self.PE_PAIR if pairs else None
         result = np.array(
             [
                 [
-                    self.price_estimate(
-                        tknb=b,
-                        tknq=q,
-                        raiseonerror=False,
-                        result=self.PE_PAIR if pairs else None,
-                    )
+                    self.price_estimate(tknb=b, tknq=q, raiseonerror=False, result=resulttp)
                     for b in tknbs
-                ]
+                ] 
                 for q in tknqs
             ]
         )
-        
+        #print(f"[price_estimates] PAIRS [{time.time()-start_time:.2f}s]")
         flattened = result.flatten()
         nmissing = len([r for r in flattened if r is None])
         if verbose:
             print(f"[price_estimates] pair estimates: {len(flattened)-nmissing} found, {nmissing} missing")
             if nmissing > 0 and not triangulate:
                 print(f"[price_estimates] {nmissing} missing pairs may be triangulated, but triangulation disabled [{triangulate}]")
             if nmissing == 0 and triangulate:
@@ -2315,28 +2265,37 @@
             if triangulate is True:
                 triangulate = self.TRIANGTOKENS
             if isinstance(triangulate, str):
                 triangulate = [t.strip() for t in triangulate.split(",")]
             if verbose:
                 print("[price_estimates] triangulation tokens", triangulate)
             for ib, b in enumerate(tknbs):
+                #print(f"TOKENB={b:22} [{time.time()-start_time:.4f}s]")
                 for iq, q in enumerate(tknqs):
+                    #print(f" TOKENQ={q:21} [{time.time()-start_time:.4f}s]")
                     if result[iq][ib] is None:
                         result1 = []
                         for tkn in triangulate:
+                            #print(f"  TKN={tkn:23} [{time.time()-start_time:.4f}s]")
                             #print(f"[price_estimates] triangulating tknb={b} tknq={q} via {tkn}")
                             b_tkn = self.price_estimate(tknb=b, tknq=tkn, raiseonerror=False)
                             q_tkn = self.price_estimate(tknb=q, tknq=tkn, raiseonerror=False)
                             #print(f"[price_estimates] triangulating {b}/{tkn} = {b_tkn}, {q}/{tkn} = {q_tkn}")
                             if not b_tkn is None and not q_tkn is None:
-                                #print(f"[price_estimates] triangulating {b}/{q} = {b_tkn/q_tkn}")
+                                if verbose:
+                                    print(f"[price_estimates] triangulated {b}/{q} via {tkn} [={b_tkn/q_tkn}]")
                                 result1 += [b_tkn / q_tkn]
-                        result1 = np.mean(result1) if len(result1) > 0 else None
-                        #print(f"[price_estimates] final result {b}/{q} = {result1}")
-                        result[iq][ib] = result1
+                                if stopatfirst:
+                                    #print(f"[price_estimates] stop at first")
+                                    break
+                                # else:
+                                #     print(f"[price_estimates] continue {stopatfirst}")
+                        result2 = np.mean(result1) if len(result1) > 0 else None
+                        #print(f"[price_estimates] final result {b}/{q} = {result2} [{len(result1)}]")
+                        result[iq][ib] = result2
         
         flattened = result.flatten()
         nmissing = len([r for r in flattened if r is None])
         if verbose:
             if nmissing > 0:
                 missing = {
                     f"{b}/{q}"
@@ -2359,14 +2318,15 @@
                 raise ValueError(
                     f"no price found for {len(missing)} pairs",
                     result,
                     missing,
                     len(missing),
                 )
 
+        #print(f"[price_estimates] DONE [{time.time()-start_time:.2f}s]")
         if unwrapsingle and len(tknqs) == 1:
             result = result[0]
         return result
 
     @dataclass
     class TokenTableEntry:
         """
```

### Comparing `fastlane_bot-2.2.0/fastlane_bot/tools/params.py` & `fastlane_bot-2.3.0/fastlane_bot/tools/params.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/tools/simplepair.py` & `fastlane_bot-2.3.0/fastlane_bot/tools/simplepair.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 simple representation of a pair of tokens, used by cpc and arbgraph
 
 (c) Copyright Bprotocol foundation 2023. 
 Licensed under MIT
 """
-__VERSION__ = "2.0"
-__DATE__ = "5/May/2023"
+__VERSION__ = "2.1"
+__DATE__ = "18/May/2023"
 
 from dataclasses import dataclass, field, asdict, InitVar
 
 
 @dataclass
 class SimplePair:
     """
@@ -89,14 +89,15 @@
                 "USDS",
                 "sUSD",
                 "mUSD",
                 "HUSD",
                 "USDN",
                 "USDP",
                 "USDQ",
+                "BNT",
                 "ETH",
                 "WETH",
                 "WBTC",
                 "BTC",
             ]
         )
     }
```

### Comparing `fastlane_bot-2.2.0/fastlane_bot/tools/tokenscale.py` & `fastlane_bot-2.3.0/fastlane_bot/tools/tokenscale.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/tools/univ3calc_DELETE.py` & `fastlane_bot-2.3.0/fastlane_bot/tools/univ3calc_DELETE.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot/utils.py` & `fastlane_bot-2.3.0/fastlane_bot/utils.py`

 * *Files identical despite different names*

### Comparing `fastlane_bot-2.2.0/fastlane_bot.egg-info/PKG-INFO` & `fastlane_bot-2.3.0/fastlane_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlane-bot
-Version: 2.2.0
+Version: 2.3.0
 Summary: Carbon Arbitrage Bot, an open-source arbitrage protocol, allows any user to perform arbitrage between Bancor ecosystem protocols and external exchanges and redirect arbitrage profits back to the protocol.
 Home-page: https://github.com/bancorprotocol/carbon-bot
 Author: Bancor Network
 Author-email: mike@bancor.network
 Requires-Python: >= 3.8, != 3.11.*
 Description-Content-Type: text/markdown
 Provides-Extra: complete
```

### Comparing `fastlane_bot-2.2.0/fastlane_bot.egg-info/SOURCES.txt` & `fastlane_bot-2.3.0/fastlane_bot.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -71,16 +71,46 @@
 fastlane_bot/modes/pairwise_single.py
 fastlane_bot/modes/triangle_bancor_v3_two_hop.py
 fastlane_bot/modes/triangle_multi.py
 fastlane_bot/modes/triangle_single.py
 fastlane_bot/modes/triangle_single_bancor3.py
 fastlane_bot/modes/tests/__init__.py
 fastlane_bot/modes/tests/test_pairwise_single.py
+fastlane_bot/tests/__init__.py
+fastlane_bot/tests/nbtest/__init__.py
+fastlane_bot/tests/nbtest/test_000_Template.py
+fastlane_bot/tests/nbtest/test_002_CPCandOptimizer.py
+fastlane_bot/tests/nbtest/test_003_Serialization.py
+fastlane_bot/tests/nbtest/test_004_GraphCode.py
+fastlane_bot/tests/nbtest/test_005_Uniswap.py
+fastlane_bot/tests/nbtest/test_007_NoneResult.py
+fastlane_bot/tests/nbtest/test_033_Pools.py
+fastlane_bot/tests/nbtest/test_034_Interface.py
+fastlane_bot/tests/nbtest/test_035_Utils.py
+fastlane_bot/tests/nbtest/test_036_Manager.py
+fastlane_bot/tests/nbtest/test_037_Exchanges.py
+fastlane_bot/tests/nbtest/test_038_TestBancorV3Mode.py
+fastlane_bot/tests/nbtest/test_039_TestMultiMode.py
+fastlane_bot/tests/nbtest/test_040_TestSingleMode.py
+fastlane_bot/tests/nbtest/test_042_TestBancorV3ModeTwoHop.py
+fastlane_bot/tests/nbtest/test_043_TestEmptyCarbonOrders.py
+fastlane_bot/tests/nbtest/test_047_Randomizer.py
+fastlane_bot/tests/nbtest/test_900_OptimizerDetailedSlow.py
+fastlane_bot/tests/nbtest/test_901_TestMultiTriangleModeSlow.py
+fastlane_bot/tests/nbtest/test_902_ValidatorSlow.py
 fastlane_bot/tools/__init__.py
 fastlane_bot/tools/analyzer.py
 fastlane_bot/tools/arbgraphs.py
 fastlane_bot/tools/cpc.py
-fastlane_bot/tools/optimizer.py
+fastlane_bot/tools/cryptocompare.py
+fastlane_bot/tools/noneresult.py
 fastlane_bot/tools/params.py
 fastlane_bot/tools/simplepair.py
 fastlane_bot/tools/tokenscale.py
-fastlane_bot/tools/univ3calc_DELETE.py
+fastlane_bot/tools/univ3calc_DELETE.py
+fastlane_bot/tools/optimizer/__init__.py
+fastlane_bot/tools/optimizer/base.py
+fastlane_bot/tools/optimizer/convexoptimizer.py
+fastlane_bot/tools/optimizer/cpcarboptimizer.py
+fastlane_bot/tools/optimizer/dcbase.py
+fastlane_bot/tools/optimizer/margpoptimizer.py
+fastlane_bot/tools/optimizer/simpleoptimizer.py
```

### Comparing `fastlane_bot-2.2.0/setup.py` & `fastlane_bot-2.3.0/setup.py`

 * *Files identical despite different names*

