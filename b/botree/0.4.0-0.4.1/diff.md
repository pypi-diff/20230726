# Comparing `tmp/botree-0.4.0.tar.gz` & `tmp/botree-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botree-0.4.0.tar", last modified: Tue Jul 25 15:31:31 2023, max compression
+gzip compressed data, was "botree-0.4.1.tar", last modified: Wed Jul 26 19:52:11 2023, max compression
```

## Comparing `botree-0.4.0.tar` & `botree-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1068 2023-07-25 14:00:58.549354 botree-0.4.0/LICENSE
--rw-r--r--   0        0        0     1507 2023-07-25 15:27:01.222710 botree-0.4.0/README.md
--rw-r--r--   0        0        0      361 2023-07-25 14:00:58.549354 botree-0.4.0/botree/__init__.py
--rw-r--r--   0        0        0     1747 2023-07-25 14:33:58.247805 botree-0.4.0/botree/core.py
--rw-r--r--   0        0        0     2103 2023-07-25 14:00:58.549354 botree-0.4.0/botree/cost_explorer.py
--rw-r--r--   0        0        0     1926 2023-07-25 14:00:58.549354 botree-0.4.0/botree/logs.py
--rw-r--r--   0        0        0     5656 2023-07-25 15:27:01.222710 botree-0.4.0/botree/s3.py
--rw-r--r--   0        0        0     6276 2023-07-25 15:27:01.222710 botree-0.4.0/botree/secrets_manager.py
--rw-r--r--   0        0        0     1511 2023-07-25 15:31:31.020294 botree-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-25 14:05:32.946672 botree-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1557 2023-07-25 14:33:58.247805 botree-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     1719 2023-07-25 15:27:01.226710 botree-0.4.0/tests/test_cost_explorer.py
--rw-r--r--   0        0        0      812 2023-07-25 15:27:01.226710 botree-0.4.0/tests/test_logs.py
--rw-r--r--   0        0        0     2030 2023-07-25 15:27:01.226710 botree-0.4.0/tests/test_s3.py
--rw-r--r--   0        0        0     2156 2023-07-25 14:33:58.247805 botree-0.4.0/tests/test_secrets_manager.py
--rw-r--r--   0        0        0     1787 1970-01-01 00:00:00.000000 botree-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-25 14:00:58.549354 botree-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1507 2023-07-25 15:27:01.222710 botree-0.4.1/README.md
+-rw-r--r--   0        0        0      361 2023-07-25 14:00:58.549354 botree-0.4.1/botree/__init__.py
+-rw-r--r--   0        0        0     1747 2023-07-25 14:33:58.247805 botree-0.4.1/botree/core.py
+-rw-r--r--   0        0        0     2103 2023-07-25 14:00:58.549354 botree-0.4.1/botree/cost_explorer.py
+-rw-r--r--   0        0        0     1926 2023-07-25 14:00:58.549354 botree-0.4.1/botree/logs.py
+-rw-r--r--   0        0        0     5656 2023-07-25 15:27:01.222710 botree-0.4.1/botree/s3.py
+-rw-r--r--   0        0        0     6276 2023-07-25 15:27:01.222710 botree-0.4.1/botree/secrets_manager.py
+-rw-r--r--   0        0        0     1510 2023-07-26 19:52:11.848744 botree-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 14:05:32.946672 botree-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     1557 2023-07-25 14:33:58.247805 botree-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     1719 2023-07-25 15:27:01.226710 botree-0.4.1/tests/test_cost_explorer.py
+-rw-r--r--   0        0        0      812 2023-07-25 15:27:01.226710 botree-0.4.1/tests/test_logs.py
+-rw-r--r--   0        0        0     2030 2023-07-25 15:27:01.226710 botree-0.4.1/tests/test_s3.py
+-rw-r--r--   0        0        0     2156 2023-07-25 14:33:58.247805 botree-0.4.1/tests/test_secrets_manager.py
+-rw-r--r--   0        0        0     1786 1970-01-01 00:00:00.000000 botree-0.4.1/PKG-INFO
```

### Comparing `botree-0.4.0/LICENSE` & `botree-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `botree-0.4.0/README.md` & `botree-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `botree-0.4.0/botree/core.py` & `botree-0.4.1/botree/core.py`

 * *Files identical despite different names*

### Comparing `botree-0.4.0/botree/cost_explorer.py` & `botree-0.4.1/botree/cost_explorer.py`

 * *Files identical despite different names*

### Comparing `botree-0.4.0/botree/logs.py` & `botree-0.4.1/botree/logs.py`

 * *Files identical despite different names*

### Comparing `botree-0.4.0/botree/s3.py` & `botree-0.4.1/botree/s3.py`

 * *Files identical despite different names*

### Comparing `botree-0.4.0/botree/secrets_manager.py` & `botree-0.4.1/botree/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `botree-0.4.0/pyproject.toml` & `botree-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "botree"
-version = "0.4.0"
+version = "0.4.1"
 description = "A friendly wrapper for boto3."
 authors = [
     { name = "ericmiguel", email = "eric.mrib@gmail.com" },
 ]
 dependencies = [
     "boto3>=1.28.10",
     "boto3-stubs>=1.28.10",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [tool.isort]
 profile = "black"
```

### Comparing `botree-0.4.0/tests/conftest.py` & `botree-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `botree-0.4.0/tests/test_cost_explorer.py` & `botree-0.4.1/tests/test_cost_explorer.py`

 * *Files identical despite different names*

### Comparing `botree-0.4.0/tests/test_logs.py` & `botree-0.4.1/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `botree-0.4.0/tests/test_s3.py` & `botree-0.4.1/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `botree-0.4.0/tests/test_secrets_manager.py` & `botree-0.4.1/tests/test_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `botree-0.4.0/PKG-INFO` & `botree-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: botree
-Version: 0.4.0
+Version: 0.4.1
 Summary: A friendly wrapper for boto3.
 Author-Email: ericmiguel <eric.mrib@gmail.com>
 License: MIT
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Requires-Dist: boto3>=1.28.10
 Requires-Dist: boto3-stubs>=1.28.10
 Description-Content-Type: text/markdown
 
 # Botree: a friendly wrapper for boto3
 
 Botree is a higher level API for AWS services / Boto3 classes and aims to make Boto3 experience easier.
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: botree Version: 0.4.0 Summary: A friendly wrapper
+Metadata-Version: 2.1 Name: botree Version: 0.4.1 Summary: A friendly wrapper
 for boto3. Author-Email: ericmiguel
-mrib@gmail.com> License: MIT Requires-Python: >=3.10 Requires-Dist:
+mrib@gmail.com> License: MIT Requires-Python: >=3.9 Requires-Dist:
 boto3>=1.28.10 Requires-Dist: boto3-stubs>=1.28.10 Description-Content-Type:
 text/markdown # Botree: a friendly wrapper for boto3 Botree is a higher level
 API for AWS services / Boto3 classes and aims to make Boto3 experience easier.
 ## ð§° Supported AWS services Currently, there are just some Boto3 wrapped
 classes. - âï¸ S3 - âï¸ Secrets - âï¸ CloudWatch - âï¸ Cost
 Explorer - âï¸ Secrets Manager ## ð» Basic usage To start a Botree
 session, use the following: ```Python import botree session = botree.session
```

