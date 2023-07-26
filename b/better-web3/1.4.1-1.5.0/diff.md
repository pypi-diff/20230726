# Comparing `tmp/better_web3-1.4.1.tar.gz` & `tmp/better_web3-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_web3-1.4.1.tar", max compression
+gzip compressed data, was "better_web3-1.5.0.tar", max compression
```

## Comparing `better_web3-1.4.1.tar` & `better_web3-1.5.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0      403 2023-07-17 08:30:00.413000 better_web3-1.4.1/better_web3/__init__.py
--rw-r--r--   0        0        0    10461 2023-07-17 08:28:26.368000 better_web3-1.4.1/better_web3/batch_call.py
--rw-r--r--   0        0        0    15939 2023-07-23 08:52:53.716000 better_web3-1.4.1/better_web3/chain.py
--rw-r--r--   0        0        0      251 2023-07-07 12:10:25.885000 better_web3-1.4.1/better_web3/contract/__init__.py
--rw-r--r--   0        0        0      525 2023-07-11 06:39:31.842000 better_web3-1.4.1/better_web3/contract/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      687 2023-07-11 06:39:33.730000 better_web3-1.4.1/better_web3/contract/__pycache__/_abi.cpython-311.pyc
--rw-r--r--   0        0        0      351 2023-06-05 07:45:48.569000 better_web3-1.4.1/better_web3/contract/__pycache__/_paths.cpython-311.pyc
--rw-r--r--   0        0        0     2938 2023-07-11 06:39:31.913000 better_web3-1.4.1/better_web3/contract/__pycache__/contract.cpython-311.pyc
--rw-r--r--   0        0        0     1938 2023-07-11 06:39:34.027000 better_web3-1.4.1/better_web3/contract/__pycache__/disperse.cpython-311.pyc
--rw-r--r--   0        0        0     3687 2023-07-11 06:39:34.086000 better_web3-1.4.1/better_web3/contract/__pycache__/erc20.cpython-311.pyc
--rw-r--r--   0        0        0     5293 2023-07-11 06:39:34.163000 better_web3-1.4.1/better_web3/contract/__pycache__/erc721.cpython-311.pyc
--rw-r--r--   0        0        0     9601 2023-07-11 06:39:33.679000 better_web3-1.4.1/better_web3/contract/__pycache__/multicall.cpython-311.pyc
--rw-r--r--   0        0        0      352 2023-07-07 12:03:06.296000 better_web3-1.4.1/better_web3/contract/_abi.py
--rw-r--r--   0        0        0       99 2023-06-05 07:40:59.317000 better_web3-1.4.1/better_web3/contract/_paths.py
--rw-r--r--   0        0        0     1193 2023-06-23 09:34:50.869000 better_web3-1.4.1/better_web3/contract/abi/disperse.json
--rw-r--r--   0        0        0     6301 2023-06-05 07:31:12.380000 better_web3-1.4.1/better_web3/contract/abi/erc1155.json
--rw-r--r--   0        0        0     5904 2023-06-05 07:28:35.070000 better_web3-1.4.1/better_web3/contract/abi/erc20.json
--rw-r--r--   0        0        0     6755 2023-06-05 07:31:25.078000 better_web3-1.4.1/better_web3/contract/abi/erc721.json
--rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-1.4.1/better_web3/contract/abi/multicall_v3.json
--rw-r--r--   0        0        0     1264 2023-07-10 08:18:27.356000 better_web3-1.4.1/better_web3/contract/contract.py
--rw-r--r--   0        0        0      974 2023-07-07 12:13:30.821000 better_web3-1.4.1/better_web3/contract/disperse.py
--rw-r--r--   0        0        0     1747 2023-07-07 20:11:33.426000 better_web3-1.4.1/better_web3/contract/erc20.py
--rw-r--r--   0        0        0     2876 2023-07-07 20:11:33.364000 better_web3-1.4.1/better_web3/contract/erc721.py
--rw-r--r--   0        0        0     6201 2023-07-07 12:07:18.259000 better_web3-1.4.1/better_web3/contract/multicall.py
--rw-r--r--   0        0        0      165 2023-06-06 11:25:51.067000 better_web3-1.4.1/better_web3/enums.py
--rw-r--r--   0        0        0     4037 2023-07-17 10:02:59.828000 better_web3-1.4.1/better_web3/proxy.py
--rw-r--r--   0        0        0      730 2023-07-17 08:28:26.473000 better_web3-1.4.1/better_web3/utils/__init__.py
--rw-r--r--   0        0        0      917 2023-07-17 08:28:28.447000 better_web3-1.4.1/better_web3/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4132 2023-07-17 08:28:28.496000 better_web3-1.4.1/better_web3/utils/__pycache__/eth.cpython-311.pyc
--rw-r--r--   0        0        0     3469 2023-06-28 12:32:10.861000 better_web3-1.4.1/better_web3/utils/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     1398 2023-07-11 06:39:33.869000 better_web3-1.4.1/better_web3/utils/__pycache__/other.cpython-311.pyc
--rw-r--r--   0        0        0     2131 2023-07-17 08:28:26.617000 better_web3-1.4.1/better_web3/utils/eth.py
--rw-r--r--   0        0        0     1020 2023-06-28 11:42:15.374000 better_web3-1.4.1/better_web3/utils/file.py
--rw-r--r--   0        0        0      663 2023-07-07 20:05:19.087000 better_web3-1.4.1/better_web3/utils/other.py
--rw-r--r--   0        0        0     3172 2023-07-17 10:00:37.875000 better_web3-1.4.1/better_web3/wallet.py
--rw-r--r--   0        0        0      412 2023-07-23 08:52:53.613000 better_web3-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      479 2023-07-07 17:47:32.398000 better_web3-1.4.1/README.md
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 better_web3-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      403 2023-07-17 08:30:00.413000 better_web3-1.5.0/better_web3/__init__.py
+-rw-r--r--   0        0        0    10461 2023-07-17 08:28:26.368000 better_web3-1.5.0/better_web3/batch_call.py
+-rw-r--r--   0        0        0    14931 2023-07-26 13:56:34.907000 better_web3-1.5.0/better_web3/chain.py
+-rw-r--r--   0        0        0      251 2023-07-07 12:10:25.885000 better_web3-1.5.0/better_web3/contract/__init__.py
+-rw-r--r--   0        0        0      525 2023-07-11 06:39:31.842000 better_web3-1.5.0/better_web3/contract/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      687 2023-07-11 06:39:33.730000 better_web3-1.5.0/better_web3/contract/__pycache__/_abi.cpython-311.pyc
+-rw-r--r--   0        0        0      351 2023-06-05 07:45:48.569000 better_web3-1.5.0/better_web3/contract/__pycache__/_paths.cpython-311.pyc
+-rw-r--r--   0        0        0     2938 2023-07-11 06:39:31.913000 better_web3-1.5.0/better_web3/contract/__pycache__/contract.cpython-311.pyc
+-rw-r--r--   0        0        0     1938 2023-07-11 06:39:34.027000 better_web3-1.5.0/better_web3/contract/__pycache__/disperse.cpython-311.pyc
+-rw-r--r--   0        0        0     3687 2023-07-11 06:39:34.086000 better_web3-1.5.0/better_web3/contract/__pycache__/erc20.cpython-311.pyc
+-rw-r--r--   0        0        0     5293 2023-07-11 06:39:34.163000 better_web3-1.5.0/better_web3/contract/__pycache__/erc721.cpython-311.pyc
+-rw-r--r--   0        0        0     9601 2023-07-11 06:39:33.679000 better_web3-1.5.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc
+-rw-r--r--   0        0        0      352 2023-07-07 12:03:06.296000 better_web3-1.5.0/better_web3/contract/_abi.py
+-rw-r--r--   0        0        0       99 2023-06-05 07:40:59.317000 better_web3-1.5.0/better_web3/contract/_paths.py
+-rw-r--r--   0        0        0     1193 2023-06-23 09:34:50.869000 better_web3-1.5.0/better_web3/contract/abi/disperse.json
+-rw-r--r--   0        0        0     6301 2023-06-05 07:31:12.380000 better_web3-1.5.0/better_web3/contract/abi/erc1155.json
+-rw-r--r--   0        0        0     5904 2023-06-05 07:28:35.070000 better_web3-1.5.0/better_web3/contract/abi/erc20.json
+-rw-r--r--   0        0        0     6755 2023-06-05 07:31:25.078000 better_web3-1.5.0/better_web3/contract/abi/erc721.json
+-rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-1.5.0/better_web3/contract/abi/multicall_v3.json
+-rw-r--r--   0        0        0     1264 2023-07-10 08:18:27.356000 better_web3-1.5.0/better_web3/contract/contract.py
+-rw-r--r--   0        0        0      974 2023-07-07 12:13:30.821000 better_web3-1.5.0/better_web3/contract/disperse.py
+-rw-r--r--   0        0        0     1747 2023-07-07 20:11:33.426000 better_web3-1.5.0/better_web3/contract/erc20.py
+-rw-r--r--   0        0        0     2876 2023-07-07 20:11:33.364000 better_web3-1.5.0/better_web3/contract/erc721.py
+-rw-r--r--   0        0        0     6201 2023-07-07 12:07:18.259000 better_web3-1.5.0/better_web3/contract/multicall.py
+-rw-r--r--   0        0        0     4059 2023-07-26 11:29:17.505000 better_web3-1.5.0/better_web3/proxy.py
+-rw-r--r--   0        0        0      730 2023-07-17 08:28:26.473000 better_web3-1.5.0/better_web3/utils/__init__.py
+-rw-r--r--   0        0        0      917 2023-07-17 08:28:28.447000 better_web3-1.5.0/better_web3/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4132 2023-07-17 08:28:28.496000 better_web3-1.5.0/better_web3/utils/__pycache__/eth.cpython-311.pyc
+-rw-r--r--   0        0        0     3469 2023-06-28 12:32:10.861000 better_web3-1.5.0/better_web3/utils/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     1398 2023-07-11 06:39:33.869000 better_web3-1.5.0/better_web3/utils/__pycache__/other.cpython-311.pyc
+-rw-r--r--   0        0        0     2131 2023-07-17 08:28:26.617000 better_web3-1.5.0/better_web3/utils/eth.py
+-rw-r--r--   0        0        0     1020 2023-06-28 11:42:15.374000 better_web3-1.5.0/better_web3/utils/file.py
+-rw-r--r--   0        0        0      663 2023-07-07 20:05:19.087000 better_web3-1.5.0/better_web3/utils/other.py
+-rw-r--r--   0        0        0     3227 2023-07-26 11:29:17.244000 better_web3-1.5.0/better_web3/wallet.py
+-rw-r--r--   0        0        0      412 2023-07-26 11:29:17.377000 better_web3-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      479 2023-07-07 17:47:32.398000 better_web3-1.5.0/README.md
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 better_web3-1.5.0/PKG-INFO
```

### Comparing `better_web3-1.4.1/better_web3/batch_call.py` & `better_web3-1.5.0/better_web3/batch_call.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/chain.py` & `better_web3-1.5.0/better_web3/chain.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     TxParams,
     TxReceipt,
     Wei,
 )
 
 from .batch_call import BatchCallManager
 from .contract import Contract, Multicall, Disperse, ERC20, ERC721
-from .enums import TxSpeed
 from .utils import link_by_tx_hash
 
 
 @dataclass
 class NativeToken:
     symbol: str = "ETH"
     decimals: int = 18
@@ -55,44 +54,48 @@
             multicall_v3_contract_address: ChecksumAddress | str = None,
             # Disperse
             disperse_contract_address: ChecksumAddress | str = None,
             # Batch request
             batch_request_size: int = 10,
             batch_request_delay: int = 1,
             # Tx params
+            gas: int = None,
+            # legacy pricing
             gas_price: Wei | int = None,
+            # dynamic fee pricing
+            max_fee_per_gas: Wei | int = None,
+            max_priority_fee_per_gas: Wei | int = None,
     ):
         self._rpc = rpc
         self.name = name
         self.is_testnet = is_testnet
         self.token = NativeToken(symbol=symbol, decimals=decimals)
         self.explorer_url = explorer_url
         self.use_eip1559 = use_eip1559
 
         self.http_session = self._prepare_http_session(retry_count)
         self.timeout = provider_timeout
-        self.slow_timeout = slow_provider_timeout
 
         self.w3_provider = self._create_http_provider(provider_timeout)
-        self.w3_slow_provider = self._create_http_provider(slow_provider_timeout)
 
         self.w3 = Web3(provider=self.w3_provider)
-        self.slow_w3 = Web3(provider=self.w3_slow_provider)
 
         if use_poa_middleware:
             self.w3.middleware_onion.inject(geth_poa_middleware, layer=0)
-            self.slow_w3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
         self.multicall = Multicall(chain=self, address=multicall_v3_contract_address)
         self.disperse = Disperse(chain=self, address=disperse_contract_address)
 
         self.batch_request = BatchCallManager(
             self, batch_request_size, batch_request_delay)
 
-        self.gas_price = gas_price
+        self.default_gas = gas
+        self.default_gas_price = gas_price
+        self.default_max_fee_per_gas = max_fee_per_gas
+        self.default_max_priority_fee_per_gas = max_priority_fee_per_gas
 
     def _create_http_provider(self, timeout: int) -> HTTPProvider:
         return HTTPProvider(
             self._rpc,
             request_kwargs={"timeout": timeout},
             session=self.http_session,
         )
@@ -238,66 +241,49 @@
             value: Wei | int,
             *,
             gas: int = None,
             nonce: Nonce | int = None,
             # legacy pricing
             gas_price: Wei | int = None,
             # dynamic fee pricing
-            max_fee_per_gas: Wei = None,
-            max_priority_fee_per_gas: Wei = None,
-            tx_speed: TxSpeed = TxSpeed.NORMAL,
+            max_fee_per_gas: Wei | int = None,
+            max_priority_fee_per_gas: Wei | int = None,
     ) -> HexStr:
-        gas_price = gas_price or self.gas_price
+        gas_price = gas_price or self.default_gas_price
         tx_params = self._build_tx_base_params(gas, account_from.address, address_to, nonce, value)
         gas = self.w3.eth.estimate_gas(tx_params)
         tx_params = self._build_tx_base_params(gas, tx_params=tx_params)
         tx_params = self._build_tx_fee_params(
-            gas_price, max_fee_per_gas, max_priority_fee_per_gas, tx_speed, tx_params=tx_params)
+            gas_price, max_fee_per_gas, max_priority_fee_per_gas, tx_params=tx_params)
         return self.sign_and_send_tx(account_from, tx_params)
 
     def transfer_all(
             self,
             account_from: LocalAccount,
             address_to: Address | ChecksumAddress | str,
             *,
             gas: int = None,
             nonce: Nonce | int = None,
             # legacy pricing
             gas_price: Wei | int = None,
             # dynamic fee pricing
-            max_fee_per_gas: Wei = None,
-            max_priority_fee_per_gas: Wei = None,
-            tx_speed: TxSpeed = TxSpeed.NORMAL,
+            max_fee_per_gas: Wei | int = None,
+            max_priority_fee_per_gas: Wei | int = None,
     ):
         raise NotImplementedError  # TODO Реализовать метод Chain.transfer_all()
 
     ################################################################################
     # Gas price shortcuts
     ################################################################################
 
-    def get_gas_price(self) -> Wei:
+    def request_gas_price(self) -> Wei:
         return self.w3.eth.gas_price
 
-    def estimate_eip1559_fees(self, tx_speed: TxSpeed = TxSpeed.NORMAL) -> tuple[int, int]:
-        tx_speed_percentiles = {
-            TxSpeed.SLOWEST: 0,
-            TxSpeed.VERY_SLOW: 10,
-            TxSpeed.SLOW: 25,
-            TxSpeed.NORMAL: 50,
-            TxSpeed.FAST: 75,
-            TxSpeed.VERY_FAST: 90,
-            TxSpeed.FASTEST: 100,
-        }
-        percentile = tx_speed_percentiles[tx_speed]
-        result = self.w3.eth.fee_history(1, "latest", reward_percentiles=[percentile])
-        # Get next block `base_fee_per_gas`
-        base_fee_per_gas = result["baseFeePerGas"][-1]
-        max_priority_fee_per_gas = result["reward"][0][0]
-        max_fee_per_gas = base_fee_per_gas + max_priority_fee_per_gas
-        return max_fee_per_gas, max_priority_fee_per_gas
+    def request_max_priority_fee(self) -> Wei:
+        return self.w3.eth.max_priority_fee
 
     ################################################################################
     # Working with transactions
     ################################################################################
 
     def _send_tx(self, tx: TxParams) -> HexBytes:
         return self.w3.eth.send_transaction(tx)
@@ -307,15 +293,15 @@
 
     def _build_tx_base_params(
             self,
             gas: int = None,
             address_from: Address | ChecksumAddress | str = None,
             address_to: Address | ChecksumAddress | str = None,
             nonce: Nonce | int = None,
-            value: Wei = None,
+            value: Wei | int = None,
             *,
             tx_params: TxParams = None,
     ) -> TxParams:
         if tx_params is None:
             tx_params = dict()
         tx_params = tx_params.copy()
 
@@ -336,38 +322,36 @@
             tx_params["nonce"] = self.get_nonce(address_from)
 
         return tx_params
 
     def _build_tx_fee_params(
             self,
             # legacy pricing
-            gas_price: Wei = None,
+            gas_price: Wei | int = None,
             # dynamic fee pricing
-            max_fee_per_gas: Wei = None,
-            max_priority_fee_per_gas: Wei = None,
-            tx_speed: TxSpeed = TxSpeed.NORMAL,
+            max_fee_per_gas: Wei | int = None,
+            max_priority_fee_per_gas: Wei | int = None,
             *,
             tx_params: TxParams = None,
     ) -> TxParams:
         if tx_params is None:
             tx_params = dict()
         tx_params = tx_params.copy()
 
+        max_fee_per_gas = max_fee_per_gas or self.default_max_fee_per_gas
+        max_priority_fee_per_gas = max_priority_fee_per_gas or self.default_max_priority_fee_per_gas
+
         if (self.is_eip1559_supported and
                 ((gas_price is None and self.use_eip1559)
                  or max_fee_per_gas is not None
                  or max_priority_fee_per_gas is not None)):
-            if max_fee_per_gas is None or max_priority_fee_per_gas is None:
-                estimated_max_fee_per_gas, estimated_max_priority_fee_per_gas = self.estimate_eip1559_fees(tx_speed)
-                max_fee_per_gas = max_fee_per_gas or estimated_max_fee_per_gas
-                max_priority_fee_per_gas = max_priority_fee_per_gas or estimated_max_priority_fee_per_gas
-            tx_params["maxFeePerGas"] = max_fee_per_gas
-            tx_params["maxPriorityFeePerGas"] = max_priority_fee_per_gas
+            tx_params["maxFeePerGas"] = max_fee_per_gas or self.request_gas_price()
+            tx_params["maxPriorityFeePerGas"] = max_priority_fee_per_gas or self.request_max_priority_fee()
         else:
-            tx_params["gasPrice"] = gas_price or self.get_gas_price()
+            tx_params["gasPrice"] = gas_price or self.request_gas_price()
 
         return tx_params
 
     def build_tx(
             self,
             contract_function: ContractFunction,
             gas: int = None,
@@ -376,22 +360,21 @@
             nonce: Nonce | int = None,
             value: Wei | int = None,
             # legacy pricing
             gas_price: Wei | int = None,
             # dynamic fee pricing
             max_fee_per_gas: Wei | int = None,
             max_priority_fee_per_gas: Wei | int = None,
-            tx_speed: TxSpeed = TxSpeed.NORMAL,
     ) -> TxParams:
-        gas_price = gas_price or self.gas_price
+        gas_price = gas_price or self.default_gas_price
         tx_params = self._build_tx_base_params(gas, address_from, address_to, nonce, value)
         gas = contract_function.estimate_gas(tx_params)
         tx_params = self._build_tx_base_params(gas, tx_params=tx_params)
         tx_params = self._build_tx_fee_params(
-            gas_price, max_fee_per_gas, max_priority_fee_per_gas, tx_speed, tx_params=tx_params)
+            gas_price, max_fee_per_gas, max_priority_fee_per_gas, tx_params=tx_params)
         return contract_function.build_transaction(tx_params)
 
     def sign_and_send_tx(self, account: LocalAccount, tx: TxParams) -> HexStr:
         signed_tx = account.sign_transaction(tx)
         tx_hash = self._send_raw_tx(signed_tx.rawTransaction)
         return HexStr(tx_hash.hex())
 
@@ -404,22 +387,20 @@
             nonce: Nonce | int = None,
             value: Wei | int = None,
             # legacy pricing
             gas_price: Wei | int = None,
             # dynamic fee pricing
             max_fee_per_gas: Wei | int = None,
             max_priority_fee_per_gas: Wei | int = None,
-            tx_speed: TxSpeed = TxSpeed.NORMAL,
     ) -> HexStr:
         tx = self.build_tx(
             fn,
             address_from=account.address,
             gas=gas,
             nonce=nonce,
             value=value,
             gas_price=gas_price,
             max_fee_per_gas=max_fee_per_gas,
             max_priority_fee_per_gas=max_priority_fee_per_gas,
-            tx_speed=tx_speed,
         )
         tx_hash = self.sign_and_send_tx(account, tx)
         return tx_hash
```

### Comparing `better_web3-1.4.1/better_web3/contract/__pycache__/__init__.cpython-311.pyc` & `better_web3-1.5.0/better_web3/contract/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/__pycache__/_abi.cpython-311.pyc` & `better_web3-1.5.0/better_web3/contract/__pycache__/_abi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/__pycache__/contract.cpython-311.pyc` & `better_web3-1.5.0/better_web3/contract/__pycache__/contract.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/__pycache__/disperse.cpython-311.pyc` & `better_web3-1.5.0/better_web3/contract/__pycache__/disperse.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/__pycache__/erc20.cpython-311.pyc` & `better_web3-1.5.0/better_web3/contract/__pycache__/erc20.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/__pycache__/erc721.cpython-311.pyc` & `better_web3-1.5.0/better_web3/contract/__pycache__/erc721.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/__pycache__/multicall.cpython-311.pyc` & `better_web3-1.5.0/better_web3/contract/__pycache__/multicall.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/abi/disperse.json` & `better_web3-1.5.0/better_web3/contract/abi/disperse.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/abi/erc1155.json` & `better_web3-1.5.0/better_web3/contract/abi/erc1155.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/abi/erc20.json` & `better_web3-1.5.0/better_web3/contract/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/abi/erc721.json` & `better_web3-1.5.0/better_web3/contract/abi/erc721.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/abi/multicall_v3.json` & `better_web3-1.5.0/better_web3/contract/abi/multicall_v3.json`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/contract.py` & `better_web3-1.5.0/better_web3/contract/contract.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/disperse.py` & `better_web3-1.5.0/better_web3/contract/disperse.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/erc20.py` & `better_web3-1.5.0/better_web3/contract/erc20.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/erc721.py` & `better_web3-1.5.0/better_web3/contract/erc721.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/contract/multicall.py` & `better_web3-1.5.0/better_web3/contract/multicall.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/proxy.py` & `better_web3-1.5.0/better_web3/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                 + f"{self.ip}:{self.port}")
 
     def __repr__(self):
         return f"Proxy(ip={self.ip}, port={self.port})"
 
     def __str__(self) -> str:
         info = f"[{self.number:03}] [{self.ip:>15}:{str(self.port):<5}]"
-        if self.tags: info += f" ({', '.join(self.tags)})"
+        if self.tags: info += f" ({', '.join((str(tag) for tag in self.tags))})"
         return info
 
     def __hash__(self):
         return hash((self.ip, self.port, self.protocol, self.login, self.password))
 
     def __eq__(self, other):
         if isinstance(other, Proxy):
```

### Comparing `better_web3-1.4.1/better_web3/utils/__init__.py` & `better_web3-1.5.0/better_web3/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/utils/__pycache__/__init__.cpython-311.pyc` & `better_web3-1.5.0/better_web3/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/utils/__pycache__/eth.cpython-311.pyc` & `better_web3-1.5.0/better_web3/utils/__pycache__/eth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/utils/__pycache__/file.cpython-311.pyc` & `better_web3-1.5.0/better_web3/utils/__pycache__/file.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/utils/__pycache__/other.cpython-311.pyc` & `better_web3-1.5.0/better_web3/utils/__pycache__/other.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/utils/eth.py` & `better_web3-1.5.0/better_web3/utils/eth.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/utils/file.py` & `better_web3-1.5.0/better_web3/utils/file.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/utils/other.py` & `better_web3-1.5.0/better_web3/utils/other.py`

 * *Files identical despite different names*

### Comparing `better_web3-1.4.1/better_web3/wallet.py` & `better_web3-1.5.0/better_web3/wallet.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         Wallet._number += 1
 
     def __repr__(self):
         return f"Wallet(address={self.address})"
 
     def __str__(self) -> str:
         info = f"[{self.number:03}] [{self.address}]"
-        if self.tags: info += f" ({', '.join(self.tags)})"
+        if self.tags: info += f" ({', '.join((str(tag) for tag in self.tags))})"
         return info
 
     @classmethod
     def generate(cls, extra_entropy: str = "", tags: Iterable[str] = None) -> "Wallet":
         account = Account.create(extra_entropy)
         return cls(account, tags=tags)
 
@@ -83,12 +83,12 @@
 
     def tx_receipt(self, chain: Chain, tx_receipt: TxReceipt | str, value: Wei | int = None) -> str:
         tx_hash = tx_receipt.transactionHash.hex()
         message = self.tx_hash(chain, tx_hash, value)
         tx_fee_wei = tx_receipt.gasUsed * tx_receipt.effectiveGasPrice
         tx_fee = from_wei(tx_fee_wei, "ether")
         message += f"\n\tFee: {tx_fee} {chain.token.symbol}"
-        nonce = tx_receipt.transactionIndex
-        message += f"\n\tNonce: {nonce}"
+        # position = tx_receipt.transactionIndex
+        # message += f"\n\tPosition (Transaction index): {position}"
         status = tx_receipt.status
         message += f"\n\tStatus: {status}"
         return message
```

### Comparing `better_web3-1.4.1/PKG-INFO` & `better_web3-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-web3
-Version: 1.4.1
+Version: 1.5.0
 Summary: Chains, Contracts(Multicall, Disperse, ERC20/ERC721), batch calls and other..
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: web3 (>=6.6.1,<7.0.0)
```

