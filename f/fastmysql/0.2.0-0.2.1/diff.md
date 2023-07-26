# Comparing `tmp/fastmysql-0.2.0.tar.gz` & `tmp/fastmysql-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmysql-0.2.0.tar", last modified: Wed Jul 26 06:52:10 2023, max compression
+gzip compressed data, was "fastmysql-0.2.1.tar", last modified: Wed Jul 26 07:26:56 2023, max compression
```

## Comparing `fastmysql-0.2.0.tar` & `fastmysql-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 06:52:10.147163 fastmysql-0.2.0/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-26 06:52:10.147045 fastmysql-0.2.0/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1442 2023-02-22 07:55:41.000000 fastmysql-0.2.0/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 06:52:10.145950 fastmysql-0.2.0/fastmysql/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      238 2023-07-26 03:48:57.000000 fastmysql-0.2.0/fastmysql/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    47563 2023-07-24 10:45:49.000000 fastmysql-0.2.0/fastmysql/fastmysql.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    25482 2023-07-26 06:51:37.000000 fastmysql-0.2.0/fastmysql/fastmysql_test.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 06:52:10.146869 fastmysql-0.2.0/fastmysql.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-26 06:52:10.000000 fastmysql-0.2.0/fastmysql.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      255 2023-07-26 06:52:10.000000 fastmysql-0.2.0/fastmysql.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-07-26 06:52:10.000000 fastmysql-0.2.0/fastmysql.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)      146 2023-07-26 06:52:10.000000 fastmysql-0.2.0/fastmysql.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-07-26 06:52:10.000000 fastmysql-0.2.0/fastmysql.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-07-26 06:52:10.147209 fastmysql-0.2.0/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1102 2023-07-26 06:51:37.000000 fastmysql-0.2.0/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 07:26:56.061557 fastmysql-0.2.1/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-26 07:26:56.061446 fastmysql-0.2.1/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1442 2023-02-22 07:55:41.000000 fastmysql-0.2.1/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 07:26:56.060468 fastmysql-0.2.1/fastmysql/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      238 2023-07-26 03:48:57.000000 fastmysql-0.2.1/fastmysql/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    47563 2023-07-24 10:45:49.000000 fastmysql-0.2.1/fastmysql/fastmysql.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    25529 2023-07-26 07:26:27.000000 fastmysql-0.2.1/fastmysql/fastmysql_test.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 07:26:56.061280 fastmysql-0.2.1/fastmysql.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-26 07:26:56.000000 fastmysql-0.2.1/fastmysql.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      255 2023-07-26 07:26:56.000000 fastmysql-0.2.1/fastmysql.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-07-26 07:26:56.000000 fastmysql-0.2.1/fastmysql.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      146 2023-07-26 07:26:56.000000 fastmysql-0.2.1/fastmysql.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-07-26 07:26:56.000000 fastmysql-0.2.1/fastmysql.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-07-26 07:26:56.061591 fastmysql-0.2.1/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1102 2023-07-26 07:26:11.000000 fastmysql-0.2.1/setup.py
```

### Comparing `fastmysql-0.2.0/PKG-INFO` & `fastmysql-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmysql
-Version: 0.2.0
+Version: 0.2.1
 Summary: make it easy to use pymysql
 Home-page: https://gitee.com/ZeroSeeker/fastmysql
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fastmysql-0.2.0/README.md` & `fastmysql-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fastmysql-0.2.0/fastmysql/fastmysql.py` & `fastmysql-0.2.1/fastmysql/fastmysql.py`

 * *Files identical despite different names*

### Comparing `fastmysql-0.2.0/fastmysql/fastmysql_test.py` & `fastmysql-0.2.1/fastmysql/fastmysql_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,33 +19,33 @@
 env_file_name_default = 'mysql.env'  # 默认数据库连接环境文件名
 reconnect_errors = (ConnectionError, ConnectionAbortedError, TimeoutError)
 default_charset = 'utf8'
 default_show_sql = False
 
 
 class FastMySQL:
-    # -------- 单例模式 --------
-    _instance = None
-
-    def __new__(cls, *args, **kwargs):
-        """
-        单例模式
-
-        FastMySQL 类的 _instance 类变量用于存储唯一的实例。
-        在 __new__ 方法中，首先检查 _instance 是否已经存在实例，
-        如果不存在，则使用 super() 调用父类的 __new__ 方法创建一个新实例，并将其赋值给 _instance 类变量。
-        如果已经存在实例，直接返回现有实例，确保只有一个实例存在。
-
-        使用单例模式可以有效地避免多次创建相同对象的开销，并确保全局只有一个对象实例，适用于需要共享状态或资源的场景。
-        """
-        if not cls._instance:
-            cls._instance = super(FastMySQL, cls).__new__(cls)
-            cls._instance.__init__(*args, **kwargs)
-        return cls._instance
-    # -------- 单例模式 --------
+    # # -------- 单例模式 --------
+    # _instance = None
+    #
+    # def __new__(cls, *args, **kwargs):
+    #     """
+    #     单例模式
+    #
+    #     FastMySQL 类的 _instance 类变量用于存储唯一的实例。
+    #     在 __new__ 方法中，首先检查 _instance 是否已经存在实例，
+    #     如果不存在，则使用 super() 调用父类的 __new__ 方法创建一个新实例，并将其赋值给 _instance 类变量。
+    #     如果已经存在实例，直接返回现有实例，确保只有一个实例存在。
+    #
+    #     使用单例模式可以有效地避免多次创建相同对象的开销，并确保全局只有一个对象实例，适用于需要共享状态或资源的场景。
+    #     """
+    #     if not cls._instance:
+    #         cls._instance = super(FastMySQL, cls).__new__(cls)
+    #         cls._instance.__init__(*args, **kwargs)
+    #     return cls._instance
+    # # -------- 单例模式 --------
 
     def __init__(
             self,
             env_file_name: str = env_file_name_default,
             silence: bool = silence_default,
             ssc: bool = False,
             auto_reconnect: bool = True,
```

### Comparing `fastmysql-0.2.0/fastmysql.egg-info/PKG-INFO` & `fastmysql-0.2.1/fastmysql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmysql
-Version: 0.2.0
+Version: 0.2.1
 Summary: make it easy to use pymysql
 Home-page: https://gitee.com/ZeroSeeker/fastmysql
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fastmysql-0.2.0/setup.py` & `fastmysql-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fastmysql",
-    version="0.2.0",
+    version="0.2.1",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     description="make it easy to use pymysql",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ZeroSeeker/fastmysql",
     packages=setuptools.find_packages(),
```

