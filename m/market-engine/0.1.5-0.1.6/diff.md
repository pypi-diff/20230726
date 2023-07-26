# Comparing `tmp/market-engine-0.1.5.tar.gz` & `tmp/market-engine-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market-engine-0.1.5.tar", last modified: Wed Jul 26 20:14:46 2023, max compression
+gzip compressed data, was "market-engine-0.1.6.tar", last modified: Wed Jul 26 20:17:32 2023, max compression
```

## Comparing `market-engine-0.1.5.tar` & `market-engine-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 20:14:46.624888 market-engine-0.1.5/
--rw-rw-rw-   0        0        0      216 2023-07-26 20:14:46.624888 market-engine-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 20:14:46.619387 market-engine-0.1.5/market_engine/
-drwxrwxrwx   0        0        0        0 2023-07-26 20:14:46.622888 market-engine-0.1.5/market_engine/API/
--rw-rw-rw-   0        0        0     3166 2023-07-25 21:19:06.000000 market-engine-0.1.5/market_engine/API/ManifestAPI.py
--rw-rw-rw-   0        0        0     5903 2023-07-25 21:05:50.000000 market-engine-0.1.5/market_engine/API/MarketAPI.py
--rw-rw-rw-   0        0        0     6633 2023-07-25 22:30:19.000000 market-engine-0.1.5/market_engine/API/RelicsRunAPI.py
--rw-rw-rw-   0        0        0        0 2023-07-24 20:09:05.000000 market-engine-0.1.5/market_engine/API/__init__.py
--rw-rw-rw-   0        0        0     7954 2023-07-26 01:21:00.000000 market-engine-0.1.5/market_engine/Common.py
--rw-rw-rw-   0        0        0    41612 2023-07-26 20:13:48.000000 market-engine-0.1.5/market_engine/ManifestParser.py
-drwxrwxrwx   0        0        0        0 2023-07-26 20:14:46.624387 market-engine-0.1.5/market_engine/Models/
--rw-rw-rw-   0        0        0    27005 2023-07-26 20:11:38.000000 market-engine-0.1.5/market_engine/Models/MarketDatabase.py
--rw-rw-rw-   0        0        0    12476 2023-07-26 19:57:21.000000 market-engine-0.1.5/market_engine/Models/MarketItem.py
--rw-rw-rw-   0        0        0     7066 2023-07-26 19:57:21.000000 market-engine-0.1.5/market_engine/Models/MarketUser.py
--rw-rw-rw-   0        0        0        0 2023-07-25 16:48:26.000000 market-engine-0.1.5/market_engine/Models/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.1.5/market_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 20:14:46.620887 market-engine-0.1.5/market_engine.egg-info/
--rw-rw-rw-   0        0        0      216 2023-07-26 20:14:46.000000 market-engine-0.1.5/market_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      544 2023-07-26 20:14:46.000000 market-engine-0.1.5/market_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 20:14:46.000000 market-engine-0.1.5/market_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      251 2023-07-26 20:14:46.000000 market-engine-0.1.5/market_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-26 20:14:46.000000 market-engine-0.1.5/market_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 20:14:46.625388 market-engine-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-07-26 20:14:42.000000 market-engine-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:17:32.299163 market-engine-0.1.6/
+-rw-rw-rw-   0        0        0      216 2023-07-26 20:17:32.299163 market-engine-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 20:17:32.293646 market-engine-0.1.6/market_engine/
+drwxrwxrwx   0        0        0        0 2023-07-26 20:17:32.297147 market-engine-0.1.6/market_engine/API/
+-rw-rw-rw-   0        0        0     3166 2023-07-25 21:19:06.000000 market-engine-0.1.6/market_engine/API/ManifestAPI.py
+-rw-rw-rw-   0        0        0     5903 2023-07-25 21:05:50.000000 market-engine-0.1.6/market_engine/API/MarketAPI.py
+-rw-rw-rw-   0        0        0     6633 2023-07-25 22:30:19.000000 market-engine-0.1.6/market_engine/API/RelicsRunAPI.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 20:09:05.000000 market-engine-0.1.6/market_engine/API/__init__.py
+-rw-rw-rw-   0        0        0     7954 2023-07-26 01:21:00.000000 market-engine-0.1.6/market_engine/Common.py
+-rw-rw-rw-   0        0        0    41618 2023-07-26 20:17:10.000000 market-engine-0.1.6/market_engine/ManifestParser.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:17:32.298150 market-engine-0.1.6/market_engine/Models/
+-rw-rw-rw-   0        0        0    27005 2023-07-26 20:11:38.000000 market-engine-0.1.6/market_engine/Models/MarketDatabase.py
+-rw-rw-rw-   0        0        0    12476 2023-07-26 19:57:21.000000 market-engine-0.1.6/market_engine/Models/MarketItem.py
+-rw-rw-rw-   0        0        0     7066 2023-07-26 19:57:21.000000 market-engine-0.1.6/market_engine/Models/MarketUser.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 16:48:26.000000 market-engine-0.1.6/market_engine/Models/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.1.6/market_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:17:32.295648 market-engine-0.1.6/market_engine.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-07-26 20:17:32.000000 market-engine-0.1.6/market_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      544 2023-07-26 20:17:32.000000 market-engine-0.1.6/market_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 20:17:32.000000 market-engine-0.1.6/market_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      251 2023-07-26 20:17:32.000000 market-engine-0.1.6/market_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 20:17:32.000000 market-engine-0.1.6/market_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 20:17:32.299668 market-engine-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-26 20:17:27.000000 market-engine-0.1.6/setup.py
```

### Comparing `market-engine-0.1.5/market_engine/API/ManifestAPI.py` & `market-engine-0.1.6/market_engine/API/ManifestAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.5/market_engine/API/MarketAPI.py` & `market-engine-0.1.6/market_engine/API/MarketAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.5/market_engine/API/RelicsRunAPI.py` & `market-engine-0.1.6/market_engine/API/RelicsRunAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.5/market_engine/Common.py` & `market-engine-0.1.6/market_engine/Common.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.5/market_engine/ManifestParser.py` & `market-engine-0.1.6/market_engine/ManifestParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 
 
 async def get_node_list():
     """
     Fetches the node list from relics.run
     :return: the node list
     """
-    with cache_manager() as cache, session_manager() as session:
+    async with cache_manager() as cache, session_manager() as session:
         return await fetch_api_data(cache=cache,
                                     session=session,
                                     url='https://relics.run/json/solNodes.json',
                                     return_type='json')
 
 
 def parse_name(name: str, parser: Dict) -> str:
```

### Comparing `market-engine-0.1.5/market_engine/Models/MarketDatabase.py` & `market-engine-0.1.6/market_engine/Models/MarketDatabase.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.5/market_engine/Models/MarketItem.py` & `market-engine-0.1.6/market_engine/Models/MarketItem.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.5/market_engine/Models/MarketUser.py` & `market-engine-0.1.6/market_engine/Models/MarketUser.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.5/market_engine.egg-info/SOURCES.txt` & `market-engine-0.1.6/market_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.5/setup.py` & `market-engine-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='market-engine',
-    version='0.1.5',
+    version='0.1.6',
     description='Engine for easily getting the orders, statistics, and other stats from warframe.market.',
     author='Jacob McBride',
     author_email='jake55111@gmail.com',
     packages=find_packages(),
     install_requires=[
         'aiohttp~=3.8.4',
         'discord~=2.2.2',
```

