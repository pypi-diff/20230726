# Comparing `tmp/datamazing-2.0.1.tar.gz` & `tmp/datamazing-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamazing-2.0.1.tar", max compression
+gzip compressed data, was "datamazing-2.0.2.tar", max compression
```

## Comparing `datamazing-2.0.1.tar` & `datamazing-2.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        0 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/__init__.py
--rw-r--r--   0        0        0      277 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/_conform.py
--rw-r--r--   0        0        0      402 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/__init__.py
--rw-r--r--   0        0        0      309 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/datacollection/__init__.py
--rw-r--r--   0        0        0      126 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/testing/__init__.py
--rw-r--r--   0        0        0      766 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/testing/assertions.py
--rw-r--r--   0        0        0     4016 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/testing/data.py
--rw-r--r--   0        0        0        0 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/transformations/__init__.py
--rw-r--r--   0        0        0      649 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/transformations/basic.py
--rw-r--r--   0        0        0     3497 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/transformations/grouping.py
--rw-r--r--   0        0        0     1012 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/transformations/resampling.py
--rw-r--r--   0        0        0      660 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pandas/types.py
--rw-r--r--   0        0        0      184 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pyspark/__init__.py
--rw-r--r--   0        0        0       92 2023-07-21 08:46:39.142649 datamazing-2.0.1/datamazing/pyspark/testing/__init__.py
--rw-r--r--   0        0        0      295 2023-07-21 08:46:39.146649 datamazing-2.0.1/datamazing/pyspark/testing/assertions.py
--rw-r--r--   0        0        0     2064 2023-07-21 08:46:39.146649 datamazing-2.0.1/datamazing/pyspark/testing/data.py
--rw-r--r--   0        0        0        0 2023-07-21 08:46:39.146649 datamazing-2.0.1/datamazing/pyspark/transformations/__init__.py
--rw-r--r--   0        0        0     3058 2023-07-21 08:46:39.146649 datamazing-2.0.1/datamazing/pyspark/transformations/grouping.py
--rw-r--r--   0        0        0      708 2023-07-21 08:46:39.146649 datamazing-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 datamazing-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/__init__.py
+-rw-r--r--   0        0        0      277 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/_conform.py
+-rw-r--r--   0        0        0      463 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pandas/__init__.py
+-rw-r--r--   0        0        0      309 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pandas/datacollection/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pandas/testing/__init__.py
+-rw-r--r--   0        0        0      766 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pandas/testing/assertions.py
+-rw-r--r--   0        0        0     4016 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pandas/testing/data.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pandas/transformations/__init__.py
+-rw-r--r--   0        0        0     1871 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pandas/transformations/basic.py
+-rw-r--r--   0        0        0     3497 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pandas/transformations/grouping.py
+-rw-r--r--   0        0        0     1012 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pandas/transformations/resampling.py
+-rw-r--r--   0        0        0      660 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pandas/types.py
+-rw-r--r--   0        0        0      184 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pyspark/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pyspark/testing/__init__.py
+-rw-r--r--   0        0        0      295 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pyspark/testing/assertions.py
+-rw-r--r--   0        0        0     2064 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pyspark/testing/data.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pyspark/transformations/__init__.py
+-rw-r--r--   0        0        0     3058 2023-07-26 07:53:08.571698 datamazing-2.0.2/datamazing/pyspark/transformations/grouping.py
+-rw-r--r--   0        0        0      708 2023-07-26 07:53:08.571698 datamazing-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 datamazing-2.0.2/PKG-INFO
```

### Comparing `datamazing-2.0.1/datamazing/pandas/testing/assertions.py` & `datamazing-2.0.2/datamazing/pandas/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `datamazing-2.0.1/datamazing/pandas/testing/data.py` & `datamazing-2.0.2/datamazing/pandas/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-2.0.1/datamazing/pandas/transformations/grouping.py` & `datamazing-2.0.2/datamazing/pandas/transformations/grouping.py`

 * *Files identical despite different names*

### Comparing `datamazing-2.0.1/datamazing/pandas/transformations/resampling.py` & `datamazing-2.0.2/datamazing/pandas/transformations/resampling.py`

 * *Files identical despite different names*

### Comparing `datamazing-2.0.1/datamazing/pandas/types.py` & `datamazing-2.0.2/datamazing/pandas/types.py`

 * *Files identical despite different names*

### Comparing `datamazing-2.0.1/datamazing/pyspark/testing/data.py` & `datamazing-2.0.2/datamazing/pyspark/testing/data.py`

 * *Files identical despite different names*

### Comparing `datamazing-2.0.1/datamazing/pyspark/transformations/grouping.py` & `datamazing-2.0.2/datamazing/pyspark/transformations/grouping.py`

 * *Files identical despite different names*

### Comparing `datamazing-2.0.1/pyproject.toml` & `datamazing-2.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datamazing"
-version = "2.0.1"
+version = "2.0.2"
 description = "Package for working with pandas Dataset, but wit specialized functions used for Energinet"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "datamazing" },
 ]
 
 [tool.poetry.dependencies]
```

