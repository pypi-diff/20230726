# Comparing `tmp/fruitcraft-0.0.6.tar.gz` & `tmp/fruitcraft-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fruitcraft-0.0.6.tar", max compression
+gzip compressed data, was "fruitcraft-0.0.7.tar", max compression
```

## Comparing `fruitcraft-0.0.6.tar` & `fruitcraft-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/LICENSE
--rw-r--r--   0        0        0      128 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/README.md
--rw-r--r--   0        0        0      157 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/fruitcraft/__init__.py
--rw-r--r--   0        0        0    23815 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/fruitcraft/client.py
--rw-r--r--   0        0        0    23696 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/fruitcraft/f_types/__init__.py
--rw-r--r--   0        0        0     1317 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/fruitcraft/f_types/errors.py
--rw-r--r--   0        0        0     3985 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/fruitcraft/f_types/utils.py
--rw-r--r--   0        0        0      809 2023-07-23 22:19:30.620277 fruitcraft-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 fruitcraft-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/LICENSE
+-rw-r--r--   0        0        0      128 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/README.md
+-rw-r--r--   0        0        0      157 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/fruitcraft/__init__.py
+-rw-r--r--   0        0        0    25421 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/fruitcraft/client.py
+-rw-r--r--   0        0        0    24569 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/fruitcraft/f_types/__init__.py
+-rw-r--r--   0        0        0   351313 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/fruitcraft/f_types/cards.py
+-rw-r--r--   0        0        0     1317 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/fruitcraft/f_types/errors.py
+-rw-r--r--   0        0        0     3985 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/fruitcraft/f_types/utils.py
+-rw-r--r--   0        0        0      809 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 fruitcraft-0.0.7/PKG-INFO
```

### Comparing `fruitcraft-0.0.6/LICENSE` & `fruitcraft-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.6/fruitcraft/client.py` & `fruitcraft-0.0.7/fruitcraft/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Optional, List
+from typing import (
+    Optional, List, Union
+)
 import string
 import random
 import time
 import httpx
 import asyncio
 from .f_types import (
     DScaffold,
@@ -49,14 +51,18 @@
     QuestResponse,
     SetCardForLiveBattleRequest,
     SetCardForLiveBattleResponse,
     TribeMembersRequest,
     TribeMembersResponse,
     TribeRankingsRequest,
     TribeRankingsResponse,
+    CollectGoldRequest,
+    CollectGoldResponse,
+    EvolveCardRequest,
+    EvolveCardResponse,
 )
 from .f_types.utils import (
     xor_decrypt,
     choose_strongest_atk_ids,
     choose_strongest_atk_id,
     hash_q_string,
 )
@@ -103,28 +109,56 @@
         
         self.mut = asyncio.Lock()
         self.http_client = httpx.AsyncClient()
         self.passport = passport
         if not self.logger:
             self.logger = logging.getLogger(__name__)
     
+    async def evolve_card(self, sacrifices: Union[CardsSelection, int]) -> EvolveCardResponse:
+        if isinstance(sacrifices, int):
+            sacrifices = new_int_array([sacrifices])
+        
+        return await self.evolve_card_with_options(EvolveCardRequest(
+            sacrifices=sacrifices,
+        ))
+    
+    async def evolve_card_with_options(self, opt: EvolveCardRequest) -> EvolveCardResponse:
+        api_response: APIResponse = await self.send_and_parse(
+            "cards/evolve", opt, EvolveCardResponse)
+        return api_response.data
+    
+    async def collect_gold(self) -> CollectGoldResponse:
+        return await self.collect_gold_with_options(CollectGoldRequest())
+    
+    async def collect_gold_with_options(self, opt: CollectGoldRequest) -> CollectGoldResponse:
+        opt.set_default_values()
+        
+        api_response: APIResponse = await self.send_and_parse(
+            "cards/collectgold", opt, CollectGoldResponse)
+        return api_response.data
+    
     async def get_player_info(self, player_id: int) -> GetPlayerInfoResponse:
         return await self.get_player_info_with_options(GetPlayerInfoRequest(player_id=player_id))
     
     async def get_player_info_with_options(self, opt: GetPlayerInfoRequest) -> GetPlayerInfoResponse:
         api_response: APIResponse = await self.send_and_parse(
             "player/getplayerinfo", opt, GetPlayerInfoResponse)
         return api_response.data
     
     async def potionize(self, hero_id: int, amount: int) -> PotionizeResponse:
         return await self.potionize_with_options(PotionizeRequest(potion=amount, hero_id=hero_id))
     
     async def potionize_with_options(self, opt: PotionizeRequest) -> PotionizeResponse:
         api_response: APIResponse = await self.send_and_parse(
             "cards/potionize", opt, PotionizeResponse)
+        
+        player_potion = getattr(api_response.data, "player_potion", None)
+        if player_potion != None and isinstance(player_potion, int):
+            self.last_loaded_player.potion_number = player_potion
+        
         return api_response.data
     
     async def fill_potions(self, amount: int = 50) -> FillPotionResponse:
         return await self.fill_potions_with_options(FillPotionRequest(amount=amount))
     
     async def fill_potions_with_options(self, opt: FillPotionRequest) -> FillPotionResponse:
         api_response: APIResponse = await self.send_and_parse(
@@ -488,21 +522,22 @@
     
     """
         Unsafe way of loading the player, please use the `load_player_with_options` method instead.
     """
     async def __load_player_with_options(self, opt: PlayerLoadRequest) -> PlayerLoadResponse:
         current_tries = 0
         while True:
-            api_response: APIResponse = await self.send_and_parse("player/load", opt, PlayerLoadResponse)
+            api_response: APIResponse = await self.send_and_parse(
+                "player/load", opt, PlayerLoadResponse, no_err_handling=True)
             if api_response.data != None and self.is_sim_err_code(getattr(api_response.data, "code", None)):
                 if current_tries > self._max_login_tries:
                     raise PlayerLoadException("Max login tries reached", api_response.data)
                 
                 sleep_amount: int = self._error_codes_to_sleep[getattr(api_response.data, "code")]
-                self.logger.warning("player/load: sleeping for %s seconds", sleep_amount)
+                self.logger.warning("player/load: sleeping for %i seconds", sleep_amount)
                 await asyncio.sleep(sleep_amount)
                 current_tries += 1
                 continue
             
             break
         
         load_response = api_response.data
@@ -550,15 +585,21 @@
         return FruitServerException(
             req_path=req_path, 
             error_code=error_code,
             message=self.cached_errors[str(error_code)],
             response=response
         )
 
-    async def send_and_parse(self, req_path: str, req_data: DScaffold, return_type: type = None) -> APIResponse:
+    async def send_and_parse(
+        self,
+        req_path: str,
+        req_data: DScaffold,
+        return_type: type = None,
+        no_err_handling: bool = False
+    ) -> APIResponse:
         serialized_data = req_data.get_serialized(self._serialize_key)
         
         parser_method = getattr(req_data, 'parse_response', None)
         if not return_type and not parser_method:
             return None
 
         target_pass = getattr(req_data, "_other_pass", None)
@@ -568,29 +609,33 @@
         respond_bytes = await self.invoke_request(path=req_path, data=serialized_data, the_pass=target_pass)
         if parser_method and inspect.ismethod(parser_method):
             return parser_method(respond_bytes)
         
         if self.log_before_resp_parsing:
             print(f"Response: {respond_bytes}")
         
+        the_err = None
         respond_decrypted = xor_decrypt(respond_bytes)
         j_value = json.loads(respond_decrypted)
         if not j_value or not j_value['status']:
             if j_value['data']['code'] != 0:
                 the_err = await self.get_error_by_code(
                     req_path=req_data,
                     error_code=j_value['data']['code'],
                     response=respond_bytes,
                 )
-                if isinstance(the_err, Exception):
+                
+                if not no_err_handling and isinstance(the_err, Exception):
                     raise the_err
-        
-            raise UnknownError(f"Unknown error occurred for {req_path}", respond_bytes)
+                    
+            if not no_err_handling:
+                raise UnknownError(f"Unknown error occurred for {req_path}", respond_bytes)
         
         api_response: APIResponse = APIResponse(j_value)
+        api_response.the_err = the_err
         response_data = j_value['data']
         if return_type:
             api_response.data = return_type(**response_data)
         
         return api_response
```

### Comparing `fruitcraft-0.0.6/fruitcraft/f_types/__init__.py` & `fruitcraft-0.0.7/fruitcraft/f_types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from pydantic import BaseModel
 from .utils import xor_encrypt
+from .cards import all_cards
 from typing import (
     Any, List, Dict, Optional
 )
 import time
 import random
 
 class IntArray(str):
     pass
 
+def get_all_cards() -> dict: return all_cards
+
 LeagueWinnerRanges = Dict[str, int]
 
 class LoadRequestDefaults:
 	DEFAULT_GAME_VERSION      = "1.9.10691"
 	DEFAULT_OS_TYPE           = 2
 	DEFAULT_OS_VERSION        = "7.1.2"
 	DEFAULT_PHONE_MODEL       = "google pixel 2"
@@ -36,15 +39,14 @@
     return IntArray(output)
     
 
 class Scaffold():
     def get_action(self) -> str:
         pass
     
-    
 
 class DScaffold(Scaffold, BaseModel):
     """
     DScaffold is a base class for all data classes that need to be sent to the server.
     """
     pass
     
@@ -55,23 +57,40 @@
         return xor_encrypt(self.json(), key=key)
 
 class APIResponse:
     status: Optional[bool] = False
     code: Optional[int] = 0
     data: DScaffold = None
     arguments: Optional[Any] = None
+    the_err = None
     
     def __init__(self, j_value: dict) -> None:
         if not isinstance(j_value, dict):
             raise TypeError("j_value must be a dict")
         
         self.status = j_value.get('status', False)
         self.arguments = j_value.get('arguments', None)
 
 
+class CollectGoldRequest(DScaffold):
+    client: Optional[str] = ""
+    
+    def set_default_values(self):
+        if not self.client:
+            self.client = LoadRequestDefaults.DEFAULT_CLIENT_VALUE
+
+class CollectGoldResponse(DScaffold):
+    collected_gold: Optional[int] = 0
+    player_gold: Optional[int] = 0
+    gold_collection_allowed: Optional[bool] = False
+    gold_collection_allowed_at: Optional[int] = 0
+    gold_collection_extraction: Optional[int] = 0
+    last_gold_collected_at: Optional[int] = 0
+    needs_captcha: Optional[bool] = False
+
 class CardInfo(DScaffold):
     type: Optional[int] = 0
     cards: Optional[Any] = None
     card_pack_type: int = int
 
 class AttackCardInfo(DScaffold):
     id: Optional[int] = 0
@@ -80,14 +99,21 @@
     base_card_id: Optional[int] = 0
     player_id: Optional[int] = 0
     internal_last_time_used: Optional[int] = 0
 
     def set_as_used(self):
         self.internal_last_time_used = time.time()
 
+class EvolveCardRequest(DScaffold):
+    sacrifices: Optional[IntArray] = None
+
+class EvolveCardResponse(DScaffold):
+    gold: Optional[int] = 0
+    card: Optional[AttackCardInfo] = None
+    hero_max_rarity: Optional[int] = None
 
 class QuestResponse(DScaffold):
     code: Optional[int] = 0
     arguments: Optional[List[Any]] = []
     outcome: Optional[bool] = False
     boss_mode: Optional[bool] = False
     gold: Optional[int] = 0
```

### Comparing `fruitcraft-0.0.6/fruitcraft/f_types/errors.py` & `fruitcraft-0.0.7/fruitcraft/f_types/errors.py`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.6/fruitcraft/f_types/utils.py` & `fruitcraft-0.0.7/fruitcraft/f_types/utils.py`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.6/pyproject.toml` & `fruitcraft-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fruitcraft"
-version = "0.0.6"
+version = "0.0.7"
 description = "Full Python Wrapper for fruitcraft game API. By Mr.AW ."
 authors = ["Mr. AW <mrawfruitly@gmail.com>"]
 packages = [
     { include = "fruitcraft" }
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `fruitcraft-0.0.6/PKG-INFO` & `fruitcraft-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fruitcraft
-Version: 0.0.6
+Version: 0.0.7
 Summary: Full Python Wrapper for fruitcraft game API. By Mr.AW .
 Home-page: https://github.com/MrAwFruitly/FruitcraftClient-py
 Keywords: fruit,fruitcraft,fruit-craft,game-library
 Author: Mr. AW
 Author-email: mrawfruitly@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

