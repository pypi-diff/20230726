# Comparing `tmp/eth-tester-0.9.0b2.tar.gz` & `tmp/eth-tester-0.9.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-tester-0.9.0b2.tar", last modified: Thu Jun 29 16:33:27 2023, max compression
+gzip compressed data, was "eth-tester-0.9.1b1.tar", last modified: Wed Jul 26 16:27:58 2023, max compression
```

## Comparing `eth-tester-0.9.0b2.tar` & `eth-tester-0.9.1b1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.569672 eth-tester-0.9.0b2/
--rw-r--r--   0 fselmo     (501) staff       (20)     1080 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/LICENSE
--rw-r--r--   0 fselmo     (501) staff       (20)      121 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/MANIFEST.in
--rw-r--r--   0 fselmo     (501) staff       (20)    35021 2023-06-29 16:33:27.569154 eth-tester-0.9.0b2/PKG-INFO
--rw-r--r--   0 fselmo     (501) staff       (20)    34123 2023-04-27 17:15:42.000000 eth-tester-0.9.0b2/README.md
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.531983 eth-tester-0.9.0b2/eth_tester/
--rw-r--r--   0 fselmo     (501) staff       (20)      331 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/eth_tester/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.537466 eth-tester-0.9.0b2/eth_tester/backends/
--rw-r--r--   0 fselmo     (501) staff       (20)     1652 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/backends/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2889 2023-06-28 15:53:58.000000 eth-tester-0.9.0b2/eth_tester/backends/base.py
--rw-r--r--   0 fselmo     (501) staff       (20)      540 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/backends/common.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.541611 eth-tester-0.9.0b2/eth_tester/backends/mock/
--rw-r--r--   0 fselmo     (501) staff       (20)       53 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/eth_tester/backends/mock/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      304 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/backends/mock/common.py
--rw-r--r--   0 fselmo     (501) staff       (20)    13229 2023-05-11 22:34:02.000000 eth-tester-0.9.0b2/eth_tester/backends/mock/factory.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9480 2023-06-28 15:53:58.000000 eth-tester-0.9.0b2/eth_tester/backends/mock/main.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3068 2023-05-11 22:34:02.000000 eth-tester-0.9.0b2/eth_tester/backends/mock/serializers.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.545902 eth-tester-0.9.0b2/eth_tester/backends/pyevm/
--rw-r--r--   0 fselmo     (501) staff       (20)      173 2021-11-18 21:01:41.000000 eth-tester-0.9.0b2/eth_tester/backends/pyevm/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)    26856 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/backends/pyevm/main.py
--rw-r--r--   0 fselmo     (501) staff       (20)     8556 2023-05-11 22:34:02.000000 eth-tester-0.9.0b2/eth_tester/backends/pyevm/serializers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      515 2021-11-18 21:01:41.000000 eth-tester-0.9.0b2/eth_tester/backends/pyevm/utils.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1725 2023-05-11 22:34:02.000000 eth-tester-0.9.0b2/eth_tester/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)      413 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/eth_tester/exceptions.py
--rw-r--r--   0 fselmo     (501) staff       (20)    30564 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/main.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.551534 eth-tester-0.9.0b2/eth_tester/normalization/
--rw-r--r--   0 fselmo     (501) staff       (20)      702 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/normalization/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3429 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/normalization/base.py
--rw-r--r--   0 fselmo     (501) staff       (20)      924 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/normalization/common.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2869 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/normalization/default.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3171 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/normalization/inbound.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5748 2023-06-26 21:57:05.000000 eth-tester-0.9.0b2/eth_tester/normalization/outbound.py
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/eth_tester/rpc.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.553273 eth-tester-0.9.0b2/eth_tester/tools/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-10 20:58:14.000000 eth-tester-0.9.0b2/eth_tester/tools/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2235 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/tools/gas_burner_contract.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.563598 eth-tester-0.9.0b2/eth_tester/utils/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/eth_tester/utils/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      152 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/eth_tester/utils/accounts.py
--rw-r--r--   0 fselmo     (501) staff       (20)      243 2021-07-08 21:12:50.000000 eth-tester-0.9.0b2/eth_tester/utils/address.py
--rw-r--r--   0 fselmo     (501) staff       (20)    64238 2023-06-28 15:53:58.000000 eth-tester-0.9.0b2/eth_tester/utils/backend_testing.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9633 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/utils/emitter_contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)      323 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/utils/encoding.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5244 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/utils/filters.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4324 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/utils/math_contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)      906 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/utils/module_loading.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5035 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/utils/throws_contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1191 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/utils/transactions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.568182 eth-tester-0.9.0b2/eth_tester/validation/
--rw-r--r--   0 fselmo     (501) staff       (20)      658 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/eth_tester/validation/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3075 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/validation/base.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5833 2023-05-11 22:34:02.000000 eth-tester-0.9.0b2/eth_tester/validation/common.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3114 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/validation/default.py
--rw-r--r--   0 fselmo     (501) staff       (20)    11442 2023-06-29 16:20:17.000000 eth-tester-0.9.0b2/eth_tester/validation/inbound.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9124 2023-05-11 22:34:02.000000 eth-tester-0.9.0b2/eth_tester/validation/outbound.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-06-29 16:33:27.535329 eth-tester-0.9.0b2/eth_tester.egg-info/
--rw-r--r--   0 fselmo     (501) staff       (20)    35021 2023-06-29 16:33:27.000000 eth-tester-0.9.0b2/eth_tester.egg-info/PKG-INFO
--rw-r--r--   0 fselmo     (501) staff       (20)     1616 2023-06-29 16:33:27.000000 eth-tester-0.9.0b2/eth_tester.egg-info/SOURCES.txt
--rw-r--r--   0 fselmo     (501) staff       (20)        1 2023-06-29 16:33:27.000000 eth-tester-0.9.0b2/eth_tester.egg-info/dependency_links.txt
--rw-r--r--   0 fselmo     (501) staff       (20)        1 2022-11-21 22:09:50.000000 eth-tester-0.9.0b2/eth_tester.egg-info/not-zip-safe
--rw-r--r--   0 fselmo     (501) staff       (20)      988 2023-06-29 16:33:27.000000 eth-tester-0.9.0b2/eth_tester.egg-info/requires.txt
--rw-r--r--   0 fselmo     (501) staff       (20)       11 2023-06-29 16:33:27.000000 eth-tester-0.9.0b2/eth_tester.egg-info/top_level.txt
--rw-r--r--   0 fselmo     (501) staff       (20)     1055 2023-02-01 16:36:02.000000 eth-tester-0.9.0b2/pyproject.toml
--rw-r--r--   0 fselmo     (501) staff       (20)       38 2023-06-29 16:33:27.569839 eth-tester-0.9.0b2/setup.cfg
--rw-r--r--   0 fselmo     (501) staff       (20)     2529 2023-06-29 16:32:33.000000 eth-tester-0.9.0b2/setup.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.462478 eth-tester-0.9.1b1/
+-rw-r--r--   0 eve        (501) staff       (20)     1080 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/LICENSE
+-rw-r--r--   0 eve        (501) staff       (20)      121 2022-08-25 19:50:54.000000 eth-tester-0.9.1b1/MANIFEST.in
+-rw-r--r--   0 eve        (501) staff       (20)    35041 2023-07-26 16:27:58.462303 eth-tester-0.9.1b1/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)    34123 2023-04-27 21:21:30.000000 eth-tester-0.9.1b1/README.md
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.453862 eth-tester-0.9.1b1/eth_tester/
+-rw-r--r--   0 eve        (501) staff       (20)      331 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/eth_tester/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.455057 eth-tester-0.9.1b1/eth_tester/backends/
+-rw-r--r--   0 eve        (501) staff       (20)     1652 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/backends/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     2889 2022-11-21 19:35:20.000000 eth-tester-0.9.1b1/eth_tester/backends/base.py
+-rw-r--r--   0 eve        (501) staff       (20)      540 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/backends/common.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.456229 eth-tester-0.9.1b1/eth_tester/backends/mock/
+-rw-r--r--   0 eve        (501) staff       (20)       53 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/eth_tester/backends/mock/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      304 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/backends/mock/common.py
+-rw-r--r--   0 eve        (501) staff       (20)    13229 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/backends/mock/factory.py
+-rw-r--r--   0 eve        (501) staff       (20)     9480 2022-11-21 19:35:20.000000 eth-tester-0.9.1b1/eth_tester/backends/mock/main.py
+-rw-r--r--   0 eve        (501) staff       (20)     3068 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/backends/mock/serializers.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.457208 eth-tester-0.9.1b1/eth_tester/backends/pyevm/
+-rw-r--r--   0 eve        (501) staff       (20)      173 2021-11-18 18:37:46.000000 eth-tester-0.9.1b1/eth_tester/backends/pyevm/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    27687 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/backends/pyevm/main.py
+-rw-r--r--   0 eve        (501) staff       (20)     8556 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/backends/pyevm/serializers.py
+-rw-r--r--   0 eve        (501) staff       (20)      515 2021-11-18 18:37:46.000000 eth-tester-0.9.1b1/eth_tester/backends/pyevm/utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     1725 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)      413 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/eth_tester/exceptions.py
+-rw-r--r--   0 eve        (501) staff       (20)    30564 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/main.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.458428 eth-tester-0.9.1b1/eth_tester/normalization/
+-rw-r--r--   0 eve        (501) staff       (20)      702 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/normalization/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     3429 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/normalization/base.py
+-rw-r--r--   0 eve        (501) staff       (20)      924 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/normalization/common.py
+-rw-r--r--   0 eve        (501) staff       (20)     2869 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/normalization/default.py
+-rw-r--r--   0 eve        (501) staff       (20)     3358 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/normalization/inbound.py
+-rw-r--r--   0 eve        (501) staff       (20)     5748 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/normalization/outbound.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/eth_tester/rpc.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.458659 eth-tester-0.9.1b1/eth_tester/tools/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-11-10 19:15:57.000000 eth-tester-0.9.1b1/eth_tester/tools/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     2235 2022-11-21 19:35:20.000000 eth-tester-0.9.1b1/eth_tester/tools/gas_burner_contract.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.461003 eth-tester-0.9.1b1/eth_tester/utils/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/eth_tester/utils/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      152 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/eth_tester/utils/accounts.py
+-rw-r--r--   0 eve        (501) staff       (20)      243 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/eth_tester/utils/address.py
+-rw-r--r--   0 eve        (501) staff       (20)    65774 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/utils/backend_testing.py
+-rw-r--r--   0 eve        (501) staff       (20)     9633 2022-11-21 19:35:20.000000 eth-tester-0.9.1b1/eth_tester/utils/emitter_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)      323 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/utils/encoding.py
+-rw-r--r--   0 eve        (501) staff       (20)     5244 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/utils/filters.py
+-rw-r--r--   0 eve        (501) staff       (20)     4324 2022-11-21 19:35:20.000000 eth-tester-0.9.1b1/eth_tester/utils/math_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)      906 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/utils/module_loading.py
+-rw-r--r--   0 eve        (501) staff       (20)     5035 2022-11-21 19:35:20.000000 eth-tester-0.9.1b1/eth_tester/utils/throws_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)     1191 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/utils/transactions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.462050 eth-tester-0.9.1b1/eth_tester/validation/
+-rw-r--r--   0 eve        (501) staff       (20)      658 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/validation/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     3075 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/validation/base.py
+-rw-r--r--   0 eve        (501) staff       (20)     5833 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/validation/common.py
+-rw-r--r--   0 eve        (501) staff       (20)     3114 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/validation/default.py
+-rw-r--r--   0 eve        (501) staff       (20)    11728 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/validation/inbound.py
+-rw-r--r--   0 eve        (501) staff       (20)     9124 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/validation/outbound.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.454489 eth-tester-0.9.1b1/eth_tester.egg-info/
+-rw-r--r--   0 eve        (501) staff       (20)    35041 2023-07-26 16:27:58.000000 eth-tester-0.9.1b1/eth_tester.egg-info/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)     1616 2023-07-26 16:27:58.000000 eth-tester-0.9.1b1/eth_tester.egg-info/SOURCES.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-07-26 16:27:58.000000 eth-tester-0.9.1b1/eth_tester.egg-info/dependency_links.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-07-26 16:27:58.000000 eth-tester-0.9.1b1/eth_tester.egg-info/not-zip-safe
+-rw-r--r--   0 eve        (501) staff       (20)      988 2023-07-26 16:27:58.000000 eth-tester-0.9.1b1/eth_tester.egg-info/requires.txt
+-rw-r--r--   0 eve        (501) staff       (20)       11 2023-07-26 16:27:58.000000 eth-tester-0.9.1b1/eth_tester.egg-info/top_level.txt
+-rw-r--r--   0 eve        (501) staff       (20)     1055 2022-11-21 19:35:20.000000 eth-tester-0.9.1b1/pyproject.toml
+-rw-r--r--   0 eve        (501) staff       (20)       38 2023-07-26 16:27:58.462519 eth-tester-0.9.1b1/setup.cfg
+-rw-r--r--   0 eve        (501) staff       (20)     2529 2023-07-26 16:27:18.000000 eth-tester-0.9.1b1/setup.py
```

### Comparing `eth-tester-0.9.0b2/LICENSE` & `eth-tester-0.9.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/PKG-INFO` & `eth-tester-0.9.1b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: eth-tester
-Version: 0.9.0b2
+Version: 0.9.1b1
 Summary: Tools for testing Ethereum applications.
 Home-page: https://github.com/ethereum/eth-tester
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -1032,7 +1033,9 @@
 
 
 # Use with Web3.py
 
 See the [web3.py documentation](http://web3py.readthedocs.io/en/latest/) for
 information on the `EthereumTester` provider which integrates with this
 library.
+
+
```

### Comparing `eth-tester-0.9.0b2/README.md` & `eth-tester-0.9.1b1/README.md`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/backends/__init__.py` & `eth-tester-0.9.1b1/eth_tester/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/backends/base.py` & `eth-tester-0.9.1b1/eth_tester/backends/base.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/backends/common.py` & `eth-tester-0.9.1b1/eth_tester/backends/common.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/backends/mock/factory.py` & `eth-tester-0.9.1b1/eth_tester/backends/mock/factory.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/backends/mock/main.py` & `eth-tester-0.9.1b1/eth_tester/backends/mock/main.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/backends/mock/serializers.py` & `eth-tester-0.9.1b1/eth_tester/backends/mock/serializers.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/backends/pyevm/main.py` & `eth-tester-0.9.1b1/eth_tester/backends/pyevm/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,21 +127,27 @@
     for i in range(1, quantity + 1):
         pk_bytes = int_to_big_endian(i).rjust(32, b"\x00")
         private_key = keys.PrivateKey(pk_bytes)
         yield private_key
 
 
 @to_tuple
-def get_account_keys_from_mnemonic(mnemonic, quantity=None):
+def get_account_keys_from_mnemonic(mnemonic, quantity=None, hd_path=None):
     keys = KeyAPI()
     seed = seed_from_mnemonic(mnemonic, "")
     quantity = quantity or 10
+
+    if hd_path is None:
+        # default HD path
+        hd_path = "m/44'/60'/0'"
+
     for i in range(0, quantity):
-        hd_path = HDPath(f"m/44'/60'/0'/{i}")
-        private_key = keys.PrivateKey(hd_path.derive(seed))
+        # create unique HDPath to derive the private key for each account
+        key = HDPath(f"{hd_path}/{i}").derive(seed)
+        private_key = keys.PrivateKey(key)
         yield private_key
 
 
 @to_dict
 def generate_genesis_state_for_keys(account_keys, overrides=None):
     for private_key in account_keys:
         account_state = get_default_account_state(overrides=overrides)
@@ -179,14 +185,15 @@
 
 def setup_tester_chain(
     genesis_params=None,
     genesis_state=None,
     num_accounts=None,
     vm_configuration=None,
     mnemonic=None,
+    hd_path=None,
     genesis_is_post_merge=True,
 ):
     from eth.chains.base import MiningChain
     from eth.consensus import (
         NoProofConsensus,
         ConsensusApplier,
     )
@@ -227,15 +234,17 @@
             overrides["mix_hash"] = GENESIS_MIX_HASH
         genesis_params = get_default_genesis_params(overrides=overrides)
 
     if genesis_state:
         num_accounts = len(genesis_state)
 
     if mnemonic:
-        account_keys = get_account_keys_from_mnemonic(mnemonic, quantity=num_accounts)
+        account_keys = get_account_keys_from_mnemonic(
+            mnemonic, quantity=num_accounts, hd_path=hd_path
+        )
     else:
         account_keys = get_default_account_keys(quantity=num_accounts)
 
     if genesis_state is None:
         genesis_state = generate_genesis_state_for_keys(account_keys)
 
     base_db = get_db_backend()
@@ -317,14 +326,15 @@
 
     def __init__(
         self,
         genesis_parameters=None,
         genesis_state=None,
         vm_configuration=None,
         mnemonic=None,
+        hd_path=None,
     ):
         """
         :param genesis_parameters: A dict of chain parameters for overriding default
              values when setting up the chain.
         :param genesis_state: A dict (or list of tuples) matching accounts to state
              properties, such as `balance`.
         :param vm_configuration: The tuple of virtual machines defining a chain
@@ -338,37 +348,50 @@
                 "The `PyEVMBackend` requires py-evm to be installed and importable. "
                 "Please install or update the `py-evm` library."
             )
 
         self.account_keys = None  # set below
         accounts = len(genesis_state) if genesis_state else None
         self.reset_to_genesis(
-            genesis_parameters, genesis_state, accounts, vm_configuration, mnemonic
+            genesis_parameters,
+            genesis_state,
+            accounts,
+            vm_configuration,
+            mnemonic,
+            hd_path,
         )
 
     @classmethod
     def from_mnemonic(
         cls,
         mnemonic,
         genesis_state_overrides=None,
         num_accounts=None,
         genesis_parameters=None,
         vm_configuration=None,
+        hd_path=None,
     ):
+        """
+        Create a genesis state pre-populated with accounts. A number of accounts can be
+        initialized with a mnemonic phrase and heirarchical deterministic path. If no
+        overrides are provided, a default set of accounts will be used.
+        """
         genesis_state = PyEVMBackend.generate_genesis_state(
             mnemonic=mnemonic,
             overrides=genesis_state_overrides or {},
             num_accounts=num_accounts,
+            hd_path=hd_path,
         )
 
         return cls(
             genesis_parameters=genesis_parameters,
             genesis_state=genesis_state,
             vm_configuration=vm_configuration,
             mnemonic=mnemonic,
+            hd_path=hd_path,
         )
 
     #
     # Genesis
     #
 
     @classmethod
@@ -376,24 +399,31 @@
         return cls._generate_genesis_params(overrides=overrides)
 
     @staticmethod
     def _generate_genesis_params(overrides=None):
         return get_default_genesis_params(overrides=overrides)
 
     @classmethod
-    def generate_genesis_state(cls, overrides=None, num_accounts=None, mnemonic=None):
+    def generate_genesis_state(
+        cls, overrides=None, num_accounts=None, mnemonic=None, hd_path=None
+    ):
         return cls._generate_genesis_state(
-            overrides=overrides, num_accounts=num_accounts, mnemonic=mnemonic
+            overrides=overrides,
+            num_accounts=num_accounts,
+            mnemonic=mnemonic,
+            hd_path=hd_path,
         )
 
     @staticmethod
-    def _generate_genesis_state(overrides=None, num_accounts=None, mnemonic=None):
+    def _generate_genesis_state(
+        overrides=None, num_accounts=None, mnemonic=None, hd_path=None
+    ):
         if mnemonic:
             account_keys = get_account_keys_from_mnemonic(
-                mnemonic, quantity=num_accounts
+                mnemonic, quantity=num_accounts, hd_path=hd_path
             )
         else:
             account_keys = get_default_account_keys(quantity=num_accounts)
 
         return generate_genesis_state_for_keys(
             account_keys=account_keys, overrides=overrides
         )
@@ -401,21 +431,23 @@
     def reset_to_genesis(
         self,
         genesis_params=None,
         genesis_state=None,
         num_accounts=None,
         vm_configuration=None,
         mnemonic=None,
+        hd_path=None,
     ):
         self.account_keys, self.chain = setup_tester_chain(
             genesis_params,
             genesis_state,
             num_accounts,
             vm_configuration,
             mnemonic,
+            hd_path,
         )
 
     #
     # Private Accounts API
     #
     @property
     def _key_lookup(self):
```

### Comparing `eth-tester-0.9.0b2/eth_tester/backends/pyevm/serializers.py` & `eth-tester-0.9.1b1/eth_tester/backends/pyevm/serializers.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/backends/pyevm/utils.py` & `eth-tester-0.9.1b1/eth_tester/backends/pyevm/utils.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/constants.py` & `eth-tester-0.9.1b1/eth_tester/constants.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/main.py` & `eth-tester-0.9.1b1/eth_tester/main.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/normalization/__init__.py` & `eth-tester-0.9.1b1/eth_tester/normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/normalization/base.py` & `eth-tester-0.9.1b1/eth_tester/normalization/base.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/normalization/common.py` & `eth-tester-0.9.1b1/eth_tester/normalization/common.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/normalization/default.py` & `eth-tester-0.9.1b1/eth_tester/normalization/default.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/normalization/inbound.py` & `eth-tester-0.9.1b1/eth_tester/normalization/inbound.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,23 +23,29 @@
 from .common import (
     normalize_array,
     normalize_dict,
     normalize_if,
 )
 
 from eth_tester.validation.inbound import (
+    is_32byte_hex_string,
+    is_32_bytes,
     is_valid_topic_array,
 )
 
 
 def normalize_topic(topic):
     if topic is None:
         return None
-    else:
+    if is_32byte_hex_string(topic):
         return decode_hex(topic)
+    if is_32_bytes(topic):
+        return topic
+
+    raise TypeError(f"Topic is not in a recognized format: {topic}")
 
 
 @to_tuple
 def normalize_topic_list(topics):
     for topic in topics:
         yield normalize_topic(topic)
```

### Comparing `eth-tester-0.9.0b2/eth_tester/normalization/outbound.py` & `eth-tester-0.9.1b1/eth_tester/normalization/outbound.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/tools/gas_burner_contract.py` & `eth-tester-0.9.1b1/eth_tester/tools/gas_burner_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/utils/backend_testing.py` & `eth-tester-0.9.1b1/eth_tester/utils/backend_testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,17 @@
     _make_call_throws_transaction,
     _decode_throws_result,
 )
 from eth_tester.tools.gas_burner_contract import (
     _deploy_gas_burner,
     _make_call_gas_burner_transaction,
 )
+from eth_utils import (
+    encode_hex,
+)
 
 PK_A = "0x58d23b55bc9cdce1f18c2500f40ff4ab7245df9a89505e9b1fa4851f623d241d"
 PK_A_ADDRESS = "0xdc544d1aa88ff8bbd2f2aec754b1f1e99e1812fd"
 
 NON_DEFAULT_GAS_PRICE = 1000000000
 
 SIMPLE_TRANSACTION = {
@@ -1501,22 +1504,32 @@
             [
                 [
                     "0xf70fe689e290d8ce2b2a388ac28db36fbb0e16a6d89c6804c461f65a1b40bb15",  # noqa: E501
                     "0x" + "00" * 31 + "99",
                 ],
                 0,
             ],
+            [
+                [
+                    (
+                        b"\xf7\x0f\xe6\x89\xe2\x90\xd8\xce+*8\x8a\xc2\x8d\xb3o\xbb\x0e"
+                        b"\x16\xa6\xd8\x9ch\x04\xc4a\xf6Z\x1b@\xbb\x15"
+                    )
+                ],
+                1,
+            ],
         ),
         ids=[
             "filter None",
             "filter []",
             "filter Event only",
             "filter Event and None",
             "filter Event and argument",
             "filter Event and wrong argument",
+            "filter Event only bytes",
         ],
     )
     def test_log_filter_picks_up_new_logs(self, eth_tester, filter_topics, expected):
         """
         Cases to test:
         - filter multiple transactions in one block.
         - filter mined.
@@ -1547,14 +1560,53 @@
         specific_logs_changes = eth_tester.get_only_filter_changes(filter_event)
         specific_logs_all = eth_tester.get_all_filter_logs(filter_event)
         specific_direct_logs_all = eth_tester.get_logs(topics=filter_topics)
         assert len(specific_logs_changes) == expected
         assert len(specific_logs_all) == expected
         assert len(specific_direct_logs_all) == expected
 
+    @pytest.mark.parametrize(
+        "filter_topics",
+        (
+            "not a list",
+            {},
+            1,
+            [1],
+            [1, 2],
+            [1, None],
+            [None, 1],
+            [encode_hex(b"\x00" * 30 + b"\x01")],
+            [encode_hex(b"\x00" * 32 + b"\x01")],
+        ),
+        ids=[
+            "filter string",
+            "filter dict",
+            "filter int",
+            "filter int in list",
+            "filter multiple ints in list",
+            "filter int and None in list",
+            "filter None and int in list",
+            "filter bytes with less than 32 bytes",
+            "filter bytes with more than 32 bytes",
+        ],
+    )
+    def test_log_filter_invalid_topics_throws_error(self, eth_tester, filter_topics):
+        self.skip_if_no_evm_execution()
+
+        emitter_address = _deploy_emitter(eth_tester)
+        _call_emitter(
+            eth_tester,
+            emitter_address,
+            "logSingle",
+            [EMITTER_ENUM["LogSingleWithIndex"], 1],
+        )
+
+        with pytest.raises(ValidationError):
+            eth_tester.create_log_filter(from_block=0, topics=filter_topics)
+
     def test_log_filter_includes_old_logs(self, eth_tester):
         """
         Cases to test:
         - filter multiple transactions in one block.
         - filter mined.
         self.skip_if_no_evm_execution()
```

### Comparing `eth-tester-0.9.0b2/eth_tester/utils/emitter_contract.py` & `eth-tester-0.9.1b1/eth_tester/utils/emitter_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/utils/filters.py` & `eth-tester-0.9.1b1/eth_tester/utils/filters.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/utils/math_contract.py` & `eth-tester-0.9.1b1/eth_tester/utils/math_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/utils/module_loading.py` & `eth-tester-0.9.1b1/eth_tester/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/utils/throws_contract.py` & `eth-tester-0.9.1b1/eth_tester/utils/throws_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/utils/transactions.py` & `eth-tester-0.9.1b1/eth_tester/utils/transactions.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/validation/__init__.py` & `eth-tester-0.9.1b1/eth_tester/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/validation/base.py` & `eth-tester-0.9.1b1/eth_tester/validation/base.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/validation/common.py` & `eth-tester-0.9.1b1/eth_tester/validation/common.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/validation/default.py` & `eth-tester-0.9.1b1/eth_tester/validation/default.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester/validation/inbound.py` & `eth-tester-0.9.1b1/eth_tester/validation/inbound.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     List,
     Union,
 )
 
 from eth_typing import HexStr
 from eth_utils import (
     is_boolean,
+    is_bytes,
     is_checksum_address,
     is_checksum_formatted_address,
     is_dict,
     is_hex,
     is_hex_address,
     is_hexstr,
     is_integer,
@@ -43,20 +44,24 @@
     validate_uint256,
     validate_uint64,
     validate_uint8,
     validate_text,
 )
 
 
+def is_32_bytes(value):
+    return is_bytes(value) and len(value) == 32
+
+
 def is_32byte_hex_string(value):
     return is_text(value) and is_hex(value) and len(remove_0x_prefix(value)) == 64
 
 
 def is_topic(value):
-    return value is None or is_32byte_hex_string(value)
+    return value is None or is_32byte_hex_string(value) or is_32_bytes(value)
 
 
 def validate_32_byte_hex_value(value, name):
     error_message = (
         "{} must be a hexadecimal encoded 32 byte string.  Got: "
         "{}".format(name, value)
     )
@@ -151,16 +156,18 @@
             )
         for sub_address in address:
             validate_account(sub_address)
     elif not is_hex_address(address):
         validate_account(address)
 
     invalid_topics_message = (
-        "Topics must be one of `None`, an array of 32 byte hexadecimal encoded "
-        "strings, or an array of arrays of 32 byte hexadecimal strings"
+        "Topics must be one of `None` or an array of topics. Each topic must be 32 "
+        "bytes, represented as a bytestring or its hex string equivalent. A "
+        'filter query of topics using "OR" can be achieved using a sub-array of '
+        "topics. See https://eth.wiki/json-rpc/API#eth_newfilter for more details."
     )
     # topics
     if topics is None:
         pass
     elif not is_list_like(topics):
         raise ValidationError(invalid_topics_message)
     elif is_valid_topic_array(topics):
```

### Comparing `eth-tester-0.9.0b2/eth_tester/validation/outbound.py` & `eth-tester-0.9.1b1/eth_tester/validation/outbound.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester.egg-info/PKG-INFO` & `eth-tester-0.9.1b1/eth_tester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: eth-tester
-Version: 0.9.0b2
+Version: 0.9.1b1
 Summary: Tools for testing Ethereum applications.
 Home-page: https://github.com/ethereum/eth-tester
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -1032,7 +1033,9 @@
 
 
 # Use with Web3.py
 
 See the [web3.py documentation](http://web3py.readthedocs.io/en/latest/) for
 information on the `EthereumTester` provider which integrates with this
 library.
+
+
```

### Comparing `eth-tester-0.9.0b2/eth_tester.egg-info/SOURCES.txt` & `eth-tester-0.9.1b1/eth_tester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/eth_tester.egg-info/requires.txt` & `eth-tester-0.9.1b1/eth_tester.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [dev]
 bumpversion<1.0.0,>=0.5.3
 tox<3.0.0,>=2.9.1
 wheel<1.0.0,>=0.30.0
 pytest>=7.0.0
 pytest-xdist<3,>=2.0.0
 eth-hash[pycryptodome]<1.0.0,>=0.1.4
-py-evm==0.7.0a2
+py-evm==0.7.0a4
 black<23,>=22
 flake8<4.0.0,>=3.5.0
 towncrier<22,>=21
 
 [dev:implementation_name == "cpython"]
 eth-hash[pysha3]<1.0.0,>=0.1.4
 
@@ -27,24 +27,24 @@
 towncrier<22,>=21
 
 [lint]
 black<23,>=22
 flake8<4.0.0,>=3.5.0
 
 [py-evm]
-py-evm==0.7.0a2
+py-evm==0.7.0a4
 
 [py-evm:implementation_name == "cpython"]
 eth-hash[pysha3]<1.0.0,>=0.1.4
 
 [py-evm:implementation_name == "pypy"]
 eth-hash[pycryptodome]<1.0.0,>=0.1.4
 
 [pyevm]
-py-evm==0.7.0a2
+py-evm==0.7.0a4
 
 [pyevm:implementation_name == "cpython"]
 eth-hash[pysha3]<1.0.0,>=0.1.4
 
 [pyevm:implementation_name == "pypy"]
 eth-hash[pycryptodome]<1.0.0,>=0.1.4
```

### Comparing `eth-tester-0.9.0b2/pyproject.toml` & `eth-tester-0.9.1b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.0b2/setup.py` & `eth-tester-0.9.1b1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "bumpversion>=0.5.3,<1.0.0",
         "tox>=2.9.1,<3.0.0",
         "wheel>=0.30.0,<1.0.0",
     ],
     "py-evm": [
         # Pin py-evm to exact version, until it leaves alpha.
         # EVM is very high velocity and might change API at each alpha.
-        "py-evm==0.7.0a2",
+        "py-evm==0.7.0a4",
         "eth-hash[pysha3]>=0.1.4,<1.0.0;implementation_name=='cpython'",
         "eth-hash[pycryptodome]>=0.1.4,<1.0.0;implementation_name=='pypy'",
     ],
     "docs": [
         "towncrier>=21,<22",
     ],
 }
@@ -45,15 +45,15 @@
 
 with open("./README.md") as readme:
     long_description = readme.read()
 
 setup(
     name="eth-tester",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="0.9.0-beta.2",
+    version="0.9.1-beta.1",
     description="""Tools for testing Ethereum applications.""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Piper Merriam",
     author_email="pipermerriam@gmail.com",
     url="https://github.com/ethereum/eth-tester",
     include_package_data=True,
```

