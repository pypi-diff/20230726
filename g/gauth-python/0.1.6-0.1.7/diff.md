# Comparing `tmp/gauth_python-0.1.6.tar.gz` & `tmp/gauth_python-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauth_python-0.1.6.tar", last modified: Wed Jul 26 11:10:03 2023, max compression
+gzip compressed data, was "gauth_python-0.1.7.tar", last modified: Wed Jul 26 11:15:32 2023, max compression
```

## Comparing `gauth_python-0.1.6.tar` & `gauth_python-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 11:10:03.010054 gauth_python-0.1.6/
--rw-r--r--   0 yohan      (501) staff       (20)     1061 2023-07-26 08:05:07.000000 gauth_python-0.1.6/LICENSE
--rw-r--r--   0 yohan      (501) staff       (20)     2424 2023-07-26 11:10:03.009904 gauth_python-0.1.6/PKG-INFO
--rw-r--r--   0 yohan      (501) staff       (20)     1960 2023-07-26 11:07:34.000000 gauth_python-0.1.6/README.md
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 11:10:03.008757 gauth_python-0.1.6/gauth_python/
--rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 10:32:26.000000 gauth_python-0.1.6/gauth_python/__init__.py
--rw-r--r--   0 yohan      (501) staff       (20)     1342 2023-07-26 11:04:45.000000 gauth_python-0.1.6/gauth_python/requests.py
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 11:10:03.009364 gauth_python-0.1.6/gauth_python.egg-info/
--rw-r--r--   0 yohan      (501) staff       (20)     2424 2023-07-26 11:10:02.000000 gauth_python-0.1.6/gauth_python.egg-info/PKG-INFO
--rw-r--r--   0 yohan      (501) staff       (20)      300 2023-07-26 11:10:02.000000 gauth_python-0.1.6/gauth_python.egg-info/SOURCES.txt
--rw-r--r--   0 yohan      (501) staff       (20)        1 2023-07-26 11:10:02.000000 gauth_python-0.1.6/gauth_python.egg-info/dependency_links.txt
--rw-r--r--   0 yohan      (501) staff       (20)        9 2023-07-26 11:10:02.000000 gauth_python-0.1.6/gauth_python.egg-info/requires.txt
--rw-r--r--   0 yohan      (501) staff       (20)       19 2023-07-26 11:10:02.000000 gauth_python-0.1.6/gauth_python.egg-info/top_level.txt
--rw-r--r--   0 yohan      (501) staff       (20)       38 2023-07-26 11:10:03.010099 gauth_python-0.1.6/setup.cfg
--rw-r--r--   0 yohan      (501) staff       (20)      815 2023-07-26 11:05:01.000000 gauth_python-0.1.6/setup.py
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 11:10:03.009580 gauth_python-0.1.6/tests/
--rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 08:46:30.000000 gauth_python-0.1.6/tests/__init__.py
--rw-r--r--   0 yohan      (501) staff       (20)      296 2023-07-26 10:49:49.000000 gauth_python-0.1.6/tests/test_gauth_python.py
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 11:15:32.649754 gauth_python-0.1.7/
+-rw-r--r--   0 yohan      (501) staff       (20)     1061 2023-07-26 08:05:07.000000 gauth_python-0.1.7/LICENSE
+-rw-r--r--   0 yohan      (501) staff       (20)     2423 2023-07-26 11:15:32.649600 gauth_python-0.1.7/PKG-INFO
+-rw-r--r--   0 yohan      (501) staff       (20)     1959 2023-07-26 11:12:40.000000 gauth_python-0.1.7/README.md
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 11:15:32.648363 gauth_python-0.1.7/gauth_python/
+-rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 10:32:26.000000 gauth_python-0.1.7/gauth_python/__init__.py
+-rw-r--r--   0 yohan      (501) staff       (20)     1342 2023-07-26 11:04:45.000000 gauth_python-0.1.7/gauth_python/requests.py
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 11:15:32.648970 gauth_python-0.1.7/gauth_python.egg-info/
+-rw-r--r--   0 yohan      (501) staff       (20)     2423 2023-07-26 11:15:32.000000 gauth_python-0.1.7/gauth_python.egg-info/PKG-INFO
+-rw-r--r--   0 yohan      (501) staff       (20)      300 2023-07-26 11:15:32.000000 gauth_python-0.1.7/gauth_python.egg-info/SOURCES.txt
+-rw-r--r--   0 yohan      (501) staff       (20)        1 2023-07-26 11:15:32.000000 gauth_python-0.1.7/gauth_python.egg-info/dependency_links.txt
+-rw-r--r--   0 yohan      (501) staff       (20)        9 2023-07-26 11:15:32.000000 gauth_python-0.1.7/gauth_python.egg-info/requires.txt
+-rw-r--r--   0 yohan      (501) staff       (20)       19 2023-07-26 11:15:32.000000 gauth_python-0.1.7/gauth_python.egg-info/top_level.txt
+-rw-r--r--   0 yohan      (501) staff       (20)       38 2023-07-26 11:15:32.649803 gauth_python-0.1.7/setup.cfg
+-rw-r--r--   0 yohan      (501) staff       (20)      815 2023-07-26 11:15:27.000000 gauth_python-0.1.7/setup.py
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 11:15:32.649174 gauth_python-0.1.7/tests/
+-rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 08:46:30.000000 gauth_python-0.1.7/tests/__init__.py
+-rw-r--r--   0 yohan      (501) staff       (20)      296 2023-07-26 10:49:49.000000 gauth_python-0.1.7/tests/test_gauth_python.py
```

### Comparing `gauth_python-0.1.6/LICENSE` & `gauth_python-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gauth_python-0.1.6/PKG-INFO` & `gauth_python-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauth_python
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python sdk from Gauth.
 Home-page: https://github.com/GSM-MSG/GAuth-SDK-Python
 Author: Noh Gaseong
 Author-email: dev.yohan05@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GAuth-Python
 
->> 단 하나의 계정으로 모든 GSM의 서비스를 이용할 수 있게.
+> 단 하나의 계정으로 모든 GSM의 서비스를 이용할 수 있게.
 
 ```
       ___           ___           ___                       ___     
      /  /\         /  /\         /__/\          ___        /__/\    
     /  /:/_       /  /::\        \  \:\        /  /\       \  \:\   
    /  /:/ /\     /  /:/\:\        \  \:\      /  /:/        \__\:\  
   /  /:/_/::\   /  /:/ /::\   ___  \  \:\    /  /:/     ___ /  /::\
```

### Comparing `gauth_python-0.1.6/README.md` & `gauth_python-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # GAuth-Python
 
->> 단 하나의 계정으로 모든 GSM의 서비스를 이용할 수 있게.
+> 단 하나의 계정으로 모든 GSM의 서비스를 이용할 수 있게.
 
 ```
       ___           ___           ___                       ___     
      /  /\         /  /\         /__/\          ___        /__/\    
     /  /:/_       /  /::\        \  \:\        /  /\       \  \:\   
    /  /:/ /\     /  /:/\:\        \  \:\      /  /:/        \__\:\  
   /  /:/_/::\   /  /:/ /::\   ___  \  \:\    /  /:/     ___ /  /::\
```

### Comparing `gauth_python-0.1.6/gauth_python/requests.py` & `gauth_python-0.1.7/gauth_python/requests.py`

 * *Files identical despite different names*

### Comparing `gauth_python-0.1.6/gauth_python.egg-info/PKG-INFO` & `gauth_python-0.1.7/gauth_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauth-python
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python sdk from Gauth.
 Home-page: https://github.com/GSM-MSG/GAuth-SDK-Python
 Author: Noh Gaseong
 Author-email: dev.yohan05@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GAuth-Python
 
->> 단 하나의 계정으로 모든 GSM의 서비스를 이용할 수 있게.
+> 단 하나의 계정으로 모든 GSM의 서비스를 이용할 수 있게.
 
 ```
       ___           ___           ___                       ___     
      /  /\         /  /\         /__/\          ___        /__/\    
     /  /:/_       /  /::\        \  \:\        /  /\       \  \:\   
    /  /:/ /\     /  /:/\:\        \  \:\      /  /:/        \__\:\  
   /  /:/_/::\   /  /:/ /::\   ___  \  \:\    /  /:/     ___ /  /::\
```

### Comparing `gauth_python-0.1.6/setup.py` & `gauth_python-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='gauth_python',
-    version='0.1.6',
+    version='0.1.7',
     description='Python sdk from Gauth.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = "https://github.com/GSM-MSG/GAuth-SDK-Python",
     packages=setuptools.find_packages(),
     classifiers = [        
         "Programming Language :: Python :: 3",
```

