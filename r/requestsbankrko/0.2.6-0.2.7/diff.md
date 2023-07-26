# Comparing `tmp/requestsbankrko-0.2.6.tar.gz` & `tmp/requestsbankrko-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requestsbankrko-0.2.6.tar", last modified: Tue Jul 25 06:08:29 2023, max compression
+gzip compressed data, was "requestsbankrko-0.2.7.tar", last modified: Wed Jul 26 08:48:49 2023, max compression
```

## Comparing `requestsbankrko-0.2.6.tar` & `requestsbankrko-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:08:29.312160 requestsbankrko-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-25 06:08:29.312160 requestsbankrko-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 06:08:29.312160 requestsbankrko-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:08:29.312160 requestsbankrko-0.2.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29322 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/src/bank_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/src/open_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:08:29.312160 requestsbankrko-0.2.6/src/requestsbankrko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-25 06:08:29.000000 requestsbankrko-0.2.6/src/requestsbankrko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-25 06:08:29.000000 requestsbankrko-0.2.6/src/requestsbankrko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:08:29.000000 requestsbankrko-0.2.6/src/requestsbankrko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-25 06:08:29.000000 requestsbankrko-0.2.6/src/requestsbankrko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 06:08:29.000000 requestsbankrko-0.2.6/src/requestsbankrko.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/src/zip_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:08:29.312160 requestsbankrko-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    57078 2023-07-25 06:08:16.000000 requestsbankrko-0.2.6/tests/test_bank_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:48:49.623319 requestsbankrko-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-26 08:48:36.000000 requestsbankrko-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-26 08:48:49.623319 requestsbankrko-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-26 08:48:36.000000 requestsbankrko-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-26 08:48:36.000000 requestsbankrko-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 08:48:49.623319 requestsbankrko-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:48:49.619319 requestsbankrko-0.2.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 08:48:36.000000 requestsbankrko-0.2.7/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29682 2023-07-26 08:48:36.000000 requestsbankrko-0.2.7/src/bank_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-26 08:48:36.000000 requestsbankrko-0.2.7/src/open_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:48:49.623319 requestsbankrko-0.2.7/src/requestsbankrko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-26 08:48:49.000000 requestsbankrko-0.2.7/src/requestsbankrko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-26 08:48:49.000000 requestsbankrko-0.2.7/src/requestsbankrko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 08:48:49.000000 requestsbankrko-0.2.7/src/requestsbankrko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-26 08:48:49.000000 requestsbankrko-0.2.7/src/requestsbankrko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 08:48:49.000000 requestsbankrko-0.2.7/src/requestsbankrko.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-26 08:48:36.000000 requestsbankrko-0.2.7/src/zip_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:48:49.623319 requestsbankrko-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    57359 2023-07-26 08:48:36.000000 requestsbankrko-0.2.7/tests/test_bank_methods.py
```

### Comparing `requestsbankrko-0.2.6/LICENSE` & `requestsbankrko-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.6/PKG-INFO` & `requestsbankrko-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.2.6
+Version: 0.2.7
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `requestsbankrko-0.2.6/pyproject.toml` & `requestsbankrko-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "requestsbankrko"
-version = "0.2.6"
+version = "0.2.7"
 description = "Гарантированно успешные web-запросы в Банки РКО"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = [ "requestsgarant>=0.0.7", "requests>=2.28", "jsoncustom>=0.0.2", "python-dotenv>=0.20.0",]
 [[project.authors]]
 name = "plp-kolyan"
```

### Comparing `requestsbankrko-0.2.6/src/bank_methods.py` & `requestsbankrko-0.2.7/src/bank_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -789,14 +789,26 @@
                 self.success = True
                 return inn_freedom
             elif self.response_json['status'] == 'ALREADY_EXISTS':
                 self.success = True
                 return inn_busy
 
 
+class PSBdtfmqueue(PSBParent):
+    def __init__(self, json_dict, test):
+        super().__init__(test)
+        self.json = json_dict
+        self.endpoint = f'/dfm/queue'
+        self.method = 'post'
+
+class PSBdtfmqueueid(PSBParent):
+    def __init__(self, params, test):
+        super().__init__(test)
+        self.params = params
+        self.method = 'get'
 
 
 
 class PSBLead(PSBParent):
 
 
     def __init__(self, json_dict, test=test):
```

### Comparing `requestsbankrko-0.2.6/src/open_methods.py` & `requestsbankrko-0.2.7/src/open_methods.py`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.6/src/requestsbankrko.egg-info/PKG-INFO` & `requestsbankrko-0.2.7/src/requestsbankrko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.2.6
+Version: 0.2.7
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `requestsbankrko-0.2.6/src/zip_functions.py` & `requestsbankrko-0.2.7/src/zip_functions.py`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.6/tests/test_bank_methods.py` & `requestsbankrko-0.2.7/tests/test_bank_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1179,25 +1179,26 @@
         obj = PSBToken(True)
 
         print(obj.get_rezult())
 
 
     def test_1(self):
         # {'code': 404, 'status': 'NOT_EXISTS', 'message': 'Создание заявки с данным ИНН разрешено'}
-        test = True
+        test = False
 
 
         inns = ["6382094062", "5007117617", "9705184265", "4705097662", "7734465242", "7813668661", "6320072051", "9719031558", "9723172375", "9704171432", "9725098952", "9725098960", "9725099000", "9725099032", "9703113607", "9727011971", "9726024618", "9704171601", "9728076523", "9727011925", "9727011932", "9728076587", "9701224453", "9701224478", "9728076594", "9727011989", "9729331977", "9725098977", "9705180415", "9726024590", "9727011940", "9727011957", "9728076604", "9729331952", "9727012012", "9725098945", "9726024583", "9728076611", "9718205890", "9703113597", "9727011918", "9706027434", "5009133639", "5262389062", "5032348840", "5029273458", "5075041684", "5018213256", "1684009258", "700006760", "5032348858", "5045069026", "3513003845", "1832165912", "1831207863", "5906175062", "1655489708", "1683010476", "1684009265", "1650418887", "5257212077", "1685008190", "3527024852", "5031148849", "9724109591", "5031148831", "5017130695", "5027311838", "1674003480", "1675001816", "6168118814", "1685008144", "5017130688", "5263150855", "5906175055", "1674003465", "1655489715", "5031148856", "1686020850", "1686020835", "1655489698", "5260487674", "3700000844", "5003154230", "5040182162", "3521007120", "3522004919", "5005072569", "1655489578", "1685008151", "5018213249", "5012108960", "3100009700", "9102286098", "1832165920", "5044137481", "1644101338", "1655489641", "1673003293", "9408000035"]
         for inn in inns[0:1]:
             json = {'inn': inn}
 
             obj_s = PSBScoring(json, test)
 
 
             print(obj_s.get_rezult())
+            print(obj_s.args_request)
             # print(obj_s.response_status_code)
             # print(obj_s.response.text)
             # print(obj_s.response.headers)
             time.sleep(1)
 
     def test_1_1(self):
         def write_token():
@@ -1388,8 +1389,18 @@
 
         # }
         print(KonturProspectiveSales(json, True).get_rezult())
 
 class DevelopTest(TestCase):
     def test_0(self):
         inn = '800009370'
-        print(mutation_inn(inn))
+        print(mutation_inn(inn))
+
+
+class PSBdtfmqueueTestCase(TestCase):
+    def test_0(self):
+        json_dict = {
+            "inns": ['665813932028']
+        }
+        obj = PSBdtfmqueue(json_dict, False).get_obj_rezult()
+        print(obj.response.text)
+        print()
```

