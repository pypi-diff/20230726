# Comparing `tmp/fruitcraft-0.0.7.tar.gz` & `tmp/fruitcraft-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fruitcraft-0.0.7.tar", max compression
+gzip compressed data, was "fruitcraft-0.0.8.tar", max compression
```

## Comparing `fruitcraft-0.0.7.tar` & `fruitcraft-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/LICENSE
--rw-r--r--   0        0        0      128 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/README.md
--rw-r--r--   0        0        0      157 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/fruitcraft/__init__.py
--rw-r--r--   0        0        0    25421 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/fruitcraft/client.py
--rw-r--r--   0        0        0    24569 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/fruitcraft/f_types/__init__.py
--rw-r--r--   0        0        0   351313 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/fruitcraft/f_types/cards.py
--rw-r--r--   0        0        0     1317 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/fruitcraft/f_types/errors.py
--rw-r--r--   0        0        0     3985 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/fruitcraft/f_types/utils.py
--rw-r--r--   0        0        0      809 2023-07-26 17:09:09.102130 fruitcraft-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 fruitcraft-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-26 17:15:49.696553 fruitcraft-0.0.8/LICENSE
+-rw-r--r--   0        0        0      128 2023-07-26 17:15:49.696553 fruitcraft-0.0.8/README.md
+-rw-r--r--   0        0        0      157 2023-07-26 17:15:49.696553 fruitcraft-0.0.8/fruitcraft/__init__.py
+-rw-r--r--   0        0        0    25694 2023-07-26 17:15:49.696553 fruitcraft-0.0.8/fruitcraft/client.py
+-rw-r--r--   0        0        0    24569 2023-07-26 17:15:49.696553 fruitcraft-0.0.8/fruitcraft/f_types/__init__.py
+-rw-r--r--   0        0        0   351313 2023-07-26 17:15:49.700553 fruitcraft-0.0.8/fruitcraft/f_types/cards.py
+-rw-r--r--   0        0        0     1317 2023-07-26 17:15:49.700553 fruitcraft-0.0.8/fruitcraft/f_types/errors.py
+-rw-r--r--   0        0        0     3985 2023-07-26 17:15:49.700553 fruitcraft-0.0.8/fruitcraft/f_types/utils.py
+-rw-r--r--   0        0        0      809 2023-07-26 17:15:49.700553 fruitcraft-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 fruitcraft-0.0.8/PKG-INFO
```

### Comparing `fruitcraft-0.0.7/LICENSE` & `fruitcraft-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.7/fruitcraft/client.py` & `fruitcraft-0.0.8/fruitcraft/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,18 +153,24 @@
         
         player_potion = getattr(api_response.data, "player_potion", None)
         if player_potion != None and isinstance(player_potion, int):
             self.last_loaded_player.potion_number = player_potion
         
         return api_response.data
     
-    async def fill_potions(self, amount: int = 50) -> FillPotionResponse:
+    async def fill_potions(self, amount: int = None) -> FillPotionResponse:
         return await self.fill_potions_with_options(FillPotionRequest(amount=amount))
     
     async def fill_potions_with_options(self, opt: FillPotionRequest) -> FillPotionResponse:
+        if not opt.amount and self.last_loaded_player:
+            opt.amount = 50 - self.last_loaded_player.potion_number
+            
+            if not opt.amount:
+                return FillPotionResponse(potion_number=self.last_loaded_player.potion_number)
+        
         api_response: APIResponse = await self.send_and_parse(
             "player/fillpotion", opt, FillPotionResponse)
         
         fill_result = api_response.data
         if not isinstance(fill_result, FillPotionResponse):
             return None
```

### Comparing `fruitcraft-0.0.7/fruitcraft/f_types/__init__.py` & `fruitcraft-0.0.8/fruitcraft/f_types/__init__.py`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.7/fruitcraft/f_types/cards.py` & `fruitcraft-0.0.8/fruitcraft/f_types/cards.py`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.7/fruitcraft/f_types/errors.py` & `fruitcraft-0.0.8/fruitcraft/f_types/errors.py`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.7/fruitcraft/f_types/utils.py` & `fruitcraft-0.0.8/fruitcraft/f_types/utils.py`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.7/pyproject.toml` & `fruitcraft-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fruitcraft"
-version = "0.0.7"
+version = "0.0.8"
 description = "Full Python Wrapper for fruitcraft game API. By Mr.AW ."
 authors = ["Mr. AW <mrawfruitly@gmail.com>"]
 packages = [
     { include = "fruitcraft" }
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `fruitcraft-0.0.7/PKG-INFO` & `fruitcraft-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fruitcraft
-Version: 0.0.7
+Version: 0.0.8
 Summary: Full Python Wrapper for fruitcraft game API. By Mr.AW .
 Home-page: https://github.com/MrAwFruitly/FruitcraftClient-py
 Keywords: fruit,fruitcraft,fruit-craft,game-library
 Author: Mr. AW
 Author-email: mrawfruitly@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

