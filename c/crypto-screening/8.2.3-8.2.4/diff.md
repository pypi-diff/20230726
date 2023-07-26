# Comparing `tmp/crypto-screening-8.2.3.tar.gz` & `tmp/crypto-screening-8.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-8.2.3.tar", last modified: Tue Jul 25 10:48:19 2023, max compression
+gzip compressed data, was "crypto-screening-8.2.4.tar", last modified: Wed Jul 26 10:57:23 2023, max compression
```

## Comparing `crypto-screening-8.2.3.tar` & `crypto-screening-8.2.4.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 10:48:19.266373 crypto-screening-8.2.3/
--rw-rw-rw-   0        0        0      196 2023-07-25 10:48:18.000000 crypto-screening-8.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-25 10:48:19.266373 crypto-screening-8.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.2.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.2.3/build.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:48:19.026556 crypto-screening-8.2.3/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-25 10:48:19.063571 crypto-screening-8.2.3/crypto_screening/collect/
--rw-rw-rw-   0        0        0    16957 2023-07-24 18:32:29.000000 crypto-screening-8.2.3/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     5005 2023-07-24 18:29:23.000000 crypto-screening-8.2.3/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:48:19.090734 crypto-screening-8.2.3/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.2.3/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.2.3/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.2.3/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.2.3/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:48:19.113706 crypto-screening-8.2.3/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.2.3/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24665 2023-07-24 09:29:05.000000 crypto-screening-8.2.3/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16516 2023-07-24 09:29:05.000000 crypto-screening-8.2.3/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21653 2023-07-24 09:29:05.000000 crypto-screening-8.2.3/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.2.3/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    17976 2023-07-24 18:15:45.000000 crypto-screening-8.2.3/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19569 2023-07-24 18:21:12.000000 crypto-screening-8.2.3/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-8.2.3/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.2.3/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-8.2.3/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:48:19.181740 crypto-screening-8.2.3/crypto_screening/screeners/
--rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.2.3/crypto_screening/screeners/__init__.py
--rw-rw-rw-   0        0        0    23312 2023-07-24 09:37:18.000000 crypto-screening-8.2.3/crypto_screening/screeners/base.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:48:19.205902 crypto-screening-8.2.3/crypto_screening/screeners/callbacks/
--rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.2.3/crypto_screening/screeners/callbacks/__init__.py
--rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.2.3/crypto_screening/screeners/callbacks/base.py
--rw-rw-rw-   0        0        0     4400 2023-07-24 09:29:05.000000 crypto-screening-8.2.3/crypto_screening/screeners/callbacks/database.py
--rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.2.3/crypto_screening/screeners/callbacks/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:48:19.226928 crypto-screening-8.2.3/crypto_screening/screeners/collectors/
--rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.2.3/crypto_screening/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     6271 2023-07-24 09:29:05.000000 crypto-screening-8.2.3/crypto_screening/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.2.3/crypto_screening/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.2.3/crypto_screening/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.2.3/crypto_screening/screeners/combined.py
--rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.2.3/crypto_screening/screeners/container.py
--rw-rw-rw-   0        0        0    10976 2023-07-24 09:29:05.000000 crypto-screening-8.2.3/crypto_screening/screeners/database.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:48:19.247405 crypto-screening-8.2.3/crypto_screening/screeners/foundation/
--rw-rw-rw-   0        0        0    10462 2023-07-24 09:37:33.000000 crypto-screening-8.2.3/crypto_screening/screeners/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.2.3/crypto_screening/screeners/foundation/protocols.py
--rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.2.3/crypto_screening/screeners/foundation/state.py
--rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.2.3/crypto_screening/screeners/foundation/waiting.py
--rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.2.3/crypto_screening/screeners/market.py
--rw-rw-rw-   0        0        0    22099 2023-07-24 09:38:59.000000 crypto-screening-8.2.3/crypto_screening/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    11814 2023-07-24 09:39:14.000000 crypto-screening-8.2.3/crypto_screening/screeners/orderbook.py
--rw-rw-rw-   0        0        0    11410 2023-07-24 09:39:34.000000 crypto-screening-8.2.3/crypto_screening/screeners/orders.py
--rw-rw-rw-   0        0        0    16982 2023-07-24 18:21:12.000000 crypto-screening-8.2.3/crypto_screening/screeners/recorder.py
--rw-rw-rw-   0        0        0    11479 2023-07-24 09:39:59.000000 crypto-screening-8.2.3/crypto_screening/screeners/trades.py
--rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.2.3/crypto_screening/screeners/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:48:18.996616 crypto-screening-8.2.3/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-07-25 10:48:19.251404 crypto-screening-8.2.3/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.2.3/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10353 2023-07-25 10:48:04.000000 crypto-screening-8.2.3/crypto_screening/symbols.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:48:19.265405 crypto-screening-8.2.3/crypto_screening/utils/
--rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.2.3/crypto_screening/utils/base.py
--rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.2.3/crypto_screening/utils/process.py
--rw-rw-rw-   0        0        0     3485 2023-07-24 18:15:45.000000 crypto-screening-8.2.3/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-25 10:48:19.040577 crypto-screening-8.2.3/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-25 10:48:18.000000 crypto-screening-8.2.3/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2145 2023-07-25 10:48:18.000000 crypto-screening-8.2.3/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 10:48:18.000000 crypto-screening-8.2.3/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-25 10:48:18.000000 crypto-screening-8.2.3/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-25 10:48:18.000000 crypto-screening-8.2.3/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-25 10:48:18.000000 crypto-screening-8.2.3/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.2.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.2.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 10:48:19.266373 crypto-screening-8.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-25 10:48:12.000000 crypto-screening-8.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.104889 crypto-screening-8.2.4/
+-rw-rw-rw-   0        0        0      196 2023-07-26 10:57:21.000000 crypto-screening-8.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-26 10:57:23.103890 crypto-screening-8.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.2.4/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.2.4/build.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:22.933188 crypto-screening-8.2.4/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:22.965495 crypto-screening-8.2.4/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    16957 2023-07-24 18:32:29.000000 crypto-screening-8.2.4/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     5005 2023-07-24 18:29:23.000000 crypto-screening-8.2.4/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:22.994465 crypto-screening-8.2.4/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.2.4/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.2.4/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.016529 crypto-screening-8.2.4/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.2.4/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24665 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    16516 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21653 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    18731 2023-07-26 10:53:46.000000 crypto-screening-8.2.4/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    19569 2023-07-24 18:21:12.000000 crypto-screening-8.2.4/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    14801 2023-07-20 08:05:34.000000 crypto-screening-8.2.4/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.2.4/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-8.2.4/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.056038 crypto-screening-8.2.4/crypto_screening/screeners/
+-rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.2.4/crypto_screening/screeners/__init__.py
+-rw-rw-rw-   0        0        0    23312 2023-07-24 09:37:18.000000 crypto-screening-8.2.4/crypto_screening/screeners/base.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.067038 crypto-screening-8.2.4/crypto_screening/screeners/callbacks/
+-rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.2.4/crypto_screening/screeners/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.2.4/crypto_screening/screeners/callbacks/base.py
+-rw-rw-rw-   0        0        0     4400 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/screeners/callbacks/database.py
+-rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/screeners/callbacks/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.078038 crypto-screening-8.2.4/crypto_screening/screeners/collectors/
+-rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.2.4/crypto_screening/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6271 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.2.4/crypto_screening/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.2.4/crypto_screening/screeners/combined.py
+-rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.2.4/crypto_screening/screeners/container.py
+-rw-rw-rw-   0        0        0    10976 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/screeners/database.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.086038 crypto-screening-8.2.4/crypto_screening/screeners/foundation/
+-rw-rw-rw-   0        0        0    10462 2023-07-24 09:37:33.000000 crypto-screening-8.2.4/crypto_screening/screeners/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.2.4/crypto_screening/screeners/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.2.4/crypto_screening/screeners/foundation/state.py
+-rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.2.4/crypto_screening/screeners/foundation/waiting.py
+-rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.2.4/crypto_screening/screeners/market.py
+-rw-rw-rw-   0        0        0    22099 2023-07-24 09:38:59.000000 crypto-screening-8.2.4/crypto_screening/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    11814 2023-07-24 09:39:14.000000 crypto-screening-8.2.4/crypto_screening/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    11410 2023-07-24 09:39:34.000000 crypto-screening-8.2.4/crypto_screening/screeners/orders.py
+-rw-rw-rw-   0        0        0    16982 2023-07-24 18:21:12.000000 crypto-screening-8.2.4/crypto_screening/screeners/recorder.py
+-rw-rw-rw-   0        0        0    11479 2023-07-24 09:39:59.000000 crypto-screening-8.2.4/crypto_screening/screeners/trades.py
+-rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.2.4/crypto_screening/screeners/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:22.898298 crypto-screening-8.2.4/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.091069 crypto-screening-8.2.4/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.2.4/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10353 2023-07-25 10:48:04.000000 crypto-screening-8.2.4/crypto_screening/symbols.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:23.102888 crypto-screening-8.2.4/crypto_screening/utils/
+-rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.2.4/crypto_screening/utils/base.py
+-rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.2.4/crypto_screening/utils/process.py
+-rw-rw-rw-   0        0        0     3485 2023-07-24 18:15:45.000000 crypto-screening-8.2.4/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:22.947189 crypto-screening-8.2.4/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-26 10:57:22.000000 crypto-screening-8.2.4/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2145 2023-07-26 10:57:22.000000 crypto-screening-8.2.4/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 10:57:22.000000 crypto-screening-8.2.4/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-26 10:57:22.000000 crypto-screening-8.2.4/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 10:57:22.000000 crypto-screening-8.2.4/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-26 10:57:21.000000 crypto-screening-8.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.2.4/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.2.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 10:57:23.104889 crypto-screening-8.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-07-26 10:57:18.000000 crypto-screening-8.2.4/setup.py
```

### Comparing `crypto-screening-8.2.3/PKG-INFO` & `crypto-screening-8.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.2.3
+Version: 8.2.4
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.2.3/README.md` & `crypto-screening-8.2.4/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/build.py` & `crypto-screening-8.2.4/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/collect/assets.py` & `crypto-screening-8.2.4/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/collect/exchanges.py` & `crypto-screening-8.2.4/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-8.2.4/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/collect/market/orderbook.py` & `crypto-screening-8.2.4/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/collect/market/orders.py` & `crypto-screening-8.2.4/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/collect/market/state/assets.py` & `crypto-screening-8.2.4/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/collect/market/state/base.py` & `crypto-screening-8.2.4/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-8.2.4/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/collect/market/trades.py` & `crypto-screening-8.2.4/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/collect/screeners.py` & `crypto-screening-8.2.4/crypto_screening/collect/screeners.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,29 @@
 __all__ = [
     "matching_screener_signatures",
     "matching_screener_pair",
     "matching_screener_pairs",
     "MarketScreenerSignature",
     "find_screeners",
     "structure_screeners",
-    "live_nonempty_screeners",
+    "running_nonempty_screeners",
     "remove_empty_screeners",
     "screeners_exchanges_symbols",
     "structure_exchanges_symbols_screeners",
     "structure_exchanges_symbols_screener",
     "gather_screeners",
     "exchanges_symbols_screeners",
     "screeners_to_multiple_symbols_screeners",
     "screeners_to_assets_screeners",
     "screeners_to_symbols_screeners",
     "screeners_to_multiple_assets_screeners",
     "screeners_to_multiple_assets_datasets",
     "screeners_to_multiple_symbols_datasets",
-    "nonempty_screeners"
+    "nonempty_screeners",
+    "running_screeners"
 ]
 
 AssetMatches = Iterable[Iterable[str]]
 
 def matching_screener_pair(
         screener1: BaseScreener,
         screener2: BaseScreener, /, *,
@@ -203,15 +204,15 @@
                 (len(screener.market) > 0) and
                 isinstance(screener, BaseScreener)
             )
         )
     }
 # end nonempty_screeners
 
-def live_nonempty_screeners(
+def running_nonempty_screeners(
         screeners: Iterable[Union[BaseScreener, BaseMarketScreener]]
 ) -> Set[Union[BaseScreener, BaseMarketScreener]]:
     """
     Returns a list of all the live create_screeners.
 
     :param screeners: The create_screeners to search from.
 
@@ -219,24 +220,50 @@
     """
 
     return {
         screener for screener in screeners
         if (
             (
                 isinstance(screener, BaseMarketScreener) and
-                live_nonempty_screeners(screener.screeners)
+                running_nonempty_screeners(screener.screeners)
             ) or
             (
                 screener.screening and
                 (len(screener.market) > 0) and
                 isinstance(screener, BaseScreener)
             )
         )
     }
-# end live_nonempty_screeners
+# end running_nonempty_screeners
+
+def running_screeners(
+    screeners: Iterable[Union[BaseScreener, BaseMarketScreener]]
+) -> Set[Union[BaseScreener, BaseMarketScreener]]:
+    """
+    Returns a list of all the live create_screeners.
+
+    :param screeners: The create_screeners to search from.
+
+    :return: A list the live create_screeners.
+    """
+
+    return {
+        screener for screener in screeners
+        if (
+            (
+                isinstance(screener, BaseMarketScreener) and
+                running_screeners(screener.screeners)
+            ) or
+            (
+                screener.screening and
+                isinstance(screener, BaseScreener)
+            )
+        )
+    }
+# end running_screeners
 
 def structure_screeners(
         screeners: Iterable[BaseScreener]
 ) -> Dict[str, Dict[str, Set[BaseScreener]]]:
     """
     Structures the screener objects by exchanges and symbols
```

### Comparing `crypto-screening-8.2.3/crypto_screening/collect/symbols.py` & `crypto-screening-8.2.4/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/dataset.py` & `crypto-screening-8.2.4/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/exchanges.py` & `crypto-screening-8.2.4/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/interval.py` & `crypto-screening-8.2.4/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/base.py` & `crypto-screening-8.2.4/crypto_screening/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/callbacks/base.py` & `crypto-screening-8.2.4/crypto_screening/screeners/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/callbacks/database.py` & `crypto-screening-8.2.4/crypto_screening/screeners/callbacks/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/callbacks/sockets.py` & `crypto-screening-8.2.4/crypto_screening/screeners/callbacks/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/collectors/base.py` & `crypto-screening-8.2.4/crypto_screening/screeners/collectors/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/collectors/database.py` & `crypto-screening-8.2.4/crypto_screening/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/collectors/sockets.py` & `crypto-screening-8.2.4/crypto_screening/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/combined.py` & `crypto-screening-8.2.4/crypto_screening/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/container.py` & `crypto-screening-8.2.4/crypto_screening/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/database.py` & `crypto-screening-8.2.4/crypto_screening/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/foundation/data.py` & `crypto-screening-8.2.4/crypto_screening/screeners/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/foundation/protocols.py` & `crypto-screening-8.2.4/crypto_screening/screeners/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/foundation/state.py` & `crypto-screening-8.2.4/crypto_screening/screeners/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/foundation/waiting.py` & `crypto-screening-8.2.4/crypto_screening/screeners/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/market.py` & `crypto-screening-8.2.4/crypto_screening/screeners/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/ohlcv.py` & `crypto-screening-8.2.4/crypto_screening/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/orderbook.py` & `crypto-screening-8.2.4/crypto_screening/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/orders.py` & `crypto-screening-8.2.4/crypto_screening/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/recorder.py` & `crypto-screening-8.2.4/crypto_screening/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/trades.py` & `crypto-screening-8.2.4/crypto_screening/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/screeners/waiting.py` & `crypto-screening-8.2.4/crypto_screening/screeners/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-8.2.4/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/symbols.py` & `crypto-screening-8.2.4/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/utils/base.py` & `crypto-screening-8.2.4/crypto_screening/utils/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/utils/process.py` & `crypto-screening-8.2.4/crypto_screening/utils/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening/validate.py` & `crypto-screening-8.2.4/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-8.2.4/crypto_screening.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.2.3
+Version: 8.2.4
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.2.3/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-8.2.4/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.3/pyproject.toml` & `crypto-screening-8.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '8.2.3'
+version = '8.2.4'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-8.2.3/setup.py` & `crypto-screening-8.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "crypto_screening/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='8.2.3',
+        version='8.2.4',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

