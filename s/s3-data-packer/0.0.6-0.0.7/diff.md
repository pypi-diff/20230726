# Comparing `tmp/s3_data_packer-0.0.6.tar.gz` & `tmp/s3_data_packer-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3_data_packer-0.0.6.tar", max compression
+gzip compressed data, was "s3_data_packer-0.0.7.tar", max compression
```

## Comparing `s3_data_packer-0.0.6.tar` & `s3_data_packer-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      613 2022-10-12 17:57:52.454141 s3_data_packer-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       22 2022-10-12 17:57:52.454141 s3_data_packer-0.0.6/s3_data_packer/__init__.py
--rw-r--r--   0        0        0      162 2022-10-12 17:57:52.454141 s3_data_packer-0.0.6/s3_data_packer/constants.py
--rw-r--r--   0        0        0     1489 2022-10-12 17:57:52.454141 s3_data_packer-0.0.6/s3_data_packer/helpers.py
--rw-r--r--   0        0        0     8832 2022-10-12 17:57:52.454141 s3_data_packer-0.0.6/s3_data_packer/s3_data_packer.py
--rw-r--r--   0        0        0     4998 2022-10-12 17:57:52.454141 s3_data_packer-0.0.6/s3_data_packer/s3_output_store.py
--rw-r--r--   0        0        0     3484 2022-10-12 17:57:52.454141 s3_data_packer-0.0.6/s3_data_packer/s3_table_store.py
--rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 s3_data_packer-0.0.6/setup.py
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 s3_data_packer-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      610 2023-07-26 10:23:40.028367 s3_data_packer-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-26 10:23:40.028367 s3_data_packer-0.0.7/s3_data_packer/__init__.py
+-rw-r--r--   0        0        0      162 2023-07-26 10:23:40.028367 s3_data_packer-0.0.7/s3_data_packer/constants.py
+-rw-r--r--   0        0        0     1489 2023-07-26 10:23:40.028367 s3_data_packer-0.0.7/s3_data_packer/helpers.py
+-rw-r--r--   0        0        0     8832 2023-07-26 10:23:40.028367 s3_data_packer-0.0.7/s3_data_packer/s3_data_packer.py
+-rw-r--r--   0        0        0     4998 2023-07-26 10:23:40.028367 s3_data_packer-0.0.7/s3_data_packer/s3_output_store.py
+-rw-r--r--   0        0        0     3484 2023-07-26 10:23:40.028367 s3_data_packer-0.0.7/s3_data_packer/s3_table_store.py
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 s3_data_packer-0.0.7/PKG-INFO
```

### Comparing `s3_data_packer-0.0.6/pyproject.toml` & `s3_data_packer-0.0.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "s3_data_packer"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = [
     "s-ducks <stephen.bias@digital.justice.gov.uk>",
     "dataengineering <dataengineering@digital.justice.gov.uk>",
     "danjiv <danjiv.ramkhalawon@digital.justice.gov.uk>"
 ]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<4"
 dataengineeringutils3 = "^1.2.1"
 arrow-pd-parser = "^1.3.0"
 awswrangler = "^2.11.0"
 mojap-metadata = "^1.10.0"
 numpy = "^1.22"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `s3_data_packer-0.0.6/s3_data_packer/helpers.py` & `s3_data_packer-0.0.7/s3_data_packer/helpers.py`

 * *Files identical despite different names*

### Comparing `s3_data_packer-0.0.6/s3_data_packer/s3_data_packer.py` & `s3_data_packer-0.0.7/s3_data_packer/s3_data_packer.py`

 * *Files identical despite different names*

### Comparing `s3_data_packer-0.0.6/s3_data_packer/s3_output_store.py` & `s3_data_packer-0.0.7/s3_data_packer/s3_output_store.py`

 * *Files identical despite different names*

### Comparing `s3_data_packer-0.0.6/s3_data_packer/s3_table_store.py` & `s3_data_packer-0.0.7/s3_data_packer/s3_table_store.py`

 * *Files identical despite different names*

### Comparing `s3_data_packer-0.0.6/PKG-INFO` & `s3_data_packer-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: s3-data-packer
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 License: MIT
 Author: s-ducks
 Author-email: stephen.bias@digital.justice.gov.uk
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arrow-pd-parser (>=1.3.0,<2.0.0)
 Requires-Dist: awswrangler (>=2.11.0,<3.0.0)
 Requires-Dist: dataengineeringutils3 (>=1.2.1,<2.0.0)
 Requires-Dist: mojap-metadata (>=1.10.0,<2.0.0)
 Requires-Dist: numpy (>=1.22,<2.0)
```

