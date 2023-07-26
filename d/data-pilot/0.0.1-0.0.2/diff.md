# Comparing `tmp/data_pilot-0.0.1.tar.gz` & `tmp/data_pilot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_pilot-0.0.1.tar", max compression
+gzip compressed data, was "data_pilot-0.0.2.tar", max compression
```

## Comparing `data_pilot-0.0.1.tar` & `data_pilot-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rwxr-xr-x   0        0        0      672 2023-07-14 12:02:45.342805 data_pilot-0.0.1/README.md
--rwxr-xr-x   0        0        0        0 2023-07-13 20:34:26.195269 data_pilot-0.0.1/data_pilot/__init__.py
--rwxr-xr-x   0        0        0        4 2023-07-14 11:49:39.527988 data_pilot-0.0.1/data_pilot/data_preprocessing.py
--rwxr-xr-x   0        0        0      580 2023-07-14 12:12:08.558569 data_pilot-0.0.1/data_pilot/supabase_api.py
--rwxr-xr-x   0        0        0      513 2023-07-14 12:16:00.435871 data_pilot-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 data_pilot-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     2746 2023-07-26 06:52:43.075596 data_pilot-0.0.2/DataPilot/AI_API.py
+-rwxr-xr-x   0        0        0      519 2023-07-26 06:48:26.306364 data_pilot-0.0.2/DataPilot/DataAnalysis.py
+-rwxr-xr-x   0        0        0      410 2023-07-26 06:51:01.575015 data_pilot-0.0.2/DataPilot/DataPreprocessing.py
+-rwxr-xr-x   0        0        0     1148 2023-07-26 06:53:13.969925 data_pilot-0.0.2/DataPilot/DataSource.py
+-rwxr-xr-x   0        0        0     1172 2023-07-14 21:04:55.728856 data_pilot-0.0.2/DataPilot/NN.py
+-rwxr-xr-x   0        0        0       98 2023-07-26 06:54:42.771236 data_pilot-0.0.2/DataPilot/__init__.py
+-rwxr-xr-x   0        0        0     7187 2023-07-26 06:50:59.322604 data_pilot-0.0.2/README.md
+-rwxr-xr-x   0        0        0      512 2023-07-26 06:54:44.447774 data_pilot-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7950 1970-01-01 00:00:00.000000 data_pilot-0.0.2/PKG-INFO
```

### Comparing `data_pilot-0.0.1/pyproject.toml` & `data_pilot-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "data-pilot"
-version = "0.0.1"
+version = "0.0.2"
 description = "Use LLMs to automate data science tasks"
 authors = ["Amar <amar439412@gmail.com>"]
 readme = "README.md"
-packages = [{include = "data_pilot"}]
+packages = [{include = "DataPilot"}]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 replicate = "^0.8.4"
 openai = "^0.27.8"
 pyspark = "^3.4.1"
```

