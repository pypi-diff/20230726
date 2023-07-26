# Comparing `tmp/sqlx-exec-1.1.6.tar.gz` & `tmp/sqlx-exec-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.1.6.tar", last modified: Tue Jul 25 08:25:34 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.2.0.tar", last modified: Wed Jul 26 08:38:02 2023, max compression
```

## Comparing `sqlx-exec-1.1.6.tar` & `sqlx-exec-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.1.6/LICENSE
--rw-rw-rw-   0        0        0     2701 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2159 2023-07-22 02:28:05.000000 sqlx-exec-1.1.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1195 2023-07-25 08:25:10.000000 sqlx-exec-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/sqlexec/
--rw-rw-rw-   0        0        0      529 2023-07-23 08:55:03.000000 sqlx-exec-1.1.6/sqlexec/constant.py
--rw-rw-rw-   0        0        0     4615 2023-07-25 07:49:14.000000 sqlx-exec-1.1.6/sqlexec/engin.py
--rw-rw-rw-   0        0        0    11712 2023-07-25 05:43:20.000000 sqlx-exec-1.1.6/sqlexec/exec.py
--rw-rw-rw-   0        0        0     1030 2023-07-21 22:35:47.000000 sqlx-exec-1.1.6/sqlexec/log_support.py
--rw-rw-rw-   0        0        0      629 2023-07-23 22:45:17.000000 sqlx-exec-1.1.6/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1556 2023-07-23 13:53:53.000000 sqlx-exec-1.1.6/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4275 2023-07-23 09:51:27.000000 sqlx-exec-1.1.6/sqlexec/support.py
--rw-rw-rw-   0        0        0      389 2023-07-23 13:53:53.000000 sqlx-exec-1.1.6/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-23 13:22:36.000000 sqlx-exec-1.1.6/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2701 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 08:25:34.000000 sqlx-exec-1.1.6/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:02.000000 sqlx-exec-1.2.0/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2770 2023-07-26 08:38:02.000000 sqlx-exec-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2261 2023-07-26 08:32:11.000000 sqlx-exec-1.2.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:38:02.000000 sqlx-exec-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2023-07-26 08:37:31.000000 sqlx-exec-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:02.000000 sqlx-exec-1.2.0/sqlexec/
+-rw-rw-rw-   0        0        0      136 2023-07-26 00:53:39.000000 sqlx-exec-1.2.0/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     1410 2023-07-26 08:07:43.000000 sqlx-exec-1.2.0/sqlexec/engin.py
+-rw-rw-rw-   0        0        0    11421 2023-07-26 07:55:26.000000 sqlx-exec-1.2.0/sqlexec/exec.py
+-rw-rw-rw-   0        0        0      813 2023-07-25 16:57:35.000000 sqlx-exec-1.2.0/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0      833 2023-07-25 17:51:41.000000 sqlx-exec-1.2.0/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     1157 2023-07-26 02:18:21.000000 sqlx-exec-1.2.0/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.2.0/sqlexec/support.py
+-rw-rw-rw-   0        0        0      328 2023-07-25 17:38:22.000000 sqlx-exec-1.2.0/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:38:02.000000 sqlx-exec-1.2.0/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:38:01.000000 sqlx-exec-1.2.0/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-23 13:22:36.000000 sqlx-exec-1.2.0/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2770 2023-07-26 08:38:01.000000 sqlx-exec-1.2.0/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-07-26 08:38:02.000000 sqlx-exec-1.2.0/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 08:38:01.000000 sqlx-exec-1.2.0/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.1.6/LICENSE` & `sqlx-exec-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.1.6/PKG-INFO` & `sqlx-exec-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.1.6
-Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction. Now support MySQL and PostgreSQL.
+Version: 1.2.0
+Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
@@ -17,16 +17,17 @@
 
 .. code:: python
 
    import sqlexec
    from sqlexec import Engin
 
    if __name__ == '__main__':
-       sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, engin=Engin.PostgreSQL)
+       sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, driver='psycopg2')
 
+       # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
 
        count = sqlexec.get('select count(1) from person')
        # result: 3
```

### Comparing `sqlx-exec-1.1.6/README.rst` & `sqlx-exec-1.2.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 
 .. code:: python
 
    import sqlexec
    from sqlexec import Engin
 
    if __name__ == '__main__':
-       sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, engin=Engin.PostgreSQL)
+       sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, driver='psycopg2')
 
+       # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
 
        count = sqlexec.get('select count(1) from person')
        # result: 3
```

### Comparing `sqlx-exec-1.1.6/setup.py` & `sqlx-exec-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,18 +10,18 @@
         return fp.read()
 
 long_description = read("README.rst")
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
-    description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction. Now support MySQL and PostgreSQL.",
+    description="sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.1.6',
+    version='1.2.0',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.1.6/sqlexec/exec.py` & `sqlx-exec-1.2.0/sqlexec/exec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,96 +1,84 @@
 import functools
 import importlib
+from .engin import Engin
 from . import sql_support
-from .engin import Engin, DBEngin
-from .constant import MAPPER_PATH, DRIVER
-from .log_support import logger, insert_log, save_log, get_log, page_log
+from .constant import DRIVERS
+from .log_support import logger, insert_log, save_log, get_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
 
 _DB_CTX = None
+_SHOW_SQL = False
 
 
-def init_db(connect=None, host='127.0.0.1', port=3306, database='test', user='root', password='', engin=Engin.MYSQL, pool_size=0, show_sql=False, **kwargs):
-    DBEngin.init_db_engin(engin, show_sql)
-    _del_kwarg(MAPPER_PATH, kwargs)
-    driver = kwargs.pop(DRIVER) if DRIVER in kwargs else None
-    if 'debug' in kwargs:
-        if kwargs.pop('debug'):
-            from logging import DEBUG
-            logger.setLevel(DEBUG)
-
-    if connect:
-        import types
-        assert isinstance(connect, types.FunctionType), '`connect` must be a function, you can use like `connect=lambda: connect(**kwargs)`.'
-        _init_db(connect, engin, pool_size, driver)
-    else:
-        kwargs['user'] = user
-        kwargs['password'] = password
-        kwargs['database'] = database
-        kwargs['host'] = host
-        kwargs['port'] = port
-
-        _import_init(engin, pool_size, driver, **kwargs)
-
-
-def _import_init(engin, pool_size, driver, **kwargs):
+def init_db(host='127.0.0.1', port=3306, database='test', user='root', password='', driver='', pool_size=0, show_sql=False, debug=False, **kwargs):
+    global _DB_CTX, _SHOW_SQL
     prepared = False
-    if engin == Engin.MYSQL:
-        if not driver:
-            driver = 'pymysql'
-            logger.warning("Not set MySQL driver, will use default driver: 'pymysql'.")
-        creator = _import(driver)
-        if 'mysql.connector' == driver:
-            prepared = True
-            if pool_size > 0:
-                kwargs['pool_size'] = pool_size
-                pool_size = 0
-
-    elif engin == Engin.POSTGRESQL:
-        if not driver:
-            driver = 'psycopg2'
-            logger.warning("Not set PostgreSQL driver, will use default driver: 'psycopg2'.")
-        creator = _import(driver)
-        _del_kwarg('use_unicode', kwargs)
-    elif engin == Engin.OTHER:
-        if driver:
-            creator = _import(driver)
-        _del_kwarg('use_unicode', kwargs)
+    kwargs['user'] = user
+    kwargs['password'] = password
+    kwargs['database'] = database
+    kwargs['host'] = host
+    kwargs['port'] = port
+    if debug:
+        from logging import DEBUG
+        logger.setLevel(DEBUG)
+
+    if driver:
+        if driver not in DRIVERS:
+            logger.warning(f"Driver '{driver}' not support now, may be you should adapte it youself.")
+        engin_name = DRIVERS.get(driver)
+        creator = _import(driver, engin_name)
     else:
-        raise DBError('Engin is invalid: %s', engin)
+        current_engin = Engin.current_engin()
+        drivers = dict(filter(lambda x: x[1] == current_engin, DRIVERS.items())) if current_engin else DRIVERS
+        for driver in drivers:
+            try:
+                creator = importlib.import_module(driver)
+                engin_name = DRIVERS.get(driver)
+                break
+            except ModuleNotFoundError:
+                pass
+        if not creator:
+            raise DBError(f"You may forget install driver, now suppor: {list(DRIVERS.keys())}")
+
+    if 'mysql.connector' == driver:
+        prepared = True
+        kwargs['pool_size'] = pool_size
 
-    if pool_size >= 1 and driver != 'mysql.connector':
+    if pool_size <= 0 or prepared:
+        connect = lambda: creator.connect(**kwargs)
+    else:
         from .pooling import pooled_connect
         connect = pooled_connect(creator, pool_size, **kwargs)
-        _init_db(connect, engin, pool_size, driver, prepared)
+
+    with DB_LOCK:
+        if _DB_CTX is not None:
+            raise DBError('DB is already initialized.')
+        _SHOW_SQL = show_sql
+        _DB_CTX = DBCtx(connect=connect, prepared=prepared)
+
+    Engin.init(engin_name)
+    if pool_size > 0:
+        logger.info("Inited db engine <%s> of %s with driver: '%s' and pool size: %d." % (hex(id(_DB_CTX)), engin_name, driver, pool_size))
     else:
-        _init_db(lambda: creator.connect(**kwargs), engin, pool_size, driver, prepared)
+        logger.info("Inited db engine <%s> of %s with driver: '%s'." % (hex(id(_DB_CTX)), engin_name, driver))
 
+def _import(driver, engin_name):
 
-def _import(driver):
     try:
         return importlib.import_module(driver)
     except ModuleNotFoundError:
-        raise DBError(f"Import db driver '{driver}' failed, please sure it was installed or change other driver.")
+        raise DBError(f"Import {engin_name} driver '{driver}' failed, please sure it was installed or change other driver.")
 
 
 def _del_kwarg(key, kwargs):
     if key in kwargs:
         del kwargs[key]
 
 
-def _init_db(connect, engin, pool_size, driver, prepared=False):
-    global _DB_CTX
-    with DB_LOCK:
-        if _DB_CTX is not None:
-            raise DBError('DB is already initialized.')
-        _DB_CTX = DBCtx(connect=connect, pool_size=pool_size, prepared=prepared)
-    logger.info("Init db engine <%s> of %s with driver: '%s', pool size is %d." % (hex(id(_DB_CTX)), engin.value, driver, pool_size))
-
-
 def connection():
     """
     Return _ConnectionCtx object that can be used by 'with' statement:
     with connection():
         pass
     """
     global _DB_CTX
@@ -148,15 +136,15 @@
 def execute(sql: str, *args):
     """
     Execute sql return effect rowcount
     sql: insert into person(name, age) values(?, ?)  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = DBEngin.before_execute('execute', sql.strip(), *args)
+    sql = _before_execute('execute', sql.strip(), *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
         effect_rowcount = cursor.rowcount
         try_commit(_DB_CTX)
         return effect_rowcount
     finally:
@@ -197,15 +185,15 @@
     :param sql: table
     :param args:
     :return: Primary key
     """
     global _DB_CTX
     cursor = None
     logger.debug("Exec func 'sqlexec.%s', 'select_key': %s \n\t sql: %s \n\t args: %s" % ('save_sql', select_key, sql, args))
-    sql = DBEngin.before_execute('save_sql', sql, *args)
+    sql = _before_execute('save_sql', sql, *args)
     try:
         cursor = _DB_CTX.connection.cursor()
         cursor.execute(sql, args)
         cursor.execute(select_key)
         result = cursor.fetchone()
         try_commit(_DB_CTX)
         return result[0]
@@ -235,15 +223,15 @@
     :param args: All number must have same size.
     :return: Effect rowcount
     """
     global _DB_CTX
     cursor = None
     if isinstance(args[0], dict):
         sql, args = sql_support.batch_named_sql_args(sql, *args)
-    sql = DBEngin.before_execute('batch_execute', sql.strip(), *args)
+    sql = _before_execute('batch_execute', sql.strip(), *args)
     args = sql_support.get_batch_args(*args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.executemany(sql, args)
         effect_rowcount = cursor.rowcount
         try_commit(_DB_CTX)
         return effect_rowcount
@@ -273,15 +261,15 @@
 def select(sql: str, *args):
     """
     execute select SQL and return unique result or list results(tuple).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = DBEngin.before_execute('select', sql.strip(), *args)
+    sql = _before_execute('select', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         return cursor.fetchall()
     finally:
         if cursor:
             cursor.close()
@@ -291,39 +279,39 @@
 def select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = DBEngin.before_execute('select_one', sql.strip(), *args)
+    sql = _before_execute('select_one', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         return cursor.fetchone()
     finally:
         if cursor:
             cursor.close()
 
 
-def select_page(sql: str, page_num, page_size, *args):
-    page_log('select_page', sql.strip(), page_num, page_size, args)
-    sql, args = sql_support.page_sql_args(sql, page_num, page_size, *args)
-    return select(sql, *args)
+# def select_page(sql: str, page_num, page_size, *args):
+#     page_log('select_page', sql.strip(), page_num, page_size, args)
+#     sql, args = sql_support.page_sql_args(sql, page_num, page_size, *args)
+#     return select(sql, *args)
 
 
 @with_connection
 def query(sql: str, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = DBEngin.before_execute('query', sql.strip(), *args)
+    sql = _before_execute('query', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         results = cursor.fetchall()
         if results and cursor.description:
             names = [x[0] for x in cursor.description]
             return [Dict(names, x) for x in results]
@@ -338,33 +326,39 @@
 def query_one(sql: str, *args):
     """
     execute select SQL and return unique result(dict), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     global _DB_CTX
     cursor = None
-    sql = DBEngin.before_execute('query_one', sql.strip(), *args)
+    sql = _before_execute('query_one', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
         result = cursor.fetchone()
         if result and cursor.description:
             names = [x[0] for x in cursor.description]
             return Dict(names, result)
         return result
     finally:
         if cursor:
             cursor.close()
 
 
-def query_page(sql: str, page_num, page_size, *args):
-    page_log('query_page', sql.strip(), page_num, page_size, args)
-    sql, args = sql_support.page_sql_args(sql, page_num, page_size, *args)
-    return query(sql, *args)
+# def query_page(sql: str, page_num, page_size, *args):
+#     page_log('query_page', sql.strip(), page_num, page_size, args)
+#     sql, args = sql_support.page_sql_args(sql, page_num, page_size, *args)
+#     return query(sql, *args)
 
 
 def get_connection():
     global _DB_CTX
-    if _DB_CTX.is_not_init():
-        _DB_CTX.init()
+    _DB_CTX.try_init()
     return _DB_CTX.connection
 
+
+def _before_execute(function: str, sql: str, *args):
+    if _SHOW_SQL:
+        logger.info("Exec func 'sqlexec.%s' \n\tSQL: %s \n\tARGS: %s" % (function, sql, args))
+    if '%' in sql and 'like' in sql.lower():
+        sql = sql.replace('%', '%%').replace('%%%%', '%%')
+    return sql.replace('?', '%s')
```

### Comparing `sqlx-exec-1.1.6/sqlexec/log_support.py` & `sqlx-exec-1.2.0/sqlexec/log_support.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,14 +12,10 @@
     logger.debug("Exec func 'sqlexec.%s', 'select_key': %s \n\t Table: '%s', kwargs: %s" % (function, select_key, table, kwargs))
 
 
 def get_log(function: str, sql: str, *args):
     logger.debug("Exec func 'sqlexec.%s' \n\t sql: %s \n\t args: %s" % (function, sql, args))
 
 
-def page_log(function: str, sql: str, page_num, page_size, *args):
-    logger.debug("Exec func 'sqlexec.%s', page_num: %d, page_size: %d \n\t sql: %s \n\t args: %s" % (function, page_num, page_size, sql, args))
-
-
 def db_ctx_log(action, connection):
     logger.debug('%s connection <%s>...' % (action, hex(id(connection))))
```

### Comparing `sqlx-exec-1.1.6/sqlexec/support.py` & `sqlx-exec-1.2.0/sqlexec/support.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,28 +18,30 @@
 
 
 class DBCtx(threading.local):
     """
     Thread local object that holds connection info.
     """
 
-    def __init__(self, connect, pool_size, prepared=False):
+    def __init__(self, connect, prepared=False):
         self.connect = connect
         self.connection = None
         self.transactions = 0
-        self.pool_size = pool_size
         self.prepared = prepared
 
-    def is_not_init(self):
-        return self.connection is None
+    # def is_not_init(self):
+    #     return self.connection is None
 
-    def init(self):
-        self.transactions = 0
-        self.connection = self.connect()
-        self.log('Use')
+    def try_init(self):
+        if self.connection is None:
+            self.transactions = 0
+            self.connection = self.connect()
+            self.log('Use')
+            return 1
+        return 0
 
     def release(self):
         if self.connection:
             self.log('Release')
             self.connection.close()
             self.connection = None
 
@@ -53,20 +55,15 @@
     def statement(self, sql: str):
         """
         Return statement
         """
         return self.connection.statement(sql)
 
     def log(self, action: str):
-        if self.prepared and self.pool_size >= 1:
-            db_ctx_log(action, self.connection._cnx)
-        elif self.pool_size >= 1:
-            db_ctx_log(action, self.connection._con)
-        else:
-            db_ctx_log(action, self.connection)
+        db_ctx_log(action, self.connection)
 
 class ConnectionCtx(object):
     """
     ConnectionCtx object that can open and close connection context. ConnectionCtx object can be nested and only the most
     outer connection has effect.
     with connection():
         pass
@@ -75,16 +72,15 @@
     """
 
     def __init__(self, db_ctx):
         self.db_ctx = db_ctx
 
     def __enter__(self):
         self.should_cleanup = False
-        if self.db_ctx.is_not_init():
-            self.db_ctx.init()
+        if self.db_ctx.try_init():
             self.should_cleanup = True
         return self
 
     def __exit__(self, exctype, excvalue, traceback):
         if self.should_cleanup:
             self.db_ctx.release()
 
@@ -97,17 +93,16 @@
     """
 
     def __init__(self, db_ctx):
         self.db_ctx = db_ctx
 
     def __enter__(self):
         self.should_close_conn = False
-        if self.db_ctx.is_not_init():
+        if self.db_ctx.try_init():
             # needs open a connection first:
-            self.db_ctx.init()
             self.should_close_conn = True
         self.db_ctx.transactions += 1
         logger.debug('Begin transaction...' if self.db_ctx.transactions == 1 else 'Join current transaction...')
         return self
 
     def __exit__(self, exctype, excvalue, traceback):
         self.db_ctx.transactions -= 1
```

### Comparing `sqlx-exec-1.1.6/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.2.0/sqlx_exec.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.1.6
-Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction. Now support MySQL and PostgreSQL.
+Version: 1.2.0
+Summary: sqlx-exec is a simple sql executor for Python, it help you auto manage database connection and transaction.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,python
 Platform: UNKNOWN
 Requires-Python: >=3.5
@@ -17,16 +17,17 @@
 
 .. code:: python
 
    import sqlexec
    from sqlexec import Engin
 
    if __name__ == '__main__':
-       sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, engin=Engin.PostgreSQL)
+       sqlexec.init_engin(host='127.0.0.1', port='3306', person='xxx', password='xxx', database='test', show_sql=True, driver='psycopg2')
 
+       # if driver is 'pymysql' or 'mysql.connector' of MySQL, the select_key is 'SELECT LAST_INSERT_ID()'
        select_key = "SELECT currval('person_id_seq')"
        id = sqlexec.save(select_key=select_key, table='person', name='zhangsan', age=15)
        id = sqlexec.save_sql(select_key, 'INSERT INTO person(name,age) VALUES(?,?)', 'lisi', 26)
        rowcount = sqlexec.insert(table='person', name='wangwu', age=38)
 
        count = sqlexec.get('select count(1) from person')
        # result: 3
```

