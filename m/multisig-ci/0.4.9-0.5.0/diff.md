# Comparing `tmp/multisig_ci-0.4.9.tar.gz` & `tmp/multisig_ci-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multisig_ci-0.4.9.tar", max compression
+gzip compressed data, was "multisig_ci-0.5.0.tar", max compression
```

## Comparing `multisig_ci-0.4.9.tar` & `multisig_ci-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/LICENSE
--rw-r--r--   0        0        0        0 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/__init__.py
--rw-r--r--   0        0        0      570 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/__main__.py
--rw-r--r--   0        0        0     7536 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/ci_override.py
--rw-r--r--   0        0        0     5811 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/hydrate_ci_cache.py
--rw-r--r--   0        0        0     2033 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/run_brownie.py
--rw-r--r--   0        0        0      811 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/safes.py
--rw-r--r--   0        0        0     1580 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/sign.py
--rw-r--r--   0        0        0     1913 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/telegram.py
--rwxr-xr-x   0        0        0      651 2023-05-19 17:25:06.644107 multisig_ci-0.4.9/multisig_ci/test_telegram.sh
--rw-r--r--   0        0        0      492 2023-05-19 17:25:06.648108 multisig_ci-0.4.9/pyproject.toml
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 multisig_ci-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/__init__.py
+-rw-r--r--   0        0        0      570 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/__main__.py
+-rw-r--r--   0        0        0     8265 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/ci_override.py
+-rw-r--r--   0        0        0     5811 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/hydrate_ci_cache.py
+-rw-r--r--   0        0        0     2033 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/run_brownie.py
+-rw-r--r--   0        0        0      811 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/safes.py
+-rw-r--r--   0        0        0     1580 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/sign.py
+-rw-r--r--   0        0        0     1913 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/telegram.py
+-rwxr-xr-x   0        0        0      651 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/test_telegram.sh
+-rw-r--r--   0        0        0      504 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 multisig_ci-0.5.0/PKG-INFO
```

### Comparing `multisig_ci-0.4.9/LICENSE` & `multisig_ci-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.9/multisig_ci/__main__.py` & `multisig_ci-0.5.0/multisig_ci/__main__.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.9/multisig_ci/ci_override.py` & `multisig_ci-0.5.0/multisig_ci/ci_override.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,23 +34,39 @@
         56: 'http://mainnet.gnosis.yearn.tools/bsc:{0}/transactions/queue',
         100: 'http://mainnet.gnosis.yearn.tools/xdai:{0}/transactions/queue',
         137: 'http://mainnet.gnosis.yearn.tools/matic:{0}/transactions/queue',
         42161: 'http://mainnet.gnosis.yearn.tools/arb1:{0}/transactions/queue'
     }
 }
 
+patched_transaction_service_urls = {
+    1: 'https://safe-transaction-mainnet.safe.global',
+    5: 'https://safe-transaction-goerli.safe.global',
+    10: 'https://safe-transaction-optimism.safe.global',
+    56: 'https://safe-transaction-bsc.safe.global',
+    100: 'https://safe-transaction-gnosis-chain.safe.global',
+    137: 'https://safe-transaction-polygon.safe.global',
+    246: 'https://safe-transaction-ewc.safe.global',
+    250: 'https://safe-txservice.fantom.network',
+    288: 'https://safe-transaction.mainnet.boba.network',
+    42161: 'https://safe-transaction-arbitrum.safe.global',
+    43114: 'https://safe-transaction-avalanche.safe.global',
+    73799: 'https://safe-transaction-volta.safe.global',
+    1313161554: 'https://safe-transaction-aurora.safe.global',
+}
 
 class DelegateSafe(ApeSafe):
     def __init__(self, address, base_url=None, multisend=None):
         """
         Create an ApeSafe from an address or a ENS name and use a default connection.
         """
         
-        transaction_service[250] = "https://safe-txservice.fantom.network"
-        transaction_service[10] = "https://safe-transaction.optimism.gnosis.io"
+        for n, url in patched_transaction_service_urls.items():
+            transaction_service[n] = url
+
         multisends[10] = "0x998739BFdAAdde7C933B942a68053933098f9EDa"
         backend_urls = {
             'gnosis': transaction_service,
             'yearn': {1: 'https://safe-transaction.mainnet.gnosis.yearn.tools/'}
         }
 
         # default to gnosis if we don't have a yearn version
```

### Comparing `multisig_ci-0.4.9/multisig_ci/hydrate_ci_cache.py` & `multisig_ci-0.5.0/multisig_ci/hydrate_ci_cache.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.9/multisig_ci/run_brownie.py` & `multisig_ci-0.5.0/multisig_ci/run_brownie.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.9/multisig_ci/safes.py` & `multisig_ci-0.5.0/multisig_ci/safes.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.9/multisig_ci/sign.py` & `multisig_ci-0.5.0/multisig_ci/sign.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.9/multisig_ci/telegram.py` & `multisig_ci-0.5.0/multisig_ci/telegram.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.9/multisig_ci/test_telegram.sh` & `multisig_ci-0.5.0/multisig_ci/test_telegram.sh`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.4.9/PKG-INFO` & `multisig_ci-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: multisig-ci
-Version: 0.4.9
+Version: 0.5.0
 Summary: Gnosis safe ci scripts.
 License: AGPLv3
 Author: kx9x
 Author-email: kx9x@protonmail.com
 Requires-Python: >=3.8,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: ape_safe (==0.5.0)
-Requires-Dist: eth_brownie (==1.17)
-Requires-Dist: gnosis-py (==3.6.0)
-Requires-Dist: psutil (==5.8.0)
-Requires-Dist: requests (==2.26.0)
-Requires-Dist: tenacity (==8.0.1)
+Requires-Dist: ape_safe (>=0.5.0)
+Requires-Dist: eth-brownie (==1.19.2)
+Requires-Dist: psutil (>=5.8.0)
+Requires-Dist: requests (>=2.26.0)
+Requires-Dist: safe-eth-py (==4.3.2)
+Requires-Dist: tenacity (>=8.0.1)
```

