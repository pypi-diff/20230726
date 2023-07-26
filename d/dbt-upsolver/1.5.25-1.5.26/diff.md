# Comparing `tmp/dbt-upsolver-1.5.25.tar.gz` & `tmp/dbt-upsolver-1.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-upsolver-1.5.25.tar", last modified: Sat Jun 24 12:41:15 2023, max compression
+gzip compressed data, was "dbt-upsolver-1.5.26.tar", last modified: Wed Jul 26 19:42:10 2023, max compression
```

## Comparing `dbt-upsolver-1.5.25.tar` & `dbt-upsolver-1.5.26.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.968070 dbt-upsolver-1.5.25/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.968070 dbt-upsolver-1.5.25/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt/adapters/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt/adapters/upsolver/options/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/options/connection_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/options/copy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/options/target_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/options/transformation_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/adapters/upsolver/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.968070 dbt-upsolver-1.5.25/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt/include/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/connection.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/materializedview.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/utils/alter_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/utils/create_table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/utils/expextations.sql
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/utils/render_options.sql
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/dbt/include/upsolver/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/dbt_upsolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-06-24 12:41:15.000000 dbt-upsolver-1.5.25/dbt_upsolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-24 12:41:15.000000 dbt-upsolver-1.5.25/dbt_upsolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 12:41:15.000000 dbt-upsolver-1.5.25/dbt_upsolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 12:41:15.000000 dbt-upsolver-1.5.25/dbt_upsolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-24 12:41:15.000000 dbt-upsolver-1.5.25/dbt_upsolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-24 12:41:15.000000 dbt-upsolver-1.5.25/dbt_upsolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 12:41:15.972070 dbt-upsolver-1.5.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-24 12:41:06.000000 dbt-upsolver-1.5.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:42:10.887916 dbt-upsolver-1.5.26/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-07-26 19:42:10.883916 dbt-upsolver-1.5.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:42:10.875916 dbt-upsolver-1.5.26/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:42:10.875916 dbt-upsolver-1.5.26/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:42:10.879916 dbt-upsolver-1.5.26/dbt/adapters/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/adapters/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/adapters/upsolver/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/adapters/upsolver/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/adapters/upsolver/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:42:10.879916 dbt-upsolver-1.5.26/dbt/adapters/upsolver/options/
+-rw-r--r--   0 runner    (1001) docker     (123)    20845 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/adapters/upsolver/options/connection_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39828 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/adapters/upsolver/options/copy_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:42:10.879916 dbt-upsolver-1.5.26/dbt/adapters/upsolver/options/dbt_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/adapters/upsolver/options/dbt_docs/geterate_options_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/adapters/upsolver/options/target_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27668 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/adapters/upsolver/options/transformation_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/adapters/upsolver/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:42:10.875916 dbt-upsolver-1.5.26/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:42:10.879916 dbt-upsolver-1.5.26/dbt/include/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/include/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/include/upsolver/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:42:10.879916 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:42:10.883916 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/connection.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:42:10.883916 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/materializedview.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:42:10.883916 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/utils/alter_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/utils/create_table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/utils/expextations.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/utils/render_options.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/dbt/include/upsolver/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:42:10.883916 dbt-upsolver-1.5.26/dbt_upsolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-07-26 19:42:10.000000 dbt-upsolver-1.5.26/dbt_upsolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-26 19:42:10.000000 dbt-upsolver-1.5.26/dbt_upsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:42:10.000000 dbt-upsolver-1.5.26/dbt_upsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:42:10.000000 dbt-upsolver-1.5.26/dbt_upsolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-26 19:42:10.000000 dbt-upsolver-1.5.26/dbt_upsolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-26 19:42:10.000000 dbt-upsolver-1.5.26/dbt_upsolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:42:10.887916 dbt-upsolver-1.5.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-26 19:41:58.000000 dbt-upsolver-1.5.26/setup.py
```

### Comparing `dbt-upsolver-1.5.25/LICENSE` & `dbt-upsolver-1.5.26/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.25/PKG-INFO` & `dbt-upsolver-1.5.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 1.5.25
+Version: 1.5.26
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -274,7 +274,9 @@
 ## Further reading
 
 [Projects examples](https://github.com/Upsolver/dbt-upsolver/tree/main/examples)
 
 [Upsolver sqlake documentation](https://docs.upsolver.com/sqlake/)
 
 [DBT documentation](https://docs.getdbt.com/docs/introduction)
+
+[Upsolver Comunity Slack](https://join.slack.com/t/upsolvercommunity/shared_invite/zt-1zo1dbyys-hj28WfaZvMh4Z4Id3OkkhA)
```

### Comparing `dbt-upsolver-1.5.25/README.md` & `dbt-upsolver-1.5.26/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -252,7 +252,9 @@
 ## Further reading
 
 [Projects examples](https://github.com/Upsolver/dbt-upsolver/tree/main/examples)
 
 [Upsolver sqlake documentation](https://docs.upsolver.com/sqlake/)
 
 [DBT documentation](https://docs.getdbt.com/docs/introduction)
+
+[Upsolver Comunity Slack](https://join.slack.com/t/upsolvercommunity/shared_invite/zt-1zo1dbyys-hj28WfaZvMh4Z4Id3OkkhA)
```

### Comparing `dbt-upsolver-1.5.25/dbt/adapters/upsolver/connections.py` & `dbt-upsolver-1.5.26/dbt/adapters/upsolver/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,19 @@
     """
 
     token: str
     api_url: str
     database: str
     schema: str
 
+    _ALIASES = {
+        "target_schema": "schema",
+        "target_connection": "database",
+    }
+
     @property
     def type(self):
         return "upsolver"
 
     @property
     def unique_field(self):
         """
```

### Comparing `dbt-upsolver-1.5.25/dbt/adapters/upsolver/impl.py` & `dbt-upsolver-1.5.26/dbt/adapters/upsolver/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,20 +84,44 @@
             for key, value in option_value.items():
                 item = [f'{key}=']
                 if isinstance(value, list):
                     item.append('(')
                     item.append(' ,'.join(value))
                     item.append(')')
                 else:
+                    item.append("'") if key.lower() == 'column' else False
                     item.append(value)
+                    item.append("'") if key.lower() == 'column' else False
                 res.append(''.join(item))
             return f"({' ,'.join(res)})"
         except Exception:
             raise dbt.exceptions.ParsingError(f"Error while parsing value: {value}. Expected type: dictionary")
 
+    def render_option_from_dict_str(self, option_value):
+        try:
+            res = []
+            for key, value in option_value.items():
+                item = [f'{key}=']
+                item.append("'")
+                item.append(value)
+                item.append("'")
+                res.append(''.join(item))
+            return f"({' ,'.join(res)})"
+        except Exception:
+            raise dbt.exceptions.ParsingError(f"Error while parsing value: {value}. Expected type: dictionary")
+
+    def render_option_from_list_dict(self, option_value):
+        try:
+            res = []
+            for value in option_value:
+                res.append(self.render_option_from_dict(value))
+            return f"({' ,'.join(res)})"
+        except Exception:
+            raise dbt.exceptions.ParsingError(f"Error while parsing value: {value}. Expected type: dictionary")
+
     def render_option_from_list(self, option_value):
         try:
             if isinstance(option_value, list) and len(option_value) > 1:
                 return tuple(i for i in option_value)
             else:
                 return f"('{''.join(option_value)}')"
         except Exception:
@@ -110,14 +134,18 @@
         for option, value in config_options.items():
             find_value = options.get(option.lower(), None)
             if find_value:
                 if options[option.lower()]['type'] == 'list':
                     value = self.render_option_from_list(value)
                 elif options[option.lower()]['type'] == 'dict':
                     value = self.render_option_from_dict(value)
+                elif options[option.lower()]['type'] == 'dict_str':
+                    value = self.render_option_from_dict_str(value)
+                elif options[option.lower()]['type'] == 'list_dict':
+                    value = self.render_option_from_list_dict(value)
                 enriched_options[option] = find_value
                 enriched_options[option]['value'] = value
             else:
                 logger.warning(f"Options not found: {option}")
         return enriched_options
 
     @available
```

### Comparing `dbt-upsolver-1.5.25/dbt/adapters/upsolver/relation.py` & `dbt-upsolver-1.5.26/dbt/adapters/upsolver/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/adapters.sql` & `dbt-upsolver-1.5.26/dbt/include/upsolver/macros/adapters.sql`

 * *Files 6% similar despite different names*

```diff
@@ -138,7 +138,22 @@
   {% if (model_constraints or column_constraints) and incremental_strategy  and  incremental_strategy != 'copy' %}
     {{ exceptions.raise_compiler_error("Constraints not available for incremental strategy " ~ incremental_strategy) }}
   {% endif %}
   {% if (model_constraints or column_constraints)  and  target_type  not in ['datalake', 'snowflake']  %}
     {{ exceptions.raise_compiler_error("Constraints not available for target " ~ target_type) }}
   {% endif %}
 {% endmacro %}
+
+{% macro upsolver__generate_schema_name(custom_schema_name, node) -%}
+
+    {%- set default_schema = target.schema -%}
+    {%- if custom_schema_name is none -%}
+
+        {{ default_schema }}
+
+    {%- else -%}
+
+        {{ custom_schema_name | trim }}
+
+    {%- endif -%}
+
+{%- endmacro %}
```

### Comparing `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/catalog.sql` & `dbt-upsolver-1.5.26/dbt/include/upsolver/macros/catalog.sql`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 {% macro upsolver__get_catalog(information_schema, schemas)-%}
-  {{ log("information_schema " ~ information_schema ) }}
-  {{ log("schemas " ~ schemas ) }}
 
   {%- if (schemas | length) == 0 -%}
    {% set msg -%}
     There is no schemas
    {%endset-%}
    {% do exceptions.raise_compiler_error(msg) %}
   {%- endif -%}
@@ -31,11 +29,10 @@
         '{{row['comment']}}' as "column_comment"
       FROM system.information_schema.columns
       WHERE catalog='default_glue_catalog' AND   schema='{{row['schema']}}' AND "table"='{{row['name']}}'
     {%- endset -%}
     {% set columns = run_query(columns_query) %}
     {% do columns_list.append(columns) %}
   {% endfor %}
-
   {{ return(adapter.merge_tables(columns_list)) }}
 
 {% endmacro %}
```

### Comparing `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/connection.sql` & `dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/connection.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql` & `dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql` & `dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql` & `dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/incremental/incremental.sql` & `dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/incremental/incremental.sql`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,14 @@
   {%- set identifier = model['alias'] -%}
   {%- set model_config = model['config'] -%}
   {%- set incremental_strategy = adapter.get(model_config, 'incremental_strategy', False) -%}
   {%- set sync = adapter.get(model_config, 'sync', False) -%}
   {%- set options = adapter.get(model_config, 'options', {}) -%}
   {%- set source = adapter.get(model_config, 'source') -%}
   {%- set target_type = adapter.get(model_config, 'target_type', 'datalake').lower() -%}
-  {%- set target_table_alias = adapter.get(model_config, 'target_table_alias', identifier) -%}
   {%- set delete_condition = adapter.get(model_config, 'delete_condition', False) -%}
   {%- set partition_by = adapter.get(model_config, 'partition_by', []) -%}
   {%- set primary_key = adapter.get(model_config, 'primary_key', []) -%}
   {%- set map_columns_by_name = adapter.get(model_config, 'map_columns_by_name', False) -%}
   {%- set job_identifier = identifier + '_job' %}
   {%- set model_constraints = adapter.render_raw_model_constraints(raw_constraints=model['constraints']) -%}
   {%- set column_constraints = adapter.render_raw_columns_constraints(raw_columns=model['columns']) -%}
@@ -30,28 +29,24 @@
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
   {{ log("model[config]: " ~ model['config'] ) }}
   {{ log("model['columns']): " ~ model['columns'] ) }}
   {{ log("model['constraints']: " ~ model['constraints'] ) }}
 
   {% if target_type  == 'datalake' %}
-    {%- set target_connection = adapter.get(model_config, 'target_connection', database) -%}
-    {%- set target_schema = adapter.get(model_config, 'target_schema', schema) -%}
-    {%- set table_relation = api.Relation.create(identifier=target_table_alias,
-                                                 schema=target_schema,
-                                                 database=target_connection,
+    {%- set table_relation = api.Relation.create(identifier=identifier,
+                                                 schema=schema,
+                                                 database=database,
                                                  type='table') -%}
     {%- set into_relation = table_relation -%}
     {%- call statement('create_table_if_not_exists') -%}
       {{ get_create_table_if_not_exists_sql(table_relation, partition_by, primary_key, options) }}
     {%- endcall -%}
   {%- else -%}
-    {%- set target_schema = adapter.require(model_config, 'target_schema') -%}
-    {% set target_connection = adapter.require(model_config, 'target_connection') %}
-    {%- set into_relation = target_connection + '.' + target_schema + '.' + target_table_alias -%}
+    {%- set into_relation = database + '.' + schema + '.' + identifier -%}
   {%- endif %}
 
   {%- if old_relation -%}
     {%- call statement('main') -%}
       {{ get_alter_job_sql(job_identifier, options, incremental_strategy, source) }}
     {%- endcall %}
     {{ get_add_expectations_if_not_exists_sql(job_identifier, rendered_constraints = column_constraints + model_constraints) }}
```

### Comparing `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/materializedview.sql` & `dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/materializedview.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/utils/alter_job.sql` & `dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/utils/alter_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/utils/create_table.sql` & `dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/utils/create_table.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.25/dbt/include/upsolver/macros/materializations/utils/expextations.sql` & `dbt-upsolver-1.5.26/dbt/include/upsolver/macros/materializations/utils/expextations.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-1.5.25/dbt_upsolver.egg-info/PKG-INFO` & `dbt-upsolver-1.5.26/dbt_upsolver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 1.5.25
+Version: 1.5.26
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -274,7 +274,9 @@
 ## Further reading
 
 [Projects examples](https://github.com/Upsolver/dbt-upsolver/tree/main/examples)
 
 [Upsolver sqlake documentation](https://docs.upsolver.com/sqlake/)
 
 [DBT documentation](https://docs.getdbt.com/docs/introduction)
+
+[Upsolver Comunity Slack](https://join.slack.com/t/upsolvercommunity/shared_invite/zt-1zo1dbyys-hj28WfaZvMh4Z4Id3OkkhA)
```

### Comparing `dbt-upsolver-1.5.25/dbt_upsolver.egg-info/SOURCES.txt` & `dbt-upsolver-1.5.26/dbt_upsolver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 dbt/adapters/upsolver/connections.py
 dbt/adapters/upsolver/impl.py
 dbt/adapters/upsolver/relation.py
 dbt/adapters/upsolver/options/connection_options.py
 dbt/adapters/upsolver/options/copy_options.py
 dbt/adapters/upsolver/options/target_options.py
 dbt/adapters/upsolver/options/transformation_options.py
+dbt/adapters/upsolver/options/dbt_docs/geterate_options_docs.py
 dbt/include/upsolver/__init__.py
 dbt/include/upsolver/dbt_project.yml
 dbt/include/upsolver/profile_template.yml
 dbt/include/upsolver/macros/adapters.sql
 dbt/include/upsolver/macros/catalog.sql
 dbt/include/upsolver/macros/materializations/connection.sql
 dbt/include/upsolver/macros/materializations/materializedview.sql
```

### Comparing `dbt-upsolver-1.5.25/setup.py` & `dbt-upsolver-1.5.26/setup.py`

 * *Files identical despite different names*

