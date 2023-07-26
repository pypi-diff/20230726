# Comparing `tmp/rabbitmq_broker-1.1.3-py3-none-any.whl.zip` & `tmp/rabbitmq_broker-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 16621 bytes, number of entries: 24
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-06 15:36 rmq_broker/__init__.py
+Zip file size: 16974 bytes, number of entries: 24
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-26 09:39 rmq_broker/__init__.py
 -rw-r--r--  2.0 unx     1080 b- defN 23-May-31 15:11 rmq_broker/schemas.py
 -rw-r--r--  2.0 unx      508 b- defN 23-May-26 07:16 rmq_broker/settings.py
 -rw-r--r--  2.0 unx      257 b- defN 23-Jun-06 15:36 rmq_broker/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/async_chains/__init__.py
--rw-r--r--  2.0 unx     8403 b- defN 23-Jun-06 15:36 rmq_broker/async_chains/base.py
+-rw-r--r--  2.0 unx     9175 b- defN 23-Jul-26 12:19 rmq_broker/async_chains/base.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/chains/__init__.py
 -rw-r--r--  2.0 unx     4333 b- defN 23-Jun-06 15:36 rmq_broker/chains/base.py
 -rw-r--r--  2.0 unx       37 b- defN 23-Jun-06 15:36 rmq_broker/documentation/__init__.py
--rw-r--r--  2.0 unx     3262 b- defN 23-Jun-06 15:36 rmq_broker/documentation/base.py
+-rw-r--r--  2.0 unx     3542 b- defN 23-Jul-26 12:19 rmq_broker/documentation/base.py
 -rw-r--r--  2.0 unx    10645 b- defN 23-Jun-06 15:36 rmq_broker/documentation/models.py
 -rw-r--r--  2.0 unx      136 b- defN 23-Jun-06 15:36 rmq_broker/documentation/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 15:36 rmq_broker/documentation/mixins/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 15:36 rmq_broker/documentation/mixins/pydantic/__init__.py
 -rw-r--r--  2.0 unx     1278 b- defN 23-Jun-06 15:36 rmq_broker/documentation/mixins/pydantic/chains.py
 -rw-r--r--  2.0 unx     1307 b- defN 23-Jun-06 15:36 rmq_broker/documentation/mixins/pydantic/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-26 07:16 rmq_broker/queues/__init__.py
 -rw-r--r--  2.0 unx     1107 b- defN 23-May-26 07:16 rmq_broker/queues/base.py
 -rw-r--r--  2.0 unx     1765 b- defN 23-May-26 07:16 rmq_broker/queues/rabbitmq.py
--rw-r--r--  2.0 unx     1074 b- defN 23-Jun-06 15:37 rabbitmq_broker-1.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     4405 b- defN 23-Jun-06 15:37 rabbitmq_broker-1.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 15:37 rabbitmq_broker-1.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-06 15:37 rabbitmq_broker-1.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2104 b- defN 23-Jun-06 15:37 rabbitmq_broker-1.1.3.dist-info/RECORD
-24 files, 41826 bytes uncompressed, 13145 bytes compressed:  68.6%
+-rw-r--r--  2.0 unx     1074 b- defN 23-Jul-26 12:49 rabbitmq_broker-1.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4405 b- defN 23-Jul-26 12:49 rabbitmq_broker-1.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 12:49 rabbitmq_broker-1.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-26 12:49 rabbitmq_broker-1.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2104 b- defN 23-Jul-26 12:49 rabbitmq_broker-1.1.4.dist-info/RECORD
+24 files, 42878 bytes uncompressed, 13498 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -51,23 +51,23 @@
 
 Filename: rmq_broker/queues/base.py
 Comment: 
 
 Filename: rmq_broker/queues/rabbitmq.py
 Comment: 
 
-Filename: rabbitmq_broker-1.1.3.dist-info/LICENSE
+Filename: rabbitmq_broker-1.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: rabbitmq_broker-1.1.3.dist-info/METADATA
+Filename: rabbitmq_broker-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: rabbitmq_broker-1.1.3.dist-info/WHEEL
+Filename: rabbitmq_broker-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: rabbitmq_broker-1.1.3.dist-info/top_level.txt
+Filename: rabbitmq_broker-1.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: rabbitmq_broker-1.1.3.dist-info/RECORD
+Filename: rabbitmq_broker-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rmq_broker/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.3"
+__version__ = "1.1.4"
```

## rmq_broker/async_chains/base.py

```diff
@@ -106,17 +106,26 @@
     Базовый классов обработчиков.
 
     Args:
         AbstractChain: Интерфейс классов обработчиков.
 
     Attributes:
         request_type (str): Тип запроса, который обработчик способен обработать.
+        include_in_schema (bool): True (значение по умолчанию) - выводить Chain в Swagger документацию;
+                                False - исключить Chain из Swagger документации.
+        deprecated (bool): False (значение по умолчанию) - Chain актуален;
+                        True - отметить Chain, как устаревший.
+        actual (str): Наименование актуального Chain в Swagger документации. Отображается
+                    рядом с устаревшим Chain (где include_in_schema = True, deprecated = True).
     """
 
     request_type: str = ""
+    include_in_schema: bool = True
+    deprecated: bool = False
+    actual: str = ""
 
     async def handle(self, data: IncomingMessage) -> OutgoingMessage:
         """
         Обрабатывает запрос, пропуская его через методы обработки
         заголовка и тела запроса.
 
         Args:
```

## rmq_broker/documentation/base.py

```diff
@@ -13,25 +13,30 @@
 
 
 class BaseDocsChain:
     openapi: dict = {}
     title: str = settings.SERVICE_NAME
     openapi_version: str = "3.0.2"
     version: str = "0.1"
+    include_in_schema = False
 
     def make_chain_description(self, chain: BaseChain, model_name_map: dict) -> dict:
         name = chain.__class__.__name__
         required = getattr(chain, "body_model", None) in model_name_map
         # todo: Обязательность относительно обязательных параметров формы
         operation = {
             "tags": [f"RPC: {get_class_dir(chain)}"],
             "summary": name,
             "description": chain.__class__.__doc__,
             "operationId": chain.request_type,
         }
+        if chain.deprecated:
+            operation['deprecated'] = True
+            if chain.actual:
+                operation['summary'] += ". Актуальный - " + chain.actual + "."
         request_body = {
             "required": required,
         }
         if required:
             model_name = model_name_map.get(chain.body_model)
             request_body["content"] = {
                 "application/json": {"schema": {"$ref": f"{REF_PREFIX}{model_name}"}}
@@ -46,26 +51,26 @@
         self,
         chain_manager: ChainManager,
     ) -> dict:
         output: dict = {
             "openapi": self.openapi_version,
             "info": {"title": self.title, "version": self.version},
         }
-        chains = [chain() for chain in chain_manager.chains.values()]
+        chains = [chain() for chain in chain_manager.chains.values() if chain.include_in_schema]
         components: dict = {}
         paths = defaultdict(dict)
 
         typed_requests = [
             chain.body_model for chain in chains if getattr(chain, "body_model", None)
         ]
         model_name_map, definitions = self.process_forms(models=typed_requests)
 
         for chain in chains:
             operation = self.make_chain_description(chain, model_name_map)
-            name = operation["summary"]
+            name = "/" + get_class_dir(chain) + "/" + chain.request_type
             paths[name]["post"] = operation
 
         if definitions:
             components["schemas"] = {k: definitions[k] for k in sorted(definitions)}
         if components:
             output["components"] = components
         output["paths"] = dict(
```

## Comparing `rabbitmq_broker-1.1.3.dist-info/LICENSE` & `rabbitmq_broker-1.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rabbitmq_broker-1.1.3.dist-info/METADATA` & `rabbitmq_broker-1.1.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbitmq-broker
-Version: 1.1.3
+Version: 1.1.4
 Summary: RPC брокер сообщений
 Author-email: Nikita Sysoev <njt55cs@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

## Comparing `rabbitmq_broker-1.1.3.dist-info/RECORD` & `rabbitmq_broker-1.1.4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-rmq_broker/__init__.py,sha256=u9ExJqoMv3fQc8WmLTw4I2FnQo6u4xRrBc6DLy6G1IE,22
+rmq_broker/__init__.py,sha256=XxXhu8-QnuD9hA8Ah0WX5rgpt_DwOQmAwcK-FtpngyQ,22
 rmq_broker/schemas.py,sha256=1XNpJKdyX34IU1RGnpVpYdH5LgzQfejDT7pAi27_mWg,1080
 rmq_broker/settings.py,sha256=kqSzECBSLWz6n7jjpuDzIM_Fvn_BQqtlR19axAia2Cc,508
 rmq_broker/utils.py,sha256=en9PcLeHH6ZZ4QWllXmGDcBoUYEHbGhIbpNT1cmfQlA,257
 rmq_broker/async_chains/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-rmq_broker/async_chains/base.py,sha256=bA6lQdBXPWN76kPMcVM_Ym1tooRPhcsuLjpmqSTKhkY,8403
+rmq_broker/async_chains/base.py,sha256=fgTehwMSsknuwzQ5VZvjE7eNsGDIIeFJXMbqqfdj7CE,9175
 rmq_broker/chains/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rmq_broker/chains/base.py,sha256=UCCkAcO0QLoZBhnygxxSOsB9nOiRMYGxZAuZ4zdy5Us,4333
 rmq_broker/documentation/__init__.py,sha256=-JASC9CfKyUXByBfarQKfYyhIMF77gz_UUCH4aiQ7UY,37
-rmq_broker/documentation/base.py,sha256=LYBc34r9IP3ViGJ1tmiKIBdQCuUfpivlY1jNQw5Zbj0,3262
+rmq_broker/documentation/base.py,sha256=XBCxhHjtQMH5VoFoyrBbXDwv1UZK2opW24fPYmiNrek,3542
 rmq_broker/documentation/models.py,sha256=YA84fcsPVjTwcM7t8pMMBT9MJ4acKc24IOAq71S-OM0,10645
 rmq_broker/documentation/utils.py,sha256=ej76hHKJFAh73xZ2_wDo4aQrpxxhCQqA_7W599fCYGE,136
 rmq_broker/documentation/mixins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rmq_broker/documentation/mixins/pydantic/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rmq_broker/documentation/mixins/pydantic/chains.py,sha256=vZsVZA4WdEp1FisayPvBAaDnvjp0lgtvjT9ZXYHbjbA,1278
 rmq_broker/documentation/mixins/pydantic/utils.py,sha256=3IAa7--LakKyyfcFcsfbOScSppYOyNNrmX42RpY3EsI,1307
 rmq_broker/queues/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rmq_broker/queues/base.py,sha256=XgUIn04MxoulYjN-v8LVcPKprmiSHy9UmKTzoBfyBug,1107
 rmq_broker/queues/rabbitmq.py,sha256=cujY9KKwld146SEyCHhcXe08cgHxRn3ARIxOfXuIViQ,1765
-rabbitmq_broker-1.1.3.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-rabbitmq_broker-1.1.3.dist-info/METADATA,sha256=HFJocOleB8huFBvDXzZ7TChBq7DPEv6827B7BIkwCqA,4405
-rabbitmq_broker-1.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rabbitmq_broker-1.1.3.dist-info/top_level.txt,sha256=gyiGN4_aIuuxH76M_A_yn64Bxy2nj4fFJ1C84g3BPQQ,11
-rabbitmq_broker-1.1.3.dist-info/RECORD,,
+rabbitmq_broker-1.1.4.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+rabbitmq_broker-1.1.4.dist-info/METADATA,sha256=eF4GwqMeUY-WHaKcgv2vzEc_eyJD3QwxLY0QWS0dzdo,4405
+rabbitmq_broker-1.1.4.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+rabbitmq_broker-1.1.4.dist-info/top_level.txt,sha256=gyiGN4_aIuuxH76M_A_yn64Bxy2nj4fFJ1C84g3BPQQ,11
+rabbitmq_broker-1.1.4.dist-info/RECORD,,
```

