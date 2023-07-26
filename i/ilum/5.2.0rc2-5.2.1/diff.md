# Comparing `tmp/ilum-5.2.0rc2.tar.gz` & `tmp/ilum-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilum-5.2.0rc2.tar", last modified: Tue Jul 25 07:16:27 2023, max compression
+gzip compressed data, was "ilum-5.2.1.tar", last modified: Wed Jul 26 12:53:45 2023, max compression
```

## Comparing `ilum-5.2.0rc2.tar` & `ilum-5.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-07-25 07:16:27.980725 ilum-5.2.0rc2/
--rw-r--r--   0 runner    (1001) runner    (1001)     2240 2023-07-25 07:16:27.979725 ilum-5.2.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)     1512 2023-07-25 07:08:41.000000 ilum-5.2.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-07-25 07:16:27.978726 ilum-5.2.0rc2/ilum/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-07-25 07:08:41.000000 ilum-5.2.0rc2/ilum/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      642 2023-07-25 07:08:41.000000 ilum-5.2.0rc2/ilum/api.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-07-25 07:16:27.979725 ilum-5.2.0rc2/ilum.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     2240 2023-07-25 07:16:27.000000 ilum-5.2.0rc2/ilum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      159 2023-07-25 07:16:27.000000 ilum-5.2.0rc2/ilum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-07-25 07:16:27.000000 ilum-5.2.0rc2/ilum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        5 2023-07-25 07:16:27.000000 ilum-5.2.0rc2/ilum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2023-07-25 07:16:27.980725 ilum-5.2.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)     1076 2023-07-25 07:15:36.000000 ilum-5.2.0rc2/setup.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-07-26 12:53:45.492216 ilum-5.2.1/
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2241 2023-07-26 12:53:45.492216 ilum-5.2.1/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1516 2023-07-26 12:43:50.000000 ilum-5.2.1/README.md
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-07-26 12:53:45.492216 ilum-5.2.1/ilum/
+-rw-rw-r--   0 oem      (29999) oem      (29999)        0 2023-07-26 08:27:37.000000 ilum-5.2.1/ilum/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)      642 2023-07-26 08:27:37.000000 ilum-5.2.1/ilum/api.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-07-26 12:53:45.492216 ilum-5.2.1/ilum.egg-info/
+-rw-rw-r--   0 oem      (29999) oem      (29999)     2241 2023-07-26 12:53:45.000000 ilum-5.2.1/ilum.egg-info/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)      159 2023-07-26 12:53:45.000000 ilum-5.2.1/ilum.egg-info/SOURCES.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)        1 2023-07-26 12:53:45.000000 ilum-5.2.1/ilum.egg-info/dependency_links.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)        5 2023-07-26 12:53:45.000000 ilum-5.2.1/ilum.egg-info/top_level.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)       38 2023-07-26 12:53:45.492216 ilum-5.2.1/setup.cfg
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1072 2023-07-26 12:52:06.000000 ilum-5.2.1/setup.py
```

### Comparing `ilum-5.2.0rc2/PKG-INFO` & `ilum-5.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilum
-Version: 5.2.0rc2
+Version: 5.2.1
 Summary: Ilum job python api
 Home-page: https://ilum.cloud
 Author: Ilum Labs LLC
 Author-email: info@ilum.cloud
 License: apache-2.0
 Project-URL: Documentation, https://ilum.cloud/docs/
 Project-URL: API Ref, https://ilum.cloud/docs/api/
@@ -31,15 +31,15 @@
 pip install ilum
 ```
 
 ## Usage
 Here's a simple example of how to use it:
 
 ```python
-from ilum import IlumJob
+from ilum.api import IlumJob
 from random import random
 from operator import add
 
 
 class SparkPiInteractiveExample(IlumJob):
 
     def run(self, spark, config):
```

### Comparing `ilum-5.2.0rc2/README.md` & `ilum-5.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 pip install ilum
 ```
 
 ## Usage
 Here's a simple example of how to use it:
 
 ```python
-from ilum import IlumJob
+from ilum.api import IlumJob
 from random import random
 from operator import add
 
 
 class SparkPiInteractiveExample(IlumJob):
 
     def run(self, spark, config):
```

### Comparing `ilum-5.2.0rc2/ilum/api.py` & `ilum-5.2.1/ilum/api.py`

 * *Files identical despite different names*

### Comparing `ilum-5.2.0rc2/ilum.egg-info/PKG-INFO` & `ilum-5.2.1/ilum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilum
-Version: 5.2.0rc2
+Version: 5.2.1
 Summary: Ilum job python api
 Home-page: https://ilum.cloud
 Author: Ilum Labs LLC
 Author-email: info@ilum.cloud
 License: apache-2.0
 Project-URL: Documentation, https://ilum.cloud/docs/
 Project-URL: API Ref, https://ilum.cloud/docs/api/
@@ -31,15 +31,15 @@
 pip install ilum
 ```
 
 ## Usage
 Here's a simple example of how to use it:
 
 ```python
-from ilum import IlumJob
+from ilum.api import IlumJob
 from random import random
 from operator import add
 
 
 class SparkPiInteractiveExample(IlumJob):
 
     def run(self, spark, config):
```

### Comparing `ilum-5.2.0rc2/setup.py` & `ilum-5.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ilum",
-    version="5.2.0-RC2",
+    version="5.2.1",
     packages=find_packages(),
     package_data={"": ["ilum/*"]},
     url="https://ilum.cloud",
     author="Ilum Labs LLC",
     author_email="info@ilum.cloud",
     description="Ilum job python api",
     long_description=long_description,
```

