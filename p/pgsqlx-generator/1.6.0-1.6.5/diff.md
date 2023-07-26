# Comparing `tmp/pgsqlx-generator-1.6.0.tar.gz` & `tmp/pgsqlx-generator-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-generator-1.6.0.tar", last modified: Tue Jul 25 08:29:19 2023, max compression
+gzip compressed data, was "dist\pgsqlx-generator-1.6.5.tar", last modified: Wed Jul 26 08:40:27 2023, max compression
```

## Comparing `pgsqlx-generator-1.6.0.tar` & `pgsqlx-generator-1.6.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/
-drwxrwxrwx   0        0        0        0 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx/
--rw-rw-rw-   0        0        0     6673 2023-07-25 08:10:07.000000 pgsqlx-generator-1.6.0/pgsqlx/generator.py
--rw-rw-rw-   0        0        0     1905 2023-07-24 06:46:00.000000 pgsqlx-generator-1.6.0/pgsqlx/generator.tpl
--rw-rw-rw-   0        0        0      629 2023-07-25 06:13:56.000000 pgsqlx-generator-1.6.0/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2868 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0      317 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2868 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     2395 2023-07-24 07:34:39.000000 pgsqlx-generator-1.6.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-25 08:29:19.000000 pgsqlx-generator-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1122 2023-07-25 08:28:28.000000 pgsqlx-generator-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:40:27.000000 pgsqlx-generator-1.6.5/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:40:27.000000 pgsqlx-generator-1.6.5/pgsqlx/
+-rw-rw-rw-   0        0        0     6673 2023-07-25 08:10:07.000000 pgsqlx-generator-1.6.5/pgsqlx/generator.py
+-rw-rw-rw-   0        0        0     1905 2023-07-24 06:46:00.000000 pgsqlx-generator-1.6.5/pgsqlx/generator.tpl
+-rw-rw-rw-   0        0        0      662 2023-07-26 07:37:24.000000 pgsqlx-generator-1.6.5/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:40:27.000000 pgsqlx-generator-1.6.5/pgsqlx_generator.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:40:27.000000 pgsqlx-generator-1.6.5/pgsqlx_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-26 08:40:27.000000 pgsqlx-generator-1.6.5/pgsqlx_generator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2868 2023-07-26 08:40:27.000000 pgsqlx-generator-1.6.5/pgsqlx_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-26 08:40:27.000000 pgsqlx-generator-1.6.5/pgsqlx_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      317 2023-07-26 08:40:27.000000 pgsqlx-generator-1.6.5/pgsqlx_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 08:40:27.000000 pgsqlx-generator-1.6.5/pgsqlx_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2868 2023-07-26 08:40:27.000000 pgsqlx-generator-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2395 2023-07-24 07:34:39.000000 pgsqlx-generator-1.6.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:40:27.000000 pgsqlx-generator-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1122 2023-07-26 08:40:18.000000 pgsqlx-generator-1.6.5/setup.py
```

### Comparing `pgsqlx-generator-1.6.0/pgsqlx/generator.py` & `pgsqlx-generator-1.6.5/pgsqlx/generator.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-generator-1.6.0/pgsqlx/generator.tpl` & `pgsqlx-generator-1.6.5/pgsqlx/generator.tpl`

 * *Files identical despite different names*

### Comparing `pgsqlx-generator-1.6.0/pgsqlx_generator.egg-info/PKG-INFO` & `pgsqlx-generator-1.6.5/pgsqlx_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx-generator
-Version: 1.6.0
+Version: 1.6.5
 Summary: pgsqlx-generator is a model code generator from tables for PgSqlx.
 Home-page: https://gitee.com/summry/pgsqlx/blob/master/generator.md
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: PostgreSQL,PgSqlx,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-generator-1.6.0/PKG-INFO` & `pgsqlx-generator-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx-generator
-Version: 1.6.0
+Version: 1.6.5
 Summary: pgsqlx-generator is a model code generator from tables for PgSqlx.
 Home-page: https://gitee.com/summry/pgsqlx/blob/master/generator.md
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: PostgreSQL,PgSqlx,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-generator-1.6.0/README.rst` & `pgsqlx-generator-1.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `pgsqlx-generator-1.6.0/setup.py` & `pgsqlx-generator-1.6.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 setup(
     name='pgsqlx-generator',
     packages=['pgsqlx'],
     description="pgsqlx-generator is a model code generator from tables for PgSqlx.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        'sqlx-batis>=0.0.8',
+        'sqlx-batis>=0.0.9',
     ],
-    version='1.6.0',
+    version='1.6.5',
     url='https://gitee.com/summry/pgsqlx/blob/master/generator.md',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['PostgreSQL', 'PgSqlx', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

