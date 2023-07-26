# Comparing `tmp/EstymaApiWrapper-0.0.55.tar.gz` & `tmp/EstymaApiWrapper-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EstymaApiWrapper-0.0.55.tar", last modified: Wed Jul 26 11:40:02 2023, max compression
+gzip compressed data, was "EstymaApiWrapper-0.0.56.tar", last modified: Wed Jul 26 18:17:51 2023, max compression
```

## Comparing `EstymaApiWrapper-0.0.55.tar` & `EstymaApiWrapper-0.0.56.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 11:40:02.559762 EstymaApiWrapper-0.0.55/
--rw-rw-rw-   0        0        0        0 2023-07-26 11:34:52.000000 EstymaApiWrapper-0.0.55/LICENSE
--rw-rw-rw-   0        0        0      821 2023-07-26 11:40:02.560274 EstymaApiWrapper-0.0.55/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-07-26 11:34:52.000000 EstymaApiWrapper-0.0.55/README.md
--rw-rw-rw-   0        0        0      108 2023-07-26 11:34:52.000000 EstymaApiWrapper-0.0.55/pyproject.toml
--rw-rw-rw-   0        0        0      719 2023-07-26 11:40:02.563290 EstymaApiWrapper-0.0.55/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-07-26 11:34:52.000000 EstymaApiWrapper-0.0.55/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:40:02.515318 EstymaApiWrapper-0.0.55/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:40:02.537789 EstymaApiWrapper-0.0.55/src/EstymaApiWrapper/
--rw-rw-rw-   0        0        0      329 2023-07-26 11:34:52.000000 EstymaApiWrapper-0.0.55/src/EstymaApiWrapper/CustomErrors.py
--rw-rw-rw-   0        0        0    15893 2023-07-26 11:36:34.000000 EstymaApiWrapper-0.0.55/src/EstymaApiWrapper/EstymaApi.py
--rw-rw-rw-   0        0        0       32 2023-07-26 11:34:52.000000 EstymaApiWrapper-0.0.55/src/EstymaApiWrapper/__init__.py
--rw-rw-rw-   0        0        0     4267 2023-07-26 11:34:52.000000 EstymaApiWrapper-0.0.55/src/EstymaApiWrapper/api_translation_table.json
--rw-rw-rw-   0        0        0      292 2023-07-26 11:34:52.000000 EstymaApiWrapper-0.0.55/src/EstymaApiWrapper/languageTable.json
-drwxrwxrwx   0        0        0        0 2023-07-26 11:40:02.558309 EstymaApiWrapper-0.0.55/src/EstymaApiWrapper.egg-info/
--rw-rw-rw-   0        0        0      821 2023-07-26 11:40:02.000000 EstymaApiWrapper-0.0.55/src/EstymaApiWrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-07-26 11:40:02.000000 EstymaApiWrapper-0.0.55/src/EstymaApiWrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 11:40:02.000000 EstymaApiWrapper-0.0.55/src/EstymaApiWrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 11:40:02.000000 EstymaApiWrapper-0.0.55/src/EstymaApiWrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 18:17:51.045323 EstymaApiWrapper-0.0.56/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:55:30.000000 EstymaApiWrapper-0.0.56/LICENSE
+-rw-rw-rw-   0        0        0      821 2023-07-26 18:17:51.046322 EstymaApiWrapper-0.0.56/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-07-26 17:55:30.000000 EstymaApiWrapper-0.0.56/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-26 17:55:30.000000 EstymaApiWrapper-0.0.56/pyproject.toml
+-rw-rw-rw-   0        0        0      719 2023-07-26 18:17:51.051834 EstymaApiWrapper-0.0.56/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-07-26 17:55:30.000000 EstymaApiWrapper-0.0.56/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:17:51.016565 EstymaApiWrapper-0.0.56/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 18:17:51.029739 EstymaApiWrapper-0.0.56/src/EstymaApiWrapper/
+-rw-rw-rw-   0        0        0      329 2023-07-26 17:55:30.000000 EstymaApiWrapper-0.0.56/src/EstymaApiWrapper/CustomErrors.py
+-rw-rw-rw-   0        0        0    15930 2023-07-26 18:10:03.000000 EstymaApiWrapper-0.0.56/src/EstymaApiWrapper/EstymaApi.py
+-rw-rw-rw-   0        0        0       32 2023-07-26 17:55:30.000000 EstymaApiWrapper-0.0.56/src/EstymaApiWrapper/__init__.py
+-rw-rw-rw-   0        0        0     4267 2023-07-26 17:55:30.000000 EstymaApiWrapper-0.0.56/src/EstymaApiWrapper/api_translation_table.json
+-rw-rw-rw-   0        0        0      292 2023-07-26 17:55:30.000000 EstymaApiWrapper-0.0.56/src/EstymaApiWrapper/languageTable.json
+drwxrwxrwx   0        0        0        0 2023-07-26 18:17:51.044320 EstymaApiWrapper-0.0.56/src/EstymaApiWrapper.egg-info/
+-rw-rw-rw-   0        0        0      821 2023-07-26 18:17:50.000000 EstymaApiWrapper-0.0.56/src/EstymaApiWrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-07-26 18:17:51.000000 EstymaApiWrapper-0.0.56/src/EstymaApiWrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 18:17:50.000000 EstymaApiWrapper-0.0.56/src/EstymaApiWrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 18:17:50.000000 EstymaApiWrapper-0.0.56/src/EstymaApiWrapper.egg-info/top_level.txt
```

### Comparing `EstymaApiWrapper-0.0.55/PKG-INFO` & `EstymaApiWrapper-0.0.56/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EstymaApiWrapper
-Version: 0.0.55
+Version: 0.0.56
 Summary: Wrapper for the EstymaApi
 Home-page: https://github.com/Tabisch/EstymaApi
 Author: Tabisch
 Author-email: tobithieman@gmail.com
 Project-URL: Bug Tracker, https://github.com/Tabisch/EstymaApi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `EstymaApiWrapper-0.0.55/setup.cfg` & `EstymaApiWrapper-0.0.56/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2045 7374 796d 6141 7069 5772 6170   = EstymaApiWrap
 00000020: 7065 720d 0a76 6572 7369 6f6e 203d 2030  per..version = 0
-00000030: 2e30 2e35 350d 0a61 7574 686f 7220 3d20  .0.55..author = 
+00000030: 2e30 2e35 360d 0a61 7574 686f 7220 3d20  .0.56..author = 
 00000040: 5461 6269 7363 680d 0a61 7574 686f 725f  Tabisch..author_
 00000050: 656d 6169 6c20 3d20 746f 6269 7468 6965  email = tobithie
 00000060: 6d61 6e40 676d 6169 6c2e 636f 6d0d 0a64  man@gmail.com..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2057 7261  escription = Wra
 00000080: 7070 6572 2066 6f72 2074 6865 2045 7374  pper for the Est
 00000090: 796d 6141 7069 0d0a 6c6f 6e67 5f64 6573  ymaApi..long_des
 000000a0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
```

### Comparing `EstymaApiWrapper-0.0.55/src/EstymaApiWrapper/EstymaApi.py` & `EstymaApiWrapper-0.0.56/src/EstymaApiWrapper/EstymaApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,18 +114,20 @@
 
         raise Exception
 
     async def _logout(self):
         self._loggedIn = False
 
         try:
-            if(await self._makeRequest("get", self.logout_url.format(self.http_url)).status == 302):
+            if((await self._makeRequest("get", self.logout_url.format(self.http_url))).status == 302):
                 return
         except:
             return
+        
+        return
 
     async def _relog(self):
         try:
             await self._logout()
             await self._login()
             await self.switchLanguage(self._language)
         except:
@@ -134,21 +136,21 @@
     #fetch data for all devices
     async def _fetchDevicedatatask(self, deviceid):
         resp = await (await self._makeRequest("post", self.update_url.format(self.http_url), data=self.fetchDevicedataBody.format(deviceid))).json(content_type='text/html')
         resp["licznik_paliwa_sub1"] = int(str(resp["licznik_paliwa_sub1"])[:-1])
         resp["daystats_data"]["pierwszy_pomiar_paliwa"] = int(str(resp["daystats_data"]["pierwszy_pomiar_paliwa"])[:-1])
         resp["consumption_fuel_current_day"] = resp["licznik_paliwa_sub1"] - resp["daystats_data"]["pierwszy_pomiar_paliwa"]
         resp["online"]["diffSeconds"] = await self._calculateUpdateDiffSeconds(resp["online"]["diff"])
-        resp["staleData"] = await self._determineStaleData(resp["online"]["diffSeconds"])
+        resp["dataUpToDate"] = await self._determineDataUpToDate(resp["online"]["diffSeconds"])
         resp["device_id"] = deviceid
 
         return resp
     
-    async def _determineStaleData(self, diffSeconds: int):
-        if diffSeconds > self._staleDataThresholdSeconds:
+    async def _determineDataUpToDate(self, diffSeconds: int):
+        if diffSeconds < self._staleDataThresholdSeconds:
             return True
         else:
             return False
 
     async def _calculateUpdateDiffSeconds(self, diffString: str):
         seconds = 0
```

### Comparing `EstymaApiWrapper-0.0.55/src/EstymaApiWrapper/api_translation_table.json` & `EstymaApiWrapper-0.0.56/src/EstymaApiWrapper/api_translation_table.json`

 * *Files identical despite different names*

### Comparing `EstymaApiWrapper-0.0.55/src/EstymaApiWrapper.egg-info/PKG-INFO` & `EstymaApiWrapper-0.0.56/src/EstymaApiWrapper.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EstymaApiWrapper
-Version: 0.0.55
+Version: 0.0.56
 Summary: Wrapper for the EstymaApi
 Home-page: https://github.com/Tabisch/EstymaApi
 Author: Tabisch
 Author-email: tobithieman@gmail.com
 Project-URL: Bug Tracker, https://github.com/Tabisch/EstymaApi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

