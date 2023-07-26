# Comparing `tmp/qrwr-0.0.3-py3-none-any.whl.zip` & `tmp/qrwr-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3798 bytes, number of entries: 6
+Zip file size: 3805 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Oct-04 04:45 rfid_web_reader/__init__.py
--rw-rw-rw-  2.0 fat     7842 b- defN 22-Oct-06 09:20 rfid_web_reader/main.py
--rw-rw-rw-  2.0 fat      107 b- defN 22-Oct-06 09:21 qrwr-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Oct-06 09:21 qrwr-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 22-Oct-06 09:21 qrwr-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      446 b- defN 22-Oct-06 09:21 qrwr-0.0.3.dist-info/RECORD
-6 files, 8503 bytes uncompressed, 2988 bytes compressed:  64.9%
+-rw-rw-rw-  2.0 fat     7856 b- defN 22-Oct-12 09:06 rfid_web_reader/main.py
+-rw-rw-rw-  2.0 fat      107 b- defN 22-Oct-12 09:07 qrwr-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-Oct-12 09:07 qrwr-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 22-Oct-12 09:07 qrwr-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      446 b- defN 22-Oct-12 09:07 qrwr-0.0.4.dist-info/RECORD
+6 files, 8517 bytes uncompressed, 2995 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: rfid_web_reader/__init__.py
 Comment: 
 
 Filename: rfid_web_reader/main.py
 Comment: 
 
-Filename: qrwr-0.0.3.dist-info/METADATA
+Filename: qrwr-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: qrwr-0.0.3.dist-info/WHEEL
+Filename: qrwr-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: qrwr-0.0.3.dist-info/top_level.txt
+Filename: qrwr-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: qrwr-0.0.3.dist-info/RECORD
+Filename: qrwr-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rfid_web_reader/main.py

```diff
@@ -58,15 +58,16 @@
                 mark_ant = mark['ant']
                 if rfid_list[mark_ant]['EPC'] is None:
                     rf_id = mark['EPC']
                     rf_time = mark['time']
                     rfid_list[mark_ant]['EPC'] = rf_id
                     rfid_list[mark_ant]['time'] = rf_time
         except json.decoder.JSONDecodeError:
-            return rfid_list
+            pass
+        return rfid_list
 
 
     def start_reading(self):
         """
         Запрос начала пересылки событий считывания
         """
         x = requests.get(self.startListGet)
```

