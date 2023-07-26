# Comparing `tmp/xjet-0.1.2.tar.gz` & `tmp/xjet-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xjet-0.1.2.tar", max compression
+gzip compressed data, was "xjet-0.1.3.tar", max compression
```

## Comparing `xjet-0.1.2.tar` & `xjet-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-01-15 16:26:30.059724 xjet-0.1.2/LICENSE
--rw-r--r--   0        0        0     1296 2023-05-03 09:38:23.542817 xjet-0.1.2/README.md
--rw-r--r--   0        0        0      798 2023-05-03 09:36:57.069787 xjet-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1918 2023-05-03 09:23:09.871940 xjet-0.1.2/xjet/__init__.py
--rw-r--r--   0        0        0     5738 2023-05-03 10:45:04.960289 xjet-0.1.2/xjet/api.py
--rw-r--r--   0        0        0      256 2023-01-15 16:42:40.104778 xjet-0.1.2/xjet/constants.py
--rw-r--r--   0        0        0     1228 2023-01-15 16:42:40.142189 xjet-0.1.2/xjet/sync.py
--rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 xjet-0.1.2/setup.py
--rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 xjet-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-15 16:26:30.059724 xjet-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3596 2023-07-26 17:16:04.984537 xjet-0.1.3/README.md
+-rw-r--r--   0        0        0      798 2023-07-26 17:41:01.639637 xjet-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3048 2023-07-26 17:39:13.325732 xjet-0.1.3/xjet/__init__.py
+-rw-r--r--   0        0        0     7480 2023-07-26 17:24:20.211970 xjet-0.1.3/xjet/api.py
+-rw-r--r--   0        0        0     1228 2023-07-26 17:41:18.063263 xjet-0.1.3/xjet/sync.py
+-rw-r--r--   0        0        0     4514 1970-01-01 00:00:00.000000 xjet-0.1.3/setup.py
+-rw-r--r--   0        0        0     4565 1970-01-01 00:00:00.000000 xjet-0.1.3/PKG-INFO
```

### Comparing `xjet-0.1.2/LICENSE` & `xjet-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xjet-0.1.2/pyproject.toml` & `xjet-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xjet"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python SDK for t.me/xJetSwapBot"
 readme = "README.md"
 authors = [
     "delpydoc <delpydoc@proton.me>",
 ]
 maintainers = []
 repository = "https://github.com/xJetLabs/python-sdk"
@@ -20,12 +20,12 @@
 
 [tool.setuptools.package-data]
 xjet = []
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 httpx = ">=0.23.1"
-PyNaCl = ">=1.5.0"
+ecdsa = ">=0.18.0"
 
 [build-system]
 requires = ["poetry>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `xjet-0.1.2/xjet/api.py` & `xjet-0.1.3/xjet/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Union
+
 
 class System:
 
     """ System class.
 
     Available methods:
 
@@ -39,20 +41,20 @@
         """ Get balance """
         return await self.request(method = 'account.balances')
 
     async def submit_deposit(self):
         """ Check for deposit """
         return await self.request(method = 'account.submitDeposit')
 
-    async def withdraw(self, ton_address: str, currency: str, amount: float):
+    async def withdraw(self, ton_address: str, currency: str, amount: Union[int, float]):
         """ Withdraw funds 
         
         :param `ton_address` [str]: TON address
         :param `currency` [str]: Currency of withdraw
-        :param `amount` [float]: Amount of withdraw
+        :param `amount` Union[int, float]: Amount of withdraw
         """
         return await self.request(
             method = 'account.withdraw', 
             json = self.sign_message({
                 'ton_address': ton_address, 'currency': currency, 'amount': amount
             })
         )
@@ -76,19 +78,19 @@
     * `cheque_create` - Create cheques
     * `cheque_status` - Get cheque status
     * `cheque_list` - Get list of cheques
     * `cheque_activate` - Activate cheque
     
     """
 
-    async def cheque_create(self, currency: str, amount: int, expires: int = None, description: str = '', activates_count: int = 1, groups_id: list = None, personal_id: str = None, password: str = None, **kwargs):
+    async def cheque_create(self, currency: str, amount: Union[int, float], expires: int = None, description: str = '', activates_count: int = 1, groups_id: list = None, personal_id: str = None, password: str = None, **kwargs):
         """ Create cheques 
         
         :param `currency` [str]: Currency of cheque
-        :param `amount` [int]: Amount of cheque
+        :param `amount` Union[int, float]: Amount of cheque
         :param `expires` [int]: Expiration time of cheque
         :param `description` [str]: Description of cheque
         :param `activates_count` [int]: Number of activations
         :param `groups_id` [list]: List of groups
         :param `personal_id` [str]: Personal id
         :param `password` [str]: Password
 
@@ -135,19 +137,19 @@
     
     * invoice_create()
     * invoice_status()
     * invoice_list()
 
     """
 
-    async def invoice_create(self, currency: str, amount: int, description: str = None, max_payments: int = 1, expires: int = None):
+    async def invoice_create(self, currency: str, amount: Union[int, float], description: str = None, max_payments: int = 1, expires: int = None):
         """ Create invoice 
         
         :param `currency` [str]: Currency of invoice
-        :param `amount` [int]: Amount of invoice
+        :param `amount` Union[int, float]: Amount of invoice
         :param `description` [str]: Description of invoice
         :param `max_payments` [int]: Max payments
         """
         return await self.request(
             method = 'invoice.create', 
             json = {
                 'currency': currency.lower(),
@@ -196,7 +198,62 @@
             method = 'nft.transfer',
             json = self.sign_message({
                 'nft_address': nft_address,
                 'to_address': to_address
             }) 
         )
         
+
+class Exchanges:
+
+    """ Exchange methods wrapper. 
+    
+    Available methods:
+    
+    * pairs()
+    * estimate()
+    * create_order()
+    * order_status()
+
+    """
+
+    async def pairs(self):
+        """ Get list of pairs """
+        return await self.request(method = 'exchanges.pairs', request_method = 'GET')
+
+    async def estimate(self, pair: list, action_type: str, amount: Union[int, float]):
+        """ Estimate
+
+        :param `pair` [list]: Pair
+        :param `type` [str]: Type
+        :param `amount` Union[int, float]: Amount
+        
+        """
+        return await self.request(
+            method = 'exchanges.estimate', 
+            json = {
+                'pair': pair, 'type': action_type, 'amount': amount
+            }
+        )
+
+    async def create_order(self, pair: list, action_type: str, amount: Union[int, float], min_excepted_amount: Union[int, float]):
+        """ Create order
+
+        :param `pair` [list]: Pair
+        :param `action_type` [str]: Action type
+        :param `amount` Union[int, float]: Amount
+        :param `min_excepted_amount` Union[int, float]: Min excepted amount
+        
+        """
+        return await self.request(
+            method = 'exchanges.createOrder', 
+            json = self.sign_message({
+                'pair': pair, 'type': action_type, 'amount': amount, 'min_expected_amount': min_excepted_amount
+            })
+        )
+
+    async def order_status(self, order_id: str):
+        """ Get order status
+        
+        :param `order_id` [str]: Order id
+        """
+        return await self.request(method = 'exchanges.orderStatus', params = {'id': order_id})
```

### Comparing `xjet-0.1.2/xjet/sync.py` & `xjet-0.1.3/xjet/sync.py`

 * *Files identical despite different names*

