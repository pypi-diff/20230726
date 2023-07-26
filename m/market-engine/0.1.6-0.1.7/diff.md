# Comparing `tmp/market-engine-0.1.6.tar.gz` & `tmp/market-engine-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market-engine-0.1.6.tar", last modified: Wed Jul 26 20:17:32 2023, max compression
+gzip compressed data, was "market-engine-0.1.7.tar", last modified: Wed Jul 26 20:21:59 2023, max compression
```

## Comparing `market-engine-0.1.6.tar` & `market-engine-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 20:17:32.299163 market-engine-0.1.6/
--rw-rw-rw-   0        0        0      216 2023-07-26 20:17:32.299163 market-engine-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 20:17:32.293646 market-engine-0.1.6/market_engine/
-drwxrwxrwx   0        0        0        0 2023-07-26 20:17:32.297147 market-engine-0.1.6/market_engine/API/
--rw-rw-rw-   0        0        0     3166 2023-07-25 21:19:06.000000 market-engine-0.1.6/market_engine/API/ManifestAPI.py
--rw-rw-rw-   0        0        0     5903 2023-07-25 21:05:50.000000 market-engine-0.1.6/market_engine/API/MarketAPI.py
--rw-rw-rw-   0        0        0     6633 2023-07-25 22:30:19.000000 market-engine-0.1.6/market_engine/API/RelicsRunAPI.py
--rw-rw-rw-   0        0        0        0 2023-07-24 20:09:05.000000 market-engine-0.1.6/market_engine/API/__init__.py
--rw-rw-rw-   0        0        0     7954 2023-07-26 01:21:00.000000 market-engine-0.1.6/market_engine/Common.py
--rw-rw-rw-   0        0        0    41618 2023-07-26 20:17:10.000000 market-engine-0.1.6/market_engine/ManifestParser.py
-drwxrwxrwx   0        0        0        0 2023-07-26 20:17:32.298150 market-engine-0.1.6/market_engine/Models/
--rw-rw-rw-   0        0        0    27005 2023-07-26 20:11:38.000000 market-engine-0.1.6/market_engine/Models/MarketDatabase.py
--rw-rw-rw-   0        0        0    12476 2023-07-26 19:57:21.000000 market-engine-0.1.6/market_engine/Models/MarketItem.py
--rw-rw-rw-   0        0        0     7066 2023-07-26 19:57:21.000000 market-engine-0.1.6/market_engine/Models/MarketUser.py
--rw-rw-rw-   0        0        0        0 2023-07-25 16:48:26.000000 market-engine-0.1.6/market_engine/Models/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.1.6/market_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 20:17:32.295648 market-engine-0.1.6/market_engine.egg-info/
--rw-rw-rw-   0        0        0      216 2023-07-26 20:17:32.000000 market-engine-0.1.6/market_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      544 2023-07-26 20:17:32.000000 market-engine-0.1.6/market_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 20:17:32.000000 market-engine-0.1.6/market_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      251 2023-07-26 20:17:32.000000 market-engine-0.1.6/market_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-26 20:17:32.000000 market-engine-0.1.6/market_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 20:17:32.299668 market-engine-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-07-26 20:17:27.000000 market-engine-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:21:59.403644 market-engine-0.1.7/
+-rw-rw-rw-   0        0        0      216 2023-07-26 20:21:59.403644 market-engine-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 20:21:59.397040 market-engine-0.1.7/market_engine/
+drwxrwxrwx   0        0        0        0 2023-07-26 20:21:59.401136 market-engine-0.1.7/market_engine/API/
+-rw-rw-rw-   0        0        0     3166 2023-07-25 21:19:06.000000 market-engine-0.1.7/market_engine/API/ManifestAPI.py
+-rw-rw-rw-   0        0        0     6246 2023-07-26 20:21:41.000000 market-engine-0.1.7/market_engine/API/MarketAPI.py
+-rw-rw-rw-   0        0        0     6633 2023-07-25 22:30:19.000000 market-engine-0.1.7/market_engine/API/RelicsRunAPI.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 20:09:05.000000 market-engine-0.1.7/market_engine/API/__init__.py
+-rw-rw-rw-   0        0        0     7954 2023-07-26 01:21:00.000000 market-engine-0.1.7/market_engine/Common.py
+-rw-rw-rw-   0        0        0    41618 2023-07-26 20:17:10.000000 market-engine-0.1.7/market_engine/ManifestParser.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:21:59.403145 market-engine-0.1.7/market_engine/Models/
+-rw-rw-rw-   0        0        0    27005 2023-07-26 20:11:38.000000 market-engine-0.1.7/market_engine/Models/MarketDatabase.py
+-rw-rw-rw-   0        0        0    12476 2023-07-26 19:57:21.000000 market-engine-0.1.7/market_engine/Models/MarketItem.py
+-rw-rw-rw-   0        0        0     7066 2023-07-26 19:57:21.000000 market-engine-0.1.7/market_engine/Models/MarketUser.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 16:48:26.000000 market-engine-0.1.7/market_engine/Models/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.1.7/market_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:21:59.399636 market-engine-0.1.7/market_engine.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-07-26 20:21:59.000000 market-engine-0.1.7/market_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      544 2023-07-26 20:21:59.000000 market-engine-0.1.7/market_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 20:21:59.000000 market-engine-0.1.7/market_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      251 2023-07-26 20:21:59.000000 market-engine-0.1.7/market_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 20:21:59.000000 market-engine-0.1.7/market_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 20:21:59.403644 market-engine-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-26 20:21:55.000000 market-engine-0.1.7/setup.py
```

### Comparing `market-engine-0.1.6/market_engine/API/ManifestAPI.py` & `market-engine-0.1.7/market_engine/API/ManifestAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.6/market_engine/API/MarketAPI.py` & `market-engine-0.1.7/market_engine/API/MarketAPI.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,24 +65,30 @@
         parsed_info['set_items'] = []
 
     return parsed_info
 
 
 async def fetch_statistics_from_warframe_market(cache: redis.Redis | None,
                                                 session: aiohttp.ClientSession,
-                                                platform: str = 'pc') -> Tuple[Dict[str, Any], Dict[str, Any]]:
+                                                platform: str = 'pc', items: Dict = None, item_ids: Dict = None) -> \
+        Tuple[Dict[str, Any], Dict[str, Any]]:
     """
     Fetches statistics from warframe.market
     :param cache: redis cache
     :param session: aiohttp session
     :param platform: platform to fetch statistics for
+    :param items: list of warframe.market items, as returned by fetch_items_from_warframe_market; if None, will fetch
+    :param item_ids: dictionary of item names to item ids, as returned by build_item_ids; if None, will build
     :return: tuple of statistic history dictionary and item info dictionary
     """
-    items = await fetch_items_from_warframe_market(cache=cache, session=session)
-    item_ids = build_item_ids(items)
+    if items is None:
+        items = await fetch_items_from_warframe_market(cache=cache, session=session)
+
+    if item_ids is None:
+        item_ids = build_item_ids(items)
 
     statistic_history_dict = defaultdict(lambda: defaultdict(list))
     item_info = {}
 
     time_periods = ['90days']
     statistic_types = ['statistics_closed', 'statistics_live']
```

### Comparing `market-engine-0.1.6/market_engine/API/RelicsRunAPI.py` & `market-engine-0.1.7/market_engine/API/RelicsRunAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.6/market_engine/Common.py` & `market-engine-0.1.7/market_engine/Common.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.6/market_engine/ManifestParser.py` & `market-engine-0.1.7/market_engine/ManifestParser.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.6/market_engine/Models/MarketDatabase.py` & `market-engine-0.1.7/market_engine/Models/MarketDatabase.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.6/market_engine/Models/MarketItem.py` & `market-engine-0.1.7/market_engine/Models/MarketItem.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.6/market_engine/Models/MarketUser.py` & `market-engine-0.1.7/market_engine/Models/MarketUser.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.6/market_engine.egg-info/SOURCES.txt` & `market-engine-0.1.7/market_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.6/setup.py` & `market-engine-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='market-engine',
-    version='0.1.6',
+    version='0.1.7',
     description='Engine for easily getting the orders, statistics, and other stats from warframe.market.',
     author='Jacob McBride',
     author_email='jake55111@gmail.com',
     packages=find_packages(),
     install_requires=[
         'aiohttp~=3.8.4',
         'discord~=2.2.2',
```

