# Comparing `tmp/nsj_queue_lib-0.1.5.tar.gz` & `tmp/nsj_queue_lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_queue_lib-0.1.5.tar", last modified: Mon Jul 24 20:19:52 2023, max compression
+gzip compressed data, was "nsj_queue_lib-0.2.0.tar", last modified: Tue Jul 25 23:17:43 2023, max compression
```

## Comparing `nsj_queue_lib-0.1.5.tar` & `nsj_queue_lib-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-24 20:19:52.260893 nsj_queue_lib-0.1.5/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2542 2023-07-24 20:19:52.260893 nsj_queue_lib-0.1.5/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1976 2023-07-21 22:40:47.000000 nsj_queue_lib-0.1.5/README.md
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-24 20:19:52.256893 nsj_queue_lib-0.1.5/nsj_queue_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-19 18:24:10.000000 nsj_queue_lib-0.1.5/nsj_queue_lib/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       45 2023-07-19 18:24:10.000000 nsj_queue_lib-0.1.5/nsj_queue_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1090 2023-07-22 22:37:18.000000 nsj_queue_lib-0.1.5/nsj_queue_lib/lock_dao.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7337 2023-07-22 23:56:41.000000 nsj_queue_lib-0.1.5/nsj_queue_lib/main_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3938 2023-07-22 23:56:52.000000 nsj_queue_lib-0.1.5/nsj_queue_lib/notify_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3243 2023-07-22 23:57:02.000000 nsj_queue_lib-0.1.5/nsj_queue_lib/purge_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2914 2023-07-23 00:11:01.000000 nsj_queue_lib-0.1.5/nsj_queue_lib/queue_client.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4913 2023-07-22 23:57:41.000000 nsj_queue_lib-0.1.5/nsj_queue_lib/retry_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3887 2023-07-24 19:14:51.000000 nsj_queue_lib-0.1.5/nsj_queue_lib/retry_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1824 2023-07-19 18:24:10.000000 nsj_queue_lib-0.1.5/nsj_queue_lib/settings.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7252 2023-07-22 23:56:10.000000 nsj_queue_lib-0.1.5/nsj_queue_lib/tarefa_dao.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      860 2023-07-19 18:24:10.000000 nsj_queue_lib-0.1.5/nsj_queue_lib/worker_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      252 2023-07-22 18:37:53.000000 nsj_queue_lib-0.1.5/nsj_queue_lib/worker_fila_teste.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-24 20:19:52.260893 nsj_queue_lib-0.1.5/nsj_queue_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2542 2023-07-24 20:19:52.000000 nsj_queue_lib-0.1.5/nsj_queue_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      661 2023-07-24 20:19:52.000000 nsj_queue_lib-0.1.5/nsj_queue_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-24 20:19:52.000000 nsj_queue_lib-0.1.5/nsj_queue_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       64 2023-07-24 20:19:52.000000 nsj_queue_lib-0.1.5/nsj_queue_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2023-07-24 20:19:52.000000 nsj_queue_lib-0.1.5/nsj_queue_lib.egg-info/top_level.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.1.5/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      786 2023-07-24 20:19:52.260893 nsj_queue_lib-0.1.5/setup.cfg
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-24 20:19:52.260893 nsj_queue_lib-0.1.5/tests/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1324 2023-07-22 22:40:40.000000 nsj_queue_lib-0.1.5/tests/test_push_notification.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-25 23:17:43.993229 nsj_queue_lib-0.2.0/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2542 2023-07-25 23:17:43.993229 nsj_queue_lib-0.2.0/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1976 2023-07-21 22:40:47.000000 nsj_queue_lib-0.2.0/README.md
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-25 23:17:43.993229 nsj_queue_lib-0.2.0/nsj_queue_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-19 18:24:10.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       98 2023-07-25 22:33:41.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1090 2023-07-22 22:37:18.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/lock_dao.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    10309 2023-07-25 22:49:38.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/main_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3938 2023-07-25 19:59:05.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/notify_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3243 2023-07-22 23:57:02.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/purge_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2989 2023-07-25 19:59:54.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/queue_client.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4913 2023-07-22 23:57:41.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/retry_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4063 2023-07-25 18:59:20.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/retry_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1960 2023-07-25 19:58:20.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/settings.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9170 2023-07-25 20:41:12.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/tarefa_dao.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1126 2023-07-25 22:50:19.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/worker_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      325 2023-07-25 22:56:30.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/worker_fila_teste.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1395 2023-07-25 23:11:07.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/worker_pub_sub_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      509 2023-07-25 22:43:19.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/worker_pub_sub_teste.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2162 2023-07-25 22:51:30.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/worker_webhook.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-25 23:17:43.993229 nsj_queue_lib-0.2.0/nsj_queue_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2542 2023-07-25 23:17:43.000000 nsj_queue_lib-0.2.0/nsj_queue_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      742 2023-07-25 23:17:43.000000 nsj_queue_lib-0.2.0/nsj_queue_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-25 23:17:43.000000 nsj_queue_lib-0.2.0/nsj_queue_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       64 2023-07-25 23:17:43.000000 nsj_queue_lib-0.2.0/nsj_queue_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2023-07-25 23:17:43.000000 nsj_queue_lib-0.2.0/nsj_queue_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.2.0/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      786 2023-07-25 23:17:43.993229 nsj_queue_lib-0.2.0/setup.cfg
```

### Comparing `nsj_queue_lib-0.1.5/PKG-INFO` & `nsj_queue_lib-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_queue_lib
-Version: 0.1.5
+Version: 0.2.0
 Summary: Biblioteca para facilitar a implementação de filas e workers.
 Home-page: https://github.com/Nasajon/nsj-queue-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-queue-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_queue_lib-0.1.5/README.md` & `nsj_queue_lib-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.1.5/nsj_queue_lib/lock_dao.py` & `nsj_queue_lib-0.2.0/nsj_queue_lib/lock_dao.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.1.5/nsj_queue_lib/notify_thread.py` & `nsj_queue_lib-0.2.0/nsj_queue_lib/notify_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.1.5/nsj_queue_lib/purge_thread.py` & `nsj_queue_lib-0.2.0/nsj_queue_lib/purge_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.1.5/nsj_queue_lib/queue_client.py` & `nsj_queue_lib-0.2.0/nsj_queue_lib/queue_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 from nsj_sql_utils_lib.dbadapter3 import DBAdapter3
 
 from tarefa_dao import TarefaDAO
 
 
 class QueueClient:
-    def __init__(self, bd_conn, queue_table: str) -> None:
-        self._tarefa_dao = TarefaDAO(DBAdapter3(bd_conn), queue_table)
+    def __init__(self, bd_conn, queue_table: str, queue_subscriber_table: str) -> None:
+        self._tarefa_dao = TarefaDAO(
+            DBAdapter3(bd_conn), queue_table, queue_subscriber_table
+        )
 
     def insert_task(
         self,
         origem: str,
         destino: str,
         processo: str,
         chave_externa: str,
```

### Comparing `nsj_queue_lib-0.1.5/nsj_queue_lib/retry_thread.py` & `nsj_queue_lib-0.2.0/nsj_queue_lib/retry_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.1.5/nsj_queue_lib/retry_util.py` & `nsj_queue_lib-0.2.0/nsj_queue_lib/retry_util.py`

 * *Files 15% similar despite different names*

```diff
@@ -72,14 +72,17 @@
                     "id_anterior": tarefa["id"],
                     "data_hora_anterior": tarefa["data_hora"],
                     "status_anterior": tarefa["status"],
                     "mensagem_anterior": tarefa["mensagem"],
                     "tenant": tarefa["tenant"],
                     "grupo_empresarial": tarefa["grupo_empresarial"],
                     "payload_hash": tarefa["payload_hash"],
+                    "pub_sub": tarefa["pub_sub"],
+                    "publication_id": tarefa["publication_id"],
+                    "subscriber_id": tarefa["subscriber_id"],
                 }
 
                 dao.insert(tarefa)
             else:
                 # Atualizando status da tarefa para indicar falha,
                 # e marcando estouro de tentativas
                 logger.info(
```

### Comparing `nsj_queue_lib-0.1.5/nsj_queue_lib/settings.py` & `nsj_queue_lib-0.2.0/nsj_queue_lib/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 DB_PORT = int(os.environ["DB_PORT"])
 DB_BASE = os.environ["DB_BASE"]
 DB_USER = os.environ["DB_USER"]
 DB_PASS = os.environ["DB_PASS"]
 
 QUEUE_NAME = os.environ["QUEUE_NAME"]
 QUEUE_TABLE = os.environ["QUEUE_TABLE"]
+QUEUE_SUBSCRIBER_TABLE = os.getenv("QUEUE_SUBSCRIBER_TABLE")
 
 QUEUE_MAX_RETRY = int(os.getenv("QUEUE_MAX_RETRY", "100"))
 QUEUE_BASE_INTERVAL_RETRY = int(os.getenv("QUEUE_BASE_INTERVAL_RETRY", "5"))
 
 QUEUE_MINUTE_RETRY_THREAD = os.getenv(
     "QUEUE_MINUTE_RETRY_THREAD", "0,5,10,15,20,25,30,35,40,45,50,55"
 )
@@ -24,14 +25,16 @@
 QUEUE_MINUTE_NOTIFY_THREAD = os.getenv(
     "QUEUE_MINUTE_NOTIFY_THREAD", "0,5,10,15,20,25,30,35,40,45,50,55"
 )
 
 QUEUE_PURGE_MAX_AGE = int(os.getenv("QUEUE_PURGE_MAX_AGE", "60"))
 QUEUE_PURGE_LIMIT = int(os.getenv("QUEUE_PURGE_LIMIT", "1000"))
 
+DEFAULT_WEBHOOK_TIMEOUT = int(os.getenv("DEFAULT_WEBHOOK_TIMEOUT", "20"))
+
 ENV = os.getenv("ENV", "DEV").upper()
 GRAFANA_URL = os.getenv("GRAFANA_URL")
 LOG_DEBUG = os.getenv("LOG_DEBUG", "False").upper() == "TRUE"
 
 # Resolvendo as constantes e variáveis globais
 WORKER_NAME = f"{QUEUE_NAME}_WORKER_{uuid.uuid4()}"
 GLOBAL_RUN = True
```

### Comparing `nsj_queue_lib-0.1.5/nsj_queue_lib/tarefa_dao.py` & `nsj_queue_lib-0.2.0/nsj_queue_lib/tarefa_dao.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import datetime
 import hashlib
 
-from nsj_sql_utils_lib import dao_util
+from nsj_gcf_utils.json_util import json_dumps
 
+from nsj_sql_utils_lib import dao_util
 from nsj_sql_utils_lib.dbadapter3 import DBAdapter3
+
 from nsj_queue_lib.exception import NotFoundException
 
 
 class TarefaDAO:
     COLUNAS = [
         "id",
         "id_inicial",
@@ -23,44 +25,90 @@
         "mensagem",
         "id_anterior",
         "data_hora_anterior",
         "status_anterior",
         "mensagem_anterior",
         "tenant",
         "grupo_empresarial",
+        "payload",
         "payload_hash",
+        "pub_sub",
+        "publication_id",
+        "subscriber_id",
     ]
     COLUNAS_STR = "tarefa." + ", tarefa.".join(COLUNAS)
 
-    def __init__(self, db: DBAdapter3, queue_table: str):
+    COLUNAS_SUBSCRIBER = [
+        "id",
+        "tenant",
+        "grupo_empresarial",
+        "processo",
+        "url",
+        "http_method",
+        "headers",
+        "ativo",
+        "created_at",
+    ]
+    COLUNAS_SUBSCRIBER_STR = "sub." + ", sub.".join(COLUNAS_SUBSCRIBER)
+
+    def __init__(
+        self, db: DBAdapter3, queue_table: str, queue_subscriber_table: str = None
+    ):
         self.db = db
         self.queue_table = queue_table
+        self.queue_subscriber_table = queue_subscriber_table
 
     def get(self, id: int):
         """
         Recupera uma tarefa, por meio de seu ID
         """
         sql = f"""
             select
                 {TarefaDAO.COLUNAS_STR},
                 coalesce(tarefa.payload, inicial.payload) as payload
             from
                 {self.queue_table} as tarefa
                 left join {self.queue_table} as inicial
-                on (tarefa.id_inicial = inicial.id)
+                    on (tarefa.id_inicial = inicial.id)
             where
                 tarefa.id = %(id)s
         """
         result, count = self.db.execute(sql, id=id)
 
         if count != 1:
             raise NotFoundException("Não encontrada tarefa com ID {id}")
 
         return result[0]
 
+    def list_subscribers(self, processo: str, tenant: int, grupo_empresarial: str):
+        """
+        Recupera uma tarefa, por meio de seu ID
+        """
+        if self.queue_subscriber_table is None:
+            raise Exception(
+                f"Tabela de assinaturas não informada para a fila: {self.queue_table}"
+            )
+
+        sql = f"""
+            select
+                {TarefaDAO.COLUNAS_SUBSCRIBER_STR}
+            from
+                {self.queue_subscriber_table} as sub
+            where
+                (sub.tenant is null or sub.tenant=%(tenant)s)
+                and (sub.grupo_empresarial is null or sub.grupo_empresarial=%(grupo_empresarial)s)
+                and sub.processo=%(processo)s
+                and sub.ativo
+        """
+        result, _ = self.db.execute(
+            sql, processo=processo, tenant=tenant, grupo_empresarial=grupo_empresarial
+        )
+
+        return result
+
     # def get_recuperacao_falhas(self, max_retries: int):
     #     """
     #     Lista as tarefas que tiveram falha, mas ainda passíveis de novo tratamento.
     #     """
     #     sql = f"""
     #         select
     #             {TarefaDAO.COLUNAS}
@@ -125,16 +173,24 @@
     def insert(self, tarefa: dict[str, any]):
         # Calculando o hash do payload
         if (
             "payload" in tarefa
             and tarefa["payload"] is not None
             and tarefa["payload"] != ""
         ):
-            payload_hash = hashlib.sha256(tarefa["payload"].encode()).hexdigest()
+            if isinstance(tarefa["payload"], dict):
+                payload = json_dumps(tarefa["payload"])
+            elif not isinstance(tarefa["payload"], str):
+                payload = f"{tarefa['payload']}"
+            else:
+                payload = tarefa["payload"]
+
+            payload_hash = hashlib.sha256(payload.encode()).hexdigest()
             tarefa["payload_hash"] = payload_hash
+            tarefa["payload"] = payload
 
         # Verificando os fields recebidos
         fields = []
         for col in TarefaDAO.COLUNAS:
             if col in tarefa:
                 fields.append(col)
 
@@ -194,19 +250,24 @@
                     data_hora > clock_timestamp() - interval '{max_age} days'
                 ORDER BY data_hora
                 LIMIT {purge_limit}
             )        
         """
         self.db.execute(sql)
 
-    def update_status(self, tarefa_id: int, status: str):
+    def update_status(self, tarefa_id: int, status: str, mensagem: str = None):
+        msg_sql = ""
+        if mensagem is not None:
+            msg_sql = ", mensagem = %(mensagem)s"
+
         sql = f"""
-            update {self.queue_table} set status = %(status)s where id=%(id)s
+            update {self.queue_table} set status = %(status)s{msg_sql} where id=%(id)s
         """
-        self.db.execute(sql, id=tarefa_id, status=status)
+
+        self.db.execute(sql, id=tarefa_id, status=status, mensagem=mensagem)
 
     def notify(self, nome_fila: str):
         sql = f"""
             notify {nome_fila}, ''
         """
         self.db.execute(sql)
```

### Comparing `nsj_queue_lib-0.1.5/nsj_queue_lib.egg-info/PKG-INFO` & `nsj_queue_lib-0.2.0/nsj_queue_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-queue-lib
-Version: 0.1.5
+Version: 0.2.0
 Summary: Biblioteca para facilitar a implementação de filas e workers.
 Home-page: https://github.com/Nasajon/nsj-queue-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-queue-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_queue_lib-0.1.5/setup.cfg` & `nsj_queue_lib-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_queue_lib
-version = 0.1.5
+version = 0.2.0
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para facilitar a implementação de filas e workers.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj-queue-lib
 project_urls =
```

