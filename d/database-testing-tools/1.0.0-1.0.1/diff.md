# Comparing `tmp/database_testing_tools-1.0.0.tar.gz` & `tmp/database_testing_tools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_testing_tools-1.0.0.tar", max compression
+gzip compressed data, was "database_testing_tools-1.0.1.tar", max compression
```

## Comparing `database_testing_tools-1.0.0.tar` & `database_testing_tools-1.0.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0    40943 2023-04-03 17:02:10.691312 database_testing_tools-1.0.0/database_testing_tools/__init__.py
--rw-r--r--   0        0        0     3982 2023-04-03 17:02:10.691312 database_testing_tools-1.0.0/database_testing_tools/utils.py
--rw-r--r--   0        0        0      965 2023-04-03 17:02:10.691312 database_testing_tools-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 database_testing_tools-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3846 2023-07-26 12:03:41.752716 database_testing_tools-1.0.1/README.md
+-rw-r--r--   0        0        0    40943 2023-07-26 12:03:41.752716 database_testing_tools-1.0.1/database_testing_tools/__init__.py
+-rw-r--r--   0        0        0     3982 2023-07-26 12:03:41.752716 database_testing_tools-1.0.1/database_testing_tools/utils.py
+-rw-r--r--   0        0        0     1067 2023-07-26 12:03:41.756716 database_testing_tools-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4761 1970-01-01 00:00:00.000000 database_testing_tools-1.0.1/PKG-INFO
```

### Comparing `database_testing_tools-1.0.0/database_testing_tools/__init__.py` & `database_testing_tools-1.0.1/database_testing_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `database_testing_tools-1.0.0/database_testing_tools/utils.py` & `database_testing_tools-1.0.1/database_testing_tools/utils.py`

 * *Files identical despite different names*

### Comparing `database_testing_tools-1.0.0/pyproject.toml` & `database_testing_tools-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [tool.poetry]
 name = "database-testing-tools"
-version = "1.0.0"
+version = "1.0.1"
 description = "A package to test our databases"
-authors = ["Stephen Bias <stephen.bias@digital.justice.gov.uk>",
+authors = ["Thomas Hirsch <thomas.hirsch@digital.justice.gov.uk>",
+           "Stephen Bias <stephen.bias@digital.justice.gov.uk>",
            "Tapan Perkins <tapan.perkins@digital.justice.gov.uk>",
            "Matt Laverty <matthew.laverty@justice.gov.uk>",
-           "Thomas Hirsch <thomas.hirsch@digital.justice.gov.uk>",
            "Karik Isichei <karik.isichei@digital.justice.gov.uk>",
            "George Kelly <george.kelly@digital.justice.gov.uk>",
-	   "Anthony Fitzroy <anthony.fitzroy@digital.justice.gov.uk>"]
+	       "Anthony Fitzroy <anthony.fitzroy@digital.justice.gov.uk>"]
+readme = "README.md"
+homepage = "https://github.com/moj-analytical-services/database-testing-tools"
+
 
 [tool.poetry.dependencies]
-python = ">=3.8, <3.11"
+python = ">=3.8, <4"
 altair = "^4.1"
 pydbtools = "^5.2"
 dataengineeringutils3 = "^1.4"
 papermill = "^2.3.3"
 duckdb = "^0.4.0"
 arrow-pd-parser = "^1.3.1"
 mojap-metadata = "^1.10.0"
```

