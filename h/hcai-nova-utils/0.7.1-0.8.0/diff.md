# Comparing `tmp/hcai-nova-utils-0.7.1.tar.gz` & `tmp/hcai-nova-utils-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-utils-0.7.1.tar", last modified: Thu Jun 22 07:31:50 2023, max compression
+gzip compressed data, was "hcai-nova-utils-0.8.0.tar", last modified: Wed Jul 26 13:35:06 2023, max compression
```

## Comparing `hcai-nova-utils-0.7.1.tar` & `hcai-nova-utils-0.8.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-22 07:31:50.000000 hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-22 07:31:50.000000 hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 07:31:50.000000 hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-22 07:31:50.000000 hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-22 07:31:50.000000 hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/nova_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/nova_utils/db_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/db_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/db_utils/nova_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/nova_utils/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      616 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/interfaces/dataset_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)     5915 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/interfaces/server_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/nova_utils/ssi_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/ssi_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7930 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_data_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     3749 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_sample_list_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4545 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8551 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_xml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/nova_utils/storage_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/storage_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/nova_utils/storage_utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 07:31:50.654689 hcai-nova-utils-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-06-22 07:31:42.000000 hcai-nova-utils-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:35:06.315693 hcai-nova-utils-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-07-26 13:35:06.315693 hcai-nova-utils-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:35:06.315693 hcai-nova-utils-0.8.0/hcai_nova_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-07-26 13:35:06.000000 hcai-nova-utils-0.8.0/hcai_nova_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-07-26 13:35:06.000000 hcai-nova-utils-0.8.0/hcai_nova_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 13:35:06.000000 hcai-nova-utils-0.8.0/hcai_nova_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-26 13:35:06.000000 hcai-nova-utils-0.8.0/hcai_nova_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-26 13:35:06.000000 hcai-nova-utils-0.8.0/hcai_nova_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:35:06.315693 hcai-nova-utils-0.8.0/nova_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/nova_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:35:06.315693 hcai-nova-utils-0.8.0/nova_utils/db_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/nova_utils/db_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/nova_utils/db_utils/nova_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:35:06.315693 hcai-nova-utils-0.8.0/nova_utils/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/nova_utils/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      616 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/nova_utils/interfaces/dataset_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5915 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/nova_utils/interfaces/server_module.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:35:06.315693 hcai-nova-utils-0.8.0/nova_utils/ssi_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/nova_utils/ssi_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7927 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/nova_utils/ssi_utils/ssi_anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/nova_utils/ssi_utils/ssi_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3749 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/nova_utils/ssi_utils/ssi_sample_list_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4545 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/nova_utils/ssi_utils/ssi_stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8551 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/nova_utils/ssi_utils/ssi_xml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:35:06.315693 hcai-nova-utils-0.8.0/nova_utils/storage_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/nova_utils/storage_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/nova_utils/storage_utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-26 13:35:06.315693 hcai-nova-utils-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-07-26 13:34:55.000000 hcai-nova-utils-0.8.0/setup.py
```

### Comparing `hcai-nova-utils-0.7.1/PKG-INFO` & `hcai-nova-utils-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-utils
-Version: 0.7.1
+Version: 0.8.0
 Summary: This repository contains utility functions and interfaces that can be used to interact with the NOVA annotation tool.
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/PKG-INFO` & `hcai-nova-utils-0.8.0/hcai_nova_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-utils
-Version: 0.7.1
+Version: 0.8.0
 Summary: This repository contains utility functions and interfaces that can be used to interact with the NOVA annotation tool.
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcai-nova-utils-0.7.1/hcai_nova_utils.egg-info/SOURCES.txt` & `hcai-nova-utils-0.8.0/hcai_nova_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.1/nova_utils/db_utils/nova_types.py` & `hcai-nova-utils-0.8.0/nova_utils/db_utils/nova_types.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.1/nova_utils/interfaces/dataset_iterable.py` & `hcai-nova-utils-0.8.0/nova_utils/interfaces/dataset_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.1/nova_utils/interfaces/server_module.py` & `hcai-nova-utils-0.8.0/nova_utils/interfaces/server_module.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_anno_utils.py` & `hcai-nova-utils-0.8.0/nova_utils/ssi_utils/ssi_anno_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class LabelDataType(Enum):
     DISCRETE = np.dtype(
         [
             ("from", np.float64),
             ("to", np.float64),
-            ("class", np.int32),
+            ("id", np.int32),
             ("conf", np.float32),
         ]
     )  # {'names':('from', 'to', 'name', 'conf'),
 
     FREE = np.dtype(
         [
             ("from", np.float64),
```

### Comparing `hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_data_types.py` & `hcai-nova-utils-0.8.0/nova_utils/ssi_utils/ssi_data_types.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_sample_list_utils.py` & `hcai-nova-utils-0.8.0/nova_utils/ssi_utils/ssi_sample_list_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_stream_utils.py` & `hcai-nova-utils-0.8.0/nova_utils/ssi_utils/ssi_stream_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.1/nova_utils/ssi_utils/ssi_xml_utils.py` & `hcai-nova-utils-0.8.0/nova_utils/ssi_utils/ssi_xml_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.1/nova_utils/storage_utils/cache.py` & `hcai-nova-utils-0.8.0/nova_utils/storage_utils/cache.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.7.1/setup.py` & `hcai-nova-utils-0.8.0/setup.py`

 * *Files identical despite different names*

