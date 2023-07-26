# Comparing `tmp/rubi-2.2.1.tar.gz` & `tmp/rubi-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.2.1.tar", max compression
+gzip compressed data, was "rubi-2.3.0.tar", max compression
```

## Comparing `rubi-2.2.1.tar` & `rubi-2.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    11357 2023-07-25 22:42:00.027885 rubi-2.2.1/LICENSE
--rw-r--r--   0        0        0     2757 2023-07-25 22:42:00.027885 rubi-2.2.1/README.md
--rw-r--r--   0        0        0     6735 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      833 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/arbitrum_one/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/arbitrum_one/abis/router.json
--rw-r--r--   0        0        0      840 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/arbitrum_one/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      858 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      760 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      832 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0     1746 2023-07-25 22:42:25.812710 rubi-2.2.1/pyproject.toml
--rw-r--r--   0        0        0      124 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/__init__.py
--rw-r--r--   0        0        0    30804 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/client.py
--rw-r--r--   0        0        0      163 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    65755 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/aid.py
--rw-r--r--   0        0        0    12337 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0       74 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/contract_types/__init__.py
--rw-r--r--   0        0        0    15898 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/contract_types/events.py
--rw-r--r--   0        0        0     2805 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/contract_types/transaction_reciept.py
--rw-r--r--   0        0        0    18565 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24880 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/market.py
--rw-r--r--   0        0        0    14915 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/router.py
--rw-r--r--   0        0        0       77 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/data/README.md
--rw-r--r--   0        0        0       31 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/data/__init__.py
--rw-r--r--   0        0        0    17073 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/data/market.py
--rw-r--r--   0        0        0       72 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/network/__init__.py
--rw-r--r--   0        0        0     8475 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/network/network.py
--rw-r--r--   0        0        0      121 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/rubicon_types/__init__.py
--rw-r--r--   0        0        0    16249 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/rubicon_types/order.py
--rw-r--r--   0        0        0    11701 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/rubicon_types/order_query.py
--rw-r--r--   0        0        0     6323 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/rubicon_types/orderbook.py
--rw-r--r--   0        0        0     2779 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/rubicon_types/pair.py
--rw-r--r--   0        0        0    11414 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/rubicon_types/trade_query.py
--rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 rubi-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 21:40:36.050669 rubi-2.3.0/LICENSE
+-rw-r--r--   0        0        0     2757 2023-07-26 21:40:36.050669 rubi-2.3.0/README.md
+-rw-r--r--   0        0        0     6735 2023-07-26 21:40:36.050669 rubi-2.3.0/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-07-26 21:40:36.050669 rubi-2.3.0/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-07-26 21:40:36.050669 rubi-2.3.0/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-26 21:40:36.054669 rubi-2.3.0/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      833 2023-07-26 21:40:36.054669 rubi-2.3.0/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-26 21:40:36.054669 rubi-2.3.0/network_config/arbitrum_one/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-26 21:40:36.054669 rubi-2.3.0/network_config/arbitrum_one/abis/router.json
+-rw-r--r--   0        0        0      840 2023-07-26 21:40:36.054669 rubi-2.3.0/network_config/arbitrum_one/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-26 21:40:36.054669 rubi-2.3.0/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-26 21:40:36.054669 rubi-2.3.0/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      858 2023-07-26 21:40:36.054669 rubi-2.3.0/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-26 21:40:36.054669 rubi-2.3.0/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-26 21:40:36.054669 rubi-2.3.0/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      760 2023-07-26 21:40:36.054669 rubi-2.3.0/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-26 21:40:36.054669 rubi-2.3.0/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-26 21:40:36.054669 rubi-2.3.0/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      832 2023-07-26 21:40:36.054669 rubi-2.3.0/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0     1746 2023-07-26 21:41:05.003143 rubi-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-07-26 21:40:36.054669 rubi-2.3.0/rubi/__init__.py
+-rw-r--r--   0        0        0    33458 2023-07-26 21:40:36.054669 rubi-2.3.0/rubi/client.py
+-rw-r--r--   0        0        0      163 2023-07-26 21:40:36.054669 rubi-2.3.0/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    65755 2023-07-26 21:40:36.054669 rubi-2.3.0/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    15707 2023-07-26 21:40:36.054669 rubi-2.3.0/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0       74 2023-07-26 21:40:36.054669 rubi-2.3.0/rubi/contracts/contract_types/__init__.py
+-rw-r--r--   0        0        0    16374 2023-07-26 21:40:36.054669 rubi-2.3.0/rubi/contracts/contract_types/events.py
+-rw-r--r--   0        0        0     3701 2023-07-26 21:40:36.054669 rubi-2.3.0/rubi/contracts/contract_types/transaction_reciept.py
+-rw-r--r--   0        0        0    18883 2023-07-26 21:40:36.054669 rubi-2.3.0/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    25130 2023-07-26 21:40:36.054669 rubi-2.3.0/rubi/contracts/market.py
+-rw-r--r--   0        0        0    15165 2023-07-26 21:40:36.058669 rubi-2.3.0/rubi/contracts/router.py
+-rw-r--r--   0        0        0       77 2023-07-26 21:40:36.058669 rubi-2.3.0/rubi/data/README.md
+-rw-r--r--   0        0        0       31 2023-07-26 21:40:36.058669 rubi-2.3.0/rubi/data/__init__.py
+-rw-r--r--   0        0        0    17073 2023-07-26 21:40:36.058669 rubi-2.3.0/rubi/data/market.py
+-rw-r--r--   0        0        0       72 2023-07-26 21:40:36.058669 rubi-2.3.0/rubi/network/__init__.py
+-rw-r--r--   0        0        0     8475 2023-07-26 21:40:36.058669 rubi-2.3.0/rubi/network/network.py
+-rw-r--r--   0        0        0      121 2023-07-26 21:40:36.058669 rubi-2.3.0/rubi/rubicon_types/__init__.py
+-rw-r--r--   0        0        0    16249 2023-07-26 21:40:36.058669 rubi-2.3.0/rubi/rubicon_types/order.py
+-rw-r--r--   0        0        0    11701 2023-07-26 21:40:36.058669 rubi-2.3.0/rubi/rubicon_types/order_query.py
+-rw-r--r--   0        0        0     6323 2023-07-26 21:40:36.058669 rubi-2.3.0/rubi/rubicon_types/orderbook.py
+-rw-r--r--   0        0        0     2779 2023-07-26 21:40:36.058669 rubi-2.3.0/rubi/rubicon_types/pair.py
+-rw-r--r--   0        0        0    11414 2023-07-26 21:40:36.058669 rubi-2.3.0/rubi/rubicon_types/trade_query.py
+-rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 rubi-2.3.0/PKG-INFO
```

### Comparing `rubi-2.2.1/LICENSE` & `rubi-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/README.md` & `rubi-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/ERC20.json` & `rubi-2.3.0/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/README.md` & `rubi-2.3.0/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/abitrum_goerli/abis/market.json` & `rubi-2.3.0/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/abitrum_goerli/abis/router.json` & `rubi-2.3.0/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/abitrum_goerli/network.yaml` & `rubi-2.3.0/network_config/abitrum_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/arbitrum_one/abis/market.json` & `rubi-2.3.0/network_config/arbitrum_one/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/arbitrum_one/abis/router.json` & `rubi-2.3.0/network_config/arbitrum_one/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/arbitrum_one/network.yaml` & `rubi-2.3.0/network_config/arbitrum_one/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/optimism/abis/market.json` & `rubi-2.3.0/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/optimism/abis/router.json` & `rubi-2.3.0/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/optimism/network.yaml` & `rubi-2.3.0/network_config/optimism/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/optimism_goerli/abis/market.json` & `rubi-2.3.0/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/optimism_goerli/abis/router.json` & `rubi-2.3.0/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/optimism_goerli/network.yaml` & `rubi-2.3.0/network_config/optimism_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/polygon_mumbai/abis/market.json` & `rubi-2.3.0/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/polygon_mumbai/abis/router.json` & `rubi-2.3.0/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/network_config/polygon_mumbai/network.yaml` & `rubi-2.3.0/network_config/polygon_mumbai/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/pyproject.toml` & `rubi-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rubi"
-version = "2.2.1"
+version = "2.3.0"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 include = ["network_config/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `rubi-2.2.1/rubi/client.py` & `rubi-2.3.0/rubi/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,20 @@
 
 from rubi.contracts import (
     RubiconMarket,
     RubiconRouter,
     ERC20,
     TransactionReceipt,
     EmitFeeEvent,
+    EmitSwap,
+    EmitOfferEvent,
+    EmitTakeEvent,
+    EmitCancelEvent,
 )
+from rubi.data import MarketData
 from rubi.network import (
     Network,
 )
 from rubi.rubicon_types import (
     OrderSide,
     NewMarketOrder,
     NewLimitOrder,
@@ -31,16 +36,14 @@
     OrderEvent,
     Transaction,
     BaseNewOrder,
     NewCancelOrder,
     UpdateLimitOrder,
 )
 
-from rubi.data import MarketData
-
 
 class Client:
     """This class is a client for Rubicon. It aims to provide a simple and understandable interface when interacting
     with the Rubicon protocol. If not instantiated with a wallet and key then all the methods that require signing
     will throw an error.
 
     :param network: A Network instance
@@ -460,106 +463,118 @@
     def place_market_order(self, transaction: Transaction) -> TransactionReceipt:
         """Place a market order transaction by executing the specified transaction object. The transaction
         object should contain a single order of type NewMarketOrder. The order is retrieved from the transaction and
         the corresponding market buy or sell method is called based on the order side.
 
         :param transaction: Transaction object containing the market order.
         :type transaction: Transaction
-        :return: The transaction hash of the executed market order.
-        :rtype: str
+        :return: The transaction receipt of the executed market order.
+        :rtype: TransactionReceipt
         :raises Exception: If the transaction contains more than one order.
         """
         if len(transaction.orders) > 1:
             raise Exception("call place_order with one order only")
 
         order: NewMarketOrder = transaction.orders[0]  # noqa
 
         pair = self.get_pair(pair_name=order.pair)
 
         match order.order_side:
             case OrderSide.BUY:
-                return self.market.buy_all_amount(
+                transaction_receipt = self.market.buy_all_amount(
                     buy_gem=pair.base_asset.address,
                     buy_amt=pair.base_asset.to_integer(order.size),
                     pay_gem=pair.quote_asset.address,
                     max_fill_amount=pair.quote_asset.to_integer(
                         order.worst_execution_price * order.size
                     ),
                     **transaction.args(),
                 )
             case OrderSide.SELL:
-                return self.market.sell_all_amount(
+                transaction_receipt = self.market.sell_all_amount(
                     pay_gem=pair.base_asset.address,
                     pay_amt=pair.base_asset.to_integer(order.size),
                     buy_gem=pair.quote_asset.address,
                     min_fill_amount=pair.quote_asset.to_integer(
                         order.worst_execution_price * order.size
                     ),
                     **transaction.args(),
                 )
+            case _:
+                raise Exception("OrderSide must be BUY or SELL")
+
+        return self._handle_transaction_receipt_raw_events(transaction_receipt)
 
     def place_limit_order(self, transaction: Transaction) -> TransactionReceipt:
         """Place a limit order transaction by executing the specified transaction object. The transaction object should
         contain a single order of type NewLimitOrder.
 
         :param transaction: Transaction object containing the limit order.
         :type transaction: Transaction
-        :return: The transaction hash of the executed limit order.
-        :rtype: str
+        :return: The transaction receipt of the executed limit order.
+        :rtype: TransactionReceipt
         :raises Exception: If the transaction contains more than one order.
         """
         if len(transaction.orders) > 1:
             raise Exception("call place_order with one order only")
 
         order: NewLimitOrder = transaction.orders[0]  # noqa
 
         pair = self.get_pair(pair_name=order.pair)
 
         match order.order_side:
             case OrderSide.BUY:
-                return self.market.offer(
+                transaction_receipt = self.market.offer(
                     pay_amt=pair.quote_asset.to_integer(order.price * order.size),
                     pay_gem=pair.quote_asset.address,
                     buy_amt=pair.base_asset.to_integer(order.size),
                     buy_gem=pair.base_asset.address,
                     **transaction.args(),
                 )
             case OrderSide.SELL:
-                return self.market.offer(
+                transaction_receipt = self.market.offer(
                     pay_amt=pair.base_asset.to_integer(order.size),
                     pay_gem=pair.base_asset.address,
                     buy_amt=pair.quote_asset.to_integer(order.price * order.size),
                     buy_gem=pair.quote_asset.address,
                     **transaction.args(),
                 )
+            case _:
+                raise Exception("OrderSide must be BUY or SELL")
+
+        return self._handle_transaction_receipt_raw_events(transaction_receipt)
 
     def cancel_limit_order(self, transaction: Transaction) -> TransactionReceipt:
         """Place a limit order cancel transaction by executing the specified transaction object. The transaction object
         should contain a single order of type NewCancelOrder.
 
         :param transaction: Transaction object containing the cancel order.
         :type transaction: Transaction
-        :return: The transaction hash of the executed cancel order.
-        :rtype: str
+        :return: The transaction receipt of the executed cancel order.
+        :rtype: TransactionReceipt
         :raises Exception: If the transaction contains more than one order.
         """
         if len(transaction.orders) > 1:
             raise Exception("call place_order with one order only")
 
         order: NewCancelOrder = transaction.orders[0]  # noqa
 
-        return self.market.cancel(id=order.order_id, **transaction.args())
+        transaction_receipt = self.market.cancel(
+            id=order.order_id, **transaction.args()
+        )
+
+        return self._handle_transaction_receipt_raw_events(transaction_receipt)
 
     def batch_place_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Place multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit orders.
         :type transaction: Transaction
-        :return: The transaction hash of the executed batch limit orders.
-        :rtype: str
+        :return: The transaction receipt of the executed batch limit orders.
+        :rtype: TransactionReceipt
         """
         pay_amts = []
         pay_gems = []
         buy_amts = []
         buy_gems = []
 
         for order in transaction.orders:
@@ -578,29 +593,31 @@
                     pay_amts.append(pair.base_asset.to_integer(order.size))
                     pay_gems.append(pair.base_asset.address)
                     buy_amts.append(
                         pair.quote_asset.to_integer(order.price * order.size)
                     )
                     buy_gems.append(pair.quote_asset.address)
 
-        return self.market.batch_offer(
+        transaction_receipt = self.market.batch_offer(
             pay_amts=pay_amts,
             pay_gems=pay_gems,
             buy_amts=buy_amts,
             buy_gems=buy_gems,
             **transaction.args(),
         )
 
+        return self._handle_transaction_receipt_raw_events(transaction_receipt)
+
     def batch_update_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Update multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit order updates.
         :type transaction: Transaction
-        :return: The transaction hash of the executed batch limit order updates.
-        :rtype: str
+        :return: The transaction receipt of the executed batch limit order updates.
+        :rtype: TransactionReceipt
         """
         order_ids = []
         pay_amts = []
         pay_gems = []
         buy_amts = []
         buy_gems = []
 
@@ -622,42 +639,48 @@
                     pay_amts.append(pair.base_asset.to_integer(order.size))
                     pay_gems.append(pair.base_asset.address)
                     buy_amts.append(
                         pair.quote_asset.to_integer(order.price * order.size)
                     )
                     buy_gems.append(pair.quote_asset.address)
 
-        return self.market.batch_requote(
+        transaction_receipt = self.market.batch_requote(
             ids=order_ids,
             pay_amts=pay_amts,
             pay_gems=pay_gems,
             buy_amts=buy_amts,
             buy_gems=buy_gems,
             **transaction.args(),
         )
 
+        return self._handle_transaction_receipt_raw_events(transaction_receipt)
+
     def batch_cancel_limit_orders(self, transaction: Transaction) -> TransactionReceipt:
         """Cancel multiple limit orders in a batch transaction.
 
         :param transaction: Transaction object containing multiple limit order cancellations.
         :type transaction: Transaction
-        :return: The transaction hash of the executed batch limit order cancellations.
-        :rtype: str
+        :return: The transaction receipt of the executed batch limit order cancellations.
+        :rtype: TransactionReceipt
         """
         order_ids = []
 
         for order in transaction.orders:
             order: NewCancelOrder
 
             order_ids.append(order.order_id)
 
-        return self.market.batch_cancel(ids=order_ids, **transaction.args())
+        transaction_receipt = self.market.batch_cancel(
+            ids=order_ids, **transaction.args()
+        )
+
+        return self._handle_transaction_receipt_raw_events(transaction_receipt)
 
     ######################################################################
-    # data methods 
+    # data methods
     ######################################################################
 
     # TODO: i would like to remove pay_gem and buy_gem and follow the same pattern as the get_trades method but do not want to cause breaking changes
     def get_offers(
         self,
         first: int = 10000000,  # TODO: decide on a default value
         order_by: str = "timestamp",
@@ -762,7 +785,53 @@
             )
         )
 
     # TODO: implement this and use check transactions before they go through to prevent failure
     @staticmethod
     def _check_allowance(pair: Pair, order: BaseNewOrder):
         pass
+
+    def _handle_transaction_receipt_raw_events(
+        self, transaction_receipt: TransactionReceipt
+    ) -> TransactionReceipt:
+        """
+        Transforms the raw transaction receipt events to human-readable events
+
+        :param transaction_receipt:
+        :type transaction_receipt: TransactionReceipt
+        :return: The transaction receipt with human-readable events populated
+        :rtype: TransactionReceipt
+        """
+        events: List[OrderEvent] = []
+        for raw_event in transaction_receipt.raw_events:
+            if (
+                isinstance(raw_event, EmitFeeEvent)
+                or isinstance(raw_event, EmitSwap)
+                or isinstance(raw_event, Dict)
+            ):
+                # TODO: handle these events correctly
+                continue
+            else:
+                raw_event: Union[EmitOfferEvent, EmitTakeEvent, EmitCancelEvent]
+
+                event_pair = None
+                for pair in self._pairs.values():
+                    if (
+                        pair.ask_identifier == raw_event.pair
+                        or pair.bid_identifier == raw_event.pair
+                    ):
+                        event_pair = pair
+                        break
+
+                if not event_pair:
+                    # We don't have a pair setup to correctly decode this event
+                    continue
+
+                events.append(
+                    OrderEvent.from_event(
+                        pair=event_pair, event=raw_event, wallet=self.wallet
+                    )
+                )
+
+        transaction_receipt.set_events(events=events)
+
+        return transaction_receipt
```

### Comparing `rubi-2.2.1/rubi/contracts/aid.py` & `rubi-2.3.0/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/rubi/contracts/base_contract.py` & `rubi-2.3.0/rubi/contracts/base_contract.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,73 @@
 import logging as log
 import time
+from enum import Enum
 from threading import Thread
 from time import sleep
-from typing import Optional, Callable, Type, Dict, Any
+from typing import Optional, Callable, Type, Dict, Any, List
 
 from eth_account.datastructures import SignedTransaction
 from eth_typing import ChecksumAddress
+from hexbytes import HexBytes
 from web3 import Web3
 from web3._utils.filters import LogFilter  # noqa
 from web3.contract import Contract
 from web3.contract.contract import (
     ContractFunction,
 )  # TODO: figure out why jupyter notebook is complaining about this
-from web3.types import ABI, Nonce
+from web3.logs import DISCARD
+from web3.types import ABI, Nonce, TxReceipt, EventData
 
 from rubi.contracts.contract_types import BaseEvent, TransactionReceipt
 
 
+class ContractType(Enum):
+    """Enum to distinguish the type of contract instantiated
+
+    Should only be used internally
+    """
+
+    RUBICON_MARKET = "RUBICON_MARKET"
+    RUBICON_ROUTER = "RUBICON_ROUTER"
+    ERC20 = "ERC20"
+
+
 class BaseContract:
     """Base class representation of a contract which defines the structure of a contract and provides several helpful
     methods that can be used by subclass contracts that extend this contract.
 
     :param w3: Web3 instance
     :type w3: Web3
     :param contract: Contract instance
     :type contract: Contract
+    :param contract_type: the type of contract
+    :type contract_type: ContractType
     :param wallet: a wallet address of the signer (optional, default is None)
     :type wallet: Optional[ChecksumAddress]
     :param key: the private key of the signer (optional, default is None)
     :type key: Optional[str]
     """
 
     def __init__(
         self,
         w3: Web3,
         contract: Contract,
+        contract_type: ContractType,
         wallet: Optional[ChecksumAddress] = None,
         key: Optional[str] = None,
     ):
         """constructor method"""
         if (wallet is None) != (key is None):
             raise Exception(
                 "both a wallet and a key are required to sign transactions. provide both or omit both"
             )
 
         self.contract = contract
         self.address = contract.address
+        self.contract_type = contract_type
         self.w3 = w3
         self.chain_id = self.w3.eth.chain_id
 
         # Signing permissions
         self.signing_permissions = wallet is not None and key is not None
 
         if self.signing_permissions:
@@ -61,36 +79,59 @@
 
     @classmethod
     def from_address_and_abi(
         cls,
         w3: Web3,
         address: ChecksumAddress,
         contract_abi: ABI,
+        contract_type: ContractType,
         wallet: Optional[ChecksumAddress] = None,
         key: Optional[str] = None,
     ) -> "BaseContract":
         """Create a BaseContract instance from the contract address and ABI.
 
         :param w3: The Web3 instance.
         :type w3: Web3
         :param address: The address of the contract.
         :type address: ChecksumAddress
         :param contract_abi: The ABI of the contract.
         :type contract_abi: ABI
+        :param contract_type: The type of contract we are instantiating.
+        :type contract_type: ContractType
         :param wallet: The wallet address to use for interacting with the contract (optional, default is None).
         :type wallet: Optional[ChecksumAddress]
         :param key: The private key of the wallet (optional, default is None).
         :type key: Optional[str]
         :return: An instance of BaseContract.
         :rtype: BaseContract
         """
 
         contract = w3.eth.contract(address=address, abi=contract_abi)
 
-        return cls(w3=w3, contract=contract, wallet=wallet, key=key)
+        return cls(
+            w3=w3,
+            contract=contract,
+            contract_type=contract_type,
+            wallet=wallet,
+            key=key,
+        )
+
+    ######################################################################
+    # useful methods
+    ######################################################################
+
+    def get_transaction_receipt(self, transaction_hash: str) -> TransactionReceipt:
+        """Get a transaction receipt for the give transaction_hash.
+
+        :param transaction_hash: The transaction hash.
+        :type transaction_hash: str
+        :return: A TransactionReceipt for the transaction hash.
+        :rtype: TransactionReceipt
+        """
+        return self._wait_for_transaction_receipt(transaction_hash=transaction_hash)
 
     ######################################################################
     # event listeners
     ######################################################################
 
     # TODO: revisit poll time. Right now it is set to block production time of optimism according to:
     #  https://community.optimism.io/docs/protocol/2-rollup-protocol/#block-storage
@@ -281,22 +322,76 @@
             "nonce": nonce,
             "from": self.wallet,
         }
 
         return {key: value for key, value in transaction.items() if value is not None}
 
     def _wait_for_transaction_receipt(
-        self, transaction: SignedTransaction
+        self,
+        transaction: Optional[SignedTransaction] = None,
+        transaction_hash: Optional[str] = None,
     ) -> TransactionReceipt:
         """Wait for the transaction receipt and check if the transaction was successful.
 
         :param transaction: The signed transaction object.
         :type transaction: SignedTransaction
         """
 
+        if transaction:
+            tx_receipt = self.w3.eth.wait_for_transaction_receipt(transaction.hash)
+        elif transaction_hash:
+            tx_receipt = self.w3.eth.wait_for_transaction_receipt(
+                HexBytes(transaction_hash)
+            )
+        else:
+            raise Exception("Provide either a transaction or a transaction_hash")
+
+        raw_events = self._process_receipt_logs_into_raw_events(receipt=tx_receipt)
+
         result = TransactionReceipt.from_tx_receipt(
-            tx_receipt=self.w3.eth.wait_for_transaction_receipt(transaction.hash)
+            tx_receipt=tx_receipt, raw_events=raw_events
         )
 
         log.debug(f"RECEIVED RESULT, timestamp: {time.time_ns()}")
 
         return result
+
+    def _process_receipt_logs_into_raw_events(
+        self, receipt: TxReceipt
+    ) -> List[BaseEvent | EventData]:
+        """
+        Processes the logs of a given transaction receipt and returns a list of events associated with the transaction.
+
+        :param receipt:
+        :type receipt: TxReceipt
+        :return: The list of events associated with the given transaction receipt
+        :rtype: List[BaseEvent]
+        """
+        match self.contract_type:
+            case ContractType.RUBICON_MARKET:
+                event_names = ["emitTake", "emitOffer", "emitCancel"]
+            case ContractType.RUBICON_ROUTER:
+                event_names = ["emitSwap"]
+            case ContractType.ERC20:
+                event_names = ["Approval", "Transfer"]
+            case _:
+                raise Exception("Unexpected ContractType")
+
+        raw_events = []
+        for event_name in event_names:
+            transaction_events_data = self.contract.events[
+                event_name
+            ]().process_receipt(receipt, DISCARD)
+
+            for event_data in transaction_events_data:
+                if self.contract_type == ContractType.ERC20:
+                    raw_events.append(event_data)
+
+                raw_events.append(
+                    BaseEvent.builder(
+                        name=event_name,
+                        block_number=event_data["blockNumber"],
+                        **event_data["args"],
+                    )
+                )
+
+        return raw_events
```

### Comparing `rubi-2.2.1/rubi/contracts/contract_types/events.py` & `rubi-2.3.0/rubi/contracts/contract_types/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,28 @@
         :type block_number: int
         :param args: Additional arguments for the event.
         :type args: dict
         """
         self.block_number = block_number
 
     @staticmethod
+    def builder(
+        name: str, **kwargs
+    ) -> Union["EmitOfferEvent", "EmitTakeEvent", "EmitCancelEvent", "EmitSwap"]:
+        match name:
+            case "emitOffer":
+                return EmitOfferEvent(**kwargs)
+            case "emitTake":
+                return EmitTakeEvent(**kwargs)
+            case "emitCancel":
+                return EmitCancelEvent(**kwargs)
+            case "emitSwap":
+                return EmitSwap(**kwargs)
+
+    @staticmethod
     @abstractmethod
     def get_event_contract(
         market: _RubiconMarket, router: _RubiconRouter
     ) -> Union[_RubiconMarket, _RubiconRouter]:
         """Abstract method to determine the contract an event corresponds to. Must be overridden in subclasses.
 
         :param market: The RubiconMarket instance.
@@ -143,15 +157,15 @@
     def __init__(
         self,
         maker: ChecksumAddress,
         pay_gem: ChecksumAddress,
         buy_gem: ChecksumAddress,
         pay_amt: int,
         buy_amt: int,
-        **args
+        **args,
     ):
         """Initialize an EmitOfferEvent instance.
 
         :param maker: The maker address.
         :type maker: ChecksumAddress
         :param pay_gem: The address of the token to be paid.
         :type pay_gem: ChecksumAddress
@@ -195,15 +209,15 @@
         self,
         maker: ChecksumAddress,
         taker: ChecksumAddress,
         pay_gem: ChecksumAddress,
         buy_gem: ChecksumAddress,
         take_amt: int,
         give_amt: int,
-        **args
+        **args,
     ):
         """Initialize an EmitTakeEvent instance.
 
         :param maker: The maker address.
         :type maker: ChecksumAddress
         :param taker: The taker address.
         :type taker: ChecksumAddress
@@ -254,15 +268,15 @@
     def __init__(
         self,
         maker: ChecksumAddress,
         pay_gem: ChecksumAddress,
         buy_gem: ChecksumAddress,
         pay_amt: int,
         buy_amt: int,
-        **args
+        **args,
     ):
         """Initialize an EmitCancelEvent instance.
 
         :param maker: The maker address.
         :type maker: ChecksumAddress
         :param pay_gem: The address of the token to be paid of the cancelled offer.
         :type pay_gem: ChecksumAddress
@@ -305,15 +319,15 @@
 
     def __init__(
         self,
         taker: ChecksumAddress,
         feeTo: ChecksumAddress,
         asset: ChecksumAddress,
         feeAmt: int,
-        **args
+        **args,
     ):
         """Initialize an EmitFeeEvent instance.
 
         :param taker: The taker address.
         :type taker: ChecksumAddress
         :param feeTo: The address to receive the fee.
         :type feeTo: ChecksumAddress
@@ -395,15 +409,15 @@
         recipient: ChecksumAddress,
         inputERC20: ChecksumAddress,
         targetERC20: ChecksumAddress,
         pair: bytes,
         inputAmount: int,
         realizedFill: int,
         hurdleBuyAmtMin: int,
-        **args
+        **args,
     ):
         """Initialize an EmitSwap instance.
 
         :param recipient: The address of the recipient of the swap.
         :type recipient: ChecksumAddress
         :param inputERC20: The address of the input ERC20 token.
         :type inputERC20: ChecksumAddress
```

### Comparing `rubi-2.2.1/rubi/contracts/contract_types/transaction_reciept.py` & `rubi-2.3.0/rubi/contracts/contract_types/transaction_reciept.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,38 @@
 from _decimal import Decimal
-from typing import Optional
+from enum import Enum
+from typing import Optional, List, Any
 
 from eth_typing import BlockNumber, ChecksumAddress
 from hexbytes import HexBytes
-from web3.types import Wei, TxReceipt
+from web3.types import Wei, TxReceipt, EventData
+
+from rubi.contracts.contract_types import BaseEvent
+
+
+class TransactionStatus(Enum):
+    """Enum representing the status of a transaction."""
+
+    SUCCESS = "SUCCESS"
+    FAILURE = "FAILURE"
+
+    def __eq__(self, other):
+        return self.name is other.name and self.value == other.value
+
+    @classmethod
+    def from_int(cls, status: int) -> "TransactionStatus":
+        """
+        Transform the TxReceipt status into an Enum
+        """
+        if status == 0:
+            return cls.FAILURE
+        else:
+            return cls.SUCCESS
 
 
-# TODO: a TxReceipt contains logs which can be decoded into events that were emitted by calling the contract function.
-#  It may be useful in future to add the logs field to the TransactionReceipt object and decode them into objects.
 class TransactionReceipt:
     def __init__(
         self,
         block_number: BlockNumber,
         contract_address: Optional[ChecksumAddress],
         effective_gas_price: Wei,
         gas_used: int,
@@ -20,31 +41,38 @@
         status: int,
         transaction_hash: HexBytes,
         transaction_index: int,
         l1_fee: Optional[int] = None,
         l1_gas_price: Optional[int] = None,
         l1_gas_used: Optional[int] = None,
         l1_fee_scalar: Optional[Decimal] = None,
+        raw_events: Optional[List[BaseEvent]] = None,
     ):
         self.block_number = block_number
         self.contract_address = contract_address
         self.effective_gas_price = effective_gas_price
         self.gas_used = gas_used
         self.from_address = from_address
         self.to_address = to_address
         self.status = status
+        # Do this so that introducing TransactionStatus is not a breaking change
+        self.transaction_status = TransactionStatus.from_int(status=status)
         self.transaction_hash = transaction_hash
         self.transaction_index = transaction_index
         self.l1_fee = l1_fee
         self.l1_gas_price = l1_gas_price
         self.l1_gas_used = l1_gas_used
         self.l1_fee_scalar = l1_fee_scalar
+        self.raw_events = raw_events
+        self.events = None
 
     @classmethod
-    def from_tx_receipt(cls, tx_receipt: TxReceipt) -> "TransactionReceipt":
+    def from_tx_receipt(
+        cls, tx_receipt: TxReceipt, raw_events: List[BaseEvent | EventData]
+    ) -> "TransactionReceipt":
         return cls(
             block_number=tx_receipt["blockNumber"],
             contract_address=tx_receipt["contractAddress"],
             effective_gas_price=tx_receipt["effectiveGasPrice"],
             gas_used=tx_receipt["gasUsed"],
             from_address=tx_receipt["from"],
             to_address=tx_receipt["to"],
@@ -59,12 +87,17 @@
             else int(tx_receipt.get("l1GasPrice"), 16),
             l1_gas_used=None
             if tx_receipt.get("l1GasUsed") is None
             else int(tx_receipt.get("l1GasUsed"), 16),
             l1_fee_scalar=None
             if tx_receipt.get("l1FeeScalar") is None
             else Decimal(tx_receipt.get("l1FeeScalar")),
+            raw_events=raw_events,
         )
 
+    # TODO: Any is used to avoid circular dependencies, look at a restructure. These are OrderEvents.
+    def set_events(self, events: List[Any]):
+        self.events = events
+
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
```

### Comparing `rubi-2.2.1/rubi/contracts/erc20.py` & `rubi-2.3.0/rubi/contracts/erc20.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Optional
 
 from eth_typing import ChecksumAddress
 from web3 import Web3
 from web3.contract import Contract
 from web3.types import ABI
 
-from rubi.contracts.base_contract import BaseContract
+from rubi.contracts.base_contract import BaseContract, ContractType
 from rubi.contracts.contract_types import TransactionReceipt
 from rubi.network import Network
 
 
 class ERC20(BaseContract):
     """this class represents a contract that implements the ERC20 standard. it is used to read the contract instance.
     if a wallet and key are passed in instantiation then this class can also be used to write to the contract instance.
@@ -27,19 +27,26 @@
     :type key: Optional[str]
     """
 
     def __init__(
         self,
         w3: Web3,
         contract: Contract,
+        contract_type: ContractType = ContractType.ERC20,
         wallet: Optional[ChecksumAddress] = None,
         key: Optional[str] = None,
     ):
         """constructor method"""
-        super().__init__(w3=w3, contract=contract, wallet=wallet, key=key)
+        super().__init__(
+            w3=w3,
+            contract=contract,
+            contract_type=ContractType.ERC20,
+            wallet=wallet,
+            key=key,
+        )
 
         self.name: str = self.name()
         self.symbol: str = self.symbol()
         self.decimal: int = self.decimals()
 
     @classmethod
     def from_network(
@@ -83,14 +90,15 @@
                 "ERC20.json abi not found. this file should in the network_config folder"
             )
 
         return cls.from_address_and_abi(
             w3=network.w3,
             address=network.token_addresses[name],
             contract_abi=abi,
+            contract_type=ContractType.ERC20,
             wallet=wallet,
             key=key,
         )
 
     @classmethod
     def from_address(
         cls,
@@ -123,15 +131,20 @@
 
         except FileNotFoundError:
             raise Exception(
                 "ERC20.json abi not found. this file should in the network_config folder"
             )
 
         return cls.from_address_and_abi(
-            w3=w3, address=address, contract_abi=abi, wallet=wallet, key=key
+            w3=w3,
+            address=address,
+            contract_abi=abi,
+            contract_type=ContractType.ERC20,
+            wallet=wallet,
+            key=key,
         )
 
     ######################################################################
     # read calls
     ######################################################################
 
     # allowance(owner (address), spender (address)) -> uint256
```

### Comparing `rubi-2.2.1/rubi/contracts/market.py` & `rubi-2.3.0/rubi/contracts/market.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Tuple, List
 
 from eth_typing import ChecksumAddress
 from web3 import Web3
 from web3.contract import Contract
 
-from rubi.contracts.base_contract import BaseContract
+from rubi.contracts.base_contract import BaseContract, ContractType
 from rubi.contracts.contract_types import TransactionReceipt
 from rubi.network import Network
 
 
 class RubiconMarket(BaseContract):
     """This class represents the RubiconMarket.sol contract and by default has read functionality.
     If a wallet and key are passed in instantiation then this class can also be used to write to the contract instance.
@@ -23,19 +23,26 @@
     :type key: Optional[str]
     """
 
     def __init__(
         self,
         w3: Web3,
         contract: Contract,
+        contract_type: ContractType = ContractType.RUBICON_MARKET,
         wallet: Optional[ChecksumAddress] = None,
         key: Optional[str] = None,
     ) -> None:
         """constructor method"""
-        super().__init__(w3=w3, contract=contract, wallet=wallet, key=key)
+        super().__init__(
+            w3=w3,
+            contract=contract,
+            contract_type=ContractType.RUBICON_MARKET,
+            wallet=wallet,
+            key=key,
+        )
 
     @classmethod
     def from_network(
         cls,
         network: Network,
         wallet: Optional[ChecksumAddress] = None,
         key: Optional[str] = None,
@@ -51,14 +58,15 @@
         :return: A RubiconMarket instance based on the Network instance.
         :rtype: RubiconMarket
         """
         return cls.from_address_and_abi(
             w3=network.w3,
             address=network.rubicon.market.address,
             contract_abi=network.rubicon.market.abi,
+            contract_type=ContractType.RUBICON_MARKET,
             wallet=wallet,
             key=key,
         )
 
     ######################################################################
     # read calls
     ######################################################################
```

### Comparing `rubi-2.2.1/rubi/contracts/router.py` & `rubi-2.3.0/rubi/contracts/router.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Tuple, List
 
 from eth_typing import ChecksumAddress
 from web3 import Web3
 from web3.contract import Contract
 
-from rubi.contracts.base_contract import BaseContract
+from rubi.contracts.base_contract import BaseContract, ContractType
 from rubi.contracts.contract_types import TransactionReceipt
 from rubi.network import Network
 
 
 class RubiconRouter(BaseContract):
     """This class represents the RubiconRouter.sol contract and by default has read functionality.
     If a wallet and key are passed in instantiation then this class can also be used to write to the contract instance.
@@ -23,19 +23,26 @@
     :type key: Optional[str]
     """
 
     def __init__(
         self,
         w3: Web3,
         contract: Contract,
+        contract_type: ContractType = ContractType.RUBICON_ROUTER,
         wallet: Optional[ChecksumAddress] = None,
         key: Optional[str] = None,
     ) -> None:
         """constructor method"""
-        super().__init__(w3=w3, contract=contract, wallet=wallet, key=key)
+        super().__init__(
+            w3=w3,
+            contract=contract,
+            contract_type=ContractType.RUBICON_ROUTER,
+            wallet=wallet,
+            key=key,
+        )
 
     @classmethod
     def from_network(
         cls,
         network: Network,
         wallet: Optional[ChecksumAddress] = None,
         key: Optional[str] = None,
@@ -51,14 +58,15 @@
         :return: A RubiconRouter instance based on the Network instance.
         :rtype: RubiconRouter
         """
         return cls.from_address_and_abi(
             w3=network.w3,
             address=network.rubicon.router.address,
             contract_abi=network.rubicon.router.abi,
+            contract_type=ContractType.RUBICON_ROUTER,
             wallet=wallet,
             key=key,
         )
 
     ######################################################################
     # read calls
     ######################################################################
```

### Comparing `rubi-2.2.1/rubi/data/market.py` & `rubi-2.3.0/rubi/data/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/rubi/network/network.py` & `rubi-2.3.0/rubi/network/network.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/rubi/rubicon_types/order.py` & `rubi-2.3.0/rubi/rubicon_types/order.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/rubi/rubicon_types/order_query.py` & `rubi-2.3.0/rubi/rubicon_types/order_query.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/rubi/rubicon_types/orderbook.py` & `rubi-2.3.0/rubi/rubicon_types/orderbook.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/rubi/rubicon_types/pair.py` & `rubi-2.3.0/rubi/rubicon_types/pair.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/rubi/rubicon_types/trade_query.py` & `rubi-2.3.0/rubi/rubicon_types/trade_query.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.1/PKG-INFO` & `rubi-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.2.1
+Version: 2.3.0
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

