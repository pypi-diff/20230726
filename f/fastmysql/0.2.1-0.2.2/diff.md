# Comparing `tmp/fastmysql-0.2.1.tar.gz` & `tmp/fastmysql-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmysql-0.2.1.tar", last modified: Wed Jul 26 07:26:56 2023, max compression
+gzip compressed data, was "fastmysql-0.2.2.tar", last modified: Wed Jul 26 07:51:57 2023, max compression
```

## Comparing `fastmysql-0.2.1.tar` & `fastmysql-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 07:26:56.061557 fastmysql-0.2.1/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-26 07:26:56.061446 fastmysql-0.2.1/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1442 2023-02-22 07:55:41.000000 fastmysql-0.2.1/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 07:26:56.060468 fastmysql-0.2.1/fastmysql/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      238 2023-07-26 03:48:57.000000 fastmysql-0.2.1/fastmysql/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    47563 2023-07-24 10:45:49.000000 fastmysql-0.2.1/fastmysql/fastmysql.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    25529 2023-07-26 07:26:27.000000 fastmysql-0.2.1/fastmysql/fastmysql_test.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 07:26:56.061280 fastmysql-0.2.1/fastmysql.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-26 07:26:56.000000 fastmysql-0.2.1/fastmysql.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      255 2023-07-26 07:26:56.000000 fastmysql-0.2.1/fastmysql.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-07-26 07:26:56.000000 fastmysql-0.2.1/fastmysql.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)      146 2023-07-26 07:26:56.000000 fastmysql-0.2.1/fastmysql.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-07-26 07:26:56.000000 fastmysql-0.2.1/fastmysql.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-07-26 07:26:56.061591 fastmysql-0.2.1/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1102 2023-07-26 07:26:11.000000 fastmysql-0.2.1/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 07:51:57.138688 fastmysql-0.2.2/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-26 07:51:57.138575 fastmysql-0.2.2/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1442 2023-02-22 07:55:41.000000 fastmysql-0.2.2/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 07:51:57.137582 fastmysql-0.2.2/fastmysql/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      238 2023-07-26 03:48:57.000000 fastmysql-0.2.2/fastmysql/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    47563 2023-07-24 10:45:49.000000 fastmysql-0.2.2/fastmysql/fastmysql.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    25775 2023-07-26 07:40:51.000000 fastmysql-0.2.2/fastmysql/fastmysql_test.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 07:51:57.138421 fastmysql-0.2.2/fastmysql.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-26 07:51:57.000000 fastmysql-0.2.2/fastmysql.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      255 2023-07-26 07:51:57.000000 fastmysql-0.2.2/fastmysql.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-07-26 07:51:57.000000 fastmysql-0.2.2/fastmysql.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      146 2023-07-26 07:51:57.000000 fastmysql-0.2.2/fastmysql.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-07-26 07:51:57.000000 fastmysql-0.2.2/fastmysql.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-07-26 07:51:57.138728 fastmysql-0.2.2/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1102 2023-07-26 07:51:25.000000 fastmysql-0.2.2/setup.py
```

### Comparing `fastmysql-0.2.1/PKG-INFO` & `fastmysql-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmysql
-Version: 0.2.1
+Version: 0.2.2
 Summary: make it easy to use pymysql
 Home-page: https://gitee.com/ZeroSeeker/fastmysql
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fastmysql-0.2.1/README.md` & `fastmysql-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fastmysql-0.2.1/fastmysql/fastmysql.py` & `fastmysql-0.2.2/fastmysql/fastmysql.py`

 * *Files identical despite different names*

### Comparing `fastmysql-0.2.1/fastmysql/fastmysql_test.py` & `fastmysql-0.2.2/fastmysql/fastmysql_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,32 +146,39 @@
         return con_info
 
     def query(
             self,
             sql: str = None,
             sql_list: list = None,
             args=None,
-            executemany: bool = False
+            executemany: bool = False,
+            database_name: str = None
     ):
         """
         查询结果以list(dict)形式输出
         [不包含重试机制，需要在外部执行重试]
         :param sql: SELECT * FROM users WHERE username = %s
         :param sql_list:
         :param args: 参数化查询语句避免SQL注入
         :param executemany: 是否批量执行
+        :param database_name: 指定数据库名
         :return: {"data": [], "affected_rows": 0}
         """
         retries = 0
         affected_rows = 0
         data = list()
         while True:
             connection = self.POOL.connection()  # 从连接池中获取连接对象
             try:
                 with connection.cursor() as cursor:
+                    if database_name:
+                        cursor.execute(f"USE {database_name};")
+                    else:
+                        pass
+
                     if executemany:
                         if sql:
                             cursor.executemany(
                                 query=sql,
                                 args=args
                             )
                             affected_rows = cursor.rowcount
```

### Comparing `fastmysql-0.2.1/fastmysql.egg-info/PKG-INFO` & `fastmysql-0.2.2/fastmysql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmysql
-Version: 0.2.1
+Version: 0.2.2
 Summary: make it easy to use pymysql
 Home-page: https://gitee.com/ZeroSeeker/fastmysql
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fastmysql-0.2.1/setup.py` & `fastmysql-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fastmysql",
-    version="0.2.1",
+    version="0.2.2",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     description="make it easy to use pymysql",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ZeroSeeker/fastmysql",
     packages=setuptools.find_packages(),
```

