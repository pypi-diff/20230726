# Comparing `tmp/quantfactortest-1.1.tar.gz` & `tmp/quantfactortest-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantfactortest-1.1.tar", last modified: Wed Jul 26 01:55:37 2023, max compression
+gzip compressed data, was "quantfactortest-1.2.tar", last modified: Wed Jul 26 02:52:43 2023, max compression
```

## Comparing `quantfactortest-1.1.tar` & `quantfactortest-1.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 01:55:37.637673 quantfactortest-1.1/
--rw-rw-rw-   0        0        0      597 2023-07-26 01:55:37.635681 quantfactortest-1.1/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-07-19 02:18:20.000000 quantfactortest-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 01:55:37.634684 quantfactortest-1.1/quantfactortest.egg-info/
--rw-rw-rw-   0        0        0      597 2023-07-26 01:55:37.000000 quantfactortest-1.1/quantfactortest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-07-26 01:55:37.000000 quantfactortest-1.1/quantfactortest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 01:55:37.000000 quantfactortest-1.1/quantfactortest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-26 01:55:37.000000 quantfactortest-1.1/quantfactortest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 01:55:37.000000 quantfactortest-1.1/quantfactortest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 01:55:37.637673 quantfactortest-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1354 2023-07-26 01:55:25.000000 quantfactortest-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 02:52:43.929515 quantfactortest-1.2/
+-rw-rw-rw-   0        0        0      597 2023-07-26 02:52:43.928518 quantfactortest-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-07-19 02:18:20.000000 quantfactortest-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 02:52:43.928518 quantfactortest-1.2/quantfactortest.egg-info/
+-rw-rw-rw-   0        0        0      597 2023-07-26 02:52:43.000000 quantfactortest-1.2/quantfactortest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-07-26 02:52:43.000000 quantfactortest-1.2/quantfactortest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 02:52:43.000000 quantfactortest-1.2/quantfactortest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-26 02:52:43.000000 quantfactortest-1.2/quantfactortest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-26 02:52:43.000000 quantfactortest-1.2/quantfactortest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    39995 2023-07-26 01:52:13.000000 quantfactortest-1.2/quantfactortest.py
+-rw-rw-rw-   0        0        0       42 2023-07-26 02:52:43.929515 quantfactortest-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1353 2023-07-26 02:52:30.000000 quantfactortest-1.2/setup.py
```

### Comparing `quantfactortest-1.1/PKG-INFO` & `quantfactortest-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantfactortest
-Version: 1.1
+Version: 1.2
 Summary: 单因子的测试（日级别and分钟级别）,非交互式
 Home-page: https://github.com/Masteryeda
 Author: IDEA_Wenzhi
 Author-email: 1259429314@qq.com
 Maintainer: IDEA_Wenzhi
 Maintainer-email: 1259429314@qq.com
 License: MIT License
```

### Comparing `quantfactortest-1.1/quantfactortest.egg-info/PKG-INFO` & `quantfactortest-1.2/quantfactortest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantfactortest
-Version: 1.1
+Version: 1.2
 Summary: 单因子的测试（日级别and分钟级别）,非交互式
 Home-page: https://github.com/Masteryeda
 Author: IDEA_Wenzhi
 Author-email: 1259429314@qq.com
 Maintainer: IDEA_Wenzhi
 Maintainer-email: 1259429314@qq.com
 License: MIT License
```

### Comparing `quantfactortest-1.1/setup.py` & `quantfactortest-1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
  
 setup(
     name='quantfactortest',#包名
-    version='1.1',#版本
+    version='1.2',#版本
     description="单因子的测试（日级别and分钟级别）,非交互式",#包简介
     long_description=open('README.md').read(),#读取文件中介绍包的详细内容
     include_package_data=True,#是否允许上传资源文件
     author='IDEA_Wenzhi',#作者
     author_email='1259429314@qq.com',#作者邮件
     maintainer='IDEA_Wenzhi',#维护者
     maintainer_email='1259429314@qq.com',#维护者邮件
@@ -24,10 +24,10 @@
     install_requires=['pandas',
                       "numpy",
                       "statsmodels",
                       "matplotlib",
                       "seaborn",
                       "scipy",
                       "baostock"],#安装所需要的库
-    py_modules=['singlefactortest']
+    py_modules=['quantfactortest']
     )
```

