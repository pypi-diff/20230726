# Comparing `tmp/schemawizard_package-2.5.1.tar.gz` & `tmp/schemawizard_package-2.5.2.tar.gz`

## Comparing `schemawizard_package-2.5.1.tar` & `schemawizard_package-2.5.2.tar`

### file list

```diff
@@ -1,39 +1,42 @@
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/dateformat_readme.md
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/methods.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/.schemawiz_config1
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/.schemawiz_config2
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/.schemawiz_config3
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/a.csv
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/floats.csv
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/postgres_data.tsv
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/sample7.csv
--rw-r--r--   0        0        0    35077 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/schemawizard.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/sqlite.station_years.ddl
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/sqlite.tablea.ddl
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/sqlite.tablec.ddl
--rw-r--r--   0        0        0   106414 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/station_months.tsv
--rw-r--r--   0        0        0   503697 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/station_years.tsv
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/testcase1.csv
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/src/schemawizard_package/z.canweather.station_years.ddl
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/chk_ddl.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/create_and_load.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/create_and_load_mysql.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/create_and_load_postgres.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/csv_load.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/floats.csv
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/generate_bigqueryddl.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/generate_ddl_knowing_delimiter.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/generate_externalbigqueryddl.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/generate_mysqlddl.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/generate_postgresddl.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/load_mysql.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/load_postgres.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/sample.csv
--rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/tesla.csv
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/tests/tester.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/LICENSE
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/README.md
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/pyproject.toml
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 schemawizard_package-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/dateformat_readme.md
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/methods.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/.schemawiz_config1
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/.schemawiz_config2
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/.schemawiz_config3
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/a.csv
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/floats.csv
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/postgres_data.tsv
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/sample7.csv
+-rw-r--r--   0        0        0    35324 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/schemawizard.py
+-rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/servers.csv
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/sqlite.station_years.ddl
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/sqlite.tablea.ddl
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/sqlite.tablec.ddl
+-rw-r--r--   0        0        0   106414 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/station_months.tsv
+-rw-r--r--   0        0        0   503697 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/station_years.tsv
+-rw-r--r--   0        0        0  1455077 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/test.csv
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/testcase1.csv
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/testconnects.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/src/schemawizard_package/z.canweather.station_years.ddl
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/chk_ddl.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/create_and_load.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/create_and_load_mysql.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/create_and_load_postgres.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/csv_load.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/floats.csv
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/generate_bigqueryddl.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/generate_ddl_knowing_delimiter.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/generate_externalbigqueryddl.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/generate_mysqlddl.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/generate_postgresddl.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/load_mysql.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/load_postgres.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/sample.csv
+-rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/tesla.csv
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/tests/tester.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/LICENSE
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/README.md
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 schemawizard_package-2.5.2/PKG-INFO
```

### Comparing `schemawizard_package-2.5.1/dateformat_readme.md` & `schemawizard_package-2.5.2/dateformat_readme.md`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.5.1/methods.md` & `schemawizard_package-2.5.2/methods.md`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.5.1/src/schemawizard_package/schemawizard.py` & `schemawizard_package-2.5.2/src/schemawizard_package/schemawizard.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from sqlitedave_package.sqlitedave import sqlite_db
 from postgresdave_package.postgresdave import postgres_db 
 from mysqldave_package.mysqldave import mysql_db 
 from garbledave_package.garbledave import garbledave 
 
 def main():
 	obj = schemawiz()
-	obj.loadcsvfile('testcase1.csv')
-	print(obj.guess_sqlite_ddl('testcase1'))
-	
-	#tbl = obj.createload_postgres_from_csv('projects.tsv','gcp_projects')
+	#obj.loadcsvfile('test.csv')
+	#tbl = obj.createload_mysql_from_csv('test.csv','test3')
+	#obj.justload_sqlite_from_csv('servers.csv','servers',True)
+	#print(obj.guess_sqlite_ddl('servers'))
 
 """	
 	csvfilename = 'a.csv'
 	ddl = obj.guess_postgres_ddl(csvfilename.replace('.','_'))
 	print(ddl)
 	print('/* Tablename used : ' + obj.lastcall_tablename + ' */ \n')
 	print('/* Postgres DDL - END   ----- ----- ----- ----- */ \n')
@@ -739,14 +739,19 @@
 							found_datatypes[self.column_names[j]] == 'text'
 						elif found_datatypes[self.column_names[j]] == 'numeric' or thisdatatype == 'numeric':
 							found_datatypes[self.column_names[j]] == 'numeric'
 						elif found_datatypes[self.column_names[j]] == 'date' or thisdatatype == 'date':
 							found_datatypes[self.column_names[j]] == 'text'
 
 		for k in range(0,len(self.column_names)):
+			if self.column_names[k] not in found_datavalues:
+				found_datavalues[self.column_names[k]] = ''
+				found_datefomat[self.column_names[k]] = ''
+				found_datatypes[self.column_names[k]] = 'text'
+			
 			self.column_sample.append(found_datavalues[self.column_names[k]].replace('"',''))
 			self.column_dateformats.append(found_datefomat[self.column_names[k]])
 
 			self.column_datatypes.append(found_datatypes[self.column_names[k]])
 			self.mysql_datatypes.append(self.translate_dt(database_type.MySQL,found_datatypes[self.column_names[k]]))
 
 			self.BigQuery_datatypes.append(self.translate_dt(database_type.BigQuery,found_datatypes[self.column_names[k]]))
```

### Comparing `schemawizard_package-2.5.1/src/schemawizard_package/sqlite.tablea.ddl` & `schemawizard_package-2.5.2/src/schemawizard_package/sqlite.tablea.ddl`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.5.1/src/schemawizard_package/station_months.tsv` & `schemawizard_package-2.5.2/src/schemawizard_package/station_months.tsv`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.5.1/src/schemawizard_package/station_years.tsv` & `schemawizard_package-2.5.2/src/schemawizard_package/station_years.tsv`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.5.1/tests/create_and_load.py` & `schemawizard_package-2.5.2/tests/create_and_load.py`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.5.1/tests/tesla.csv` & `schemawizard_package-2.5.2/tests/tesla.csv`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.5.1/tests/tester.py` & `schemawizard_package-2.5.2/tests/tester.py`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.5.1/LICENSE` & `schemawizard_package-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `schemawizard_package-2.5.1/pyproject.toml` & `schemawizard_package-2.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling","postgresdave_package","mysqldave_package","sqlitedave_package","garbledave_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "schemawizard_package"
-version = "2.5.1"
+version = "2.5.2"
 dependencies = [
   'postgresdave_package >= 1.8.0',
   'mysqldave_package >= 1.5.0',
   'sqlitedave_package >= 1.3.0',
   'garbledave_package >= 1.0.0 '
 ]
 authors = [
```

### Comparing `schemawizard_package-2.5.1/PKG-INFO` & `schemawizard_package-2.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemawizard_package
-Version: 2.5.1
+Version: 2.5.2
 Summary: Reads a csv and generates a table design for Postgres, MySQL, sqlite or BigQuery
 Project-URL: Homepage, https://github.com/daveskura/schemawizard
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

