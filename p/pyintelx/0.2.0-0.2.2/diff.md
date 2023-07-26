# Comparing `tmp/pyintelx-0.2.0.tar.gz` & `tmp/pyintelx-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyintelx-0.2.0.tar", last modified: Wed Jun 28 15:48:05 2023, max compression
+gzip compressed data, was "pyintelx-0.2.2.tar", last modified: Wed Jul 26 18:36:49 2023, max compression
```

## Comparing `pyintelx-0.2.0.tar` & `pyintelx-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:48:05.280073 pyintelx-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-28 15:48:05.280073 pyintelx-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-28 15:47:55.000000 pyintelx-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:48:05.280073 pyintelx-0.2.0/pyintelx/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 15:47:55.000000 pyintelx-0.2.0/pyintelx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:48:05.280073 pyintelx-0.2.0/pyintelx/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-06-28 15:47:55.000000 pyintelx-0.2.0/pyintelx/cli/pyintelx
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-28 15:47:55.000000 pyintelx-0.2.0/pyintelx/pyintelx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:48:05.280073 pyintelx-0.2.0/pyintelx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-28 15:48:05.000000 pyintelx-0.2.0/pyintelx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-28 15:48:05.000000 pyintelx-0.2.0/pyintelx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 15:48:05.000000 pyintelx-0.2.0/pyintelx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-28 15:48:05.000000 pyintelx-0.2.0/pyintelx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 15:48:05.280073 pyintelx-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-28 15:47:55.000000 pyintelx-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:36:49.294386 pyintelx-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-26 18:36:49.294386 pyintelx-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-26 18:36:38.000000 pyintelx-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:36:49.294386 pyintelx-0.2.2/pyintelx/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-26 18:36:38.000000 pyintelx-0.2.2/pyintelx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:36:49.294386 pyintelx-0.2.2/pyintelx/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-07-26 18:36:38.000000 pyintelx-0.2.2/pyintelx/cli/pyintelx
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-26 18:36:38.000000 pyintelx-0.2.2/pyintelx/pyintelx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:36:49.294386 pyintelx-0.2.2/pyintelx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-26 18:36:49.000000 pyintelx-0.2.2/pyintelx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-26 18:36:49.000000 pyintelx-0.2.2/pyintelx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:36:49.000000 pyintelx-0.2.2/pyintelx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 18:36:49.000000 pyintelx-0.2.2/pyintelx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 18:36:49.294386 pyintelx-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-26 18:36:38.000000 pyintelx-0.2.2/setup.py
```

### Comparing `pyintelx-0.2.0/PKG-INFO` & `pyintelx-0.2.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintelx
-Version: 0.2.0
+Version: 0.2.2
 Summary: This lib add support to use the Identity API from Intelx.io
 Home-page: https://github.com/csirtamericas/pyintelxio
 Author: Fermin Baudino, Einar Lanfranco, Federico Carrilao
 License: MIT
 Keywords: python, package, distribution
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -65,25 +65,45 @@
 
 Usage as library
 ================
 
 * Print account information
 
 ```python
-import pyintelx
-api = 
+from pyintelx import intelx
+API_KEY = "your api key"
 
+intelx_service = intelx(API_KEY)
+
+intelx_service.GET_CAPABILITIES()
+
+```
+
+* Search for using intelx service
+
+```python
+from pyintelx import intelx
+API_KEY = "your api key"
+
+intelx_service = intelx(API_KEY)
+intelx_service.search("example@example.com", maxresults=max_results, datefrom=date_from, dateto=date_to, buckets=[])
 ```
 
-* Search for 
+* Search for using identity service
 
 ```python
-import pyintelx
+from pyintelx import IdentityService
+API_KEY = "your api key"
+
+identity_service = IdentityService(API_KEY)
+
+identity_service.search("example@example.com", maxresults=max_results, datefrom=date_from, dateto=date_to, buckets=[])
 ```
 
+
 ## Buckets list
 - darknet.tor
 - darknet.i2p
 - documents.public.scihub
 - dumpster
 - leaks.private.general
 - leaks.public.general
```

### Comparing `pyintelx-0.2.0/README.md` & `pyintelx-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -49,25 +49,45 @@
 
 Usage as library
 ================
 
 * Print account information
 
 ```python
-import pyintelx
-api = 
+from pyintelx import intelx
+API_KEY = "your api key"
 
+intelx_service = intelx(API_KEY)
+
+intelx_service.GET_CAPABILITIES()
+
+```
+
+* Search for using intelx service
+
+```python
+from pyintelx import intelx
+API_KEY = "your api key"
+
+intelx_service = intelx(API_KEY)
+intelx_service.search("example@example.com", maxresults=max_results, datefrom=date_from, dateto=date_to, buckets=[])
 ```
 
-* Search for 
+* Search for using identity service
 
 ```python
-import pyintelx
+from pyintelx import IdentityService
+API_KEY = "your api key"
+
+identity_service = IdentityService(API_KEY)
+
+identity_service.search("example@example.com", maxresults=max_results, datefrom=date_from, dateto=date_to, buckets=[])
 ```
 
+
 ## Buckets list
 - darknet.tor
 - darknet.i2p
 - documents.public.scihub
 - dumpster
 - leaks.private.general
 - leaks.public.general
```

### Comparing `pyintelx-0.2.0/pyintelx/cli/pyintelx` & `pyintelx-0.2.2/pyintelx/cli/pyintelx`

 * *Files identical despite different names*

### Comparing `pyintelx-0.2.0/pyintelx/pyintelx.py` & `pyintelx-0.2.2/pyintelx/pyintelx.py`

 * *Files identical despite different names*

### Comparing `pyintelx-0.2.0/pyintelx.egg-info/PKG-INFO` & `pyintelx-0.2.2/pyintelx.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintelx
-Version: 0.2.0
+Version: 0.2.2
 Summary: This lib add support to use the Identity API from Intelx.io
 Home-page: https://github.com/csirtamericas/pyintelxio
 Author: Fermin Baudino, Einar Lanfranco, Federico Carrilao
 License: MIT
 Keywords: python, package, distribution
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -65,25 +65,45 @@
 
 Usage as library
 ================
 
 * Print account information
 
 ```python
-import pyintelx
-api = 
+from pyintelx import intelx
+API_KEY = "your api key"
 
+intelx_service = intelx(API_KEY)
+
+intelx_service.GET_CAPABILITIES()
+
+```
+
+* Search for using intelx service
+
+```python
+from pyintelx import intelx
+API_KEY = "your api key"
+
+intelx_service = intelx(API_KEY)
+intelx_service.search("example@example.com", maxresults=max_results, datefrom=date_from, dateto=date_to, buckets=[])
 ```
 
-* Search for 
+* Search for using identity service
 
 ```python
-import pyintelx
+from pyintelx import IdentityService
+API_KEY = "your api key"
+
+identity_service = IdentityService(API_KEY)
+
+identity_service.search("example@example.com", maxresults=max_results, datefrom=date_from, dateto=date_to, buckets=[])
 ```
 
+
 ## Buckets list
 - darknet.tor
 - darknet.i2p
 - documents.public.scihub
 - dumpster
 - leaks.private.general
 - leaks.public.general
```

### Comparing `pyintelx-0.2.0/setup.py` & `pyintelx-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 
 setup(
     name='pyintelx',
-    version='0.2.0',
+    version='0.2.2',
     description='This lib add support to use the Identity API from Intelx.io',
     license='MIT',
     keywords=['python, package, distribution'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Fermin Baudino, Einar Lanfranco, Federico Carrilao',
     url='https://github.com/csirtamericas/pyintelxio',
```

