# Comparing `tmp/fruitcraft-0.0.8.tar.gz` & `tmp/fruitcraft-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fruitcraft-0.0.8.tar", max compression
+gzip compressed data, was "fruitcraft-0.0.9.tar", max compression
```

## Comparing `fruitcraft-0.0.8.tar` & `fruitcraft-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-07-26 17:15:49.696553 fruitcraft-0.0.8/LICENSE
--rw-r--r--   0        0        0      128 2023-07-26 17:15:49.696553 fruitcraft-0.0.8/README.md
--rw-r--r--   0        0        0      157 2023-07-26 17:15:49.696553 fruitcraft-0.0.8/fruitcraft/__init__.py
--rw-r--r--   0        0        0    25694 2023-07-26 17:15:49.696553 fruitcraft-0.0.8/fruitcraft/client.py
--rw-r--r--   0        0        0    24569 2023-07-26 17:15:49.696553 fruitcraft-0.0.8/fruitcraft/f_types/__init__.py
--rw-r--r--   0        0        0   351313 2023-07-26 17:15:49.700553 fruitcraft-0.0.8/fruitcraft/f_types/cards.py
--rw-r--r--   0        0        0     1317 2023-07-26 17:15:49.700553 fruitcraft-0.0.8/fruitcraft/f_types/errors.py
--rw-r--r--   0        0        0     3985 2023-07-26 17:15:49.700553 fruitcraft-0.0.8/fruitcraft/f_types/utils.py
--rw-r--r--   0        0        0      809 2023-07-26 17:15:49.700553 fruitcraft-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 fruitcraft-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-26 19:35:39.641113 fruitcraft-0.0.9/LICENSE
+-rw-r--r--   0        0        0      128 2023-07-26 19:35:39.641113 fruitcraft-0.0.9/README.md
+-rw-r--r--   0        0        0      157 2023-07-26 19:35:39.641113 fruitcraft-0.0.9/fruitcraft/__init__.py
+-rw-r--r--   0        0        0    25806 2023-07-26 19:35:39.641113 fruitcraft-0.0.9/fruitcraft/client.py
+-rw-r--r--   0        0        0    24569 2023-07-26 19:35:39.641113 fruitcraft-0.0.9/fruitcraft/f_types/__init__.py
+-rw-r--r--   0        0        0   351313 2023-07-26 19:35:39.641113 fruitcraft-0.0.9/fruitcraft/f_types/cards.py
+-rw-r--r--   0        0        0     1317 2023-07-26 19:35:39.641113 fruitcraft-0.0.9/fruitcraft/f_types/errors.py
+-rw-r--r--   0        0        0     3985 2023-07-26 19:35:39.641113 fruitcraft-0.0.9/fruitcraft/f_types/utils.py
+-rw-r--r--   0        0        0      809 2023-07-26 19:35:39.645113 fruitcraft-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 fruitcraft-0.0.9/PKG-INFO
```

### Comparing `fruitcraft-0.0.8/LICENSE` & `fruitcraft-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.8/fruitcraft/client.py` & `fruitcraft-0.0.9/fruitcraft/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -660,14 +660,17 @@
         if the_pass != "" and the_pass != "none" and the_pass != "null":
             headers['Cookie'] = f"\u0046\u0052\u0055\u0049\u0054\u0050\u0041\u0053\u0053\u0050\u004f\u0052\u0054={the_pass};"
 
         response = await self.http_client.post(f"{self._default_url}/{path}", data=data_value, headers=headers)
         response.raise_for_status()
         return response.content
         
-
+    async def aclose(self):
+        try:
+            return await self.http_client.aclose()
+        except: pass
     
     @staticmethod
     def generate_passport() -> str:
         return ''.join(random.choices("abcdef0123456789", k=_MAX_PASSPORT_LENGTH))
```

### Comparing `fruitcraft-0.0.8/fruitcraft/f_types/__init__.py` & `fruitcraft-0.0.9/fruitcraft/f_types/__init__.py`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.8/fruitcraft/f_types/cards.py` & `fruitcraft-0.0.9/fruitcraft/f_types/cards.py`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.8/fruitcraft/f_types/errors.py` & `fruitcraft-0.0.9/fruitcraft/f_types/errors.py`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.8/fruitcraft/f_types/utils.py` & `fruitcraft-0.0.9/fruitcraft/f_types/utils.py`

 * *Files identical despite different names*

### Comparing `fruitcraft-0.0.8/pyproject.toml` & `fruitcraft-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fruitcraft"
-version = "0.0.8"
+version = "0.0.9"
 description = "Full Python Wrapper for fruitcraft game API. By Mr.AW ."
 authors = ["Mr. AW <mrawfruitly@gmail.com>"]
 packages = [
     { include = "fruitcraft" }
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `fruitcraft-0.0.8/PKG-INFO` & `fruitcraft-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fruitcraft
-Version: 0.0.8
+Version: 0.0.9
 Summary: Full Python Wrapper for fruitcraft game API. By Mr.AW .
 Home-page: https://github.com/MrAwFruitly/FruitcraftClient-py
 Keywords: fruit,fruitcraft,fruit-craft,game-library
 Author: Mr. AW
 Author-email: mrawfruitly@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

