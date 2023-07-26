# Comparing `tmp/empiric_network-1.6.6.tar.gz` & `tmp/empiric_network-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empiric_network-1.6.6.tar", max compression
+gzip compressed data, was "empiric_network-1.6.7.tar", max compression
```

## Comparing `empiric_network-1.6.6.tar` & `empiric_network-1.6.7.tar`

### file list

```diff
@@ -1,42 +1,47 @@
--rw-r--r--   0        0        0      284 2023-07-16 09:13:07.883196 empiric_network-1.6.6/README.md
--rw-r--r--   0        0        0        0 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/__init__.py
--rw-r--r--   0        0        0      193 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/__init__.py
--rw-r--r--   0        0        0      284 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/abis/__init__.py
--rw-r--r--   0        0        0    14135 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/abis/oracle.py
--rw-r--r--   0        0        0     1436 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/abis/proxy.py
--rw-r--r--   0        0        0     3896 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/abis/publisher_registry.py
--rw-r--r--   0        0        0     5912 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/abis/randomness.py
--rw-r--r--   0        0        0      868 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/abis/summary_stats.py
--rw-r--r--   0        0        0     4257 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/client.py
--rw-r--r--   0        0        0     2618 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/config.py
--rw-r--r--   0        0        0     3919 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/contract.py
--rw-r--r--   0        0        0     9972 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/entry.py
--rw-r--r--   0        0        0      387 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/logger.py
--rw-r--r--   0        0        0      295 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/mixins/__init__.py
--rw-r--r--   0        0        0    25441 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/mixins/evm.py
--rw-r--r--   0        0        0     3074 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/mixins/nonce.py
--rw-r--r--   0        0        0     8808 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/mixins/oracle.py
--rw-r--r--   0        0        0     2287 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/mixins/publisher_registry.py
--rw-r--r--   0        0        0     3065 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/mixins/randomness.py
--rw-r--r--   0        0        0      669 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/mixins/transactions.py
--rw-r--r--   0        0        0     4177 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/types.py
--rw-r--r--   0        0        0      880 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/core/utils.py
--rw-r--r--   0        0        0       82 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/__init__.py
--rw-r--r--   0        0        0     2716 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/assets.py
--rw-r--r--   0        0        0     2261 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/client.py
--rw-r--r--   0        0        0      354 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/__init__.py
--rw-r--r--   0        0        0     3755 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/ascendex.py
--rw-r--r--   0        0        0     3017 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/bitstamp.py
--rw-r--r--   0        0        0     3380 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/cex.py
--rw-r--r--   0        0        0     2953 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/coinbase.py
--rw-r--r--   0        0        0     3980 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/coingecko.py
--rw-r--r--   0        0        0     3826 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/defillama.py
--rw-r--r--   0        0        0     3814 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/gemini.py
--rw-r--r--   0        0        0     3754 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/kaiko.py
--rw-r--r--   0        0        0     3631 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/okx.py
--rw-r--r--   0        0        0     3762 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/fetchers/thegraph.py
--rw-r--r--   0        0        0      668 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/publisher/types.py
--rw-r--r--   0        0        0        0 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/test/__init__.py
--rw-r--r--   0        0        0     5965 2023-07-16 09:13:07.883196 empiric_network-1.6.6/empiric/test/interface_consistency.py
--rw-r--r--   0        0        0     1016 2023-07-16 09:13:07.883196 empiric_network-1.6.6/pyproject.toml
--rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 empiric_network-1.6.6/PKG-INFO
+-rw-r--r--   0        0        0      284 2023-07-26 20:36:55.629989 empiric_network-1.6.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/__init__.py
+-rw-r--r--   0        0        0      284 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/abis/__init__.py
+-rw-r--r--   0        0        0    31179 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/abis/oracle.py
+-rw-r--r--   0        0        0     1436 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/abis/proxy.py
+-rw-r--r--   0        0        0     3896 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/abis/publisher_registry.py
+-rw-r--r--   0        0        0     5912 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/abis/randomness.py
+-rw-r--r--   0        0        0      868 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/abis/summary_stats.py
+-rw-r--r--   0        0        0     4257 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/client.py
+-rw-r--r--   0        0        0     2618 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/config.py
+-rw-r--r--   0        0        0     3922 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/contract.py
+-rw-r--r--   0        0        0    10045 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/entry.py
+-rw-r--r--   0        0        0      387 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/logger.py
+-rw-r--r--   0        0        0      295 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/mixins/__init__.py
+-rw-r--r--   0        0        0    25441 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/mixins/evm.py
+-rw-r--r--   0        0        0     3074 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/mixins/nonce.py
+-rw-r--r--   0        0        0     9442 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/mixins/oracle.py
+-rw-r--r--   0        0        0     2287 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/mixins/publisher_registry.py
+-rw-r--r--   0        0        0     3065 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/mixins/randomness.py
+-rw-r--r--   0        0        0      669 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/mixins/transactions.py
+-rw-r--r--   0        0        0     4177 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/types.py
+-rw-r--r--   0        0        0      880 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/core/utils.py
+-rw-r--r--   0        0        0       82 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/__init__.py
+-rw-r--r--   0        0        0     3368 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/assets.py
+-rw-r--r--   0        0        0     2262 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/client.py
+-rw-r--r--   0        0        0      354 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/__init__.py
+-rw-r--r--   0        0        0     3755 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/ascendex.py
+-rw-r--r--   0        0        0     3017 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/bitstamp.py
+-rw-r--r--   0        0        0     3380 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/cex.py
+-rw-r--r--   0        0        0     2953 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/coinbase.py
+-rw-r--r--   0        0        0     3980 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/coingecko.py
+-rw-r--r--   0        0        0     3826 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/defillama.py
+-rw-r--r--   0        0        0     3814 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/gemini.py
+-rw-r--r--   0        0        0     3754 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/kaiko.py
+-rw-r--r--   0        0        0     3631 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/okx.py
+-rw-r--r--   0        0        0     3762 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/fetchers/thegraph.py
+-rw-r--r--   0        0        0       71 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/future_fetchers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/future_fetchers/binance.py
+-rw-r--r--   0        0        0     3791 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/future_fetchers/bybit.py
+-rw-r--r--   0        0        0     5675 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/future_fetchers/okx.py
+-rw-r--r--   0        0        0     4282 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/future_fetchers/test.py
+-rw-r--r--   0        0        0      668 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/publisher/types.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/test/__init__.py
+-rw-r--r--   0        0        0     5965 2023-07-26 20:36:55.629989 empiric_network-1.6.7/empiric/test/interface_consistency.py
+-rw-r--r--   0        0        0     1016 2023-07-26 20:36:55.629989 empiric_network-1.6.7/pyproject.toml
+-rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 empiric_network-1.6.7/PKG-INFO
```

### Comparing `empiric_network-1.6.6/empiric/core/abis/proxy.py` & `empiric_network-1.6.7/empiric/core/abis/proxy.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/core/abis/publisher_registry.py` & `empiric_network-1.6.7/empiric/core/abis/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/core/abis/randomness.py` & `empiric_network-1.6.7/empiric/core/abis/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/core/abis/summary_stats.py` & `empiric_network-1.6.7/empiric/core/abis/summary_stats.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/core/client.py` & `empiric_network-1.6.7/empiric/core/client.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/core/config.py` & `empiric_network-1.6.7/empiric/core/config.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/core/contract.py` & `empiric_network-1.6.7/empiric/core/contract.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,26 +42,27 @@
 
     transaction = await self._account.sign_invoke_transaction(
         calls=self,
         max_fee=self.max_fee,
         auto_estimate=auto_estimate,
     )
     response = await self._client.send_transaction(transaction)
+
     if callback:
         await callback(transaction.nonce, response.transaction_hash)
 
     invoke_result = InvokeResult(
         hash=response.transaction_hash,
         _client=self._client,
         contract=self._contract_data,
         invoke_transaction=transaction,
     )
 
     # don't return invoke result until it is received or errors
-    await wait_for_received(self._client, invoke_result.hash)
+    # await wait_for_received(self._client, invoke_result.hash)
 
     return invoke_result
 
 
 async def wait_for_received(
     client,
     tx_hash,
```

### Comparing `empiric_network-1.6.6/empiric/core/entry.py` & `empiric_network-1.6.7/empiric/core/entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -220,82 +220,83 @@
         return list(filter(lambda item: item is not None, serialized_entries))
 
     def __repr__(self):
         return f'SpotEntry(pair_id="{felt_to_str(self.pair_id)}", price={self.price}, timestamp={self.base.timestamp}, source="{felt_to_str(self.base.source)}", publisher="{felt_to_str(self.base.publisher)}, volume={self.volume})")'
 
 
 class FutureEntry(Entry):
-    timestamp: int
-    source: int
-    publisher: int
+    base : BaseEntry
     pair_id: int
     price: int
     expiry_timestamp: int
+    volume :int 
 
-    def __init__(self, timestamp, source, publisher, pair_id, price, expiry_timestamp):
+    def __init__(self, timestamp, source, publisher, pair_id, price, expiry_timestamp, volume):
         if type(pair_id) == str:
             pair_id = str_to_felt(pair_id)
 
         if type(publisher) == str:
             publisher = str_to_felt(publisher)
 
         if type(source) == str:
             source = str_to_felt(source)
 
-        if type(expiry_timestamp) == str:
-            expiry_timestamp = str_to_felt(expiry_timestamp)
-
         self.base = BaseEntry(timestamp, source, publisher)
         self.pair_id = pair_id
         self.price = price
         self.expiry_timestamp = expiry_timestamp
+        self.volume = volume
 
     def __eq__(self, other):
         if isinstance(other, FutureEntry):
             return (
                 self.pair_id == other.pair_id
                 and self.price == other.price
                 and self.base.timestamp == other.base.timestamp
                 and self.base.source == other.base.source
                 and self.base.publisher == other.base.publisher
                 and self.expiry_timestamp == other.expiry_timestamp
+                and self.volume == other.volume
             )
         # This supports comparing against entries that are returned by starknet.py,
         # which will be namedtuples.
         if isinstance(other, Tuple) and len(other) == 4:
             return (
                 self.pair_id == other.pair_id
                 and self.price == other.price
                 and self.base.timestamp == other.base.timestamp
                 and self.base.source == other.base.source
                 and self.base.publisher == other.base.publisher
                 and self.expiry_timestamp == other.expiry_timestamp
+                and self.volume == other.volume
             )
         return False
 
     def to_tuple(self):
         return (
             self.base.timestamp,
             self.base.source,
             self.base.publisher,
             self.pair_id,
             self.price,
             self.expiry_timestamp,
+            self.volume,
         )
 
     def serialize(self) -> Dict[str, str]:
         return {
             "base": {
                 "timestamp": self.base.timestamp,
                 "source": self.base.source,
                 "publisher": self.base.publisher,
             },
             "pair_id": self.pair_id,
             "price": self.price,
             "expiry_timestamp": self.expiry_timestamp,
+            "volume": self.volume,
         }
 
     @staticmethod
     def serialize_entries(entries: List[FutureEntry]) -> List[Dict[str, int]]:
         """serialize entries to a List of dictionaries"""
         # TODO (rlkelly): log errors
         serialized_entries = [
```

### Comparing `empiric_network-1.6.6/empiric/core/mixins/evm.py` & `empiric_network-1.6.7/empiric/core/mixins/evm.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/core/mixins/nonce.py` & `empiric_network-1.6.7/empiric/core/mixins/nonce.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/core/mixins/oracle.py` & `empiric_network-1.6.7/empiric/core/mixins/oracle.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             },
             max_fee=max_fee,
         )
         return invocation
 
     async def publish_many(
         self,
-        entries: List[SpotEntry],
+        entries: List[any],
         pagination: Optional[int] = 40,
         max_fee=int(1e18),
     ) -> List[InvokeResult]:
         if len(entries) == 0:
             logger.warning("Skipping publishing as entries array is empty")
             return
 
@@ -210,14 +210,33 @@
             pair_id,
             aggregation_mode,
             callback=self.track_nonce,
             max_fee=max_fee,
         )
         return invocation
 
+    async def set_future_checkpoint(
+        self,
+        pair_id: int,
+        expiry_timestamp: int,
+        aggregation_mode: int = str_to_felt("MEDIAN"),
+        max_fee=int(1e16),
+    ) -> InvokeResult:
+        if not self.is_user_client:
+            raise AttributeError(
+                "Must set account.  You may do this by invoking self._setup_account_client(private_key, account_contract_address)"
+            )
+        invocation = await self.oracle.set_future_checkpoint.invoke(
+            pair_id,
+            expiry_timestamp,
+            aggregation_mode,
+            max_fee=max_fee,
+        )
+        return invocation
+
     async def set_checkpoints(
         self,
         pair_ids: List[int],
         aggregation_mode: int = str_to_felt("MEDIAN"),
         max_fee=int(1e18),
         pagination: Optional[int] = 15,
     ) -> InvokeResult:
```

### Comparing `empiric_network-1.6.6/empiric/core/mixins/publisher_registry.py` & `empiric_network-1.6.7/empiric/core/mixins/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/core/mixins/randomness.py` & `empiric_network-1.6.7/empiric/core/mixins/randomness.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/core/mixins/transactions.py` & `empiric_network-1.6.7/empiric/core/mixins/transactions.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/core/types.py` & `empiric_network-1.6.7/empiric/core/types.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/core/utils.py` & `empiric_network-1.6.7/empiric/core/utils.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/publisher/client.py` & `empiric_network-1.6.7/empiric/publisher/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 from typing import List
 
 import aiohttp
 from empiric.core.client import EmpiricClient
-from empiric.core.entry import SpotEntry
+from empiric.core.entry import SpotEntry, FutureEntry
 from empiric.publisher.types import PublisherInterfaceT
 
 
 class EmpiricPublisherClient(EmpiricClient):
     """
     This client extends the empiric client with functionality for fetching from our third party sources.
     It can be used to synchronously or asynchronously fetch assets using the Asset format, ie.
@@ -41,25 +41,25 @@
 
     def add_fetchers(self, fetchers: List[PublisherInterfaceT]):
         self.fetchers.extend(fetchers)
 
     def add_fetcher(self, fetcher: PublisherInterfaceT):
         self.fetchers.append(fetcher)
 
-    async def fetch(self, filter_exceptions=True) -> List[SpotEntry]:
+    async def fetch(self, filter_exceptions=True) -> List[any]:
         tasks = []
         timeout = aiohttp.ClientTimeout(total=10)  # 10 seconds per request
         async with aiohttp.ClientSession(timeout=timeout) as session:
             for fetcher in self.fetchers:
                 data = fetcher.fetch(session)
                 tasks.append(data)
             result = await asyncio.gather(*tasks, return_exceptions=True)
             if filter_exceptions:
                 result = [subl for subl in result if not isinstance(subl, Exception)]
             return [val for subl in result for val in subl]
 
-    def fetch_sync(self) -> List[SpotEntry]:
+    def fetch_sync(self) -> List[any]:
         results = []
         for fetcher in self.fetchers:
             data = fetcher.fetch_sync()
             results.extend(data)
         return results
```

### Comparing `empiric_network-1.6.6/empiric/publisher/fetchers/ascendex.py` & `empiric_network-1.6.7/empiric/publisher/fetchers/ascendex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/publisher/fetchers/bitstamp.py` & `empiric_network-1.6.7/empiric/publisher/fetchers/bitstamp.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/publisher/fetchers/cex.py` & `empiric_network-1.6.7/empiric/publisher/fetchers/cex.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/publisher/fetchers/coinbase.py` & `empiric_network-1.6.7/empiric/publisher/fetchers/coinbase.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/publisher/fetchers/coingecko.py` & `empiric_network-1.6.7/empiric/publisher/fetchers/coingecko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/publisher/fetchers/defillama.py` & `empiric_network-1.6.7/empiric/publisher/fetchers/defillama.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/publisher/fetchers/gemini.py` & `empiric_network-1.6.7/empiric/publisher/fetchers/gemini.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/publisher/fetchers/kaiko.py` & `empiric_network-1.6.7/empiric/publisher/fetchers/kaiko.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/publisher/fetchers/okx.py` & `empiric_network-1.6.7/empiric/publisher/fetchers/okx.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/publisher/fetchers/thegraph.py` & `empiric_network-1.6.7/empiric/publisher/fetchers/thegraph.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/publisher/types.py` & `empiric_network-1.6.7/empiric/publisher/types.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/empiric/test/interface_consistency.py` & `empiric_network-1.6.7/empiric/test/interface_consistency.py`

 * *Files identical despite different names*

### Comparing `empiric_network-1.6.6/pyproject.toml` & `empiric_network-1.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "empiric-network"
-version = "1.6.6"
+version = "1.6.7"
 authors = ["Pragma <contact@pragmaoracle.com>"]
 description = "Core package for rollup-native Pragma Oracle"
 readme = "README.md"
 homepage = "https://pragmaoracle.com"
 repository = "https://github.com/Astraly-Labs/Pragma"
 documentation = "https://docs.pragmaoracle.com"
 classifiers = [
```

### Comparing `empiric_network-1.6.6/PKG-INFO` & `empiric_network-1.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empiric-network
-Version: 1.6.6
+Version: 1.6.7
 Summary: Core package for rollup-native Pragma Oracle
 Home-page: https://pragmaoracle.com
 Author: Pragma
 Author-email: contact@pragmaoracle.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

