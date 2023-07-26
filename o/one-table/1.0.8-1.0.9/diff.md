# Comparing `tmp/one_table-1.0.8-py3-none-any.whl.zip` & `tmp/one_table-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3557 bytes, number of entries: 7
--rw-r--r--  2.0 unx     8059 b- defN 21-Dec-28 19:51 one_table/Table.py
+Zip file size: 3591 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     8363 b- defN 21-Dec-29 16:26 one_table/Table.py
 -rw-r--r--  2.0 unx      344 b- defN 21-Dec-13 04:40 one_table/Utils.py
 -rw-r--r--  2.0 unx      123 b- defN 21-Dec-13 04:38 one_table/__init__.py
--rw-r--r--  2.0 unx      590 b- defN 21-Dec-28 19:54 one_table-1.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Dec-28 19:54 one_table-1.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 21-Dec-28 19:54 one_table-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      531 b- defN 21-Dec-28 19:54 one_table-1.0.8.dist-info/RECORD
-7 files, 9749 bytes uncompressed, 2617 bytes compressed:  73.2%
+-rw-r--r--  2.0 unx      590 b- defN 21-Dec-29 16:27 one_table-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Dec-29 16:27 one_table-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 21-Dec-29 16:27 one_table-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      531 b- defN 21-Dec-29 16:27 one_table-1.0.9.dist-info/RECORD
+7 files, 10053 bytes uncompressed, 2651 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: one_table/Utils.py
 Comment: 
 
 Filename: one_table/__init__.py
 Comment: 
 
-Filename: one_table-1.0.8.dist-info/METADATA
+Filename: one_table-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: one_table-1.0.8.dist-info/WHEEL
+Filename: one_table-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: one_table-1.0.8.dist-info/top_level.txt
+Filename: one_table-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: one_table-1.0.8.dist-info/RECORD
+Filename: one_table-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## one_table/Table.py

```diff
@@ -7,15 +7,15 @@
 from one_table.Utils import get_iso_8601_date
 
 
 class Table(object):
     def __init__(self, params: dict):
         if 'name' not in params:
             raise Exception('Missing name property')
-
+        self.debug = params.get('debug', False)
         self.table_name = params['name']
         self.schema = params['schema']
         self.models = params['schema']['models']
         self.client = params['client'].Table(params['name'])
         self.pk_key = self.schema['indexes']['primary']['hash']
         self.sk_key = self.schema['indexes']['primary']['sort']
 
@@ -84,14 +84,16 @@
                 'UpdateExpression': 'set {}'.format(', '.join(update_expression)),
                 'ReturnValues': 'ALL_NEW',
                 'Key': {
                     'pk': pk_key_parsed,
                     'sk': sk_key_parsed
                 }
             }
+            if self.debug:
+                print(request)
             response = self.client.update_item(**request)
             # _schema["createdAt"] = ""
             # _schema["updateAt"] = ""
             if 'Attributes' in response:
                 return {k: v for k, v in response['Attributes'].items() if k in _schema.keys()}
             return response
         else:
@@ -115,14 +117,16 @@
 
             },
             'FilterExpression': '#_2 = :_2',
             'KeyConditionExpression': '#n0 = :v0 and begins_with(#n1, :v1)',
         }
         _schema["createdAt"] = ""
         _schema["updatedAt"] = ""
+        if self.debug:
+            print(request)
         response = self.client.query(**request)
         if len(response['Items']) > 0:
             return {k: v for k, v in response['Items'][0].items() if k in _schema.keys()}
 
         return response['Items']
 
     def find(self, model, key, value, limit=100, next_key=None):
@@ -150,14 +154,16 @@
             "ScanIndexForward": True,
             "Limit": limit,
         }
         if next_key:
             request['ExclusiveStartKey'] = next_key
         _schema["createdAt"] = ""
         _schema["updatedAt"] = ""
+        if self.debug:
+            print(request)
         response = self.client.query(**request)
         if len(response['Items']) > 0:
             r = []
             for idx, item in enumerate(response['Items']):
                 r.append({k: v for k, v in item.items() if k in _schema.keys()})
             return r
 
@@ -174,15 +180,16 @@
             "ExpressionAttributeValues": {
                 ':val': Decimal(1)
             },
             'ReturnValues': 'ALL_NEW',
             "ExpressionAttributeNames": {
                 "#att": query["key"]
             }}
-
+        if self.debug:
+            print(request)
         response = self.client.update_item(**request)
         return response.get('Attributes')
 
     def find_by_sort_key(self, model: str, query: dict, limit=100, next_key=None):
         _schema = copy.deepcopy(self.models[model])
         del _schema[self.pk_key]
         del _schema[self.sk_key]
@@ -203,14 +210,16 @@
             "Limit": limit,
         }
         if next_key:
             request['ExclusiveStartKey'] = next_key
 
         _schema["createdAt"] = ""
         _schema["updatedAt"] = ""
+        if self.debug:
+            print(request)
         response = self.client.query(**request)
         if len(response['Items']) > 0:
             r = []
             for idx, item in enumerate(response['Items']):
                 r.append({k: v for k, v in item.items() if k in _schema.keys()})
             return r
```

## Comparing `one_table-1.0.8.dist-info/METADATA` & `one_table-1.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-table
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python dynamoDB one table
 Home-page: UNKNOWN
 Author: Gerswin Pineda
 Author-email: g3rswin@gmail.com
 License: UNKNOWN
 Keywords: python,dynamodb
 Platform: UNKNOWN
```

