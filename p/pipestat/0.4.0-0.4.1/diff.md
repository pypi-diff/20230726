# Comparing `tmp/pipestat-0.4.0.tar.gz` & `tmp/pipestat-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipestat-0.4.0.tar", last modified: Thu Jun 29 19:25:12 2023, max compression
+gzip compressed data, was "pipestat-0.4.1.tar", last modified: Wed Jul 26 13:49:14 2023, max compression
```

## Comparing `pipestat-0.4.0.tar` & `pipestat-0.4.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:25:12.569878 pipestat-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-29 19:25:01.000000 pipestat-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-29 19:25:01.000000 pipestat-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-29 19:25:12.569878 pipestat-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-29 19:25:01.000000 pipestat-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:25:12.569878 pipestat-0.4.0/pipestat/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:25:12.569878 pipestat-0.4.0/pipestat/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/backends/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    26413 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/backends/dbbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/backends/filebackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/parsed_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    21733 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/pipestat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:25:12.569878 pipestat-0.4.0/pipestat/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/schemas/pipestat_config_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/schemas/status_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-29 19:25:01.000000 pipestat-0.4.0/pipestat/schemas/status_table_schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:25:12.569878 pipestat-0.4.0/pipestat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-29 19:25:12.000000 pipestat-0.4.0/pipestat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-29 19:25:12.000000 pipestat-0.4.0/pipestat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:25:12.000000 pipestat-0.4.0/pipestat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-29 19:25:12.000000 pipestat-0.4.0/pipestat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-29 19:25:12.000000 pipestat-0.4.0/pipestat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 19:25:12.000000 pipestat-0.4.0/pipestat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-29 19:25:01.000000 pipestat-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:25:12.569878 pipestat-0.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-29 19:25:01.000000 pipestat-0.4.0/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 19:25:01.000000 pipestat-0.4.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-29 19:25:01.000000 pipestat-0.4.0/requirements/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 19:25:01.000000 pipestat-0.4.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:25:12.569878 pipestat-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-29 19:25:01.000000 pipestat-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:14.613767 pipestat-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-26 13:49:05.000000 pipestat-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-26 13:49:05.000000 pipestat-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-26 13:49:14.613767 pipestat-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-26 13:49:05.000000 pipestat-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:14.613767 pipestat-0.4.1/pipestat/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:14.613767 pipestat-0.4.1/pipestat/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/backends/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26413 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/backends/dbbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/backends/filebackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/parsed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21733 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/pipestat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:14.613767 pipestat-0.4.1/pipestat/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/schemas/pipestat_config_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/schemas/status_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-26 13:49:05.000000 pipestat-0.4.1/pipestat/schemas/status_table_schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:14.613767 pipestat-0.4.1/pipestat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-26 13:49:14.000000 pipestat-0.4.1/pipestat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-26 13:49:14.000000 pipestat-0.4.1/pipestat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:49:14.000000 pipestat-0.4.1/pipestat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-26 13:49:14.000000 pipestat-0.4.1/pipestat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-26 13:49:14.000000 pipestat-0.4.1/pipestat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 13:49:14.000000 pipestat-0.4.1/pipestat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 13:49:05.000000 pipestat-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:49:14.613767 pipestat-0.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-26 13:49:05.000000 pipestat-0.4.1/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 13:49:05.000000 pipestat-0.4.1/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-26 13:49:05.000000 pipestat-0.4.1/requirements/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 13:49:05.000000 pipestat-0.4.1/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:49:14.613767 pipestat-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-26 13:49:05.000000 pipestat-0.4.1/setup.py
```

### Comparing `pipestat-0.4.0/LICENSE` & `pipestat-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.0/PKG-INFO` & `pipestat-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipestat
-Version: 0.4.0
+Version: 0.4.1
 Summary: A pipeline results reporter
 Home-page: https://github.com/pepkit/pipestat
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pipestat-0.4.0/README.md` & `pipestat-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.0/pipestat/argparser.py` & `pipestat-0.4.1/pipestat/argparser.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.0/pipestat/backends/abstract.py` & `pipestat-0.4.1/pipestat/backends/abstract.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.0/pipestat/backends/dbbackend.py` & `pipestat-0.4.1/pipestat/backends/dbbackend.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.0/pipestat/backends/filebackend.py` & `pipestat-0.4.1/pipestat/backends/filebackend.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.0/pipestat/cli.py` & `pipestat-0.4.1/pipestat/cli.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.0/pipestat/const.py` & `pipestat-0.4.1/pipestat/const.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.0/pipestat/exceptions.py` & `pipestat-0.4.1/pipestat/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.0/pipestat/helpers.py` & `pipestat-0.4.1/pipestat/helpers.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.0/pipestat/parsed_schema.py` & `pipestat-0.4.1/pipestat/parsed_schema.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.0/pipestat/pipestat.py` & `pipestat-0.4.1/pipestat/pipestat.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.0/pipestat/schemas/pipestat_config_schema.yaml` & `pipestat-0.4.1/pipestat/schemas/pipestat_config_schema.yaml`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.0/pipestat.egg-info/PKG-INFO` & `pipestat-0.4.1/pipestat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipestat
-Version: 0.4.0
+Version: 0.4.1
 Summary: A pipeline results reporter
 Home-page: https://github.com/pepkit/pipestat
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pipestat-0.4.0/pipestat.egg-info/SOURCES.txt` & `pipestat-0.4.1/pipestat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipestat-0.4.0/setup.py` & `pipestat-0.4.1/setup.py`

 * *Files identical despite different names*

