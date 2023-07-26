# Comparing `tmp/brownie_safe-0.8.0.tar.gz` & `tmp/brownie_safe-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brownie_safe-0.8.0.tar", max compression
+gzip compressed data, was "brownie_safe-0.8.1.tar", max compression
```

## Comparing `brownie_safe-0.8.0.tar` & `brownie_safe-0.8.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    17686 2023-07-04 18:56:06.394943 brownie_safe-0.8.0/brownie_safe.py
--rw-r--r--   0        0        0      539 2023-07-04 18:57:17.353280 brownie_safe-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      910 2023-06-28 16:20:48.160418 brownie_safe-0.8.0/readme.md
--rw-r--r--   0        0        0     1634 1970-01-01 00:00:00.000000 brownie_safe-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    17692 2023-07-26 08:46:56.122840 brownie_safe-0.8.1/brownie_safe.py
+-rw-r--r--   0        0        0      539 2023-07-26 08:36:01.799721 brownie_safe-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      910 2023-06-28 16:20:48.160418 brownie_safe-0.8.1/readme.md
+-rw-r--r--   0        0        0     1584 1970-01-01 00:00:00.000000 brownie_safe-0.8.1/PKG-INFO
```

### Comparing `brownie_safe-0.8.0/brownie_safe.py` & `brownie_safe-0.8.1/brownie_safe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import warnings
 from copy import copy
 from typing import Dict, List, Optional, Union
+from enum import Enum
 
 import click
 from gnosis.eth import EthereumClient, EthereumNetwork
 from web3 import Web3  # don't move below brownie import
 from brownie import Contract, accounts, chain, history, web3
 from brownie.convert.datatypes import EthAddress
 from brownie.network.account import LocalAccount
@@ -13,21 +14,20 @@
 from eth_abi import encode_abi
 from eth_utils import is_address, to_checksum_address, encode_hex, keccak
 from gnosis.safe import Safe, SafeOperation
 from gnosis.safe.multi_send import MultiSend, MultiSendOperation, MultiSendTx
 from gnosis.safe.safe_tx import SafeTx
 from gnosis.safe.signatures import signature_split, signature_to_bytes
 from gnosis.safe.api import TransactionServiceApi
+from gnosis.eth.ethereum_client import EthereumNetworkNotSupported
 from hexbytes import HexBytes
 from trezorlib import ethereum, tools, ui
 from trezorlib.client import TrezorClient
 from trezorlib.messages import EthereumSignMessage
 from trezorlib.transport import get_transport
-from enum import Enum
-from gnosis.eth.ethereum_client import EthereumNetworkNotSupported
 
 MULTISEND_CALL_ONLY = '0x40A2aCCbd92BCA938b02010E17A5b8929b49130D'
 multisends = {
     10: '0x998739BFdAAdde7C933B942a68053933098f9EDa',
     250: '0x10B62CC1E8D9a9f1Ad05BCC491A7984697c19f7E',
     288: '0x2Bd65cd56cAAC777f87d7808d13DEAF88e54E0eA',
     43114: '0x998739BFdAAdde7C933B942a68053933098f9EDa'
@@ -63,15 +63,15 @@
         EthereumNetworkBackport.OPTIMISM: "https://safe-transaction-optimism.safe.global",
         EthereumNetworkBackport.ENERGY_WEB_VOLTA_TESTNET: "https://safe-transaction-volta.safe.global",
         EthereumNetworkBackport.GNOSIS: "https://safe-transaction-gnosis-chain.safe.global",
         EthereumNetworkBackport.FANTOM: "https://safe-txservice.fantom.network",
         EthereumNetworkBackport.BOBA_NETWORK: "https://safe-transaction.mainnet.boba.network",
     }
 
-    def __init__(self, network: EthereumNetwork, ethereum_client: EthereumClient | None = None, base_url: str | None = None):
+    def __init__(self, network: EthereumNetwork, ethereum_client: Optional[EthereumClient] = None, base_url: Optional[str] = None):
         self.network = network
         self.ethereum_client = ethereum_client
         self.base_url = base_url or self.URL_BY_NETWORK.get(EthereumNetworkBackport(network.value))
         if not self.base_url:
             raise EthereumNetworkNotSupported(network)
```

### Comparing `brownie_safe-0.8.0/pyproject.toml` & `brownie_safe-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "brownie-safe"
-version = "0.8.0"
+version = "0.8.1"
 description = "Build complex Gnosis Safe transactions and safely preview them in a forked environment."
 authors = ["banteg"]
 license = "MIT"
 repository = "https://github.com/banteg/brownie-safe"
 readme = "readme.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.9,<3.11"
 eth-brownie = "1.19.2"
 safe-eth-py = "4.3.2"
 trezor = "0.13.7"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
```

### Comparing `brownie_safe-0.8.0/readme.md` & `brownie_safe-0.8.1/readme.md`

 * *Files identical despite different names*

### Comparing `brownie_safe-0.8.0/PKG-INFO` & `brownie_safe-0.8.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: brownie-safe
-Version: 0.8.0
+Version: 0.8.1
 Summary: Build complex Gnosis Safe transactions and safely preview them in a forked environment.
 Home-page: https://github.com/banteg/brownie-safe
 License: MIT
 Author: banteg
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: eth-brownie (==1.19.2)
 Requires-Dist: safe-eth-py (==4.3.2)
 Requires-Dist: trezor (==0.13.7)
 Project-URL: Repository, https://github.com/banteg/brownie-safe
 Description-Content-Type: text/markdown
```

