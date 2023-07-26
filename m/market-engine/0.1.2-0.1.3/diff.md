# Comparing `tmp/market-engine-0.1.2.tar.gz` & `tmp/market-engine-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market-engine-0.1.2.tar", last modified: Wed Jul 26 19:54:18 2023, max compression
+gzip compressed data, was "market-engine-0.1.3.tar", last modified: Wed Jul 26 19:57:31 2023, max compression
```

## Comparing `market-engine-0.1.2.tar` & `market-engine-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 19:54:18.761540 market-engine-0.1.2/
--rw-rw-rw-   0        0        0      216 2023-07-26 19:54:18.761540 market-engine-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 19:54:18.756225 market-engine-0.1.2/market_engine/
-drwxrwxrwx   0        0        0        0 2023-07-26 19:54:18.759540 market-engine-0.1.2/market_engine/API/
--rw-rw-rw-   0        0        0     3166 2023-07-25 21:19:06.000000 market-engine-0.1.2/market_engine/API/ManifestAPI.py
--rw-rw-rw-   0        0        0     5903 2023-07-25 21:05:50.000000 market-engine-0.1.2/market_engine/API/MarketAPI.py
--rw-rw-rw-   0        0        0     6633 2023-07-25 22:30:19.000000 market-engine-0.1.2/market_engine/API/RelicsRunAPI.py
--rw-rw-rw-   0        0        0        0 2023-07-24 20:09:05.000000 market-engine-0.1.2/market_engine/API/__init__.py
--rw-rw-rw-   0        0        0     7954 2023-07-26 01:21:00.000000 market-engine-0.1.2/market_engine/Common.py
--rw-rw-rw-   0        0        0    41600 2023-07-26 19:54:08.000000 market-engine-0.1.2/market_engine/ManifestParser.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:54:18.761040 market-engine-0.1.2/market_engine/Models/
--rw-rw-rw-   0        0        0    26804 2023-07-26 18:15:33.000000 market-engine-0.1.2/market_engine/Models/MarketDatabase.py
--rw-rw-rw-   0        0        0    12514 2023-07-26 01:09:08.000000 market-engine-0.1.2/market_engine/Models/MarketItem.py
--rw-rw-rw-   0        0        0     7106 2023-07-26 01:14:25.000000 market-engine-0.1.2/market_engine/Models/MarketUser.py
--rw-rw-rw-   0        0        0        0 2023-07-25 16:48:26.000000 market-engine-0.1.2/market_engine/Models/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.1.2/market_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:54:18.758025 market-engine-0.1.2/market_engine.egg-info/
--rw-rw-rw-   0        0        0      216 2023-07-26 19:54:18.000000 market-engine-0.1.2/market_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      568 2023-07-26 19:54:18.000000 market-engine-0.1.2/market_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 19:54:18.000000 market-engine-0.1.2/market_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      251 2023-07-26 19:54:18.000000 market-engine-0.1.2/market_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-26 19:54:18.000000 market-engine-0.1.2/market_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 19:54:18.762040 market-engine-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-07-26 19:54:15.000000 market-engine-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:57:31.691510 market-engine-0.1.3/
+-rw-rw-rw-   0        0        0      216 2023-07-26 19:57:31.691510 market-engine-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 19:57:31.685503 market-engine-0.1.3/market_engine/
+drwxrwxrwx   0        0        0        0 2023-07-26 19:57:31.689007 market-engine-0.1.3/market_engine/API/
+-rw-rw-rw-   0        0        0     3166 2023-07-25 21:19:06.000000 market-engine-0.1.3/market_engine/API/ManifestAPI.py
+-rw-rw-rw-   0        0        0     5903 2023-07-25 21:05:50.000000 market-engine-0.1.3/market_engine/API/MarketAPI.py
+-rw-rw-rw-   0        0        0     6633 2023-07-25 22:30:19.000000 market-engine-0.1.3/market_engine/API/RelicsRunAPI.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 20:09:05.000000 market-engine-0.1.3/market_engine/API/__init__.py
+-rw-rw-rw-   0        0        0     7954 2023-07-26 01:21:00.000000 market-engine-0.1.3/market_engine/Common.py
+-rw-rw-rw-   0        0        0    41600 2023-07-26 19:54:08.000000 market-engine-0.1.3/market_engine/ManifestParser.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:57:31.691010 market-engine-0.1.3/market_engine/Models/
+-rw-rw-rw-   0        0        0    26804 2023-07-26 18:15:33.000000 market-engine-0.1.3/market_engine/Models/MarketDatabase.py
+-rw-rw-rw-   0        0        0    12476 2023-07-26 19:57:21.000000 market-engine-0.1.3/market_engine/Models/MarketItem.py
+-rw-rw-rw-   0        0        0     7066 2023-07-26 19:57:21.000000 market-engine-0.1.3/market_engine/Models/MarketUser.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 16:48:26.000000 market-engine-0.1.3/market_engine/Models/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.1.3/market_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:57:31.686995 market-engine-0.1.3/market_engine.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-07-26 19:57:31.000000 market-engine-0.1.3/market_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      544 2023-07-26 19:57:31.000000 market-engine-0.1.3/market_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 19:57:31.000000 market-engine-0.1.3/market_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      251 2023-07-26 19:57:31.000000 market-engine-0.1.3/market_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 19:57:31.000000 market-engine-0.1.3/market_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 19:57:31.691510 market-engine-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-26 19:57:27.000000 market-engine-0.1.3/setup.py
```

### Comparing `market-engine-0.1.2/market_engine/API/ManifestAPI.py` & `market-engine-0.1.3/market_engine/API/ManifestAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.2/market_engine/API/MarketAPI.py` & `market-engine-0.1.3/market_engine/API/MarketAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.2/market_engine/API/RelicsRunAPI.py` & `market-engine-0.1.3/market_engine/API/RelicsRunAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.2/market_engine/Common.py` & `market-engine-0.1.3/market_engine/Common.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.2/market_engine/ManifestParser.py` & `market-engine-0.1.3/market_engine/ManifestParser.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.2/market_engine/Models/MarketDatabase.py` & `market-engine-0.1.3/market_engine/Models/MarketDatabase.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.2/market_engine/Models/MarketItem.py` & `market-engine-0.1.3/market_engine/Models/MarketItem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import asyncio
 from typing import List, Dict, Union, Tuple, Coroutine, Any, Optional
 
-from .MarketDatabase import MarketDatabase
 from ..Common import fetch_api_data, get_wfm_headers, cache_manager, session_manager
 
 
 class MarketItem:
     """
     Base class for market items
     """
     base_api_url: str = "https://api.warframe.market/v1"  # Base URL for warframe.market API
     base_url: str = "warframe.market/items"  # Base URL for warframe.market items
     asset_url: str = "https://warframe.market/static/assets"  # Base URL for warframe.market assets
 
-    def __init__(self, database: MarketDatabase,
+    def __init__(self, database: "MarketDatabase",
                  item_id: str, item_name: str, item_type: str, item_url_name: str, thumb: str, max_rank: str,
                  aliases: List, platform: str = 'pc') -> None:
         """
         Initializes a MarketItem object.
         :param database: database object
         :param item_id: the warframe.market item id
         :param item_name: the english item name
         :param item_type: the type of the item (e.g. 'Mods', 'Relics', etc.)
         :param item_url_name: the url name of the item, as used in the warframe.market url
         :param thumb: the url of the item's thumbnail
         :param max_rank: the maximum rank of the item (for mods)
         :param aliases: a list of aliases for the item
         :param platform: the platform to fetch the item for
         """
-        self.database: MarketDatabase = database
+        self.database: "MarketDatabase" = database
         self.item_id: str = item_id
         self.item_name: str = item_name
         self.item_type: str = item_type
         self.item_url_name: str = item_url_name
         self.thumb: str = thumb
         self.max_rank: str = max_rank
         self.aliases: List = aliases
@@ -45,15 +44,15 @@
         self.part_price_history_fetched: bool = False
         self.part_demand_history_fetched: bool = False
         self.price_history: Dict[str, str] = {}
         self.demand_history: Dict[str, str] = {}
         self.platform = platform
 
     @classmethod
-    async def create(cls, database: MarketDatabase, item_id: str, item_name: str, item_type: str,
+    async def create(cls, database: "MarketDatabase", item_id: str, item_name: str, item_type: str,
                      item_url_name: str, thumb: str, max_rank: str, aliases: List, fetch_orders: bool = True,
                      fetch_parts: bool = True, fetch_part_orders: bool = True,
                      fetch_price_history: bool = True, fetch_demand_history: bool = True,
                      platform: str = 'pc') -> "MarketItem":
         """
         Creates a MarketItem object and fetches the relevant data.
         :param database: database object
```

### Comparing `market-engine-0.1.2/market_engine/Models/MarketUser.py` & `market-engine-0.1.3/market_engine/Models/MarketUser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import asyncio
 from typing import Dict, List, Union, Any
 
-from .MarketDatabase import MarketDatabase
 from ..Common import fetch_api_data, cache_manager, session_manager
 
 
 class MarketUser:
     """
     Represents a user on warframe.market
     """
     base_api_url: str = "https://api.warframe.market/v1"  # Base URL for warframe.market API
     base_url: str = "https://warframe.market/profile"  # Base URL for warframe.market profiles
     asset_url: str = "https://warframe.market/static/assets"  # Base URL for warframe.market assets
 
-    def __init__(self, database: MarketDatabase, user_id: str, username: str):
+    def __init__(self, database: "MarketDatabase", user_id: str, username: str):
         """
         Initializes a MarketUser object.
         :param database: database object
         :param user_id: the user's warframe.market id
         :param username: the user's warframe.market username
         """
         self.database = database
@@ -35,15 +34,15 @@
         self.banned = None
         self.status = None
         self.region = None
         self.orders: Dict[str, List[Dict[str, Union[str, int]]]] = {'buy': [], 'sell': []}
         self.reviews: List[str] = []
 
     @classmethod
-    async def create(cls, database: MarketDatabase, user_id: str, username: str,
+    async def create(cls, database: "MarketDatabase", user_id: str, username: str,
                      fetch_user_data: bool = True, fetch_orders: bool = True, fetch_reviews: bool = True):
         """
         Creates a MarketUser object.
         :param database: database object
         :param user_id: the user's warframe.market id
         :param username: the user's warframe.market username
         :param fetch_user_data: whether or not to fetch the user's data from warframe.market
```

### Comparing `market-engine-0.1.2/market_engine.egg-info/SOURCES.txt` & `market-engine-0.1.3/market_engine.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 setup.py
 market_engine/Common.py
 market_engine/ManifestParser.py
 market_engine/__init__.py
-market_engine/common.py
 market_engine.egg-info/PKG-INFO
 market_engine.egg-info/SOURCES.txt
 market_engine.egg-info/dependency_links.txt
 market_engine.egg-info/requires.txt
 market_engine.egg-info/top_level.txt
 market_engine/API/ManifestAPI.py
 market_engine/API/MarketAPI.py
```

### Comparing `market-engine-0.1.2/setup.py` & `market-engine-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='market-engine',
-    version='0.1.2',
+    version='0.1.3',
     description='Engine for easily getting the orders, statistics, and other stats from warframe.market.',
     author='Jacob McBride',
     author_email='jake55111@gmail.com',
     packages=find_packages(),
     install_requires=[
         'aiohttp~=3.8.4',
         'discord~=2.2.2',
```

