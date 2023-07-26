# Comparing `tmp/market-engine-0.1.0.tar.gz` & `tmp/market-engine-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market-engine-0.1.0.tar", last modified: Wed Jul 26 01:43:41 2023, max compression
+gzip compressed data, was "market-engine-0.1.1.tar", last modified: Wed Jul 26 18:58:10 2023, max compression
```

## Comparing `market-engine-0.1.0.tar` & `market-engine-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 01:43:41.449317 market-engine-0.1.0/
--rw-rw-rw-   0        0        0      216 2023-07-26 01:43:41.448815 market-engine-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 01:43:41.443316 market-engine-0.1.0/market_engine/
-drwxrwxrwx   0        0        0        0 2023-07-26 01:43:41.447315 market-engine-0.1.0/market_engine/API/
--rw-rw-rw-   0        0        0     3166 2023-07-25 21:19:06.000000 market-engine-0.1.0/market_engine/API/ManifestAPI.py
--rw-rw-rw-   0        0        0     5903 2023-07-25 21:05:50.000000 market-engine-0.1.0/market_engine/API/MarketAPI.py
--rw-rw-rw-   0        0        0     6633 2023-07-25 22:30:19.000000 market-engine-0.1.0/market_engine/API/RelicsRunAPI.py
--rw-rw-rw-   0        0        0        0 2023-07-24 20:09:05.000000 market-engine-0.1.0/market_engine/API/__init__.py
--rw-rw-rw-   0        0        0     7954 2023-07-26 01:21:00.000000 market-engine-0.1.0/market_engine/Common.py
--rw-rw-rw-   0        0        0    41633 2023-07-26 01:42:45.000000 market-engine-0.1.0/market_engine/ManifestParser.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:43:41.448815 market-engine-0.1.0/market_engine/Models/
--rw-rw-rw-   0        0        0    26839 2023-07-26 01:09:08.000000 market-engine-0.1.0/market_engine/Models/MarketDatabase.py
--rw-rw-rw-   0        0        0    12514 2023-07-26 01:09:08.000000 market-engine-0.1.0/market_engine/Models/MarketItem.py
--rw-rw-rw-   0        0        0     7106 2023-07-26 01:14:25.000000 market-engine-0.1.0/market_engine/Models/MarketUser.py
--rw-rw-rw-   0        0        0        0 2023-07-25 16:48:26.000000 market-engine-0.1.0/market_engine/Models/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.1.0/market_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:43:41.445816 market-engine-0.1.0/market_engine.egg-info/
--rw-rw-rw-   0        0        0      216 2023-07-26 01:43:41.000000 market-engine-0.1.0/market_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      568 2023-07-26 01:43:41.000000 market-engine-0.1.0/market_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 01:43:41.000000 market-engine-0.1.0/market_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      251 2023-07-26 01:43:41.000000 market-engine-0.1.0/market_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-26 01:43:41.000000 market-engine-0.1.0/market_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 01:43:41.449317 market-engine-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-07-26 01:43:37.000000 market-engine-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:58:10.418831 market-engine-0.1.1/
+-rw-rw-rw-   0        0        0      216 2023-07-26 18:58:10.418831 market-engine-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 18:58:10.412315 market-engine-0.1.1/market_engine/
+drwxrwxrwx   0        0        0        0 2023-07-26 18:58:10.416831 market-engine-0.1.1/market_engine/API/
+-rw-rw-rw-   0        0        0     3166 2023-07-25 21:19:06.000000 market-engine-0.1.1/market_engine/API/ManifestAPI.py
+-rw-rw-rw-   0        0        0     5903 2023-07-25 21:05:50.000000 market-engine-0.1.1/market_engine/API/MarketAPI.py
+-rw-rw-rw-   0        0        0     6633 2023-07-25 22:30:19.000000 market-engine-0.1.1/market_engine/API/RelicsRunAPI.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 20:09:05.000000 market-engine-0.1.1/market_engine/API/__init__.py
+-rw-rw-rw-   0        0        0     7954 2023-07-26 01:21:00.000000 market-engine-0.1.1/market_engine/Common.py
+-rw-rw-rw-   0        0        0    41594 2023-07-26 17:29:33.000000 market-engine-0.1.1/market_engine/ManifestParser.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:58:10.418331 market-engine-0.1.1/market_engine/Models/
+-rw-rw-rw-   0        0        0    26804 2023-07-26 18:15:33.000000 market-engine-0.1.1/market_engine/Models/MarketDatabase.py
+-rw-rw-rw-   0        0        0    12514 2023-07-26 01:09:08.000000 market-engine-0.1.1/market_engine/Models/MarketItem.py
+-rw-rw-rw-   0        0        0     7106 2023-07-26 01:14:25.000000 market-engine-0.1.1/market_engine/Models/MarketUser.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 16:48:26.000000 market-engine-0.1.1/market_engine/Models/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.1.1/market_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:58:10.414830 market-engine-0.1.1/market_engine.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-07-26 18:58:10.000000 market-engine-0.1.1/market_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2023-07-26 18:58:10.000000 market-engine-0.1.1/market_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 18:58:10.000000 market-engine-0.1.1/market_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2023-07-26 18:58:10.000000 market-engine-0.1.1/market_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 18:58:10.000000 market-engine-0.1.1/market_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 18:58:10.418831 market-engine-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      573 2023-07-26 18:41:54.000000 market-engine-0.1.1/setup.py
```

### Comparing `market-engine-0.1.0/market_engine/API/ManifestAPI.py` & `market-engine-0.1.1/market_engine/API/ManifestAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.0/market_engine/API/MarketAPI.py` & `market-engine-0.1.1/market_engine/API/MarketAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.0/market_engine/API/RelicsRunAPI.py` & `market-engine-0.1.1/market_engine/API/RelicsRunAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.0/market_engine/Common.py` & `market-engine-0.1.1/market_engine/Common.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.0/market_engine/ManifestParser.py` & `market-engine-0.1.1/market_engine/ManifestParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import re
 from typing import Dict
 
-import requests
-
 from market_engine.Common import fetch_api_data, cache_manager, session_manager
 
 # Additional categories that are exclusive to warframe.market
 ADDITIONAL_CATEGORIES = ['ArcaneHelmets', 'Imprints', 'VeiledRivenMods', 'Emotes',
                          'ArmorPieces', "CollectorItems"]
 
 # Overrides for items that have different names on warframe.market
@@ -177,15 +175,15 @@
     with cache_manager() as cache, session_manager() as session:
         return await fetch_api_data(cache=cache,
                                     session=session,
                                     url='https://relics.run/json/solNodes.json',
                                     return_type='json')
 
 
-def parse_name(name: str, parser: Dict[str, str]) -> str:
+def parse_name(name: str, parser: Dict) -> str:
     """
     Parses the name of the given item using the parser dictionary
     :param name: the name of the manifest item to parse
     :param parser: the parser dictionary
     :return: the parsed name
     """
     if name in parser:
@@ -202,15 +200,15 @@
                 return parser[parser[name]]
             else:
                 return parser[name]
     else:
         return name
 
 
-def build_parser(manifest_dict: Dict[str, str]) -> Dict[str, str]:
+def build_parser(manifest_dict: Dict) -> Dict[str, str]:
     """
     Builds the parser dictionary from the manifest dictionary
     :param manifest_dict: the manifest dictionary
     :return: the parser dictionary, converting internal names to user-friendly names
     """
     # Base parser dictionary
     parser_base = {'AP_POWER': 'Zenurik',
```

### Comparing `market-engine-0.1.0/market_engine/Models/MarketDatabase.py` & `market-engine-0.1.1/market_engine/Models/MarketDatabase.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,19 +272,19 @@
         :param database: the database to connect to
         """
         self.connection: Connection = pymysql.connect(user=user,
                                                       password=password,
                                                       host=host,
                                                       database=database)
 
-        self.all_items = self._get_all_items()
+        self.all_items = self.get_all_items()
         self.users: Dict[str, str] = {}
 
-    def _execute_query(self, query: str, *params, fetch: str = 'all',
-                       commit: bool = False, many: bool = False) -> Union[Tuple, List[Tuple], None]:
+    def execute_query(self, query: str, *params, fetch: str = 'all',
+                      commit: bool = False, many: bool = False) -> Union[Tuple, List[Tuple], None]:
         """
         Executes a query on the database, and returns the result if applicable
         :param query: the query to execute
         :param params: the parameters to pass to the query, accepts multiple parameters
         :param fetch: the type of fetch to perform, either 'one' or 'all'
         :param commit: whether or not to commit the query
         :param many: whether or not to execute the query with multiple parameters
@@ -302,33 +302,33 @@
                 self.connection.commit()
 
             if fetch == 'one':
                 return cur.fetchone()
             elif fetch == 'all':
                 return cur.fetchall()
 
-    def _get_all_items(self) -> List[dict]:
+    def get_all_items(self) -> List[dict]:
         """
         Gets all items from the database
         :return: a list of all items
         """
-        all_data = self._execute_query(self._GET_ALL_ITEMS_QUERY)
+        all_data = self.execute_query(self._GET_ALL_ITEMS_QUERY)
 
         all_items: List[dict] = []
         for item_id, item_name, item_type, url_name, thumb, max_rank, alias in all_data:
             aliases = []
             if alias:
                 aliases = alias.split(',')
 
             all_items.append({'id': item_id, 'item_name': item_name, 'item_type': item_type,
                               'url_name': url_name, 'thumb': thumb, 'max_rank': max_rank, 'aliases': aliases})
 
         return all_items
 
-    def _save_items(self, items, item_ids, item_info) -> None:
+    def save_items(self, items, item_ids, item_info) -> None:
         """
         Saves items to the database
         :param items: dictionary of items to save
         :param item_ids: dictionary of item names to item ids
         :param item_info: dictionary of item info
         :return: None
         """
@@ -341,88 +341,88 @@
 
         new_item_ids = {}
         for item, item_id in item_ids.items():
             if item_id not in [x['id'] for x in items]:
                 new_item_ids[item] = item_id
         data_list.extend([(new_item_ids[item], item, None, None, None) for item in new_item_ids])
 
-        self._execute_query(self._INSERT_ITEM_QUERY, data_list, many=True, commit=True)
+        self.execute_query(self._INSERT_ITEM_QUERY, data_list, many=True, commit=True)
 
-    def _save_item_tags(self, item_info: Dict[str, Any]) -> None:
+    def save_item_tags(self, item_info: Dict[str, Any]) -> None:
         """
         Saves item tags to the database
         :param item_info: dictionary of item info
         :return: None
         """
         data_list = []
         for item in item_info:
             for tag in item_info[item]['tags']:
                 data_list.append((item, tag))
 
-        self._execute_query(self._INSERT_ITEM_TAGS_QUERY, data_list, many=True, commit=True)
+        self.execute_query(self._INSERT_ITEM_TAGS_QUERY, data_list, many=True, commit=True)
 
-    def _save_item_subtypes(self, item_info: Dict[str, Any]) -> None:
+    def save_item_subtypes(self, item_info: Dict[str, Any]) -> None:
         """
         Saves item subtypes to the database
         :param item_info: dictionary of item info
         :return: None
         """
         data_list = []
         for item in item_info:
             for subtype in item_info[item]['subtypes']:
                 data_list.append((item, subtype))
 
-        self._execute_query(self._INSERT_ITEM_SUBTYPE_QUERY, data_list, many=True, commit=True)
+        self.execute_query(self._INSERT_ITEM_SUBTYPE_QUERY, data_list, many=True, commit=True)
 
-    def _save_items_in_set(self, item_info: Dict[str, Any]) -> None:
+    def save_items_in_set(self, item_info: Dict[str, Any]) -> None:
         """
         Saves items in a set to the database
         :param item_info: dictionary of item info
         :return: None
         """
         data_list = []
         for item in item_info:
             for item_in_set in item_info[item]['set_items']:
                 data_list.append((item, item_in_set))
 
-        self._execute_query(self._INSERT_ITEMS_IN_SET_QUERY, data_list, many=True, commit=True)
+        self.execute_query(self._INSERT_ITEMS_IN_SET_QUERY, data_list, many=True, commit=True)
 
     def get_sub_type_data(self) -> Dict[str, List[str]]:
         """
         Gets sub type data from the database
         :return: dictionary of item names to sub types
         """
-        sub_type_data = self._execute_query(self._GET_SUBTYPE_DATA_QUERY)
+        sub_type_data = self.execute_query(self._GET_SUBTYPE_DATA_QUERY)
 
         return {row[0]: row[1].split(',') for row in sub_type_data}
 
     def get_item_id_dict(self) -> Dict[str, str]:
         """
         Gets item data from the database
         :return: dictionary of item names to item ids
         """
-        return dict(self._execute_query(self._GET_ITEM_DICT_QUERY))
+        return dict(self.execute_query(self._GET_ITEM_DICT_QUERY))
 
     def get_all_sets(self) -> Dict[str, str]:
         """
         Gets all sets from the database
         :return: dictionary of set ids to set names
         """
-        return dict(self._execute_query(self._GET_ALL_SETS_QUERY))
+        return dict(self.execute_query(self._GET_ALL_SETS_QUERY))
 
     def save_item_categories(self, item_categories: Dict[str, Dict[str, str]]) -> None:
         """
         Saves item categories to the database
         :param item_categories: dictionary of item types to item ids
         :return: None
         """
         for item_type in item_categories:
-            self._execute_query(self._SET_ITEM_CATEGORIES_QUERY,
-                                *[(item_type, item_id) for item_id in item_categories[item_type].values()],
-                                many=True, commit=True)
+            self.execute_query(self._SET_ITEM_CATEGORIES_QUERY,
+                               *[(item_type, item_id) for item_id in item_categories[item_type].values()],
+                               many=True, commit=True)
 
     def insert_item_statistics(self, last_save_date: datetime = None,
                                platform: str = 'pc') -> None:
         """
         Inserts item statistics into the database
         :param last_save_date: the date to fetch files after
         :param platform: the platform to fetch files for
@@ -458,15 +458,15 @@
                 logger.info(f"Progress: Batch {i // batch_size + 1} of {total_batches} completed")
 
     def get_most_recent_statistic_date(self) -> Optional[datetime]:
         """
         Gets the most recent date in the database
         :return: the most recent date in the database if applicable, otherwise None
         """
-        most_recent_datetime: datetime = self._execute_query(self._GET_MOST_RECENT_DATE_QUERY, fetch='one')[0]
+        most_recent_datetime: datetime = self.execute_query(self._GET_MOST_RECENT_DATE_QUERY, fetch='one')[0]
 
         most_recent_date = None
         if most_recent_datetime is not None:
             # Convert the datetime to UTC
             utc_datetime = most_recent_datetime.astimezone(timezone('UTC'))
             most_recent_date = utc_datetime.date()
 
@@ -480,15 +480,15 @@
         Gets a user from the database
         :param user: the user to get
         :param fetch_user_data: whether or not to fetch user data from the API
         :param fetch_orders: whether or not to fetch orders from the API
         :param fetch_reviews: whether or not to fetch reviews from the API
         :return: the user if applicable, otherwise None
         """
-        result = self._execute_query(self._GET_CORRECT_CASE_QUERY, user, fetch='one')
+        result = self.execute_query(self._GET_CORRECT_CASE_QUERY, user, fetch='one')
 
         if result is None:
             # Username not found, attempt to fetch from API
             profile = await MarketUser.fetch_user_data(user)
 
             if profile is None:
                 return None
@@ -539,40 +539,40 @@
 
     def get_item_statistics(self, item_id: str) -> Tuple[Tuple[Any, ...], ...]:
         """
         Gets item statistics from the database
         :param item_id: the item to get statistics for
         :return: the item statistics
         """
-        return self._execute_query(self._GET_ITEM_STATISTICS_QUERY, item_id, fetch='all')
+        return self.execute_query(self._GET_ITEM_STATISTICS_QUERY, item_id, fetch='all')
 
     def get_item_volume(self, item_id: str, days: int = 31) -> Tuple[Tuple[Any, ...], ...]:
         """
         Gets item volume from the database
         :param item_id: the item to get volume for
         :param days: the number of days to get volume for
         :return: the item volume
         """
-        return self._execute_query(self._GET_ITEM_VOLUME_QUERY, days, item_id, fetch='all')
+        return self.execute_query(self._GET_ITEM_VOLUME_QUERY, days, item_id, fetch='all')
 
     def get_item_price_history(self, item_id: str) -> Dict[str, str]:
         """
         Gets item price history from the database
         :param item_id: the item to get price history for
         :return: the item price history
         """
-        return dict(self._execute_query(self._GET_PRICE_HISTORY_QUERY, item_id, fetch='all'))
+        return dict(self.execute_query(self._GET_PRICE_HISTORY_QUERY, item_id, fetch='all'))
 
     def get_item_demand_history(self, item_id: str) -> Dict[str, str]:
         """
         Gets item demand history from the database
         :param item_id: the item to get demand history for
         :return: the item demand history
         """
-        return dict(self._execute_query(self._GET_DEMAND_HISTORY_QUERY, item_id, fetch='all'))
+        return dict(self.execute_query(self._GET_DEMAND_HISTORY_QUERY, item_id, fetch='all'))
 
     def _get_fuzzy_item(self, item_name: str) -> Optional[Dict[str, str]]:
         """
         Gets the best match for an item name from the database
         :param item_name: the item name to get a match for
         :return: the best match if applicable, otherwise None
         """
@@ -582,53 +582,53 @@
 
     def get_item_parts(self, item_id: str) -> Tuple[Tuple[Any, ...], ...]:
         """
         Gets item parts from the database
         :param item_id: the item to get parts for
         :return: the item parts
         """
-        return self._execute_query(self._GET_ITEMS_IN_SET_QUERY, item_id, fetch='all')
+        return self.execute_query(self._GET_ITEMS_IN_SET_QUERY, item_id, fetch='all')
 
     def get_word_aliases(self) -> Dict[str, str]:
         """
         Gets word aliases from the database
         :return: the word aliases
         """
-        return dict(self._execute_query(self._GET_ALL_WORD_ALIASES_QUERY, fetch='all'))
+        return dict(self.execute_query(self._GET_ALL_WORD_ALIASES_QUERY, fetch='all'))
 
     async def add_item_alias(self, item_id: str, alias: str) -> None:
         """
         Adds an alias to an item
         :param item_id: the item to add an alias to
         :param alias: the alias to add
         :return: None
         """
-        self._execute_query(self._ADD_ITEM_ALIAS_QUERY, item_id, alias, commit=True)
-        self.all_items = self._get_all_items()  # Update the list of all items
+        self.execute_query(self._ADD_ITEM_ALIAS_QUERY, item_id, alias, commit=True)
+        self.all_items = self.get_all_items()  # Update the list of all items
 
     def remove_item_alias(self, item_id: str, alias: str) -> None:
-        self._execute_query(self._REMOVE_ITEM_ALIAS_QUERY, item_id, alias, commit=True)
-        self.all_items = self._get_all_items()  # Update the list of all items
+        self.execute_query(self._REMOVE_ITEM_ALIAS_QUERY, item_id, alias, commit=True)
+        self.all_items = self.get_all_items()  # Update the list of all items
 
     async def add_word_alias(self, word: str, alias: str) -> None:
         """
         Adds an alias to a word, used for fuzzy matching
         :param word: the word to add an alias to
         :param alias: the alias to add
         :return: None
         """
-        self._execute_query(self._ADD_WORD_ALIAS_QUERY, word, alias, commit=True)
+        self.execute_query(self._ADD_WORD_ALIAS_QUERY, word, alias, commit=True)
 
     def update_usernames(self) -> None:
         """
         Updates usernames in the database
         :return: None
         """
         # Fetch all user data first
-        user_data = dict(self._execute_query(self._GET_ALL_USERS_QUERY, fetch='all'))
+        user_data = dict(self.execute_query(self._GET_ALL_USERS_QUERY, fetch='all'))
 
         # Prepare batch queries
         update_queries = []
         history_queries = []
         now = datetime.now()
 
         users = self.users.copy()
@@ -642,11 +642,11 @@
                 logger.info(f"Updating username for user {user_id} to {new_ingame_name}")
 
                 update_queries.append((user_id, new_ingame_name))
                 history_queries.append((user_id, new_ingame_name, now))
 
         # Execute the queries
         if update_queries:
-            self._execute_query(self._UPSERT_USER_QUERY, update_queries, commit=True, many=True)
+            self.execute_query(self._UPSERT_USER_QUERY, update_queries, commit=True, many=True)
 
         if history_queries:
-            self._execute_query(self._INSERT_USERNAME_HISTORY_QUERY, history_queries, commit=True, many=True)
+            self.execute_query(self._INSERT_USERNAME_HISTORY_QUERY, history_queries, commit=True, many=True)
```

### Comparing `market-engine-0.1.0/market_engine/Models/MarketItem.py` & `market-engine-0.1.1/market_engine/Models/MarketItem.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.0/market_engine/Models/MarketUser.py` & `market-engine-0.1.1/market_engine/Models/MarketUser.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.0/market_engine.egg-info/SOURCES.txt` & `market-engine-0.1.1/market_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.0/setup.py` & `market-engine-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='market-engine',
-    version='0.1.0',
+    version='0.1.1',
     description='Engine for easily getting the orders, statistics, and other stats from warframe.market.',
     author='Jacob McBride',
     author_email='jake55111@gmail.com',
     packages=find_packages(),
     install_requires=[
         'aiohttp~=3.8.4',
-        'discord~=2.2.2',
-        'aiolimiter~=1.0.0',
-        'redis~=4.5.4',
-        'requests~=2.29.0',
+        'redis~=4.6.0',
         'beautifulsoup4~=4.12.2',
-        'PyMySQL~=1.0.3',
+        'PyMySQL~=1.1.0',
         'fuzzywuzzy~=0.18.0',
         'pytz~=2023.3',
-        'python-Levenshtein~=0.21.0',
-        'beautifulsoup4~=4.12.2',
-        'Markdown~=3.4.3',
-        'cryptography~=40.0.2',
+        'aiolimiter~=1.1.0',
         'tenacity~=8.2.2'
     ],
 )
```

