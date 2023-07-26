# Comparing `tmp/ohdsi-database-connector-0.2.2.tar.gz` & `tmp/ohdsi-database-connector-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohdsi-database-connector-0.2.2.tar", last modified: Fri Jul 14 10:13:53 2023, max compression
+gzip compressed data, was "ohdsi-database-connector-0.2.3.tar", last modified: Wed Jul 26 08:39:37 2023, max compression
```

## Comparing `ohdsi-database-connector-0.2.2.tar` & `ohdsi-database-connector-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.834680 ohdsi-database-connector-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-14 10:13:53.834680 ohdsi-database-connector-0.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.834680 ohdsi-database-connector-0.2.2/ohdsi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.834680 ohdsi-database-connector-0.2.2/ohdsi/database_connector/
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-14 10:13:44.000000 ohdsi-database-connector-0.2.2/ohdsi/database_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.834680 ohdsi-database-connector-0.2.2/ohdsi/database_connector/java/
--rw-r--r--   0 runner    (1001) docker     (123)  1004719 2023-07-14 10:13:44.000000 ohdsi-database-connector-0.2.2/ohdsi/database_connector/java/postgresql-42.2.18.jar
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.834680 ohdsi-database-connector-0.2.2/ohdsi_database_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-14 10:13:53.000000 ohdsi-database-connector-0.2.2/ohdsi_database_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 10:13:53.000000 ohdsi-database-connector-0.2.2/ohdsi_database_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:13:53.000000 ohdsi-database-connector-0.2.2/ohdsi_database_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 10:13:53.000000 ohdsi-database-connector-0.2.2/ohdsi_database_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 10:13:53.000000 ohdsi-database-connector-0.2.2/ohdsi_database_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:13:53.834680 ohdsi-database-connector-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-14 10:13:44.000000 ohdsi-database-connector-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:37.161831 ohdsi-database-connector-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-26 08:39:37.161831 ohdsi-database-connector-0.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:37.157831 ohdsi-database-connector-0.2.3/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:37.157831 ohdsi-database-connector-0.2.3/ohdsi/database_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-26 08:39:24.000000 ohdsi-database-connector-0.2.3/ohdsi/database_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:37.157831 ohdsi-database-connector-0.2.3/ohdsi/database_connector/java/
+-rw-r--r--   0 runner    (1001) docker     (123)  1004719 2023-07-26 08:39:24.000000 ohdsi-database-connector-0.2.3/ohdsi/database_connector/java/postgresql-42.2.18.jar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:37.157831 ohdsi-database-connector-0.2.3/ohdsi_database_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-26 08:39:37.000000 ohdsi-database-connector-0.2.3/ohdsi_database_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-26 08:39:37.000000 ohdsi-database-connector-0.2.3/ohdsi_database_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 08:39:37.000000 ohdsi-database-connector-0.2.3/ohdsi_database_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-26 08:39:37.000000 ohdsi-database-connector-0.2.3/ohdsi_database_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 08:39:37.000000 ohdsi-database-connector-0.2.3/ohdsi_database_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 08:39:37.161831 ohdsi-database-connector-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-26 08:39:24.000000 ohdsi-database-connector-0.2.3/setup.py
```

### Comparing `ohdsi-database-connector-0.2.2/PKG-INFO` & `ohdsi-database-connector-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohdsi-database-connector
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python wrapper for the OHDSI R packages
 Home-page: https://github.com/vantage6/python-ohdsi
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # python-ohdsi
@@ -12,14 +12,21 @@
 supporting OMOP data sources in [vantage6](https://vantage6.ai).
 
 Make sure you have a working R environment with the OHDSI packages installed.
 
 # Building documentation
 ```bash
 cd docs
+export
+make html
+```
+
+```powershell
+cd docs
+Set-Item -Path Env:IGNORE_R_IMPORTS -Value True
 make html
 ```
 
 You can set the `IGNORE_R_IMPORTS` environment variable to ignore the R imports
 in the documentation. This is useful when you don't have the R packages
 installed but want to build the documentation anyway.
```

### Comparing `ohdsi-database-connector-0.2.2/ohdsi/database_connector/__init__.py` & `ohdsi-database-connector-0.2.3/ohdsi/database_connector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     ) -> ListVector:
         """
         Create Connection Details.
 
         Creates a list containing all details needed to connect to a database.
         There are three ways to call this function:
 
-        - ``create_connection_details(dbms, user, password, server, port,
-                                      extraSettings, oracleDriver,
+        - ``create_connection_details(dbms, user, password, server, port, \
+                                      extraSettings, oracleDriver, \
                                       pathToDriver)``
         - ``create_connection_details(dbms, connectionString, pathToDriver)``
-        - ``create_connection_details(dbms, connectionString, user, password,
+        - ``create_connection_details(dbms, connectionString, user, password, \
                                       pathToDriver)``
 
         Parameters
         ----------
         dbms : str
             The DBMS type.
         user : str | None, optional
```

### Comparing `ohdsi-database-connector-0.2.2/ohdsi/database_connector/java/postgresql-42.2.18.jar` & `ohdsi-database-connector-0.2.3/ohdsi/database_connector/java/postgresql-42.2.18.jar`

 * *Files identical despite different names*

### Comparing `ohdsi-database-connector-0.2.2/ohdsi_database_connector.egg-info/PKG-INFO` & `ohdsi-database-connector-0.2.3/ohdsi_database_connector.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohdsi-database-connector
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python wrapper for the OHDSI R packages
 Home-page: https://github.com/vantage6/python-ohdsi
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # python-ohdsi
@@ -12,14 +12,21 @@
 supporting OMOP data sources in [vantage6](https://vantage6.ai).
 
 Make sure you have a working R environment with the OHDSI packages installed.
 
 # Building documentation
 ```bash
 cd docs
+export
+make html
+```
+
+```powershell
+cd docs
+Set-Item -Path Env:IGNORE_R_IMPORTS -Value True
 make html
 ```
 
 You can set the `IGNORE_R_IMPORTS` environment variable to ignore the R imports
 in the documentation. This is useful when you don't have the R packages
 installed but want to build the documentation anyway.
```

### Comparing `ohdsi-database-connector-0.2.2/setup.py` & `ohdsi-database-connector-0.2.3/setup.py`

 * *Files identical despite different names*

