# Comparing `tmp/moneywiz-api-0.0.2.tar.gz` & `tmp/moneywiz-api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneywiz-api-0.0.2.tar", last modified: Sun Jul  2 20:51:18 2023, max compression
+gzip compressed data, was "moneywiz-api-0.0.3.tar", last modified: Wed Jul 26 20:23:16 2023, max compression
```

## Comparing `moneywiz-api-0.0.2.tar` & `moneywiz-api-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:18.907366 moneywiz-api-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-02 20:51:18.907366 moneywiz-api-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 20:51:18.907366 moneywiz-api-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:18.903366 moneywiz-api-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:18.903366 moneywiz-api-0.0.2/src/moneywiz_api/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/database_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:18.907366 moneywiz-api-0.0.2/src/moneywiz_api/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/managers/account_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/managers/category_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/managers/investment_holding_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/managers/payee_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/managers/record_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/managers/transaction_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:18.907366 moneywiz-api-0.0.2/src/moneywiz_api/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/model/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/model/category.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/model/investment_holding.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/model/payee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/model/record.py
--rw-r--r--   0 runner    (1001) docker     (123)    10962 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/model/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/moneywiz_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:18.907366 moneywiz-api-0.0.2/src/moneywiz_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-02 20:51:18.000000 moneywiz-api-0.0.2/src/moneywiz_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-02 20:51:18.000000 moneywiz-api-0.0.2/src/moneywiz_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:51:18.000000 moneywiz-api-0.0.2/src/moneywiz_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 20:51:18.000000 moneywiz-api-0.0.2/src/moneywiz_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:18.907366 moneywiz-api-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:23:16.127571 moneywiz-api-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-26 20:23:16.127571 moneywiz-api-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 20:23:16.127571 moneywiz-api-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:23:16.123571 moneywiz-api-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:23:16.123571 moneywiz-api-0.0.3/src/moneywiz_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/database_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:23:16.127571 moneywiz-api-0.0.3/src/moneywiz_api/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/managers/account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/managers/category_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/managers/investment_holding_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/managers/payee_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/managers/record_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/managers/transaction_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:23:16.127571 moneywiz-api-0.0.3/src/moneywiz_api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/model/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/model/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/model/investment_holding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/model/payee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/model/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/model/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/moneywiz_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/src/moneywiz_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:23:16.123571 moneywiz-api-0.0.3/src/moneywiz_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-26 20:23:16.000000 moneywiz-api-0.0.3/src/moneywiz_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-26 20:23:16.000000 moneywiz-api-0.0.3/src/moneywiz_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:23:16.000000 moneywiz-api-0.0.3/src/moneywiz_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 20:23:16.000000 moneywiz-api-0.0.3/src/moneywiz_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:23:16.127571 moneywiz-api-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-26 20:23:06.000000 moneywiz-api-0.0.3/tests/test_config.py
```

### Comparing `moneywiz-api-0.0.2/LICENSE` & `moneywiz-api-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.2/PKG-INFO` & `moneywiz-api-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneywiz-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python api to access moneywiz sqlite database
 Author-email: iLeoDo <iLeoDo@gmail.com>
 Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moneywiz-api Version: 0.0.2 Summary: A Python api
+Metadata-Version: 2.1 Name: moneywiz-api Version: 0.0.3 Summary: A Python api
 to access moneywiz sqlite database Author-email: iLeoDo
 gmail.com> Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # MoneyWiz-API ![Static Badge](https://img.shields.io/badge/Python-3-
```

### Comparing `moneywiz-api-0.0.2/README.md` & `moneywiz-api-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.2/pyproject.toml` & `moneywiz-api-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "moneywiz-api"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="iLeoDo", email="iLeoDo@gmail.com" },
 ]
 description = "A Python api to access moneywiz sqlite database"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `moneywiz-api-0.0.2/src/moneywiz_api/database_accessor.py` & `moneywiz-api-0.0.3/src/moneywiz_api/database_accessor.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.2/src/moneywiz_api/managers/account_manager.py` & `moneywiz-api-0.0.3/src/moneywiz_api/managers/account_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.2/src/moneywiz_api/managers/category_manager.py` & `moneywiz-api-0.0.3/src/moneywiz_api/managers/category_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.2/src/moneywiz_api/managers/investment_holding_manager.py` & `moneywiz-api-0.0.3/src/moneywiz_api/managers/investment_holding_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.2/src/moneywiz_api/managers/record_manager.py` & `moneywiz-api-0.0.3/src/moneywiz_api/managers/record_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.2/src/moneywiz_api/managers/transaction_manager.py` & `moneywiz-api-0.0.3/src/moneywiz_api/managers/transaction_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.2/src/moneywiz_api/model/account.py` & `moneywiz-api-0.0.3/src/moneywiz_api/model/account.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.2/src/moneywiz_api/model/category.py` & `moneywiz-api-0.0.3/src/moneywiz_api/model/category.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.2/src/moneywiz_api/model/investment_holding.py` & `moneywiz-api-0.0.3/src/moneywiz_api/model/investment_holding.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.2/src/moneywiz_api/model/record.py` & `moneywiz-api-0.0.3/src/moneywiz_api/model/record.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.2/src/moneywiz_api/model/transaction.py` & `moneywiz-api-0.0.3/src/moneywiz_api/model/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,31 @@
 
 @dataclass
 class Transaction(Record, ABC):
     """
     ENT: 36
     """
 
+    reconciled: bool
+
     amount: float
     description: str
     date: float
     notes: Optional[str]
 
     def __init__(self, row):
         super().__init__(row)
+        self.reconciled = row["ZRECONCILED"] == 1
         self.amount = row["ZAMOUNT1"]
         self.description = row["ZDESC2"]
         self.date = row["ZDATE1"]
         self.notes = row["ZNOTES1"]
 
         # Validate
+        assert self.reconciled is not None
         assert self.amount is not None
         assert self.description is not None
         assert self.date is not None
         # self.notes can be None
 
 
 @dataclass
```

### Comparing `moneywiz-api-0.0.2/src/moneywiz_api/moneywiz_api.py` & `moneywiz-api-0.0.3/src/moneywiz_api/moneywiz_api.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.2/src/moneywiz_api/shell.py` & `moneywiz-api-0.0.3/src/moneywiz_api/shell.py`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.2/src/moneywiz_api.egg-info/PKG-INFO` & `moneywiz-api-0.0.3/src/moneywiz_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneywiz-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python api to access moneywiz sqlite database
 Author-email: iLeoDo <iLeoDo@gmail.com>
 Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moneywiz-api Version: 0.0.2 Summary: A Python api
+Metadata-Version: 2.1 Name: moneywiz-api Version: 0.0.3 Summary: A Python api
 to access moneywiz sqlite database Author-email: iLeoDo
 gmail.com> Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # MoneyWiz-API ![Static Badge](https://img.shields.io/badge/Python-3-
```

### Comparing `moneywiz-api-0.0.2/src/moneywiz_api.egg-info/SOURCES.txt` & `moneywiz-api-0.0.3/src/moneywiz_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

