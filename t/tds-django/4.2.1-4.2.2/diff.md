# Comparing `tmp/tds-django-4.2.1.tar.gz` & `tmp/tds-django-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tds-django-4.2.1.tar", last modified: Fri May 12 15:14:16 2023, max compression
+gzip compressed data, was "tds-django-4.2.2.tar", last modified: Wed Jul 26 09:07:29 2023, max compression
```

## Comparing `tds-django-4.2.1.tar` & `tds-django-4.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 15:14:16.471518 tds-django-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-12 15:14:01.000000 tds-django-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-05-12 15:14:16.471518 tds-django-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-05-12 15:14:01.000000 tds-django-4.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-12 15:14:16.471518 tds-django-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-05-12 15:14:01.000000 tds-django-4.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 15:14:16.467518 tds-django-4.2.1/tds_django/
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6197 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     7431 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/creation.py
--rw-r--r--   0 runner    (1001) docker     (122)    14532 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/features.py
--rw-r--r--   0 runner    (1001) docker     (122)     8818 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     6969 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/introspection.py
--rw-r--r--   0 runner    (1001) docker     (122)    12859 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/operations.py
--rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/patches.py
--rw-r--r--   0 runner    (1001) docker     (122)    21732 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 15:14:16.471518 tds-django-4.2.1/tds_django/sql/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7800 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/sql/clr.sql
--rw-r--r--   0 runner    (1001) docker     (122)     4961 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/sql/init.sql
--rw-r--r--   0 runner    (1001) docker     (122)     6236 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/sql/queries.py
--rw-r--r--   0 runner    (1001) docker     (122)    21250 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/tz.py
--rw-r--r--   0 runner    (1001) docker     (122)      816 2023-05-12 15:14:01.000000 tds-django-4.2.1/tds_django/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 15:14:16.467518 tds-django-4.2.1/tds_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-05-12 15:14:16.000000 tds-django-4.2.1/tds_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-05-12 15:14:16.000000 tds-django-4.2.1/tds_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 15:14:16.000000 tds-django-4.2.1/tds_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-12 15:14:16.000000 tds-django-4.2.1/tds_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:07:29.282133 tds-django-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-07-26 09:07:16.000000 tds-django-4.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-07-26 09:07:29.282133 tds-django-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1768 2023-07-26 09:07:16.000000 tds-django-4.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-26 09:07:29.282133 tds-django-4.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-07-26 09:07:16.000000 tds-django-4.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:07:29.278133 tds-django-4.2.2/tds_django/
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6248 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7431 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/creation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15351 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8818 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6969 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12859 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/operations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/patches.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21732 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:07:29.282133 tds-django-4.2.2/tds_django/sql/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7800 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/sql/clr.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     4961 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/sql/init.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     6236 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/sql/queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21250 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/tz.py
+-rw-r--r--   0 runner    (1001) docker     (122)      816 2023-07-26 09:07:16.000000 tds-django-4.2.2/tds_django/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:07:29.278133 tds-django-4.2.2/tds_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-07-26 09:07:29.000000 tds-django-4.2.2/tds_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-07-26 09:07:29.000000 tds-django-4.2.2/tds_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 09:07:29.000000 tds-django-4.2.2/tds_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-26 09:07:29.000000 tds-django-4.2.2/tds_django.egg-info/top_level.txt
```

### Comparing `tds-django-4.2.1/LICENSE` & `tds-django-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.1/PKG-INFO` & `tds-django-4.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tds-django
-Version: 4.2.1
+Version: 4.2.2
 Summary: Django backend for SQL Server using tds
 Home-page: https://github.com/ecogels/tds-django
 Author: Etienne Cogels
 Author-email: ecogels@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/ecogels/tds-django/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -49,15 +49,15 @@
 - queryset iterator with chunk size
 
 ## Warning If you have used another backend before
 - this one uses `uniqueidentifier` field for UUIDField while others may have used nvarchar.
 
 # Installation
 For django 4.2
-`pip install bitarray python-tds tds_django==4.2.0`
+`pip install bitarray python-tds tds_django~=4.2`
 
 For django 4.1
 `pip install bitarray python-tds tds_django==4.1.0`
 
 For django 4.0
 `pip install bitarray python-tds tds_django==4.0.0`
```

### Comparing `tds-django-4.2.1/README.md` & `tds-django-4.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 - queryset iterator with chunk size
 
 ## Warning If you have used another backend before
 - this one uses `uniqueidentifier` field for UUIDField while others may have used nvarchar.
 
 # Installation
 For django 4.2
-`pip install bitarray python-tds tds_django==4.2.0`
+`pip install bitarray python-tds tds_django~=4.2`
 
 For django 4.1
 `pip install bitarray python-tds tds_django==4.1.0`
 
 For django 4.0
 `pip install bitarray python-tds tds_django==4.0.0`
```

### Comparing `tds-django-4.2.1/setup.py` & `tds-django-4.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tds-django",
-    version="4.2.1",
+    version="4.2.2",
     author="Etienne Cogels",
     author_email="ecogels@users.noreply.github.com",
     description="Django backend for SQL Server using tds",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ecogels/tds-django",
     project_urls={
```

### Comparing `tds-django-4.2.1/tds_django/base.py` & `tds-django-4.2.2/tds_django/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     data_types_suffix = {
         'AutoField': 'IDENTITY (1, 1)',
         'BigAutoField': 'IDENTITY (1, 1)',
         'SmallAutoField': 'IDENTITY (1, 1)',
     }
 
     data_type_check_constraints = {
+        'JSONField': '(ISJSON("%(column)s") = 1)',
         'PositiveIntegerField': '[%(column)s] >= 0',
         'PositiveSmallIntegerField': '[%(column)s] >= 0',
     }
     operators = {
         # Since '=' is used not only for string comparison there is no way
         # to make it case (in)sensitive.
         'exact': '= %s',
```

### Comparing `tds-django-4.2.1/tds_django/compiler.py` & `tds-django-4.2.2/tds_django/compiler.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.1/tds_django/creation.py` & `tds-django-4.2.2/tds_django/creation.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.1/tds_django/features.py` & `tds-django-4.2.2/tds_django/features.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from django.db.backends.base.features import BaseDatabaseFeatures
 from django.utils.functional import cached_property
 
 
 class DatabaseFeatures(BaseDatabaseFeatures):
-
     supports_timezones = False  # has datetimeoffset but would break things if mixed with datetimefield2?
 
     # json
-    supports_json_field = False
+    # supports_json_field = False
     can_introspect_json_field = False  # ISJSON only validates json objects, not literals
+    supports_primitives_in_json_field = False
     has_json_object_function = False
     supports_json_field_contains = False
-    
+
     allow_sliced_subqueries_with_in = False  # TODO CHECK
     allows_group_by_select_index = False
 
     can_create_inline_fk = False
 
     can_return_columns_from_insert = True
     can_return_id_from_insert = True
@@ -50,17 +50,17 @@
 
     ignores_unnecessary_order_by_in_subqueries = False
 
     test_db_allows_multiple_connections = False
 
     django_test_skips = {
         "no need to test this": {
-          'cache.tests.FileBasedCacheTests',
-          'cache.tests.FileBasedCachePathLibTests',
-          'cache.tests.LocMemCacheTests',
+            'cache.tests.FileBasedCacheTests',
+            'cache.tests.FileBasedCachePathLibTests',
+            'cache.tests.LocMemCacheTests',
         },
         "test assumption not correct for SQL Server": {
             # sql server allows double quoted table names
             'schema.tests.SchemaTests.test_add_foreign_key_quoted_db_table',
             # hardcoded SUBSTR
             'custom_lookups.tests.BilateralTransformTests.test_transform_order_by',
             # hardcoded RETURNING
@@ -149,55 +149,65 @@
             'schema.tests.SchemaTests.test_alter_primary_key_db_collation',
             # pass with wrong error without mars, not pass on mars, pytds bug?
             'backends.tests.BackendTestCase.test_cursor_contextmanager',
             # TODO check more
             'expressions.tests.FTimeDeltaTests.test_durationfield_multiply_divide',
             # doable but low priority
             'queries.test_bulk_update.BulkUpdateTests.test_updated_rows_when_passing_duplicates',
-            # TODO json, currenlty marked as not available in features
-            # 'model_fields.test_jsonfield.TestQuerying.test_has_any_keys',
-            # 'model_fields.test_jsonfield.TestQuerying.test_array_key_contains',
-            # 'model_fields.test_jsonfield.TestQuerying.test_contained_by',
-            # 'model_fields.test_jsonfield.TestQuerying.test_contains_contained_by_with_key_transform',
-            # 'model_fields.test_jsonfield.TestQuerying.test_contains_primitives',
-            # 'model_fields.test_jsonfield.TestQuerying.test_deep_lookup_array',
-            # 'model_fields.test_jsonfield.TestQuerying.test_deep_lookup_mixed',
-            # 'model_fields.test_jsonfield.TestQuerying.test_deep_lookup_objs',
-            # 'model_fields.test_jsonfield.TestQuerying.test_deep_lookup_transform',
-            # 'model_fields.test_jsonfield.TestQuerying.test_exact',
-            # 'model_fields.test_jsonfield.TestQuerying.test_exact_complex',
-            # 'model_fields.test_jsonfield.TestQuerying.test_expression_wrapper_key_transform',
-            # 'model_fields.test_jsonfield.TestQuerying.test_join_key_transform_annotation_expression',
-            # 'model_fields.test_jsonfield.TestQuerying.test_isnull_key_or_none',
-            # 'model_fields.test_jsonfield.TestQuerying.test_isnull',
-            # 'model_fields.test_jsonfield.TestQuerying.test_deep_values',
-            # 'model_fields.test_jsonfield.TestQuerying.test_contains',
-            # 'model_fields.test_jsonfield.TestQuerying.test_has_key',
-            # 'model_fields.test_jsonfield.TestQuerying.test_has_key_deep',
-            # 'model_fields.test_jsonfield.TestQuerying.test_has_key_list',
-            # 'model_fields.test_jsonfield.TestQuerying.test_has_key_null_value',
-            # 'model_fields.test_jsonfield.TestQuerying.test_has_keys',
-            # 'model_fields.test_jsonfield.TestQuerying.test_key_iregex',
-            # 'model_fields.test_jsonfield.TestQuerying.test_key_quoted_string',
-            # 'model_fields.test_jsonfield.TestQuerying.test_key_regex',
-            # 'model_fields.test_jsonfield.TestQuerying.test_lookups_with_key_transform',
-            # 'model_fields.test_jsonfield.TestQuerying.test_order_grouping_custom_decoder',
-            # 'model_fields.test_jsonfield.TestQuerying.test_ordering_grouping_by_count',
-            # 'model_fields.test_jsonfield.TestQuerying.test_ordering_grouping_by_key_transform',
-            # 'model_fields.test_jsonfield.JSONFieldTests.test_db_check_constraints',
-            # 'model_fields.test_jsonfield.TestQuerying.test_isnull_key',
-            # 'model_fields.test_jsonfield.TestQuerying.test_key_in',
-            # 'model_fields.test_jsonfield.TestQuerying.test_key_transform_expression',
-            # 'model_fields.test_jsonfield.TestQuerying.test_key_values',
-            # 'model_fields.test_jsonfield.TestQuerying.test_nested_key_transform_expression',
-            # 'model_fields.test_jsonfield.TestQuerying.test_none_key',
-            # 'model_fields.test_jsonfield.TestQuerying.test_none_key_and_exact_lookup',
-            # 'model_fields.test_jsonfield.TestQuerying.test_none_key_exclude',
-            # 'model_fields.test_jsonfield.TestQuerying.test_ordering_by_transform',
-            # 'model_fields.test_jsonfield.TestQuerying.test_shallow_lookup_obj_target',
+            # TODO json
+             'model_fields.test_jsonfield.TestQuerying.test_deep_lookup_array',
+             'model_fields.test_jsonfield.TestQuerying.test_deep_lookup_mixed',
+             'model_fields.test_jsonfield.TestQuerying.test_deep_lookup_objs',
+             'model_fields.test_jsonfield.TestQuerying.test_deep_lookup_transform',
+             'model_fields.test_jsonfield.TestQuerying.test_deep_values',
+             'model_fields.test_jsonfield.TestQuerying.test_expression_wrapper_key_transform',
+             'model_fields.test_jsonfield.TestQuerying.test_has_key_null_value',
+             'model_fields.test_jsonfield.TestQuerying.test_has_key_number',
+             'model_fields.test_jsonfield.TestQuerying.test_isnull_key',
+             'model_fields.test_jsonfield.TestQuerying.test_isnull_key_or_none',
+             'model_fields.test_jsonfield.TestQuerying.test_join_key_transform_annotation_expression',
+             'model_fields.test_jsonfield.TestQuerying.test_key_endswith',
+             'model_fields.test_jsonfield.TestQuerying.test_key_escape',
+             'model_fields.test_jsonfield.TestQuerying.test_key_icontains',
+             'model_fields.test_jsonfield.TestQuerying.test_key_iendswith',
+             'model_fields.test_jsonfield.TestQuerying.test_key_iexact',
+             'model_fields.test_jsonfield.TestQuerying.test_key_in',
+             'model_fields.test_jsonfield.TestQuerying.test_key_iregex',
+             'model_fields.test_jsonfield.TestQuerying.test_key_istartswith',
+             'model_fields.test_jsonfield.TestQuerying.test_key_quoted_string',
+             'model_fields.test_jsonfield.TestQuerying.test_key_regex',
+             'model_fields.test_jsonfield.TestQuerying.test_key_sql_injection_escape',
+             'model_fields.test_jsonfield.TestQuerying.test_key_startswith',
+             'model_fields.test_jsonfield.TestQuerying.test_key_text_transform_char_lookup',
+             'model_fields.test_jsonfield.TestQuerying.test_key_text_transform_from_lookup',
+             'model_fields.test_jsonfield.TestQuerying.test_key_transform_annotation_expression',
+             'model_fields.test_jsonfield.TestQuerying.test_key_transform_expression',
+             'model_fields.test_jsonfield.TestQuerying.test_key_transform_raw_expression',
+             'model_fields.test_jsonfield.TestQuerying.test_key_values',
+             'model_fields.test_jsonfield.TestQuerying.test_key_values_boolean',
+             'model_fields.test_jsonfield.TestQuerying.test_lookup_exclude',
+             'model_fields.test_jsonfield.TestQuerying.test_lookup_exclude_nonexistent_key',
+             'model_fields.test_jsonfield.TestQuerying.test_nested_key_transform_annotation_expression',
+             'model_fields.test_jsonfield.TestQuerying.test_nested_key_transform_expression',
+             'model_fields.test_jsonfield.TestQuerying.test_nested_key_transform_on_subquery',
+             'model_fields.test_jsonfield.TestQuerying.test_nested_key_transform_raw_expression',
+             'model_fields.test_jsonfield.TestQuerying.test_none_key',
+             'model_fields.test_jsonfield.TestQuerying.test_none_key_and_exact_lookup',
+             'model_fields.test_jsonfield.TestQuerying.test_none_key_exclude',
+             'model_fields.test_jsonfield.TestQuerying.test_obj_subquery_lookup',
+             'model_fields.test_jsonfield.TestQuerying.test_order_grouping_custom_decoder',
+             'model_fields.test_jsonfield.TestQuerying.test_ordering_by_transform',
+             'model_fields.test_jsonfield.TestQuerying.test_ordering_grouping_by_count',
+             'model_fields.test_jsonfield.TestQuerying.test_ordering_grouping_by_key_transform',
+             'model_fields.test_jsonfield.TestQuerying.test_shallow_list_lookup',
+             'model_fields.test_jsonfield.TestQuerying.test_shallow_lookup_obj_target',
+             'model_fields.test_jsonfield.TestQuerying.test_shallow_obj_lookup',
+             'model_fields.test_jsonfield.TestQuerying.test_usage_in_subquery',
+
+             'expressions_window.tests.WindowFunctionTests.test_key_transform',
         },
         "SQL Server does not natively support unique (with multiple) nullable fields so a FK to such field will fail": {
             "many_to_one_null.tests.ManyToOneNullTests.test_add_efficiency",
             "many_to_one_null.tests.ManyToOneNullTests.test_assign_clear_related_set",
             "many_to_one_null.tests.ManyToOneNullTests.test_assign_with_queryset",
             "many_to_one_null.tests.ManyToOneNullTests.test_clear_efficiency",
             "many_to_one_null.tests.ManyToOneNullTests.test_created_via_related_set",
```

### Comparing `tds-django-4.2.1/tds_django/functions.py` & `tds-django-4.2.2/tds_django/functions.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.1/tds_django/introspection.py` & `tds-django-4.2.2/tds_django/introspection.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.1/tds_django/operations.py` & `tds-django-4.2.2/tds_django/operations.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.1/tds_django/patches.py` & `tds-django-4.2.2/tds_django/patches.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.1/tds_django/schema.py` & `tds-django-4.2.2/tds_django/schema.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.1/tds_django/sql/clr.sql` & `tds-django-4.2.2/tds_django/sql/clr.sql`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.1/tds_django/sql/init.sql` & `tds-django-4.2.2/tds_django/sql/init.sql`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.1/tds_django/sql/queries.py` & `tds-django-4.2.2/tds_django/sql/queries.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.1/tds_django/tz.py` & `tds-django-4.2.2/tds_django/tz.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.1/tds_django/validation.py` & `tds-django-4.2.2/tds_django/validation.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.2.1/tds_django.egg-info/PKG-INFO` & `tds-django-4.2.2/tds_django.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tds-django
-Version: 4.2.1
+Version: 4.2.2
 Summary: Django backend for SQL Server using tds
 Home-page: https://github.com/ecogels/tds-django
 Author: Etienne Cogels
 Author-email: ecogels@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/ecogels/tds-django/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -49,15 +49,15 @@
 - queryset iterator with chunk size
 
 ## Warning If you have used another backend before
 - this one uses `uniqueidentifier` field for UUIDField while others may have used nvarchar.
 
 # Installation
 For django 4.2
-`pip install bitarray python-tds tds_django==4.2.0`
+`pip install bitarray python-tds tds_django~=4.2`
 
 For django 4.1
 `pip install bitarray python-tds tds_django==4.1.0`
 
 For django 4.0
 `pip install bitarray python-tds tds_django==4.0.0`
```

### Comparing `tds-django-4.2.1/tds_django.egg-info/SOURCES.txt` & `tds-django-4.2.2/tds_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

