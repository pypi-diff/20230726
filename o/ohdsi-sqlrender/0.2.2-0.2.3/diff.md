# Comparing `tmp/ohdsi-sqlrender-0.2.2.tar.gz` & `tmp/ohdsi-sqlrender-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohdsi-sqlrender-0.2.2.tar", last modified: Fri Jul 14 10:13:54 2023, max compression
+gzip compressed data, was "ohdsi-sqlrender-0.2.3.tar", last modified: Wed Jul 26 08:39:37 2023, max compression
```

## Comparing `ohdsi-sqlrender-0.2.2.tar` & `ohdsi-sqlrender-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:54.322689 ohdsi-sqlrender-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-14 10:13:54.322689 ohdsi-sqlrender-0.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:54.318689 ohdsi-sqlrender-0.2.2/ohdsi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:54.318689 ohdsi-sqlrender-0.2.2/ohdsi/sqlrender/
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-07-14 10:13:44.000000 ohdsi-sqlrender-0.2.2/ohdsi/sqlrender/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:54.322689 ohdsi-sqlrender-0.2.2/ohdsi_sqlrender.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-14 10:13:54.000000 ohdsi-sqlrender-0.2.2/ohdsi_sqlrender.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-14 10:13:54.000000 ohdsi-sqlrender-0.2.2/ohdsi_sqlrender.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:13:54.000000 ohdsi-sqlrender-0.2.2/ohdsi_sqlrender.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 10:13:54.000000 ohdsi-sqlrender-0.2.2/ohdsi_sqlrender.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 10:13:54.000000 ohdsi-sqlrender-0.2.2/ohdsi_sqlrender.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:13:54.322689 ohdsi-sqlrender-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-14 10:13:44.000000 ohdsi-sqlrender-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:37.637842 ohdsi-sqlrender-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-26 08:39:37.637842 ohdsi-sqlrender-0.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:37.637842 ohdsi-sqlrender-0.2.3/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:37.637842 ohdsi-sqlrender-0.2.3/ohdsi/sqlrender/
+-rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-07-26 08:39:24.000000 ohdsi-sqlrender-0.2.3/ohdsi/sqlrender/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:37.637842 ohdsi-sqlrender-0.2.3/ohdsi_sqlrender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-26 08:39:37.000000 ohdsi-sqlrender-0.2.3/ohdsi_sqlrender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-26 08:39:37.000000 ohdsi-sqlrender-0.2.3/ohdsi_sqlrender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 08:39:37.000000 ohdsi-sqlrender-0.2.3/ohdsi_sqlrender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-26 08:39:37.000000 ohdsi-sqlrender-0.2.3/ohdsi_sqlrender.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 08:39:37.000000 ohdsi-sqlrender-0.2.3/ohdsi_sqlrender.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 08:39:37.637842 ohdsi-sqlrender-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-26 08:39:24.000000 ohdsi-sqlrender-0.2.3/setup.py
```

### Comparing `ohdsi-sqlrender-0.2.2/PKG-INFO` & `ohdsi-sqlrender-0.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohdsi-sqlrender
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

### Comparing `ohdsi-sqlrender-0.2.2/ohdsi/sqlrender/__init__.py` & `ohdsi-sqlrender-0.2.3/ohdsi/sqlrender/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         >>> sql = "SELECT * FROM table WHERE id = @id"
         >>> RenderSql.render("SELECT * FROM @a;", a = "myTable")
         """
         return sql_render_r.render(sql, warn_on_missing_parameters, **kwargs)
 
     @staticmethod
     def translate(sql: str, target_dialect: str,
-                  temp_emulation_schema: str | None) -> StrVector:
+                  temp_emulation_schema: str | None = None) -> StrVector:
         """
         ``translate`` translates SQL from one dialect to another.
 
         Parameters
         ----------
         sql : str
             The SQL to be translated
@@ -127,15 +127,15 @@
                 base_r.getOption("sqlRenderTempEmulationSchema")
 
         return sql_render_r.translate(sql, target_dialect,
                                       temp_emulation_schema)
 
     @staticmethod
     def translate_single_statement(
-        sql: str, target_dialect: str, temp_emulation_schema: str | None
+        sql: str, target_dialect: str, temp_emulation_schema: str | None = None
     ) -> StrVector:
         """
         Translates a single SQL statement from one dialect to another.
 
         This function takes SQL in one dialect and translates it into another.
         It uses simple pattern replacement, so its functionality is limited.
         This removes any trailing semicolon as required by Oracle when
@@ -290,15 +290,15 @@
         """
         sql_render_r.renderSqlFile(source_file, target_file,
                                    warnOnMissingParameters, **kwargs)
 
     @staticmethod
     def translate_sql_file(source_file: str | Path, target_file: str | Path,
                            target_dialect: str,
-                           temp_emulation_schema: str | None) -> None:
+                           temp_emulation_schema: str | None = None) -> None:
         """
         Translate a SQL file.
 
         This function takes SQL and translates it to a different dialect.
 
         Parameters
         ----------
@@ -330,15 +330,16 @@
                 base_r.getOption("sqlRenderTempEmulationSchema")
 
         sql_render_r.translateSqlFile(source_file, target_file, target_dialect,
                                       temp_emulation_schema)
 
     @staticmethod
     def load_render_translate_sql(sql_file: str | Path, package_name: str,
-                                  dbms: str, temp_emulation_schema: str | None,
+                                  dbms: str,
+                                  temp_emulation_schema: str | None = None,
                                   warn_on_missing_parameters: bool = True) \
             -> StrVector:
         """
         Load, render, and translate a SQL file in a package.
 
         ``loadRenderTranslateSql`` Loads a SQL file contained in a package,
         renders it and translates it to the specified dialect'
```

### Comparing `ohdsi-sqlrender-0.2.2/ohdsi_sqlrender.egg-info/PKG-INFO` & `ohdsi-sqlrender-0.2.3/ohdsi_sqlrender.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohdsi-sqlrender
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

### Comparing `ohdsi-sqlrender-0.2.2/setup.py` & `ohdsi-sqlrender-0.2.3/setup.py`

 * *Files identical despite different names*

