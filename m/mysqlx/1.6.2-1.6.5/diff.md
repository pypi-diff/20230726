# Comparing `tmp/mysqlx-1.6.2.tar.gz` & `tmp/mysqlx-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.6.2.tar", last modified: Tue Jul 25 08:29:33 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.6.5.tar", last modified: Wed Jul 26 08:41:02 2023, max compression
```

## Comparing `mysqlx-1.6.2.tar` & `mysqlx-1.6.5.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:29:33.000000 mysqlx-1.6.2/
-drwxrwxrwx   0        0        0        0 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx/
--rw-rw-rw-   0        0        0      687 2023-07-25 07:29:18.000000 mysqlx-1.6.2/mysqlx/db.py
--rw-rw-rw-   0        0        0      344 2023-07-24 01:32:22.000000 mysqlx-1.6.2/mysqlx/log_support.py
--rw-rw-rw-   0        0        0     6065 2023-07-25 08:13:53.000000 mysqlx-1.6.2/mysqlx/orm.py
--rw-rw-rw-   0        0        0      626 2023-07-25 06:08:48.000000 mysqlx-1.6.2/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4511 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      265 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-25 08:29:33.000000 mysqlx-1.6.2/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4511 2023-07-25 08:29:33.000000 mysqlx-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     4007 2023-07-25 08:23:23.000000 mysqlx-1.6.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-25 08:29:33.000000 mysqlx-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-07-25 08:29:07.000000 mysqlx-1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:41:02.000000 mysqlx-1.6.5/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx/
+-rw-rw-rw-   0        0        0     2726 2023-07-26 07:18:22.000000 mysqlx-1.6.5/mysqlx/db.py
+-rw-rw-rw-   0        0        0     1897 2023-07-26 07:24:54.000000 mysqlx-1.6.5/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0      763 2023-07-26 07:58:39.000000 mysqlx-1.6.5/mysqlx/engin.py
+-rw-rw-rw-   0        0        0     1704 2023-07-26 07:24:54.000000 mysqlx-1.6.5/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0     9895 2023-07-26 07:32:28.000000 mysqlx-1.6.5/mysqlx/orm.py
+-rw-rw-rw-   0        0        0      339 2023-07-26 07:19:23.000000 mysqlx-1.6.5/mysqlx/sql_support.py
+-rw-rw-rw-   0        0        0      641 2023-07-26 08:02:46.000000 mysqlx-1.6.5/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4511 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      317 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 08:41:02.000000 mysqlx-1.6.5/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4511 2023-07-26 08:41:02.000000 mysqlx-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4007 2023-07-25 08:23:23.000000 mysqlx-1.6.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:41:02.000000 mysqlx-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2023-07-26 08:40:53.000000 mysqlx-1.6.5/setup.py
```

### Comparing `mysqlx-1.6.2/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.6.5/mysqlx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.6.2
+Version: 1.6.5
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-1.6.2/PKG-INFO` & `mysqlx-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.6.2
+Version: 1.6.5
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-1.6.2/README.rst` & `mysqlx-1.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `mysqlx-1.6.2/setup.py` & `mysqlx-1.6.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     name='mysqlx',
     packages=['mysqlx'],
     description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # 'Jinja2>=2.7.0',
-        'sqlx-batis>=0.0.8',
+        'sqlx-batis>=0.0.9',
         # 'mysql-connector-python>=8.0.13',
     ],
-    version='1.6.2',
+    version='1.6.5',
     url='https://gitee.com/summry/mysqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

