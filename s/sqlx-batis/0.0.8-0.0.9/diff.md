# Comparing `tmp/sqlx-batis-0.0.8.tar.gz` & `tmp/sqlx-batis-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.0.8.tar", last modified: Tue Jul 25 08:26:54 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-0.0.9.tar", last modified: Wed Jul 26 08:39:15 2023, max compression
```

## Comparing `sqlx-batis-0.0.8.tar` & `sqlx-batis-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/
--rw-rw-rw-   0        0        0     3401 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2920 2023-07-25 08:19:31.000000 sqlx-batis-0.0.8/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1209 2023-07-25 08:26:28.000000 sqlx-batis-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/sqlbatis/
--rw-rw-rw-   0        0        0      394 2023-07-23 23:51:01.000000 sqlx-batis-0.0.8/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     7935 2023-07-25 06:01:24.000000 sqlx-batis-0.0.8/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6141 2023-07-25 06:01:24.000000 sqlx-batis-0.0.8/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0      806 2023-07-23 23:51:27.000000 sqlx-batis-0.0.8/sqlbatis/exec_support.py
--rw-rw-rw-   0        0        0     3839 2023-07-24 13:45:51.000000 sqlx-batis-0.0.8/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    39064 2023-07-25 08:11:50.000000 sqlx-batis-0.0.8/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     2402 2023-07-25 04:27:05.000000 sqlx-batis-0.0.8/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.0.8/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     4126 2023-07-23 23:51:27.000000 sqlx-batis-0.0.8/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1421 2023-07-23 14:00:47.000000 sqlx-batis-0.0.8/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      354 2023-07-23 22:35:05.000000 sqlx-batis-0.0.8/sqlbatis/support.py
--rw-rw-rw-   0        0        0      690 2023-07-25 06:01:24.000000 sqlx-batis-0.0.8/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.0.8/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3401 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      471 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-07-25 08:26:54.000000 sqlx-batis-0.0.8/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/
+-rw-rw-rw-   0        0        0     3373 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2892 2023-07-26 08:34:15.000000 sqlx-batis-0.0.9/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1209 2023-07-26 08:38:48.000000 sqlx-batis-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/sqlbatis/
+-rw-rw-rw-   0        0        0      782 2023-07-26 05:51:44.000000 sqlx-batis-0.0.9/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     6894 2023-07-26 08:13:40.000000 sqlx-batis-0.0.9/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6234 2023-07-26 04:35:24.000000 sqlx-batis-0.0.9/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0     1391 2023-07-26 08:20:25.000000 sqlx-batis-0.0.9/sqlbatis/engin.py
+-rw-rw-rw-   0        0        0     2324 2023-07-26 05:27:34.000000 sqlx-batis-0.0.9/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    34936 2023-07-26 06:54:32.000000 sqlx-batis-0.0.9/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.0.9/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.0.9/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     4939 2023-07-26 06:52:58.000000 sqlx-batis-0.0.9/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1646 2023-07-26 05:39:42.000000 sqlx-batis-0.0.9/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.0.9/sqlbatis/support.py
+-rw-rw-rw-   0        0        0      779 2023-07-26 07:56:33.000000 sqlx-batis-0.0.9/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 23:08:12.000000 sqlx-batis-0.0.9/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3373 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      464 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 08:39:15.000000 sqlx-batis-0.0.9/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.0.8/PKG-INFO` & `sqlx-batis-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.0.8
+Version: 0.0.9
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -56,15 +56,15 @@
    def query_all(): List(Mapping)
 
    @sql('select id, name, age from person where name=?')
    def query_by_name(name: str): List(Mapping)
 
 
    if __name__ == '__main__':
-       dbx.init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, mapper_path='./mapper', engin=Engin.PostgreSQL)
+       init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, mapper_path='./mapper')
        
        persons = select_all()
        # result:
        # (3, 'zhangsan', 15)
        # (4, 'lisi', 26)
        # (5, 'wangwu', 38)
```

### Comparing `sqlx-batis-0.0.8/README.rst` & `sqlx-batis-0.0.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
    def query_all(): List(Mapping)
 
    @sql('select id, name, age from person where name=?')
    def query_by_name(name: str): List(Mapping)
 
 
    if __name__ == '__main__':
-       dbx.init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, mapper_path='./mapper', engin=Engin.PostgreSQL)
+       init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, mapper_path='./mapper')
        
        persons = select_all()
        # result:
        # (3, 'zhangsan', 15)
        # (4, 'lisi', 26)
        # (5, 'wangwu', 38)
```

### Comparing `sqlx-batis-0.0.8/setup.py` & `sqlx-batis-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     name='sqlx-batis',
     packages=['sqlbatis'],
     description="sqlx-batis is a sql executor for Python like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'sqlx-exec>=1.1.6',
+        'sqlx-exec>=1.2.0',
     ],
-    version='0.0.8',
+    version='0.0.9',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.0.8/sqlbatis/db.py` & `sqlx-batis-0.0.9/sqlbatis/db.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from . import sql_support
-from .log_support import sql_log, page_log, do_sql_log
+from .log_support import sql_log, do_sql_log
 
 # Don't remove. Import for not repetitive implementation
-from sqlexec import insert, save, batch_insert, batch_execute, execute as supper_execute, get as supper_get, query_one as supper_query_one, \
-    query as supper_query, query_page as supper_query_page, select as supper_select, select_one as supper_select_one, select_page as supper_select_page
+from sqlexec import insert, save, save_sql, batch_insert, batch_execute, execute as supper_execute, get as supper_get, query_one as supper_query_one,\
+    query as supper_query, select as supper_select, select_one as supper_select_one
 
 
 # ----------------------------------------------------------Update function------------------------------------------------------------------
 def execute(sql: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO user(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
@@ -76,36 +76,14 @@
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_log('select_one', sql, *args, **kwargs)
     sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
     return do_select_one(sql, *args)
 
 
-def query_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
-    """
-    Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-         SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-    """
-    page_log('query_page', sql, page_num, page_size, *args, **kwargs)
-    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
-    return do_query_page(sql, page_num, page_size, *args)
-
-
-def select_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
-    """
-    Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-         SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-    """
-    page_log('select_page', sql, page_num, page_size, *args, **kwargs)
-    sql, args = sql_support.dynamic_sql(sql, *args, **kwargs)
-    return do_select_page(sql, page_num, page_size, *args)
-
-
 # ----------------------------------------------------------Do function------------------------------------------------------------------
 def do_execute(sql: str, *args):
     """
     Execute sql return effect rowcount
     sql: insert into user(name, age) values(?, ?)  -->  args: ('张三', 20)
     """
     return supper_execute(sql, *args)
@@ -154,21 +132,25 @@
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     do_sql_log('do_select_one', sql, *args)
     sql, args = sql_support.limit_one_sql_args(sql, *args)
     return supper_select_one(sql, *args)
 
 
-def do_query_page(sql: str, page_num=1, page_size=10, *args):
-    """
-    Execute select SQL and return list results(dict).
-    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-    """
-    return supper_query_page(sql, page_num, page_size, *args)
-
-
-def do_select_page(sql: str, page_num=1, page_size=10, *args):
-    """
-    Execute select SQL and return list results(dict).
-    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-    """
-    return supper_select_page(sql, page_num, page_size, *args)
+# def do_query_page(sql: str, page_num=1, page_size=10, *args):
+#     """
+#     Execute select SQL and return list results(dict).
+#     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+#     """
+#     do_page_log('select_page', sql.strip(), page_num, page_size, args)
+#     sql, args = sql_support.page_sql_args(sql, page_num, page_size, *args)
+#     return supper_query(sql, *args)
+
+
+# def do_select_page(sql: str, page_num=1, page_size=10, *args):
+#     """
+#     Execute select SQL and return list results(dict).
+#     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
+#     """
+#     do_page_log('do_select_page', sql.strip(), page_num, page_size, args)
+#     sql, args = sql_support.page_sql_args(sql, page_num, page_size, *args)
+#     return supper_select(sql, *args)
```

### Comparing `sqlx-batis-0.0.8/sqlbatis/dbx.py` & `sqlx-batis-0.0.9/sqlbatis/dbx.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from .exec_support import do_save
 from .sql_support import get_batch_args
 from . import Engin, sql_holder as holder
-from .log_support import logger, sql_id_log, page_sql_id_log
+from .log_support import logger, sql_id_log
 
 # Don't remove. Import for not repetitive implementation
-from .db import(do_execute, insert, batch_insert, batch_execute as db_batch_execute, do_get, do_query, do_query_one, do_query_page, do_select, \
-                do_select_one, do_select_page)
+from .db import(do_execute, insert, save_sql, batch_insert, batch_execute as db_batch_execute, do_get, do_query, do_query_one, do_select, do_select_one)
 
 
 def save(sql_id: str, *args, **kwargs):
     """
     Execute insert SQL, return primary key.
     :return: Primary key
     """
     sql_id_log('dbx.save', sql_id, *args, **kwargs)
     sql_model = holder.get_sql_model(sql_id)
-    return do_save(sql_model, False, None, *args, **kwargs)
+    sql, args = holder.get_sql(sql_id, *args, **kwargs)
+    select_key = sql_model.select_key
+    if not select_key:
+        select_key = Engin.get_select_key()
+    return save_sql(select_key, sql, *args)
 
 
 def execute(sql_id: str, *args, **kwargs):
     """
     Execute SQL.
     sql: INSERT INTO person(name, age) VALUES(?, ?)  -->  args: ('张三', 20)
          INSERT INTO person(name, age) VALUES(:name,:age)  -->  kwargs: {'name': '张三', 'age': 20}
@@ -100,28 +102,28 @@
          SELECT * FROM person WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql_id_log('select_one', sql_id, *args, **kwargs)
     sql, args = holder.get_sql(sql_id, *args, **kwargs)
     return do_select_one(sql, *args)
 
 
-def query_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
-    """
-    Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-         SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-    """
-    page_sql_id_log('query_page', sql_id, page_num, page_size, *args, **kwargs)
-    sql, args = holder.get_sql(sql_id, *args, **kwargs)
-    return do_query_page(sql, page_num, page_size, *args)
-
-
-def select_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
-    """
-    Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
-    sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
-         SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
-    """
-    page_sql_id_log('select_page', sql_id, page_num, page_size, *args, **kwargs)
-    sql, args = holder.get_sql(sql_id, *args, **kwargs)
-    return do_select_page(sql, page_num, page_size, *args)
+# def query_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
+#     """
+#     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
+#     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+#          SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+#     """
+#     page_sql_id_log('query_page', sql_id, page_num, page_size, *args, **kwargs)
+#     sql, args = holder.get_sql(sql_id, *args, **kwargs)
+#     return do_query_page(sql, page_num, page_size, *args)
+
+
+# def select_page(sql_id: str, page_num=1, page_size=10, *args, **kwargs):
+#     """
+#     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
+#     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
+#          SELECT * FROM person WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
+#     """
+#     page_sql_id_log('select_page', sql_id, page_num, page_size, *args, **kwargs)
+#     sql, args = holder.get_sql(sql_id, *args, **kwargs)
+#     return do_select_page(sql, page_num, page_size, *args)
```

### Comparing `sqlx-batis-0.0.8/sqlbatis/orm.py` & `sqlx-batis-0.0.9/sqlbatis/orm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import sys
-import sqlexec
+from .engin import Engin
 from datetime import datetime
 from enum import Enum, IntEnum
-from functools import lru_cache
 from .sql_support import simple_sql
 from .snowflake import get_snowflake_id
+from . import db, log_support, transaction
 from .support import DBError, NotFoundError
 from typing import Sequence, Union, List, Tuple
-from . import db, log_support, transaction, DBEngin
-from .constant import LIMIT_1, NO_LIMIT, DEFAULT_KEY_FIELD, KEY, KEY_SEQ, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY, CACHE_SIZE
+from .constant import LIMIT_1, NO_LIMIT, DEFAULT_KEY_FIELD, KEY, SELECT_KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY
 
 
 class DelFlag(IntEnum):
     UN_DELETE = 0
     DELETED = 1
 
 
@@ -184,36 +183,38 @@
         return: Effect rowcount
         """
         log_support.orm_insert_log('insert', cls.__name__, **kwargs)
         key, table = cls._get_key_and_table()
         key_strategy = cls._get_key_strategy()
         if key_strategy == KeyStrategy.SNOWFLAKE and key not in kwargs:
             kwargs[key] = get_snowflake_id()
-        return sqlexec.insert(table, **kwargs)
+        return db.insert(table, **kwargs)
 
     @classmethod
     def save(cls, **kwargs):
         """
         id = Person.save(name='张三', age=20)
         :return: Primary key
         """
         log_support.orm_insert_log('save', cls.__name__, **kwargs)
         key, table = cls._get_key_and_table()
         if key in kwargs:
-            sqlexec.insert(table, **kwargs)
+            db.insert(table, **kwargs)
             return kwargs[key]
 
         key_strategy = cls._get_key_strategy()
         if key_strategy == KeyStrategy.SNOWFLAKE:
             kwargs[key] = get_snowflake_id()
-            sqlexec.insert(table, **kwargs)
+            db.insert(table, **kwargs)
             return kwargs[key]
         else:
-            key_seq = cls._get_key_seq()
-            return sqlexec.save(DBEngin.get_select_key(key_seq=key_seq), table, **kwargs)
+            select_key = cls._get_select_key()
+            if not select_key:
+                select_key = Engin.get_select_key(table=table)
+            return db.save(select_key, table, **kwargs)
 
     @classmethod
     def create(cls, **kwargs):
         """
         person = Person.create(name='张三', age=20)
         :return: Instance object
         """
@@ -232,15 +233,15 @@
         assert kwargs, 'Must set update kv'
         key = cls._get_key()
         where = '%s = ?' % key
         cols, args = zip(*kwargs.items())
         sql, update_time_arg = cls._update_sql(where, *cols)
         if update_time_arg:
             args = [*args, update_time_arg]
-        return sqlexec.execute(sql, *args, _id)
+        return db.do_execute(sql, *args, _id)
 
     @classmethod
     def logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
         """
         Logic delete only update the del flag
         rowcount = Person.delete_by_id(id=1, update_by=100)
         return: Effect rowcount
@@ -286,27 +287,27 @@
         return: Effect rowcount
         """
         log_support.orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         assert where.lower().startswith('where'), "Must start with 'WHERE' in the where parameter."
         table = cls._get_table()
         sql = 'DELETE FROM %s %s' % (table, where)
         sql, args = simple_sql(sql, *args, **kwargs)
-        return sqlexec.execute(sql, *args)
+        return db.do_execute(sql, *args)
 
     @classmethod
     def delete_by_id(cls, _id: Union[int, str]):
         """
         Physical delete
         rowcount = Person.delete_by_id(id=1)
         return: Effect rowcount
         """
         log_support.logger.debug("Exec func 'sqlbatis.orm.Model.%s' \n\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
         key, table = cls._get_key_and_table()
         sql = 'DELETE FROM %s WHERE %s = ?' % (table, key)
-        return sqlexec.execute(sql, _id)
+        return db.do_execute(sql, _id)
 
     @classmethod
     def delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], batch_size=128):
         """
         Batch physical delete, they will be executed in batches if there are too many
         rowcount = Person.delete_by_ids(id=[1,2])
         return: Effect rowcount
@@ -330,15 +331,15 @@
         Batch physical delete, please use delete_by_ids if there are too many
         rowcount = Person.do_delete_by_ids(id=[1,2])
         return: Effect rowcount
         """
         ids_size = len(ids)
         key, table = cls._get_key_and_table()
         sql = 'DELETE FROM {} WHERE {} in ({})'.format(table, key, ','.join(['?' for _ in range(ids_size)]))
-        return sqlexec.execute(sql, *ids)
+        return db.do_execute(sql, *ids)
 
     @classmethod
     def batch_insert(cls, *args):
         """
         Batch insert
         rowcount = Person.batch_insert([{'name': '张三', 'age': 55},{'name': '李四', 'age': 66}])
         :param args: All number must have same key.
@@ -349,49 +350,49 @@
         key, table = cls._get_key_and_table()
         key_strategy = cls._get_key_strategy()
         if key_strategy == KeyStrategy.SNOWFLAKE:
             for arg in args:
                 if key not in arg:
                     arg[key] = get_snowflake_id()
 
-        return sqlexec.batch_insert(table, *args)
+        return db.batch_insert(table, *args)
 
     # ------------------------------------------------Class query method--------------------------------------------------------
     @classmethod
     def count(cls, **kwargs):
         """
         count = Person.count(name='张三', age=55)
         """
         log_support.orm_count_log('count', cls.__name__, **kwargs)
         table = cls._get_table()
-        where, args, _ = _get_where_arg_limit(**kwargs)
+        where, args, _ = get_where_arg_limit(**kwargs)
         fields = 'count(1)'
-        sql = _select_sql(table, where, LIMIT_1, fields)
-        return sqlexec.get(sql, *args, LIMIT_1)
+        sql = select_sql(table, where, LIMIT_1, fields)
+        return db.do_get(sql, *args, LIMIT_1)
 
     @classmethod
     def count_by(cls, where: str, *args, **kwargs):
         """
         Automatically add 'limit ?' where if not.
         count = Person.count_by('where name=?', '李四')
         """
         log_support.orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         assert where.lower().startswith('where'), "Must start with 'where' in the where parameter."
         table = cls._get_table()
         sql = "SELECT count(1) FROM {} {}".format(table, where)
         sql, args = simple_sql(sql, *args, **kwargs)
-        return sqlexec.get(sql, *args)
+        return db.do_get(sql, *args)
 
     @classmethod
     def exists(cls, **kwargs):
         log_support.orm_count_log('exists', cls.__name__, **kwargs)
         table = cls._get_table()
-        where, args, _ = _get_where_arg_limit(**kwargs)
+        where, args, _ = get_where_arg_limit(**kwargs)
         sql = "SELECT 1 FROM {} {} limit ?".format(table, where)
-        return sqlexec.get(sql, *args, LIMIT_1) == 1
+        return db.do_get(sql, *args, LIMIT_1) == 1
 
     @classmethod
     def exists_by(cls, where: str, *args, **kwargs):
         log_support.orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         assert where.lower().startswith('where'), "Must start with 'where' in the where parameter."
         table = cls._get_table()
         sql = "SELECT 1 FROM {} {}".format(table, where)
@@ -425,36 +426,14 @@
         Return list(dict) or empty list if no result.
         rows = Person.find_by('where name=?', '李四')
         """
         log_support.orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         return [cls.to_obj(**d) for d in cls.query_by(where, *args, **kwargs)]
 
     @classmethod
-    def find_page(cls, page_num=1, page_size=10, *fields, **kwargs):
-        """
-        Return list(object) or empty list if no result.
-        persons = Person.find_page(1, 10, 'name', 'age', name='张三', age=55)
-        :param page_num: page number
-        :param page_size: page size
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_page_log('find_page', page_num, page_size, cls.__name__, *fields, **kwargs)
-        result = cls.query_page(page_num, page_size, *fields, **kwargs)
-        return [cls.to_obj(**d) for d in result]
-
-    @classmethod
-    def find_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
-        """
-        Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
-        rows = Person.find_by_page(1, 10, 'where name=?', '李四')
-        """
-        log_support.orm_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
-        return [cls.to_obj(**d) for d in cls.query_page_by(page_num, page_size, where, *args, **kwargs)]
-
-    @classmethod
     def find_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one class object or None if no result.
         person = Person.find_by_id(1, 'id', 'name', 'age')
         :param _id: key
         :param fields: Default select all fields if not set
         """
@@ -477,87 +456,61 @@
     def query(cls, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         persons = Person.query('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_log('query', cls.__name__, *fields, **kwargs)
-        where, args, limit = _get_where_arg_limit(**kwargs)
+        where, args, limit = get_where_arg_limit(**kwargs)
         table = cls._get_table()
-        sql = _select_sql(table, where, limit, *fields)
+        sql = select_sql(table, where, limit, *fields)
         if limit:
             if isinstance(limit, int):
                 args = [*args, limit]
             else:
                 args = [*args, *limit]
-        return sqlexec.query(sql, *args)
+        return db.do_query(sql, *args)
 
     @classmethod
     def query_one(cls, *fields, **kwargs):
         """
         Return unique result(dict) or None if no result.
         persons = Person.query_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_log('query_one', cls.__name__, *fields, **kwargs)
-        where, args, _ = _get_where_arg_limit(**kwargs)
+        where, args, _ = get_where_arg_limit(**kwargs)
         table = cls._get_table()
-        sql = _select_sql(table, where, LIMIT_1, *fields)
-        return sqlexec.query_one(sql, *args, LIMIT_1)
+        sql = select_sql(table, where, LIMIT_1, *fields)
+        return db.do_query_one(sql, *args, LIMIT_1)
 
     @classmethod
     def query_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.query_by('where name=?', '李四')
         """
         log_support.orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
-        return sqlexec.query(sql, *args)
-
-    @classmethod
-    def query_page(cls, page_num=1, page_size=10, *fields, **kwargs):
-        """
-        Return list(dict) or empty list if no result.
-        persons = Person.query_page(1, 10, 'id', 'name', 'age', name='张三', age=55)
-        :param page_num: page number
-        :param page_size: page size
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
-        table = cls._get_table()
-        where, args, _ = _get_where_arg_limit(**kwargs)
-        sql = _select_sql(table, where, NO_LIMIT, *fields)
-        return sqlexec.query_page(sql, page_num, page_size, *args)
-
-    @classmethod
-    def query_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
-        """
-        Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
-        rows = Person.query_by_page(1, 10, 'where name=?', '李四')
-        """
-        log_support.orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
-        sql = cls._where_sql(where)
-        sql, args = simple_sql(sql, *args, **kwargs)
-        return sqlexec.query_page(sql, page_num, page_size, *args)
+        return db.do_query(sql, *args)
 
     @classmethod
     def query_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one row(dict) or None if no result.
         person = Person.query_by_id(1, 'id', 'name', 'age')
         :param _id: key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_id_log('query_by_id', cls.__name__, _id, *fields)
         key, table = cls._get_key_and_table()
         where = 'WHERE {} = ?'.format(key)
-        sql = _select_sql(table, where, LIMIT_1, *fields)
-        return sqlexec.query_one(sql, _id, LIMIT_1)
+        sql = select_sql(table, where, LIMIT_1, *fields)
+        return db.do_query_one(sql, _id, LIMIT_1)
 
     @classmethod
     def query_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         persons = Person.query_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of key
@@ -565,98 +518,72 @@
         """
         log_support.orm_find_by_ids_log('query_by_ids', cls.__name__, ids, *fields)
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
         key, table = cls._get_key_and_table()
         where = 'WHERE {} in ({})'.format(key, ','.join(['?' for _ in range(ids_size)]))
-        sql = _select_sql(table, where, ids_size, *fields)
-        return sqlexec.query(sql, *ids, ids_size)
+        sql = select_sql(table, where, ids_size, *fields)
+        return db.do_query(sql, *ids, ids_size)
 
     @classmethod
     def select(cls, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.select('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_log('select', cls.__name__, *fields, **kwargs)
-        where, args, limit = _get_where_arg_limit(**kwargs)
+        where, args, limit = get_where_arg_limit(**kwargs)
         table = cls._get_table()
-        sql = _select_sql(table, where, limit, *fields)
+        sql = select_sql(table, where, limit, *fields)
         if limit:
             if isinstance(limit, int):
                 args = [*args, limit]
             else:
                 args = [*args, *limit]
-        return sqlexec.select(sql, *args)
+        return db.do_select(sql, *args)
 
     @classmethod
     def select_one(cls, *fields, **kwargs):
         """
         Return unique result(tuple) or None if no result.
         row = Person.select_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_log('select_one', cls.__name__, *fields, **kwargs)
-        where, args, _ = _get_where_arg_limit(**kwargs)
+        where, args, _ = get_where_arg_limit(**kwargs)
         table = cls._get_table()
-        sql = _select_sql(table, where, LIMIT_1, *fields)
-        return sqlexec.select_one(sql, *args, LIMIT_1)
+        sql = select_sql(table, where, LIMIT_1, *fields)
+        return db.do_select_one(sql, *args, LIMIT_1)
 
     @classmethod
     def select_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.select_by('where name=?', '李四')
         """
         log_support.orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         sql = cls._where_sql(where)
         sql, args = simple_sql(sql, *args, **kwargs)
-        return sqlexec.select(sql, *args)
-
-    @classmethod
-    def select_page(cls, page_num=1, page_size=10, *fields, **kwargs):
-        """
-        Return list(dict) or empty list if no result.
-        rows = Person.select_page('id', 'name', 'age', name='张三', age=55)
-        :param page_num: page number
-        :param page_size: page size
-        :param fields: Default select all fields if not set
-        """
-        log_support.orm_page_log('select_page', page_num, page_size, cls.__name__, *fields, **kwargs)
-        table = cls._get_table()
-        where, args, _ = _get_where_arg_limit(**kwargs)
-        sql = _select_sql(table, where, NO_LIMIT, *fields)
-        return sqlexec.select_page(sql, page_num, page_size, *args)
-
-    @classmethod
-    def select_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
-        """
-        Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
-        rows = Person.select_by_page(1, 10, 'where name=?', '李四')
-        """
-        log_support.orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
-        sql = cls._where_sql(where)
-        sql, args = simple_sql(sql, *args, **kwargs)
-        return sqlexec.select_page(sql, page_num, page_size, *args)
+        return db.do_select(sql, *args)
 
     @classmethod
     def select_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one row(dict) or None if no result.
         row = Person.select_by_id(1, 'id', 'name', 'age')
         :param _id: key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_id_log('select_by_id', cls.__name__, _id, *fields)
         key, table = cls._get_key_and_table()
         where = 'WHERE {} = ?'.format(key)
-        sql = _select_sql(table, where, LIMIT_1, *fields)
-        return sqlexec.select_one(sql, _id, LIMIT_1)
+        sql = select_sql(table, where, LIMIT_1, *fields)
+        return db.do_select_one(sql, _id, LIMIT_1)
 
     @classmethod
     def select_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         rows = Person.select_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of key
@@ -664,16 +591,16 @@
         """
         log_support.orm_find_by_ids_log('select_by_ids', cls.__name__, ids, *fields)
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
         key, table = cls._get_key_and_table()
         where = 'WHERE {} in ({})'.format(key, ','.join(['?' for _ in range(ids_size)]))
-        sql = _select_sql(table, where, ids_size, *fields)
-        return sqlexec.select(sql, *ids, ids_size)
+        sql = select_sql(table, where, ids_size, *fields)
+        return db.do_select(sql, *ids, ids_size)
 
     @classmethod
     def to_obj(cls, **kwargs):
         model = cls.__new__(cls)
         model.__dict__.update(**kwargs)
         return model
 
@@ -696,21 +623,21 @@
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
         where = '%s = ?' % key
         if update_by is not None and update_by_field is not None:
             sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
             if update_time_arg:
-                return sqlexec.execute(sql, del_status.value, update_by, update_time_arg, _id)
-            return sqlexec.execute(sql, del_status.value, update_by, _id)
+                return db.do_execute(sql, del_status.value, update_by, update_time_arg, _id)
+            return db.do_execute(sql, del_status.value, update_by, _id)
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
             if update_time_arg:
-                return sqlexec.execute(sql, del_status.value, update_time_arg, _id)
-            return sqlexec.execute(sql, del_status.value, _id)
+                return db.do_execute(sql, del_status.value, update_time_arg, _id)
+            return db.do_execute(sql, del_status.value, _id)
 
     @classmethod
     def _logical_delete_by_ids_op(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128,
             del_status=DelFlag.DELETED):
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
@@ -730,36 +657,34 @@
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
         where = '%s in (%s)' % (key, ','.join(['?' for _ in range(len(ids))]))
         if update_by is not None and update_by_field is not None:
             sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
             if update_time_arg:
-                return sqlexec.execute(sql, del_status.value, update_by, update_time_arg, *ids)
-            return sqlexec.execute(sql, del_status.value, update_by, *ids)
+                return db.do_execute(sql, del_status.value, update_by, update_time_arg, *ids)
+            return db.do_execute(sql, del_status.value, update_by, *ids)
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
             if update_time_arg:
-                return sqlexec.execute(sql, del_status.value, update_time_arg, *ids)
-            return sqlexec.execute(sql, del_status.value, *ids)
+                return db.do_execute(sql, del_status.value, update_time_arg, *ids)
+            return db.do_execute(sql, del_status.value, *ids)
 
     @classmethod
     def _get_key(cls):
         if hasattr(cls, KEY):
             return cls.__key__
         log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, KEY))
         return DEFAULT_KEY_FIELD
 
     @classmethod
-    def _get_key_seq(cls):
-        if hasattr(cls, KEY_SEQ):
-            return cls.__key_seq__
-        log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, KEY_SEQ))
-        key, table = cls._get_key_and_table()
-        return "{}_{}_seq".format(table, key)
+    def _get_select_key(cls):
+        if hasattr(cls, SELECT_KEY):
+            return cls.__select_key__
+        return None
 
     @classmethod
     def _get_table(cls):
         if hasattr(cls, TABLE):
             return cls.__table__
         log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, TABLE))
         return _get_table_name(cls.__name__)
@@ -804,43 +729,38 @@
         return 'UPDATE {} SET {} WHERE {}'.format(table, update_fields, where), update_time_arg
 
     @classmethod
     def _where_sql(cls, where: str):
         low_where = where.lower()
         if low_where.startswith('where'):
             table = cls._get_table()
-            return _select_sql(table, where, NO_LIMIT)
+            return select_sql(table, where, NO_LIMIT)
         elif low_where.startswith('select'):
             return where
         raise DBError("The where parameter must be a complete SQL statement or conditions start with 'where'")
 
 
 # ----------------------------------------------------------Private function------------------------------------------------------------------
-def _select_sql(table: str, where: str, limit: Union[int, Tuple[int], List[int]], *fields):
+def select_sql(table: str, where: str, limit: Union[int, Tuple[int], List[int]], *fields):
     if fields:
         fields = ','.join([col if '(' in col else '{}'.format(col) for col in fields])
     else:
-        fields = _get_table_columns(table)
+        fields = Engin.get_table_columns(table)
 
     if limit:
         if isinstance(limit, int):
             return 'SELECT {} FROM {} {} LIMIT ?'.format(fields, table, where)
         elif (isinstance(limit, Tuple) or isinstance(limit, List)) and len(limit) == 2:
             return 'SELECT {} FROM {} {} LIMIT ? OFFSET ?'.format(fields, table, where)
         else:
             raise ValueError("The type of the parameter 'limit' must be 'int' or tuple, list, and it length is 2.")
     else:
         return 'SELECT {} FROM {} {}'.format(fields, table, where)
 
 
-@lru_cache(maxsize=CACHE_SIZE)
-def _get_table_columns(table: str):
-    return sqlexec.get(DBEngin.get_column_sql(), table, LIMIT_1)
-
-
 def _get_condition_arg(k: str, v: object):
     if k.endswith("__eq"):
         return "{} = ?".format(k[:-4]), v
     if k.endswith("__ne"):
         return "{} != ?".format(k[:-4]), v
     if k.endswith("__gt"):
         return "{} > ?".format(k[:-4]), v
@@ -879,15 +799,15 @@
         return "{} between ? and ?".format(k[:-9]), v
     if k.endswith("__range") or k.endswith("__between"):
         return ValueError("Must is instance of Sequence with length 2 when use range or between statement")
 
     return "{} = ?".format(k), v
 
 
-def _get_where_arg_limit(**kwargs):
+def get_where_arg_limit(**kwargs):
     where, args, limit = '', [], 0
     if 'limit' in kwargs:
         limit = kwargs.pop('limit')
 
     if kwargs:
         conditions, tmp_args = zip(*[_get_condition_arg(k, v) for k, v in kwargs.items()])
         tmp_args = [arg for arg in tmp_args if arg is not None]
```

### Comparing `sqlx-batis-0.0.8/sqlbatis/snowflake.py` & `sqlx-batis-0.0.9/sqlbatis/snowflake.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-from .support import DB_LOCK
+from sqlexec.support import DB_LOCK
 
 _SNOWFLAKE = None
 _WORKER_BITS = 10
 _SEQUENCE_BITS = 12
 _EPOCH = 1688140800000
 # _SEQUENCE_MASK = 4095
```

### Comparing `sqlx-batis-0.0.8/sqlbatis/sql_holder.py` & `sqlx-batis-0.0.9/sqlbatis/sql_holder.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.0.8/sqlbatis/sql_mapper.py` & `sqlx-batis-0.0.9/sqlbatis/sql_mapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,83 +1,94 @@
 import os
 import sqlexec
 import functools
+from .engin import Engin
 from .support import SqlAction
 from .log_support import logger
-from .exec_support import do_save, do_save0
 from .sql_support import simple_sql, get_named_sql_args
 from .sql_holder import get_sql_model, do_get_sql, build_sql_id
 
 _UPDATE_ACTIONS = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.CALL.value)
 
 
-def mapper(namespace: str = None, sql_id: str = None, batch=False, return_key=False):
+def mapper(namespace: str = None, sql_id: str = None, batch=False, return_key=False, select_key=None):
     def _decorator(func):
         @functools.wraps(func)
         def _wrapper(*args, **kwargs):
             param_names = func.__code__.co_varnames
-            full_sql_id, func_name = _before(func, namespace, sql_id, *args, **kwargs)
+            full_sql_id, func_name = before(func, namespace, sql_id, *args, **kwargs)
             sql_model = get_sql_model(full_sql_id)
-            exec_func = _get_exec_func(func, sql_model.action, batch)
+            exec_func = get_exec_func(func, sql_model.action, batch)
             if return_key:
-                return do_save(sql_model, batch, param_names, *args, **kwargs)
+                use_select_key = select_key
+                use_sql, args = do_get_sql(sql_model,  batch, param_names, *args, **kwargs)
+                if use_select_key is None:
+                    use_select_key = sql_model.select_key
+                    if use_select_key is None:
+                        use_select_key = Engin.get_select_key(sql=use_sql)
+                assert use_select_key, "'selectKey' should not be None in sql_id: '{}'".format(full_sql_id)
+                return sqlexec.save_sql(use_select_key, use_sql, *args)
             if batch:
                 if kwargs:
                     logger.warning("Batch exec sql better use like '{}(args)' or '{}(*args)' then '{}(args=args)'".format(func_name, func_name, func_name))
                     args = list(kwargs.values())[0]
                 use_sql, _ = do_get_sql(sql_model, batch, param_names, *args)
             else:
                 use_sql, args = do_get_sql(sql_model, batch, param_names, *args, **kwargs)
             return exec_func(use_sql, *args)
 
         return _wrapper
     return _decorator
 
 
-def sql(value: str, batch=False, return_key=False, select_key=None, key_seq=None):
+def sql(value: str, batch=False, return_key=False, select_key=None):
     def _decorator(func):
         @functools.wraps(func)
         def _wrapper(*args, **kwargs):
             use_sql = value
             low_sql = value.lower()
             if any([action in low_sql for action in _UPDATE_ACTIONS]):
                 if batch:
                     if kwargs:
                         args = list(kwargs.values())[0]
                     return sqlexec.batch_execute(use_sql, *args)
                 if return_key:
+                    use_select_key = select_key
+                    if use_select_key is None:
+                        use_select_key = Engin.get_select_key(sql=use_sql)
+                    assert use_select_key, "'select_key' should not be None in func '{}' at file: '{}' line {}.".format(func.__name__, func.__code__.co_filename, func.__code__.co_firstlineno)
                     assert SqlAction.INSERT.value in low_sql, 'Only insert sql can return primary key.'
                     if kwargs:
                         use_sql, args = get_named_sql_args(use_sql, **kwargs)
-                    return do_save0(select_key, key_seq, use_sql, *args)
+                    return sqlexec.save_sql(use_select_key, use_sql, *args)
 
                 if kwargs:
                     use_sql, args = get_named_sql_args(use_sql, **kwargs)
                 return sqlexec.execute(use_sql, *args)
             elif SqlAction.SELECT.value in low_sql:
-                select_func = _get_select_func(func)
+                select_func = get_select_func(func)
                 use_sql, args = simple_sql(use_sql, *args, **kwargs)
                 return select_func(use_sql, *args)
             else:
                 return ValueError("Invalid sql: {}.".format(sql))
 
         return _wrapper
     return _decorator
 
 
-def _get_exec_func(func, action, batch):
+def get_exec_func(func, action, batch):
     if action == SqlAction.SELECT.value:
-        return _get_select_func(func)
+        return get_select_func(func)
     elif batch:
         return sqlexec.batch_execute
     else:
         return sqlexec.execute
 
 
-def _get_select_func(func):
+def get_select_func(func):
     names = func.__code__.co_names
     is_list = 'list' in names or 'List' in names
     if 'Mapping' in names and is_list:
         return sqlexec.query
     elif 'Mapping' in names:
         return sqlexec.query_one
     elif len(names) == 1 and names[0] in ('int', 'float', 'Decimal', 'str', 'AnyStr', 'date', 'time', 'datetime'):
@@ -86,15 +97,15 @@
         return sqlexec.select_one
     elif is_list:
         return sqlexec.select
     else:
         return sqlexec.query
 
 
-def _before(func, namespace, _id, *args, **kwargs):
+def before(func, namespace, _id, *args, **kwargs):
     file_name = os.path.basename(func.__code__.co_filename)[:-3]
     _namespace = namespace if namespace else file_name
     _id = _id if _id else func.__name__
     sql_id = build_sql_id(_namespace, _id)
     func_name = file_name + '.' + func.__name__
     logger.debug("Exec mapper func: '%s', sql_id: '%s', args: %s, kwargs: %s" % (func_name, sql_id, args, kwargs))
     return sql_id, func_name
```

### Comparing `sqlx-batis-0.0.8/sqlbatis/sql_support.py` & `sqlx-batis-0.0.9/sqlbatis/sql_support.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 from jinja2 import Template
 from functools import lru_cache
 from .support import MapperError
 from .constant import LIMIT_1, DYNAMIC_REGEX, CACHE_SIZE
+
 # Don't remove. Import for not repetitive implementation
-from sqlexec.sql_support import require_limit, get_named_args, get_named_sql, get_batch_args
+from sqlexec.sql_support import get_named_args, get_named_sql, get_batch_args
 
 
 def simple_sql(sql: str, *args, **kwargs):
     return get_named_sql_args(sql, **kwargs) if kwargs else (sql, args)
 
 
 def dynamic_sql(sql: str, *args, **kwargs):
@@ -33,14 +34,24 @@
 
 
 def get_named_sql_args(sql: str, **kwargs):
     args = get_named_args(sql, **kwargs)
     return get_named_sql(sql), args
 
 
+def require_limit(sql: str):
+    lower_sql = sql.lower()
+    if 'limit' not in lower_sql:
+        return True
+    idx = lower_sql.rindex('limit')
+    if idx > 0 and ')' in lower_sql[idx:]:
+        return True
+    return False
+
+
 @lru_cache(maxsize=2*CACHE_SIZE)
 def _get_sql_type(sql: str):
     """
     :return: 0: placeholder, 1: dynamic, 2: named mapping
     """
     if is_dynamic_sql(sql):
         return 1
```

### Comparing `sqlx-batis-0.0.8/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-0.0.9/sqlx_batis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.0.8
+Version: 0.0.9
 Summary: sqlx-batis is a sql executor for Python like MyBatis.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -56,15 +56,15 @@
    def query_all(): List(Mapping)
 
    @sql('select id, name, age from person where name=?')
    def query_by_name(name: str): List(Mapping)
 
 
    if __name__ == '__main__':
-       dbx.init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, mapper_path='./mapper', engin=Engin.PostgreSQL)
+       init_db(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, mapper_path='./mapper')
        
        persons = select_all()
        # result:
        # (3, 'zhangsan', 15)
        # (4, 'lisi', 26)
        # (5, 'wangwu', 38)
```

