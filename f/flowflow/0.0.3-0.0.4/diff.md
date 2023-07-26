# Comparing `tmp/flowflow-0.0.3-py3-none-any.whl.zip` & `tmp/flowflow-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,6 @@
-Zip file size: 2596 bytes, number of entries: 5
--rw-r--r--  2.0 unx     2506 b- defN 23-Jul-26 11:27 flowflow/__init__.py
--rw-r--r--  2.0 unx      570 b- defN 23-Jul-26 11:27 flowflow/example.py
--rw-r--r--  2.0 unx       81 b- defN 16-Jan-01 00:00 flowflow-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx      639 b- defN 16-Jan-01 00:00 flowflow-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx      360 b- defN 16-Jan-01 00:00 flowflow-0.0.3.dist-info/RECORD
-5 files, 4156 bytes uncompressed, 1928 bytes compressed:  53.6%
+Zip file size: 2090 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2506 b- defN 23-Jul-26 16:05 flowflow/__init__.py
+-rw-r--r--  2.0 unx       81 b- defN 16-Jan-01 00:00 flowflow-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx      646 b- defN 16-Jan-01 00:00 flowflow-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      285 b- defN 16-Jan-01 00:00 flowflow-0.0.4.dist-info/RECORD
+4 files, 3518 bytes uncompressed, 1536 bytes compressed:  56.3%
```

## zipnote {}

```diff
@@ -1,16 +1,13 @@
 Filename: flowflow/__init__.py
 Comment: 
 
-Filename: flowflow/example.py
+Filename: flowflow-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: flowflow-0.0.3.dist-info/WHEEL
+Filename: flowflow-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: flowflow-0.0.3.dist-info/METADATA
-Comment: 
-
-Filename: flowflow-0.0.3.dist-info/RECORD
+Filename: flowflow-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `flowflow-0.0.3.dist-info/METADATA` & `flowflow-0.0.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: flowflow
-Version: 0.0.3
-Summary: Flowflow.AI Client
+Version: 0.0.4
+Summary: Flowflow.AI Python Client
 Author-email: Mick Vermaat <support@flowflow.ai>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: API Docs, https://documentation.flowflow.ai/?python#api-reference
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flowflow Version: 0.0.3 Summary: Flowflow.AI Client
-Author-email: Mick Vermaat
+Metadata-Version: 2.1 Name: flowflow Version: 0.0.4 Summary: Flowflow.AI Python
+Client Author-email: Mick Vermaat
 flowflow.ai> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent Project-
 URL: API Docs, https://documentation.flowflow.ai/?python#api-reference Project-
 URL: Homepage, https://flowflow.ai # FlowFlow Python Client ## API
 Documentation https://documentation.flowflow.ai/?python#api-reference
```

