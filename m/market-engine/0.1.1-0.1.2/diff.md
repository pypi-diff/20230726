# Comparing `tmp/market-engine-0.1.1.tar.gz` & `tmp/market-engine-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market-engine-0.1.1.tar", last modified: Wed Jul 26 18:58:10 2023, max compression
+gzip compressed data, was "market-engine-0.1.2.tar", last modified: Wed Jul 26 19:54:18 2023, max compression
```

## Comparing `market-engine-0.1.1.tar` & `market-engine-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 18:58:10.418831 market-engine-0.1.1/
--rw-rw-rw-   0        0        0      216 2023-07-26 18:58:10.418831 market-engine-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 18:58:10.412315 market-engine-0.1.1/market_engine/
-drwxrwxrwx   0        0        0        0 2023-07-26 18:58:10.416831 market-engine-0.1.1/market_engine/API/
--rw-rw-rw-   0        0        0     3166 2023-07-25 21:19:06.000000 market-engine-0.1.1/market_engine/API/ManifestAPI.py
--rw-rw-rw-   0        0        0     5903 2023-07-25 21:05:50.000000 market-engine-0.1.1/market_engine/API/MarketAPI.py
--rw-rw-rw-   0        0        0     6633 2023-07-25 22:30:19.000000 market-engine-0.1.1/market_engine/API/RelicsRunAPI.py
--rw-rw-rw-   0        0        0        0 2023-07-24 20:09:05.000000 market-engine-0.1.1/market_engine/API/__init__.py
--rw-rw-rw-   0        0        0     7954 2023-07-26 01:21:00.000000 market-engine-0.1.1/market_engine/Common.py
--rw-rw-rw-   0        0        0    41594 2023-07-26 17:29:33.000000 market-engine-0.1.1/market_engine/ManifestParser.py
-drwxrwxrwx   0        0        0        0 2023-07-26 18:58:10.418331 market-engine-0.1.1/market_engine/Models/
--rw-rw-rw-   0        0        0    26804 2023-07-26 18:15:33.000000 market-engine-0.1.1/market_engine/Models/MarketDatabase.py
--rw-rw-rw-   0        0        0    12514 2023-07-26 01:09:08.000000 market-engine-0.1.1/market_engine/Models/MarketItem.py
--rw-rw-rw-   0        0        0     7106 2023-07-26 01:14:25.000000 market-engine-0.1.1/market_engine/Models/MarketUser.py
--rw-rw-rw-   0        0        0        0 2023-07-25 16:48:26.000000 market-engine-0.1.1/market_engine/Models/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.1.1/market_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 18:58:10.414830 market-engine-0.1.1/market_engine.egg-info/
--rw-rw-rw-   0        0        0      216 2023-07-26 18:58:10.000000 market-engine-0.1.1/market_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      568 2023-07-26 18:58:10.000000 market-engine-0.1.1/market_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 18:58:10.000000 market-engine-0.1.1/market_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-07-26 18:58:10.000000 market-engine-0.1.1/market_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-26 18:58:10.000000 market-engine-0.1.1/market_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 18:58:10.418831 market-engine-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      573 2023-07-26 18:41:54.000000 market-engine-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:54:18.761540 market-engine-0.1.2/
+-rw-rw-rw-   0        0        0      216 2023-07-26 19:54:18.761540 market-engine-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 19:54:18.756225 market-engine-0.1.2/market_engine/
+drwxrwxrwx   0        0        0        0 2023-07-26 19:54:18.759540 market-engine-0.1.2/market_engine/API/
+-rw-rw-rw-   0        0        0     3166 2023-07-25 21:19:06.000000 market-engine-0.1.2/market_engine/API/ManifestAPI.py
+-rw-rw-rw-   0        0        0     5903 2023-07-25 21:05:50.000000 market-engine-0.1.2/market_engine/API/MarketAPI.py
+-rw-rw-rw-   0        0        0     6633 2023-07-25 22:30:19.000000 market-engine-0.1.2/market_engine/API/RelicsRunAPI.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 20:09:05.000000 market-engine-0.1.2/market_engine/API/__init__.py
+-rw-rw-rw-   0        0        0     7954 2023-07-26 01:21:00.000000 market-engine-0.1.2/market_engine/Common.py
+-rw-rw-rw-   0        0        0    41600 2023-07-26 19:54:08.000000 market-engine-0.1.2/market_engine/ManifestParser.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:54:18.761040 market-engine-0.1.2/market_engine/Models/
+-rw-rw-rw-   0        0        0    26804 2023-07-26 18:15:33.000000 market-engine-0.1.2/market_engine/Models/MarketDatabase.py
+-rw-rw-rw-   0        0        0    12514 2023-07-26 01:09:08.000000 market-engine-0.1.2/market_engine/Models/MarketItem.py
+-rw-rw-rw-   0        0        0     7106 2023-07-26 01:14:25.000000 market-engine-0.1.2/market_engine/Models/MarketUser.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 16:48:26.000000 market-engine-0.1.2/market_engine/Models/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.1.2/market_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:54:18.758025 market-engine-0.1.2/market_engine.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-07-26 19:54:18.000000 market-engine-0.1.2/market_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2023-07-26 19:54:18.000000 market-engine-0.1.2/market_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 19:54:18.000000 market-engine-0.1.2/market_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      251 2023-07-26 19:54:18.000000 market-engine-0.1.2/market_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 19:54:18.000000 market-engine-0.1.2/market_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 19:54:18.762040 market-engine-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-26 19:54:15.000000 market-engine-0.1.2/setup.py
```

### Comparing `market-engine-0.1.1/market_engine/API/ManifestAPI.py` & `market-engine-0.1.2/market_engine/API/ManifestAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.1/market_engine/API/MarketAPI.py` & `market-engine-0.1.2/market_engine/API/MarketAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.1/market_engine/API/RelicsRunAPI.py` & `market-engine-0.1.2/market_engine/API/RelicsRunAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.1/market_engine/Common.py` & `market-engine-0.1.2/market_engine/Common.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.1/market_engine/ManifestParser.py` & `market-engine-0.1.2/market_engine/ManifestParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     }
     for key in rarities:
         if relic_name.endswith(key):
             return rarities[key]
     return ""
 
 
-def get_node_list():
+async def get_node_list():
     """
     Fetches the node list from relics.run
     :return: the node list
     """
     with cache_manager() as cache, session_manager() as session:
         return await fetch_api_data(cache=cache,
                                     session=session,
```

### Comparing `market-engine-0.1.1/market_engine/Models/MarketDatabase.py` & `market-engine-0.1.2/market_engine/Models/MarketDatabase.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.1/market_engine/Models/MarketItem.py` & `market-engine-0.1.2/market_engine/Models/MarketItem.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.1/market_engine/Models/MarketUser.py` & `market-engine-0.1.2/market_engine/Models/MarketUser.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.1/market_engine.egg-info/SOURCES.txt` & `market-engine-0.1.2/market_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.1/setup.py` & `market-engine-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='market-engine',
-    version='0.1.1',
+    version='0.1.2',
     description='Engine for easily getting the orders, statistics, and other stats from warframe.market.',
     author='Jacob McBride',
     author_email='jake55111@gmail.com',
     packages=find_packages(),
     install_requires=[
         'aiohttp~=3.8.4',
-        'redis~=4.6.0',
+        'discord~=2.2.2',
+        'aiolimiter~=1.0.0',
+        'redis~=4.5.4',
+        'requests~=2.29.0',
         'beautifulsoup4~=4.12.2',
-        'PyMySQL~=1.1.0',
+        'PyMySQL~=1.0.3',
         'fuzzywuzzy~=0.18.0',
         'pytz~=2023.3',
-        'aiolimiter~=1.1.0',
+        'python-Levenshtein~=0.21.0',
+        'beautifulsoup4~=4.12.2',
+        'Markdown~=3.4.3',
+        'cryptography~=40.0.2',
         'tenacity~=8.2.2'
     ],
 )
```

