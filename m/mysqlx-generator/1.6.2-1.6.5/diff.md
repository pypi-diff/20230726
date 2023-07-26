# Comparing `tmp/mysqlx-generator-1.6.2.tar.gz` & `tmp/mysqlx-generator-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-generator-1.6.2.tar", last modified: Tue Jul 25 08:29:44 2023, max compression
+gzip compressed data, was "dist\mysqlx-generator-1.6.5.tar", last modified: Wed Jul 26 08:42:05 2023, max compression
```

## Comparing `mysqlx-generator-1.6.2.tar` & `mysqlx-generator-1.6.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:29:44.000000 mysqlx-generator-1.6.2/
-drwxrwxrwx   0        0        0        0 2023-07-25 08:29:44.000000 mysqlx-generator-1.6.2/mysqlx/
--rw-rw-rw-   0        0        0     6186 2023-07-25 08:14:17.000000 mysqlx-generator-1.6.2/mysqlx/generator.py
--rw-rw-rw-   0        0        0     1802 2023-07-24 02:58:28.000000 mysqlx-generator-1.6.2/mysqlx/generator.tpl
--rw-rw-rw-   0        0        0      626 2023-07-25 06:08:48.000000 mysqlx-generator-1.6.2/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:29:44.000000 mysqlx-generator-1.6.2/mysqlx_generator.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-25 08:29:44.000000 mysqlx-generator-1.6.2/mysqlx_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 08:29:44.000000 mysqlx-generator-1.6.2/mysqlx_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2826 2023-07-25 08:29:44.000000 mysqlx-generator-1.6.2/mysqlx_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-25 08:29:44.000000 mysqlx-generator-1.6.2/mysqlx_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0      317 2023-07-25 08:29:44.000000 mysqlx-generator-1.6.2/mysqlx_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-25 08:29:44.000000 mysqlx-generator-1.6.2/mysqlx_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2826 2023-07-25 08:29:44.000000 mysqlx-generator-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     2358 2023-07-24 01:17:21.000000 mysqlx-generator-1.6.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-25 08:29:44.000000 mysqlx-generator-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1118 2023-07-25 08:29:07.000000 mysqlx-generator-1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:42:05.000000 mysqlx-generator-1.6.5/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:42:05.000000 mysqlx-generator-1.6.5/mysqlx/
+-rw-rw-rw-   0        0        0     6196 2023-07-26 08:02:46.000000 mysqlx-generator-1.6.5/mysqlx/generator.py
+-rw-rw-rw-   0        0        0     1802 2023-07-24 02:58:28.000000 mysqlx-generator-1.6.5/mysqlx/generator.tpl
+-rw-rw-rw-   0        0        0      641 2023-07-26 08:02:46.000000 mysqlx-generator-1.6.5/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:42:05.000000 mysqlx-generator-1.6.5/mysqlx_generator.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:42:05.000000 mysqlx-generator-1.6.5/mysqlx_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-26 08:42:05.000000 mysqlx-generator-1.6.5/mysqlx_generator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2826 2023-07-26 08:42:05.000000 mysqlx-generator-1.6.5/mysqlx_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-26 08:42:05.000000 mysqlx-generator-1.6.5/mysqlx_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      317 2023-07-26 08:42:05.000000 mysqlx-generator-1.6.5/mysqlx_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 08:42:05.000000 mysqlx-generator-1.6.5/mysqlx_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2826 2023-07-26 08:42:05.000000 mysqlx-generator-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2358 2023-07-24 01:17:21.000000 mysqlx-generator-1.6.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:42:05.000000 mysqlx-generator-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1118 2023-07-26 08:42:02.000000 mysqlx-generator-1.6.5/setup.py
```

### Comparing `mysqlx-generator-1.6.2/mysqlx/generator.py` & `mysqlx-generator-1.6.5/mysqlx/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
+from mysqlx import MySqlEngin
+from sqlbatis import db, init_db
 from typing import Union, Iterable
-from sqlbatis import db, Engin, init_db
 from jinja2 import FileSystemLoader, Environment
 from sqlbatis.constant import KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY
 
 COMMON_COLS = ['create_by', 'create_time']
 ATTRIBUTES = {KEY: 'id', UPDATE_BY: 'update_by', UPDATE_TIME: 'update_time', DEL_FLAG: 'del_flag'}
 
 
@@ -13,16 +14,16 @@
     comma2 = '，'
     sql = '''
     SELECT column_name, data_type, character_maximum_length, NUMERIC_precision, NUMERIC_scale, column_key FROM information_schema.columns
      WHERE table_schema = (SELECT DATABASE()) AND table_name = ? 
     '''
 
     def __init__(self, user='root', password='', database='test', host='127.0.0.1', port=3306, pool_size=0, show_sql=False, use_unicode=True, **kwargs):
-        init_db(user=user, password=password, database=database, host=host, port=port, engin=Engin.MYSQL, pool_size=pool_size, show_sql=show_sql, \
-                   use_unicode=use_unicode, **kwargs)
+        MySqlEngin.init()
+        init_db(user=user, password=password, database=database, host=host, port=port, pool_size=pool_size, show_sql=show_sql, use_unicode=use_unicode, **kwargs)
 
     def generate_with_schema(self, schema: str = None, path: str = None, *args, **kwargs):
         if schema:
             db.execute('use %s' % schema)
         tables = db.select('show tables')
         tables = [table[0] for table in tables]
         self.generate_with_tables(tables=tables, path=path, *args, **kwargs)
```

### Comparing `mysqlx-generator-1.6.2/mysqlx/generator.tpl` & `mysqlx-generator-1.6.5/mysqlx/generator.tpl`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.6.2/mysqlx_generator.egg-info/PKG-INFO` & `mysqlx-generator-1.6.5/mysqlx_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.6.2
+Version: 1.6.5
 Summary: mysqlx-generator is a model code generator from tables for MySqlx.
 Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-generator-1.6.2/PKG-INFO` & `mysqlx-generator-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.6.2
+Version: 1.6.5
 Summary: mysqlx-generator is a model code generator from tables for MySqlx.
 Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-generator-1.6.2/README.rst` & `mysqlx-generator-1.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.6.2/setup.py` & `mysqlx-generator-1.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 setup(
     name='mysqlx-generator',
     packages=['mysqlx'],
     description="mysqlx-generator is a model code generator from tables for MySqlx.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        'sqlx-batis>=0.0.8',
+        'sqlx-batis>=0.0.9',
     ],
-    version='1.6.2',
+    version='1.6.5',
     url='https://gitee.com/summry/mysqlx/blob/master/generator.md',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['MySQL', 'mysqlx', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

