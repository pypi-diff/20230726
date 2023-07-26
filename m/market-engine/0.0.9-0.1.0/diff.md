# Comparing `tmp/market-engine-0.0.9.tar.gz` & `tmp/market-engine-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market-engine-0.0.9.tar", last modified: Thu Jun 15 00:44:59 2023, max compression
+gzip compressed data, was "market-engine-0.1.0.tar", last modified: Wed Jul 26 01:43:41 2023, max compression
```

## Comparing `market-engine-0.0.9.tar` & `market-engine-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 00:44:59.728463 market-engine-0.0.9/
--rw-rw-rw-   0        0        0      216 2023-06-15 00:44:59.728463 market-engine-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 00:44:59.723464 market-engine-0.0.9/market_engine/
--rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.0.9/market_engine/__init__.py
--rw-rw-rw-   0        0        0      932 2023-05-26 19:30:35.000000 market-engine-0.0.9/market_engine/common.py
-drwxrwxrwx   0        0        0        0 2023-06-15 00:44:59.728463 market-engine-0.0.9/market_engine/modules/
--rw-rw-rw-   0        0        0    13903 2023-06-15 00:44:05.000000 market-engine-0.0.9/market_engine/modules/MarketAPI.py
--rw-rw-rw-   0        0        0     6661 2023-06-14 23:56:00.000000 market-engine-0.0.9/market_engine/modules/MarketDB.py
--rw-rw-rw-   0        0        0    15103 2023-06-15 00:38:10.000000 market-engine-0.0.9/market_engine/modules/MarketData.py
--rw-rw-rw-   0        0        0        0 2023-05-26 19:04:43.000000 market-engine-0.0.9/market_engine/modules/__init__.py
--rw-rw-rw-   0        0        0    38904 2023-05-26 19:04:00.000000 market-engine-0.0.9/market_engine/modules/categories.py
-drwxrwxrwx   0        0        0        0 2023-06-15 00:44:59.726464 market-engine-0.0.9/market_engine.egg-info/
--rw-rw-rw-   0        0        0      216 2023-06-15 00:44:59.000000 market-engine-0.0.9/market_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2023-06-15 00:44:59.000000 market-engine-0.0.9/market_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 00:44:59.000000 market-engine-0.0.9/market_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-06-15 00:44:59.000000 market-engine-0.0.9/market_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-15 00:44:59.000000 market-engine-0.0.9/market_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 00:44:59.728463 market-engine-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-06-15 00:44:54.000000 market-engine-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:43:41.449317 market-engine-0.1.0/
+-rw-rw-rw-   0        0        0      216 2023-07-26 01:43:41.448815 market-engine-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 01:43:41.443316 market-engine-0.1.0/market_engine/
+drwxrwxrwx   0        0        0        0 2023-07-26 01:43:41.447315 market-engine-0.1.0/market_engine/API/
+-rw-rw-rw-   0        0        0     3166 2023-07-25 21:19:06.000000 market-engine-0.1.0/market_engine/API/ManifestAPI.py
+-rw-rw-rw-   0        0        0     5903 2023-07-25 21:05:50.000000 market-engine-0.1.0/market_engine/API/MarketAPI.py
+-rw-rw-rw-   0        0        0     6633 2023-07-25 22:30:19.000000 market-engine-0.1.0/market_engine/API/RelicsRunAPI.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 20:09:05.000000 market-engine-0.1.0/market_engine/API/__init__.py
+-rw-rw-rw-   0        0        0     7954 2023-07-26 01:21:00.000000 market-engine-0.1.0/market_engine/Common.py
+-rw-rw-rw-   0        0        0    41633 2023-07-26 01:42:45.000000 market-engine-0.1.0/market_engine/ManifestParser.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:43:41.448815 market-engine-0.1.0/market_engine/Models/
+-rw-rw-rw-   0        0        0    26839 2023-07-26 01:09:08.000000 market-engine-0.1.0/market_engine/Models/MarketDatabase.py
+-rw-rw-rw-   0        0        0    12514 2023-07-26 01:09:08.000000 market-engine-0.1.0/market_engine/Models/MarketItem.py
+-rw-rw-rw-   0        0        0     7106 2023-07-26 01:14:25.000000 market-engine-0.1.0/market_engine/Models/MarketUser.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 16:48:26.000000 market-engine-0.1.0/market_engine/Models/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.1.0/market_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:43:41.445816 market-engine-0.1.0/market_engine.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-07-26 01:43:41.000000 market-engine-0.1.0/market_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2023-07-26 01:43:41.000000 market-engine-0.1.0/market_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 01:43:41.000000 market-engine-0.1.0/market_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      251 2023-07-26 01:43:41.000000 market-engine-0.1.0/market_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 01:43:41.000000 market-engine-0.1.0/market_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 01:43:41.449317 market-engine-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-26 01:43:37.000000 market-engine-0.1.0/setup.py
```

### Comparing `market-engine-0.0.9/market_engine/modules/categories.py` & `market-engine-0.1.0/market_engine/ManifestParser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import re
+from typing import Dict
 
 import requests
 
+from market_engine.Common import fetch_api_data, cache_manager, session_manager
+
+# Additional categories that are exclusive to warframe.market
 ADDITIONAL_CATEGORIES = ['ArcaneHelmets', 'Imprints', 'VeiledRivenMods', 'Emotes',
                          'ArmorPieces', "CollectorItems"]
 
+# Overrides for items that have different names on warframe.market
 OVERRIDES = {
     'Prisma Dual Decurions': 'Prisma Dual Decurion'
 }
 
+# Manual categories for items that are not in the manifest
 MANUAL_CATEGORIES = {
     'Scan Aquatic Lifeforms': 'Mods',
     "Kavasa Prime Kubrow Collar Blueprint": "Misc",
     'Equilibrium (Steam Pinnacle Pack)': 'CollectorItems',
     'Corpus Void Key': 'CollectorItems',
     'Vay Hek Frequency Triangulator': 'CollectorItems',
     'Ancient Fusion Core': 'CollectorItems',
@@ -29,30 +35,40 @@
     'Meridian Armor Set': 'ArmorPieces',
     'Perrin Armor Set': 'ArmorPieces',
     'Ostron Armor Set': 'ArmorPieces',
     'Hexis Armor Set': 'ArmorPieces',
     'Kavasa Prime Kubrow Collar Set': 'Misc'
 }
 
+# Armor types that are used to determine the category of an item
 ARMOR_TYPES = [
     'Chest Plate', 'Arm Spurs', 'Arm Plates', 'Leg Spurs', 'Arm Guards', 'Leg Guards',
     'Chest Marker', 'Knee Guards', 'Chest Piece', 'Spurs', 'Chest Guard', "Arm Insignia"
 ]
 
+# Category mappings for items that are not in the manifest
 CATEGORY_MAPPINGS = [
     (re.compile(r"Arcane.*Helmet"), 'ArcaneHelmets'),
     (re.compile(r".*Imprint"), 'Imprints'),
     (re.compile(r".*Augment Mod"), 'Mods'),
     (re.compile(r".*(Veiled)"), 'VeiledRivenMods'),
     (re.compile(r".*Emote"), 'Emotes'),
     (re.compile("|".join(ARMOR_TYPES)), 'ArmorPieces'),
     (re.compile(r"(.*) Set"), lambda match, d: d.get(match.group(1))),
 ]
 
-def find_category(item, flattened_type_dict):
+
+def find_category(item: str,
+                  flattened_type_dict: Dict[str, str]) -> str:
+    """
+    Finds the category of the given item using the flattened type dictionary
+    :param item: item to find the category of
+    :param flattened_type_dict: flattened type dictionary, as returned by gen_type_dict
+    :return: category of the item
+    """
     # Check if the item is in MANUAL_CATEGORIES
     if item in MANUAL_CATEGORIES:
         return MANUAL_CATEGORIES[item]
 
     # Returns the next item in the iterable that evaluates to True
     # If no item evaluates to True, returns 'Misc'
     # Uses CATEGORY_MAPPINGS to determine the category
@@ -63,15 +79,34 @@
                             for pattern, category
                             in CATEGORY_MAPPINGS
                             if pattern.match(item)),
                            (None, 'Misc'))
     return category(match, flattened_type_dict) if callable(category) else category
 
 
-def process_item(item, item_type, wfm_item_data, wfm_item_data_lower, wfm_items_categorized, all_items, overrides, manual_categories):
+def process_item(item: str,
+                 item_type: str,
+                 wfm_item_data: Dict[str, str],
+                 wfm_item_data_lower: Dict[str, str],
+                 wfm_items_categorized: Dict[str, Dict[str, str]],
+                 all_items: set,
+                 overrides: Dict[str, str],
+                 manual_categories: Dict[str, str]) -> None:
+    """
+    Processes the given item, and adds it to the appropriate category
+    :param item: the item to process
+    :param item_type: the item type of the item
+    :param wfm_item_data: the warframe.market item data
+    :param wfm_item_data_lower: the warframe.market item data, with the keys converted to lowercase
+    :param wfm_items_categorized: the categorized warframe.market item data
+    :param all_items: set of all items
+    :param overrides: overrides for items that have different names on warframe.market
+    :param manual_categories: manual categories for items that are not in the manifest
+    :return: None
+    """
     if item in overrides:
         item = overrides[item]
 
     if item in manual_categories:
         return
 
     original_item_name = wfm_item_data_lower.get(item.lower())
@@ -79,57 +114,84 @@
     if original_item_name:
         all_items.add(original_item_name)
         wfm_items_categorized[item_type][original_item_name] = wfm_item_data[original_item_name]
     else:
         all_items.add(item)
 
 
-def get_wfm_item_categorized(wfm_item_data, manifest_dict, wf_parser):
+def get_wfm_item_categorized(wfm_item_data: Dict[str, str],
+                             manifest_dict: Dict[str, str],
+                             wf_parser: Dict[str, str]) -> Dict[str, Dict[str, str]]:
+    """
+    Categorizes the warframe.market item data
+    :param wfm_item_data: the warframe.market item data
+    :param manifest_dict: the manifest dictionary
+    :param wf_parser: the warframe parser dictionary
+    :return: the categorized warframe.market item data
+    """
     type_dict = gen_type_dict(manifest_dict, wf_parser)
     wfm_item_data_lower = {k.lower(): k for k, v in wfm_item_data.items()}
     all_items = set()
 
     wfm_items_categorized = {k: {} for k in list(type_dict) + ADDITIONAL_CATEGORIES}
 
     for item_type, items in type_dict.items():
         for item in items:
-            process_item(item, item_type, wfm_item_data, wfm_item_data_lower, wfm_items_categorized, all_items, OVERRIDES, MANUAL_CATEGORIES)
+            process_item(item, item_type, wfm_item_data, wfm_item_data_lower, wfm_items_categorized, all_items,
+                         OVERRIDES, MANUAL_CATEGORIES)
 
     flattened_type_dict = {item: item_type for item_type, items in type_dict.items() for item in items}
     uncategorized_items = set(wfm_item_data.keys()) - all_items
 
     for item in uncategorized_items:
         category = find_category(item, flattened_type_dict)
         wfm_items_categorized[category][item] = wfm_item_data[item]
 
     wfm_items_categorized = {item_type: items for item_type, items in sorted(wfm_items_categorized.items()) if items}
 
     return wfm_items_categorized
 
 
-def parse_rarity(relic_name):
+def parse_rarity(relic_name: str):
+    """
+    Parses the rarity of the given relic name
+    :param relic_name: the relic name to parse
+    :return: the rarity of the relic
+    """
     rarities = {
         "Bronze": "Intact",
         "Silver": "Exceptional",
         "Gold": "Flawless",
         "Platinum": "Radiant"
     }
     for key in rarities:
         if relic_name.endswith(key):
             return rarities[key]
     return ""
 
 
 def get_node_list():
-    nodes = requests.get('https://relics.run/json/solNodes.json').json()
-
-    return nodes
-
-
-def parse_name(name, parser):
+    """
+    Fetches the node list from relics.run
+    :return: the node list
+    """
+    with cache_manager() as cache, session_manager() as session:
+        return await fetch_api_data(cache=cache,
+                                    session=session,
+                                    url='https://relics.run/json/solNodes.json',
+                                    return_type='json')
+
+
+def parse_name(name: str, parser: Dict[str, str]) -> str:
+    """
+    Parses the name of the given item using the parser dictionary
+    :param name: the name of the manifest item to parse
+    :param parser: the parser dictionary
+    :return: the parsed name
+    """
     if name in parser:
         if isinstance(parser[name], dict):
             mission_node = parser[name]['node']
             if 'planet' in parser[name]:
                 mission_node += f" - {parser[name]['planet']}"
             return mission_node
         else:
@@ -140,15 +202,21 @@
                 return parser[parser[name]]
             else:
                 return parser[name]
     else:
         return name
 
 
-def build_parser(manifest_dict):
+def build_parser(manifest_dict: Dict[str, str]) -> Dict[str, str]:
+    """
+    Builds the parser dictionary from the manifest dictionary
+    :param manifest_dict: the manifest dictionary
+    :return: the parser dictionary, converting internal names to user-friendly names
+    """
+    # Base parser dictionary
     parser_base = {'AP_POWER': 'Zenurik',
                    'AP_TACTIC': 'Naramon',
                    'AP_DEFENSE': 'Vazarin',
                    'AP_PRECEPT': 'Penjaga',
                    'AP_ATTACK': 'Madurai',
                    'AP_UMBRA': 'Umbra',
                    'AP_WARD': 'Unairu',
@@ -180,15 +248,14 @@
                    '/Lotus/Weapons/SolarisUnited/Secondary/LotusModularSecondary': 'Kitgun',
                    '/Lotus/Weapons/Ostron/Melee/LotusModularWeapon': 'Zaw',
                    '/Lotus/Weapons/SolarisUnited/Secondary/LotusModularSecondaryBeam': 'Kitgun',
                    '/Lotus/Powersuits/Wraith/Reaper': 'Shadow Claws',
                    '/Lotus/Powersuits/Yareli/BoardSuit': 'Merulina',
                    '/Lotus/Types/Friendly/Pets/MoaPets/MoaPetPowerSuit': 'Moa',
                    '/Lotus/Types/Game/CrewShip/RailJack/DefaultHarness': 'Railjack Harness',
-                   '/Lotus/Types/Gameplay/InfestedMicroplanet/EncounterObjects/TestPartItem': 'TestPartItem',
                    '/Lotus/Upgrades/CosmeticEnhancers/Offensive/SecondaryDamageOnMeleeKill': 'Secondary Dexterity',
                    '/Lotus/Upgrades/CosmeticEnhancers/Zariman/PrimaryOnAbilityReloadSpeed': 'Fractalized Reset',
                    '/Lotus/Upgrades/CosmeticEnhancers/Zariman/SecondaryOnOvershieldCritChance': 'Cascadia Overcharge',
                    '/Lotus/Upgrades/CosmeticEnhancers/Offensive/SecondaryDamageOnHeatProc': 'Cascadia Flare',
                    '/Lotus/Types/Gameplay/InfestedMicroplanet/EncounterObjects/TestPartItem': 'TestPartItem',
                    '/Lotus/Types/Game/ShipScenes/PrimeLisetFiligreeScene': 'Filigree Prime',
                    '/Lotus/Weapons/SolarisUnited/Primary/LotusModularPrimary': 'Kitgun',
@@ -403,15 +470,21 @@
     parser['/Lotus/Types/Items/Research/DojoColors/GenericDojoColorPigment'] = 'Dojo Color Pigment'
 
     parser.update(parser_base)
 
     return parser
 
 
-def gen_type_dict(manifest_dict: dict, parser: dict):
+def gen_type_dict(manifest_dict: dict, parser: dict) -> dict:
+    """
+    Generates the type dictionary from the manifest dictionary
+    :param manifest_dict: the public manifest dictionary from warframe.com
+    :param parser: the parser dictionary
+    :return: the type dictionary
+    """
     type_dict = {'Relics': set(),
                  'Arcanes': set(),
                  'Mods': set(),
                  'Avionics': set(),
                  'Warframes': set(),
                  'PrimeWarframes': set(),
                  'WarframeParts': set(),
@@ -495,30 +568,28 @@
                  '/Lotus/Types/Items/MiscItems/FocusLens': 'FocusLens',
                  '/Lotus/Types/Items/MiscItems/ShipComponentItem': 'ShipComponents',
                  '/Lotus/Types/Items/ShipDecos/ShipDecoItem': 'Decorations',
                  '/Lotus/Types/Items/ShipDecos/ChildDrawingBase': 'Decorations',
                  '/Lotus/Types/Items/ShipDecos/InstrumentDecoItem': 'Decorations',
                  '/Lotus/Types/Items/ShipDecos/BaseFishTrophy': 'Decorations',
                  '/Lotus/Types/Items/ShipDecos/LotusShawzinPlayableBase': 'Decorations',
-                 '/Lotus/Types/Items/ShipDecos/BaseFishTrophy': 'Decorations',
                  '/Lotus/Types/Items/ShipDecos/Vignettes/Enemies/ShipDecoItem': 'Decorations',
                  '/Lotus/Types/Items/ShipDecos/Plushies/PlushyThumper': 'Decorations',
                  '/Lotus/Types/Items/Research/SampleBase': 'Misc',
                  '/Lotus/Types/Items/RailjackMiscItems/BaseRailjackItem': 'Misc',
                  '/Lotus/Types/Items/Plants/MiscItems/PlantItem': 'Plants',
                  '/Lotus/Types/Items/Gems/GemItem': 'Gems',
                  '/Lotus/Types/Items/FusionTreasures/FusionOrnament': 'AyatanStars',
                  '/Lotus/Types/Items/FusionTreasure': 'AyatanSculptures',
                  '/Lotus/Types/Items/Fish/Solaris/SolarisWarmRareFishAItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Solaris/RareFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Solaris/SolarisCoolUncommonFishAItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Solaris/UncommonFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Solaris/SolarisCoolCommonFishAItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Solaris/OrokinCoolRareFishAItem': 'Fish',
-                 '/Lotus/Types/Items/Fish/Solaris/RareFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Solaris/OrokinBothRareFishAItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Solaris/SolarisBothCommonFishAItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Solaris/OrokinBothLegendaryFishAItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Solaris/LegendaryFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Solaris/CorpusWarmUncommonFishAItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Solaris/CorpusWarmCommonFishBItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Solaris/CorpusWarmCommonFishAItem': 'Fish',
@@ -526,33 +597,29 @@
                  '/Lotus/Types/Items/Fish/Solaris/CorpusCoolCommonFishAItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Solaris/CorpusBothUncommonFishAItem': 'Fish',
                  '/Lotus/Types/Items/Fish/FishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/FishPartItem': 'Misc',
                  '/Lotus/Types/Items/Fish/Eidolon/NightRareFishBItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/RareFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/NightRareFishAItem': 'Fish',
-                 '/Lotus/Types/Items/Fish/Eidolon/RareFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/NightLegendaryFishAItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/LegendaryFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/DayUncommonFishBItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/UncommonFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/DayUncommonFishAItem': 'Fish',
-                 '/Lotus/Types/Items/Fish/Eidolon/UncommonFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/DayCommonFishCItem': 'Fish',
-                 '/Lotus/Types/Items/Fish/Eidolon/CommonFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/DayCommonFishBItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/CommonFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/DayCommonFishAItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/BothUncommonFishBItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/BothUncommonFishAItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/BothRareFishAItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/BothCommonFishBItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Eidolon/BothCommonFishAItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Deimos/OrokinUncommonAFishItem': 'Fish',
-                 '/Lotus/Types/Items/Fish/Deimos/UncommonFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Deimos/OrokinRareAFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Deimos/OrokinLegendaryAFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Deimos/LegendaryFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Deimos/InfestedUncommonAFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Deimos/UncommonFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Deimos/InfestedRareAFishItem': 'Fish',
                  '/Lotus/Types/Items/Fish/Deimos/CommonFishItem': 'Fish',
```

### Comparing `market-engine-0.0.9/setup.py` & `market-engine-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='market-engine',
-    version='0.0.9',
+    version='0.1.0',
     description='Engine for easily getting the orders, statistics, and other stats from warframe.market.',
     author='Jacob McBride',
     author_email='jake55111@gmail.com',
     packages=find_packages(),
     install_requires=[
         'aiohttp~=3.8.4',
         'discord~=2.2.2',
@@ -17,9 +17,10 @@
         'PyMySQL~=1.0.3',
         'fuzzywuzzy~=0.18.0',
         'pytz~=2023.3',
         'python-Levenshtein~=0.21.0',
         'beautifulsoup4~=4.12.2',
         'Markdown~=3.4.3',
         'cryptography~=40.0.2',
+        'tenacity~=8.2.2'
     ],
 )
```

