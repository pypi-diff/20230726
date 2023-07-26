# Comparing `tmp/multisig_ci-0.5.0.tar.gz` & `tmp/multisig_ci-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multisig_ci-0.5.0.tar", max compression
+gzip compressed data, was "multisig_ci-0.6.0.tar", max compression
```

## Comparing `multisig_ci-0.5.0.tar` & `multisig_ci-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    34523 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/LICENSE
--rw-r--r--   0        0        0        0 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/__init__.py
--rw-r--r--   0        0        0      570 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/__main__.py
--rw-r--r--   0        0        0     8265 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/ci_override.py
--rw-r--r--   0        0        0     5811 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/hydrate_ci_cache.py
--rw-r--r--   0        0        0     2033 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/run_brownie.py
--rw-r--r--   0        0        0      811 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/safes.py
--rw-r--r--   0        0        0     1580 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/sign.py
--rw-r--r--   0        0        0     1913 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/telegram.py
--rwxr-xr-x   0        0        0      651 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/multisig_ci/test_telegram.sh
--rw-r--r--   0        0        0      504 2023-07-26 05:58:12.072521 multisig_ci-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 multisig_ci-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-26 07:17:14.343462 multisig_ci-0.6.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-26 07:17:14.343462 multisig_ci-0.6.0/multisig_ci/__init__.py
+-rw-r--r--   0        0        0      570 2023-07-26 07:17:14.343462 multisig_ci-0.6.0/multisig_ci/__main__.py
+-rw-r--r--   0        0        0     8308 2023-07-26 07:17:14.347462 multisig_ci-0.6.0/multisig_ci/ci_override.py
+-rw-r--r--   0        0        0     5811 2023-07-26 07:17:14.347462 multisig_ci-0.6.0/multisig_ci/hydrate_ci_cache.py
+-rw-r--r--   0        0        0     2033 2023-07-26 07:17:14.347462 multisig_ci-0.6.0/multisig_ci/run_brownie.py
+-rw-r--r--   0        0        0      811 2023-07-26 07:17:14.347462 multisig_ci-0.6.0/multisig_ci/safes.py
+-rw-r--r--   0        0        0     1580 2023-07-26 07:17:14.347462 multisig_ci-0.6.0/multisig_ci/sign.py
+-rw-r--r--   0        0        0     1913 2023-07-26 07:17:14.347462 multisig_ci-0.6.0/multisig_ci/telegram.py
+-rwxr-xr-x   0        0        0      651 2023-07-26 07:17:14.347462 multisig_ci-0.6.0/multisig_ci/test_telegram.sh
+-rw-r--r--   0        0        0      508 2023-07-26 07:17:14.347462 multisig_ci-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 multisig_ci-0.6.0/PKG-INFO
```

### Comparing `multisig_ci-0.5.0/LICENSE` & `multisig_ci-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.5.0/multisig_ci/__main__.py` & `multisig_ci-0.6.0/multisig_ci/__main__.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.5.0/multisig_ci/ci_override.py` & `multisig_ci-0.6.0/multisig_ci/ci_override.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from copy import copy
-from ape_safe import ApeSafe, transaction_service, multisends
+from brownie_safe import BrownieSafe as ApeSafe
+from brownie_safe import transaction_service, multisends
 from brownie import accounts, network, chain, Contract
 from gnosis.safe.safe_tx import SafeTx
 from eth_abi import encode_abi
 from typing import Optional, Union
 from brownie.network.account import LocalAccount
 from brownie._config import CONFIG
```

### Comparing `multisig_ci-0.5.0/multisig_ci/hydrate_ci_cache.py` & `multisig_ci-0.6.0/multisig_ci/hydrate_ci_cache.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.5.0/multisig_ci/run_brownie.py` & `multisig_ci-0.6.0/multisig_ci/run_brownie.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.5.0/multisig_ci/safes.py` & `multisig_ci-0.6.0/multisig_ci/safes.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.5.0/multisig_ci/sign.py` & `multisig_ci-0.6.0/multisig_ci/sign.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.5.0/multisig_ci/telegram.py` & `multisig_ci-0.6.0/multisig_ci/telegram.py`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.5.0/multisig_ci/test_telegram.sh` & `multisig_ci-0.6.0/multisig_ci/test_telegram.sh`

 * *Files identical despite different names*

### Comparing `multisig_ci-0.5.0/PKG-INFO` & `multisig_ci-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: multisig-ci
-Version: 0.5.0
+Version: 0.6.0
 Summary: Gnosis safe ci scripts.
 License: AGPLv3
 Author: kx9x
 Author-email: kx9x@protonmail.com
 Requires-Python: >=3.8,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: ape_safe (>=0.5.0)
+Requires-Dist: brownie_safe (>=0.8.0)
 Requires-Dist: eth-brownie (==1.19.2)
 Requires-Dist: psutil (>=5.8.0)
 Requires-Dist: requests (>=2.26.0)
 Requires-Dist: safe-eth-py (==4.3.2)
 Requires-Dist: tenacity (>=8.0.1)
```

