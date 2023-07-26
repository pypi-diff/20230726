# Comparing `tmp/mysqlx-generator-1.6.6.tar.gz` & `tmp/mysqlx-generator-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-generator-1.6.6.tar", last modified: Wed Jul 26 09:00:04 2023, max compression
+gzip compressed data, was "dist\mysqlx-generator-1.6.8.tar", last modified: Wed Jul 26 09:11:55 2023, max compression
```

## Comparing `mysqlx-generator-1.6.6.tar` & `mysqlx-generator-1.6.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 09:00:04.000000 mysqlx-generator-1.6.6/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:00:04.000000 mysqlx-generator-1.6.6/mysqlx/
--rw-rw-rw-   0        0        0     6196 2023-07-26 08:02:46.000000 mysqlx-generator-1.6.6/mysqlx/generator.py
--rw-rw-rw-   0        0        0     1802 2023-07-24 02:58:28.000000 mysqlx-generator-1.6.6/mysqlx/generator.tpl
--rw-rw-rw-   0        0        0      641 2023-07-26 08:02:46.000000 mysqlx-generator-1.6.6/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:00:04.000000 mysqlx-generator-1.6.6/mysqlx_generator.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-26 09:00:04.000000 mysqlx-generator-1.6.6/mysqlx_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-26 09:00:04.000000 mysqlx-generator-1.6.6/mysqlx_generator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2826 2023-07-26 09:00:04.000000 mysqlx-generator-1.6.6/mysqlx_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-26 09:00:04.000000 mysqlx-generator-1.6.6/mysqlx_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0      317 2023-07-26 09:00:04.000000 mysqlx-generator-1.6.6/mysqlx_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 09:00:04.000000 mysqlx-generator-1.6.6/mysqlx_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2826 2023-07-26 09:00:04.000000 mysqlx-generator-1.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     2358 2023-07-24 01:17:21.000000 mysqlx-generator-1.6.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-26 09:00:04.000000 mysqlx-generator-1.6.6/setup.cfg
--rw-rw-rw-   0        0        0     1114 2023-07-26 08:59:53.000000 mysqlx-generator-1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/
+drwxrwxrwx   0        0        0        0 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx/
+-rw-rw-rw-   0        0        0     6196 2023-07-26 08:02:46.000000 mysqlx-generator-1.6.8/mysqlx/generator.py
+-rw-rw-rw-   0        0        0     1802 2023-07-24 02:58:28.000000 mysqlx-generator-1.6.8/mysqlx/generator.tpl
+-rw-rw-rw-   0        0        0      641 2023-07-26 08:02:46.000000 mysqlx-generator-1.6.8/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx_generator.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx_generator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2826 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      317 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/mysqlx_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2826 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2358 2023-07-24 01:17:21.000000 mysqlx-generator-1.6.8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-26 09:11:55.000000 mysqlx-generator-1.6.8/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2023-07-26 09:11:49.000000 mysqlx-generator-1.6.8/setup.py
```

### Comparing `mysqlx-generator-1.6.6/mysqlx/generator.py` & `mysqlx-generator-1.6.8/mysqlx/generator.py`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.6.6/mysqlx/generator.tpl` & `mysqlx-generator-1.6.8/mysqlx/generator.tpl`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.6.6/mysqlx/__init__.py` & `mysqlx-generator-1.6.8/mysqlx/__init__.py`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.6.6/mysqlx_generator.egg-info/PKG-INFO` & `mysqlx-generator-1.6.8/mysqlx_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.6.6
+Version: 1.6.8
 Summary: mysqlx-generator is a model code generator from tables for MySqlx.
 Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-generator-1.6.6/PKG-INFO` & `mysqlx-generator-1.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx-generator
-Version: 1.6.6
+Version: 1.6.8
 Summary: mysqlx-generator is a model code generator from tables for MySqlx.
 Home-page: https://gitee.com/summry/mysqlx/blob/master/generator.md
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: MySQL,mysqlx,python
 Platform: UNKNOWN
```

### Comparing `mysqlx-generator-1.6.6/README.rst` & `mysqlx-generator-1.6.8/README.rst`

 * *Files identical despite different names*

### Comparing `mysqlx-generator-1.6.6/setup.py` & `mysqlx-generator-1.6.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 setup(
     name='mysqlx-generator',
     packages=['mysqlx'],
     description="mysqlx-generator is a model code generator from tables for MySqlx.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
-        'pgsqlx>=1.6.5',
+        'mysqlx>=1.6.5',
     ],
-    version='1.6.6',
+    version='1.6.8',
     url='https://gitee.com/summry/mysqlx/blob/master/generator.md',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['MySQL', 'mysqlx', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

