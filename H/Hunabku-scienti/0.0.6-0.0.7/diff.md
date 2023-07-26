# Comparing `tmp/Hunabku_scienti-0.0.6.tar.gz` & `tmp/Hunabku_scienti-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hunabku_scienti-0.0.6.tar", last modified: Mon Jun 26 15:56:30 2023, max compression
+gzip compressed data, was "Hunabku_scienti-0.0.7.tar", last modified: Wed Jul 26 18:39:10 2023, max compression
```

## Comparing `Hunabku_scienti-0.0.6.tar` & `Hunabku_scienti-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:56:30.136212 Hunabku_scienti-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:56:30.132212 Hunabku_scienti-0.0.6/Hunabku_scienti.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-26 15:56:30.000000 Hunabku_scienti-0.0.6/Hunabku_scienti.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-26 15:56:30.000000 Hunabku_scienti-0.0.6/Hunabku_scienti.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:56:30.000000 Hunabku_scienti-0.0.6/Hunabku_scienti.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 15:56:30.000000 Hunabku_scienti-0.0.6/Hunabku_scienti.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 15:56:30.000000 Hunabku_scienti-0.0.6/Hunabku_scienti.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-26 15:56:13.000000 Hunabku_scienti-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-26 15:56:13.000000 Hunabku_scienti-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-26 15:56:30.132212 Hunabku_scienti-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-26 15:56:13.000000 Hunabku_scienti-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:56:30.132212 Hunabku_scienti-0.0.6/hunabku_scienti/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:56:13.000000 Hunabku_scienti-0.0.6/hunabku_scienti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 15:56:13.000000 Hunabku_scienti-0.0.6/hunabku_scienti/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:56:30.132212 Hunabku_scienti-0.0.6/hunabku_scienti/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)    32902 2023-06-26 15:56:13.000000 Hunabku_scienti-0.0.6/hunabku_scienti/endpoints/Scienti.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:56:30.136212 Hunabku_scienti-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-26 15:56:13.000000 Hunabku_scienti-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:39:10.378165 Hunabku_scienti-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:39:10.378165 Hunabku_scienti-0.0.7/Hunabku_scienti.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-26 18:39:10.000000 Hunabku_scienti-0.0.7/Hunabku_scienti.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-26 18:39:10.000000 Hunabku_scienti-0.0.7/Hunabku_scienti.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:39:10.000000 Hunabku_scienti-0.0.7/Hunabku_scienti.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-26 18:39:10.000000 Hunabku_scienti-0.0.7/Hunabku_scienti.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 18:39:10.000000 Hunabku_scienti-0.0.7/Hunabku_scienti.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-26 18:38:55.000000 Hunabku_scienti-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 18:38:55.000000 Hunabku_scienti-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-26 18:39:10.378165 Hunabku_scienti-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-26 18:38:55.000000 Hunabku_scienti-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:39:10.378165 Hunabku_scienti-0.0.7/hunabku_scienti/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:38:55.000000 Hunabku_scienti-0.0.7/hunabku_scienti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-26 18:38:55.000000 Hunabku_scienti-0.0.7/hunabku_scienti/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:39:10.378165 Hunabku_scienti-0.0.7/hunabku_scienti/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)    48470 2023-07-26 18:38:55.000000 Hunabku_scienti-0.0.7/hunabku_scienti/endpoints/Scienti.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 18:39:10.378165 Hunabku_scienti-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-26 18:38:55.000000 Hunabku_scienti-0.0.7/setup.py
```

### Comparing `Hunabku_scienti-0.0.6/Hunabku_scienti.egg-info/PKG-INFO` & `Hunabku_scienti-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Hunabku-scienti
-Version: 0.0.6
+Name: Hunabku_scienti
+Version: 0.0.7
 Summary: Hunabku scienti plugin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Hunabku_scienti-0.0.6/LICENSE` & `Hunabku_scienti-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Hunabku_scienti-0.0.6/PKG-INFO` & `Hunabku_scienti-0.0.7/Hunabku_scienti.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Hunabku_scienti
-Version: 0.0.6
+Name: Hunabku-scienti
+Version: 0.0.7
 Summary: Hunabku scienti plugin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Hunabku_scienti-0.0.6/README.md` & `Hunabku_scienti-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `Hunabku_scienti-0.0.6/hunabku_scienti/endpoints/Scienti.py` & `Hunabku_scienti-0.0.7/hunabku_scienti/endpoints/Scienti.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,36 @@
 from hunabku.HunabkuBase import HunabkuPluginBase, endpoint
 from hunabku.Config import Config, Param
 from pymongo import MongoClient
+from elasticsearch import Elasticsearch, __version__ as es_version
+from elasticsearch_dsl import Search
 import sys
 import re
+import time
 
 
 class Scienti(HunabkuPluginBase):
     config = Config()
     config += Param(db_uri="mongodb://localhost:27017/",
                     doc="MongoDB string connection")
+    config += Param(es_uri="http://localhost:9200",
+                    doc="Elastic Search url")
+    config += Param(es_user="elastic",
+                    doc="Elastic Search user")
+    config += Param(es_pass="",
+                    doc="Elastic Search password")
 
     def __init__(self, hunabku):
         super().__init__(hunabku)
         self.dbclient = MongoClient(self.config.db_uri)
+        auth = (self.config.es_user, self.config.es_pass)
+        if es_version[0] < 8:
+            self.es = Elasticsearch(self.config.es_uri, http_auth=auth)
+        else:
+            self.es = Elasticsearch(self.config.es_uri, basic_auth=auth)
 
     def check_required_parameters(self, req_args):
         """
         Method to check mandatory parameters for the request.
         if a required parameter is not found, returns error code 400 (Bad Request)
         """
         model_year = req_args.get('model_year')
@@ -72,14 +86,34 @@
                 response=self.json.dumps(data),
                 status=400,
                 mimetype='application/json'
             )
             return response
         return None
 
+    def es_multi_match(self, keyword, fields, es_index):
+        """
+        Method to perform the elasticsearch multi_match query.
+        """
+        body = {
+            "query": {
+                "multi_match": {
+                    "query": keyword,
+                    "type": "phrase_prefix",
+                    "fields": fields
+                },
+            }
+        }
+        s = Search(using=self.es, index=es_index)
+        s = s.update_from_dict(body)
+        s = s.extra(track_total_hits=True)
+        s.execute()
+        data = [hit.to_dict() for hit in s.scan()]
+        return data
+
     @endpoint('/scienti/product', methods=['GET'])
     def scienti_product(self):
         """
         @api {get} /scienti/product Scienti prouduct endpoint
         @apiName product
         @apiGroup Scienti
         @apiDescription Allows to perform queries for products,
@@ -88,41 +122,52 @@
 
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} COD_RH  User primary key
         @apiParam {String} COD_PRODUCTO  Product key (require COD_RH)
         @apiParam {String} SGL_CATEGORIA  Category of the product
         @apiParam {String} model_year  Year of the scienti model, example: 2022
         @apiParam {String} institution Institution initials. supported example: udea, uec, unaula, univalle
+        @apiParam {String} search Allows to search text keywords in several fields of the product collection using elastic search.
+        @apiParam {String} group_id  Returns products for the given group id.
+
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
             # all the products for the user
             curl -i http://apis.colav.co/scienti/product?apikey=XXXX&model_year=2022&institution=udea&COD_RH=0000000639
             # An specific product
             curl -i http://apis.colav.co/scienti/product?apikey=XXXX&model_year=2022&institution=udea&COD_RH=0000000639&COD_PRODUCTO=24
             # An specific product category
-            curl -i http://apis.colav.co/scienti/product?apikey=XXXX&model_year=2022&institution=udea
+            curl -i http://apis.colav.co/scienti/product?apikey=XXXX&model_year=2022&institution=udea&SGL_CATEGORIA=ART-ART_A1
+            # Text search for a keyword using elastic search
+            curl -i http://apis.colav.co/scienti/product?apikey=XXXX&model_year=2022&institution=udea&search="machine learning"
+            # return products for the given group id
+            curl -i http://apis.colav.co/scienti/product?apikey=XXXX&model_year=2022&institution=udea&group_id=COL0008423
+
+
         """
 
         if self.valid_apikey():
             cod_rh = self.request.args.get('COD_RH')
             cod_prod = self.request.args.get('COD_PRODUCTO')
             sgl_cat = self.request.args.get('SGL_CATEGORIA')
             model_year = self.request.args.get('model_year')
             institution = self.request.args.get('institution')
+            keyword = self.request.args.get('search')
+            group_id = self.request.args.get('group_id')
 
             response = self.check_required_parameters(self.request.args)
             if response is not None:
                 return response
             response = self.check_parameters(
-                ['apikey', 'COD_RH', 'COD_PRODUCTO', 'SGL_CATEGORIA', 'model_year', 'institution'], self.request.args.keys())
+                ['apikey', 'COD_RH', 'COD_PRODUCTO', 'SGL_CATEGORIA', 'model_year', 'institution', 'search', 'group_id'], self.request.args.keys())
             if response is not None:
                 return response
 
             db_name = f'scienti_{institution}_{model_year}'
 
             response = self.check_db(db_name)
             if response is not None:
@@ -154,14 +199,69 @@
                         {'SGL_CATEGORIA': sgl_cat}, {"_id": 0}))
                     response = self.app.response_class(
                         response=self.json.dumps(data),
                         status=200,
                         mimetype='application/json'
                     )
                     return response
+                if keyword:
+                    es_index = f'scienti_{institution}_{model_year}_product'
+
+                    # not required extra fields for search, at least for product
+                    # article, audiovisual, book, book_chapter, event, journal, journal_others, music_sheet
+                    # oriented_thesis
+                    fields = ["TXT_NME_PROD",
+                              "TXT_RESUMEN_PROD",
+                              "TXT_OBSERV_PROD",
+                              "DSC_PROJETO",
+                              # campos application_sector (es recursivo a 3 niveles)
+                              # https://github.com/colav/KayPacha/blob/main/kaypacha/models/scienti/graph_schema_product.py#L636
+                              "details.application_sector.TXT_NME_SECTOR_APLIC",
+                              "details.application_sector.application_sector.TXT_NME_SECTOR_APLIC",
+                              "details.application_sector.application_sector.application_sector.TXT_NME_SECTOR_APLIC",
+                              # community
+                              "details.community.TXT_CARACTERIZACION",
+                              # course
+                              "details.course.TXT_FINALIDAD",
+                              # keywords
+                              "details.keywords.TXT_NME_PALABRA_CLAVE",
+                              # memory chapter
+                              "details.memory_chapter.TXT_NME_PONENCIA",
+                              "details.memory_chapter.TXT_NME_EVENTO",
+                              # prod_art
+                              "details.prod_art.prod_art_detail.TXT_NME_EVENTO",
+                              "details.prod_art.prod_art_detail.knowledge_area.TXT_NME_AREA_FULL",
+                              # technical
+                              "details.technical.TXT_NME_COMERCIAL",
+                              "details.technical.TXT_FINALIDAD"]
+
+                    # get the start time
+                    st = time.time()
+                    data = self.es_multi_match(keyword, fields, es_index)
+                    # get the end time
+                    et = time.time()
+                    # get the execution time
+                    elapsed_time = et - st
+                    print(f'Search for "{keyword}" in {es_index} Execution time:',
+                          elapsed_time, 'seconds')
+                    response = self.app.response_class(
+                        response=self.json.dumps(data),
+                        status=200,
+                        mimetype='application/json'
+                    )
+                    return response
+                if group_id:
+                    data = list(self.db["product"].find(
+                        {'group.COD_ID_GRUPO': group_id}, {"_id": 0}))
+                    response = self.app.response_class(
+                        response=self.json.dumps(data),
+                        status=200,
+                        mimetype='application/json'
+                    )
+                    return response
 
                 data = {
                     "error": "Bad Request", "message": "invalid parameters, please select the right combination of parameters."}
                 response = self.app.response_class(
                     response=self.json.dumps(data),
                     status=400,
                     mimetype='application/json'
@@ -191,41 +291,50 @@
 
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} COD_RH  User primary key
         @apiParam {String} COD_RED  network key (require COD_RH)
         @apiParam {String} SGL_CATEGORIA  category of the network
         @apiParam {String} model_year  year of the scienti model, example: 2022
         @apiParam {String} institution institution initials. supported example: udea, uec, unaula, univalle
+        @apiParam {String} search Allows to search text keywords in several fields of the network collection using elastic search.
+        @apiParam {String} group_id  Returns networks for the given group id.
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
             # all the networks for the user
             curl -i http://apis.colav.co/scienti/network?apikey=XXXX&model_year=2022&institution=udea&COD_RH=0000172057
             # An specific network
             curl -i http://apis.colav.co/scienti/network?apikey=XXXX&model_year=2022&institution=udea&COD_RH=0000172057&COD_RED=1
             # An specific network category
             curl -i http://apis.colav.co/scienti/network?apikey=XXXX&model_year=2022&institution=udea&SGL_CATEGORIA=RC-RC_A
+            # Text search for a keyword using elastic search
+            curl -i http://apis.colav.co/scienti/network?apikey=XXXX&model_year=2022&institution=udea&search="educación"
+            # return networks for the given group id
+            curl -i http://apis.colav.co/scienti/network?apikey=XXXX&model_year=2022&institution=udea&group_id=COL0053803
+
         """
 
         if self.valid_apikey():
             cod_rh = self.request.args.get('COD_RH')
             cod_red = self.request.args.get('COD_RED')
             sgl_cat = self.request.args.get('SGL_CATEGORIA')
             model_year = self.request.args.get('model_year')
             institution = self.request.args.get('institution')
+            keyword = self.request.args.get('search')
+            group_id = self.request.args.get('group_id')
 
             response = self.check_required_parameters(self.request.args)
             if response is not None:
                 return response
             response = self.check_parameters(
-                ['apikey', 'COD_RH', 'COD_RED', 'SGL_CATEGORIA', 'model_year', 'institution'], self.request.args.keys())
+                ['apikey', 'COD_RH', 'COD_RED', 'SGL_CATEGORIA', 'model_year', 'institution', 'search', 'group_id'], self.request.args.keys())
             if response is not None:
                 return response
 
             db_name = f'scienti_{institution}_{model_year}'
 
             response = self.check_db(db_name)
             if response is not None:
@@ -258,14 +367,66 @@
                         {'SGL_CATEGORIA': sgl_cat}, {"_id": 0}))
                     response = self.app.response_class(
                         response=self.json.dumps(data),
                         status=200,
                         mimetype='application/json'
                     )
                     return response
+                if keyword:
+                    es_index = f'scienti_{institution}_{model_year}_network'
+
+                    fields = ["TXT_NME_RED",
+                              "details.community.TXT_NME_COMUNIDAD",
+                              "details.community.TXT_CARACTERIZACION",
+                              "details.community.product.TXT_NME_PROD",
+                              "details.community.product.TXT_RESUMEN_PROD",
+                              "details.community.product.TXT_OBSERV_PROD",
+                              "details.community.product.DSC_PROJETO",
+                              "details.community.project.TXT_NME_PROYECTO",
+                              "details.community.project.TXT_OBSERV_PROYECTO",
+                              "details.community.project.TXT_RESUMEN_PROYECTO",
+                              "group.NME_GRUPO",
+                              "group.TXT_PLAN_TRABAJO",
+                              "group.TXT_ESTADO_ARTE",
+                              "group.TXT_OBJETIVOS",
+                              "group.TXT_PROD_DESTACADA",
+                              "group.TXT_RETOS",
+                              "group.TXT_VISION",
+                              "group.knowledge_area.TXT_NME_AREA",  # recursive level 0
+                              "group.knowledge_area.TXT_NME_AREA_FULL"
+                              "group.knowledge_area.knowledge_area.TXT_NME_AREA",  # level 1
+                              "group.knowledge_area.knowledge_area.TXT_NME_AREA_FULL"
+                              "group.knowledge_area.knowledge_area.knowledge_area.TXT_NME_AREA",  # level 3
+                              "group.knowledge_area.knowledge_area.knowledge_area.TXT_NME_AREA_FULL"
+                              ]
+
+                    # get the start time
+                    st = time.time()
+                    data = self.es_multi_match(keyword, fields, es_index)
+                    # get the end time
+                    et = time.time()
+                    # get the execution time
+                    elapsed_time = et - st
+                    print(f'Search for "{keyword}" Execution time:',
+                          elapsed_time, 'seconds')
+                    response = self.app.response_class(
+                        response=self.json.dumps(data),
+                        status=200,
+                        mimetype='application/json'
+                    )
+                    return response
+                if group_id:
+                    data = list(self.db["network"].find(
+                        {'group.COD_ID_GRUPO': group_id}, {"_id": 0}))
+                    response = self.app.response_class(
+                        response=self.json.dumps(data),
+                        status=200,
+                        mimetype='application/json'
+                    )
+                    return response
 
                 data = {
                     "error": "Bad Request", "message": "invalid parameters, please select the right combination of parameters"}
                 response = self.app.response_class(
                     response=self.json.dumps(data),
                     status=400,
                     mimetype='application/json'
@@ -296,41 +457,50 @@
 
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} COD_RH  User primary key
         @apiParam {String} COD_PROYECTO  project key (require COD_RH)
         @apiParam {String} SGL_CATEGORIA  category of the network
         @apiParam {String} model_year  year of the scienti model, example: 2022
         @apiParam {String} institution institution initials. supported example: udea, uec, unaula, univalle
+        @apiParam {String} search Allows to search text keywords in several fields of the project collection using elastic search.
+        @apiParam {String} group_id  Returns projects for the given group id.
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
             # all the projects for the user
             curl -i http://apis.colav.co/scienti/project?apikey=XXXX&model_year=2022&institution=udea&COD_RH=0000000930
             # An specific project
             curl -i http://apis.colav.co/scienti/project?apikey=XXXX&model_year=2022&institution=udea&COD_RH=0000000930&COD_PROYECTO=1
             # An specific project category
             curl -i http://apis.colav.co/scienti/project?apikey=XXXX&model_year=2022&institution=udea&SGL_CATEGORIA=PID-00
+            # Text search for a keyword using elastic search
+            curl -i http://apis.colav.co/scienti/project?apikey=XXXX&model_year=2022&institution=udea&search="machine learning"
+            # return projects for the given group id
+            curl -i http://apis.colav.co/scienti/project?apikey=XXXX&model_year=2022&institution=udea&group_id=COL0008423
+
         """
 
         if self.valid_apikey():
             cod_rh = self.request.args.get('COD_RH')
             cod_projecto = self.request.args.get('COD_PROYECTO')
             sgl_cat = self.request.args.get('SGL_CATEGORIA')
             model_year = self.request.args.get('model_year')
             institution = self.request.args.get('institution')
+            keyword = self.request.args.get('search')
+            group_id = self.request.args.get('group_id')
 
             response = self.check_required_parameters(self.request.args)
             if response is not None:
                 return response
             response = self.check_parameters(
-                ['apikey', 'COD_RH', 'COD_PROYECTO', 'SGL_CATEGORIA', 'model_year', 'institution'], self.request.args.keys())
+                ['apikey', 'COD_RH', 'COD_PROYECTO', 'SGL_CATEGORIA', 'model_year', 'institution', 'search', 'group_id'], self.request.args.keys())
             if response is not None:
                 return response
 
             db_name = f'scienti_{institution}_{model_year}'
 
             response = self.check_db(db_name)
             if response is not None:
@@ -362,14 +532,52 @@
                         {'SGL_CATEGORIA': sgl_cat}, {"_id": 0}))
                     response = self.app.response_class(
                         response=self.json.dumps(data),
                         status=200,
                         mimetype='application/json'
                     )
                     return response
+                if keyword:
+                    es_index = f'scienti_{institution}_{model_year}_project'
+
+                    # only required fields for search are product and community, at least for project.
+                    fields = ["TXT_NME_PROYECTO",
+                              "TXT_OBSERV_PROYECTO",
+                              "TXT_RESUMEN_PROYECTO",
+                              "details.product.TXT_NME_PROD",
+                              "details.product.TXT_RESUMEN_PROD",
+                              "details.product.TXT_OBSERV_PROD",
+                              "details.product.DSC_PROJETO",
+                              "details.community.TXT_NME_COMUNIDAD",
+                              "details.community.TXT_CARACTERIZACION"]
+                    # get the start time
+                    st = time.time()
+                    data = self.es_multi_match(keyword, fields, es_index)
+                    # get the end time
+                    et = time.time()
+                    # get the execution time
+                    elapsed_time = et - st
+                    print(f'Search for "{keyword}" Execution time:',
+                          elapsed_time, 'seconds')
+                    response = self.app.response_class(
+                        response=self.json.dumps(data),
+                        status=200,
+                        mimetype='application/json'
+                    )
+                    return response
+
+                if group_id:
+                    data = list(self.db["project"].find(
+                        {'group.COD_ID_GRUPO': group_id}, {"_id": 0}))
+                    response = self.app.response_class(
+                        response=self.json.dumps(data),
+                        status=200,
+                        mimetype='application/json'
+                    )
+                    return response
 
                 data = {
                     "error": "Bad Request", "message": "invalid parameters, please select the right combination of parameters"}
                 response = self.app.response_class(
                     response=self.json.dumps(data),
                     status=400,
                     mimetype='application/json'
@@ -400,40 +608,49 @@
 
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} COD_RH  User primary key
         @apiParam {String} COD_EVENTO  event key (require COD_RH)
         @apiParam {String} SGL_CATEGORIA  category of the network
         @apiParam {String} model_year  year of the scienti model, example: 2022
         @apiParam {String} institution institution initials. supported example: udea, uec, unaula, univalle
+        @apiParam {String} search Allows to search text keywords in several fields of the event collection using elastic search.
+        @apiParam {String} group_id  Returns events for the given group id.
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
             # all the events for the user
             curl -i http://apis.colav.co/scienti/event?apikey=XXXX&model_year=2022&institution=udea&COD_RH=0000000016
             # An specific event
             curl -i http://apis.colav.co/scienti/event?apikey=XXXX&model_year=2022&institution=udea&COD_RH=0000000016&COD_EVENTO=2
             # An specific event category
             curl -i http://apis.colav.co/scienti/event?apikey=XXXX&model_year=2022&institution=udea&SGL_CATEGORIA=EC-EC_B
+            # Text search for a keyword using elastic search
+            curl -i http://apis.colav.co/scienti/event?apikey=XXXX&model_year=2022&institution=udea&search="machine learning"
+            # return event for the given group id
+            curl -i http://apis.colav.co/scienti/event?apikey=XXXX&model_year=2022&institution=udea&group_id=COL0008423
+
         """
         if self.valid_apikey():
             cod_rh = self.request.args.get('COD_RH')
             cod_evento = self.request.args.get('COD_EVENTO')
             sgl_cat = self.request.args.get('SGL_CATEGORIA')
             model_year = self.request.args.get('model_year')
             institution = self.request.args.get('institution')
+            keyword = self.request.args.get('search')
+            group_id = self.request.args.get('group_id')
 
             response = self.check_required_parameters(self.request.args)
             if response is not None:
                 return response
             response = self.check_parameters(
-                ['apikey', 'COD_RH', 'COD_PROYECTO', 'COD_EVENTO', 'model_year', 'institution'], self.request.args.keys())
+                ['apikey', 'COD_RH', 'COD_PROYECTO', 'COD_EVENTO', 'model_year', 'institution', 'search', 'group_id'], self.request.args.keys())
             if response is not None:
                 return response
 
             db_name = f'scienti_{institution}_{model_year}'
 
             response = self.check_db(db_name)
             if response is not None:
@@ -465,14 +682,54 @@
                         {'SGL_CATEGORIA': sgl_cat}, {"_id": 0}))
                     response = self.app.response_class(
                         response=self.json.dumps(data),
                         status=200,
                         mimetype='application/json'
                     )
                     return response
+                if keyword:
+                    es_index = f'scienti_{institution}_{model_year}_event'
+
+                    fields = ["TXT_NME_EVENTO",
+                              "TXT_RESUMEN_EVENTO",
+                              "TXT_ACTIVIDADES",
+                              "project.TXT_NME_PROYECTO",
+                              "project.TXT_RESUMEN_PROYECTO",
+                              "details.product.TXT_NME_PROD",
+                              "details.product.TXT_RESUMEN_PROD",
+                              "details.product.TXT_OBSERV_PROD",
+                              "details.product.DSC_PROJETO",
+                              "details.keywords.TXT_NME_PALABRA_CLAVE",
+                              "details.application_sector.TXT_NME_SECTOR_APLIC",  # recursive 2 times
+                              "details.application_sector.application_sector.TXT_NME_SECTOR_APLIC",
+                              ]
+                    # get the start time
+                    st = time.time()
+                    data = self.es_multi_match(keyword, fields, es_index)
+                    # get the end time
+                    et = time.time()
+                    # get the execution time
+                    elapsed_time = et - st
+                    print(f'Search for "{keyword}" Execution time:',
+                          elapsed_time, 'seconds')
+                    response = self.app.response_class(
+                        response=self.json.dumps(data),
+                        status=200,
+                        mimetype='application/json'
+                    )
+                    return response
+                if group_id:
+                    data = list(self.db["event"].find(
+                        {'group.COD_ID_GRUPO': group_id}, {"_id": 0}))
+                    response = self.app.response_class(
+                        response=self.json.dumps(data),
+                        status=200,
+                        mimetype='application/json'
+                    )
+                    return response
 
                 data = {
                     "error": "Bad Request", "message": "invalid parameters, please select the right combination of parameters"}
                 response = self.app.response_class(
                     response=self.json.dumps(data),
                     status=400,
                     mimetype='application/json'
@@ -503,40 +760,44 @@
 
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} COD_RH  User primary key
         @apiParam {String} COD_PATENTE  patent key (require COD_RH)
         @apiParam {String} SGL_CATEGORIA  category of the network
         @apiParam {String} model_year  year of the scienti model, example: 2022
         @apiParam {String} institution institution initials. supported example: udea, uec, unaula, univalle
+        @apiParam {String} search Allows to search text keywords in several fields of the patent collection using elastic search.
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
             # all the patents for the user
             curl -i http://apis.colav.co/scienti/patent?apikey=XXXX&model_year=2022&institution=udea&COD_RH=0000204234
             # An specific patent
             curl -i http://apis.colav.co/scienti/patent?apikey=XXXX&model_year=2022&institution=udea&COD_RH=0000204234&COD_PATENTE=2
             # An specific patent category
             curl -i http://apis.colav.co/scienti/patent?apikey=XXXX&model_year=2022&institution=udea&SGL_CATEGORIA=PIV-00
+            # Text search for a keyword using elastic search
+            curl -i http://apis.colav.co/scienti/patent?apikey=XXXX&model_year=2022&institution=udea&search="process"
         """
         if self.valid_apikey():
             cod_rh = self.request.args.get('COD_RH')
             cod_patente = self.request.args.get('COD_PATENTE')
             sgl_cat = self.request.args.get('SGL_CATEGORIA')
             model_year = self.request.args.get('model_year')
             institution = self.request.args.get('institution')
+            keyword = self.request.args.get('search')
 
             response = self.check_required_parameters(self.request.args)
             if response is not None:
                 return response
             response = self.check_parameters(
-                ['apikey', 'COD_RH', 'COD_PROYECTO', 'COD_PATENTE', 'model_year', 'institution'], self.request.args.keys())
+                ['apikey', 'COD_RH', 'COD_PROYECTO', 'COD_PATENTE', 'model_year', 'institution', 'search'], self.request.args.keys())
             if response is not None:
                 return response
 
             db_name = f'scienti_{institution}_{model_year}'
 
             response = self.check_db(db_name)
             if response is not None:
@@ -568,15 +829,39 @@
                         {'SGL_CATEGORIA': sgl_cat}, {"_id": 0}))
                     response = self.app.response_class(
                         response=self.json.dumps(data),
                         status=200,
                         mimetype='application/json'
                     )
                     return response
+                if keyword:
+                    es_index = f'scienti_{institution}_{model_year}_patent'
 
+                    # only required field for search is technical, at least for patent.
+                    fields = ["TXT_NME_PATENTE",
+                              "details.technical.product.TXT_NME_PROD",
+                              "details.technical.product.TXT_RESUMEN_PROD",
+                              "details.technical.product.TXT_OBSERV_PROD",
+                              "details.technical.product.DSC_PROJETO"
+                              ]
+                    # get the start time
+                    st = time.time()
+                    data = self.es_multi_match(keyword, fields, es_index)
+                    # get the end time
+                    et = time.time()
+                    # get the execution time
+                    elapsed_time = et - st
+                    print(f'Search for "{keyword}" Execution time:',
+                          elapsed_time, 'seconds')
+                    response = self.app.response_class(
+                        response=self.json.dumps(data),
+                        status=200,
+                        mimetype='application/json'
+                    )
+                    return response
                 data = {
                     "error": "Bad Request", "message": "invalid parameters, please select the right combination of parameters"}
                 response = self.app.response_class(
                     response=self.json.dumps(data),
                     status=400,
                     mimetype='application/json'
                 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Hunabku_scienti-0.0.6/setup.py` & `Hunabku_scienti-0.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,14 +79,16 @@
 
         # Dependent packages (distributions)
         # put you packages here
         install_requires=[
             'flask>=1.1.2',
             'requests>=2.22.0',
             'hunabku',
-            'pymongo'
+            'pymongo',
+            'elasticsearch>=7.0.0',
+            'elasticsearch-dsl>=7.0.0'  # there is not release for es 8 yet, but it works.
         ],
     )
 
 
 if __name__ == "__main__":
     main()
```

