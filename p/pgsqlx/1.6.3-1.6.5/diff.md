# Comparing `tmp/pgsqlx-1.6.3.tar.gz` & `tmp/pgsqlx-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.6.3.tar", last modified: Tue Jul 25 08:28:37 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.6.5.tar", last modified: Wed Jul 26 08:40:07 2023, max compression
```

## Comparing `pgsqlx-1.6.3.tar` & `pgsqlx-1.6.5.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/
-drwxrwxrwx   0        0        0        0 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx/
--rw-rw-rw-   0        0        0     1072 2023-07-25 07:22:11.000000 pgsqlx-1.6.3/pgsqlx/db.py
--rw-rw-rw-   0        0        0      534 2023-07-24 00:56:26.000000 pgsqlx-1.6.3/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0     1892 2023-07-25 08:08:47.000000 pgsqlx-1.6.3/pgsqlx/orm.py
--rw-rw-rw-   0        0        0      629 2023-07-25 06:13:56.000000 pgsqlx-1.6.3/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4612 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      265 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4612 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     4096 2023-07-25 08:21:22.000000 pgsqlx-1.6.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-25 08:28:37.000000 pgsqlx-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1237 2023-07-25 08:27:48.000000 pgsqlx-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:40:07.000000 pgsqlx-1.6.5/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:40:07.000000 pgsqlx-1.6.5/pgsqlx/
+-rw-rw-rw-   0        0        0      156 2023-07-26 07:07:24.000000 pgsqlx-1.6.5/pgsqlx/constant.py
+-rw-rw-rw-   0        0        0     3107 2023-07-26 07:17:42.000000 pgsqlx-1.6.5/pgsqlx/db.py
+-rw-rw-rw-   0        0        0     2002 2023-07-26 07:26:12.000000 pgsqlx-1.6.5/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0     1532 2023-07-26 07:59:16.000000 pgsqlx-1.6.5/pgsqlx/engin.py
+-rw-rw-rw-   0        0        0     1896 2023-07-26 07:25:39.000000 pgsqlx-1.6.5/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0     6066 2023-07-26 07:29:24.000000 pgsqlx-1.6.5/pgsqlx/orm.py
+-rw-rw-rw-   0        0        0     3310 2023-07-26 07:10:47.000000 pgsqlx-1.6.5/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0      349 2023-07-26 05:51:44.000000 pgsqlx-1.6.5/pgsqlx/sql_support.py
+-rw-rw-rw-   0        0        0      662 2023-07-26 07:37:24.000000 pgsqlx-1.6.5/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:40:07.000000 pgsqlx-1.6.5/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:40:07.000000 pgsqlx-1.6.5/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-26 08:40:07.000000 pgsqlx-1.6.5/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4612 2023-07-26 08:40:07.000000 pgsqlx-1.6.5/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-26 08:40:07.000000 pgsqlx-1.6.5/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      357 2023-07-26 08:40:07.000000 pgsqlx-1.6.5/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 08:40:07.000000 pgsqlx-1.6.5/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4612 2023-07-26 08:40:07.000000 pgsqlx-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4096 2023-07-25 08:21:22.000000 pgsqlx-1.6.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:40:07.000000 pgsqlx-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1237 2023-07-26 08:39:58.000000 pgsqlx-1.6.5/setup.py
```

### Comparing `pgsqlx-1.6.3/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.6.5/pgsqlx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.6.3
+Version: 1.6.5
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.6.3/PKG-INFO` & `pgsqlx-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.6.3
+Version: 1.6.5
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.6.3/README.rst` & `pgsqlx-1.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.6.3/setup.py` & `pgsqlx-1.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     packages=['pgsqlx'],
     description="PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # 'Jinja2>=2.7.0',
         # 'psycopg2>=2.7.4',
-        'sqlx-batis>=0.0.8',
+        'sqlx-batis>=0.0.9',
     ],
-    version='1.6.3',
+    version='1.6.5',
     url='https://gitee.com/summry/pgsqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

