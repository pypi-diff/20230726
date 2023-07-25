# Comparing `tmp/rubi-2.2.0.tar.gz` & `tmp/rubi-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.2.0.tar", max compression
+gzip compressed data, was "rubi-2.2.1.tar", max compression
```

## Comparing `rubi-2.2.0.tar` & `rubi-2.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    11357 2023-07-25 19:28:26.901551 rubi-2.2.0/LICENSE
--rw-r--r--   0        0        0     2757 2023-07-25 19:28:26.901551 rubi-2.2.0/README.md
--rw-r--r--   0        0        0     6735 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      833 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/arbitrum_one/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/arbitrum_one/abis/router.json
--rw-r--r--   0        0        0      840 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/arbitrum_one/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      858 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      760 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-25 19:28:26.905551 rubi-2.2.0/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      832 2023-07-25 19:28:26.905551 rubi-2.2.0/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0     1746 2023-07-25 19:28:52.861166 rubi-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      124 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/__init__.py
--rw-r--r--   0        0        0    30904 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/client.py
--rw-r--r--   0        0        0      163 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    65755 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/aid.py
--rw-r--r--   0        0        0    12337 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0       74 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/contract_types/__init__.py
--rw-r--r--   0        0        0    15898 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/contract_types/events.py
--rw-r--r--   0        0        0     2805 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/contract_types/transaction_reciept.py
--rw-r--r--   0        0        0    18565 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24880 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/market.py
--rw-r--r--   0        0        0    14915 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/router.py
--rw-r--r--   0        0        0       77 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/data/README.md
--rw-r--r--   0        0        0       31 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/data/__init__.py
--rw-r--r--   0        0        0    17073 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/data/market.py
--rw-r--r--   0        0        0       72 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/network/__init__.py
--rw-r--r--   0        0        0     8475 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/network/network.py
--rw-r--r--   0        0        0      121 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/rubicon_types/__init__.py
--rw-r--r--   0        0        0    16249 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/rubicon_types/order.py
--rw-r--r--   0        0        0    11701 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/rubicon_types/order_query.py
--rw-r--r--   0        0        0     6323 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/rubicon_types/orderbook.py
--rw-r--r--   0        0        0     2779 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/rubicon_types/pair.py
--rw-r--r--   0        0        0    11414 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/rubicon_types/trade_query.py
--rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 rubi-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 22:42:00.027885 rubi-2.2.1/LICENSE
+-rw-r--r--   0        0        0     2757 2023-07-25 22:42:00.027885 rubi-2.2.1/README.md
+-rw-r--r--   0        0        0     6735 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      833 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/arbitrum_one/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/arbitrum_one/abis/router.json
+-rw-r--r--   0        0        0      840 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/arbitrum_one/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      858 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      760 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      832 2023-07-25 22:42:00.027885 rubi-2.2.1/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0     1746 2023-07-25 22:42:25.812710 rubi-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/__init__.py
+-rw-r--r--   0        0        0    30804 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/client.py
+-rw-r--r--   0        0        0      163 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    65755 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    12337 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0       74 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/contract_types/__init__.py
+-rw-r--r--   0        0        0    15898 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/contract_types/events.py
+-rw-r--r--   0        0        0     2805 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/contract_types/transaction_reciept.py
+-rw-r--r--   0        0        0    18565 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24880 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14915 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/contracts/router.py
+-rw-r--r--   0        0        0       77 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/data/README.md
+-rw-r--r--   0        0        0       31 2023-07-25 22:42:00.027885 rubi-2.2.1/rubi/data/__init__.py
+-rw-r--r--   0        0        0    17073 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/data/market.py
+-rw-r--r--   0        0        0       72 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/network/__init__.py
+-rw-r--r--   0        0        0     8475 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/network/network.py
+-rw-r--r--   0        0        0      121 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/rubicon_types/__init__.py
+-rw-r--r--   0        0        0    16249 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/rubicon_types/order.py
+-rw-r--r--   0        0        0    11701 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/rubicon_types/order_query.py
+-rw-r--r--   0        0        0     6323 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/rubicon_types/orderbook.py
+-rw-r--r--   0        0        0     2779 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/rubicon_types/pair.py
+-rw-r--r--   0        0        0    11414 2023-07-25 22:42:00.031885 rubi-2.2.1/rubi/rubicon_types/trade_query.py
+-rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 rubi-2.2.1/PKG-INFO
```

### Comparing `rubi-2.2.0/LICENSE` & `rubi-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/README.md` & `rubi-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/ERC20.json` & `rubi-2.2.1/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/README.md` & `rubi-2.2.1/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/abitrum_goerli/abis/market.json` & `rubi-2.2.1/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/abitrum_goerli/abis/router.json` & `rubi-2.2.1/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/abitrum_goerli/network.yaml` & `rubi-2.2.1/network_config/abitrum_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/arbitrum_one/abis/market.json` & `rubi-2.2.1/network_config/arbitrum_one/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/arbitrum_one/abis/router.json` & `rubi-2.2.1/network_config/arbitrum_one/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/arbitrum_one/network.yaml` & `rubi-2.2.1/network_config/arbitrum_one/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/optimism/abis/market.json` & `rubi-2.2.1/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/optimism/abis/router.json` & `rubi-2.2.1/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/optimism/network.yaml` & `rubi-2.2.1/network_config/optimism/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/optimism_goerli/abis/market.json` & `rubi-2.2.1/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/optimism_goerli/abis/router.json` & `rubi-2.2.1/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/optimism_goerli/network.yaml` & `rubi-2.2.1/network_config/optimism_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/polygon_mumbai/abis/market.json` & `rubi-2.2.1/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/polygon_mumbai/abis/router.json` & `rubi-2.2.1/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/network_config/polygon_mumbai/network.yaml` & `rubi-2.2.1/network_config/polygon_mumbai/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/pyproject.toml` & `rubi-2.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rubi"
-version = "2.2.0"
+version = "2.2.1"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 include = ["network_config/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `rubi-2.2.0/rubi/client.py` & `rubi-2.2.1/rubi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -649,15 +649,15 @@
             order: NewCancelOrder
 
             order_ids.append(order.order_id)
 
         return self.market.batch_cancel(ids=order_ids, **transaction.args())
 
     ######################################################################
-    # data methods (raw data) TODO: once we have cleanly formatted data functions, we can switch to only exposing those
+    # data methods 
     ######################################################################
 
     # TODO: i would like to remove pay_gem and buy_gem and follow the same pattern as the get_trades method but do not want to cause breaking changes
     def get_offers(
         self,
         first: int = 10000000,  # TODO: decide on a default value
         order_by: str = "timestamp",
```

### Comparing `rubi-2.2.0/rubi/contracts/aid.py` & `rubi-2.2.1/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/rubi/contracts/base_contract.py` & `rubi-2.2.1/rubi/contracts/base_contract.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/rubi/contracts/contract_types/events.py` & `rubi-2.2.1/rubi/contracts/contract_types/events.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/rubi/contracts/contract_types/transaction_reciept.py` & `rubi-2.2.1/rubi/contracts/contract_types/transaction_reciept.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/rubi/contracts/erc20.py` & `rubi-2.2.1/rubi/contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/rubi/contracts/market.py` & `rubi-2.2.1/rubi/contracts/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/rubi/contracts/router.py` & `rubi-2.2.1/rubi/contracts/router.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/rubi/data/market.py` & `rubi-2.2.1/rubi/data/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/rubi/network/network.py` & `rubi-2.2.1/rubi/network/network.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/rubi/rubicon_types/order.py` & `rubi-2.2.1/rubi/rubicon_types/order.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/rubi/rubicon_types/order_query.py` & `rubi-2.2.1/rubi/rubicon_types/order_query.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/rubi/rubicon_types/orderbook.py` & `rubi-2.2.1/rubi/rubicon_types/orderbook.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/rubi/rubicon_types/pair.py` & `rubi-2.2.1/rubi/rubicon_types/pair.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/rubi/rubicon_types/trade_query.py` & `rubi-2.2.1/rubi/rubicon_types/trade_query.py`

 * *Files identical despite different names*

### Comparing `rubi-2.2.0/PKG-INFO` & `rubi-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.2.0
+Version: 2.2.1
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

