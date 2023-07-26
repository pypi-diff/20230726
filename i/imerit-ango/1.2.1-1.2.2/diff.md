# Comparing `tmp/imerit_ango-1.2.1-py3-none-any.whl.zip` & `tmp/imerit_ango-1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9822 bytes, number of entries: 11
+Zip file size: 9819 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 08:52 imerit_ango/__init__.py
 -rw-r--r--  2.0 unx     1304 b- defN 23-Jul-10 08:52 imerit_ango/plugin_logger.py
--rw-r--r--  2.0 unx     6966 b- defN 23-Jul-17 15:46 imerit_ango/plugins.py
+-rw-r--r--  2.0 unx     6952 b- defN 23-Jul-21 11:09 imerit_ango/plugins.py
 -rw-r--r--  2.0 unx    16630 b- defN 23-Jul-17 15:49 imerit_ango/sdk.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-10 08:52 imerit_ango/models/__init__.py
 -rw-r--r--  2.0 unx       93 b- defN 23-Jul-10 08:52 imerit_ango/models/enums.py
 -rw-r--r--  2.0 unx     5452 b- defN 23-Jul-10 08:52 imerit_ango/models/label_category.py
--rw-r--r--  2.0 unx     1940 b- defN 23-Jul-17 15:52 imerit_ango-1.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 15:52 imerit_ango-1.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-17 15:52 imerit_ango-1.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      890 b- defN 23-Jul-17 15:52 imerit_ango-1.2.1.dist-info/RECORD
-11 files, 33379 bytes uncompressed, 8308 bytes compressed:  75.1%
+-rw-r--r--  2.0 unx     1940 b- defN 23-Jul-21 11:16 imerit_ango-1.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-21 11:16 imerit_ango-1.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-21 11:16 imerit_ango-1.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      890 b- defN 23-Jul-21 11:16 imerit_ango-1.2.2.dist-info/RECORD
+11 files, 33365 bytes uncompressed, 8305 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: imerit_ango/models/enums.py
 Comment: 
 
 Filename: imerit_ango/models/label_category.py
 Comment: 
 
-Filename: imerit_ango-1.2.1.dist-info/METADATA
+Filename: imerit_ango-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: imerit_ango-1.2.1.dist-info/WHEEL
+Filename: imerit_ango-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: imerit_ango-1.2.1.dist-info/top_level.txt
+Filename: imerit_ango-1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: imerit_ango-1.2.1.dist-info/RECORD
+Filename: imerit_ango-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## imerit_ango/plugins.py

```diff
@@ -148,15 +148,15 @@
         while True:
             data = self.queue.get()
             data["batches"] = data.get('tags', [])
             api_key = data.get('apiKey')
             task_id = data.get('taskId')
             sdk = SDK(api_key=api_key, host=self.host)
             answer = self.callback(**data)
-            sdk._annotate(task_id, answer.get("answer"))
+            sdk._annotate(task_id, answer)
 
     def on_plugin(self, data):
         workflow = data.get('workflow')
         if not workflow:
             return super().on_plugin(data)
         self.queue.put(data)
```

## Comparing `imerit_ango-1.2.1.dist-info/METADATA` & `imerit_ango-1.2.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imerit-ango
-Version: 1.2.1
+Version: 1.2.2
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: imerit_ango,ango-hub,imerit_ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

## Comparing `imerit_ango-1.2.1.dist-info/RECORD` & `imerit_ango-1.2.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 imerit_ango/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 imerit_ango/plugin_logger.py,sha256=kE3Bv8wqzXJzXHSxyZb7AdoTW0QeytZc137GDqcFsSI,1304
-imerit_ango/plugins.py,sha256=x6wY54iLDCLkgxapRcZ5efLET4LMR8cLnpmfCktBFy4,6966
+imerit_ango/plugins.py,sha256=pdXqIaulhAfQy9-caq6JhmA_qcZhXAFZBgf8C_DhSto,6952
 imerit_ango/sdk.py,sha256=ghc4OPRASM0h1tu8obq73e42hqGxO-lTZeVABmaKnfw,16630
 imerit_ango/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 imerit_ango/models/enums.py,sha256=vy38MqYeZkiRop8viSLmua-Mj0soMfBnjILTSOr8uSk,93
 imerit_ango/models/label_category.py,sha256=c46Lve-vV1NoHi5-kk8D0BO8pYSS177d4sNYeA19CZQ,5452
-imerit_ango-1.2.1.dist-info/METADATA,sha256=iVOLdmjz12lDWk120VpKxFIc7JWltFIKLWkLu1eBhvk,1940
-imerit_ango-1.2.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-imerit_ango-1.2.1.dist-info/top_level.txt,sha256=rL30Gcrxa2AgOWg8EXn6b4NzT5STPtJ20PSJPK9IgH0,12
-imerit_ango-1.2.1.dist-info/RECORD,,
+imerit_ango-1.2.2.dist-info/METADATA,sha256=jVesuPyd7iYzRlvSAOhmIGMXPRNpZ_88WA9eLP5dtFQ,1940
+imerit_ango-1.2.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+imerit_ango-1.2.2.dist-info/top_level.txt,sha256=rL30Gcrxa2AgOWg8EXn6b4NzT5STPtJ20PSJPK9IgH0,12
+imerit_ango-1.2.2.dist-info/RECORD,,
```

