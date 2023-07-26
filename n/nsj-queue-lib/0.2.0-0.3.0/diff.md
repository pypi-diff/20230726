# Comparing `tmp/nsj_queue_lib-0.2.0.tar.gz` & `tmp/nsj_queue_lib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_queue_lib-0.2.0.tar", last modified: Tue Jul 25 23:17:43 2023, max compression
+gzip compressed data, was "nsj_queue_lib-0.3.0.tar", last modified: Wed Jul 26 18:47:05 2023, max compression
```

## Comparing `nsj_queue_lib-0.2.0.tar` & `nsj_queue_lib-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-25 23:17:43.993229 nsj_queue_lib-0.2.0/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2542 2023-07-25 23:17:43.993229 nsj_queue_lib-0.2.0/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1976 2023-07-21 22:40:47.000000 nsj_queue_lib-0.2.0/README.md
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-25 23:17:43.993229 nsj_queue_lib-0.2.0/nsj_queue_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-19 18:24:10.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       98 2023-07-25 22:33:41.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1090 2023-07-22 22:37:18.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/lock_dao.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    10309 2023-07-25 22:49:38.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/main_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3938 2023-07-25 19:59:05.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/notify_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3243 2023-07-22 23:57:02.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/purge_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2989 2023-07-25 19:59:54.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/queue_client.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4913 2023-07-22 23:57:41.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/retry_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4063 2023-07-25 18:59:20.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/retry_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1960 2023-07-25 19:58:20.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/settings.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     9170 2023-07-25 20:41:12.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/tarefa_dao.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1126 2023-07-25 22:50:19.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/worker_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      325 2023-07-25 22:56:30.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/worker_fila_teste.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1395 2023-07-25 23:11:07.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/worker_pub_sub_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      509 2023-07-25 22:43:19.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/worker_pub_sub_teste.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2162 2023-07-25 22:51:30.000000 nsj_queue_lib-0.2.0/nsj_queue_lib/worker_webhook.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-25 23:17:43.993229 nsj_queue_lib-0.2.0/nsj_queue_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2542 2023-07-25 23:17:43.000000 nsj_queue_lib-0.2.0/nsj_queue_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      742 2023-07-25 23:17:43.000000 nsj_queue_lib-0.2.0/nsj_queue_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-25 23:17:43.000000 nsj_queue_lib-0.2.0/nsj_queue_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       64 2023-07-25 23:17:43.000000 nsj_queue_lib-0.2.0/nsj_queue_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2023-07-25 23:17:43.000000 nsj_queue_lib-0.2.0/nsj_queue_lib.egg-info/top_level.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.2.0/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      786 2023-07-25 23:17:43.993229 nsj_queue_lib-0.2.0/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-26 18:47:05.797599 nsj_queue_lib-0.3.0/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2542 2023-07-26 18:47:05.797599 nsj_queue_lib-0.3.0/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1976 2023-07-21 22:40:47.000000 nsj_queue_lib-0.3.0/README.md
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-26 18:47:05.797599 nsj_queue_lib-0.3.0/nsj_queue_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-19 18:24:10.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       98 2023-07-25 22:33:41.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1090 2023-07-22 22:37:18.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/lock_dao.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    10609 2023-07-26 17:36:54.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/main_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3938 2023-07-25 19:59:05.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/notify_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3243 2023-07-22 23:57:02.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/purge_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4624 2023-07-26 17:21:11.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/queue_client.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4913 2023-07-22 23:57:41.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/retry_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5259 2023-07-26 18:39:19.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/retry_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1960 2023-07-25 19:58:20.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/settings.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9205 2023-07-26 18:03:22.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/tarefa_dao.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1756 2023-07-26 17:45:30.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/worker_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      368 2023-07-26 18:13:34.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/worker_fila_teste.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2733 2023-07-26 17:51:10.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/worker_pub_sub_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      509 2023-07-25 22:43:19.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/worker_pub_sub_teste.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2162 2023-07-26 17:51:34.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/worker_webhook.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-26 18:47:05.797599 nsj_queue_lib-0.3.0/nsj_queue_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2542 2023-07-26 18:47:05.000000 nsj_queue_lib-0.3.0/nsj_queue_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      742 2023-07-26 18:47:05.000000 nsj_queue_lib-0.3.0/nsj_queue_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-26 18:47:05.000000 nsj_queue_lib-0.3.0/nsj_queue_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       64 2023-07-26 18:47:05.000000 nsj_queue_lib-0.3.0/nsj_queue_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2023-07-26 18:47:05.000000 nsj_queue_lib-0.3.0/nsj_queue_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.3.0/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      786 2023-07-26 18:47:05.797599 nsj_queue_lib-0.3.0/setup.cfg
```

### Comparing `nsj_queue_lib-0.2.0/PKG-INFO` & `nsj_queue_lib-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_queue_lib
-Version: 0.2.0
+Version: 0.3.0
 Summary: Biblioteca para facilitar a implementação de filas e workers.
 Home-page: https://github.com/Nasajon/nsj-queue-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-queue-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_queue_lib-0.2.0/README.md` & `nsj_queue_lib-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.2.0/nsj_queue_lib/lock_dao.py` & `nsj_queue_lib-0.3.0/nsj_queue_lib/lock_dao.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.2.0/nsj_queue_lib/main_thread.py` & `nsj_queue_lib-0.3.0/nsj_queue_lib/main_thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,27 +150,30 @@
         # Atualizando status da tarefa para processando.
         logger.debug(
             f"Atualizando status da tarefa com ID: {tarefa['id']}, para processando."
         )
         dao.update_status(tarefa["id"], "processando")
 
         try:
-            # Verificando se é uma tarefa do tipo pub_sub
-            if tarefa["pub_sub"]:
+            if tarefa["dead"]:
+                # Verificando se é uma tarefa já morta
+                self._run_worker(tarefa, True)
+            elif tarefa["pub_sub"]:
+                # Verificando se é uma tarefa do tipo pub_sub
                 self._publish(dao, tarefa)
             else:
-                self._run_worker(tarefa)
+                self._run_worker(tarefa, False)
         except Exception as e:
             logger.exception(
                 f"Erro executando a tarefa com ID: {tarefa['id']}.", e, stack_info=True
             )
 
             RetryUtil().reenfileir_tarefa(dao, tarefa, False, str(e))
 
-    def _run_worker(self, tarefa: dict[str, any]):
+    def _run_worker(self, tarefa: dict[str, any], dead: bool):
         """
         Executa de fato o código do worker, para tratar uma tarefa. Passos:
         1. Abre nova conexão com o BD
         2. Abre nova transação
         3. Se tiver sucesso, commita e atualiza o status para sucesso
         4. Se tiver falha, faz rollback (mas, o status para falha dependerá do método
         anterior, que chama este, porque o controle de falha se dá na conexão da MainThread)
@@ -183,15 +186,18 @@
             new_db = DBAdapter3(new_dbconn.conn)
             new_dao = TarefaDAO(new_db, QUEUE_TABLE)
 
             # Iniciando transação
             new_dao.db.begin()
             try:
                 # Invocando o código customizado para execução da tarefa.
-                mensagem = self.worker.internal_execute(tarefa, new_dbconn)
+                if not dead:
+                    mensagem = self.worker.internal_execute(tarefa, new_dbconn)
+                else:
+                    mensagem = self.worker.internal_execute_dead(tarefa, new_dbconn)
 
                 if mensagem is None:
                     mensagem = "Concluído com sucesso"
 
                 # Atualizando o status para concluido com sucesso.
                 logger.debug(
                     f"Atualizando status da tarefa com ID: {tarefa['id']}, para concluido com sucesso."
```

### Comparing `nsj_queue_lib-0.2.0/nsj_queue_lib/notify_thread.py` & `nsj_queue_lib-0.3.0/nsj_queue_lib/notify_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.2.0/nsj_queue_lib/purge_thread.py` & `nsj_queue_lib-0.3.0/nsj_queue_lib/purge_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.2.0/nsj_queue_lib/retry_thread.py` & `nsj_queue_lib-0.3.0/nsj_queue_lib/retry_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.2.0/nsj_queue_lib/retry_util.py` & `nsj_queue_lib-0.3.0/nsj_queue_lib/retry_util.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     def reenfileir_tarefa(
         self,
         dao: TarefaDAO,
         tarefa: dict[str, any],
         falha_desconhecida: bool,
         msg: str = None,
     ):
+        # Tratando do status e da mensagem de falha
         if falha_desconhecida:
             msg_reenfileirar = "Falha desconhecida de processamento (processamento abortado repentinamento). Tarefa reenfileirada."
             msg_max_tentativas = "Falha desconhecida de processamento (processamento abortado repentinamento), e máximo de tentativas atingido."
             status = "falha_processando"
         else:
             if msg is None:
                 msg_reenfileirar = "Falha desconhecida. Tarefa reenfileirada."
@@ -28,19 +29,23 @@
                 )
             else:
                 msg_reenfileirar = f"{msg}. Tarefa reenfileirada."
                 msg_max_tentativas = f"{msg}. Máximo de tentativas atingido."
 
             status = "falha"
 
+        # Realizando de fato a inserção da nova tarefa no banco, e atualização do status
         try:
             # Iniciando transação
             dao.db.begin()
 
-            if tarefa["tentativa"] <= QUEUE_MAX_RETRY:
+            # Resolvendo o ID inicial
+            id_inicial = tarefa["id_inicial"] or tarefa["id"]
+
+            if tarefa["tentativa"] < QUEUE_MAX_RETRY:
                 # Calculando a data e hora da próxima tentativa
                 proxima_tentativa = tarefa["data_hora"] + datetime.timedelta(
                     minutes=(tarefa["tentativa"] * QUEUE_BASE_INTERVAL_RETRY)
                 )
 
                 # Atualizando status da tarefa para indicar falha,
                 # e sinalizando que foi reenfileirada
@@ -50,17 +55,15 @@
                 dao.update_flag_reenfileiramento_falha(
                     tarefa["id"],
                     status,
                     msg_reenfileirar,
                     proxima_tentativa,
                 )
 
-                # Inserindo uma nova tentativa para a falha
-                id_inicial = tarefa["id_inicial"] or tarefa["id"]
-
+                # Inserindo uma nova tentativa para a falha (mesmo que seja para a fila de mortos)
                 tarefa = {
                     "id_inicial": id_inicial,
                     "data_hora": proxima_tentativa,
                     "data_hora_inicial": tarefa["data_hora_inicial"],
                     "origem": tarefa["origem"],
                     "destino": tarefa["destino"],
                     "processo": tarefa["processo"],
@@ -75,14 +78,16 @@
                     "mensagem_anterior": tarefa["mensagem"],
                     "tenant": tarefa["tenant"],
                     "grupo_empresarial": tarefa["grupo_empresarial"],
                     "payload_hash": tarefa["payload_hash"],
                     "pub_sub": tarefa["pub_sub"],
                     "publication_id": tarefa["publication_id"],
                     "subscriber_id": tarefa["subscriber_id"],
+                    "dead": tarefa["dead"],
+                    "live_id": tarefa["live_id"],
                 }
 
                 dao.insert(tarefa)
             else:
                 # Atualizando status da tarefa para indicar falha,
                 # e marcando estouro de tentativas
                 logger.info(
@@ -90,12 +95,31 @@
                 )
                 dao.update_falha_max_retries(
                     tarefa["id"],
                     status,
                     msg_max_tentativas,
                 )
 
+                # Inserindo a primeira tentativa da fila de mortos nova tentativa para a falha (mesmo que seja para a fila de mortos)
+                tarefa = {
+                    "origem": tarefa["origem"],
+                    "destino": tarefa["destino"],
+                    "processo": tarefa["processo"],
+                    "chave_externa": tarefa["chave_externa"],
+                    "tentativa": 1,
+                    "tenant": tarefa["tenant"],
+                    "grupo_empresarial": tarefa["grupo_empresarial"],
+                    "payload": tarefa["payload"],
+                    "pub_sub": tarefa["pub_sub"],
+                    "publication_id": tarefa["publication_id"],
+                    "subscriber_id": tarefa["subscriber_id"],
+                    "dead": True,
+                    "live_id": id_inicial,
+                }
+
+                dao.insert(tarefa)
+
             # Commit na transação
             dao.db.commit()
         finally:
             # Rollback na transação (sao já tenha sido feito commit, não faz nada).
             dao.db.rollback()
```

### Comparing `nsj_queue_lib-0.2.0/nsj_queue_lib/settings.py` & `nsj_queue_lib-0.3.0/nsj_queue_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.2.0/nsj_queue_lib/tarefa_dao.py` & `nsj_queue_lib-0.3.0/nsj_queue_lib/tarefa_dao.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,16 @@
         "tenant",
         "grupo_empresarial",
         "payload",
         "payload_hash",
         "pub_sub",
         "publication_id",
         "subscriber_id",
+        "dead",
+        "live_id",
     ]
     COLUNAS_STR = "tarefa." + ", tarefa.".join(COLUNAS)
 
     COLUNAS_SUBSCRIBER = [
         "id",
         "tenant",
         "grupo_empresarial",
```

### Comparing `nsj_queue_lib-0.2.0/nsj_queue_lib/worker_pub_sub_base.py` & `nsj_queue_lib-0.3.0/nsj_queue_lib/worker_pub_sub_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,14 +14,25 @@
         self.subscriber_id = subscriber_id
 
     def __call__(self, func):
         Subscriber.METHOD_SUBSCRIBER_DICT[self.subscriber_id] = func
         return func
 
 
+class DeadSubscriber:
+    METHOD_DEAD_SUBSCRIBER_DICT = {}
+
+    def __init__(self, subscriber_id: str) -> None:
+        self.subscriber_id = subscriber_id
+
+    def __call__(self, func):
+        DeadSubscriber.METHOD_DEAD_SUBSCRIBER_DICT[self.subscriber_id] = func
+        return func
+
+
 class WorkerPubSubBase(WorkerBase, abc.ABC):
     def execute(self, payload: str, tarefa: dict[str, any], bd_conn) -> str:
         logger.info(f"Executando a tarefa PubSub de ID: {tarefa['id']}")
         logger.debug(f"Dados da tarefa: {tarefa}")
 
         # Recuperando os dados da tarefa
         payload = json_loads(payload)
@@ -38,7 +49,34 @@
         return Subscriber.METHOD_SUBSCRIBER_DICT[subscriber_id](
             self,
             payload,
             subscription,
             tarefa,
             bd_conn,
         )
+
+    def execute_dead(self, payload: str, tarefa: dict[str, any], bd_conn) -> str:
+        """
+        Sobreescreva esse método, se desejar customizar o comportamento da fila de mortos.
+
+        O comportamento padrão é o simples registro em log.
+        """
+        logger.info(f"Executando fila de mortos da tarefa PubSub de ID: {tarefa['id']}")
+        logger.debug(f"Dados da tarefa: {tarefa}")
+
+        # Recuperando os dados da tarefa
+        payload = json_loads(payload)
+        subscription = payload["subscription"]
+        subscriber_id = subscription["id"]
+
+        # Recuperando a função da fila de mortos registrada para o subscriber_id
+        if subscriber_id not in DeadSubscriber.METHOD_DEAD_SUBSCRIBER_DICT:
+            return super().execute_dead(payload, tarefa, bd_conn)
+
+        # Executando o método registrado para o subscriber_id
+        return DeadSubscriber.METHOD_DEAD_SUBSCRIBER_DICT[subscriber_id](
+            self,
+            payload,
+            subscription,
+            tarefa,
+            bd_conn,
+        )
```

### Comparing `nsj_queue_lib-0.2.0/nsj_queue_lib/worker_webhook.py` & `nsj_queue_lib-0.3.0/nsj_queue_lib/worker_webhook.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.2.0/nsj_queue_lib.egg-info/PKG-INFO` & `nsj_queue_lib-0.3.0/nsj_queue_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-queue-lib
-Version: 0.2.0
+Version: 0.3.0
 Summary: Biblioteca para facilitar a implementação de filas e workers.
 Home-page: https://github.com/Nasajon/nsj-queue-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-queue-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_queue_lib-0.2.0/nsj_queue_lib.egg-info/SOURCES.txt` & `nsj_queue_lib-0.3.0/nsj_queue_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.2.0/setup.cfg` & `nsj_queue_lib-0.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_queue_lib
-version = 0.2.0
+version = 0.3.0
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para facilitar a implementação de filas e workers.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj-queue-lib
 project_urls =
```

