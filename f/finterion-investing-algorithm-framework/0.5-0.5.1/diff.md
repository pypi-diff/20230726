# Comparing `tmp/finterion_investing_algorithm_framework-0.5-py3-none-any.whl.zip` & `tmp/finterion_investing_algorithm_framework-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 10443 bytes, number of entries: 13
--rw-r--r--  2.0 unx      107 b- defN 23-Jul-26 09:37 finterion_investing_algorithm_framework/__init__.py
--rw-r--r--  2.0 unx     1402 b- defN 23-Jul-26 09:37 finterion_investing_algorithm_framework/create_app.py
--rw-r--r--  2.0 unx      197 b- defN 23-Jul-26 09:37 finterion_investing_algorithm_framework/exceptions.py
--rw-r--r--  2.0 unx     1948 b- defN 23-Jul-26 09:37 finterion_investing_algorithm_framework/market_service.py
--rw-r--r--  2.0 unx      102 b- defN 23-Jul-26 09:37 finterion_investing_algorithm_framework/configuration/__init__.py
--rw-r--r--  2.0 unx       93 b- defN 23-Jul-26 09:37 finterion_investing_algorithm_framework/configuration/constants.py
--rw-r--r--  2.0 unx      176 b- defN 23-Jul-26 09:37 finterion_investing_algorithm_framework/models/__init__.py
--rw-r--r--  2.0 unx      515 b- defN 23-Jul-26 09:37 finterion_investing_algorithm_framework/models/portfolio_configuration.py
--rw-r--r--  2.0 unx    11343 b- defN 23-Jul-26 09:38 finterion_investing_algorithm_framework-0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     3287 b- defN 23-Jul-26 09:38 finterion_investing_algorithm_framework-0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 09:38 finterion_investing_algorithm_framework-0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-Jul-26 09:38 finterion_investing_algorithm_framework-0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1462 b- defN 23-Jul-26 09:38 finterion_investing_algorithm_framework-0.5.dist-info/RECORD
-13 files, 20764 bytes uncompressed, 7863 bytes compressed:  62.1%
+Zip file size: 10459 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      107 b- defN 23-Jul-26 11:36 finterion_investing_algorithm_framework/__init__.py
+-rw-r--r--  2.0 unx     1401 b- defN 23-Jul-26 11:36 finterion_investing_algorithm_framework/create_app.py
+-rw-r--r--  2.0 unx      197 b- defN 23-Jul-26 11:36 finterion_investing_algorithm_framework/exceptions.py
+-rw-r--r--  2.0 unx     1948 b- defN 23-Jul-26 11:36 finterion_investing_algorithm_framework/market_service.py
+-rw-r--r--  2.0 unx      102 b- defN 23-Jul-26 11:36 finterion_investing_algorithm_framework/configuration/__init__.py
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-26 11:36 finterion_investing_algorithm_framework/configuration/constants.py
+-rw-r--r--  2.0 unx      176 b- defN 23-Jul-26 11:36 finterion_investing_algorithm_framework/models/__init__.py
+-rw-r--r--  2.0 unx      515 b- defN 23-Jul-26 11:36 finterion_investing_algorithm_framework/models/portfolio_configuration.py
+-rw-r--r--  2.0 unx    11343 b- defN 23-Jul-26 11:37 finterion_investing_algorithm_framework-0.5.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3289 b- defN 23-Jul-26 11:37 finterion_investing_algorithm_framework-0.5.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 11:37 finterion_investing_algorithm_framework-0.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-Jul-26 11:37 finterion_investing_algorithm_framework-0.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1472 b- defN 23-Jul-26 11:37 finterion_investing_algorithm_framework-0.5.1.dist-info/RECORD
+13 files, 20775 bytes uncompressed, 7859 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: finterion_investing_algorithm_framework/models/__init__.py
 Comment: 
 
 Filename: finterion_investing_algorithm_framework/models/portfolio_configuration.py
 Comment: 
 
-Filename: finterion_investing_algorithm_framework-0.5.dist-info/LICENSE
+Filename: finterion_investing_algorithm_framework-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: finterion_investing_algorithm_framework-0.5.dist-info/METADATA
+Filename: finterion_investing_algorithm_framework-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: finterion_investing_algorithm_framework-0.5.dist-info/WHEEL
+Filename: finterion_investing_algorithm_framework-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: finterion_investing_algorithm_framework-0.5.dist-info/top_level.txt
+Filename: finterion_investing_algorithm_framework-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: finterion_investing_algorithm_framework-0.5.dist-info/RECORD
+Filename: finterion_investing_algorithm_framework-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## finterion_investing_algorithm_framework/create_app.py

```diff
@@ -36,14 +36,14 @@
     app.container.market_service.override(
         FinterionMarketService(api_key=api_key, base_url=base_url)
     )
     app.add_portfolio_configuration(portfolio_configuration)
 
     class PingTask(Task):
         interval = 30
-        time_unit = TimeUnit.MINUTES
+        time_unit = TimeUnit.MINUTE
 
         def run(self, algorithm):
             client.ping()
 
     app.add_task(PingTask)
     return app
```

## Comparing `finterion_investing_algorithm_framework-0.5.dist-info/LICENSE` & `finterion_investing_algorithm_framework-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `finterion_investing_algorithm_framework-0.5.dist-info/METADATA` & `finterion_investing_algorithm_framework-0.5.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterion-investing-algorithm-framework
-Version: 0.5
+Version: 0.5.1
 Summary: Official Finterion plugin for the investing algorithm framework
 Home-page: https://github.com/finterion/finterion-investing-algorithm-framework.git
 Author: Finterion
 License: Apache License 2.0
 Keywords: Finterion,finterion,investing-algorithm,investing-algorithm-framework,INVESTING,BOT,ALGORITHM,FRAMEWORK,investing-bots,trading-bots
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

## Comparing `finterion_investing_algorithm_framework-0.5.dist-info/RECORD` & `finterion_investing_algorithm_framework-0.5.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 finterion_investing_algorithm_framework/__init__.py,sha256=u-srn87VlLUPUJHWR5hgMAHqw2BWtb1v0eH0tQ8M16w,107
-finterion_investing_algorithm_framework/create_app.py,sha256=sm5Zlgv1hrV5QlElyh7hFxmEc0Bam9Ru6RzTSpQ8WDs,1402
+finterion_investing_algorithm_framework/create_app.py,sha256=KkOJcaFllVIGzSG5wYN39rDLypKxrWvPKz-FUlhrIY8,1401
 finterion_investing_algorithm_framework/exceptions.py,sha256=KOaDjHQC7vNpKwYYNxJ2nuaJYceMmvExW3BLSzPSWJk,197
 finterion_investing_algorithm_framework/market_service.py,sha256=viv_eQNPaY00akFMN3-i76E3vBLRO8_35Bef4UXx3aA,1948
 finterion_investing_algorithm_framework/configuration/__init__.py,sha256=370OXcHya0GtGhrA59sIuznTYSn8xJy-dciCOSTsfl8,102
 finterion_investing_algorithm_framework/configuration/constants.py,sha256=bhabsdZ8omPvAZlQmdPGM70vHQHS2pcJm2olpkSEciU,93
 finterion_investing_algorithm_framework/models/__init__.py,sha256=96Cq_doBIVXfK9OJW3SnMTiXx9WPnd9LITlpT5vEFzw,176
 finterion_investing_algorithm_framework/models/portfolio_configuration.py,sha256=1QesgEDUDoPk50ZFsDZFpFNldP_PExoUgdhKHp3w908,515
-finterion_investing_algorithm_framework-0.5.dist-info/LICENSE,sha256=wbVEDvoZiMPHufRY3sLEffvAr7GH5hOIngHF8y4HFQg,11343
-finterion_investing_algorithm_framework-0.5.dist-info/METADATA,sha256=udC3kxGiK22nPPyIwpfcoIOtQZGk-uWy437ttRL-8FI,3287
-finterion_investing_algorithm_framework-0.5.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-finterion_investing_algorithm_framework-0.5.dist-info/top_level.txt,sha256=B97hJPQAFX_vRhcLE8uVZ6ac3a5ndS79p-O8-C2y-zw,40
-finterion_investing_algorithm_framework-0.5.dist-info/RECORD,,
+finterion_investing_algorithm_framework-0.5.1.dist-info/LICENSE,sha256=wbVEDvoZiMPHufRY3sLEffvAr7GH5hOIngHF8y4HFQg,11343
+finterion_investing_algorithm_framework-0.5.1.dist-info/METADATA,sha256=PIwrDBcF63pC3oRkmABMhkKDD6nLZvWkYiQwcLKXBKo,3289
+finterion_investing_algorithm_framework-0.5.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+finterion_investing_algorithm_framework-0.5.1.dist-info/top_level.txt,sha256=B97hJPQAFX_vRhcLE8uVZ6ac3a5ndS79p-O8-C2y-zw,40
+finterion_investing_algorithm_framework-0.5.1.dist-info/RECORD,,
```

