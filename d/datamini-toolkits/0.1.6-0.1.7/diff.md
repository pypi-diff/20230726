# Comparing `tmp/datamini_toolkits-0.1.6.tar.gz` & `tmp/datamini_toolkits-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamini_toolkits-0.1.6.tar", last modified: Wed Jul 12 03:15:26 2023, max compression
+gzip compressed data, was "datamini_toolkits-0.1.7.tar", last modified: Wed Jul 26 03:41:10 2023, max compression
```

## Comparing `datamini_toolkits-0.1.6.tar` & `datamini_toolkits-0.1.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:15:26.705357 datamini_toolkits-0.1.6/
--rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-07-12 03:15:26.705241 datamini_toolkits-0.1.6/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)     2366 2023-06-29 16:08:35.000000 datamini_toolkits-0.1.6/README.md
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:15:26.702155 datamini_toolkits-0.1.6/datamini_toolkits/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 14:05:31.000000 datamini_toolkits-0.1.6/datamini_toolkits/__init__.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:15:26.703474 datamini_toolkits-0.1.6/datamini_toolkits/cmysql/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:44:01.000000 datamini_toolkits-0.1.6/datamini_toolkits/cmysql/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      348 2023-07-12 02:53:51.000000 datamini_toolkits-0.1.6/datamini_toolkits/cmysql/agent.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1720 2023-07-04 11:51:19.000000 datamini_toolkits-0.1.6/datamini_toolkits/cmysql/cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-07-04 11:47:35.000000 datamini_toolkits-0.1.6/datamini_toolkits/cmysql/logs.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1243 2023-07-12 02:53:51.000000 datamini_toolkits-0.1.6/datamini_toolkits/cmysql/prompts.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:15:26.704979 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/
--rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 09:20:13.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/__init__.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     6140 2023-07-12 03:14:44.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/agent.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1614 2023-07-12 03:14:44.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/base.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2585 2023-07-12 03:13:46.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/cli.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-06-25 00:45:21.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/logs.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2940 2023-06-28 15:27:58.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/prompts.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     2705 2023-06-29 15:32:57.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/test_tools.py
--rw-r--r--   0 jeffrey    (501) staff       (20)     1016 2023-06-29 14:42:44.000000 datamini_toolkits-0.1.6/datamini_toolkits/mock_data/tools.py
--rw-r--r--   0 jeffrey    (501) staff       (20)      442 2023-06-29 15:31:26.000000 datamini_toolkits-0.1.6/datamini_toolkits/tests.py
-drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-12 03:15:26.702830 datamini_toolkits-0.1.6/datamini_toolkits.egg-info/
--rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-07-12 03:15:26.000000 datamini_toolkits-0.1.6/datamini_toolkits.egg-info/PKG-INFO
--rw-r--r--   0 jeffrey    (501) staff       (20)      757 2023-07-12 03:15:26.000000 datamini_toolkits-0.1.6/datamini_toolkits.egg-info/SOURCES.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-07-12 03:15:26.000000 datamini_toolkits-0.1.6/datamini_toolkits.egg-info/dependency_links.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)      115 2023-07-12 03:15:26.000000 datamini_toolkits-0.1.6/datamini_toolkits.egg-info/entry_points.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       18 2023-07-12 03:15:26.000000 datamini_toolkits-0.1.6/datamini_toolkits.egg-info/top_level.txt
--rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-07-12 03:15:26.705387 datamini_toolkits-0.1.6/setup.cfg
--rw-r--r--   0 jeffrey    (501) staff       (20)      417 2023-07-12 03:15:25.000000 datamini_toolkits-0.1.6/setup.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-26 03:41:10.079855 datamini_toolkits-0.1.7/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-07-26 03:41:10.079623 datamini_toolkits-0.1.7/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2366 2023-06-29 16:08:35.000000 datamini_toolkits-0.1.7/README.md
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-26 03:41:10.073938 datamini_toolkits-0.1.7/datamini_toolkits/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 14:05:31.000000 datamini_toolkits-0.1.7/datamini_toolkits/__init__.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-26 03:41:10.075586 datamini_toolkits-0.1.7/datamini_toolkits/cmysql/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-29 15:44:01.000000 datamini_toolkits-0.1.7/datamini_toolkits/cmysql/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      348 2023-07-12 02:53:51.000000 datamini_toolkits-0.1.7/datamini_toolkits/cmysql/agent.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1720 2023-07-04 11:51:19.000000 datamini_toolkits-0.1.7/datamini_toolkits/cmysql/cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-07-04 11:47:35.000000 datamini_toolkits-0.1.7/datamini_toolkits/cmysql/logs.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1243 2023-07-12 02:53:51.000000 datamini_toolkits-0.1.7/datamini_toolkits/cmysql/prompts.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-26 03:41:10.078055 datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/
+-rw-r--r--   0 jeffrey    (501) staff       (20)        0 2023-06-24 09:20:13.000000 datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/__init__.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     6232 2023-07-12 03:21:56.000000 datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/agent.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1614 2023-07-12 03:14:44.000000 datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/base.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2759 2023-07-20 13:44:15.000000 datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/cli.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1665 2023-06-25 00:45:21.000000 datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/logs.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2940 2023-06-28 15:27:58.000000 datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/prompts.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     2705 2023-06-29 15:32:57.000000 datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/test_tools.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)     1016 2023-06-29 14:42:44.000000 datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/tools.py
+-rw-r--r--   0 jeffrey    (501) staff       (20)      442 2023-06-29 15:31:26.000000 datamini_toolkits-0.1.7/datamini_toolkits/tests.py
+drwxr-xr-x   0 jeffrey    (501) staff       (20)        0 2023-07-26 03:41:10.074760 datamini_toolkits-0.1.7/datamini_toolkits.egg-info/
+-rw-r--r--   0 jeffrey    (501) staff       (20)      137 2023-07-26 03:41:10.000000 datamini_toolkits-0.1.7/datamini_toolkits.egg-info/PKG-INFO
+-rw-r--r--   0 jeffrey    (501) staff       (20)      797 2023-07-26 03:41:10.000000 datamini_toolkits-0.1.7/datamini_toolkits.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)        1 2023-07-26 03:41:10.000000 datamini_toolkits-0.1.7/datamini_toolkits.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)      120 2023-07-26 03:41:10.000000 datamini_toolkits-0.1.7/datamini_toolkits.egg-info/entry_points.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       18 2023-07-26 03:41:10.000000 datamini_toolkits-0.1.7/datamini_toolkits.egg-info/top_level.txt
+-rw-r--r--   0 jeffrey    (501) staff       (20)       38 2023-07-26 03:41:10.080216 datamini_toolkits-0.1.7/setup.cfg
+-rw-r--r--   0 jeffrey    (501) staff       (20)      422 2023-07-26 03:41:03.000000 datamini_toolkits-0.1.7/setup.py
```

### Comparing `datamini_toolkits-0.1.6/README.md` & `datamini_toolkits-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.6/datamini_toolkits/cmysql/cli.py` & `datamini_toolkits-0.1.7/datamini_toolkits/cmysql/cli.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.6/datamini_toolkits/cmysql/logs.py` & `datamini_toolkits-0.1.7/datamini_toolkits/cmysql/logs.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.6/datamini_toolkits/cmysql/prompts.py` & `datamini_toolkits-0.1.7/datamini_toolkits/cmysql/prompts.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.6/datamini_toolkits/mock_data/agent.py` & `datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 from prompts import RECORD_CREATOR_PROMPT_TEMPLATE, TABLE_CREATOR_PROMPT_TEMPLATE, SCHEMA_DESIGNER_PROMPT_TEMPLATE
 from base import ChatOpenAIWithLog, SQLDatabaseWithLog
 from logs import log
 
 
 
 class DataMakerAgentCreator(object):
-    def __init__(self, db_uri):
+    def __init__(self, db_uri, openai_model_name="gpt-3.5-turbo"):
 
         self.db_uri = db_uri
 
         self.db = SQLDatabaseWithLog.from_uri(self.db_uri, sample_rows_in_table_info=2)
-
-        self.llm = ChatOpenAIWithLog(temperature=0, model_name="gpt-3.5-turbo", max_tokens=2000)
+        log.info('Using Model: %s' % openai_model_name)
+        self.llm = ChatOpenAIWithLog(temperature=0, model_name=openai_model_name, max_tokens=2000)
         self.llm.openai_proxy = os.environ.get("OPENAI_HTTP_PROXY", None)
         self.get_llm_callback = get_openai_callback
 
         self.db_chain = SQLDatabaseChain.from_llm(self.llm, self.db, verbose=True)
         memory = ConversationBufferMemory(memory_key="chat_history", return_messages=True)
 
         self.agent = initialize_agent(tools=self.tools,
```

### Comparing `datamini_toolkits-0.1.6/datamini_toolkits/mock_data/base.py` & `datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/base.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.6/datamini_toolkits/mock_data/cli.py` & `datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import argparse
-
 import sys,os
 sys.path.append(os.path.join(os.path.dirname(__file__)))
 
-print(sys.path)
 from agent import DataMakerAgentCreator
 from logs import log
 
 
 def get_args():
     parser = argparse.ArgumentParser(description='SQL Data Maker CLI', add_help=False)
 
@@ -20,15 +18,16 @@
     parser.add_argument('-u', '--user', dest='user', metavar='user', help='User for login')
     parser.add_argument('-p', '--password', dest='password', nargs='?', const='name',
                         help='Password to use when connecting to server. If password is not given, it\'s asked from the tty.')
     parser.add_argument('-P', '--port', dest='port', type=int, default=3306,
                         help='Port number to use for connection, default (3306).')
     parser.add_argument('--help', action='help',
                         help='Show this help message and exit.')  # 添加自定义的帮助选项
-
+    # 增加OpenAI 模型名称参数
+    parser.add_argument('-m', '--model', dest='model', metavar='model', default='gpt-3.5-turbo',  help='OpenAI Model Name')
     # 解析命令行参数
     args = parser.parse_args()
     return args
 
 
 def get_db_uri_from_args(args):
     db_host = args.host or "127.0.0.1"
@@ -42,15 +41,15 @@
 
 
 
 def main():
     args = get_args()
     db_uri = get_db_uri_from_args(args)
 
-    creator = DataMakerAgentCreator(db_uri)
+    creator = DataMakerAgentCreator(db_uri, openai_model_name=args.model)
 
     while True:
 
         # request = "生成一个看病挂号系统的数据库，并插入测试数据"
         request = input("""
 e.g. 创建一个考勤系统的数据库，并插入测试数据
      生成一个具有挂号、看病、开药、住院功能的医院系统的数据库，并插入测试数据
```

### Comparing `datamini_toolkits-0.1.6/datamini_toolkits/mock_data/logs.py` & `datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/logs.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.6/datamini_toolkits/mock_data/prompts.py` & `datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/prompts.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.6/datamini_toolkits/mock_data/test_tools.py` & `datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/test_tools.py`

 * *Files identical despite different names*

### Comparing `datamini_toolkits-0.1.6/datamini_toolkits/mock_data/tools.py` & `datamini_toolkits-0.1.7/datamini_toolkits/sql_data_maker/tools.py`

 * *Files identical despite different names*

