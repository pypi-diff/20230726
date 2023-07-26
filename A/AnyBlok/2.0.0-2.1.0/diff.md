# Comparing `tmp/AnyBlok-2.0.0.tar.gz` & `tmp/AnyBlok-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AnyBlok-2.0.0.tar", last modified: Sat Mar 11 16:29:36 2023, max compression
+gzip compressed data, was "AnyBlok-2.1.0.tar", last modified: Wed Jul 26 14:47:54 2023, max compression
```

## Comparing `AnyBlok-2.0.0.tar` & `AnyBlok-2.1.0.tar`

### file list

```diff
@@ -1,231 +1,227 @@
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.113974 AnyBlok-2.0.0/
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.073974 AnyBlok-2.0.0/AnyBlok.egg-info/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    45803 2023-03-11 16:29:36.000000 AnyBlok-2.0.0/AnyBlok.egg-info/PKG-INFO
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6528 2023-03-11 16:29:36.000000 AnyBlok-2.0.0/AnyBlok.egg-info/SOURCES.txt
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)        1 2023-03-11 16:29:36.000000 AnyBlok-2.0.0/AnyBlok.egg-info/dependency_links.txt
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2028 2023-03-11 16:29:36.000000 AnyBlok-2.0.0/AnyBlok.egg-info/entry_points.txt
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      322 2023-03-11 16:29:36.000000 AnyBlok-2.0.0/AnyBlok.egg-info/requires.txt
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       21 2023-03-11 16:29:36.000000 AnyBlok-2.0.0/AnyBlok.egg-info/top_level.txt
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    16348 2019-09-12 16:00:00.000000 AnyBlok-2.0.0/LICENSE
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      213 2020-10-16 08:44:47.000000 AnyBlok-2.0.0/MANIFEST.in
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    45803 2023-03-11 16:29:36.113974 AnyBlok-2.0.0/PKG-INFO
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4332 2023-02-20 08:54:41.000000 AnyBlok-2.0.0/README.rst
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.081974 AnyBlok-2.0.0/anyblok/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4105 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    12613 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/_graphviz.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.081974 AnyBlok-2.0.0/anyblok/authorization/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1105 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/authorization/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2804 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/authorization/binding.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2220 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/authorization/query.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.081974 AnyBlok-2.0.0/anyblok/authorization/rule/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      308 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/authorization/rule/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2609 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/authorization/rule/attraccess.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3654 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/authorization/rule/base.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2466 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/authorization/rule/modelaccess.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    10057 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/blok.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.081974 AnyBlok-2.0.0/anyblok/bloks/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      316 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/bloks/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     5347 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok-logo_alpha_256.png
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.085974 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3543 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/CODE.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4293 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      716 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/authorization.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.085974 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/core/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      738 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/core/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3826 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/core/base.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      890 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/core/instrumentedlist.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6325 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/core/query.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    25780 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/core/sqlbase.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      964 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/core/sqlviewbase.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.085974 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/documentation/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2417 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/documentation/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1669 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/documentation/blok.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.085974 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/documentation/model/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4559 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/documentation/model/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2924 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/documentation/model/attribute.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     5389 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/documentation/model/field.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      779 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/exceptions.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.089974 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1051 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    10183 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/blok.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3701 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/cache.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3936 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/column.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3144 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/field.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     5934 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/model.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3781 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/parameter.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3560 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/relationship.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6540 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/sequence.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.089974 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      316 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1302 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_core_base.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4752 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_core_query.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      438 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_core_session.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     7700 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_core_sql_base.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1468 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_documentation.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1054 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_system_blok.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      439 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_system_column.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      438 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_system_field.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      412 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_system_model.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4429 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_system_params.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      445 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_system_relationship.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3315 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_system_sequence.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1174 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_testing.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.089974 AnyBlok-2.0.0/anyblok/bloks/anyblok_test/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      624 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/anyblok_test/__init__.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.089974 AnyBlok-2.0.0/anyblok/bloks/model_authz/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      492 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/bloks/model_authz/CODE.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      323 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/bloks/model_authz/README.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      735 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/bloks/model_authz/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      639 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/bloks/model_authz/models.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.089974 AnyBlok-2.0.0/anyblok/bloks/model_authz/tests/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      308 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/bloks/model_authz/tests/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6707 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/bloks/model_authz/tests/test_shared_data_testcase.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    49640 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/column.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6304 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/common.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    33327 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/config.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3444 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/conftest.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1873 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/core.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6630 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/declarations.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3604 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/environment.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      658 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/event.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    15272 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/field.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3167 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/imp.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2906 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/logging.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    18027 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/mapper.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    57912 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/migration.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1914 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/mixin.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.093974 AnyBlok-2.0.0/anyblok/model/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    21991 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/model/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1499 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/model/cache.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3800 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/model/event.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      559 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/model/exceptions.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6985 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/model/factory.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1637 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/model/field_datetime.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3255 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/model/hybrid_method.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3392 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/model/plugins.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     7898 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/model/table_and_mapper.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1681 2023-02-22 16:45:31.000000 AnyBlok-2.0.0/anyblok/plugins.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    54833 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/registry.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    56650 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/relationship.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      959 2023-03-11 16:19:44.000000 AnyBlok-2.0.0/anyblok/release.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1944 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/schema.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     8914 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/scripts.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.093974 AnyBlok-2.0.0/anyblok/sphinx/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      316 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/sphinx/__init__.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.093974 AnyBlok-2.0.0/anyblok/sphinx/ext/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      316 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/sphinx/ext/__init__.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.093974 AnyBlok-2.0.0/anyblok/sphinx/ext/load/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      316 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/sphinx/ext/load/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3440 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/sphinx/ext/load/blok.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.093974 AnyBlok-2.0.0/anyblok/test_bloks/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      316 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      469 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/test_bloks/authorization.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.093974 AnyBlok-2.0.0/anyblok/test_bloks/test_blok1/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      600 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok1/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1039 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok1/test.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.093974 AnyBlok-2.0.0/anyblok/test_bloks/test_blok10/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      670 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok10/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1082 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok10/declarations.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.093974 AnyBlok-2.0.0/anyblok/test_bloks/test_blok11/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      600 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok11/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      469 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok11/test.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.093974 AnyBlok-2.0.0/anyblok/test_bloks/test_blok13/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      425 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok13/__init__.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.097974 AnyBlok-2.0.0/anyblok/test_bloks/test_blok14/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2224 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok14/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      552 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok14/test.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.097974 AnyBlok-2.0.0/anyblok/test_bloks/test_blok15/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      466 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok15/__init__.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.097974 AnyBlok-2.0.0/anyblok/test_bloks/test_blok16/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      638 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok16/README.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1009 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok16/__init__.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.097974 AnyBlok-2.0.0/anyblok/test_bloks/test_blok2/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      460 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok2/__init__.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.097974 AnyBlok-2.0.0/anyblok/test_bloks/test_blok3/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      335 2021-07-11 18:02:12.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok3/README.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      438 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok3/__init__.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.097974 AnyBlok-2.0.0/anyblok/test_bloks/test_blok4/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      392 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok4/__init__.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.097974 AnyBlok-2.0.0/anyblok/test_bloks/test_blok5/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      463 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok5/__init__.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.097974 AnyBlok-2.0.0/anyblok/test_bloks/test_blok6/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      438 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok6/__init__.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.097974 AnyBlok-2.0.0/anyblok/test_bloks/test_blok7/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      624 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok7/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      857 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok7/declarations.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.097974 AnyBlok-2.0.0/anyblok/test_bloks/test_blok8/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      670 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok8/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      861 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok8/declarations.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.097974 AnyBlok-2.0.0/anyblok/test_bloks/test_blok9/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      662 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok9/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      537 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/test_bloks/test_blok9/declarations.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    18129 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/testing.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.109974 AnyBlok-2.0.0/anyblok/tests/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      524 2022-02-16 20:21:07.000000 AnyBlok-2.0.0/anyblok/tests/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4141 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/conftest.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.109974 AnyBlok-2.0.0/anyblok/tests/mockblok/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      662 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/mockblok/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       12 2023-02-27 23:20:40.000000 AnyBlok-2.0.0/anyblok/tests/mockblok/mockfile.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.109974 AnyBlok-2.0.0/anyblok/tests/mockblok/mockpackage/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       66 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/mockblok/mockpackage/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       12 2023-02-27 23:20:40.000000 AnyBlok-2.0.0/anyblok/tests/mockblok/mockpackage/mockfile1.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       12 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/mockblok/mockpackage/mockfile2.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.109974 AnyBlok-2.0.0/anyblok/tests/mockblok/mockpackage/submockpackage/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       50 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/mockblok/mockpackage/submockpackage/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       79 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/mockblok/mockpackage/submockpackage/mockfile1.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       12 2023-02-27 23:20:40.000000 AnyBlok-2.0.0/anyblok/tests/mockblok/mockpackage/submockpackage/mockfile2.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6969 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_authorization.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    41200 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_blok.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2056 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/test_blok_manager.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    31044 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/tests/test_cache.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    56014 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/tests/test_column.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    22436 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_config.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3227 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/test_core.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1383 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/test_core_query.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    30129 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_core_sqlbase.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1919 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/test_declaration.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4396 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/test_environment.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    12920 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_event.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    15569 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_field.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3609 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/test_graphviz.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6380 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_hybrid_method.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    36177 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_ignore_migration.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3991 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_imp.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    15245 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_inherit.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     5506 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/test_instrumented_list.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    59015 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_many2many.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    29467 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_many2one.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    13244 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_mapper.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    49672 2023-03-11 16:17:54.000000 AnyBlok-2.0.0/anyblok/tests/test_migration.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    25616 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_migration_db_schema.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3154 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/test_mixin.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    14493 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/test_model.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    18866 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_one2many.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    16298 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_one2one.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    25346 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_polymorphic.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    27522 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_registry.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2103 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/test_registry_core.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2652 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_registry_entry.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     8107 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_registry_manager.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4346 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_relationship.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3426 2023-02-22 16:45:31.000000 AnyBlok-2.0.0/anyblok/tests/test_schema.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1445 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/test_version.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    16221 2023-03-10 09:52:13.000000 AnyBlok-2.0.0/anyblok/tests/test_view.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      670 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/tests/testcase.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1427 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/anyblok/version.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.109974 AnyBlok-2.0.0/anyblok_nose/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      316 2019-09-12 16:00:00.000000 AnyBlok-2.0.0/anyblok_nose/__init__.py
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     5803 2023-02-22 11:01:17.000000 AnyBlok-2.0.0/anyblok_nose/plugins.py
-drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-03-11 16:29:36.113974 AnyBlok-2.0.0/doc/
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    40250 2023-03-11 16:18:44.000000 AnyBlok-2.0.0/doc/CHANGES.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3655 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/doc/FRONT.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      348 2019-09-12 16:00:00.000000 AnyBlok-2.0.0/doc/LICENSE.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    70393 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/doc/MEMENTO.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1206 2019-09-12 16:00:00.000000 AnyBlok-2.0.0/doc/ROADMAP.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     7448 2019-09-12 16:00:00.000000 AnyBlok-2.0.0/doc/advanced_topics.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    37294 2023-02-18 10:31:52.000000 AnyBlok-2.0.0/doc/basic_usage.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1666 2023-02-18 10:31:52.000000 AnyBlok-2.0.0/doc/builtin_bloks.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2072 2023-02-20 09:39:16.000000 AnyBlok-2.0.0/doc/index.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     9577 2023-02-18 10:31:52.000000 AnyBlok-2.0.0/doc/internals.rst
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4382 2023-03-11 16:19:28.000000 AnyBlok-2.0.0/pyproject.toml
--rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       38 2023-03-11 16:29:36.113974 AnyBlok-2.0.0/setup.cfg
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.159172 AnyBlok-2.1.0/
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.095171 AnyBlok-2.1.0/AnyBlok.egg-info/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    46431 2023-07-26 14:47:54.000000 AnyBlok-2.1.0/AnyBlok.egg-info/PKG-INFO
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6290 2023-07-26 14:47:54.000000 AnyBlok-2.1.0/AnyBlok.egg-info/SOURCES.txt
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)        1 2023-07-26 14:47:54.000000 AnyBlok-2.1.0/AnyBlok.egg-info/dependency_links.txt
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2028 2023-07-26 14:47:54.000000 AnyBlok-2.1.0/AnyBlok.egg-info/entry_points.txt
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      322 2023-07-26 14:47:54.000000 AnyBlok-2.1.0/AnyBlok.egg-info/requires.txt
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       21 2023-07-26 14:47:54.000000 AnyBlok-2.1.0/AnyBlok.egg-info/top_level.txt
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    16348 2019-09-12 16:00:00.000000 AnyBlok-2.1.0/LICENSE
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      213 2020-10-16 08:44:47.000000 AnyBlok-2.1.0/MANIFEST.in
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    46431 2023-07-26 14:47:54.159172 AnyBlok-2.1.0/PKG-INFO
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4332 2023-03-13 09:41:18.000000 AnyBlok-2.1.0/README.rst
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.099171 AnyBlok-2.1.0/anyblok/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4105 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    12613 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/_graphviz.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.103171 AnyBlok-2.1.0/anyblok/authorization/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1105 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/authorization/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2804 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/authorization/binding.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2220 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/authorization/query.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.103171 AnyBlok-2.1.0/anyblok/authorization/rule/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      308 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/authorization/rule/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2609 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/authorization/rule/attraccess.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3654 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/authorization/rule/base.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2466 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/authorization/rule/modelaccess.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     9707 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/blok.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.107171 AnyBlok-2.1.0/anyblok/bloks/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      316 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/bloks/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     5347 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok-logo_alpha_256.png
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.115171 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3663 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/CODE.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4293 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      716 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/authorization.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.115171 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/core/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      738 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/core/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3954 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/core/base.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      890 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/core/instrumentedlist.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6452 2023-05-26 13:16:37.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/core/query.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    30565 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/core/sqlbase.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      964 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/core/sqlviewbase.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.115171 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/documentation/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2354 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/documentation/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1571 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/documentation/blok.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.127171 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/documentation/model/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4717 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/documentation/model/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2869 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/documentation/model/attribute.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4411 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/documentation/model/field.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      779 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/exceptions.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.131171 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1051 2023-07-22 18:55:04.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    10183 2023-03-11 16:17:54.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/blok.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3511 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/cache.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3955 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/column.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3163 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/field.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     5953 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/model.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3781 2023-06-29 15:52:13.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/parameter.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3579 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/relationship.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6540 2023-03-11 16:17:54.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/sequence.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.131171 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      316 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1312 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/test_core_base.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     5045 2023-07-26 14:43:41.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/test_core_query.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     7166 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/test_core_sql_base.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1468 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/test_documentation.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1054 2023-07-24 11:14:51.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/test_system_blok.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4429 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/test_system_params.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3315 2023-03-11 16:17:54.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/test_system_sequence.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1174 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/test_testing.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.131171 AnyBlok-2.1.0/anyblok/bloks/anyblok_test/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      624 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/bloks/anyblok_test/__init__.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.131171 AnyBlok-2.1.0/anyblok/bloks/model_authz/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      492 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/bloks/model_authz/CODE.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      323 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/bloks/model_authz/README.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      735 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/bloks/model_authz/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      639 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/bloks/model_authz/models.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.135172 AnyBlok-2.1.0/anyblok/bloks/model_authz/tests/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      308 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/bloks/model_authz/tests/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6707 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/bloks/model_authz/tests/test_shared_data_testcase.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    66020 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/column.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6304 2023-06-30 11:11:04.000000 AnyBlok-2.1.0/anyblok/common.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    33327 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/config.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3444 2023-03-11 16:17:54.000000 AnyBlok-2.1.0/anyblok/conftest.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1873 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/core.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6630 2023-06-30 09:52:05.000000 AnyBlok-2.1.0/anyblok/declarations.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3604 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/environment.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      658 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/event.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    15272 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/field.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3167 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/imp.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2906 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/logging.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    18043 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/mapper.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    57331 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/migration.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1914 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/mixin.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.139171 AnyBlok-2.1.0/anyblok/model/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    22557 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/model/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2415 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/model/cache.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3800 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/model/event.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      559 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/model/exceptions.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6985 2023-07-17 08:33:42.000000 AnyBlok-2.1.0/anyblok/model/factory.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1637 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/model/field_datetime.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3255 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/model/hybrid_method.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3392 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/model/plugins.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     8629 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/model/table_and_mapper.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1681 2023-02-22 16:45:31.000000 AnyBlok-2.1.0/anyblok/plugins.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    55077 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/registry.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    57148 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/relationship.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      959 2023-07-26 14:45:08.000000 AnyBlok-2.1.0/anyblok/release.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1944 2023-03-11 16:17:54.000000 AnyBlok-2.1.0/anyblok/schema.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     8914 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/scripts.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.139171 AnyBlok-2.1.0/anyblok/sphinx/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      316 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/sphinx/__init__.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.139171 AnyBlok-2.1.0/anyblok/sphinx/ext/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      316 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/sphinx/ext/__init__.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.139171 AnyBlok-2.1.0/anyblok/sphinx/ext/load/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      316 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/sphinx/ext/load/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3440 2023-03-11 16:17:54.000000 AnyBlok-2.1.0/anyblok/sphinx/ext/load/blok.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.139171 AnyBlok-2.1.0/anyblok/test_bloks/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      316 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      469 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/test_bloks/authorization.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.139171 AnyBlok-2.1.0/anyblok/test_bloks/test_blok1/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      600 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok1/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1039 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok1/test.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.139171 AnyBlok-2.1.0/anyblok/test_bloks/test_blok10/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      670 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok10/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1082 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok10/declarations.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.143172 AnyBlok-2.1.0/anyblok/test_bloks/test_blok11/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      600 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok11/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      469 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok11/test.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.143172 AnyBlok-2.1.0/anyblok/test_bloks/test_blok13/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      425 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok13/__init__.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.143172 AnyBlok-2.1.0/anyblok/test_bloks/test_blok14/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2224 2023-05-15 12:10:45.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok14/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      552 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok14/test.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.143172 AnyBlok-2.1.0/anyblok/test_bloks/test_blok15/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      466 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok15/__init__.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.143172 AnyBlok-2.1.0/anyblok/test_bloks/test_blok16/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      638 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok16/README.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1009 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok16/__init__.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.143172 AnyBlok-2.1.0/anyblok/test_bloks/test_blok2/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      460 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok2/__init__.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.143172 AnyBlok-2.1.0/anyblok/test_bloks/test_blok3/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      335 2021-07-11 18:02:12.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok3/README.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      438 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok3/__init__.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.143172 AnyBlok-2.1.0/anyblok/test_bloks/test_blok4/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      392 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok4/__init__.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.143172 AnyBlok-2.1.0/anyblok/test_bloks/test_blok5/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      463 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok5/__init__.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.143172 AnyBlok-2.1.0/anyblok/test_bloks/test_blok6/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      438 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok6/__init__.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.143172 AnyBlok-2.1.0/anyblok/test_bloks/test_blok7/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      624 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok7/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      857 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok7/declarations.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.143172 AnyBlok-2.1.0/anyblok/test_bloks/test_blok8/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      670 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok8/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      861 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok8/declarations.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.143172 AnyBlok-2.1.0/anyblok/test_bloks/test_blok9/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      662 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok9/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      537 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/test_bloks/test_blok9/declarations.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    18129 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/testing.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.155172 AnyBlok-2.1.0/anyblok/tests/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      524 2022-02-16 20:21:07.000000 AnyBlok-2.1.0/anyblok/tests/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4141 2023-06-29 15:00:15.000000 AnyBlok-2.1.0/anyblok/tests/conftest.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.155172 AnyBlok-2.1.0/anyblok/tests/mockblok/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      662 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/mockblok/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       12 2023-07-24 07:53:15.000000 AnyBlok-2.1.0/anyblok/tests/mockblok/mockfile.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.155172 AnyBlok-2.1.0/anyblok/tests/mockblok/mockpackage/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       66 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/mockblok/mockpackage/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       12 2023-07-24 07:53:15.000000 AnyBlok-2.1.0/anyblok/tests/mockblok/mockpackage/mockfile1.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       12 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/mockblok/mockpackage/mockfile2.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.155172 AnyBlok-2.1.0/anyblok/tests/mockblok/mockpackage/submockpackage/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       50 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/mockblok/mockpackage/submockpackage/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       79 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/mockblok/mockpackage/submockpackage/mockfile1.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       12 2023-07-24 07:53:15.000000 AnyBlok-2.1.0/anyblok/tests/mockblok/mockpackage/submockpackage/mockfile2.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6969 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_authorization.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    41200 2023-05-15 12:10:26.000000 AnyBlok-2.1.0/anyblok/tests/test_blok.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2056 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/test_blok_manager.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    31044 2023-03-11 16:17:54.000000 AnyBlok-2.1.0/anyblok/tests/test_cache.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    67723 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/tests/test_column.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    22436 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_config.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3227 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/test_core.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1383 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/test_core_query.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    30129 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_core_sqlbase.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1919 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/test_declaration.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2006 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/tests/test_deprecated_models.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4396 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/test_environment.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    12920 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_event.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    15569 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_field.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3609 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/test_graphviz.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     6380 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_hybrid_method.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    36177 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_ignore_migration.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3991 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_imp.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    15429 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/tests/test_inherit.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     5506 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/test_instrumented_list.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    59015 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_many2many.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    29467 2023-07-12 16:18:47.000000 AnyBlok-2.1.0/anyblok/tests/test_many2one.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    13174 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/tests/test_mapper.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    49672 2023-06-29 10:11:52.000000 AnyBlok-2.1.0/anyblok/tests/test_migration.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    25616 2023-05-15 15:01:17.000000 AnyBlok-2.1.0/anyblok/tests/test_migration_db_schema.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3154 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/test_mixin.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    14378 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/tests/test_model.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    18866 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_one2many.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    16298 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_one2one.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    26202 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/anyblok/tests/test_polymorphic.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    27522 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_registry.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2103 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/test_registry_core.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2652 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_registry_entry.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     8107 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_registry_manager.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4346 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_relationship.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3426 2023-02-22 16:45:31.000000 AnyBlok-2.1.0/anyblok/tests/test_schema.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1445 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/test_version.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    16221 2023-03-10 09:52:13.000000 AnyBlok-2.1.0/anyblok/tests/test_view.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      670 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/tests/testcase.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1427 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/anyblok/version.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.155172 AnyBlok-2.1.0/anyblok_nose/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      316 2019-09-12 16:00:00.000000 AnyBlok-2.1.0/anyblok_nose/__init__.py
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     5803 2023-02-22 11:01:17.000000 AnyBlok-2.1.0/anyblok_nose/plugins.py
+drwxr-xr-x   0 jssuzanne  (1000) jssuzanne  (1000)        0 2023-07-26 14:47:54.159172 AnyBlok-2.1.0/doc/
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    40878 2023-07-26 14:40:59.000000 AnyBlok-2.1.0/doc/CHANGES.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     3655 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/doc/FRONT.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)      348 2019-09-12 16:00:00.000000 AnyBlok-2.1.0/doc/LICENSE.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    75807 2023-07-26 14:39:20.000000 AnyBlok-2.1.0/doc/MEMENTO.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1206 2019-09-12 16:00:00.000000 AnyBlok-2.1.0/doc/ROADMAP.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     7448 2019-09-12 16:00:00.000000 AnyBlok-2.1.0/doc/advanced_topics.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)    37294 2023-02-18 10:31:52.000000 AnyBlok-2.1.0/doc/basic_usage.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     1666 2023-02-18 10:31:52.000000 AnyBlok-2.1.0/doc/builtin_bloks.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     2072 2023-02-20 09:39:16.000000 AnyBlok-2.1.0/doc/index.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     9577 2023-02-18 10:31:52.000000 AnyBlok-2.1.0/doc/internals.rst
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)     4382 2023-07-26 14:45:00.000000 AnyBlok-2.1.0/pyproject.toml
+-rw-r--r--   0 jssuzanne  (1000) jssuzanne  (1000)       38 2023-07-26 14:47:54.159172 AnyBlok-2.1.0/setup.cfg
```

### Comparing `AnyBlok-2.0.0/AnyBlok.egg-info/PKG-INFO` & `AnyBlok-2.1.0/AnyBlok.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnyBlok
-Version: 2.0.0
+Version: 2.1.0
 Summary: Anyblok is a dynamic injection blok framework
 Author-email: Jean-Sébastien Suzanne <jssuzanne@anybox.fr>
 License: MPL2
 Project-URL: Homepage, https://doc.anyblok.org/en/1.4.0/
 Keywords: django,notifications,delayed sending
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -184,14 +184,28 @@
 .. This Source Code Form is subject to the terms of the Mozilla Public License,
 .. v. 2.0. If a copy of the MPL was not distributed with this file,You can
 .. obtain one at http://mozilla.org/MPL/2.0/.
 
 CHANGELOG
 =========
 
+2.1.0 (2023-07-26)
+------------------
+
+* Implement psycopg3 capability
+* Improved TimeStamp field
+* Fixed #227 str and repr of the query call str query.sql_statement
+* Refactored main methods to get the description of the models and fields
+  without used the existing table
+* Added new column type **ModelSelection** this role is to replace a column
+  with a foreigh key to the deprecated model **Model.System.Model**
+* Added new column type **ModelFieldSelection** this role is to replace a
+  column with a foreigh key to the deprecated model **Model.System.Field**,
+  **Model.System.Column** or **Model.System.Relationship**
+
 2.0.0 (2023-03-11)
 ------------------
 
 * Upgrade version of sqlalchemy to **2.0.0**
 * Upgrade version of sqlalchemy utils to **0.40.0**
 * Upgrade version of sqlalchemy views to **0.3.2**
 * The previsous deprecated configuration are placed as removed
```

### Comparing `AnyBlok-2.0.0/AnyBlok.egg-info/SOURCES.txt` & `AnyBlok-2.1.0/AnyBlok.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -65,23 +65,18 @@
 anyblok/bloks/anyblok_core/system/model.py
 anyblok/bloks/anyblok_core/system/parameter.py
 anyblok/bloks/anyblok_core/system/relationship.py
 anyblok/bloks/anyblok_core/system/sequence.py
 anyblok/bloks/anyblok_core/tests/__init__.py
 anyblok/bloks/anyblok_core/tests/test_core_base.py
 anyblok/bloks/anyblok_core/tests/test_core_query.py
-anyblok/bloks/anyblok_core/tests/test_core_session.py
 anyblok/bloks/anyblok_core/tests/test_core_sql_base.py
 anyblok/bloks/anyblok_core/tests/test_documentation.py
 anyblok/bloks/anyblok_core/tests/test_system_blok.py
-anyblok/bloks/anyblok_core/tests/test_system_column.py
-anyblok/bloks/anyblok_core/tests/test_system_field.py
-anyblok/bloks/anyblok_core/tests/test_system_model.py
 anyblok/bloks/anyblok_core/tests/test_system_params.py
-anyblok/bloks/anyblok_core/tests/test_system_relationship.py
 anyblok/bloks/anyblok_core/tests/test_system_sequence.py
 anyblok/bloks/anyblok_core/tests/test_testing.py
 anyblok/bloks/anyblok_test/__init__.py
 anyblok/bloks/model_authz/CODE.rst
 anyblok/bloks/model_authz/README.rst
 anyblok/bloks/model_authz/__init__.py
 anyblok/bloks/model_authz/models.py
@@ -134,14 +129,15 @@
 anyblok/tests/test_cache.py
 anyblok/tests/test_column.py
 anyblok/tests/test_config.py
 anyblok/tests/test_core.py
 anyblok/tests/test_core_query.py
 anyblok/tests/test_core_sqlbase.py
 anyblok/tests/test_declaration.py
+anyblok/tests/test_deprecated_models.py
 anyblok/tests/test_environment.py
 anyblok/tests/test_event.py
 anyblok/tests/test_field.py
 anyblok/tests/test_graphviz.py
 anyblok/tests/test_hybrid_method.py
 anyblok/tests/test_ignore_migration.py
 anyblok/tests/test_imp.py
```

### Comparing `AnyBlok-2.0.0/AnyBlok.egg-info/entry_points.txt` & `AnyBlok-2.1.0/AnyBlok.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/LICENSE` & `AnyBlok-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/PKG-INFO` & `AnyBlok-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnyBlok
-Version: 2.0.0
+Version: 2.1.0
 Summary: Anyblok is a dynamic injection blok framework
 Author-email: Jean-Sébastien Suzanne <jssuzanne@anybox.fr>
 License: MPL2
 Project-URL: Homepage, https://doc.anyblok.org/en/1.4.0/
 Keywords: django,notifications,delayed sending
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -184,14 +184,28 @@
 .. This Source Code Form is subject to the terms of the Mozilla Public License,
 .. v. 2.0. If a copy of the MPL was not distributed with this file,You can
 .. obtain one at http://mozilla.org/MPL/2.0/.
 
 CHANGELOG
 =========
 
+2.1.0 (2023-07-26)
+------------------
+
+* Implement psycopg3 capability
+* Improved TimeStamp field
+* Fixed #227 str and repr of the query call str query.sql_statement
+* Refactored main methods to get the description of the models and fields
+  without used the existing table
+* Added new column type **ModelSelection** this role is to replace a column
+  with a foreigh key to the deprecated model **Model.System.Model**
+* Added new column type **ModelFieldSelection** this role is to replace a
+  column with a foreigh key to the deprecated model **Model.System.Field**,
+  **Model.System.Column** or **Model.System.Relationship**
+
 2.0.0 (2023-03-11)
 ------------------
 
 * Upgrade version of sqlalchemy to **2.0.0**
 * Upgrade version of sqlalchemy utils to **0.40.0**
 * Upgrade version of sqlalchemy views to **0.3.2**
 * The previsous deprecated configuration are placed as removed
```

### Comparing `AnyBlok-2.0.0/README.rst` & `AnyBlok-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/__init__.py` & `AnyBlok-2.1.0/anyblok/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/_graphviz.py` & `AnyBlok-2.1.0/anyblok/_graphviz.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/authorization/__init__.py` & `AnyBlok-2.1.0/anyblok/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/authorization/binding.py` & `AnyBlok-2.1.0/anyblok/authorization/binding.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/authorization/query.py` & `AnyBlok-2.1.0/anyblok/authorization/query.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/authorization/rule/attraccess.py` & `AnyBlok-2.1.0/anyblok/authorization/rule/attraccess.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/authorization/rule/base.py` & `AnyBlok-2.1.0/anyblok/authorization/rule/base.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/authorization/rule/modelaccess.py` & `AnyBlok-2.1.0/anyblok/authorization/rule/modelaccess.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/blok.py` & `AnyBlok-2.1.0/anyblok/blok.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #
 #    Copyright (C) 2014 Jean-Sebastien SUZANNE <jssuzanne@anybox.fr>
 #    Copyright (C) 2021 Jean-Sebastien SUZANNE <js.suzanne@gmail.com>
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License,
 # v. 2.0. If a copy of the MPL was not distributed with this file,You can
 # obtain one at http://mozilla.org/MPL/2.0/.
-import warnings
 from logging import getLogger
 from os.path import dirname
 from sys import modules
 from time import sleep
 
 from pkg_resources import iter_entry_points
 
@@ -283,25 +282,14 @@
     name = None  # set by the BlokManager
     author = ""
     logo = ""
 
     def __init__(self, registry):
         self.anyblok = registry
 
-    @property
-    def registry(self):  # pragma: no cover
-        warnings.warn(
-            "'registry' attribute is deprecated because SQLAlchemy 1.4 add is "
-            "own 'registry' attribute. Replace it by 'anyblok' attribute",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-
-        return self.anyblok
-
     @classmethod
     def import_declaration_module(cls):
         """Do the python import for the Declaration of the model or other"""
 
     def update(self, latest_version):
         """Called on install or update
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok-logo_alpha_256.png` & `AnyBlok-2.1.0/anyblok/bloks/anyblok-logo_alpha_256.png`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/CODE.rst` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/CODE.rst`

 * *Files 2% similar despite different names*

```diff
@@ -75,29 +75,45 @@
     :members:
 
 .. automodule:: anyblok.bloks.anyblok_core.system.field
 
 .. autoanyblok-declaration:: Field
     :members:
 
+.. warning::
+
+    Deprecated
+
 .. automodule:: anyblok.bloks.anyblok_core.system.column
 
 .. autoanyblok-declaration:: Column
     :members:
 
+.. warning::
+
+    Deprecated
+
 .. automodule:: anyblok.bloks.anyblok_core.system.relationship
 
 .. autoanyblok-declaration:: RelationShip
     :members:
 
+.. warning::
+
+    Deprecated
+
 .. automodule:: anyblok.bloks.anyblok_core.system.model
 
 .. autoanyblok-declaration:: Model
     :members:
 
+.. warning::
+
+    Deprecated
+
 .. automodule:: anyblok.bloks.anyblok_core.system.parameter
 
 .. autoanyblok-declaration:: Parameter
     :members:
 
 .. automodule:: anyblok.bloks.anyblok_core.system.sequence
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/__init__.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/authorization.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/authorization.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/core/__init__.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/core/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/core/base.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/core/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,19 @@
     def initialize_model(cls):
         """This method is called to initialize a model during the creation of
         the registry
         """
         pass
 
     @classmethod
+    def clear_all_model_caches(cls):
+        """Clear all caches in the case of bloks changes"""
+        pass
+
+    @classmethod
     def fire(cls, event, *args, **kwargs):
         """Call a specific event on the model
 
         :param event: Name of the event
         """
         events = cls.anyblok.events
         if cls.__registry_name__ in events:
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/core/instrumentedlist.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/core/instrumentedlist.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/core/query.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/core/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,20 @@
 
         return wrapper
 
     def __iter__(self):
         for res in self._execute():
             yield res
 
+    def __str__(self):
+        return str(self.sql_statement)
+
+    def __repr__(self):
+        return str(self.sql_statement)
+
     def _execute(self):
         res = self.Model.execute(self.sql_statement)
         if self.elements:
             return res
 
         return res.scalars()
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/core/sqlbase.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/core/sqlbase.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # This file is a part of the AnyBlok project
 #
 #    Copyright (C) 2014 Jean-Sebastien SUZANNE <jssuzanne@anybox.fr>
 #    Copyright (C) 2019 Jean-Sebastien SUZANNE <js.suzanne@gmail.com>
 #    Copyright (C) 2021 Jean-Sebastien SUZANNE <js.suzanne@gmail.com>
+#    Copyright (C) 2023 Jean-Sebastien SUZANNE <js.suzanne@gmail.com>
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License,
 # v. 2.0. If a copy of the MPL was not distributed with this file,You can
 # obtain one at http://mozilla.org/MPL/2.0/.
 from sqlalchemy import and_, delete, inspect, or_, select
 from sqlalchemy import update as sqla_update
 from sqlalchemy.orm import ColumnProperty, aliased
 from sqlalchemy.orm.base import LoaderCallableStatus
 from sqlalchemy.orm.session import object_state
-from sqlalchemy.sql.expression import true
 from sqlalchemy_utils.models import NOT_LOADED_REPR
 
 from anyblok.column import Column
 from anyblok.common import anyblok_column_prefix
 from anyblok.declarations import Declarations, classmethod_cache
 from anyblok.field import FieldException
 from anyblok.mapper import FakeColumn, FakeRelationShip
@@ -79,14 +79,31 @@
 
         return "<%s(%s)>" % (
             self.__class__.__registry_name__,
             ", ".join(field_reprs),
         )
 
     @classmethod
+    def initialize_model(cls):
+        super().initialize_model()
+        cls.SQLAMapper = inspect(cls)
+
+    @classmethod
+    def clear_all_model_caches(cls):
+        super().clear_all_model_caches()
+        Cache = cls.anyblok.System.Cache
+        Cache.invalidate(cls, "_fields_description")
+        Cache.invalidate(cls, "fields_name")
+        Cache.invalidate(cls, "getFieldType")
+        Cache.invalidate(cls, "get_primary_keys")
+        Cache.invalidate(cls, "find_remote_attribute_to_expire")
+        Cache.invalidate(cls, "find_relationship")
+        Cache.invalidate(cls, "get_hybrid_property_columns")
+
+    @classmethod
     def define_table_args(cls):
         return ()
 
     @classmethod
     def define_table_kwargs(cls):
         res = {}
         if cls.__db_schema__ is not None:
@@ -258,36 +275,164 @@
 
     @classmethod_cache()
     def get_primary_keys(cls):
         """return the name of the primary keys of the model
 
         :type: list of the primary keys name
         """
-        C = cls.anyblok.System.Column
-        query = C.select_sql_statement(C.name)
-        query = query.group_by(C.name)
-        query = query.where(C.model.in_(cls.get_all_registry_names()))
-        query = query.where(C.primary_key == true())
-        query_res = cls.execute_sql_statement(query)
-        return [x[0] for x in query_res]
+        return list(
+            {
+                column.key
+                for model in cls.get_all_registry_names()
+                for column in cls.anyblok.get(model).SQLAMapper.primary_key
+            }
+        )
+
+    @classmethod
+    def _fields_description_field(cls):
+        res = {}
+        fsp = cls.anyblok.loaded_namespaces_first_step[cls.__registry_name__]
+        for cname in cls.loaded_fields:
+            ftype = fsp[cname].__class__.__name__
+            res[cname] = dict(
+                id=cname,
+                label=cls.loaded_fields[cname],
+                type=ftype,
+                nullable=True,
+                primary_key=False,
+                model=None,
+            )
+            fsp[cname].update_description(
+                cls.anyblok, cls.__registry_name__, res[cname]
+            )
+
+        return res
+
+    @classmethod
+    def _fields_description_column(cls):
+        res = {}
+        fsp = cls.anyblok.loaded_namespaces_first_step[cls.__registry_name__]
+        for field in cls.SQLAMapper.columns:
+            if field.key not in fsp:
+                continue
+
+            ftype = fsp[field.key].__class__.__name__
+            res[field.key] = dict(
+                id=field.key,
+                label=field.info.get("label"),
+                type=ftype,
+                nullable=field.nullable,
+                primary_key=field.primary_key,
+                model=field.info.get("remote_model"),
+            )
+            fsp[field.key].update_description(
+                cls.anyblok, cls.__registry_name__, res[field.key]
+            )
+
+        return res
+
+    @classmethod
+    def _fields_description_relationship(cls):
+        res = {}
+        fsp = cls.anyblok.loaded_namespaces_first_step[cls.__registry_name__]
+        for field in cls.SQLAMapper.relationships:
+            key = (
+                field.key[len(anyblok_column_prefix) :]
+                if field.key.startswith(anyblok_column_prefix)
+                else field.key
+            )
+            ftype = fsp[key].__class__.__name__
+            if ftype == "FakeRelationShip":
+                Model = field.mapper.entity
+                model = Model.__registry_name__
+                nullable = True
+                remote_name = field.back_populates
+                if remote_name.startswith(anyblok_column_prefix):
+                    remote_name = remote_name[len(anyblok_column_prefix) :]
+
+                remote = getattr(Model, remote_name)
+                remote_columns = remote.info.get("local_columns", [])
+                local_columns = remote.info.get("remote_columns", [])
+                rtype = remote.info["rtype"]
+                if rtype == "Many2One":
+                    ftype = "One2Many"
+                elif rtype == "Many2Many":
+                    ftype = "Many2Many"
+                elif rtype == "One2One":
+                    ftype = "One2One"
+            else:
+                local_columns = field.info.get("local_columns", [])
+                remote_columns = field.info.get("remote_columns", [])
+                nullable = field.info.get("nullable", True)
+                model = field.info.get("remote_model")
+                remote_name = field.info.get("remote_name")
+
+            res[key] = dict(
+                id=key,
+                label=field.info.get("label"),
+                type=ftype,
+                nullable=nullable,
+                model=model,
+                local_columns=local_columns,
+                remote_columns=remote_columns,
+                remote_name=remote_name,
+                primary_key=False,
+            )
+            fsp[key].update_description(
+                cls.anyblok, cls.__registry_name__, res[key]
+            )
+
+        return res
 
     @classmethod_cache()
     def _fields_description(cls):
         """Return the information of the Field, Column, RelationShip"""
-        Field = cls.anyblok.System.Field
         res = {}
         for registry_name in cls.__depends__:
-            query = Field.query().filter(Field.model == registry_name)
-            res.update({x.name: x._description() for x in query})
+            Depend = cls.anyblok.get(registry_name)
+            res.update(Depend._fields_description())
 
-        query = Field.query().filter(Field.model == cls.__registry_name__)
-        res.update({x.name: x._description() for x in query})
+        res.update(cls._fields_description_field())
+        res.update(cls._fields_description_column())
+        res.update(cls._fields_description_relationship())
         return res
 
     @classmethod
+    def _fields_name_field(cls):
+        return [cname for cname in cls.loaded_fields]
+
+    @classmethod
+    def _fields_name_column(cls):
+        return [field.key for field in cls.SQLAMapper.columns]
+
+    @classmethod
+    def _fields_name_relationship(cls):
+        return [
+            (
+                field.key[len(anyblok_column_prefix) :]
+                if field.key.startswith(anyblok_column_prefix)
+                else field.key
+            )
+            for field in cls.SQLAMapper.relationships
+        ]
+
+    @classmethod_cache()
+    def fields_name(cls):
+        """Return the name of the Field, Column, RelationShip"""
+        res = []
+        for registry_name in cls.__depends__:
+            Depend = cls.anyblok.get(registry_name)
+            res.extend(Depend.fields_name())
+
+        res.extend(cls._fields_name_field())
+        res.extend(cls._fields_name_column())
+        res.extend(cls._fields_name_relationship())
+        return list(set(res))
+
+    @classmethod
     def fields_description(cls, fields=None):
         res = cls._fields_description()
         if fields:
             return {x: y for x, y in res.items() if x in fields}
 
         return res
 
@@ -452,20 +597,15 @@
             TheModel.getFieldType(nameOfTheColumn)
 
         this method take care if it is a polymorphic model or not
 
         :param name: name of the column
         :rtype: String, the name of the Type of column used
         """
-        Field = cls.anyblok.System.Field
-        query = Field.query()
-        query = query.filter(Field.name == name)
-        query = query.filter(Field.model.in_(cls.get_all_registry_names()))
-        query = query.limit(1)
-        return query.one().ftype
+        return cls.fields_description(name)[name]["type"]
 
     @classmethod_cache()
     def find_remote_attribute_to_expire(cls, *fields):
         res = uniquedict()
         _fields = []
         _fields.extend(fields)
         model = get_model_information(cls.anyblok, cls.__registry_name__)
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/core/sqlviewbase.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/core/sqlviewbase.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/documentation/__init__.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/documentation/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 from anyblok import Declarations, reload_module_if_blok_is_reloading
 
 
 @Declarations.register(Declarations.Mixin)
 class DocElement:
     def _auto_doc(self, Model, elements, *args, **kwargs):
         for el in Model.getelements(*args, **kwargs):
-            _el = Model(el)
-            if _el.exist(*args, **kwargs):
-                elements.append(_el)
+            elements.append(Model(el, self))
 
     def _toRST(self, doc, Model, elements):
         Model.header2RST(doc)
         for el in elements:
             el.toRST(doc)
 
         Model.footer2RST(doc)
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/documentation/blok.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/documentation/blok.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,21 @@
 #
 #    Copyright (C) 2015 Jean-Sebastien SUZANNE <jssuzanne@anybox.fr>
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License,
 # v. 2.0. If a copy of the MPL was not distributed with this file,You can
 # obtain one at http://mozilla.org/MPL/2.0/.
 from anyblok import Declarations
-from anyblok.blok import BlokManager
 
 
 @Declarations.register(Declarations.Model.Documentation)
 class Blok:
-    def __init__(self, blok):
+    def __init__(self, blok, parent):
         self.blok = blok
 
-    def exist(self):
-        return BlokManager.has(self.blok.name)
-
     @classmethod
     def filterBloks(cls, query):
         Blok = cls.anyblok.System.Blok
         return query.filter(Blok.state == "installed").order_by(Blok.order)
 
     @classmethod
     def getelements(cls):
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/documentation/model/__init__.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/documentation/model/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,82 +7,87 @@
 # obtain one at http://mozilla.org/MPL/2.0/.
 from anyblok import Declarations, reload_module_if_blok_is_reloading
 from anyblok.config import Configuration
 
 
 @Declarations.register(Declarations.Model.Documentation)
 class Model(Declarations.Mixin.DocElement):
-    def __init__(self, model):
+    def __init__(self, model, parent):
         self.model = model
         self.fields = []
         self.attributes = []
         if self.exist():
             self._auto_doc(
                 self.anyblok.Documentation.Model.Field, self.fields, self
             )
             self._auto_doc(
                 self.anyblok.Documentation.Model.Attribute,
                 self.attributes,
                 self,
             )
 
     def exist(self):
-        return self.anyblok.has(self.model.name)
+        return self.anyblok.has(self.model)
 
     @classmethod
-    def get_all_models(cls, models):  # pragma: no cover
-        Model = cls.anyblok.System.Model
-        res = []
-        for model in models:
-            if model[-2:] == ".*":
-                query = Model.query().filter(Model.name.like(model[:-1] + "%"))
-                res.extend(query.all().name)
-            else:
-                res.append(model)
-
-        return res
-
-    @classmethod
-    def filterModel(cls, query):
-        Model = cls.anyblok.System.Model
-        wanted_models = Configuration.get("doc_wanted_models")
+    def filterModel(cls, models):  # noqa: C901
+        wanted_models = Configuration.get("doc_wanted_models") or []
         if wanted_models:  # pragma: no cover
-            wanted_models = cls.get_all_models(wanted_models)
-            query = query.filter(Model.name.in_(wanted_models))
-        else:
-            wanted_models = []
+            new_models = []
+            for model in models:
+                for wanted_model in wanted_models:
+                    if wanted_model[-1] == "*" and model.startswidth(
+                        wanted_model[:-1]
+                    ):
+                        new_models.append(model)
+                    elif wanted_model == model:
+                        new_models.append(model)
+            models = new_models
 
-        unwanted_models = Configuration.get("doc_unwanted_models")
+        unwanted_models = Configuration.get("doc_unwanted_models") or []
         if unwanted_models:  # pragma: no cover
-            unwanted_models = cls.get_all_models(unwanted_models)
             unwanted_models = [
                 x for x in unwanted_models if x not in wanted_models
             ]
-            query = query.filter(Model.name.notin_(unwanted_models))
+            new_models = []
+            for model in models:
+                for unwanted_model in unwanted_models:
+                    if unwanted_model[-1] == "*" and model.startswidth(
+                        unwanted_model[:-1]
+                    ):
+                        continue
+                    elif unwanted_model == model:
+                        continue
 
-        return query
+                    new_models.append(model)
+
+            models = new_models
+
+        return models
 
     @classmethod
     def getelements(cls):
-        return cls.filterModel(cls.anyblok.System.Model.query()).all()
+        return cls.filterModel(
+            [x for x in cls.anyblok.loaded_namespaces.keys()]
+        )
 
     @classmethod
     def header2RST(cls, doc):
         doc.write(
             "Models\n======\n\n"
             "This the differents models defined "
             "on the project" + ("\n" * 2)
         )
 
     @classmethod
     def footer2RST(cls, doc):
         pass
 
     def toRST(self, doc):
-        doc.write(self.model.name + "\n" + "-" * len(self.model.name) + "\n\n")
+        doc.write(self.model + "\n" + "-" * len(self.model) + "\n\n")
         self.toRST_docstring(doc)
         self.toRST_properties(doc)
         self.toRST_field(doc)
         self.toRST_method(doc)
 
     def toRST_field(self, doc):
         if self.fields:
@@ -93,49 +98,49 @@
     def toRST_method(self, doc):
         if self.attributes:
             self._toRST(
                 doc, self.anyblok.Documentation.Model.Attribute, self.attributes
             )
 
     def toRST_docstring(self, doc):
-        Model = self.anyblok.get(self.model.name)
+        Model = self.anyblok.get(self.model)
         if hasattr(Model, "__doc__") and Model.__doc__:
             doc.write(Model.__doc__ + "\n\n")
 
     def toRST_properties_get(self):
-        Model = self.anyblok.get(self.model.name)
+        Model = self.anyblok.get(self.model)
         tablename = getattr(Model, "__tablename__", "No table")
         return {
             "table name": tablename,
         }
 
     def toRST_properties(self, doc):
         properties = self.toRST_properties_get()
         msg = "Properties:\n\n* " + "\n* ".join(
             "**%s** : %s" % (x, y) for x, y in properties.items()
         )
         doc.write(msg + "\n\n")
 
     def toUML_add_model(self, dot):
-        dot.add_class(self.model.name)
+        dot.add_class(self.model)
 
     def toUML_add_attributes(self, dot):
         for f in self.fields:
             f.toUML(dot)
 
         for attr in self.attributes:
-            attr.toUML(dot, self.model.name)
+            attr.toUML(dot, self.model)
 
     def toSQL_add_table(self, dot):
-        Model = self.anyblok.get(self.model.name)
+        Model = self.anyblok.get(self.model)
         if hasattr(Model, "__tablename__"):
             dot.add_table(Model.__tablename__)
 
     def toSQL_add_fields(self, dot):
-        Model = self.anyblok.get(self.model.name)
+        Model = self.anyblok.get(self.model)
         if hasattr(Model, "__tablename__"):
             for f in self.fields:
                 f.toSQL(dot)
 
 
 from . import field  # noqa
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/documentation/model/attribute.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/documentation/model/attribute.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,17 @@
 
 from anyblok import Declarations
 from anyblok.field import FieldException
 
 
 @Declarations.register(Declarations.Model.Documentation.Model)
 class Attribute:
-    def __init__(self, attribute):
+    def __init__(self, attribute, parent):
         self.name, self.attribute = attribute
 
-    def exist(self, model):
-        return model.exist()
-
     @classmethod
     def filterAttribute(cls, model, name):
         if name in (
             "insert",
             "update",
             "to_primary_keys",
             "to_dict",
@@ -54,15 +51,15 @@
             return True
 
         return False
 
     @classmethod
     def getelements(cls, model):
         res = []
-        Model = cls.anyblok.get(model.model.name)
+        Model = cls.anyblok.get(model.model)
         try:
             for k, v in getmembers(Model):
                 if ismodule(v) or isclass(v):
                     continue
 
                 if k.startswith("__"):
                     continue
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/documentation/model/field.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/documentation/model/field.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,96 +21,74 @@
         ("Many2Many", False): ("m2m", None),
         ("One2Many", True): ("o2m", "m2o"),
         ("One2Many", False): ("o2m", None),
         ("One2One", True): ("o2o", "o2o"),
         ("One2One", False): ("o2o", "o2o"),
     }
 
-    def exist(self, model):
-        if not model.exist():
-            return False  # pragma: no cover
-
-        M = self.anyblok.get(model.model.name)
-        if self.field.name in M.loaded_columns:
-            return True
-
-        return False  # pragma: no cover
-
-    def __init__(self, field):
+    def __init__(self, field, parent):
         self.field = field
-
-    @classmethod
-    def filterField(cls, query):
-        return query
+        self.model = parent.model
 
     @classmethod
     def getelements(cls, model):
-        query = cls.filterField(cls.anyblok.System.Field.query())
-        return query.filter(
-            cls.anyblok.System.Field.model == model.model.name
-        ).all()
+        Model = cls.anyblok.get(model.model)
+        if Model.is_sql:
+            return Model.fields_description().values()
+
+        return []
 
     @classmethod
     def header2RST(cls, doc):
         doc.write("Fields\n~~~~~~\n\n")
 
     @classmethod
     def footer2RST(cls, doc):
         pass
 
     def toRST(self, doc):
-        doc.write("* " + self.field.name + "\n\n")
+        doc.write("* " + self.field["id"] + "\n\n")
         self.toRST_docstring(doc)
         self.toRST_properties(doc)
 
     def toRST_docstring(self, doc):
         if hasattr(self.field, "__doc__") and self.field.__doc__:
             doc.write(self.field.__doc__ + "\n\n")  # pragma: no cover
 
     def toRST_properties_get(self):
-        return {x: y for x, y in self.field.to_dict().items() if x != "name"}
+        return {x: y for x, y in self.field.items() if x != "id"}
 
     def toRST_properties(self, doc):
         properties = self.toRST_properties_get()
         msg = ", ".join(" **%s** (%s)" % (x, y) for x, y in properties.items())
         doc.write(msg + "\n\n")
 
     def toUML(self, dot):
-        if self.field.entity_type == "Model.System.Field":
-            self.toUML_field(dot)
-        elif self.field.entity_type == "Model.System.Column":
-            self.toUML_column(dot)
-        elif (
-            self.field.entity_type == "Model.System.RelationShip"
-        ):  # pragma: no cover
-            self.toUML_relationship(dot)
+        if "remote_name" in self.field:
+            self.toUML_relationship(dot)  # pragma: no cover
         else:
-            logger.warning("Unknown entity type %r" % self.field.entity_type)
-
-    def toUML_field(self, dot):
-        model = dot.get_class(self.field.model)
-        model.add_column(self.field.name)
+            self.toUML_column(dot)
 
     def toUML_column(self, dot):
-        model = dot.get_class(self.field.model)
-        name = self.field.name
-        if self.field.primary_key:
+        model = dot.get_class(self.model)
+        name = self.field["id"]
+        if self.field["primary_key"]:
             name = "+PK+ " + name
 
-        if self.field.remote_model:  # pragma: no cover
-            remote_model = dot.get_class(self.field.remote_model)
+        if self.field["model"]:  # pragma: no cover
+            remote_model = dot.get_class(self.field["model"])
             multiplicity = "1"
-            if self.field.nullable:
+            if self.field["nullable"]:
                 multiplicity = "0..1"
 
             model.aggregate(
                 remote_model, label_from=name, multiplicity_from=multiplicity
             )
         else:
-            name += " (%s)" % self.field.ftype
+            name += " (%s)" % self.field["type"]
             model.add_column(name)
 
     def toUML_relationship(self, dot):  # pragma: no cover
         if self.field.remote:
             return
 
         model = dot.get_class(self.field.model)
@@ -122,46 +100,40 @@
             label_from=self.field.name,
             label_to=self.field.remote_name,
             multiplicity_from=multiplicity,
             multiplicity_to=multiplicity_to,
         )
 
     def toSQL(self, dot):
-        if self.field.entity_type == "Model.System.Field":
-            self.toSQL_field(dot)
-        elif self.field.entity_type == "Model.System.Column":
-            self.toSQL_column(dot)
-        elif (
-            self.field.entity_type == "Model.System.RelationShip"
-        ):  # pragma: no cover
-            self.toSQL_relationship(dot)
+        if "remote_name" in self.field:
+            self.toSQL_relationship(dot)  # pragma: no cover
         else:
-            logger.warning("Unknown entity type %r" % self.field.entity_type)
-
-    def toSQL_field(self, dot):
-        # DO NOTHING
-        pass
+            self.toSQL_column(dot)
 
     def toSQL_relationship(self, dot):
         # TODO
         pass  # pragma: no cover
 
     def toSQL_column(self, dot):
-        table = dot.get_table(self.anyblok.get(self.field.model).__tablename__)
-        if self.field.foreign_key:  # pragma: no cover
+        Model = self.anyblok.get(self.model)
+        if self.field["id"] in Model.loaded_fields:
+            return
+
+        table = dot.get_table(self.anyblok.get(self.model).__tablename__)
+        if self.field.get("foreign_key"):  # pragma: no cover
             remote_table = dot.get_table(self.field.foreign_key.split(".")[0])
             if remote_table is None:
                 remote_table = dot.add_label(
                     self.field.foreign_key.split(".")[0]
                 )
 
             table.add_foreign_key(
                 remote_table,
                 label=self.field.name,
                 nullable=self.field.nullable,
             )
         else:
             table.add_column(
-                self.field.name,
-                self.field.ftype,
-                primary_key=self.field.primary_key,
+                self.field["id"],
+                self.field["type"],
+                primary_key=self.field["primary_key"],
             )
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/exceptions.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/__init__.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/blok.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/blok.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/cache.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/cache.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 #    Copyright (C) 2014 Jean-Sebastien SUZANNE <jssuzanne@anybox.fr>
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License,
 # v. 2.0. If a copy of the MPL was not distributed with this file,You can
 # obtain one at http://mozilla.org/MPL/2.0/.
 from sqlalchemy import func
 
-from anyblok.column import Integer, String
+from anyblok.column import Integer, ModelSelection, String
 from anyblok.declarations import Declarations
 
 from ..exceptions import CacheException
 
 register = Declarations.register
 System = Declarations.Model.System
 
 
 @register(System)
 class Cache:
     last_cache_id = None
 
     id = Integer(primary_key=True)
-    registry_name = String(nullable=False)
+    registry_name = ModelSelection(nullable=False)
     method = String(nullable=False)
 
     @classmethod
     def get_last_id(cls):
         """Return the last primary key ``id`` value"""
         res = cls.query("id").order_by(cls.id.desc()).limit(1).first()
         if res:
             return res[0]
 
-        return 0
+        return 0  # pragma: no cover
 
     @classmethod
     def initialize_model(cls):
         """Initialize the last_cache_id known"""
         super(Cache, cls).initialize_model()
         cls.last_cache_id = cls.get_last_id()
 
@@ -58,33 +58,30 @@
 
         :param registry_name: namespace of the model
         :param method: name of the method on the model
         :exception: CacheException
         """
         caches = cls.anyblok.caches
 
-        def insert(registry_name=None, method=None):
-            if registry_name in caches:
-                if method in caches[registry_name]:
-                    cls.last_cache_id = cls.insert(
-                        registry_name=registry_name, method=method
-                    ).id
-                    for cache in caches[registry_name][method]:
-                        cache.cache_clear()
-                else:
-                    raise CacheException(  # pragma: no cover
-                        "Unknown cached method %r" % method
-                    )
-            else:
-                raise CacheException("Unknown cached model %r" % registry_name)
+        if hasattr(registry_name, "__registry_name__"):
+            registry_name = registry_name.__registry_name__
 
-        if isinstance(registry_name, str):
-            insert(registry_name=registry_name, method=method)
-        elif hasattr(registry_name, "__registry_name__"):
-            insert(registry_name=registry_name.__registry_name__, method=method)
+        if registry_name in caches:
+            if method in caches[registry_name]:
+                cls.last_cache_id = cls.insert(
+                    registry_name=registry_name, method=method
+                ).id
+                for cache in caches[registry_name][method]:
+                    cache.cache_clear()
+            else:
+                raise CacheException(  # pragma: no cover
+                    "Unknown cached method %r" % method
+                )
+        else:
+            raise CacheException("Unknown cached model %r" % registry_name)
 
     @classmethod
     def get_invalidation(cls):
         """Return the pointer of the method to invalidate"""
         res = []
         query = cls.select_sql_statement(
             func.max(cls.id).label("id"),
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/column.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/column.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file is a part of the AnyBlok project
 #
 #    Copyright (C) 2014 Jean-Sebastien SUZANNE <jssuzanne@anybox.fr>
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License,
 # v. 2.0. If a copy of the MPL was not distributed with this file,You can
 # obtain one at http://mozilla.org/MPL/2.0/.
+# pragma: no cover
 from anyblok import Declarations
 from anyblok.column import Boolean, String
 from anyblok.common import anyblok_column_prefix
 
 register = Declarations.register
 System = Declarations.Model.System
 Mixin = Declarations.Mixin
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/field.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file is a part of the AnyBlok project
 #
 #    Copyright (C) 2014 Jean-Sebastien SUZANNE <jssuzanne@anybox.fr>
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License,
 # v. 2.0. If a copy of the MPL was not distributed with this file,You can
 # obtain one at http://mozilla.org/MPL/2.0/.
+# pragma: no cover
 from anyblok import Declarations
 from anyblok.column import String
 from anyblok.schema import ForeignKeyConstraint
 
 register = Declarations.register
 System = Declarations.Model.System
 Mixin = Declarations.Mixin
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/model.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 #    Copyright (C) 2014 Jean-Sebastien SUZANNE <jssuzanne@anybox.fr>
 #    Copyright (C) 2017 Jean-Sebastien SUZANNE <jssuzanne@anybox.fr>
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License,
 # v. 2.0. If a copy of the MPL was not distributed with this file,You can
 # obtain one at http://mozilla.org/MPL/2.0/.
+# pragma: no cover
 from logging import getLogger
 
 from anyblok.column import Boolean, String
 from anyblok.declarations import Declarations, listen
 from anyblok.field import Function
 
 logger = getLogger(__name__)
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/parameter.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/parameter.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/relationship.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/relationship.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file is a part of the AnyBlok project
 #
 #    Copyright (C) 2014 Jean-Sebastien SUZANNE <jssuzanne@anybox.fr>
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License,
 # v. 2.0. If a copy of the MPL was not distributed with this file,You can
 # obtain one at http://mozilla.org/MPL/2.0/.
+# pragma: no cover
 from anyblok import Declarations
 from anyblok.column import Boolean, String
 
 register = Declarations.register
 System = Declarations.Model.System
 Mixin = Declarations.Mixin
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/system/sequence.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/system/sequence.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_core_base.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/test_core_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,10 +27,10 @@
     def test_get_primary_keys(self, rollback_registry):
         registry = rollback_registry
         with pytest.raises(CoreBaseException):
             registry.System.get_primary_keys()
 
     def test_get_model(self, rollback_registry):
         registry = rollback_registry
-        m = registry.System.Model
-        m2 = registry.System.get_model("Model.System.Model")
-        assert m == m2
+        Blok = registry.System.Blok
+        Blok2 = registry.System.get_model("Model.System.Blok")
+        assert Blok == Blok2
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_core_sql_base.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/test_core_sql_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,155 +32,137 @@
             .all()
         )
         states = [x[0] for x in states]
         assert states == ["undefined", "undefined", "undefined"]
 
     def test_from_primary_key(self, rollback_registry):
         registry = rollback_registry
-        Model = registry.System.Model
-        model = Model.query().first()
-        model2 = Model.from_primary_keys(name=model.name)
-        assert model == model2
+        Blok = registry.System.Blok
+        blok = Blok.query().first()
+        blok2 = Blok.from_primary_keys(name=blok.name)
+        assert blok == blok2
 
     def test_from_primary_keys(self, rollback_registry):
         registry = rollback_registry
-        Column = registry.System.Column
-        column = Column.query().first()
-        column2 = Column.from_primary_keys(model=column.model, name=column.name)
-        assert column == column2
+        Cache = registry.System.Cache
+        cache = Cache.query().first()
+        cache2 = Cache.from_primary_keys(id=cache.id)
+        assert cache == cache2
 
     def test_get_primary_key(self, rollback_registry):
         registry = rollback_registry
-        assert registry.System.Model.get_primary_keys() == ["name"]
+        assert registry.System.Blok.get_primary_keys() == ["name"]
 
     def test_get_primary_keys(self, rollback_registry):
         registry = rollback_registry
-        pks = registry.System.Column.get_primary_keys()
-        model_in_pks = "model" in pks
-        name_in_pks = "name" in pks
-        assert model_in_pks is True
-        assert name_in_pks is True
+        pks = registry.System.Cache.get_primary_keys()
+        assert "id" in pks
 
     def test_to_primary_key(self, rollback_registry):
         registry = rollback_registry
-        model = registry.System.Model.query().first()
-        assert model.to_primary_keys() == dict(name=model.name)
+        blok = registry.System.Blok.query().first()
+        assert blok.to_primary_keys() == dict(name=blok.name)
 
     def test_to_primary_keys(self, rollback_registry):
         registry = rollback_registry
-        column = registry.System.Column.query().first()
-        assert column.to_primary_keys() == {
-            "model": column.model,
-            "name": column.name,
+        cache = registry.System.Cache.query().first()
+        assert cache.to_primary_keys() == {
+            "id": cache.id,
         }
 
     def test_fields_description(self, rollback_registry):
         registry = rollback_registry
-        Model = registry.System.Model
+        Cache = registry.System.Cache
+        selections = [
+            (k, v.__doc__ and v.__doc__.split("\n")[0] or k)
+            for k, v in registry.loaded_namespaces.items()
+        ]
         res = {
-            "description": {
-                "id": "description",
-                "label": "Description",
-                "model": None,
-                "nullable": True,
-                "primary_key": False,
-                "type": "Function",
-            },
-            "is_sql_model": {
-                "id": "is_sql_model",
-                "label": "Is a SQL model",
-                "model": None,
-                "nullable": True,
-                "primary_key": False,
-                "type": "Boolean",
-            },
-            "name": {
-                "id": "name",
-                "label": "Name",
+            "id": {
+                "id": "id",
+                "label": "Id",
                 "model": None,
                 "nullable": False,
                 "primary_key": True,
-                "type": "String",
+                "type": "Integer",
             },
-            "table": {
-                "id": "table",
-                "label": "Table",
+            "method": {
+                "id": "method",
+                "label": "Method",
                 "model": None,
-                "nullable": True,
+                "nullable": False,
                 "primary_key": False,
                 "type": "String",
             },
-            "schema": {
-                "id": "schema",
-                "label": "Schema",
+            "registry_name": {
+                "id": "registry_name",
+                "label": "Registry name",
                 "model": None,
-                "nullable": True,
+                "nullable": False,
                 "primary_key": False,
-                "type": "String",
+                "type": "ModelSelection",
+                "selections": selections,
             },
         }
-        assert Model.fields_description() == res
+        assert Cache.fields_description() == res
 
     def test_fields_description_limited_field(self, rollback_registry):
         registry = rollback_registry
-        Model = registry.System.Model
+        Blok = registry.System.Blok
         res = {
-            "table": {
-                "id": "table",
-                "label": "Table",
+            "installed_version": {
+                "id": "installed_version",
+                "label": "Installed version",
                 "model": None,
                 "nullable": True,
                 "primary_key": False,
                 "type": "String",
             }
         }
-        assert Model.fields_description(fields=["table"]) == res
+        assert Blok.fields_description(fields=["installed_version"]) == res
 
     def test_fields_description_cache(self, rollback_registry):
         registry = rollback_registry
-        Model = registry.System.Model
-        Column = registry.System.Column
+        Blok = registry.System.Blok
         res = {
-            "table": {
-                "id": "table",
-                "label": "Table",
+            "short_description": {
+                "id": "short_description",
+                "label": "Short description",
                 "model": None,
                 "nullable": True,
                 "primary_key": False,
-                "type": "String",
+                "type": "Function",
             }
         }
-        assert Model.fields_description(fields=["table"]) == res
-        column = Column.from_primary_keys(
-            model="Model.System.Model", name="table"
-        )
-        column.label = "Test"
-        assert Model.fields_description(fields=["table"]) == res
-        Model.fire("Update Model", "Model.System.Model")
-        assert Model.fields_description(fields=["table"]) != res
+        assert Blok.fields_description(fields=["short_description"]) == res
+        Blok.loaded_fields["short_description"] = "Test"
+        assert Blok.fields_description(fields=["short_description"]) == res
+        Blok.clear_all_model_caches()
+        assert Blok.fields_description(fields=["short_description"]) != res
 
     def test_to_dict(self, rollback_registry):
         registry = rollback_registry
-        M = registry.System.Model
-        model = M.query().first()
-        assert model.to_dict() == {
-            "name": model.name,
-            "table": model.table,
-            "schema": model.schema,
-            "is_sql_model": model.is_sql_model,
-            "description": model.description,
+        Cache = registry.System.Cache
+        cache = Cache.query().first()
+        assert cache.to_dict() == {
+            "id": cache.id,
+            "method": cache.method,
+            "registry_name": cache.registry_name,
         }
 
     def test_to_dict_on_some_columns(self, rollback_registry):
         registry = rollback_registry
-        M = registry.System.Model
-        model = M.query().first()
-        assert model.to_dict("name", "table") == {
-            "name": model.name,
-            "table": model.table,
+        Blok = registry.System.Blok
+        blok = Blok.query().first()
+        assert blok.to_dict(
+            "name", "installed_version", "short_description"
+        ) == {
+            "name": blok.name,
+            "installed_version": blok.installed_version,
+            "short_description": blok.short_description,
         }
 
     def test_select_sql_statement_with_column(self, rollback_registry):
         registry = rollback_registry
         Blok = registry.System.Blok
         assert Blok.execute_sql_statement(
             Blok.select_sql_statement("name")
@@ -201,20 +183,18 @@
     def test_from_multi_primary_keys_empty(self, rollback_registry):
         registry = rollback_registry
         Blok = registry.System.Blok
         assert Blok.from_multi_primary_keys() == []
 
     def test_get_hybrid_property_columns(self, rollback_registry):
         registry = rollback_registry
-        Column = registry.System.Column
-        columns = Column.get_hybrid_property_columns()
+        Blok = registry.System.Blok
+        columns = Blok.get_hybrid_property_columns()
         for x in [
             "name",
-            "model",
-            "autoincrement",
-            "foreign_key",
-            "primary_key",
-            "unique",
-            "nullable",
-            "remote_model",
+            "state",
+            "author",
+            "order",
+            "version",
+            "installed_version",
         ]:
             assert x in columns
```

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_documentation.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/test_documentation.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_system_blok.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/test_system_blok.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_system_params.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/test_system_params.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_system_sequence.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/test_system_sequence.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_core/tests/test_testing.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_core/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/anyblok_test/__init__.py` & `AnyBlok-2.1.0/anyblok/bloks/anyblok_test/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/model_authz/__init__.py` & `AnyBlok-2.1.0/anyblok/bloks/model_authz/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/model_authz/models.py` & `AnyBlok-2.1.0/anyblok/bloks/model_authz/models.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/bloks/model_authz/tests/test_shared_data_testcase.py` & `AnyBlok-2.1.0/anyblok/bloks/model_authz/tests/test_shared_data_testcase.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/column.py` & `AnyBlok-2.1.0/anyblok/column.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #    Copyright (C) 2020 Jean-Sebastien SUZANNE <js.suzanne@gmail.com>
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License,
 # v. 2.0. If a copy of the MPL was not distributed with this file,You can
 # obtain one at http://mozilla.org/MPL/2.0/.
 import decimal
 import time
+import warnings
 from base64 import b64decode, b64encode
 from datetime import date, datetime, timedelta
 from hashlib import md5
 from inspect import ismethod
 from json import dumps, loads
 from logging import getLogger
 
@@ -233,14 +234,27 @@
 
         :param registry: the current registry
         :param args:
         :param kwargs:
         :return:
         """
         if self.foreign_key:
+            if self.foreign_key.model_name in (
+                "Model.System.Model",
+                "Model.System.Field",
+                "Model.System.Column",
+                "Model.System.Relationship",
+            ):
+                warnings.warn(
+                    f"A foreign key to {self.foreign_key.model_name} "
+                    "is depecated becauses this Model will be removed",
+                    DeprecationWarning,
+                    stacklevel=2,
+                )
+
             CompareType.validate(
                 ModelAttribute(namespace, fieldname),
                 self,
                 self.foreign_key,
                 self.foreign_key.get_type(registry),
             )
             args = args + (self.foreign_key.get_fk(registry),)
@@ -633,14 +647,23 @@
         res["is auto updated"] = self.auto_update
         if self.default_timezone:
             res["default timezone"] = self.default_timezone
 
         return res
 
 
+class TimeStampType(DateTimeType):
+    impl = types.TIMESTAMP(timezone=True)
+    cache_ok = True
+
+    @property
+    def python_type(self):
+        return time  # pragma: no cover
+
+
 class TimeStamp(DateTime):
     """TimeStamp column
 
     ::
 
         from datetime import datetime
         from anyblok.declarations import Declarations
@@ -652,15 +675,15 @@
 
             x = TimeStamp(default=datetime.now)
 
     """
 
     def __init__(self, *args, **kwargs):
         super(TimeStamp, self).__init__(*args, **kwargs)
-        self.sqlalchemy_type = types.TIMESTAMP(timezone=True)
+        self.sqlalchemy_type = TimeStampType(self)
 
     def getter_format_value(self, value):
         value = convert_string_to_datetime(value)
         return add_timezone_on_datetime(value, self.default_timezone)
 
 
 class Time(Column):
@@ -1748,14 +1771,570 @@
         enum.sort()
         key = md5()
         key.update(str(enum).encode("utf-8"))
         name = self.fieldname + "_" + key.hexdigest() + "_types"
         return [CheckConstraint(constraint, name=name)]
 
 
+def model_validator_all(Model):
+    return True
+
+
+def model_validator_is_sql(Model):
+    return Model.is_sql is True
+
+
+def model_validator_is_not_sql(Model):
+    return not model_validator_is_sql(Model)
+
+
+def model_validator_is_view(Model):
+    return hasattr(Model, "__view__")
+
+
+def model_validator_is_not_view(Model):
+    return not model_validator_is_view(Model)
+
+
+def model_validator_in_namespace(namespace):
+    if hasattr(namespace, "__registry_name__"):
+        namespace = f"{namespace.__registry_name__}."
+
+    def validator(Model):
+        return Model.__registry_name__.startswith(namespace)
+
+    return validator
+
+
+def merge_validators(*validators):
+    def validator(obj):
+        return all(v(obj) for v in validators)
+
+    return validator
+
+
+class StrModelSelection(str):
+    """Class representing the data of one column ModelSelection"""
+
+    validator = None
+    registry = None
+    selections = None
+
+    def get_selections(self):
+        """Return a dict of selections
+
+        :return: selections dict
+        """
+        if not self.selections:
+            self.__class__.selections = {
+                k: v.__doc__ and v.__doc__.split("\n")[0] or k
+                for k, v in self.registry.loaded_namespaces.items()
+                if self.validator(v)
+            }
+
+        return self.selections
+
+    def validate(self):
+        """Validate if the key is in the selections
+
+        :return: True or False
+        """
+        a = super(StrModelSelection, self).__str__()
+        return a in self.get_selections().keys()
+
+    @property
+    def Model(self):
+        """Return the class corresponding to the selection key
+
+        :return:
+        """
+        a = super(StrModelSelection, self).__str__()
+        if a:
+            return self.registry.get(a)
+
+        return None  # pragma: no cover
+
+
+class ModelSelectionType(ScalarCoercible, types.TypeDecorator):
+    """Generic type for Column ModelSelection"""
+
+    impl = types.String
+    cache_ok = True
+
+    def __init__(self, validator, registry=None, namespace=None):
+        super(ModelSelectionType, self).__init__(length=256)
+
+        if validator is None:
+            validator = model_validator_all
+
+        def _validator(obj, Model):
+            if isinstance(validator, str):
+                return getattr(registry.get(namespace), validator)(Model)
+
+            return validator(Model)
+
+        self._StrModelSelection = type(
+            "StrModelSelection",
+            (StrModelSelection,),
+            {
+                "validator": _validator,
+                "registry": registry,
+                "selections": None,
+            },
+        )
+
+    @property
+    def python_type(self):
+        return self._StrModelSelection
+
+    def process_bind_param(self, value, engine):
+        if value is not None:
+            if hasattr(value, "__registry_name__"):
+                value = value.__registry_name__
+
+            value = self.python_type(value)
+
+        return value
+
+    def process_result_value(self, value, dialect):
+        return self._coerce(value)
+
+    def _coerce(self, value):
+        if value is not None and not isinstance(value, self._StrModelSelection):
+            value = self.python_type(value)
+
+        return value
+
+
+class ModelSelection(Column):
+    """ModelSelection column
+
+    Allow to Reference an AnyBlok Model
+    ::
+
+        from anyblok.declarations import Declarations
+        from anyblok.column import ModelSelection
+
+
+        @Declarations.register(Declarations.Model)
+        class Test:
+
+            x = ModelSelection(
+                default='Model.System.Blok',
+                validator="_x_validator"
+            )
+
+            @classmethod
+            def _x_validator(cls, Model):
+                return True or False
+
+    """
+
+    def __init__(self, *args, **kwargs):
+        self.validator = None
+        if "validator" in kwargs:
+            self.validator = kwargs.pop("validator")
+
+        self.sqlalchemy_type = "tmp value for assert"
+
+        super(ModelSelection, self).__init__(*args, **kwargs)
+        if self.default_val and hasattr(self.default_val, "__registry_name__"):
+            self.default_val = self.default_val.__registry_name__
+
+    def autodoc_get_properties(self):
+        """Return properties for autodoc
+
+        :return: autodoc properties
+        """
+        res = super(ModelSelection, self).autodoc_get_properties()
+        res["validator"] = str(self.validator)
+        return res
+
+    def getter_format_value(self, value):
+        """Return formatted value
+
+        :param value:
+        :return:
+        """
+        if value is None:
+            return None
+
+        return self.sqlalchemy_type.python_type(value)
+
+    def setter_format_value(self, value):
+        """Return value or raise exception if the given value is invalid
+
+        :param value:
+        :exception FieldException
+        :return:
+        """
+        if value is not None:
+            if hasattr(value, "__registry_name__"):
+                value = value.__registry_name__
+
+            val = self.sqlalchemy_type.python_type(value)
+            if not val.validate():
+                raise FieldException(
+                    "%r is not in the selections (%s)"
+                    % (value, ", ".join(val.get_selections()))
+                )
+
+        return value
+
+    def get_sqlalchemy_mapping(
+        self, registry, namespace, fieldname, properties
+    ):
+        """Return sqlalchmy mapping
+
+        :param registry: the current registry
+        :param namespace: the namespace of the model
+        :param fieldname: the fieldname of the model
+        :param properties: the properties of the model
+        :return: instance of the real field
+        """
+        self.sqlalchemy_type = ModelSelectionType(
+            self.validator, registry=registry, namespace=namespace
+        )
+        return super(ModelSelection, self).get_sqlalchemy_mapping(
+            registry, namespace, fieldname, properties
+        )
+
+    def get_encrypt_key_type(self, registry, sqlalchemy_type, encrypt_key):
+        sqlalchemy_type = StringEncryptedType(sqlalchemy_type, encrypt_key)
+        if sgdb_in(registry.engine, ["MySQL", "MariaDB"]):
+            sqlalchemy_type.impl = types.String(265)
+
+        return sqlalchemy_type
+
+    def update_description(self, registry, model, res):
+        """Update model description
+
+        :param registry: the current registry
+        :param model:
+        :param res:
+        """
+        super(ModelSelection, self).update_description(registry, model, res)
+        sqlalchemy_type = ModelSelectionType(
+            self.validator, registry=registry, namespace=model
+        )
+        values = sqlalchemy_type._StrModelSelection().get_selections()
+        res["selections"] = [(k, v) for k, v in values.items()]
+
+
+def fieldToModelAttribute(field):
+    if hasattr(field, "anyblok_field_name"):
+        field = ModelAttribute(
+            field.anyblok_registry_name,
+            field.anyblok_field_name,
+        )
+
+    return field
+
+
+def field_validator_all(field):
+    return True
+
+
+def field_validator_is_field(field):
+    return field_validator_is_not_column(
+        field
+    ) and field_validator_is_not_relationship(field)
+
+
+def field_validator_is_not_field(field):
+    return not field_validator_is_field(field)
+
+
+def field_validator_is_column(field):
+    return isinstance(
+        fieldToModelAttribute(field).get_type(field.from_model().anyblok),
+        Column,
+    )
+
+
+def field_validator_is_not_column(field):
+    return not field_validator_is_column(field)
+
+
+def field_validator_is_relationship(field):
+    from .relationship import RelationShip
+
+    return isinstance(
+        fieldToModelAttribute(field).get_type(field.from_model().anyblok),
+        RelationShip,
+    )
+
+
+def field_validator_is_not_relationship(field):
+    return not field_validator_is_relationship(field)
+
+
+def field_validator_is_named(*names):
+    def validator(field):
+        return field.anyblok_field_name in names
+
+    return validator
+
+
+def field_validator_is_from_types(*types):
+    def validator(field):
+        return isinstance(
+            fieldToModelAttribute(field).get_type(field.from_model().anyblok),
+            types,
+        )
+
+    return validator
+
+
+class StrModelFieldSelection(str):
+    """Class representing the data of one column ModelFieldSelection"""
+
+    model_validator = None
+    field_validator = None
+    registry = None
+    selections = None
+
+    def get_selections(self):
+        """Return a dict of selections
+
+        :return: selections dict
+        """
+        if not self.selections:
+            self.__class__.selections = {
+                str(ModelAttribute(namespace, field)): (
+                    Model.__doc__ and Model.__doc__.split("\n")[0] or namespace
+                )
+                + " : "
+                + field
+                for namespace, Model in self.registry.loaded_namespaces.items()
+                if self.model_validator(Model)
+                for field in Model.fields_name()
+                if self.field_validator(getattr(Model, field))
+            }
+
+        return self.selections
+
+    def validate(self):
+        """Validate if the key is in the selections
+
+        :return: True or False
+        """
+        a = super(StrModelFieldSelection, self).__str__()
+        return a in self.get_selections().keys()
+
+    @property
+    def field(self):
+        """Return the class corresponding to the selection key
+
+        :return:
+        """
+        a = super(StrModelFieldSelection, self).__str__()
+        if a:
+            return ModelAttributeAdapter(a).get_attribute(self.registry)
+
+        return None  # pragma: no cover
+
+
+class ModelFieldSelectionType(ScalarCoercible, types.TypeDecorator):
+    """Generic type for Column ModelFieldSelection"""
+
+    impl = types.String
+    cache_ok = True
+
+    def __init__(
+        self, model_validator, field_validator, registry=None, namespace=None
+    ):
+        super(ModelFieldSelectionType, self).__init__(length=256)
+
+        if model_validator is None:
+            model_validator = model_validator_is_sql
+
+        if field_validator is None:
+            field_validator = field_validator_all
+
+        def _model_validator(obj, Model):
+            if isinstance(model_validator, str):
+                return getattr(registry.get(namespace), model_validator)(Model)
+
+            return model_validator(Model)
+
+        def _field_validator(obj, field):
+            if isinstance(field_validator, str):
+                return getattr(registry.get(namespace), field_validator)(field)
+
+            return field_validator(field)
+
+        self._StrModelFieldSelection = type(
+            "StrModelFieldSelection",
+            (StrModelFieldSelection,),
+            {
+                "model_validator": _model_validator,
+                "field_validator": _field_validator,
+                "registry": registry,
+                "selections": None,
+            },
+        )
+
+    @property
+    def python_type(self):
+        return self._StrModelFieldSelection
+
+    def process_bind_param(self, value, engine):
+        if value is not None:
+            value = self.python_type(fieldToModelAttribute(value))
+
+        return value
+
+    def process_result_value(self, value, dialect):
+        return self._coerce(value)
+
+    def _coerce(self, value):
+        if value is not None and not isinstance(
+            value, self._StrModelFieldSelection
+        ):
+            value = self.python_type(value)
+
+        return value
+
+
+class ModelFieldSelection(Column):
+    """ModelFieldSelection column
+
+    Allow to Reference an AnyBlok Model
+    ::
+
+        from anyblok.declarations import Declarations
+        from anyblok.column import ModelFieldSelection
+
+
+        @Declarations.register(Declarations.Model)
+        class Test:
+
+            x = ModelFieldSelection(
+                default='Model.System.Blok => name',
+                model_validator="_x_model_validator",
+                field_validator="_x_field_validator",
+            )
+
+            @classmethod
+            def _x_model_validator(cls, Model):
+                return True or False
+
+            @classmethod
+            def _x_field_validator(cls, field):
+                return True or False
+    """
+
+    def __init__(self, *args, **kwargs):
+        self.model_validator = None
+        if "model_validator" in kwargs:
+            self.model_validator = kwargs.pop("model_validator")
+
+        self.field_validator = None
+        if "field_validator" in kwargs:
+            self.field_validator = kwargs.pop("field_validator")
+
+        self.sqlalchemy_type = "tmp value for assert"
+
+        super(ModelFieldSelection, self).__init__(*args, **kwargs)
+
+    def autodoc_get_properties(self):
+        """Return properties for autodoc
+
+        :return: autodoc properties
+        """
+        res = super(ModelFieldSelection, self).autodoc_get_properties()
+        res["model_validator"] = str(self.model_validator)
+        res["field_validator"] = str(self.field_validator)
+        return res
+
+    def getter_format_value(self, value):
+        """Return formatted value
+
+        :param value:
+        :return:
+        """
+        if value is None:
+            return None
+
+        return self.sqlalchemy_type.python_type(value)
+
+    def setter_format_value(self, value):
+        """Return value or raise exception if the given value is invalid
+
+        :param value:
+        :exception FieldException
+        :return:
+        """
+        if value is not None:
+            if hasattr(value, "anyblok_field_name"):
+                value = str(
+                    ModelAttribute(
+                        value.anyblok_registry_name,
+                        value.anyblok_field_name,
+                    )
+                )
+
+            val = self.sqlalchemy_type.python_type(value)
+            if not val.validate():
+                raise FieldException(
+                    "%r is not in the selections (%s)"
+                    % (value, ", ".join(val.get_selections()))
+                )
+
+        return value
+
+    def get_sqlalchemy_mapping(
+        self, registry, namespace, fieldname, properties
+    ):
+        """Return sqlalchmy mapping
+
+        :param registry: the current registry
+        :param namespace: the namespace of the model
+        :param fieldname: the fieldname of the model
+        :param properties: the properties of the model
+        :return: instance of the real field
+        """
+        self.sqlalchemy_type = ModelFieldSelectionType(
+            self.model_validator,
+            self.field_validator,
+            registry=registry,
+            namespace=namespace,
+        )
+        return super(ModelFieldSelection, self).get_sqlalchemy_mapping(
+            registry, namespace, fieldname, properties
+        )
+
+    def get_encrypt_key_type(self, registry, sqlalchemy_type, encrypt_key):
+        sqlalchemy_type = StringEncryptedType(sqlalchemy_type, encrypt_key)
+        if sgdb_in(registry.engine, ["MySQL", "MariaDB"]):
+            sqlalchemy_type.impl = types.String(265)
+
+        return sqlalchemy_type
+
+    def update_description(self, registry, model, res):
+        """Update model description
+
+        :param registry: the current registry
+        :param model:
+        :param res:
+        """
+        super(ModelFieldSelection, self).update_description(
+            registry, model, res
+        )
+        sqlalchemy_type = ModelFieldSelectionType(
+            self.model_validator,
+            self.field_validator,
+            registry=registry,
+            namespace=model,
+        )
+        values = sqlalchemy_type._StrModelFieldSelection().get_selections()
+        res["selections"] = [(k, v) for k, v in values.items()]
+
+
 @CompareType.add_comparator(String, String)
 @CompareType.add_comparator(String, Selection)
 @CompareType.add_comparator(String, Sequence)
 def compare_strings(col1, type1, col2, type2):
     if type1.size != type2.size:
         raise FieldException(
             "You can't add a foreign key using based String columns with "
```

### Comparing `AnyBlok-2.0.0/anyblok/common.py` & `AnyBlok-2.1.0/anyblok/common.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/config.py` & `AnyBlok-2.1.0/anyblok/config.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/conftest.py` & `AnyBlok-2.1.0/anyblok/conftest.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/core.py` & `AnyBlok-2.1.0/anyblok/core.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/declarations.py` & `AnyBlok-2.1.0/anyblok/declarations.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/environment.py` & `AnyBlok-2.1.0/anyblok/environment.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/event.py` & `AnyBlok-2.1.0/anyblok/event.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/field.py` & `AnyBlok-2.1.0/anyblok/field.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/imp.py` & `AnyBlok-2.1.0/anyblok/imp.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/logging.py` & `AnyBlok-2.1.0/anyblok/logging.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/mapper.py` & `AnyBlok-2.1.0/anyblok/mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,15 +438,15 @@
     if isinstance(Model, str):
         if "=>" not in Model:
             raise ModelAttributeAdapterException(
                 "Wrong value %r impossible to find model and attribtue"
                 % (Model)
             )
         model, attribute = Model.split("=>")
-        return ModelAttribute(model, attribute)
+        return ModelAttribute(model.strip(), attribute.strip())
     else:
         return Model
 
 
 def ModelAdapter(Model):
     """Return a ModelRepr
```

### Comparing `AnyBlok-2.0.0/anyblok/migration.py` & `AnyBlok-2.1.0/anyblok/migration.py`

 * *Files 1% similar despite different names*

```diff
@@ -911,39 +911,28 @@
         if column.default:
             execute = self.table.migration.conn.execute
             val = column.default.arg
             table = self.table.migration.metadata.tables[self.table.name]
             table.append_column(column)
             cname = getattr(table.c, column.name)
             if column.default.is_callable:
-                Table = self.table.migration.metadata.tables["system_model"]
-                Column = self.table.migration.metadata.tables["system_column"]
-                query_pks = select(Column.c.name)
-                query_pks = query_pks.join(
-                    Table, Column.c.model == Table.c.name
-                )
-                query_pks = query_pks.where(Table.c.table == self.table.name)
-                query_pks = query_pks.where(Column.c.primary_key.is_(True))
-                columns = [x[0] for x in execute(query_pks).fetchall()]
-
+                columns = [col for col in table.columns if col.primary_key]
                 query_count = select(func.count()).select_from(table)
                 query_count = query_count.where(cname.is_(None))
                 nb_row = self.table.migration.conn.execute(
                     query_count
                 ).fetchone()[0]
                 for offset in range(nb_row):
-                    query = select(
-                        *[getattr(table.c, x).label(x) for x in columns]
-                    )
+                    query = select(*columns)
                     query = query.where(cname.is_(None))
                     query = query.limit(1)
                     res = execute(query).fetchone()
                     where = []
                     for index, col in enumerate(columns):
-                        where.append(getattr(table.c, col) == res[index])
+                        where.append(col == res[index])
 
                     if len(where) == 1:
                         where = where[0]
                     else:
                         where = and_(*where)
 
                     query_update = update(table)
```

### Comparing `AnyBlok-2.0.0/anyblok/mixin.py` & `AnyBlok-2.1.0/anyblok/mixin.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/model/__init__.py` & `AnyBlok-2.1.0/anyblok/model/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,25 @@
             properties[name] = field.get_property(
                 registry, namespace, name, properties
             )
             properties[name].sqla_column = properties[attr_name]
 
             properties["hybrid_property_columns"].append(name)
 
+        def field_description():
+            return registry.get(namespace).fields_description(name)[name]
+
+        def from_model():
+            return registry.get(namespace)
+
+        properties[name].anyblok_field_name = name
+        properties[name].anyblok_registry_name = namespace
+        properties[name].field_description = field_description
+        properties[name].from_model = from_model
+
         registry.call_plugins(
             "declare_field",
             name,
             field,
             namespace,
             properties,
             transformation_properties,
@@ -653,14 +664,19 @@
         * Column
         * RelationShip
 
         :param registry: registry to update
         """
         for Model in registry.loaded_namespaces.values():
             Model.initialize_model()
+            if not registry.loadwithoutmigration:
+                Model.clear_all_model_caches()
+
+        if registry.loadwithoutmigration:
+            return False
 
         Blok = registry.System.Blok
         if not registry.withoutautomigration:
             Model = registry.System.Model
             Model.update_list()
             registry.update_blok_list()
```

### Comparing `AnyBlok-2.0.0/anyblok/model/cache.py` & `AnyBlok-2.1.0/anyblok/model/cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,36 @@
 class CachePlugin(ModelPluginBase):
     def __init__(self, registry):
         if not hasattr(registry, "caches"):
             registry.caches = {}
 
         super(CachePlugin, self).__init__(registry)
 
+    def insert_in_bases(
+        self, new_base, namespace, properties, transformation_properties
+    ):
+        """Create overload to define the cache from __depends__.
+
+        Because the cache is defined on the depend models and this namespace
+        does not exist in caches dict
+
+        :param new_base: the base to be put on front of all bases
+        :param namespace: the namespace of the model
+        :param properties: the properties declared in the model
+        :param transformation_properties: the properties of the model
+        """
+        for dep in properties["__depends__"]:
+            if dep in self.registry.caches:
+                cache = self.registry.caches.setdefault(namespace, {})
+                for method_name, methods in self.registry.caches[dep].items():
+                    entry = cache.setdefault(method_name, [])
+                    entry.extend(methods)
+
+        return {}
+
     def transform_base_attribute(
         self,
         attr,
         method,
         namespace,
         base,
         transformation_properties,
```

### Comparing `AnyBlok-2.0.0/anyblok/model/event.py` & `AnyBlok-2.1.0/anyblok/model/event.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/model/exceptions.py` & `AnyBlok-2.1.0/anyblok/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/model/factory.py` & `AnyBlok-2.1.0/anyblok/model/factory.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/model/field_datetime.py` & `AnyBlok-2.1.0/anyblok/model/field_datetime.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/model/hybrid_method.py` & `AnyBlok-2.1.0/anyblok/model/hybrid_method.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/model/plugins.py` & `AnyBlok-2.1.0/anyblok/model/plugins.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/model/table_and_mapper.py` & `AnyBlok-2.1.0/anyblok/model/table_and_mapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,45 @@
 # This file is a part of the AnyBlok project
 #
 #    Copyright (C) 2017 Jean-Sebastien SUZANNE <jssuzanne@anybox.fr>
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License,
 # v. 2.0. If a copy of the MPL was not distributed with this file,You can
 # obtain one at http://mozilla.org/MPL/2.0/.
+import warnings
+
 from sqlalchemy import CheckConstraint, ForeignKeyConstraint
 from sqlalchemy.exc import NoInspectionAvailable
 from sqlalchemy.ext.declarative import declared_attr
 
 from ..common import sgdb_in
 from .exceptions import ModelException
 from .plugins import ModelPluginBase
 
 
+def check_deprecated_foreign_keys(res):
+    for entry in res:
+        if isinstance(entry, ForeignKeyConstraint):
+            table = entry.elements[0].target_fullname.split(".")[0]
+            if table in (
+                "system_model",
+                "system_field",
+                "system_column",
+                "system_relationship",
+            ):
+                warnings.warn(
+                    f"A foreign key to {table} is depecated becauses this "
+                    "Model will be removed",
+                    DeprecationWarning,
+                    stacklevel=2,
+                )
+
+    return res
+
+
 class TableMapperPlugin(ModelPluginBase):
     def initialisation_tranformation_properties(
         self, properties, transformation_properties
     ):
         """Initialise the transform properties: hybrid_method
 
         :param new_type_properties: param to add in a new base if need
@@ -161,27 +183,27 @@
                 except NoInspectionAvailable:  # pragma: no cover
                     raise ModelException(
                         "A Index  or constraint on the model "
                         f'"{cls_.__registry_name__}" if defined with SQLAlchemy'
                         "class use the anyblok Index or constraint"
                     )
 
-                return res
+                return check_deprecated_foreign_keys(res)
 
             new_base.__table_args__ = declared_attr(__table_args__)
         elif transformation_properties["table_args"]:
 
             def __table_args__(cls_):
-                return cls_.define_table_args()
+                return check_deprecated_foreign_keys(cls_.define_table_args())
 
             new_base.__table_args__ = declared_attr(__table_args__)
         elif transformation_properties["table_kwargs"]:  # pragma: no cover
 
             def __table_args__(cls_):
-                return cls_.define_table_kwargs()
+                return check_deprecated_foreign_keys(cls_.define_table_kwargs())
 
             new_base.__table_args__ = declared_attr(__table_args__)
 
     def insert_in_bases_mapper_args(self, new_base, transformation_properties):
         """Add table __mapper_args__ in new_base
 
         :param new_base: the base to be put on front of all bases
```

### Comparing `AnyBlok-2.0.0/anyblok/plugins.py` & `AnyBlok-2.1.0/anyblok/plugins.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/registry.py` & `AnyBlok-2.1.0/anyblok/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # v. 2.0. If a copy of the MPL was not distributed with this file,You can
 # obtain one at http://mozilla.org/MPL/2.0/.
 from logging import getLogger
 
 from pkg_resources import iter_entry_points
 from sqlalchemy import MetaData, create_engine, event, text
 from sqlalchemy.exc import (
+    InternalError,
     InvalidRequestError,
     OperationalError,
     ProgrammingError,
 )
 from sqlalchemy.orm import declarative_base, scoped_session, sessionmaker
 from sqlalchemy.orm.attributes import flag_modified
 from sqlalchemy.orm.session import close_all_sessions
@@ -609,15 +610,20 @@
 
         res = []
         query = """SELECT "order", name"""
         query += " FROM system_blok"
         query += f" WHERE {where}"
         try:
             res = self.execute(text(query).bindparams(**params), fetchall=True)
-        except (ProgrammingError, OperationalError, PyODBCProgrammingError):
+        except (
+            ProgrammingError,
+            OperationalError,
+            PyODBCProgrammingError,
+            InternalError,
+        ):
             # During the first connection the database is empty
             pass
 
         if res:
             res.sort()
             return [x[1] for x in res]
 
@@ -855,25 +861,32 @@
     def update_to_install_blok_dependencies_state(self, toinstall):
         dependencies_to_install = []
 
         for blok in toinstall:
             self.check_dependencies(blok, dependencies_to_install, toinstall)
 
         if dependencies_to_install:
-            query = """
+            params = {}
+            where = []
+            for i, dep in enumerate(dependencies_to_install):
+                key = f"blok_{i}"
+                params[key] = dep
+                where.append(f"name = :{key}")
+
+            if len(where) == 1:
+                where = where[0]
+            else:
+                where = " OR ".join(where)
+
+            query = f"""
                 update system_blok
                 set state='toinstall'
-                where name in :bloks_name
-                and state = 'uninstalled'"""
+                where ({where}) and state = 'uninstalled'"""
             try:
-                self.execute(
-                    text(query).bindparams(
-                        bloks_name=tuple(dependencies_to_install),
-                    )
-                )
+                self.execute(text(query).bindparams(**params))
             except (ProgrammingError, OperationalError):  # pragma: no cover
                 pass
 
             return True
 
         return False
 
@@ -1110,17 +1123,14 @@
 
         else:
             self.migration.auto_upgrade_database()
 
     def is_reload_needed(self):
         """Determines whether a reload is needed or not."""
 
-        if self.loadwithoutmigration:
-            return
-
         mustreload = False
         for entry in RegistryManager.declared_entries:
             if entry in RegistryManager.callback_initialize_entries:
                 logger.debug("Initialize %r entry" % entry)
                 r = RegistryManager.callback_initialize_entries[entry](self)
                 mustreload = mustreload or r
```

### Comparing `AnyBlok-2.0.0/anyblok/relationship.py` & `AnyBlok-2.1.0/anyblok/relationship.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 #    Copyright (C) 2014 Jean-Sebastien SUZANNE <jssuzanne@anybox.fr>
 #    Copyright (C) 2015 Pierre Verkest <pverkest@anybox.fr>
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License,
 # v. 2.0. If a copy of the MPL was not distributed with this file,You can
 # obtain one at http://mozilla.org/MPL/2.0/.
+import warnings
 from logging import getLogger
 from types import FunctionType
 from typing import Any, Dict
 
 from sqlalchemy import Column, ForeignKeyConstraint, Table
 from sqlalchemy import exc as sa_exc
 from sqlalchemy.ext.declarative import declared_attr
@@ -30,14 +31,16 @@
 from .field import Field, FieldException
 from .mapper import ModelAdapter, ModelAttribute, ModelRepr, format_schema
 
 logger = getLogger(__name__)
 
 
 class RelationshipProperty(relationships.RelationshipProperty):
+    inherit_cache = True
+
     def __init__(self, *args, **kwargs):
         self.relationship_field = kwargs.pop("relationship_field")
         super(RelationshipProperty, self).__init__(*args, **kwargs)
 
     def _generate_backref(self) -> None:
         """Interpret the 'backref' instruction to create a
         :func:`_orm.relationship` complementary to this one."""
@@ -139,14 +142,16 @@
     )
     descriptor.__doc__ = doc
     manager.instrument_attribute(key, descriptor)
     return descriptor
 
 
 class RelationshipProperty2(relationships.RelationshipProperty):
+    inherit_cache = True
+
     def __init__(self, *args, **kwargs):
         self.relationship_field = kwargs.pop("relationship_field")
         super(RelationshipProperty2, self).__init__(*args, **kwargs)
 
     def instrument_class(self, mapper):
         register_descriptor(
             mapper.class_,
@@ -210,14 +215,27 @@
     def __init__(self, *args, **kwargs):
         self.forbid_instance(RelationShip)
         if "model" in kwargs:
             self.model = ModelAdapter(kwargs.pop("model"))
         else:
             raise FieldException("model is required attribut")
 
+        if self.model.model_name in (
+            "Model.System.Model",
+            "Model.System.Field",
+            "Model.System.Column",
+            "Model.System.Relationship",
+        ):
+            warnings.warn(
+                f"A foreign key to {self.model.model_name} "
+                "is depecated becauses this Model will be removed",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+
         super(RelationShip, self).__init__(*args, **kwargs)
 
         if "info" not in self.kwargs:
             self.kwargs["info"] = {}
 
         self.kwargs["info"]["remote_model"] = self.model.model_name
         self.backref_properties = {}
```

### Comparing `AnyBlok-2.0.0/anyblok/release.py` & `AnyBlok-2.1.0/anyblok/release.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #    Copyright (C) 2020 Jean-Sebastien SUZANNE <js.suzanne@gmail.com>
 #    Copyright (C) 2021 Jean-Sebastien SUZANNE <js.suzanne@gmail.com>
 #    Copyright (C) 2022 Jean-Sebastien SUZANNE <js.suzanne@gmail.com>
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License,
 # v. 2.0. If a copy of the MPL was not distributed with this file,You can
 # obtain one at http://mozilla.org/MPL/2.0/.
-version = "2.0.0"
+version = "2.1.0"
```

### Comparing `AnyBlok-2.0.0/anyblok/schema.py` & `AnyBlok-2.1.0/anyblok/schema.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/scripts.py` & `AnyBlok-2.1.0/anyblok/scripts.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/sphinx/ext/load/blok.py` & `AnyBlok-2.1.0/anyblok/sphinx/ext/load/blok.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/test_bloks/test_blok1/__init__.py` & `AnyBlok-2.1.0/anyblok/test_bloks/test_blok1/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/test_bloks/test_blok1/test.py` & `AnyBlok-2.1.0/anyblok/test_bloks/test_blok1/test.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/test_bloks/test_blok10/__init__.py` & `AnyBlok-2.1.0/anyblok/test_bloks/test_blok10/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/test_bloks/test_blok10/declarations.py` & `AnyBlok-2.1.0/anyblok/test_bloks/test_blok10/declarations.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/test_bloks/test_blok11/__init__.py` & `AnyBlok-2.1.0/anyblok/test_bloks/test_blok11/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/test_bloks/test_blok14/__init__.py` & `AnyBlok-2.1.0/anyblok/test_bloks/test_blok14/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/test_bloks/test_blok14/test.py` & `AnyBlok-2.1.0/anyblok/test_bloks/test_blok14/test.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/test_bloks/test_blok16/README.rst` & `AnyBlok-2.1.0/anyblok/test_bloks/test_blok16/README.rst`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/test_bloks/test_blok16/__init__.py` & `AnyBlok-2.1.0/anyblok/test_bloks/test_blok16/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/test_bloks/test_blok7/__init__.py` & `AnyBlok-2.1.0/anyblok/test_bloks/test_blok7/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/test_bloks/test_blok7/declarations.py` & `AnyBlok-2.1.0/anyblok/test_bloks/test_blok7/declarations.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/test_bloks/test_blok8/__init__.py` & `AnyBlok-2.1.0/anyblok/test_bloks/test_blok8/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/test_bloks/test_blok8/declarations.py` & `AnyBlok-2.1.0/anyblok/test_bloks/test_blok8/declarations.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/test_bloks/test_blok9/__init__.py` & `AnyBlok-2.1.0/anyblok/test_bloks/test_blok9/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/test_bloks/test_blok9/declarations.py` & `AnyBlok-2.1.0/anyblok/test_bloks/test_blok9/declarations.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/testing.py` & `AnyBlok-2.1.0/anyblok/testing.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/__init__.py` & `AnyBlok-2.1.0/anyblok/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/conftest.py` & `AnyBlok-2.1.0/anyblok/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/mockblok/__init__.py` & `AnyBlok-2.1.0/anyblok/tests/mockblok/__init__.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_authorization.py` & `AnyBlok-2.1.0/anyblok/tests/test_authorization.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_blok.py` & `AnyBlok-2.1.0/anyblok/tests/test_blok.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_blok_manager.py` & `AnyBlok-2.1.0/anyblok/tests/test_blok_manager.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_cache.py` & `AnyBlok-2.1.0/anyblok/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_column.py` & `AnyBlok-2.1.0/anyblok/tests/test_column.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,28 +39,48 @@
     Email,
     Enum,
     Float,
     Integer,
     Interval,
     Json,
     LargeBinary,
+    ModelFieldSelection,
+    ModelSelection,
     Password,
     PhoneNumber,
     Selection,
     Sequence,
     String,
     Text,
     Time,
     TimeStamp,
     add_timezone_on_datetime,
     convert_string_to_datetime,
+    field_validator_all,
+    field_validator_is_column,
+    field_validator_is_field,
+    field_validator_is_from_types,
+    field_validator_is_named,
+    field_validator_is_not_column,
+    field_validator_is_not_field,
+    field_validator_is_not_relationship,
+    field_validator_is_relationship,
+    fieldToModelAttribute,
+    merge_validators,
+    model_validator_all,
+    model_validator_in_namespace,
+    model_validator_is_not_sql,
+    model_validator_is_not_view,
+    model_validator_is_sql,
+    model_validator_is_view,
 )
 from anyblok.config import Configuration
 from anyblok.field import FieldException
 from anyblok.mapper import ModelAttribute
+from anyblok.relationship import Many2One
 from anyblok.testing import sgdb_in, tmp_configuration
 
 from .conftest import init_registry, reset_db
 
 time_params = [DateTime]
 
 if not sgdb_in(["MsSQL"]):
@@ -152,14 +172,22 @@
         (Decimal, D("1"), {}),
         id="Decimal",
     ),
     pytest.param(
         (Json, {"name": "test"}, {}),
         id="Json",
     ),
+    pytest.param(
+        (ModelSelection, "Model.System.Blok", {}),
+        id="ModelSelection",
+    ),
+    pytest.param(
+        (ModelFieldSelection, "Model.System.Blok => name", {}),
+        id="ModelFieldSelection",
+    ),
 ]
 
 if not sgdb_in(["MySQL", "MariaDB"]):
     COLUMNS.append(pytest.param((UUID, uuid1(), {}), id="UUID"))
 
 if not sgdb_in(["MsSQL"]):
     COLUMNS.append(
@@ -529,238 +557,14 @@
             Test.update_sql_statement()
             .where(Test.id == test.id)
             .values(col=False)
         )
         self.registry.expire(test, ["col"])
         assert test.col == ""
 
-    def test_datetime_none_value(self, dt_column_type):
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        test = registry.Test.insert(col=None)
-        assert test.col is None
-
-    def test_datetime_str_conversion_1(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = datetime.datetime.now().replace(tzinfo=timezone)
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        test = registry.Test.insert(col=now.strftime("%Y-%m-%d %H:%M:%S.%f%z"))
-        assert test.col == now
-
-    def test_datetime_str_conversion_2(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = timezone.localize(datetime.datetime.now())
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        test = registry.Test.insert(col=now.strftime("%Y-%m-%d %H:%M:%S.%f%Z"))
-        assert test.col == now
-
-    def test_datetime_str_conversion_3(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = timezone.localize(datetime.datetime.now())
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        test = registry.Test.insert(col=now.strftime("%Y-%m-%d %H:%M:%S.%f"))
-        assert test.col == now
-
-    def test_datetime_str_conversion_4(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = timezone.localize(datetime.datetime.now())
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        test = registry.Test.insert(col=now.strftime("%Y-%m-%d %H:%M:%S"))
-        assert test.col == now.replace(microsecond=0)
-
-    def test_datetime_by_property(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = datetime.datetime.now().replace(tzinfo=timezone)
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        test = registry.Test.insert()
-        test.col = now
-        assert test.col == now
-
-    def test_datetime_by_property_none_value(self, dt_column_type):
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        test = registry.Test.insert()
-        test.col = None
-        assert test.col is None
-
-    def test_datetime_str_conversion_1_by_property(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = datetime.datetime.now().replace(tzinfo=timezone)
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        test = registry.Test.insert()
-        test.col = now.strftime("%Y-%m-%d %H:%M:%S.%f%z")
-        assert test.col == now
-
-    def test_datetime_str_conversion_2_by_property(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = timezone.localize(datetime.datetime.now())
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        test = registry.Test.insert()
-        test.col = now.strftime("%Y-%m-%d %H:%M:%S.%f%Z")
-        assert test.col == now
-
-    def test_datetime_str_conversion_3_by_property(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = timezone.localize(datetime.datetime.now())
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        test = registry.Test.insert()
-        test.col = now.strftime("%Y-%m-%d %H:%M:%S.%f")
-        assert test.col == now
-
-    def test_datetime_str_conversion_4_by_property(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = timezone.localize(datetime.datetime.now())
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        test = registry.Test.insert()
-        test.col = now.strftime("%Y-%m-%d %H:%M:%S")
-        assert test.col == now.replace(microsecond=0)
-
-    def test_datetime_by_query(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        d = datetime.datetime(2020, 7, 3, 18, 59, 0)
-        d = add_timezone_on_datetime(d, timezone)
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        Test = registry.Test
-        test = Test.insert()
-        Test.execute_sql_statement(Test.update_sql_statement().values(col=d))
-        registry.refresh(test)
-        assert test.col == d
-
-    def test_datetime_by_query_none_value(self, dt_column_type):
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        Test = registry.Test
-        test = Test.insert()
-        Test.execute_sql_statement(Test.update_sql_statement().values(col=None))
-        assert test.col is None
-
-    @pytest.mark.skipif(
-        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
-    )
-    def test_datetime_str_conversion_1_by_query(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = datetime.datetime.now().replace(tzinfo=timezone)
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        Test = registry.Test
-        test = Test.insert()
-        Test.execute_sql_statement(
-            Test.update_sql_statement().values(
-                col=now.strftime("%Y-%m-%d %H:%M:%S.%f%z")
-            )
-        )
-        registry.expire(test, ["col"])
-        assert test.col == now
-
-    @pytest.mark.skipif(
-        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
-    )
-    def test_datetime_str_conversion_2_by_query(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = timezone.localize(datetime.datetime.now())
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        Test = registry.Test
-        test = Test.insert()
-        Test.execute_sql_statement(
-            Test.update_sql_statement().values(
-                col=now.strftime("%Y-%m-%d %H:%M:%S.%f%Z")
-            )
-        )
-        registry.expire(test, ["col"])
-        assert test.col == now
-
-    @pytest.mark.skipif(
-        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
-    )
-    def test_datetime_str_conversion_3_by_query(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = timezone.localize(datetime.datetime.now())
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        Test = registry.Test
-        test = Test.insert()
-        Test.execute_sql_statement(
-            Test.update_sql_statement().values(
-                col=now.strftime("%Y-%m-%d %H:%M:%S.%f")
-            )
-        )
-        registry.expire(test, ["col"])
-        assert test.col == now
-
-    @pytest.mark.skipif(
-        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
-    )
-    def test_datetime_str_conversion_4_by_query(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = timezone.localize(datetime.datetime.now())
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        Test = registry.Test
-        test = Test.insert()
-        Test.execute_sql_statement(
-            Test.update_sql_statement().values(
-                col=now.strftime("%Y-%m-%d %H:%M:%S")
-            )
-        )
-        registry.expire(test, ["col"])
-        assert test.col == now.replace(microsecond=0)
-
-    @pytest.mark.skipif(
-        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
-    )
-    def test_datetime_by_query_filter(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = datetime.datetime.now().replace(tzinfo=timezone)
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        test = registry.Test.insert(col=now)
-        Test = registry.Test
-        assert Test.query().filter(Test.col == now).one() is test
-
-    @pytest.mark.skipif(
-        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
-    )
-    def test_datetime_str_conversion_1_by_query_filter(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = datetime.datetime.now().replace(tzinfo=timezone)
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        test = registry.Test.insert(col=now)
-        Test = registry.Test
-        assert (
-            Test.query()
-            .filter(Test.col == now.strftime("%Y-%m-%d %H:%M:%S.%f%z"))
-            .one()
-            is test
-        )
-
-    @pytest.mark.skipif(
-        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
-    )
-    def test_datetime_str_conversion_2_by_query_filter(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = timezone.localize(datetime.datetime.now())
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        test = registry.Test.insert(col=now)
-        Test = registry.Test
-        assert (
-            Test.query()
-            .filter(Test.col == now.strftime("%Y-%m-%d %H:%M:%S.%f%Z"))
-            .one()
-            is test
-        )
-
-    @pytest.mark.skipif(
-        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
-    )
-    def test_datetime_str_conversion_3_by_query_filter(self, dt_column_type):
-        timezone = pytz.timezone(time.tzname[0])
-        now = timezone.localize(datetime.datetime.now())
-        registry = self.init_registry(simple_column, ColumnType=dt_column_type)
-        test = registry.Test.insert(col=now)
-        Test = registry.Test
-        assert (
-            Test.query()
-            .filter(Test.col == now.strftime("%Y-%m-%d %H:%M:%S.%f"))
-            .one()
-            is test
-        )
-
     def test_datetime_without_auto_update_1(self, dt_column_type):
         def add_in_registry():
             from anyblok import Declarations
 
             @Declarations.register(Declarations.Model)
             class Test:
                 id = Integer(primary_key=True)
@@ -899,20 +703,16 @@
         SELECTIONS = [
             ("admin", "Admin"),
         ]
 
         registry = self.init_registry(
             simple_column, ColumnType=Selection, selections=SELECTIONS
         )
-        column = (
-            registry.System.Column.query()
-            .filter_by(model="Model.Test", name="col")
-            .one()
-        )
-        assert column._description() == {
+        description = registry.Test.fields_description("col")["col"]
+        assert description == {
             "id": "col",
             "label": "Col",
             "model": None,
             "nullable": True,
             "primary_key": False,
             "selections": [
                 ("admin", "Admin"),
@@ -1143,15 +943,15 @@
         assert Seq.query().filter(Seq.code == "SO").one()
 
     def test_sequence_with_foreign_key(self):
         with pytest.raises(FieldException):
             self.init_registry(
                 simple_column,
                 ColumnType=Sequence,
-                foreign_key=Model.System.Model.use("name"),
+                foreign_key=Model.System.Blok.use("name"),
             )
 
     def test_sequence_with_default(self):
         with pytest.raises(FieldException):
             self.init_registry(
                 simple_column, ColumnType=Sequence, default="default value"
             )
@@ -1520,14 +1320,617 @@
             self.init_registry(simple_column, ColumnType=cls, primary_key=True)
 
         assert (
             f"{cls} column `Model.Test.col` are not " f"allowed as primary key"
         ) == str(ex.value), "Column name should be part of raised message"
 
 
+@pytest.fixture(params=time_params, scope="class")
+def registry_dt(request):
+    reset_db()
+    registry = init_registry(simple_column, ColumnType=request.param)
+    request.addfinalizer(registry.close)
+    return registry
+
+
+@pytest.mark.relationship
+class TestColumnDT:
+    @pytest.fixture(autouse=True)
+    def transact(self, request, registry_dt):
+        transaction = registry_dt.begin_nested()
+        request.addfinalizer(transaction.rollback)
+        return
+
+    def test_none_value(self, registry_dt):
+        test = registry_dt.Test.insert(col=None)
+        assert test.col is None
+
+    def test_str_conversion_1(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = datetime.datetime.now().replace(tzinfo=timezone)
+        test = registry_dt.Test.insert(
+            col=now.strftime("%Y-%m-%d %H:%M:%S.%f%z")
+        )
+        assert test.col == now
+
+    def test_str_conversion_2(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = timezone.localize(datetime.datetime.now())
+        test = registry_dt.Test.insert(
+            col=now.strftime("%Y-%m-%d %H:%M:%S.%f%Z")
+        )
+        assert test.col == now
+
+    def test_str_conversion_3(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = timezone.localize(datetime.datetime.now())
+        test = registry_dt.Test.insert(col=now.strftime("%Y-%m-%d %H:%M:%S.%f"))
+        assert test.col == now
+
+    def test_str_conversion_4(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = timezone.localize(datetime.datetime.now())
+        test = registry_dt.Test.insert(col=now.strftime("%Y-%m-%d %H:%M:%S"))
+        assert test.col == now.replace(microsecond=0)
+
+    def test_by_property(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = datetime.datetime.now().replace(tzinfo=timezone)
+        test = registry_dt.Test.insert()
+        test.col = now
+        assert test.col == now
+
+    def test_by_property_none_value(self, registry_dt):
+        test = registry_dt.Test.insert()
+        test.col = None
+        assert test.col is None
+
+    def test_str_conversion_1_by_property(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = datetime.datetime.now().replace(tzinfo=timezone)
+        test = registry_dt.Test.insert()
+        test.col = now.strftime("%Y-%m-%d %H:%M:%S.%f%z")
+        assert test.col == now
+
+    def test_str_conversion_2_by_property(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = timezone.localize(datetime.datetime.now())
+        test = registry_dt.Test.insert()
+        test.col = now.strftime("%Y-%m-%d %H:%M:%S.%f%Z")
+        assert test.col == now
+
+    def test_str_conversion_3_by_property(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = timezone.localize(datetime.datetime.now())
+        test = registry_dt.Test.insert()
+        test.col = now.strftime("%Y-%m-%d %H:%M:%S.%f")
+        assert test.col == now
+
+    def test_str_conversion_4_by_property(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = timezone.localize(datetime.datetime.now())
+        test = registry_dt.Test.insert()
+        test.col = now.strftime("%Y-%m-%d %H:%M:%S")
+        assert test.col == now.replace(microsecond=0)
+
+    def test_by_query(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        d = datetime.datetime(2020, 7, 3, 18, 59, 0)
+        d = add_timezone_on_datetime(d, timezone)
+        Test = registry_dt.Test
+        test = Test.insert()
+        Test.execute_sql_statement(Test.update_sql_statement().values(col=d))
+        registry_dt.refresh(test)
+        assert test.col == d
+
+    def test_by_query_none_value(self, registry_dt):
+        Test = registry_dt.Test
+        test = Test.insert()
+        Test.execute_sql_statement(Test.update_sql_statement().values(col=None))
+        assert test.col is None
+
+    @pytest.mark.skipif(
+        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
+    )
+    def test_str_conversion_1_by_query(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = datetime.datetime.now().replace(tzinfo=timezone)
+        Test = registry_dt.Test
+        test = Test.insert()
+        Test.execute_sql_statement(
+            Test.update_sql_statement().values(
+                col=now.strftime("%Y-%m-%d %H:%M:%S.%f%z")
+            )
+        )
+        registry_dt.expire(test, ["col"])
+        assert test.col == now
+
+    @pytest.mark.skipif(
+        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
+    )
+    def test_str_conversion_2_by_query(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = timezone.localize(datetime.datetime.now())
+        Test = registry_dt.Test
+        test = Test.insert()
+        Test.execute_sql_statement(
+            Test.update_sql_statement().values(
+                col=now.strftime("%Y-%m-%d %H:%M:%S.%f%Z")
+            )
+        )
+        registry_dt.expire(test, ["col"])
+        assert test.col == now
+
+    @pytest.mark.skipif(
+        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
+    )
+    def test_str_conversion_3_by_query(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = timezone.localize(datetime.datetime.now())
+        Test = registry_dt.Test
+        test = Test.insert()
+        Test.execute_sql_statement(
+            Test.update_sql_statement().values(
+                col=now.strftime("%Y-%m-%d %H:%M:%S.%f")
+            )
+        )
+        registry_dt.expire(test, ["col"])
+        assert test.col == now
+
+    @pytest.mark.skipif(
+        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
+    )
+    def test_datetime_str_conversion_4_by_query(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = timezone.localize(datetime.datetime.now())
+        Test = registry_dt.Test
+        test = Test.insert()
+        Test.execute_sql_statement(
+            Test.update_sql_statement().values(
+                col=now.strftime("%Y-%m-%d %H:%M:%S")
+            )
+        )
+        registry_dt.expire(test, ["col"])
+        assert test.col == now.replace(microsecond=0)
+
+    @pytest.mark.skipif(
+        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
+    )
+    def test_datetime_by_query_filter(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = datetime.datetime.now().replace(tzinfo=timezone)
+        test = registry_dt.Test.insert(col=now)
+        Test = registry_dt.Test
+        assert Test.query().filter(Test.col == now).one() is test
+
+    @pytest.mark.skipif(
+        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
+    )
+    def test_datetime_str_conversion_1_by_query_filter(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = datetime.datetime.now().replace(tzinfo=timezone)
+        test = registry_dt.Test.insert(col=now)
+        Test = registry_dt.Test
+        assert (
+            Test.query()
+            .filter(Test.col == now.strftime("%Y-%m-%d %H:%M:%S.%f%z"))
+            .one()
+            is test
+        )
+
+    @pytest.mark.skipif(
+        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
+    )
+    def test_str_conversion_2_by_query_filter(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = timezone.localize(datetime.datetime.now())
+        test = registry_dt.Test.insert(col=now)
+        Test = registry_dt.Test
+        assert (
+            Test.query()
+            .filter(Test.col == now.strftime("%Y-%m-%d %H:%M:%S.%f%Z"))
+            .one()
+            is test
+        )
+
+    @pytest.mark.skipif(
+        sgdb_in(["MySQL", "MariaDB", "MsSQL"]), reason="ISSUE #87"
+    )
+    def test_str_conversion_3_by_query_filter(self, registry_dt):
+        timezone = pytz.timezone(time.tzname[0])
+        now = timezone.localize(datetime.datetime.now())
+        test = registry_dt.Test.insert(col=now)
+        Test = registry_dt.Test
+        assert (
+            Test.query()
+            .filter(Test.col == now.strftime("%Y-%m-%d %H:%M:%S.%f"))
+            .one()
+            is test
+        )
+
+
+def add_modelselection_in_registry():
+    @register(Model)
+    class Test:
+        id = Integer(primary_key=True)
+        col = ModelSelection(validator="my_validator")
+        col2 = ModelSelection(default=Model.System.Blok)
+
+        @classmethod
+        def my_validator(cls, Model):
+            return Model.__registry_name__ == "Model.System.Blok"
+
+
+@pytest.fixture(scope="class")
+def registry_modelselection(request, bloks_loaded):
+    reset_db()
+    registry = init_registry(add_modelselection_in_registry)
+    request.addfinalizer(registry.close)
+    return registry
+
+
+@pytest.mark.relationship
+class TestColumnModelSelection:
+    @pytest.fixture(autouse=True)
+    def transact(self, request, registry_modelselection):
+        transaction = registry_modelselection.begin_nested()
+        request.addfinalizer(transaction.rollback)
+        return
+
+    def test_setter_use_method(self, registry_modelselection):
+        test = registry_modelselection.Test.insert()
+        assert test.col is None
+        assert test.col2 == "Model.System.Blok"
+
+        with pytest.raises(FieldException):
+            test.col = "Model.System"
+
+        test.col = "Model.System.Blok"
+        assert test.col.Model is registry_modelselection.System.Blok
+
+    def test_description(self, registry_modelselection):
+        description = registry_modelselection.Test.fields_description("col")[
+            "col"
+        ]
+        assert description == {
+            "id": "col",
+            "label": "Col",
+            "model": None,
+            "nullable": True,
+            "primary_key": False,
+            "selections": [
+                ("Model.System.Blok", "Model.System.Blok"),
+            ],
+            "type": "ModelSelection",
+        }
+
+    def test_description2(self, registry_modelselection):
+        description = registry_modelselection.Test.fields_description(
+            ["col", "col2"]
+        )
+        assert (
+            description["col"]["selections"]
+            != description["col2"]["selections"]
+        )
+
+    def test_setter_model_validator_all(self, registry_modelselection):
+        assert model_validator_all(registry_modelselection.System) is True
+
+    def test_modelselection_setter_model_validator_is_sql(
+        self, registry_modelselection
+    ):
+        assert model_validator_is_sql(registry_modelselection.System) is False
+        assert (
+            model_validator_is_sql(registry_modelselection.System.Blok) is True
+        )
+
+    def test_modelselection_setter_model_validator_is_not_sql(
+        self, registry_modelselection
+    ):
+        assert (
+            model_validator_is_not_sql(registry_modelselection.System) is True
+        )
+        assert (
+            model_validator_is_not_sql(registry_modelselection.System.Blok)
+            is False
+        )
+
+    def test_modelselection_setter_model_validator_is_view(
+        self, registry_modelselection
+    ):
+        assert model_validator_is_view(registry_modelselection.System) is False
+        assert (
+            model_validator_is_view(registry_modelselection.System.Blok)
+            is False
+        )
+
+    def test_modelselection_setter_model_validator_is_not_view(
+        self, registry_modelselection
+    ):
+        assert (
+            model_validator_is_not_view(registry_modelselection.System) is True
+        )
+        assert (
+            model_validator_is_not_view(registry_modelselection.System.Blok)
+            is True
+        )
+
+    def test_modelselection_setter_model_validator_in_namespace(
+        self, registry_modelselection
+    ):
+        assert (
+            model_validator_in_namespace(Model.System)(
+                registry_modelselection.Test
+            )
+            is False
+        )
+        assert (
+            model_validator_in_namespace(Model.System)(
+                registry_modelselection.System
+            )
+            is False
+        )
+        assert (
+            model_validator_in_namespace(Model.System)(
+                registry_modelselection.System.Blok
+            )
+            is True
+        )
+
+    def test_modelselection_setter_model_validator_merge(
+        self, registry_modelselection
+    ):
+        validator = merge_validators(
+            model_validator_is_sql,
+            model_validator_is_not_view,
+            model_validator_in_namespace(Model.System),
+        )
+        assert validator(registry_modelselection.Test) is False
+        assert validator(registry_modelselection.System) is False
+        assert validator(registry_modelselection.System.Blok) is True
+
+    def test_search_with_str(self, registry_modelselection):
+        test = registry_modelselection.Test.insert()
+        test.col = "Model.System.Blok"
+        registry_modelselection.flush()
+        test2 = (
+            registry_modelselection.Test.query()
+            .filter_by(col="Model.System.Blok")
+            .one()
+        )
+        assert test is test2
+
+    def test_search_with_model(self, registry_modelselection):
+        test = registry_modelselection.Test.insert()
+        test.col = registry_modelselection.System.Blok
+        registry_modelselection.flush()
+        test2 = (
+            registry_modelselection.Test.query()
+            .filter_by(col=registry_modelselection.System.Blok)
+            .one()
+        )
+        assert test is test2
+
+    def test_search_with_declaration_model(self, registry_modelselection):
+        test = registry_modelselection.Test.insert()
+        test.col = Model.System.Blok
+        registry_modelselection.flush()
+        test2 = (
+            registry_modelselection.Test.query()
+            .filter_by(col=Model.System.Blok)
+            .one()
+        )
+        assert test is test2
+
+
+def add_modelfieldselection_in_registry():
+    @register(Model)
+    class Test:
+        id = Integer(primary_key=True)
+        col = ModelFieldSelection(
+            model_validator="my_model_validator",
+            field_validator="my_field_validator",
+        )
+        col2 = ModelFieldSelection(default=Model.System.Blok.use("name"))
+
+        @classmethod
+        def my_model_validator(cls, Model):
+            return Model.__registry_name__ == "Model.System.Blok"
+
+        @classmethod
+        def my_field_validator(cls, field):
+            return field.anyblok_field_name == "name"
+
+
+@pytest.fixture(scope="class")
+def registry_modelfieldselection(request, bloks_loaded):
+    reset_db()
+    registry = init_registry(add_modelfieldselection_in_registry)
+    request.addfinalizer(registry.close)
+    return registry
+
+
+@pytest.mark.relationship
+class TestColumnModelFieldSelection:
+    @pytest.fixture(autouse=True)
+    def transact(self, request, registry_modelfieldselection):
+        transaction = registry_modelfieldselection.begin_nested()
+        request.addfinalizer(transaction.rollback)
+        return
+
+    def test_setter_use_method(self, registry_modelfieldselection):
+        test = registry_modelfieldselection.Test.insert()
+        assert test.col is None
+        assert test.col2 == "Model.System.Blok => name"
+
+        with pytest.raises(FieldException):
+            test.col = "Model.System.Blok => version"
+
+        test.col = "Model.System.Blok => name"
+        assert test.col.field == registry_modelfieldselection.System.Blok.name
+
+    def test_description(self, registry_modelfieldselection):
+        description = registry_modelfieldselection.Test.fields_description(
+            "col"
+        )["col"]
+        assert description == {
+            "id": "col",
+            "label": "Col",
+            "model": None,
+            "nullable": True,
+            "primary_key": False,
+            "selections": [
+                ("Model.System.Blok => name", "Model.System.Blok : name"),
+            ],
+            "type": "ModelFieldSelection",
+        }
+
+    def test_description2(self, registry_modelfieldselection):
+        description = registry_modelfieldselection.Test.fields_description(
+            ["col", "col2"]
+        )
+        assert (
+            description["col"]["selections"]
+            != description["col2"]["selections"]
+        )
+
+    def test_setter_field_validator_all(self, registry_modelfieldselection):
+        assert (
+            field_validator_all(registry_modelfieldselection.System.Blok.name)
+            is True
+        )
+
+    def test_setter_field_validator_is_field(
+        self, registry_modelfieldselection
+    ):
+        assert (
+            field_validator_is_field(
+                registry_modelfieldselection.System.Blok.logo
+            )
+            is True
+        )
+
+    def test_setter_field_validator_is_not_field(
+        self, registry_modelfieldselection
+    ):
+        assert (
+            field_validator_is_not_field(
+                registry_modelfieldselection.System.Blok.logo
+            )
+            is False
+        )
+
+    def test_setter_field_validator_is_column(
+        self, registry_modelfieldselection
+    ):
+        assert (
+            field_validator_is_column(
+                registry_modelfieldselection.System.Blok.name
+            )
+            is True
+        )
+
+    def test_setter_field_validator_is_not_column(
+        self, registry_modelfieldselection
+    ):
+        assert (
+            field_validator_is_not_column(
+                registry_modelfieldselection.System.Blok.name
+            )
+            is False
+        )
+
+    def test_setter_field_validator_is_relationship(
+        self, registry_modelfieldselection
+    ):
+        assert (
+            field_validator_is_relationship(
+                registry_modelfieldselection.System.Blok.name
+            )
+            is False
+        )
+
+    def test_setter_field_validator_is_not_relationship(
+        self, registry_modelfieldselection
+    ):
+        assert (
+            field_validator_is_not_relationship(
+                registry_modelfieldselection.System.Blok.name
+            )
+            is True
+        )
+
+    def test_setter_field_validator_is_named(
+        self, registry_modelfieldselection
+    ):
+        assert (
+            field_validator_is_named("name")(
+                registry_modelfieldselection.System.Blok.name
+            )
+            is True
+        )
+
+    def test_setter_field_validator_is_from_types(
+        self, registry_modelfieldselection
+    ):
+        assert (
+            field_validator_is_from_types(String, Many2One)(
+                registry_modelfieldselection.System.Blok.name
+            )
+            is True
+        )
+
+    def test_modelselection_setter_validator_merge(
+        self, registry_modelfieldselection
+    ):
+        validator = merge_validators(
+            field_validator_is_column,
+            field_validator_is_from_types(String),
+        )
+        assert validator(registry_modelfieldselection.Test.id) is False
+        assert validator(registry_modelfieldselection.System.Blok.name) is True
+
+    def test_search_with_str(self, registry_modelfieldselection):
+        test = registry_modelfieldselection.Test.insert()
+        test.col = "Model.System.Blok => name"
+        registry_modelfieldselection.flush()
+        test2 = (
+            registry_modelfieldselection.Test.query()
+            .filter_by(col="Model.System.Blok => name")
+            .one()
+        )
+        assert test is test2
+
+    def test_search_with_model(self, registry_modelfieldselection):
+        test = registry_modelfieldselection.Test.insert()
+        test.col = registry_modelfieldselection.System.Blok.name
+        registry_modelfieldselection.flush()
+        test2 = (
+            registry_modelfieldselection.Test.query()
+            .filter_by(
+                col=fieldToModelAttribute(
+                    registry_modelfieldselection.System.Blok.name
+                )
+            )
+            .one()
+        )
+        assert test is test2
+
+    def test_search_with_declaration_model(self, registry_modelfieldselection):
+        test = registry_modelfieldselection.Test.insert()
+        test.col = Model.System.Blok.use("name")
+        registry_modelfieldselection.flush()
+        test2 = (
+            registry_modelfieldselection.Test.query()
+            .filter_by(col=Model.System.Blok.use("name"))
+            .one()
+        )
+        assert test is test2
+
+
 class TestColumnsAutoDoc:
     def call_autodoc(self, column, **kwargs):
         col = column(**kwargs)
         col.autodoc()
 
     def test_autodoc(self, column_definition):
         column, _, kwargs = column_definition
@@ -1570,14 +1973,17 @@
     def test_uuid_char32(self):
         self.call_autodoc(UUID, binary=False)
 
     @pytest.mark.skipif(not has_pycountry, reason="pycountry is not installed")
     def test_pycoundtry_at_insert_with_alpha_3(self):
         self.call_autodoc(Country, mode="alpha_3")
 
+    def test_modelselection(self):
+        self.call_autodoc(ModelSelection)
+
 
 class Test_convert_string_to_datetime:
     def test_with_none(self):
         assert convert_string_to_datetime(None) is None
 
     def test_with_datetime(self):
         now = datetime.datetime.now()
```

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_config.py` & `AnyBlok-2.1.0/anyblok/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_core.py` & `AnyBlok-2.1.0/anyblok/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_core_query.py` & `AnyBlok-2.1.0/anyblok/tests/test_core_query.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_core_sqlbase.py` & `AnyBlok-2.1.0/anyblok/tests/test_core_sqlbase.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_declaration.py` & `AnyBlok-2.1.0/anyblok/tests/test_declaration.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_environment.py` & `AnyBlok-2.1.0/anyblok/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_event.py` & `AnyBlok-2.1.0/anyblok/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_field.py` & `AnyBlok-2.1.0/anyblok/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_graphviz.py` & `AnyBlok-2.1.0/anyblok/tests/test_graphviz.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_hybrid_method.py` & `AnyBlok-2.1.0/anyblok/tests/test_hybrid_method.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_ignore_migration.py` & `AnyBlok-2.1.0/anyblok/tests/test_ignore_migration.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_imp.py` & `AnyBlok-2.1.0/anyblok/tests/test_imp.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_inherit.py` & `AnyBlok-2.1.0/anyblok/tests/test_inherit.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,15 +531,18 @@
             @register(Model)
             class Test:
                 id = Integer(primary_key=True)
 
             @register(Model)
             class Test2:
                 id = Integer(primary_key=True)
-                test = Many2One(model=Model.Test, one2many="test2")
+                test = Many2One(
+                    model=Model.Test,
+                    one2many=("test2", dict(enable_typechecks=False)),
+                )
 
             @register(Model)
             class Test3(Model.Test2):
                 id = Integer(primary_key=True)
                 test2 = Integer(foreign_key=Model.Test2.use("id"))
 
         registry = self.init_registry(add_in_registry)
@@ -555,15 +558,18 @@
             class Test:
                 id = Integer(primary_key=True)
 
             @register(Model)
             class Test2:
                 id = Integer(primary_key=True)
                 test_id = Integer(foreign_key=Model.Test.use("id"))
-                test = Many2One(model=Model.Test, one2many="test2")
+                test = Many2One(
+                    model=Model.Test,
+                    one2many=("test2", dict(enable_typechecks=False)),
+                )
 
             @register(Model)
             class Test3(Model.Test2):
                 id = Integer(primary_key=True)
                 test2 = Integer(foreign_key=Model.Test2.use("id"))
 
         registry = self.init_registry(add_in_registry)
```

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_instrumented_list.py` & `AnyBlok-2.1.0/anyblok/tests/test_instrumented_list.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_many2many.py` & `AnyBlok-2.1.0/anyblok/tests/test_many2many.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_many2one.py` & `AnyBlok-2.1.0/anyblok/tests/test_many2one.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_mapper.py` & `AnyBlok-2.1.0/anyblok/tests/test_mapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -37,23 +37,22 @@
     def transact(self, request, registry_blok):
         transaction = registry_blok.begin_nested()
         request.addfinalizer(transaction.rollback)
         return
 
     def test_get_attribute(self, registry_blok):
         registry = registry_blok
-        ma = ModelAttribute("Model.System.Model", "name")
+        ma = ModelAttribute("Model.System.Blok", "name")
         assert (
-            ma.get_attribute(registry)
-            == registry.get("Model.System.Model").name
+            ma.get_attribute(registry) == registry.get("Model.System.Blok").name
         )
 
     def test_without_attribute(self, registry_blok):
         with pytest.raises(ModelAttributeException):
-            ModelAttribute("Model.System.Model", None)
+            ModelAttribute("Model.System.Blok", None)
 
     def test_without_model(self, registry_blok):
         with pytest.raises(ModelAttributeException):
             ModelAttribute(None, "name")
 
     def test_without_model_and_attribute(self, registry_blok):
         with pytest.raises(ModelAttributeException):
@@ -63,15 +62,15 @@
         registry = registry_blok
         ma = ModelAttribute("Model.Unexisting.Model", "name")
         with pytest.raises(ModelAttributeException):
             ma.get_attribute(registry)
 
     def test_get_attribute_unexisting_attribute(self, registry_blok):
         registry = registry_blok
-        ma = ModelAttribute("Model.System.Model", "id")
+        ma = ModelAttribute("Model.System.Blok", "id")
         with pytest.raises(ModelAttributeException):
             ma.get_attribute(registry)
 
     def test_get_fk_name_with_wrong_model(self, registry_blok):
         registry = registry_blok
         ma = ModelAttribute("Model.System", "name")
         with pytest.raises(ModelAttributeException):
@@ -81,95 +80,95 @@
         registry = registry_blok
         ma = ModelAttribute("Model.Unexisting.Model", "name")
         with pytest.raises(ModelAttributeException):
             ma.get_fk_name(registry)
 
     def test_get_fk_name_unexisting_attribute(self, registry_blok):
         registry = registry_blok
-        ma = ModelAttribute("Model.System.Model", "id")
+        ma = ModelAttribute("Model.System.Blok", "id")
         with pytest.raises(ModelAttributeException):
             ma.get_fk_name(registry)
 
     def test_get_fk_name(self, registry_blok):
         registry = registry_blok
-        ma = ModelAttribute("Model.System.Model", "name")
-        assert ma.get_fk_name(registry) == "system_model.name"
+        ma = ModelAttribute("Model.System.Blok", "name")
+        assert ma.get_fk_name(registry) == "system_blok.name"
 
     def test_get_fk(self, registry_blok):
         registry = registry_blok
-        ma = ModelAttribute("Model.System.Model", "name")
+        ma = ModelAttribute("Model.System.Blok", "name")
         assert isinstance(ma.get_fk(registry), ForeignKey)
 
     def test_get_fk_with_options(self, registry_blok):
         registry = registry_blok
-        ma = ModelAttribute("Model.System.Model", "name").options(
+        ma = ModelAttribute("Model.System.Blok", "name").options(
             ondelete="cascade"
         )
         mafk = ma.get_fk(registry)
         assert isinstance(mafk, ForeignKey)
 
     def test_use(self, registry_blok):
-        ma = Declarations.Model.System.Model.use("name")
+        ma = Declarations.Model.System.Blok.use("name")
         assert isinstance(ma, ModelAttribute)
-        assert ma.model_name == "Model.System.Model"
+        assert ma.model_name == "Model.System.Blok"
         assert ma.attribute_name == "name"
 
     def test_str(self, registry_blok):
-        ma = ModelAttribute("Model.System.Model", "name")
-        assert str(ma) == "Model.System.Model => name"
+        ma = ModelAttribute("Model.System.Blok", "name")
+        assert str(ma) == "Model.System.Blok => name"
 
     def test_get_fk_remote(self, registry_blok):
         registry = registry_blok
-        ma = ModelAttribute("Model.System.Column", "name")
+        ma = ModelAttribute("Model.System.Blok", "name")
         assert ma.get_fk_remote(registry) is None
 
     def test_get_complete_remote(self, registry_blok):
         registry = registry_blok
-        ma = ModelAttribute("Model.System.Field", "name")
+        ma = ModelAttribute("Model.System.Blok", "name")
         assert ma.get_complete_remote(registry) is None
 
     def test_existing_FakeColumn(self, registry_blok):
         registry = registry_blok
-        ma = ModelAttribute("Model.System.Field", "name")
+        ma = ModelAttribute("Model.System.Blok", "name")
         assert ma.add_fake_column(registry) is None
 
     def test_existing_FakeRelationShip(self, registry_blok):
         registry = registry_blok
-        ma = ModelAttribute("Model.System.Field", "name")
+        ma = ModelAttribute("Model.System.Blok", "name")
         assert (
             ma.add_fake_relationship(registry, "Model.System", "test") is None
         )
 
     def test_get_column_name(self, registry_blok):
         registry = registry_blok
-        ma = ModelAttribute("Model.System.Field", "name")
+        ma = ModelAttribute("Model.System.Blok", "name")
         assert ma.get_column_name(registry) == "name"
 
     def test_check_model_in_first_step_no_sql_model(self, registry_blok):
         registry = registry_blok
         ma = ModelAttribute("Model.System", "name")
         with pytest.raises(ModelAttributeException):
             ma.check_model_in_first_step(registry)
 
 
 class TestModelAttributeAdapter:
     def test_from_declaration(self):
-        ma = ModelAttribute("Model.System.Model", "name")
+        ma = ModelAttribute("Model.System.Blok", "name")
         maa = ModelAttributeAdapter(ma)
         assert maa is ma
 
     def test_from_registry_name(self):
-        maa = ModelAttributeAdapter("Model.System.Model=>name")
+        maa = ModelAttributeAdapter("Model.System.Blok=>name")
         assert isinstance(maa, ModelAttribute)
-        assert maa.model_name == "Model.System.Model"
+        assert maa.model_name == "Model.System.Blok"
         assert maa.attribute_name == "name"
 
     def test_from_registry_name_without_attribute(self):
         with pytest.raises(ModelAttributeAdapterException):
-            ModelAttributeAdapter("Model.System.Model")
+            ModelAttributeAdapter("Model.System.Blok")
 
 
 class TestModelRepr:
     @pytest.fixture(autouse=True)
     def transact(self, request, registry_blok):
         transaction = registry_blok.begin_nested()
         request.addfinalizer(transaction.rollback)
@@ -179,28 +178,28 @@
         registry = registry_blok
         mr = ModelRepr("Model.Unexisting.Model")
         with pytest.raises(ModelReprException):
             mr.check_model(registry)
 
     def test_get_tablename(self, registry_blok):
         registry = registry_blok
-        mr = ModelRepr("Model.System.Model")
-        assert mr.tablename(registry) == "system_model"
+        mr = ModelRepr("Model.System.Blok")
+        assert mr.tablename(registry) == "system_blok"
 
     def test_get_registry_name(self, registry_blok):
-        mr = ModelRepr("Model.System.Model")
-        assert mr.model_name == "Model.System.Model"
+        mr = ModelRepr("Model.System.Blok")
+        assert mr.model_name == "Model.System.Blok"
 
     def test_str(self, registry_blok):
-        mr = ModelRepr("Model.System.Model")
-        assert str(mr) == "Model.System.Model"
+        mr = ModelRepr("Model.System.Blok")
+        assert str(mr) == "Model.System.Blok"
 
     def test_get_primary_keys(self, registry_blok):
         registry = registry_blok
-        mr = ModelRepr("Model.System.Model")
+        mr = ModelRepr("Model.System.Blok")
         mas = mr.primary_keys(registry)
         assert len(mas) == 1
         assert [x.attribute_name for x in mas] == ["name"]
 
     def test_without_model(self, registry_blok):
         with pytest.raises(ModelReprException):
             ModelRepr(None)
@@ -211,110 +210,110 @@
             mm.mapper(registry_blok, "Model.System.Blok")
             is registry_blok.System.Blok
         )
 
 
 class TestModelAdapter:
     def test_from_declaration(self):
-        mr = ModelRepr("Model.System.Model")
+        mr = ModelRepr("Model.System.Blok")
         mra = ModelAdapter(mr)
         assert mr is mra
 
     def test_from_registry_name(self):
-        mra = ModelAdapter("Model.System.Model")
+        mra = ModelAdapter("Model.System.Blok")
         assert isinstance(mra, ModelRepr)
-        assert mra.model_name == "Model.System.Model"
+        assert mra.model_name == "Model.System.Blok"
 
 
 class TestModelMapper:
     def test_not_capable(self):
         assert not (ModelMapper.capable(None))
 
     def test_capable_by_declaration(self):
-        assert ModelMapper.capable(Model.System.Model)
+        assert ModelMapper.capable(Model.System.Blok)
 
     def test_capable_by_registry_name(self):
-        assert ModelMapper.capable("Model.System.Model")
+        assert ModelMapper.capable("Model.System.Blok")
 
     def test_capable_by_model_repr(self):
-        assert ModelMapper.capable(ModelRepr("Model.System.Model"))
+        assert ModelMapper.capable(ModelRepr("Model.System.Blok"))
 
     def test_model_repr(self):
-        assert ModelMapper(ModelRepr("Model.System.Model"), None)
+        assert ModelMapper(ModelRepr("Model.System.Blok"), None)
 
     def test_by_declaration(self):
-        mm = ModelMapper(Model.System.Model, "even")
+        mm = ModelMapper(Model.System.Blok, "even")
         assert isinstance(mm.model, ModelRepr)
-        assert mm.model.model_name, "Model.System.Model"
+        assert mm.model.model_name, "Model.System.Blok"
 
     def test_by_registry_name(self):
-        mm = ModelMapper("Model.System.Model", "event")
+        mm = ModelMapper("Model.System.Blok", "event")
         assert isinstance(mm.model, ModelRepr)
-        assert mm.model.model_name, "Model.System.Model"
+        assert mm.model.model_name, "Model.System.Blok"
 
     def test_listen_sqlalchemy(self):
         def method():
             pass
 
-        mm = ModelMapper(Model.System.Model, "before_insert")
+        mm = ModelMapper(Model.System.Blok, "before_insert")
         mm.listen(method)
         assert method.is_an_sqlalchemy_event_listener
         assert method.sqlalchemy_listener is mm
 
     def test_listen_anyblok(self):
         def method():
             pass
 
-        mm = ModelMapper(Model.System.Model, "event")
+        mm = ModelMapper(Model.System.Blok, "event")
         mm.listen(method)
         assert method.is_an_event_listener
-        assert method.model == "Model.System.Model"
+        assert method.model == "Model.System.Blok"
         assert method.event == "event"
 
 
 class TestModelAttributeMapper:
     def test_not_str_capable(self):
-        assert not (ModelAttributeMapper.capable("Model.System.Model"))
+        assert not (ModelAttributeMapper.capable("Model.System.Blok"))
 
     def test_not_capable(self):
         assert not (ModelAttributeMapper.capable(None))
 
     def test_capable_by_declaration(self):
-        assert ModelAttributeMapper.capable(Model.System.Model.use("name"))
+        assert ModelAttributeMapper.capable(Model.System.Blok.use("name"))
 
     def test_capable_by_registry_name(self):
-        assert ModelAttributeMapper.capable("Model.System.Model=>name")
+        assert ModelAttributeMapper.capable("Model.System.Blok=>name")
 
     def test_by_declaration(self):
-        mam = ModelAttributeMapper(Model.System.Model.use("name"), "event")
+        mam = ModelAttributeMapper(Model.System.Blok.use("name"), "event")
         assert isinstance(mam.attribute, ModelAttribute)
-        assert mam.attribute.model_name == "Model.System.Model"
+        assert mam.attribute.model_name == "Model.System.Blok"
 
     def test_by_registry_name(self):
-        mam = ModelAttributeMapper("Model.System.Model=>name", "event")
+        mam = ModelAttributeMapper("Model.System.Blok=>name", "event")
         assert isinstance(mam.attribute, ModelAttribute)
-        assert mam.attribute.model_name == "Model.System.Model"
+        assert mam.attribute.model_name == "Model.System.Blok"
 
     def test_listen(self):
         def method():
             pass
 
-        mam = ModelAttributeMapper(Model.System.Model.use("name"), "set")
+        mam = ModelAttributeMapper(Model.System.Blok.use("name"), "set")
         mam.listen(method)
         assert method.is_an_sqlalchemy_event_listener
         assert method.sqlalchemy_listener is mam
 
 
 class TestMapperAdapter:
     def test_model_mapper(self):
-        mam = MapperAdapter("Model.System.Model", "event")
+        mam = MapperAdapter("Model.System.Blok", "event")
         assert isinstance(mam, ModelMapper)
 
     def test_model_attribute_mapper(self):
-        mam = MapperAdapter("Model.System.Model=>name", "event")
+        mam = MapperAdapter("Model.System.Blok=>name", "event")
         assert isinstance(mam, ModelAttributeMapper)
 
     def test_no_mapper(self):
         with pytest.raises(MapperException):
             MapperAdapter(None)
 
 
@@ -357,20 +356,20 @@
         mr = ModelRepr("Model.Test2")
         mas = mr.foreign_keys_for(registry, "Model.Test")
         assert len(mas) == 1
         assert [x.attribute_name for x in mas] == ["test_id"]
 
     def test_get_mapper(self):
         registry = self.init_registry(None)
-        mm = ModelMapper(Model.System.Model, "even")
-        assert mm.mapper(registry, None) is registry.System.Model
+        mm = ModelMapper(Model.System.Blok, "even")
+        assert mm.mapper(registry, None) is registry.System.Blok
 
     def test_get_attribute_mapper(self):
         registry = self.init_registry(None)
-        mam = ModelAttributeMapper(Model.System.Model.use("name"), "set")
+        mam = ModelAttributeMapper(Model.System.Blok.use("name"), "set")
         # We can't compare that the column are the same, because is the case
         # of the call are in the class attribute (no instance) SQLAlchemy
         # Wrap the result for each call, then each call return a différent
         # object, but it is not an error
         getted = str(mam.mapper(registry, None) == "test")
-        wanted = str(registry.System.Model.name == "test")
+        wanted = str(registry.System.Blok.name == "test")
         assert getted == wanted
```

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_migration.py` & `AnyBlok-2.1.0/anyblok/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_migration_db_schema.py` & `AnyBlok-2.1.0/anyblok/tests/test_migration_db_schema.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_mixin.py` & `AnyBlok-2.1.0/anyblok/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_model.py` & `AnyBlok-2.1.0/anyblok/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,22 +211,17 @@
         self.registry = init_registry(*args, **kwargs)
         return self.registry
 
     def test_anyblok_attribute(self):
         registry = self.init_registry(simple_model)
         self.check_registry(registry.Test)
         assert registry.System.anyblok is registry
-        assert registry.System.Model.anyblok is registry
+        assert registry.System.Blok.anyblok is registry
         t2 = registry.Test.query().first()
-        registry.System.Model.anyblok.refresh(t2)
-
-    def test_str(self):
-        registry = self.init_registry(simple_model)
-        test = registry.System.Model.query().get("Model.Test")
-        assert str(test) == "Model.Test"
+        registry.System.Blok.anyblok.refresh(t2)
 
     def test_model_is_assembled(self):
         with LogCapture("anyblok.registry", level=DEBUG) as logs:
             self.init_registry(None)
             messages = logs.get_debug_messages()
             assert "Assemble 'Model' entry" in messages
 
@@ -245,24 +240,28 @@
         t = Model1.insert(name="test")
         t2 = Model2.query().first()
         assert t2.name == t.name
 
     def test_simple_model(self):
         registry = self.init_registry(simple_model)
         self.check_registry(registry.Test)
-        model = registry.System.Model.query().get("Model.Test")
-        assert model.table == "test"
-        assert model.schema is None
+        assert registry.Test.__db_schema__ is None
+        assert registry.Test.id.field_description() == {
+            "id": "id",
+            "label": "Id",
+            "model": None,
+            "nullable": False,
+            "primary_key": True,
+            "type": "Integer",
+        }
 
     def test_simple_model_with_schema(self):
         registry = self.init_registry(simple_model_with_schema)
         self.check_registry(registry.Test)
-        model = registry.System.Model.query().get("Model.Test")
-        assert model.table == "test"
-        assert model.schema == "test_db_schema"
+        assert registry.Test.__db_schema__ == "test_db_schema"
 
     def test_simple_model_with_tablename(self):
         registry = self.init_registry(simple_model_with_tablename)
         self.check_registry(registry.Test)
         assert registry.Test.__table__.name == "othername"
         assert registry.Test.__tablename__ == "othername"
```

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_one2many.py` & `AnyBlok-2.1.0/anyblok/tests/test_one2many.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_one2one.py` & `AnyBlok-2.1.0/anyblok/tests/test_one2one.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_polymorphic.py` & `AnyBlok-2.1.0/anyblok/tests/test_polymorphic.py`

 * *Files 2% similar despite different names*

```diff
@@ -469,14 +469,35 @@
         assert registry.Employee.getFieldType("room") == "Many2One"
         assert registry.Engineer.getFieldType("id") == "Integer"
         assert registry.Engineer.getFieldType("name") == "String"
         assert registry.Engineer.getFieldType("type_entity") == "String"
         assert registry.Engineer.getFieldType("engineer_name") == "String"
         assert registry.Engineer.getFieldType("room") == "Many2One"
 
+    def test_hybrid_property_column_with_relationship(
+        self, registry_multi_table_poly_fk
+    ):
+        registry = registry_multi_table_poly_fk
+        hb_cols = registry.Employee.get_hybrid_property_columns()
+        assert "name" in hb_cols
+        assert "type_entity" in hb_cols
+        assert "room" in hb_cols
+
+        hb_cols = registry.Engineer.get_hybrid_property_columns()
+        assert "name" in hb_cols
+        assert "type_entity" in hb_cols
+        assert "room" in hb_cols
+
+    def test_get_model_information(self, registry_multi_table_poly_fk):
+        registry = registry_multi_table_poly_fk
+        res = registry.Employee.find_remote_attribute_to_expire("room")
+        assert res == {"room": ["employees"]}
+        res = registry.Engineer.find_remote_attribute_to_expire("room")
+        assert res == {"room": ["employees"]}
+
 
 def multi_table_foreign_key_with_one_define_mapper_args():
     @register(Model)
     class Room:
         id = Integer(primary_key=True)
         name = String()
```

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_registry.py` & `AnyBlok-2.1.0/anyblok/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_registry_core.py` & `AnyBlok-2.1.0/anyblok/tests/test_registry_core.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_registry_entry.py` & `AnyBlok-2.1.0/anyblok/tests/test_registry_entry.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_registry_manager.py` & `AnyBlok-2.1.0/anyblok/tests/test_registry_manager.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_relationship.py` & `AnyBlok-2.1.0/anyblok/tests/test_relationship.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_schema.py` & `AnyBlok-2.1.0/anyblok/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_version.py` & `AnyBlok-2.1.0/anyblok/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/test_view.py` & `AnyBlok-2.1.0/anyblok/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/tests/testcase.py` & `AnyBlok-2.1.0/anyblok/tests/testcase.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok/version.py` & `AnyBlok-2.1.0/anyblok/version.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/anyblok_nose/plugins.py` & `AnyBlok-2.1.0/anyblok_nose/plugins.py`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/doc/CHANGES.rst` & `AnyBlok-2.1.0/doc/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,28 @@
 .. This Source Code Form is subject to the terms of the Mozilla Public License,
 .. v. 2.0. If a copy of the MPL was not distributed with this file,You can
 .. obtain one at http://mozilla.org/MPL/2.0/.
 
 CHANGELOG
 =========
 
+2.1.0 (2023-07-26)
+------------------
+
+* Implement psycopg3 capability
+* Improved TimeStamp field
+* Fixed #227 str and repr of the query call str query.sql_statement
+* Refactored main methods to get the description of the models and fields
+  without used the existing table
+* Added new column type **ModelSelection** this role is to replace a column
+  with a foreigh key to the deprecated model **Model.System.Model**
+* Added new column type **ModelFieldSelection** this role is to replace a
+  column with a foreigh key to the deprecated model **Model.System.Field**,
+  **Model.System.Column** or **Model.System.Relationship**
+
 2.0.0 (2023-03-11)
 ------------------
 
 * Upgrade version of sqlalchemy to **2.0.0**
 * Upgrade version of sqlalchemy utils to **0.40.0**
 * Upgrade version of sqlalchemy views to **0.3.2**
 * The previsous deprecated configuration are placed as removed
```

### Comparing `AnyBlok-2.0.0/doc/FRONT.rst` & `AnyBlok-2.1.0/doc/FRONT.rst`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/doc/MEMENTO.rst` & `AnyBlok-2.1.0/doc/MEMENTO.rst`

 * *Files 4% similar despite different names*

```diff
@@ -931,3470 +931,3808 @@
 00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003a30: 2020 2020 2020 2020 2020 207c 0a2b 2d2d             |.+--
 00003a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00003a50: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
 00003a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00003a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00003a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003a90: 2b0a 7c20 6973 5f73 716c 5f76 6965 7720  +.| is_sql_view 
-00003aa0: 2020 2020 207c 2042 6f6f 6c65 616e 2066       | Boolean f
-00003ab0: 6c61 672c 2077 6869 6368 2069 6e64 6963  lag, which indic
-00003ac0: 6174 6569 7320 6966 2074 6865 206d 6f64  ateis if the mod
-00003ad0: 656c 2069 7320 6261 7365 6420 6f6e 2061  el is based on a
-00003ae0: 2053 514c 207c 0a7c 2020 2020 2020 2020   SQL |.|        
-00003af0: 2020 2020 2020 2020 2020 7c20 7669 6577            | view
-00003b00: 2e20 4465 7072 6563 6174 6564 2075 7365  . Deprecated use
-00003b10: 2066 6163 746f 7279 2020 2020 2020 2020   factory        
-00003b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a90: 2b0a 7c20 6661 6374 6f72 7920 2020 2020  +.| factory     
+00003aa0: 2020 2020 207c 2046 6163 746f 7279 2063       | Factory c
+00003ab0: 6c61 7373 2074 6f20 6275 696c 6420 7468  lass to build th
+00003ac0: 6520 4d6f 6465 6c20 636c 6173 732e 2020  e Model class.  
+00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ae0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+00003af0: 2020 2020 2020 2020 2020 7c20 4465 6661            | Defa
+00003b00: 756c 7420 3a20 6060 616e 7962 6c6f 6b2e  ult : ``anyblok.
+00003b10: 6d6f 6465 6c2e 6661 6374 6f72 792e 4d6f  model.factory.Mo
+00003b20: 6465 6c46 6163 746f 7279 6060 2020 2020  delFactory``    
 00003b30: 2020 2020 2020 2020 2020 7c0a 2b2d 2d2d            |.+---
 00003b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
 00003b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00003b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00003b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00003b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00003b90: 0a7c 2066 6163 746f 7279 2020 2020 2020  .| factory      
-00003ba0: 2020 2020 7c20 4661 6374 6f72 7920 636c      | Factory cl
-00003bb0: 6173 7320 746f 2062 7569 6c64 2074 6865  ass to build the
-00003bc0: 204d 6f64 656c 2063 6c61 7373 2e20 2020   Model class.   
-00003bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003be0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00003bf0: 2020 2020 2020 2020 207c 2044 6566 6175           | Defau
-00003c00: 6c74 203a 2060 6061 6e79 626c 6f6b 2e6d  lt : ``anyblok.m
-00003c10: 6f64 656c 2e66 6163 746f 7279 2e4d 6f64  odel.factory.Mod
-00003c20: 656c 4661 6374 6f72 7960 6020 2020 2020  elFactory``     
-00003c30: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
-00003c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-00003c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003c70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003c80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
-00003c90: 7c20 7461 626c 656e 616d 6520 2020 2020  | tablename     
-00003ca0: 2020 207c 2044 6566 696e 6520 7468 6520     | Define the 
-00003cb0: 7265 616c 206e 616d 6520 6f66 2074 6865  real name of the
-00003cc0: 2074 6162 6c65 2e20 4279 2064 6566 6175   table. By defau
-00003cd0: 6c74 2074 6865 2074 6162 6c65 206e 616d  lt the table nam
-00003ce0: 6520 207c 0a7c 2020 2020 2020 2020 2020  e  |.|          
-00003cf0: 2020 2020 2020 2020 7c20 6973 2074 6865          | is the
-00003d00: 2072 6567 6973 7472 7920 6e61 6d65 2077   registry name w
-00003d10: 6974 686f 7574 2074 6865 2064 6563 6c61  ithout the decla
-00003d20: 7261 7469 6f6e 2074 7970 652c 2061 6e64  ration type, and
-00003d30: 2077 6974 6820 2020 7c0a 7c20 2020 2020   with   |.|     
-00003d40: 2020 2020 2020 2020 2020 2020 207c 2027               | '
-00003d50: 2e27 2072 6570 6c61 6365 6420 7769 7468  .' replaced with
-00003d60: 2027 5f27 2e20 5468 6973 2061 7474 7269   '_'. This attri
-00003d70: 6275 7465 2069 7320 616c 736f 2075 7365  bute is also use
-00003d80: 6420 746f 206d 6170 2061 6e20 207c 0a7c  d to map an  |.|
+00003b90: 0a7c 2074 6162 6c65 6e61 6d65 2020 2020  .| tablename    
+00003ba0: 2020 2020 7c20 4465 6669 6e65 2074 6865      | Define the
+00003bb0: 2072 6561 6c20 6e61 6d65 206f 6620 7468   real name of th
+00003bc0: 6520 7461 626c 652e 2042 7920 6465 6661  e table. By defa
+00003bd0: 756c 7420 7468 6520 7461 626c 6520 6e61  ult the table na
+00003be0: 6d65 2020 7c0a 7c20 2020 2020 2020 2020  me  |.|         
+00003bf0: 2020 2020 2020 2020 207c 2069 7320 7468           | is th
+00003c00: 6520 7265 6769 7374 7279 206e 616d 6520  e registry name 
+00003c10: 7769 7468 6f75 7420 7468 6520 6465 636c  without the decl
+00003c20: 6172 6174 696f 6e20 7479 7065 2c20 616e  aration type, an
+00003c30: 6420 7769 7468 2020 207c 0a7c 2020 2020  d with   |.|    
+00003c40: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00003c50: 272e 2720 7265 706c 6163 6564 2077 6974  '.' replaced wit
+00003c60: 6820 275f 272e 2054 6869 7320 6174 7472  h '_'. This attr
+00003c70: 6962 7574 6520 6973 2061 6c73 6f20 7573  ibute is also us
+00003c80: 6564 2074 6f20 6d61 7020 616e 2020 7c0a  ed to map an  |.
+00003c90: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00003ca0: 2020 207c 2065 7869 7374 696e 6720 7461     | existing ta
+00003cb0: 626c 6520 6465 636c 6172 6564 2062 7920  ble declared by 
+00003cc0: 6120 7072 6576 696f 7573 204d 6f64 656c  a previous Model
+00003cd0: 2e20 416c 6c6f 7765 6420 7661 6c75 6573  . Allowed values
+00003ce0: 3a20 207c 0a7c 2020 2020 2020 2020 2020  :  |.|          
+00003cf0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d30: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+00003d40: 2020 2020 2020 2020 2020 2020 207c 202a               | *
+00003d50: 2073 7472 203a 3a20 2020 2020 2020 2020   str ::         
+00003d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d80: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003da0: 2020 7c20 6578 6973 7469 6e67 2074 6162    | existing tab
-00003db0: 6c65 2064 6563 6c61 7265 6420 6279 2061  le declared by a
-00003dc0: 2070 7265 7669 6f75 7320 4d6f 6465 6c2e   previous Model.
-00003dd0: 2041 6c6c 6f77 6564 2076 616c 7565 733a   Allowed values:
+00003da0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00003db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003de0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-00003df0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00003e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003df0: 2020 2020 2020 207c 2020 2020 4072 6567         |    @reg
+00003e00: 6973 7465 7228 4d6f 6465 6c2c 2074 6162  ister(Model, tab
+00003e10: 6c65 6e61 6d65 3d27 666f 6f27 2920 2020  lename='foo')   
 00003e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003e30: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-00003e40: 2020 2020 2020 2020 2020 2020 7c20 2a20              | * 
-00003e50: 7374 7220 3a3a 2020 2020 2020 2020 2020  str ::          
+00003e40: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00003e50: 2063 6c61 7373 2042 6172 3a20 2020 2020   class Bar:     
 00003e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003e80: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 00003e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ea0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00003ea0: 207c 2020 2020 2020 2020 7061 7373 2020   |        pass  
 00003eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003ee0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00003ef0: 2020 2020 2020 7c20 2020 2040 7265 6769        |    @regi
-00003f00: 7374 6572 284d 6f64 656c 2c20 7461 626c  ster(Model, tabl
-00003f10: 656e 616d 653d 2766 6f6f 2729 2020 2020  ename='foo')    
+00003ef0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00003f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003f30: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-00003f40: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00003f50: 636c 6173 7320 4261 723a 2020 2020 2020  class Bar:      
+00003f40: 2020 2020 2020 2020 2020 207c 202a 2064             | * d
+00003f50: 6563 6c61 7261 7469 6f6e 203a 3a20 2020  eclaration ::   
 00003f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003f80: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00003f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fa0: 7c20 2020 2020 2020 2070 6173 7320 2020  |        pass   
+00003fa0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00003fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003fe0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-00003ff0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00004000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ff0: 2020 2020 207c 2020 2020 4072 6567 6973       |    @regis
+00004000: 7465 7228 4d6f 6465 6c2c 2074 6162 6c65  ter(Model, table
+00004010: 6e61 6d65 3d4d 6f64 656c 2e46 6f6f 2920  name=Model.Foo) 
 00004020: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004030: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-00004040: 2020 2020 2020 2020 2020 7c20 2a20 6465            | * de
-00004050: 636c 6172 6174 696f 6e20 3a3a 2020 2020  claration ::    
+00004040: 2020 2020 2020 2020 2020 7c20 2020 2063            |    c
+00004050: 6c61 7373 2042 6172 3a20 2020 2020 2020  lass Bar:       
 00004060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004080: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00004090: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000040a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040a0: 2020 2020 2020 2020 7061 7373 2020 2020          pass    
 000040b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000040c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000040d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 000040e0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-000040f0: 2020 2020 7c20 2020 2040 7265 6769 7374      |    @regist
-00004100: 6572 284d 6f64 656c 2c20 7461 626c 656e  er(Model, tablen
-00004110: 616d 653d 4d6f 6465 6c2e 466f 6f29 2020  ame=Model.Foo)  
+000040f0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00004100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004110: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004130: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00004140: 2020 2020 2020 2020 207c 2020 2020 636c           |    cl
-00004150: 6173 7320 4261 723a 2020 2020 2020 2020  ass Bar:        
-00004160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004180: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00004190: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000041a0: 2020 2020 2020 2070 6173 7320 2020 2020         pass     
-000041b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041d0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00004130: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
+00004140: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+00004150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004180: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2069 676e  ---------+.| ign
+00004190: 6f72 655f 6d69 6772 6174 696f 6e20 7c20  ore_migration | 
+000041a0: 4966 2054 7275 6520 7468 656e 2074 6865  If True then the
+000041b0: 2074 6162 6c65 2077 696c 6c20 6e6f 7420   table will not 
+000041c0: 6265 2061 6c74 6572 6564 2069 6620 7468  be altered if th
+000041d0: 6520 6465 6669 6e69 7469 6f6e 2020 7c0a  e definition  |.
 000041e0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000041f0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00004200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004230: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-00004240: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00004250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004280: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 6967 6e6f  --------+.| igno
-00004290: 7265 5f6d 6967 7261 7469 6f6e 207c 2049  re_migration | I
-000042a0: 6620 5472 7565 2074 6865 6e20 7468 6520  f True then the 
-000042b0: 7461 626c 6520 7769 6c6c 206e 6f74 2062  table will not b
-000042c0: 6520 616c 7465 7265 6420 6966 2074 6865  e altered if the
-000042d0: 2064 6566 696e 6974 696f 6e20 207c 0a7c   definition  |.|
+000041f0: 2020 207c 206f 6620 7468 6520 6d6f 6465     | of the mode
+00004200: 6c20 616e 6420 7468 6520 7363 6865 6d61  l and the schema
+00004210: 2069 6e20 7468 6520 6461 7461 6261 7365   in the database
+00004220: 2061 7265 2064 6966 6572 656e 7473 203a   are diferents :
+00004230: 3a20 207c 0a7c 2020 2020 2020 2020 2020  :  |.|          
+00004240: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00004250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004280: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+00004290: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+000042a0: 2020 4072 6567 6973 7465 7228 4d6f 6465    @register(Mode
+000042b0: 6c2c 2069 676e 6f72 655f 6d69 6772 6174  l, ignore_migrat
+000042c0: 696f 6e3d 5472 7565 2920 2020 2020 2020  ion=True)       
+000042d0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 000042e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042f0: 2020 7c20 6f66 2074 6865 206d 6f64 656c    | of the model
-00004300: 2061 6e64 2074 6865 2073 6368 656d 6120   and the schema 
-00004310: 696e 2074 6865 2064 6174 6162 6173 6520  in the database 
-00004320: 6172 6520 6469 6665 7265 6e74 7320 3a3a  are diferents ::
+000042f0: 2020 7c20 2020 2063 6c61 7373 2046 6f6f    |    class Foo
+00004300: 3a20 2020 2020 2020 2020 2020 2020 2020  :               
+00004310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004320: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004330: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00004340: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00004350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004350: 7061 7373 2020 2020 2020 2020 2020 2020  pass            
 00004360: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004380: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00004390: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-000043a0: 2040 7265 6769 7374 6572 284d 6f64 656c   @register(Model
-000043b0: 2c20 6967 6e6f 7265 5f6d 6967 7261 7469  , ignore_migrati
-000043c0: 6f6e 3d54 7275 6529 2020 2020 2020 2020  on=True)        
-000043d0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-000043e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043f0: 207c 2020 2020 636c 6173 7320 466f 6f3a   |    class Foo:
-00004400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004430: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00004440: 2020 2020 2020 7c20 2020 2020 2020 2070        |        p
-00004450: 6173 7320 2020 2020 2020 2020 2020 2020  ass             
-00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004480: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-00004490: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-000044a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044d0: 2020 2020 2020 2020 2020 207c 0a2b 2d2d             |.+--
-000044e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000044f0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00004500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004530: 2b0a 0a2e 2e20 7761 726e 696e 673a 3a0a  +.... warning::.
-00004540: 0a20 2020 204d 6f64 656c 2063 616e 206f  .    Model can o
-00004550: 6e6c 7920 696e 6865 7269 7420 7369 6d70  nly inherit simp
-00004560: 6c65 2070 7974 686f 6e20 636c 6173 732c  le python class,
-00004570: 204d 6978 696e 206f 7220 4d6f 6465 6c2e   Mixin or Model.
-00004580: 0a0a 0a4e 6f6e 2053 514c 204d 6f64 656c  ...Non SQL Model
-00004590: 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a  .~~~~~~~~~~~~~..
-000045a0: 5468 6973 2069 7320 7468 6520 6465 6661  This is the defa
-000045b0: 756c 7420 6d6f 6465 6c2e 2054 6869 7320  ult model. This 
-000045c0: 6d6f 6465 6c20 6861 7320 6e6f 2074 6162  model has no tab
-000045d0: 6c65 732e 2049 7420 6973 2075 7365 6420  les. It is used 
-000045e0: 746f 0a6f 7267 616e 697a 6520 7468 6520  to.organize the 
-000045f0: 7265 6769 7374 7279 206f 7220 666f 7220  registry or for 
-00004600: 7370 6563 6966 6963 2070 726f 6365 7373  specific process
-00004610: 2e3a 3a0a 0a20 2020 2040 7265 6769 7374  .::..    @regist
-00004620: 6572 284d 6f64 656c 290a 2020 2020 636c  er(Model).    cl
-00004630: 6173 7320 466f 6f3a 0a20 2020 2020 2020  ass Foo:.       
-00004640: 2070 6173 730a 0a53 514c 204d 6f64 656c   pass..SQL Model
-00004650: 0a7e 7e7e 7e7e 7e7e 7e7e 0a0a 4120 6060  .~~~~~~~~~..A ``
-00004660: 5351 4c20 4d6f 6465 6c60 6020 6973 2061  SQL Model`` is a
-00004670: 2073 696d 706c 6520 6060 4d6f 6465 6c60   simple ``Model`
-00004680: 6020 7769 7468 2060 6043 6f6c 756d 6e60  ` with ``Column`
-00004690: 6020 6f72 2060 6052 656c 6174 696f 6e53  ` or ``RelationS
-000046a0: 6869 7060 602e 2046 6f72 0a65 6163 6820  hip``. For.each 
-000046b0: 6d6f 6465 6c2c 206f 6e65 2074 6162 6c65  model, one table
-000046c0: 2077 696c 6c20 6265 2063 7265 6174 6564   will be created
-000046d0: 2e3a 3a0a 0a20 2020 2040 7265 6769 7374  .::..    @regist
-000046e0: 6572 284d 6f64 656c 290a 2020 2020 636c  er(Model).    cl
-000046f0: 6173 7320 466f 6f3a 0a20 2020 2020 2020  ass Foo:.       
-00004700: 2023 2053 514c 204d 6f64 656c 2077 6974   # SQL Model wit
-00004710: 6820 6d61 7070 6564 2077 6974 6820 7468  h mapped with th
-00004720: 6520 7461 626c 6520 6060 666f 6f60 600a  e table ``foo``.
-00004730: 0a20 2020 2020 2020 2069 6420 3d20 496e  .        id = In
-00004740: 7465 6765 7228 7072 696d 6172 795f 6b65  teger(primary_ke
-00004750: 793d 5472 7565 290a 2020 2020 2020 2020  y=True).        
-00004760: 2320 6964 2069 7320 6120 636f 6c75 6d6e  # id is a column
-00004770: 206f 6e20 7468 6520 7461 626c 6520 6060   on the table ``
-00004780: 666f 6f60 600a 0a2e 2e20 7761 726e 696e  foo``.... warnin
-00004790: 673a 3a20 4561 6368 2053 514c 204d 6f64  g:: Each SQL Mod
-000047a0: 656c 2068 6176 6520 746f 2068 6176 6520  el have to have 
-000047b0: 676f 7420 6f6e 6520 6f72 206d 6f72 6520  got one or more 
-000047c0: 7072 696d 6172 7920 6b65 790a 0a49 6e20  primary key..In 
-000047d0: 7468 6520 6361 7365 206f 7220 796f 7520  the case or you 
-000047e0: 6e65 6564 2074 6f20 6164 6420 736f 6d65  need to add some
-000047f0: 2063 6f6e 6669 6775 7261 7469 6f6e 2069   configuration i
-00004800: 6e20 7468 6520 5351 4c41 6c63 6865 6d79  n the SQLAlchemy
-00004810: 2063 6c61 7373 0a61 7474 7269 6e75 7465   class.attrinute
-00004820: 3a0a 0a2a 205f 5f74 6162 6c65 5f61 7267  :..* __table_arg
-00004830: 735c 5f5c 5f0a 2a20 5f5f 7461 626c 655f  s\_\_.* __table_
-00004840: 6b77 6172 6773 5c5f 5c5f 0a2a 205f 5f6d  kwargs\_\_.* __m
-00004850: 6170 7065 725f 6172 6773 5c5f 5c5f 0a0a  apper_args\_\_..
-00004860: 796f 7520 6361 6e20 7573 6520 7468 6520  you can use the 
-00004870: 6e65 7874 2063 6c61 7373 206d 6574 686f  next class metho
-00004880: 6473 0a0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ds..+-----------
-00004890: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-000048a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000048b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000048c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000048d0: 2d2d 2d2b 0a7c 206d 6574 686f 6420 2020  ---+.| method   
-000048e0: 2020 2020 2020 2020 2020 207c 2064 6573             | des
-000048f0: 6372 6970 7469 6f6e 2020 2020 2020 2020  cription        
-00004900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004920: 2020 2020 7c0a 2b3d 3d3d 3d3d 3d3d 3d3d      |.+=========
-00004930: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d  ============+===
-00004940: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00004950: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00004960: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00004970: 3d3d 3d3d 3d2b 0a7c 205f 5f64 625f 7363  =====+.| __db_sc
-00004980: 6865 6d61 5f5f 2020 2020 2020 207c 2053  hema__       | S
-00004990: 696d 706c 6520 6174 7472 6962 7574 6520  imple attribute 
-000049a0: 746f 2064 6566 696e 6520 7468 6520 6e61  to define the na
-000049b0: 6d65 206f 6620 7468 6520 7363 6865 6d61  me of the schema
-000049c0: 2069 6e20 2020 7c0a 7c20 2020 2020 2020   in   |.|       
-000049d0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000049e0: 7768 6963 6820 7468 6520 6d6f 6465 6c2d  which the model-
-000049f0: 7265 6c61 7465 6420 7461 626c 6520 6973  related table is
-00004a00: 206c 6f63 6174 6564 2020 2020 2020 2020   located        
-00004a10: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
-00004a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00004a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004a60: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 6465 6669  --------+.| defi
-00004a70: 6e65 5f74 6162 6c65 5f61 7267 7320 2020  ne_table_args   
-00004a80: 7c20 4164 6420 6f70 7469 6f6e 7320 666f  | Add options fo
-00004a90: 7220 5351 4c41 6c63 6865 6d79 2074 6162  r SQLAlchemy tab
-00004aa0: 6c65 2062 7569 6c64 3a20 2020 2020 2020  le build:       
-00004ab0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00004ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ad0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+000043a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043d0: 2020 2020 2020 2020 2020 2020 7c0a 2b2d              |.+-
+000043e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000043f0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+00004400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004430: 2d2b 0a0a 2e2e 2077 6172 6e69 6e67 3a3a  -+.... warning::
+00004440: 0a0a 2020 2020 4d6f 6465 6c20 6361 6e20  ..    Model can 
+00004450: 6f6e 6c79 2069 6e68 6572 6974 2073 696d  only inherit sim
+00004460: 706c 6520 7079 7468 6f6e 2063 6c61 7373  ple python class
+00004470: 2c20 4d69 7869 6e20 6f72 204d 6f64 656c  , Mixin or Model
+00004480: 2e0a 0a0a 4e6f 6e20 5351 4c20 4d6f 6465  ....Non SQL Mode
+00004490: 6c0a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a  l.~~~~~~~~~~~~~.
+000044a0: 0a54 6869 7320 6973 2074 6865 2064 6566  .This is the def
+000044b0: 6175 6c74 206d 6f64 656c 2e20 5468 6973  ault model. This
+000044c0: 206d 6f64 656c 2068 6173 206e 6f20 7461   model has no ta
+000044d0: 626c 6573 2e20 4974 2069 7320 7573 6564  bles. It is used
+000044e0: 2074 6f0a 6f72 6761 6e69 7a65 2074 6865   to.organize the
+000044f0: 2072 6567 6973 7472 7920 6f72 2066 6f72   registry or for
+00004500: 2073 7065 6369 6669 6320 7072 6f63 6573   specific proces
+00004510: 732e 3a3a 0a0a 2020 2020 4072 6567 6973  s.::..    @regis
+00004520: 7465 7228 4d6f 6465 6c29 0a20 2020 2063  ter(Model).    c
+00004530: 6c61 7373 2046 6f6f 3a0a 2020 2020 2020  lass Foo:.      
+00004540: 2020 7061 7373 0a0a 5351 4c20 4d6f 6465    pass..SQL Mode
+00004550: 6c0a 7e7e 7e7e 7e7e 7e7e 7e0a 0a41 2060  l.~~~~~~~~~..A `
+00004560: 6053 514c 204d 6f64 656c 6060 2069 7320  `SQL Model`` is 
+00004570: 6120 7369 6d70 6c65 2060 604d 6f64 656c  a simple ``Model
+00004580: 6060 2077 6974 6820 6060 436f 6c75 6d6e  `` with ``Column
+00004590: 6060 206f 7220 6060 5265 6c61 7469 6f6e  `` or ``Relation
+000045a0: 5368 6970 6060 2e20 466f 720a 6561 6368  Ship``. For.each
+000045b0: 206d 6f64 656c 2c20 6f6e 6520 7461 626c   model, one tabl
+000045c0: 6520 7769 6c6c 2062 6520 6372 6561 7465  e will be create
+000045d0: 642e 3a3a 0a0a 2020 2020 4072 6567 6973  d.::..    @regis
+000045e0: 7465 7228 4d6f 6465 6c29 0a20 2020 2063  ter(Model).    c
+000045f0: 6c61 7373 2046 6f6f 3a0a 2020 2020 2020  lass Foo:.      
+00004600: 2020 2320 5351 4c20 4d6f 6465 6c20 7769    # SQL Model wi
+00004610: 7468 206d 6170 7065 6420 7769 7468 2074  th mapped with t
+00004620: 6865 2074 6162 6c65 2060 6066 6f6f 6060  he table ``foo``
+00004630: 0a0a 2020 2020 2020 2020 6964 203d 2049  ..        id = I
+00004640: 6e74 6567 6572 2870 7269 6d61 7279 5f6b  nteger(primary_k
+00004650: 6579 3d54 7275 6529 0a20 2020 2020 2020  ey=True).       
+00004660: 2023 2069 6420 6973 2061 2063 6f6c 756d   # id is a colum
+00004670: 6e20 6f6e 2074 6865 2074 6162 6c65 2060  n on the table `
+00004680: 6066 6f6f 6060 0a0a 2e2e 2077 6172 6e69  `foo``.... warni
+00004690: 6e67 3a3a 2045 6163 6820 5351 4c20 4d6f  ng:: Each SQL Mo
+000046a0: 6465 6c20 6861 7665 2074 6f20 6861 7665  del have to have
+000046b0: 2067 6f74 206f 6e65 206f 7220 6d6f 7265   got one or more
+000046c0: 2070 7269 6d61 7279 206b 6579 0a0a 496e   primary key..In
+000046d0: 2074 6865 2063 6173 6520 6f72 2079 6f75   the case or you
+000046e0: 206e 6565 6420 746f 2061 6464 2073 6f6d   need to add som
+000046f0: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+00004700: 696e 2074 6865 2053 514c 416c 6368 656d  in the SQLAlchem
+00004710: 7920 636c 6173 730a 6174 7472 696e 7574  y class.attrinut
+00004720: 653a 0a0a 2a20 5f5f 7461 626c 655f 6172  e:..* __table_ar
+00004730: 6773 5c5f 5c5f 0a2a 205f 5f74 6162 6c65  gs\_\_.* __table
+00004740: 5f6b 7761 7267 735c 5f5c 5f0a 2a20 5f5f  _kwargs\_\_.* __
+00004750: 6d61 7070 6572 5f61 7267 735c 5f5c 5f0a  mapper_args\_\_.
+00004760: 0a79 6f75 2063 616e 2075 7365 2074 6865  .you can use the
+00004770: 206e 6578 7420 636c 6173 7320 6d65 7468   next class meth
+00004780: 6f64 730a 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d  ods..+----------
+00004790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+000047a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000047b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000047c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000047d0: 2d2d 2d2d 2b0a 7c20 6d65 7468 6f64 2020  ----+.| method  
+000047e0: 2020 2020 2020 2020 2020 2020 7c20 6465              | de
+000047f0: 7363 7269 7074 696f 6e20 2020 2020 2020  scription       
+00004800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004820: 2020 2020 207c 0a2b 3d3d 3d3d 3d3d 3d3d       |.+========
+00004830: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d  =============+==
+00004840: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004850: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004860: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004870: 3d3d 3d3d 3d3d 2b0a 7c20 5f5f 6462 5f73  ======+.| __db_s
+00004880: 6368 656d 615f 5f20 2020 2020 2020 7c20  chema__       | 
+00004890: 5369 6d70 6c65 2061 7474 7269 6275 7465  Simple attribute
+000048a0: 2074 6f20 6465 6669 6e65 2074 6865 206e   to define the n
+000048b0: 616d 6520 6f66 2074 6865 2073 6368 656d  ame of the schem
+000048c0: 6120 696e 2020 207c 0a7c 2020 2020 2020  a in   |.|      
+000048d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000048e0: 2077 6869 6368 2074 6865 206d 6f64 656c   which the model
+000048f0: 2d72 656c 6174 6564 2074 6162 6c65 2069  -related table i
+00004900: 7320 6c6f 6361 7465 6420 2020 2020 2020  s located       
+00004910: 2020 2020 2020 2020 7c0a 2b2d 2d2d 2d2d          |.+-----
+00004920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004930: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
+00004940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004960: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2064 6566  ---------+.| def
+00004970: 696e 655f 7461 626c 655f 6172 6773 2020  ine_table_args  
+00004980: 207c 2041 6464 206f 7074 696f 6e73 2066   | Add options f
+00004990: 6f72 2053 514c 416c 6368 656d 7920 7461  or SQLAlchemy ta
+000049a0: 626c 6520 6275 696c 643a 2020 2020 2020  ble build:      
+000049b0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+000049c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049d0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+000049e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a00: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00004a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a20: 2020 207c 202a 2043 6f6e 7374 7261 696e     | * Constrain
+00004a30: 7473 206f 6e20 6d75 6c74 6970 6c65 2063  ts on multiple c
+00004a40: 6f6c 756d 6e73 2020 2020 2020 2020 2020  olumns          
+00004a50: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a70: 2020 2020 7c20 2a20 2e2e 2e20 2020 2020      | * ...     
+00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004aa0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00004ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ac0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00004ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b00: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
-00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b20: 2020 7c20 2a20 436f 6e73 7472 6169 6e74    | * Constraint
-00004b30: 7320 6f6e 206d 756c 7469 706c 6520 636f  s on multiple co
-00004b40: 6c75 6d6e 7320 2020 2020 2020 2020 2020  lumns           
-00004b50: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-00004b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b70: 2020 207c 202a 202e 2e2e 2020 2020 2020     | * ...      
+00004af0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00004b00: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00004b10: 2020 2020 2020 7c20 3a3a 2020 2020 2020        | ::      
+00004b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b40: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00004b50: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00004b60: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+00004b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ba0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00004bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bc0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00004ba0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00004bb0: 2020 2020 2020 2020 7c20 2020 2020 4063          |     @c
+00004bc0: 6c61 7373 6d65 7468 6f64 2020 2020 2020  lassmethod      
 00004bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bf0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c10: 2020 2020 207c 203a 3a20 2020 2020 2020       | ::       
-00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bf0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00004c00: 2020 2020 2020 2020 207c 2020 2020 2064           |     d
+00004c10: 6566 2064 6566 696e 655f 7461 626c 655f  ef define_table_
+00004c20: 6172 6773 2863 6c73 293a 2020 2020 2020  args(cls):      
 00004c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c40: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00004c50: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00004c60: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00004c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c90: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00004ca0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00004cb0: 2020 2020 2020 207c 2020 2020 2040 636c         |     @cl
-00004cc0: 6173 736d 6574 686f 6420 2020 2020 2020  assmethod       
+00004c40: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+00004c50: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00004c60: 2020 2020 7265 7320 3d20 7375 7065 7228      res = super(
+00004c70: 4d79 4d6f 6465 6c2c 2063 6c73 292e 6465  MyModel, cls).de
+00004c80: 6669 6e65 5f74 6162 6c65 5f61 7267 7328  fine_table_args(
+00004c90: 2920 207c 0a7c 2020 2020 2020 2020 2020  )  |.|          
+00004ca0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+00004cb0: 2020 2020 2072 6574 7572 6e20 7265 7320       return res 
+00004cc0: 2b20 6d79 5f74 7570 6c65 5f76 616c 7565  + my_tuple_value
 00004cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cf0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-00004d00: 2020 2020 2020 2020 7c20 2020 2020 6465          |     de
-00004d10: 6620 6465 6669 6e65 5f74 6162 6c65 5f61  f define_table_a
-00004d20: 7267 7328 636c 7329 3a20 2020 2020 2020  rgs(cls):       
-00004d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d40: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00004d50: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00004d60: 2020 2072 6573 203d 2073 7570 6572 284d     res = super(M
-00004d70: 794d 6f64 656c 2c20 636c 7329 2e64 6566  yModel, cls).def
-00004d80: 696e 655f 7461 626c 655f 6172 6773 2829  ine_table_args()
-00004d90: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-00004da0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00004db0: 2020 2020 7265 7475 726e 2072 6573 202b      return res +
-00004dc0: 206d 795f 7475 706c 655f 7661 6c75 6520   my_tuple_value 
-00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004de0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-00004df0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+00004ce0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+00004cf0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00004d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d30: 2020 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d       |.+--------
+00004d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00004d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004d80: 2d2d 2d2d 2d2d 2b0a 7c20 6465 6669 6e65  ------+.| define
+00004d90: 5f74 6162 6c65 5f6b 7761 7267 7320 7c20  _table_kwargs | 
+00004da0: 4164 6420 6e61 6d65 6420 6f70 7469 6f6e  Add named option
+00004db0: 7320 666f 7220 5351 4c41 6c63 6865 6d79  s for SQLAlchemy
+00004dc0: 2074 6162 6c65 2062 7569 6c64 3a20 2020   table build:   
+00004dd0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+00004de0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00004df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e30: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
-00004e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-00004e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004e80: 2d2d 2d2d 2d2b 0a7c 2064 6566 696e 655f  -----+.| define_
-00004e90: 7461 626c 655f 6b77 6172 6773 207c 2041  table_kwargs | A
-00004ea0: 6464 206e 616d 6564 206f 7074 696f 6e73  dd named options
-00004eb0: 2066 6f72 2053 514c 416c 6368 656d 7920   for SQLAlchemy 
-00004ec0: 7461 626c 6520 6275 696c 643a 2020 2020  table build:    
-00004ed0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-00004ee0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00004ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e20: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+00004e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e40: 7c20 3a3a 2020 2020 2020 2020 2020 2020  | ::            
+00004e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e70: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
+00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e90: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00004ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ec0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+00004ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ee0: 2020 7c20 2020 2020 4063 6c61 7373 6d65    |     @classme
+00004ef0: 7468 6f64 2020 2020 2020 2020 2020 2020  thod            
 00004f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f20: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-00004f30: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00004f40: 203a 3a20 2020 2020 2020 2020 2020 2020   ::             
-00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f70: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-00004f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f90: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00004fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fc0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00004fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fe0: 207c 2020 2020 2040 636c 6173 736d 6574   |     @classmet
-00004ff0: 686f 6420 2020 2020 2020 2020 2020 2020  hod             
-00005000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005010: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
-00005020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005030: 2020 7c20 2020 2020 6465 6620 6465 6669    |     def defi
-00005040: 6e65 5f74 6162 6c65 5f6b 7761 7267 7328  ne_table_kwargs(
-00005050: 636c 7329 3a20 2020 2020 2020 2020 2020  cls):           
-00005060: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-00005070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005080: 2020 207c 2020 2020 2020 2020 2072 6573     |         res
-00005090: 203d 2073 7570 6572 284d 794d 6f64 656c   = super(MyModel
-000050a0: 2c20 636c 7329 2e64 6566 696e 655f 7461  , cls).define_ta
-000050b0: 626c 655f 6b77 6172 6773 2829 7c0a 7c20  ble_kwargs()|.| 
-000050c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050d0: 2020 2020 7c20 2020 2020 2020 2020 7265      |         re
-000050e0: 732e 7570 6461 7465 286d 795f 7475 706c  s.update(my_tupl
-000050f0: 655f 7661 6c75 6529 2020 2020 2020 2020  e_value)        
-00005100: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00005110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005120: 2020 2020 207c 2020 2020 2020 2020 2072       |         r
-00005130: 6574 7572 6e20 7265 7320 2020 2020 2020  eturn res       
-00005140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005150: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00005160: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00005170: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00004f10: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00004f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f30: 2020 207c 2020 2020 2064 6566 2064 6566     |     def def
+00004f40: 696e 655f 7461 626c 655f 6b77 6172 6773  ine_table_kwargs
+00004f50: 2863 6c73 293a 2020 2020 2020 2020 2020  (cls):          
+00004f60: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00004f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f80: 2020 2020 7c20 2020 2020 2020 2020 7265      |         re
+00004f90: 7320 3d20 7375 7065 7228 4d79 4d6f 6465  s = super(MyMode
+00004fa0: 6c2c 2063 6c73 292e 6465 6669 6e65 5f74  l, cls).define_t
+00004fb0: 6162 6c65 5f6b 7761 7267 7328 297c 0a7c  able_kwargs()|.|
+00004fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fd0: 2020 2020 207c 2020 2020 2020 2020 2072       |         r
+00004fe0: 6573 2e75 7064 6174 6528 6d79 5f74 7570  es.update(my_tup
+00004ff0: 6c65 5f76 616c 7565 2920 2020 2020 2020  le_value)       
+00005000: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00005010: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00005020: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00005030: 7265 7475 726e 2072 6573 2020 2020 2020  return res      
+00005040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005050: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00005060: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00005070: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+00005080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050b0: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.+-------------
+000050c0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+000050d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000050e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000050f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005100: 2d2b 0a7c 2064 6566 696e 655f 6d61 7070  -+.| define_mapp
+00005110: 6572 5f61 7267 7320 207c 2041 6464 206f  er_args  | Add o
+00005120: 7074 696f 6e73 2066 6f72 2053 514c 416c  ptions for SQLAl
+00005130: 6368 656d 7920 6d61 7070 6572 7320 6275  chemy mappers bu
+00005140: 696c 643a 2020 2020 2020 2020 2020 2020  ild:            
+00005150: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+00005160: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00005170: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005180: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000051b0: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
-000051c0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-000051d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000051e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000051f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005200: 2b0a 7c20 6465 6669 6e65 5f6d 6170 7065  +.| define_mappe
-00005210: 725f 6172 6773 2020 7c20 4164 6420 6f70  r_args  | Add op
-00005220: 7469 6f6e 7320 666f 7220 5351 4c41 6c63  tions for SQLAlc
-00005230: 6865 6d79 206d 6170 7065 7273 2062 7569  hemy mappers bui
-00005240: 6c64 3a20 2020 2020 2020 2020 2020 2020  ld:             
-00005250: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00005260: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+000051a0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+000051b0: 2020 2020 2020 2020 2020 207c 202a 2070             | * p
+000051c0: 6f6c 796d 6f72 7068 6973 6d20 2020 2020  olymorphism     
+000051d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051f0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+00005200: 2020 2020 2020 2020 2020 2020 7c20 2a20              | * 
+00005210: 2e2e 2e20 2020 2020 2020 2020 2020 2020  ...             
+00005220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005240: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+00005250: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005270: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052a0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-000052b0: 2020 2020 2020 2020 2020 7c20 2a20 706f            | * po
-000052c0: 6c79 6d6f 7270 6869 736d 2020 2020 2020  lymorphism      
+00005290: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+000052a0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000052b0: 3a3a 2020 2020 2020 2020 2020 2020 2020  ::              
+000052c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000052d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052f0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-00005300: 2020 2020 2020 2020 2020 207c 202a 202e             | * .
-00005310: 2e2e 2020 2020 2020 2020 2020 2020 2020  ..              
+000052e0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+000052f0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00005300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005310: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005340: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00005350: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00005360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005330: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+00005340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005350: 7c20 2020 2020 4063 6c61 7373 6d65 7468  |     @classmeth
+00005360: 6f64 2020 2020 2020 2020 2020 2020 2020  od              
 00005370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005390: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-000053a0: 2020 2020 2020 2020 2020 2020 207c 203a               | :
-000053b0: 3a20 2020 2020 2020 2020 2020 2020 2020  :               
-000053c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053e0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-000053f0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00005400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005380: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
+00005390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053a0: 207c 2020 2020 2064 6566 2064 6566 696e   |     def defin
+000053b0: 655f 6d61 7070 6572 5f61 7267 7328 636c  e_mapper_args(cl
+000053c0: 7329 3a20 2020 2020 2020 2020 2020 2020  s):             
+000053d0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+000053e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053f0: 2020 7c20 2020 2020 2020 2020 7265 7475    |         retu
+00005400: 726e 206d 795f 6469 6374 5f76 616c 7565  rn my_dict_value
 00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005430: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-00005440: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00005450: 2020 2020 2040 636c 6173 736d 6574 686f       @classmetho
-00005460: 6420 2020 2020 2020 2020 2020 2020 2020  d               
-00005470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005480: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-00005490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054a0: 7c20 2020 2020 6465 6620 6465 6669 6e65  |     def define
-000054b0: 5f6d 6170 7065 725f 6172 6773 2863 6c73  _mapper_args(cls
-000054c0: 293a 2020 2020 2020 2020 2020 2020 2020  ):              
-000054d0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-000054e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054f0: 207c 2020 2020 2020 2020 2072 6574 7572   |         retur
-00005500: 6e20 6d79 5f64 6963 745f 7661 6c75 6520  n my_dict_value 
-00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005520: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
-00005530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005540: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00005550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005570: 2020 2020 2020 2020 2020 207c 0a2b 2d2d             |.+--
-00005580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005590: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-000055a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000055b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000055c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 0a2e  ------------+...
-000055d0: 2e20 6e6f 7465 3a3a 0a0a 2020 2020 4e65  . note::..    Ne
-000055e0: 7720 696e 2030 2e34 2e30 0a0a 5669 6577  w in 0.4.0..View
-000055f0: 204d 6f64 656c 0a7e 7e7e 7e7e 7e7e 7e7e   Model.~~~~~~~~~
-00005600: 7e0a 0a41 2060 6056 6965 7720 4d6f 6465  ~..A ``View Mode
-00005610: 6c60 6020 6173 2060 6053 514c 204d 6f64  l`` as ``SQL Mod
-00005620: 656c 6060 2e20 4e65 6564 2074 6865 2064  el``. Need the d
-00005630: 6563 6c61 7261 7469 6f6e 206f 6620 6060  eclaration of ``
-00005640: 436f 6c75 6d6e 6060 2061 6e64 202f 206f  Column`` and / o
-00005650: 720a 6060 5265 6c61 7469 6f6e 5368 6970  r.``RelationShip
-00005660: 6060 2e20 496e 2074 6865 2060 6072 6567  ``. In the ``reg
-00005670: 6973 7465 7260 6020 7468 6520 7061 7261  ister`` the para
-00005680: 6d20 6060 6661 6374 6f72 7960 6020 6d75  m ``factory`` mu
-00005690: 7374 2062 650a 6060 616e 7962 6c6f 6b2e  st be.``anyblok.
-000056a0: 6d6f 6465 6c2e 6661 6374 6f72 792e 5669  model.factory.Vi
-000056b0: 6577 4661 6374 6f72 7960 6020 616e 6420  ewFactory`` and 
-000056c0: 7468 6520 6060 5669 6577 204d 6f64 656c  the ``View Model
-000056d0: 6060 206d 7573 7420 6465 6669 6e65 2074  `` must define t
-000056e0: 6865 0a60 6073 716c 616c 6368 656d 795f  he.``sqlalchemy_
-000056f0: 7669 6577 5f64 6563 6c61 7261 7469 6f6e  view_declaration
-00005700: 6060 2063 6c61 7373 6d65 7468 6f64 2e3a  `` classmethod.:
-00005710: 3a0a 0a20 2020 2066 726f 6d20 616e 7962  :..    from anyb
-00005720: 6c6f 6b2e 6d6f 6465 6c2e 6661 6374 6f72  lok.model.factor
-00005730: 7920 696d 706f 7274 2056 6965 7746 6163  y import ViewFac
-00005740: 746f 7279 0a0a 2020 2020 4072 6567 6973  tory..    @regis
-00005750: 7465 7228 4d6f 6465 6c2c 2066 6163 746f  ter(Model, facto
-00005760: 7279 3d56 6965 7746 6163 746f 7279 290a  ry=ViewFactory).
-00005770: 2020 2020 636c 6173 7320 466f 6f3a 0a0a      class Foo:..
-00005780: 2020 2020 2020 2020 6964 203d 2049 6e74          id = Int
-00005790: 6567 6572 2870 7269 6d61 7279 5f6b 6579  eger(primary_key
-000057a0: 3d54 7275 6529 0a20 2020 2020 2020 206e  =True).        n
-000057b0: 616d 6520 3d20 5374 7269 6e67 2829 0a0a  ame = String()..
-000057c0: 2020 2020 2020 2020 4063 6c61 7373 6d65          @classme
-000057d0: 7468 6f64 0a20 2020 2020 2020 2064 6566  thod.        def
-000057e0: 2073 716c 616c 6368 656d 795f 7669 6577   sqlalchemy_view
-000057f0: 5f64 6563 6c61 7261 7469 6f6e 2863 6c73  _declaration(cls
-00005800: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
-00005810: 726f 6d20 7371 6c61 6c63 6865 6d79 2e73  rom sqlalchemy.s
-00005820: 716c 2069 6d70 6f72 7420 7365 6c65 6374  ql import select
-00005830: 0a20 2020 2020 2020 2020 2020 204d 6f64  .            Mod
-00005840: 656c 203d 2063 6c73 2e61 6e79 626c 6f6b  el = cls.anyblok
-00005850: 2e53 7973 7465 6d2e 4d6f 6465 6c0a 2020  .System.Model.  
-00005860: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00005870: 2073 656c 6563 7428 5b4d 6f64 656c 2e69   select([Model.i
-00005880: 642e 6c61 6265 6c28 2769 6427 292c 204d  d.label('id'), M
-00005890: 6f64 656c 2e6e 616d 652e 6c61 6265 6c28  odel.name.label(
-000058a0: 276e 616d 6527 295d 290a 0a60 6073 716c  'name')])..``sql
-000058b0: 616c 6368 656d 795f 7669 6577 5f64 6563  alchemy_view_dec
-000058c0: 6c61 7261 7469 6f6e 6060 206d 7573 7420  laration`` must 
-000058d0: 7265 7475 726e 2061 2073 656c 6563 7420  return a select 
-000058e0: 7175 6572 7920 636f 7272 6573 706f 6e64  query correspond
-000058f0: 696e 6720 746f 2074 6865 0a72 6571 7565  ing to the.reque
-00005900: 7374 206f 6620 7468 6520 5351 4c20 7669  st of the SQL vi
-00005910: 6577 2e0a 0a43 6f6c 756d 6e0a 2d2d 2d2d  ew...Column.----
-00005920: 2d2d 0a0a 546f 2064 6563 6c61 7265 2061  --..To declare a
-00005930: 2060 6043 6f6c 756d 6e60 6020 696e 2061   ``Column`` in a
-00005940: 206d 6f64 656c 2c20 6164 6420 6120 636f   model, add a co
-00005950: 6c75 6d6e 206f 6e20 7468 6520 7461 626c  lumn on the tabl
-00005960: 6520 6f66 2074 6865 206d 6f64 656c 2e3a  e of the model.:
-00005970: 3a0a 0a20 2020 2066 726f 6d20 616e 7962  :..    from anyb
-00005980: 6c6f 6b2e 6465 636c 6172 6174 696f 6e73  lok.declarations
-00005990: 2069 6d70 6f72 7420 4465 636c 6172 6174   import Declarat
-000059a0: 696f 6e73 0a20 2020 2066 726f 6d20 616e  ions.    from an
-000059b0: 7962 6c6f 6b2e 636f 6c75 6d6e 2069 6d70  yblok.column imp
-000059c0: 6f72 7420 496e 7465 6765 722c 2053 7472  ort Integer, Str
-000059d0: 696e 670a 0a0a 2020 2020 4044 6563 6c61  ing...    @Decla
-000059e0: 7261 7469 6f6e 732e 7265 6769 7374 6572  rations.register
-000059f0: 2844 6563 6c61 7261 7469 6f6e 2e4d 6f64  (Declaration.Mod
-00005a00: 656c 290a 2020 2020 636c 6173 7320 4d79  el).    class My
-00005a10: 4d6f 6465 6c3a 0a0a 2020 2020 2020 2020  Model:..        
-00005a20: 6964 203d 2049 6e74 6567 6572 2870 7269  id = Integer(pri
-00005a30: 6d61 7279 5f6b 6579 3d54 7275 6529 0a20  mary_key=True). 
-00005a40: 2020 2020 2020 206e 616d 6520 3d20 5374         name = St
-00005a50: 7269 6e67 2829 0a0a 2e2e 206e 6f74 653a  ring().... note:
-00005a60: 3a0a 0a20 2020 2053 696e 6365 2074 6865  :..    Since the
-00005a70: 2076 6572 7369 6f6e 2030 2e34 2e30 2074   version 0.4.0 t
-00005a80: 6865 2060 6043 6f6c 756d 6e73 6060 2061  he ``Columns`` a
-00005a90: 7265 206e 6f74 2060 6044 6563 6c61 7261  re not ``Declara
-00005aa0: 7469 6f6e 7360 600a 0a4c 6973 7420 6f66  tions``..List of
-00005ab0: 2074 6865 2063 6f6c 756d 6e20 7479 7065   the column type
-00005ac0: 3a0a 0a20 2a20 6060 4461 7465 5469 6d65  :.. * ``DateTime
-00005ad0: 6060 3a20 7573 6520 6461 7465 7469 6d65  ``: use datetime
-00005ae0: 2e64 6174 6574 696d 652c 2077 6974 6820  .datetime, with 
-00005af0: 7079 747a 2066 6f72 2074 6865 2074 696d  pytz for the tim
-00005b00: 657a 6f6e 650a 202a 2060 6054 696d 6553  ezone. * ``TimeS
-00005b10: 7461 6d70 6060 3a20 7573 6520 6461 7465  tamp``: use date
-00005b20: 7469 6d65 2e64 6174 6574 696d 652c 2077  time.datetime, w
-00005b30: 6974 6820 7079 747a 2066 6f72 2074 6865  ith pytz for the
-00005b40: 2074 696d 657a 6f6e 650a 202a 2060 6044   timezone. * ``D
-00005b50: 6563 696d 616c 6060 3a20 7573 6520 6465  ecimal``: use de
-00005b60: 6369 6d61 6c2e 4465 6369 6d61 6c0a 202a  cimal.Decimal. *
-00005b70: 2060 6046 6c6f 6174 6060 0a20 2a20 6060   ``Float``. * ``
-00005b80: 5469 6d65 6060 3a20 7573 6520 6461 7465  Time``: use date
-00005b90: 7469 6d65 2e74 696d 650a 202a 2060 6042  time.time. * ``B
-00005ba0: 6967 496e 7465 6765 7260 600a 202a 2060  igInteger``. * `
-00005bb0: 6042 6f6f 6c65 616e 6060 0a20 2a20 6060  `Boolean``. * ``
-00005bc0: 4461 7465 6060 3a20 7573 6520 6461 7465  Date``: use date
-00005bd0: 7469 6d65 2e64 6174 650a 202a 2060 6049  time.date. * ``I
-00005be0: 6e74 6567 6572 6060 0a20 2a20 6060 496e  nteger``. * ``In
-00005bf0: 7465 7276 616c 6060 3a20 7573 6520 6461  terval``: use da
-00005c00: 7465 7469 6d65 2e74 696d 6564 656c 7461  tetime.timedelta
-00005c10: 0a20 2a20 6060 4c61 7267 6542 696e 6172  . * ``LargeBinar
-00005c20: 7960 600a 202a 2060 6053 7472 696e 6760  y``. * ``String`
-00005c30: 600a 202a 2060 6054 6578 7460 600a 202a  `. * ``Text``. *
-00005c40: 2060 6053 656c 6563 7469 6f6e 6060 0a20   ``Selection``. 
-00005c50: 2a20 6060 456e 756d 6060 3a20 7573 6520  * ``Enum``: use 
-00005c60: 656e 756d 2e45 6e75 6d20 696e 6865 7269  enum.Enum inheri
-00005c70: 7465 6420 636c 6173 730a 202a 2060 604a  ted class. * ``J
-00005c80: 736f 6e60 600a 202a 2060 6053 6571 7565  son``. * ``Seque
-00005c90: 6e63 6560 600a 202a 2060 6043 6f6c 6f72  nce``. * ``Color
-00005ca0: 6060 3a20 7573 6520 636f 6c6f 7572 2e43  ``: use colour.C
-00005cb0: 6f6c 6f72 0a20 2a20 6060 5061 7373 776f  olor. * ``Passwo
-00005cc0: 7264 6060 3a20 7573 6520 7371 6c61 6c63  rd``: use sqlalc
-00005cd0: 6865 6d79 5f75 7469 6c73 2e74 7970 6573  hemy_utils.types
-00005ce0: 2e70 6173 7377 6f72 642e 5061 7373 776f  .password.Passwo
-00005cf0: 7264 0a20 2a20 6060 5555 4944 6060 3a20  rd. * ``UUID``: 
-00005d00: 7573 6520 7575 6964 0a20 2a20 6060 5552  use uuid. * ``UR
-00005d10: 4c60 603a 2075 7365 2066 7572 6c2e 6675  L``: use furl.fu
-00005d20: 726c 0a20 2a20 6060 5068 6f6e 654e 756d  rl. * ``PhoneNum
-00005d30: 6265 7260 603a 2075 7365 2073 716c 616c  ber``: use sqlal
-00005d40: 6368 656d 795f 7574 696c 732e 5068 6f6e  chemy_utils.Phon
-00005d50: 654e 756d 6265 720a 202a 2060 6045 6d61  eNumber. * ``Ema
-00005d60: 696c 6060 0a20 2a20 6060 436f 756e 7472  il``. * ``Countr
-00005d70: 7960 603a 2075 7365 2070 7963 6f75 6e74  y``: use pycount
-00005d80: 7279 0a0a 416c 6c20 7468 6520 636f 6c75  ry..All the colu
-00005d90: 6d6e 7320 6861 7665 2074 6865 2066 6f6c  mns have the fol
-00005da0: 6c6f 7769 6e67 206f 7074 696f 6e61 6c20  lowing optional 
-00005db0: 7061 7261 6d65 7465 7273 3a0a 0a2b 2d2d  parameters:..+--
-00005dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005dd0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00005de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
-00005e10: 2050 6172 616d 6574 6572 2020 2020 2020   Parameter      
-00005e20: 2020 7c20 4465 7363 7269 7074 696f 6e20    | Description 
-00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e50: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00005e60: 0a2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .+==============
-00005e70: 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d  ====+===========
-00005e80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005e90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005ea0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005eb0: 3d2b 0a7c 206c 6162 656c 2020 2020 2020  =+.| label      
-00005ec0: 2020 2020 2020 7c20 4c61 6265 6c20 6f66        | Label of
-00005ed0: 2074 6865 2063 6f6c 756d 6e2c 2049 6620   the column, If 
-00005ee0: 4e6f 6e65 2074 6865 206c 6162 656c 2069  None the label i
-00005ef0: 7320 7468 6520 6e61 6d65 206f 6620 2020  s the name of   
-00005f00: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-00005f10: 2020 2020 2020 2020 7c20 636f 6c75 6d6e          | column
-00005f20: 2063 6170 6974 616c 697a 6564 2020 2020   capitalized    
+00005420: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00005430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005440: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+00005450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005470: 2020 2020 2020 2020 2020 2020 7c0a 2b2d              |.+-
+00005480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005490: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+000054a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000054b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000054c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a  -------------+..
+000054d0: 2e2e 206e 6f74 653a 3a0a 0a20 2020 204e  .. note::..    N
+000054e0: 6577 2069 6e20 302e 342e 300a 0a56 6965  ew in 0.4.0..Vie
+000054f0: 7720 4d6f 6465 6c0a 7e7e 7e7e 7e7e 7e7e  w Model.~~~~~~~~
+00005500: 7e7e 0a0a 4120 6060 5669 6577 204d 6f64  ~~..A ``View Mod
+00005510: 656c 6060 2061 7320 6060 5351 4c20 4d6f  el`` as ``SQL Mo
+00005520: 6465 6c60 602e 204e 6565 6420 7468 6520  del``. Need the 
+00005530: 6465 636c 6172 6174 696f 6e20 6f66 2060  declaration of `
+00005540: 6043 6f6c 756d 6e60 6020 616e 6420 2f20  `Column`` and / 
+00005550: 6f72 0a60 6052 656c 6174 696f 6e53 6869  or.``RelationShi
+00005560: 7060 602e 2049 6e20 7468 6520 6060 7265  p``. In the ``re
+00005570: 6769 7374 6572 6060 2074 6865 2070 6172  gister`` the par
+00005580: 616d 2060 6066 6163 746f 7279 6060 206d  am ``factory`` m
+00005590: 7573 7420 6265 0a60 6061 6e79 626c 6f6b  ust be.``anyblok
+000055a0: 2e6d 6f64 656c 2e66 6163 746f 7279 2e56  .model.factory.V
+000055b0: 6965 7746 6163 746f 7279 6060 2061 6e64  iewFactory`` and
+000055c0: 2074 6865 2060 6056 6965 7720 4d6f 6465   the ``View Mode
+000055d0: 6c60 6020 6d75 7374 2064 6566 696e 6520  l`` must define 
+000055e0: 7468 650a 6060 7371 6c61 6c63 6865 6d79  the.``sqlalchemy
+000055f0: 5f76 6965 775f 6465 636c 6172 6174 696f  _view_declaratio
+00005600: 6e60 6020 636c 6173 736d 6574 686f 642e  n`` classmethod.
+00005610: 3a3a 0a0a 2020 2020 6672 6f6d 2061 6e79  ::..    from any
+00005620: 626c 6f6b 2e6d 6f64 656c 2e66 6163 746f  blok.model.facto
+00005630: 7279 2069 6d70 6f72 7420 5669 6577 4661  ry import ViewFa
+00005640: 6374 6f72 790a 0a20 2020 2040 7265 6769  ctory..    @regi
+00005650: 7374 6572 284d 6f64 656c 2c20 6661 6374  ster(Model, fact
+00005660: 6f72 793d 5669 6577 4661 6374 6f72 7929  ory=ViewFactory)
+00005670: 0a20 2020 2063 6c61 7373 2046 6f6f 3a0a  .    class Foo:.
+00005680: 0a20 2020 2020 2020 2069 6420 3d20 496e  .        id = In
+00005690: 7465 6765 7228 7072 696d 6172 795f 6b65  teger(primary_ke
+000056a0: 793d 5472 7565 290a 2020 2020 2020 2020  y=True).        
+000056b0: 6e61 6d65 203d 2053 7472 696e 6728 290a  name = String().
+000056c0: 0a20 2020 2020 2020 2040 636c 6173 736d  .        @classm
+000056d0: 6574 686f 640a 2020 2020 2020 2020 6465  ethod.        de
+000056e0: 6620 7371 6c61 6c63 6865 6d79 5f76 6965  f sqlalchemy_vie
+000056f0: 775f 6465 636c 6172 6174 696f 6e28 636c  w_declaration(cl
+00005700: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00005710: 6672 6f6d 2073 716c 616c 6368 656d 792e  from sqlalchemy.
+00005720: 7371 6c20 696d 706f 7274 2073 656c 6563  sql import selec
+00005730: 740a 2020 2020 2020 2020 2020 2020 4d6f  t.            Mo
+00005740: 6465 6c20 3d20 636c 732e 616e 7962 6c6f  del = cls.anyblo
+00005750: 6b2e 5379 7374 656d 2e4d 6f64 656c 0a20  k.System.Model. 
+00005760: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00005770: 6e20 7365 6c65 6374 285b 4d6f 6465 6c2e  n select([Model.
+00005780: 6964 2e6c 6162 656c 2827 6964 2729 2c20  id.label('id'), 
+00005790: 4d6f 6465 6c2e 6e61 6d65 2e6c 6162 656c  Model.name.label
+000057a0: 2827 6e61 6d65 2729 5d29 0a0a 6060 7371  ('name')])..``sq
+000057b0: 6c61 6c63 6865 6d79 5f76 6965 775f 6465  lalchemy_view_de
+000057c0: 636c 6172 6174 696f 6e60 6020 6d75 7374  claration`` must
+000057d0: 2072 6574 7572 6e20 6120 7365 6c65 6374   return a select
+000057e0: 2071 7565 7279 2063 6f72 7265 7370 6f6e   query correspon
+000057f0: 6469 6e67 2074 6f20 7468 650a 7265 7175  ding to the.requ
+00005800: 6573 7420 6f66 2074 6865 2053 514c 2076  est of the SQL v
+00005810: 6965 772e 0a0a 436f 6c75 6d6e 0a2d 2d2d  iew...Column.---
+00005820: 2d2d 2d0a 0a54 6f20 6465 636c 6172 6520  ---..To declare 
+00005830: 6120 6060 436f 6c75 6d6e 6060 2069 6e20  a ``Column`` in 
+00005840: 6120 6d6f 6465 6c2c 2061 6464 2061 2063  a model, add a c
+00005850: 6f6c 756d 6e20 6f6e 2074 6865 2074 6162  olumn on the tab
+00005860: 6c65 206f 6620 7468 6520 6d6f 6465 6c2e  le of the model.
+00005870: 3a3a 0a0a 2020 2020 6672 6f6d 2061 6e79  ::..    from any
+00005880: 626c 6f6b 2e64 6563 6c61 7261 7469 6f6e  blok.declaration
+00005890: 7320 696d 706f 7274 2044 6563 6c61 7261  s import Declara
+000058a0: 7469 6f6e 730a 2020 2020 6672 6f6d 2061  tions.    from a
+000058b0: 6e79 626c 6f6b 2e63 6f6c 756d 6e20 696d  nyblok.column im
+000058c0: 706f 7274 2049 6e74 6567 6572 2c20 5374  port Integer, St
+000058d0: 7269 6e67 0a0a 0a20 2020 2040 4465 636c  ring...    @Decl
+000058e0: 6172 6174 696f 6e73 2e72 6567 6973 7465  arations.registe
+000058f0: 7228 4465 636c 6172 6174 696f 6e2e 4d6f  r(Declaration.Mo
+00005900: 6465 6c29 0a20 2020 2063 6c61 7373 204d  del).    class M
+00005910: 794d 6f64 656c 3a0a 0a20 2020 2020 2020  yModel:..       
+00005920: 2069 6420 3d20 496e 7465 6765 7228 7072   id = Integer(pr
+00005930: 696d 6172 795f 6b65 793d 5472 7565 290a  imary_key=True).
+00005940: 2020 2020 2020 2020 6e61 6d65 203d 2053          name = S
+00005950: 7472 696e 6728 290a 0a2e 2e20 6e6f 7465  tring().... note
+00005960: 3a3a 0a0a 2020 2020 5369 6e63 6520 7468  ::..    Since th
+00005970: 6520 7665 7273 696f 6e20 302e 342e 3020  e version 0.4.0 
+00005980: 7468 6520 6060 436f 6c75 6d6e 7360 6020  the ``Columns`` 
+00005990: 6172 6520 6e6f 7420 6060 4465 636c 6172  are not ``Declar
+000059a0: 6174 696f 6e73 6060 0a0a 4c69 7374 206f  ations``..List o
+000059b0: 6620 7468 6520 636f 6c75 6d6e 2074 7970  f the column typ
+000059c0: 653a 0a0a 202a 2060 6044 6174 6554 696d  e:.. * ``DateTim
+000059d0: 6560 603a 2075 7365 2064 6174 6574 696d  e``: use datetim
+000059e0: 652e 6461 7465 7469 6d65 2c20 7769 7468  e.datetime, with
+000059f0: 2070 7974 7a20 666f 7220 7468 6520 7469   pytz for the ti
+00005a00: 6d65 7a6f 6e65 0a20 2a20 6060 5469 6d65  mezone. * ``Time
+00005a10: 5374 616d 7060 603a 2075 7365 2064 6174  Stamp``: use dat
+00005a20: 6574 696d 652e 6461 7465 7469 6d65 2c20  etime.datetime, 
+00005a30: 7769 7468 2070 7974 7a20 666f 7220 7468  with pytz for th
+00005a40: 6520 7469 6d65 7a6f 6e65 0a20 2a20 6060  e timezone. * ``
+00005a50: 4465 6369 6d61 6c60 603a 2075 7365 2064  Decimal``: use d
+00005a60: 6563 696d 616c 2e44 6563 696d 616c 0a20  ecimal.Decimal. 
+00005a70: 2a20 6060 466c 6f61 7460 600a 202a 2060  * ``Float``. * `
+00005a80: 6054 696d 6560 603a 2075 7365 2064 6174  `Time``: use dat
+00005a90: 6574 696d 652e 7469 6d65 0a20 2a20 6060  etime.time. * ``
+00005aa0: 4269 6749 6e74 6567 6572 6060 0a20 2a20  BigInteger``. * 
+00005ab0: 6060 426f 6f6c 6561 6e60 600a 202a 2060  ``Boolean``. * `
+00005ac0: 6044 6174 6560 603a 2075 7365 2064 6174  `Date``: use dat
+00005ad0: 6574 696d 652e 6461 7465 0a20 2a20 6060  etime.date. * ``
+00005ae0: 496e 7465 6765 7260 600a 202a 2060 6049  Integer``. * ``I
+00005af0: 6e74 6572 7661 6c60 603a 2075 7365 2064  nterval``: use d
+00005b00: 6174 6574 696d 652e 7469 6d65 6465 6c74  atetime.timedelt
+00005b10: 610a 202a 2060 604c 6172 6765 4269 6e61  a. * ``LargeBina
+00005b20: 7279 6060 0a20 2a20 6060 5374 7269 6e67  ry``. * ``String
+00005b30: 6060 0a20 2a20 6060 5465 7874 6060 0a20  ``. * ``Text``. 
+00005b40: 2a20 6060 5365 6c65 6374 696f 6e60 600a  * ``Selection``.
+00005b50: 202a 2060 6045 6e75 6d60 603a 2075 7365   * ``Enum``: use
+00005b60: 2065 6e75 6d2e 456e 756d 2069 6e68 6572   enum.Enum inher
+00005b70: 6974 6564 2063 6c61 7373 0a20 2a20 6060  ited class. * ``
+00005b80: 4a73 6f6e 6060 0a20 2a20 6060 5365 7175  Json``. * ``Sequ
+00005b90: 656e 6365 6060 0a20 2a20 6060 436f 6c6f  ence``. * ``Colo
+00005ba0: 7260 603a 2075 7365 2063 6f6c 6f75 722e  r``: use colour.
+00005bb0: 436f 6c6f 720a 202a 2060 6050 6173 7377  Color. * ``Passw
+00005bc0: 6f72 6460 603a 2075 7365 2073 716c 616c  ord``: use sqlal
+00005bd0: 6368 656d 795f 7574 696c 732e 7479 7065  chemy_utils.type
+00005be0: 732e 7061 7373 776f 7264 2e50 6173 7377  s.password.Passw
+00005bf0: 6f72 640a 202a 2060 6055 5549 4460 603a  ord. * ``UUID``:
+00005c00: 2075 7365 2075 7569 640a 202a 2060 6055   use uuid. * ``U
+00005c10: 524c 6060 3a20 7573 6520 6675 726c 2e66  RL``: use furl.f
+00005c20: 7572 6c0a 202a 2060 6050 686f 6e65 4e75  url. * ``PhoneNu
+00005c30: 6d62 6572 6060 3a20 7573 6520 7371 6c61  mber``: use sqla
+00005c40: 6c63 6865 6d79 5f75 7469 6c73 2e50 686f  lchemy_utils.Pho
+00005c50: 6e65 4e75 6d62 6572 0a20 2a20 6060 456d  neNumber. * ``Em
+00005c60: 6169 6c60 600a 202a 2060 6043 6f75 6e74  ail``. * ``Count
+00005c70: 7279 6060 3a20 7573 6520 7079 636f 756e  ry``: use pycoun
+00005c80: 7472 790a 202a 2060 604d 6f64 656c 5365  try. * ``ModelSe
+00005c90: 6c65 6374 696f 6e60 600a 202a 2060 604d  lection``. * ``M
+00005ca0: 6f64 656c 4669 656c 6453 656c 6563 7469  odelFieldSelecti
+00005cb0: 6f6e 6060 0a0a 416c 6c20 7468 6520 636f  on``..All the co
+00005cc0: 6c75 6d6e 7320 6861 7665 2074 6865 2066  lumns have the f
+00005cd0: 6f6c 6c6f 7769 6e67 206f 7074 696f 6e61  ollowing optiona
+00005ce0: 6c20 7061 7261 6d65 7465 7273 3a0a 0a2b  l parameters:..+
+00005cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005d00: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+00005d10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00005d40: 0a7c 2050 6172 616d 6574 6572 2020 2020  .| Parameter    
+00005d50: 2020 2020 7c20 4465 7363 7269 7074 696f      | Descriptio
+00005d60: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00005d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d90: 207c 0a2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   |.+============
+00005da0: 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d  ======+=========
+00005db0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005dc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005dd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005de0: 3d3d 3d2b 0a7c 206c 6162 656c 2020 2020  ===+.| label    
+00005df0: 2020 2020 2020 2020 7c20 4c61 6265 6c20          | Label 
+00005e00: 6f66 2074 6865 2063 6f6c 756d 6e2c 2049  of the column, I
+00005e10: 6620 4e6f 6e65 2074 6865 206c 6162 656c  f None the label
+00005e20: 2069 7320 7468 6520 6e61 6d65 206f 6620   is the name of 
+00005e30: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+00005e40: 2020 2020 2020 2020 2020 7c20 636f 6c75            | colu
+00005e50: 6d6e 2063 6170 6974 616c 697a 6564 2020  mn capitalized  
+00005e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e80: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+00005e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+00005ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005ed0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2064 6566  ---------+.| def
+00005ee0: 6175 6c74 2020 2020 2020 2020 2020 7c20  ault          | 
+00005ef0: 6465 6669 6e65 2061 2064 6566 6175 6c74  define a default
+00005f00: 2076 616c 7565 2066 6f72 2074 6869 7320   value for this 
+00005f10: 636f 6c75 6d6e 2e20 2020 2020 2020 2020  column.         
+00005f20: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00005f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f50: 2020 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d       |.+--------
-00005f60: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-00005f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00005fa0: 2d2d 2d2d 2d2d 2d2b 0a7c 2064 6566 6175  -------+.| defau
-00005fb0: 6c74 2020 2020 2020 2020 2020 7c20 6465  lt          | de
-00005fc0: 6669 6e65 2061 2064 6566 6175 6c74 2076  fine a default v
-00005fd0: 616c 7565 2066 6f72 2074 6869 7320 636f  alue for this co
-00005fe0: 6c75 6d6e 2e20 2020 2020 2020 2020 2020  lumn.           
-00005ff0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00006000: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00005f40: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f70: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f90: 2020 7c20 2e2e 7761 726e 696e 673a 3a20    | ..warning:: 
+00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fc0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00005fd0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00005fe0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006000: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006040: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-00006050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006060: 7c20 2e2e 7761 726e 696e 673a 3a20 2020  | ..warning::   
-00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006090: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00006020: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00006030: 2020 2020 2020 7c20 2020 2020 5468 6520        |     The 
+00006040: 6465 6661 756c 7420 7661 6c75 6520 6465  default value de
+00006050: 7065 6e64 7320 6f66 2074 6865 2063 6f6c  pends of the col
+00006060: 756d 6e20 7479 7065 2020 2020 2020 2020  umn type        
+00006070: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+00006080: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000060a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060b0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-000060c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060e0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000060f0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00006100: 2020 2020 7c20 2020 2020 5468 6520 6465      |     The de
-00006110: 6661 756c 7420 7661 6c75 6520 6465 7065  fault value depe
-00006120: 6e64 7320 6f66 2074 6865 2063 6f6c 756d  nds of the colum
-00006130: 6e20 7479 7065 2020 2020 2020 2020 2020  n type          
-00006140: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00006150: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00006160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006190: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-000061a0: 2020 2020 2020 2020 7c20 2e2e 6e6f 7465          | ..note
-000061b0: 3a3a 2020 2020 2020 2020 2020 2020 2020  ::              
+000060b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060c0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+000060d0: 2020 2020 2020 2020 2020 7c20 2e2e 6e6f            | ..no
+000060e0: 7465 3a3a 2020 2020 2020 2020 2020 2020  te::            
+000060f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006110: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+00006120: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00006130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006160: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
+00006170: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00006180: 2020 2020 5075 7420 7468 6520 6e61 6d65      Put the name
+00006190: 206f 6620 6120 636c 6173 736d 6574 686f   of a classmetho
+000061a0: 6420 746f 2063 616c 6c20 6974 2020 2020  d to call it    
+000061b0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 000061c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061e0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-000061f0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00006200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006230: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-00006240: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00006250: 2020 5075 7420 7468 6520 6e61 6d65 206f    Put the name o
-00006260: 6620 6120 636c 6173 736d 6574 686f 6420  f a classmethod 
-00006270: 746f 2063 616c 6c20 6974 2020 2020 2020  to call it      
-00006280: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00006290: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062d0: 2020 2020 2020 2020 2020 207c 0a2b 2d2d             |.+--
+000061d0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006200: 2020 2020 2020 2020 2020 2020 207c 0a2b               |.+
+00006210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006220: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+00006230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00006260: 0a7c 2069 6e64 6578 2020 2020 2020 2020  .| index        
+00006270: 2020 2020 7c20 626f 6f6c 6561 6e20 666c      | boolean fl
+00006280: 6167 2074 6f20 6465 6669 6e65 2077 6865  ag to define whe
+00006290: 7468 6572 2074 6865 2063 6f6c 756d 6e20  ther the column 
+000062a0: 6973 2069 6e64 6578 6564 2020 2020 2020  is indexed      
+000062b0: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
+000062c0: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+000062d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000062e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000062f0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00006300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
-00006330: 2069 6e64 6578 2020 2020 2020 2020 2020   index          
-00006340: 2020 7c20 626f 6f6c 6561 6e20 666c 6167    | boolean flag
-00006350: 2074 6f20 6465 6669 6e65 2077 6865 7468   to define wheth
-00006360: 6572 2074 6865 2063 6f6c 756d 6e20 6973  er the column is
-00006370: 2069 6e64 6578 6564 2020 2020 2020 207c   indexed       |
-00006380: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
-00006390: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-000063a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000063b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000063c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000063d0: 2d2b 0a7c 206e 756c 6c61 626c 6520 2020  -+.| nullable   
-000063e0: 2020 2020 2020 7c20 4465 6669 6e65 7320        | Defines 
-000063f0: 6966 2074 6865 2063 6f6c 756d 6e20 6d75  if the column mu
-00006400: 7374 2062 6520 6669 6c6c 6564 206f 7220  st be filled or 
+000062f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006300: 2d2d 2d2b 0a7c 206e 756c 6c61 626c 6520  ---+.| nullable 
+00006310: 2020 2020 2020 2020 7c20 4465 6669 6e65          | Define
+00006320: 7320 6966 2074 6865 2063 6f6c 756d 6e20  s if the column 
+00006330: 6d75 7374 2062 6520 6669 6c6c 6564 206f  must be filled o
+00006340: 7220 6e6f 7420 2020 2020 2020 2020 2020  r not           
+00006350: 2020 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d       |.+--------
+00006360: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00006370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000063a0: 2d2d 2d2d 2d2d 2d2b 0a7c 2070 7269 6d61  -------+.| prima
+000063b0: 7279 5f6b 6579 2020 2020 2020 7c20 426f  ry_key      | Bo
+000063c0: 6f6c 6561 6e20 666c 6167 2074 6f20 6465  olean flag to de
+000063d0: 6669 6e65 2069 6620 7468 6520 636f 6c75  fine if the colu
+000063e0: 6d6e 2069 7320 6120 7072 696d 6172 7920  mn is a primary 
+000063f0: 6b65 7920 6f72 2020 207c 0a7c 2020 2020  key or   |.|    
+00006400: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 00006410: 6e6f 7420 2020 2020 2020 2020 2020 2020  not             
-00006420: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-00006430: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00006440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006440: 2020 2020 2020 2020 2020 207c 0a2b 2d2d             |.+--
 00006450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006470: 2d2d 2d2d 2d2b 0a7c 2070 7269 6d61 7279  -----+.| primary
-00006480: 5f6b 6579 2020 2020 2020 7c20 426f 6f6c  _key      | Bool
-00006490: 6561 6e20 666c 6167 2074 6f20 6465 6669  ean flag to defi
-000064a0: 6e65 2069 6620 7468 6520 636f 6c75 6d6e  ne if the column
-000064b0: 2069 7320 6120 7072 696d 6172 7920 6b65   is a primary ke
-000064c0: 7920 6f72 2020 207c 0a7c 2020 2020 2020  y or   |.|      
-000064d0: 2020 2020 2020 2020 2020 2020 7c20 6e6f              | no
-000064e0: 7420 2020 2020 2020 2020 2020 2020 2020  t               
-000064f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006510: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
-00006520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-00006530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2075  -----------+.| u
-00006570: 6e69 7175 6520 2020 2020 2020 2020 2020  nique           
-00006580: 7c20 426f 6f6c 6561 6e20 666c 6167 2074  | Boolean flag t
-00006590: 6f20 6465 6669 6e65 2069 6620 7468 6520  o define if the 
-000065a0: 636f 6c75 6d6e 2076 616c 7565 206d 7573  column value mus
-000065b0: 7420 6265 2075 6e69 7175 6520 207c 0a7c  t be unique  |.|
-000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065d0: 2020 7c20 6f72 206e 6f74 2020 2020 2020    | or not      
-000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006600: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00006610: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
-00006620: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00006630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006660: 2d2b 0a7c 2066 6f72 6569 676e 5f6b 6579  -+.| foreign_key
-00006670: 2020 2020 2020 7c20 4465 6669 6e65 2061        | Define a
-00006680: 2066 6f72 6569 676e 206b 6579 206f 6e20   foreign key on 
-00006690: 7468 6973 2063 6f6c 756d 6e20 746f 2061  this column to a
-000066a0: 6e6f 7468 6572 2063 6f6c 756d 6e20 6f66  nother column of
-000066b0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-000066c0: 2020 2020 2020 2020 7c20 616e 6f74 6865          | anothe
-000066d0: 7220 6d6f 6465 6c3a 3a20 2020 2020 2020  r model::       
+00006460: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
+00006470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
+000064a0: 2075 6e69 7175 6520 2020 2020 2020 2020   unique         
+000064b0: 2020 7c20 426f 6f6c 6561 6e20 666c 6167    | Boolean flag
+000064c0: 2074 6f20 6465 6669 6e65 2069 6620 7468   to define if th
+000064d0: 6520 636f 6c75 6d6e 2076 616c 7565 206d  e column value m
+000064e0: 7573 7420 6265 2075 6e69 7175 6520 207c  ust be unique  |
+000064f0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00006500: 2020 2020 7c20 6f72 206e 6f74 2020 2020      | or not    
+00006510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006540: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
+00006550: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00006560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006570: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006590: 2d2d 2d2b 0a7c 2066 6f72 6569 676e 5f6b  ---+.| foreign_k
+000065a0: 6579 2020 2020 2020 7c20 4465 6669 6e65  ey      | Define
+000065b0: 2061 2066 6f72 6569 676e 206b 6579 206f   a foreign key o
+000065c0: 6e20 7468 6973 2063 6f6c 756d 6e20 746f  n this column to
+000065d0: 2061 6e6f 7468 6572 2063 6f6c 756d 6e20   another column 
+000065e0: 6f66 2020 207c 0a7c 2020 2020 2020 2020  of   |.|        
+000065f0: 2020 2020 2020 2020 2020 7c20 616e 6f74            | anot
+00006600: 6865 7220 6d6f 6465 6c3a 3a20 2020 2020  her model::     
+00006610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006630: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+00006640: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00006650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006680: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
+00006690: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000066a0: 2020 2040 7265 6769 7374 6572 284d 6f64     @register(Mod
+000066b0: 656c 2920 2020 2020 2020 2020 2020 2020  el)             
+000066c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066d0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 000066e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006700: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-00006710: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00006720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066f0: 7c20 2020 2063 6c61 7373 2046 6f6f 3a20  |    class Foo: 
+00006700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006720: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 00006730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006750: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-00006760: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00006770: 2040 7265 6769 7374 6572 284d 6f64 656c   @register(Model
-00006780: 2920 2020 2020 2020 2020 2020 2020 2020  )               
-00006790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067a0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-000067b0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000067c0: 2020 2063 6c61 7373 2046 6f6f 3a20 2020     class Foo:   
-000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067f0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00006740: 2020 7c20 2020 2020 2020 2069 6420 3d20    |        id = 
+00006750: 496e 7465 6765 7228 7072 696d 6172 795f  Integer(primary_
+00006760: 6b65 793d 5472 7565 2920 2020 2020 2020  key=True)       
+00006770: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00006780: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00006790: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067d0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+000067e0: 2020 2020 2020 7c20 2020 2040 7265 6769        |    @regi
+000067f0: 7374 6572 284d 6f64 656c 2920 2020 2020  ster(Model)     
 00006800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006810: 7c20 2020 2020 2020 2069 6420 3d20 496e  |        id = In
-00006820: 7465 6765 7228 7072 696d 6172 795f 6b65  teger(primary_ke
-00006830: 793d 5472 7565 2920 2020 2020 2020 2020  y=True)         
-00006840: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00006810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006820: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+00006830: 2020 2020 2020 2020 7c20 2020 2063 6c61          |    cla
+00006840: 7373 2042 6172 3a20 2020 2020 2020 2020  ss Bar:         
 00006850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006860: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00006870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006890: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000068a0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-000068b0: 2020 2020 7c20 2020 2040 7265 6769 7374      |    @regist
-000068c0: 6572 284d 6f64 656c 2920 2020 2020 2020  er(Model)       
-000068d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068f0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00006900: 2020 2020 2020 7c20 2020 2063 6c61 7373        |    class
-00006910: 2042 6172 3a20 2020 2020 2020 2020 2020   Bar:           
-00006920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006870: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+00006880: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00006890: 2020 2069 6420 3d20 496e 7465 6765 7228     id = Integer(
+000068a0: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
+000068b0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
+000068c0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+000068d0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+000068e0: 2020 2020 2066 6f6f 203d 2049 6e74 6567       foo = Integ
+000068f0: 6572 2866 6f72 6569 676e 5f6b 6579 3d4d  er(foreign_key=M
+00006900: 6f64 656c 2e46 6f6f 2e75 7365 2827 6964  odel.Foo.use('id
+00006910: 2729 2920 2020 2020 207c 0a7c 2020 2020  '))      |.|    
+00006920: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006940: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-00006950: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00006960: 2069 6420 3d20 496e 7465 6765 7228 7072   id = Integer(pr
-00006970: 696d 6172 795f 6b65 793d 5472 7565 2920  imary_key=True) 
-00006980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006990: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-000069a0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-000069b0: 2020 2066 6f6f 203d 2049 6e74 6567 6572     foo = Integer
-000069c0: 2866 6f72 6569 676e 5f6b 6579 3d4d 6f64  (foreign_key=Mod
-000069d0: 656c 2e46 6f6f 2e75 7365 2827 6964 2729  el.Foo.use('id')
-000069e0: 2920 2020 2020 207c 0a7c 2020 2020 2020  )      |.|      
-000069f0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00006a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a30: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00006a40: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00006a50: 4966 2074 6865 2060 604d 6f64 656c 6060  If the ``Model``
-00006a60: 2044 6563 6c61 7261 7469 6f6e 7320 646f   Declarations do
-00006a70: 6573 6e27 7420 6578 6973 7420 7965 742c  esn't exist yet,
-00006a80: 2079 6f75 2063 616e 2020 207c 0a7c 2020   you can   |.|  
-00006a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006aa0: 7c20 7573 6520 7468 6520 7265 6769 7372  | use the regisr
-00006ab0: 7479 206e 616d 653a 3a20 2020 2020 2020  ty name::       
-00006ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ad0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006960: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006980: 7c20 4966 2074 6865 2060 604d 6f64 656c  | If the ``Model
+00006990: 6060 2044 6563 6c61 7261 7469 6f6e 7320  `` Declarations 
+000069a0: 646f 6573 6e27 7420 6578 6973 7420 7965  doesn't exist ye
+000069b0: 742c 2079 6f75 2063 616e 2020 207c 0a7c  t, you can   |.|
+000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069d0: 2020 7c20 7573 6520 7468 6520 7265 6769    | use the regi
+000069e0: 7372 7479 206e 616d 653a 3a20 2020 2020  srty name::     
+000069f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a00: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00006a10: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00006a20: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00006a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a60: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00006a70: 2020 2020 2020 7c20 2020 2020 666f 6f20        |     foo 
+00006a80: 3d20 496e 7465 6765 7228 666f 7265 6967  = Integer(foreig
+00006a90: 6e5f 6b65 793d 274d 6f64 656c 2e46 6f6f  n_key='Model.Foo
+00006aa0: 3d3e 6964 2729 2920 2020 2020 2020 2020  =>id'))         
+00006ab0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+00006ac0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00006ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006af0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00006b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b20: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00006b30: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00006b40: 2020 2020 7c20 2020 2020 666f 6f20 3d20      |     foo = 
-00006b50: 496e 7465 6765 7228 666f 7265 6967 6e5f  Integer(foreign_
-00006b60: 6b65 793d 274d 6f64 656c 2e46 6f6f 3d3e  key='Model.Foo=>
-00006b70: 6964 2729 2920 2020 2020 2020 2020 2020  id'))           
-00006b80: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00006b90: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00006ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bd0: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-00006be0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00006bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b00: 2020 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d       |.+--------
+00006b10: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00006b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006b30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006b50: 2d2d 2d2d 2d2d 2d2b 0a7c 2064 625f 636f  -------+.| db_co
+00006b60: 6c75 6d6e 5f6e 616d 6520 2020 7c20 5374  lumn_name   | St
+00006b70: 7269 6e67 2074 6f20 6465 6669 6e65 2074  ring to define t
+00006b80: 6865 2072 6561 6c20 636f 6c75 6d6e 206e  he real column n
+00006b90: 616d 6520 696e 2074 6865 2074 6162 6c65  ame in the table
+00006ba0: 2c20 2020 2020 2020 207c 0a7c 2020 2020  ,        |.|    
+00006bb0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00006bc0: 6469 6666 6572 656e 7420 6672 6f6d 2074  different from t
+00006bd0: 6865 206d 6f64 656c 2061 7474 7269 6275  he model attribu
+00006be0: 7465 206e 616d 6520 2020 2020 2020 2020  te name         
+00006bf0: 2020 2020 2020 2020 2020 207c 0a2b 2d2d             |.+--
 00006c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006c20: 2d2d 2d2d 2d2b 0a7c 2064 625f 636f 6c75  -----+.| db_colu
-00006c30: 6d6e 5f6e 616d 6520 2020 7c20 5374 7269  mn_name   | Stri
-00006c40: 6e67 2074 6f20 6465 6669 6e65 2074 6865  ng to define the
-00006c50: 2072 6561 6c20 636f 6c75 6d6e 206e 616d   real column nam
-00006c60: 6520 696e 2074 6865 2074 6162 6c65 2c20  e in the table, 
-00006c70: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-00006c80: 2020 2020 2020 2020 2020 2020 7c20 6469              | di
-00006c90: 6666 6572 656e 7420 6672 6f6d 2074 6865  fferent from the
-00006ca0: 206d 6f64 656c 2061 7474 7269 6275 7465   model attribute
-00006cb0: 206e 616d 6520 2020 2020 2020 2020 2020   name           
-00006cc0: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
-00006cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-00006ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006d10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2065  -----------+.| e
-00006d20: 6e63 7279 7074 5f6b 6579 2020 2020 2020  ncrypt_key      
-00006d30: 7c20 4372 7970 7420 7468 6520 636f 6c75  | Crypt the colu
-00006d40: 6d6e 2069 6e20 7468 6520 6461 7461 6261  mn in the databa
-00006d50: 7365 2e20 6361 6e20 7461 6b65 2074 6865  se. can take the
-00006d60: 2076 616c 7565 733a 2020 2020 207c 0a7c   values:     |.|
-00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d80: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00006d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006db0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00006dc0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00006dd0: 2020 2020 7c20 2a20 6120 5374 7269 6e67      | * a String
-00006de0: 2065 783a 2066 6f6f 203d 2053 7472 696e   ex: foo = Strin
-00006df0: 6728 656e 6372 7970 745f 6b65 793d 2753  g(encrypt_key='S
-00006e00: 6563 7265 744b 6579 2729 2020 2020 2020  ecretKey')      
-00006e10: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00006e20: 2020 2020 2020 7c20 2a20 6120 636c 6173        | * a clas
-00006e30: 736d 6574 686f 6420 6e61 6d65 206f 6e20  smethod name on 
-00006e40: 7468 6520 6d6f 6465 6c20 2020 2020 2020  the model       
-00006e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e60: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-00006e70: 2020 2020 2020 2020 7c20 2a20 5472 7565          | * True
-00006e80: 2076 616c 7565 2c20 7365 6172 6368 2069   value, search i
-00006e90: 6e20 7468 6520 436f 6e66 6967 7572 6174  n the Configurat
-00006ea0: 696f 6e20 2020 2020 2020 2020 2020 2020  ion             
-00006eb0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-00006ec0: 2020 2020 2020 2020 2020 7c20 2020 6060            |   ``
-00006ed0: 6465 6661 756c 745f 656e 6372 7970 745f  default_encrypt_
-00006ee0: 6b65 7960 6020 7468 6520 7661 6c75 652c  key`` the value,
-00006ef0: 2074 6865 7920 6172 6520 6e6f 2064 6566   they are no def
-00006f00: 6175 6c74 2e20 207c 0a7c 2020 2020 2020  ault.  |.|      
-00006f10: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00006f20: 6966 206e 6f20 7661 6c75 6520 6578 6973  if no value exis
-00006f30: 742c 2061 6e20 6578 6365 7074 696f 6e20  t, an exception 
-00006f40: 6973 2072 6169 7365 6420 2020 2020 2020  is raised       
-00006f50: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00006f60: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00006c10: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
+00006c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
+00006c50: 2065 6e63 7279 7074 5f6b 6579 2020 2020   encrypt_key    
+00006c60: 2020 7c20 4372 7970 7420 7468 6520 636f    | Crypt the co
+00006c70: 6c75 6d6e 2069 6e20 7468 6520 6461 7461  lumn in the data
+00006c80: 6261 7365 2e20 6361 6e20 7461 6b65 2074  base. can take t
+00006c90: 6865 2076 616c 7565 733a 2020 2020 207c  he values:     |
+00006ca0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00006cb0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00006cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cf0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00006d00: 2020 2020 2020 7c20 2a20 6120 5374 7269        | * a Stri
+00006d10: 6e67 2065 783a 2066 6f6f 203d 2053 7472  ng ex: foo = Str
+00006d20: 696e 6728 656e 6372 7970 745f 6b65 793d  ing(encrypt_key=
+00006d30: 2753 6563 7265 744b 6579 2729 2020 2020  'SecretKey')    
+00006d40: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+00006d50: 2020 2020 2020 2020 7c20 2a20 6120 636c          | * a cl
+00006d60: 6173 736d 6574 686f 6420 6e61 6d65 206f  assmethod name o
+00006d70: 6e20 7468 6520 6d6f 6465 6c20 2020 2020  n the model     
+00006d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d90: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+00006da0: 2020 2020 2020 2020 2020 7c20 2a20 5472            | * Tr
+00006db0: 7565 2076 616c 7565 2c20 7365 6172 6368  ue value, search
+00006dc0: 2069 6e20 7468 6520 436f 6e66 6967 7572   in the Configur
+00006dd0: 6174 696f 6e20 2020 2020 2020 2020 2020  ation           
+00006de0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+00006df0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00006e00: 6060 6465 6661 756c 745f 656e 6372 7970  ``default_encryp
+00006e10: 745f 6b65 7960 6020 7468 6520 7661 6c75  t_key`` the valu
+00006e20: 652c 2074 6865 7920 6172 6520 6e6f 2064  e, they are no d
+00006e30: 6566 6175 6c74 2e20 207c 0a7c 2020 2020  efault.  |.|    
+00006e40: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00006e50: 2020 6966 206e 6f20 7661 6c75 6520 6578    if no value ex
+00006e60: 6973 742c 2061 6e20 6578 6365 7074 696f  ist, an exceptio
+00006e70: 6e20 6973 2072 6169 7365 6420 2020 2020  n is raised     
+00006e80: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00006e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ea0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00006eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ed0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00006ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ef0: 2020 7c20 2e2e 7761 726e 696e 673a 3a20    | ..warning:: 
+00006f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f20: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00006f30: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00006f40: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00006f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fa0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-00006fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fc0: 7c20 2e2e 7761 726e 696e 673a 3a20 2020  | ..warning::   
-00006fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ff0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00006f80: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00006f90: 2020 2020 2020 7c20 2020 2020 5468 6520        |     The 
+00006fa0: 7079 7468 6f6e 2070 6163 6b61 6765 2063  python package c
+00006fb0: 7279 7074 6f67 7261 7068 7920 6d75 7374  ryptography must
+00006fc0: 2062 6520 696e 7374 616c 6c65 6420 2020   be installed   
+00006fd0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+00006fe0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00006ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007010: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007040: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00007050: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00007060: 2020 2020 7c20 2020 2020 5468 6520 7079      |     The py
-00007070: 7468 6f6e 2070 6163 6b61 6765 2063 7279  thon package cry
-00007080: 7074 6f67 7261 7068 7920 6d75 7374 2062  ptography must b
-00007090: 6520 696e 7374 616c 6c65 6420 2020 2020  e installed     
-000070a0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-000070b0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-000070c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070f0: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-00007100: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00007110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007140: 2d2d 2d2d 2d2b 0a7c 2069 676e 6f72 655f  -----+.| ignore_
-00007150: 6d69 6772 6174 696f 6e20 7c20 6966 2054  migration | if T
-00007160: 7275 6520 7468 656e 2074 6865 2063 6f6c  rue then the col
-00007170: 756d 6e20 696e 2074 6865 2074 6162 6c65  umn in the table
-00007180: 2077 696c 6c20 6e6f 7420 6265 206d 6f64   will not be mod
-00007190: 6966 6965 6420 207c 0a7c 2020 2020 2020  ified  |.|      
-000071a0: 2020 2020 2020 2020 2020 2020 7c20 7768              | wh
-000071b0: 656e 2074 6865 2064 6566 696e 6974 696f  en the definitio
-000071c0: 6e20 6f66 2074 6865 2063 6f6c 756d 6e20  n of the column 
-000071d0: 616e 6420 7468 6520 636f 6c75 6d6e 206f  and the column o
-000071e0: 6620 7468 6520 2020 207c 0a7c 2020 2020  f the    |.|    
-000071f0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00007200: 7461 626c 6520 6172 6520 6469 6665 7265  table are difere
-00007210: 6e74 7320 2020 2020 2020 2020 2020 2020  nts             
-00007220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007230: 2020 2020 2020 2020 2020 207c 0a2b 2d2d             |.+--
-00007240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007250: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00007260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a  -------------+..
-00007290: 4f74 6865 7220 6174 7472 6962 7574 6520  Other attribute 
-000072a0: 666f 7220 6060 5374 7269 6e67 6060 3a0a  for ``String``:.
-000072b0: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  .+-------------+
-000072c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000072d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000072e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000072f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00007300: 0a7c 2050 6172 616d 2020 2020 2020 207c  .| Param       |
-00007310: 2044 6573 6372 6970 7469 6f6e 2020 2020   Description    
-00007320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007340: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00007350: 0a2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b  .+=============+
-00007360: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007370: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007380: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007390: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b  ===============+
-000073a0: 0a7c 2060 6073 697a 6560 6020 2020 207c  .| ``size``    |
-000073b0: 2043 6f6c 756d 6e20 7369 7a65 2069 6e20   Column size in 
-000073c0: 7468 6520 7461 626c 6520 2020 2020 2020  the table       
-000073d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073e0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000073f0: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  .+-------------+
-00007400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00007440: 0a0a 4f74 6865 7220 6174 7472 6962 7574  ..Other attribut
-00007450: 6520 666f 7220 6060 5365 6c65 6374 696f  e for ``Selectio
-00007460: 6e60 603a 0a0a 2b2d 2d2d 2d2d 2d2d 2d2d  n``:..+---------
-00007470: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00007480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000074a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000074b0: 2d2d 2d2d 2b0a 7c20 5061 7261 6d20 2020  ----+.| Param   
-000074c0: 2020 2020 2020 207c 2044 6573 6372 6970         | Descrip
-000074d0: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
-000074e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007500: 2020 2020 7c0a 2b3d 3d3d 3d3d 3d3d 3d3d      |.+=========
-00007510: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
-00007520: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007530: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007540: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007550: 3d3d 3d3d 2b0a 7c20 6060 7369 7a65 6060  ====+.| ``size``
-00007560: 2020 2020 2020 207c 2063 6f6c 756d 6e20         | column 
-00007570: 7369 7a65 2069 6e20 7468 6520 7461 626c  size in the tabl
-00007580: 6520 2020 2020 2020 2020 2020 2020 2020  e               
-00007590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075a0: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
-000075b0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-000075c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000075d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007020: 2020 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d       |.+--------
+00007030: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00007040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007070: 2d2d 2d2d 2d2d 2d2b 0a7c 2069 676e 6f72  -------+.| ignor
+00007080: 655f 6d69 6772 6174 696f 6e20 7c20 6966  e_migration | if
+00007090: 2054 7275 6520 7468 656e 2074 6865 2063   True then the c
+000070a0: 6f6c 756d 6e20 696e 2074 6865 2074 6162  olumn in the tab
+000070b0: 6c65 2077 696c 6c20 6e6f 7420 6265 206d  le will not be m
+000070c0: 6f64 6966 6965 6420 207c 0a7c 2020 2020  odified  |.|    
+000070d0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000070e0: 7768 656e 2074 6865 2064 6566 696e 6974  when the definit
+000070f0: 696f 6e20 6f66 2074 6865 2063 6f6c 756d  ion of the colum
+00007100: 6e20 616e 6420 7468 6520 636f 6c75 6d6e  n and the column
+00007110: 206f 6620 7468 6520 2020 207c 0a7c 2020   of the    |.|  
+00007120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007130: 7c20 7461 626c 6520 6172 6520 6469 6665  | table are dife
+00007140: 7265 6e74 7320 2020 2020 2020 2020 2020  rents           
+00007150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007160: 2020 2020 2020 2020 2020 2020 207c 0a2b               |.+
+00007170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007180: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+00007190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000071a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000071b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+000071c0: 0a0a 4f74 6865 7220 6174 7472 6962 7574  ..Other attribut
+000071d0: 6520 666f 7220 6060 5374 7269 6e67 6060  e for ``String``
+000071e0: 3a0a 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :..+------------
+000071f0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+00007200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007230: 2d2b 0a7c 2050 6172 616d 2020 2020 2020  -+.| Param      
+00007240: 207c 2044 6573 6372 6970 7469 6f6e 2020   | Description  
+00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007280: 207c 0a2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   |.+============
+00007290: 3d2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  =+==============
+000072a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000072b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000072c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000072d0: 3d2b 0a7c 2060 6073 697a 6560 6020 2020  =+.| ``size``   
+000072e0: 207c 2043 6f6c 756d 6e20 7369 7a65 2069   | Column size i
+000072f0: 6e20 7468 6520 7461 626c 6520 2020 2020  n the table     
+00007300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007320: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
+00007330: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+00007340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007370: 2d2b 0a0a 4f74 6865 7220 6174 7472 6962  -+..Other attrib
+00007380: 7574 6520 666f 7220 6060 5365 6c65 6374  ute for ``Select
+00007390: 696f 6e60 603a 0a0a 2b2d 2d2d 2d2d 2d2d  ion``:..+-------
+000073a0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+000073b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000073c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000073d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000073e0: 2d2d 2d2d 2d2d 2b0a 7c20 5061 7261 6d20  ------+.| Param 
+000073f0: 2020 2020 2020 2020 207c 2044 6573 6372           | Descr
+00007400: 6970 7469 6f6e 2020 2020 2020 2020 2020  iption          
+00007410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007430: 2020 2020 2020 7c0a 2b3d 3d3d 3d3d 3d3d        |.+=======
+00007440: 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d  =========+======
+00007450: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007460: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007470: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007480: 3d3d 3d3d 3d3d 2b0a 7c20 6060 7369 7a65  ======+.| ``size
+00007490: 6060 2020 2020 2020 207c 2063 6f6c 756d  ``       | colum
+000074a0: 6e20 7369 7a65 2069 6e20 7468 6520 7461  n size in the ta
+000074b0: 626c 6520 2020 2020 2020 2020 2020 2020  ble             
+000074c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074d0: 2020 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d        |.+-------
+000074e0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+000074f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007520: 2d2d 2d2d 2d2d 2b0a 7c20 6060 7365 6c65  ------+.| ``sele
+00007530: 6374 696f 6e73 6060 207c 2060 6064 6963  ctions`` | ``dic
+00007540: 7460 6020 6f72 2060 6064 6963 742e 6974  t`` or ``dict.it
+00007550: 656d 7360 6020 746f 2067 6976 6520 7468  ems`` to give th
+00007560: 6520 6176 6169 6c61 626c 6520 6b65 7920  e available key 
+00007570: 7769 7468 2020 7c0a 7c20 2020 2020 2020  with  |.|       
+00007580: 2020 2020 2020 2020 207c 2074 6865 2061           | the a
+00007590: 7373 6f63 6961 7465 206c 6162 656c 2020  ssociate label  
+000075a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075c0: 2020 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d        |.+-------
+000075d0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
 000075e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000075f0: 2d2d 2d2d 2b0a 7c20 6060 7365 6c65 6374  ----+.| ``select
-00007600: 696f 6e73 6060 207c 2060 6064 6963 7460  ions`` | ``dict`
-00007610: 6020 6f72 2060 6064 6963 742e 6974 656d  ` or ``dict.item
-00007620: 7360 6020 746f 2067 6976 6520 7468 6520  s`` to give the 
-00007630: 6176 6169 6c61 626c 6520 6b65 7920 7769  available key wi
-00007640: 7468 2020 7c0a 7c20 2020 2020 2020 2020  th  |.|         
-00007650: 2020 2020 2020 207c 2074 6865 2061 7373         | the ass
-00007660: 6f63 6961 7465 206c 6162 656c 2020 2020  ociate label    
-00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007690: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
-000076a0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-000076b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000076c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000076d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000076e0: 2d2d 2d2d 2b0a 0a4f 7468 6572 2061 7474  ----+..Other att
-000076f0: 7269 6275 7465 2066 6f72 2060 6053 6571  ribute for ``Seq
-00007700: 7565 6e63 6560 603a 0a0a 2b2d 2d2d 2d2d  uence``:..+-----
-00007710: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00007720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007750: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 5061 7261  --------+.| Para
-00007760: 6d20 2020 2020 2020 207c 2044 6573 6372  m        | Descr
-00007770: 6970 7469 6f6e 2020 2020 2020 2020 2020  iption          
-00007780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077a0: 2020 2020 2020 2020 7c0a 2b3d 3d3d 3d3d          |.+=====
-000077b0: 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d  =========+======
-000077c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000077d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000077e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000077f0: 3d3d 3d3d 3d3d 3d3d 2b0a 7c20 6060 7369  ========+.| ``si
-00007800: 7a65 6060 2020 2020 207c 2063 6f6c 756d  ze``     | colum
-00007810: 6e20 7369 7a65 2069 6e20 7468 6520 7461  n size in the ta
-00007820: 626c 6520 2020 2020 2020 2020 2020 2020  ble             
-00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007840: 2020 2020 2020 2020 7c0a 2b2d 2d2d 2d2d          |.+-----
-00007850: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00007860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007890: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 6060 636f  --------+.| ``co
-000078a0: 6465 6060 2020 2020 207c 2063 6f64 6520  de``     | code 
-000078b0: 6f66 2074 6865 2073 6571 7565 6e63 6520  of the sequence 
-000078c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078e0: 2020 2020 2020 2020 7c0a 2b2d 2d2d 2d2d          |.+-----
-000078f0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00007900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007930: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 6060 666f  --------+.| ``fo
-00007940: 726d 6174 6572 6060 207c 2066 6f72 6d61  rmater`` | forma
-00007950: 7465 7220 6f66 2074 6865 2073 6571 7565  ter of the seque
-00007960: 6e63 6520 2020 2020 2020 2020 2020 2020  nce             
-00007970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007980: 2020 2020 2020 2020 7c0a 2b2d 2d2d 2d2d          |.+-----
-00007990: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-000079a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000079b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000079c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000079d0: 2d2d 2d2d 2d2d 2d2d 2b0a 0a4f 7468 6572  --------+..Other
-000079e0: 2061 7474 7269 6275 7465 2066 6f72 2060   attribute for `
-000079f0: 6043 6f6c 6f72 6060 3a0a 0a2b 2d2d 2d2d  `Color``:..+----
-00007a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-00007a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007a40: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2050 6172  ---------+.| Par
-00007a50: 616d 2020 2020 2020 2020 2020 7c20 4465  am          | De
-00007a60: 7363 7269 7074 696f 6e20 2020 2020 2020  scription       
-00007a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a90: 2020 2020 2020 2020 207c 0a2b 3d3d 3d3d           |.+====
-00007aa0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d  ============+===
-00007ab0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007ac0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007ad0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007ae0: 3d3d 3d3d 3d3d 3d3d 3d2b 0a7c 2060 6073  =========+.| ``s
-00007af0: 697a 6560 6020 2020 2020 2020 7c20 636f  ize``       | co
-00007b00: 6c75 6d6e 206d 6178 2073 697a 6520 696e  lumn max size in
-00007b10: 2074 6865 2074 6162 6c65 2020 2020 2020   the table      
-00007b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b30: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
-00007b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-00007b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007b80: 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a 4f74 6865  ---------+..Othe
-00007b90: 7220 6174 7472 6962 7574 6520 666f 7220  r attribute for 
-00007ba0: 6060 5061 7373 776f 7264 6060 3a0a 0a2b  ``Password``:..+
-00007bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007bc0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-00007bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
-00007c00: 2050 6172 616d 2020 2020 2020 2020 2020   Param          
-00007c10: 2020 207c 2044 6573 6372 6970 7469 6f6e     | Description
-00007c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c40: 2020 2020 2020 2020 2020 2020 207c 0a2b               |.+
-00007c50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007c60: 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ===+============
-00007c70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007c80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007c90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 0a7c  =============+.|
-00007ca0: 2060 6073 697a 6560 6020 2020 2020 2020   ``size``       
-00007cb0: 2020 207c 2070 6173 7377 6f72 6420 6d61     | password ma
-00007cc0: 7820 7369 7a65 2069 6e20 7468 6520 7461  x size in the ta
-00007cd0: 626c 6520 2020 2020 2020 2020 2020 2020  ble             
-00007ce0: 2020 2020 2020 2020 2020 2020 207c 0a2b               |.+
-00007cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007d00: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-00007d10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
-00007d40: 2060 6063 7279 7074 5f63 6f6e 7465 7874   ``crypt_context
-00007d50: 6060 207c 2073 6565 2074 6865 206f 7074  `` | see the opt
-00007d60: 696f 6e20 666f 7220 7468 6520 7079 7468  ion for the pyth
-00007d70: 6f6e 206c 6962 2060 7061 7373 6c69 6220  on lib `passlib 
-00007d80: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00007d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007da0: 2020 207c 203c 6874 7470 733a 2f2f 7061     | <https://pa
-00007db0: 7373 6c69 622e 7265 6164 7468 6564 6f63  sslib.readthedoc
-00007dc0: 732e 696f 2f65 6e2f 7374 6162 6c65 2f6c  s.io/en/stable/l
-00007dd0: 6962 2f70 6173 736c 6962 2e63 6f7c 0a7c  ib/passlib.co|.|
-00007de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007df0: 2020 207c 206e 7465 7874 2e68 746d 6c3e     | ntext.html>
-00007e00: 605f 2020 2020 2020 2020 2020 2020 2020  `_              
-00007e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e20: 2020 2020 2020 2020 2020 2020 207c 0a2b               |.+
+000075f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007610: 2d2d 2d2d 2d2d 2b0a 0a4f 7468 6572 2061  ------+..Other a
+00007620: 7474 7269 6275 7465 2066 6f72 2060 6053  ttribute for ``S
+00007630: 6571 7565 6e63 6560 603a 0a0a 2b2d 2d2d  equence``:..+---
+00007640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00007650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007680: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 5061  ----------+.| Pa
+00007690: 7261 6d20 2020 2020 2020 207c 2044 6573  ram        | Des
+000076a0: 6372 6970 7469 6f6e 2020 2020 2020 2020  cription        
+000076b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076d0: 2020 2020 2020 2020 2020 7c0a 2b3d 3d3d            |.+===
+000076e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d  ===========+====
+000076f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007700: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007710: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007720: 3d3d 3d3d 3d3d 3d3d 3d3d 2b0a 7c20 6060  ==========+.| ``
+00007730: 7369 7a65 6060 2020 2020 207c 2063 6f6c  size``     | col
+00007740: 756d 6e20 7369 7a65 2069 6e20 7468 6520  umn size in the 
+00007750: 7461 626c 6520 2020 2020 2020 2020 2020  table           
+00007760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007770: 2020 2020 2020 2020 2020 7c0a 2b2d 2d2d            |.+---
+00007780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00007790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000077a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000077b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000077c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 6060  ----------+.| ``
+000077d0: 636f 6465 6060 2020 2020 207c 2063 6f64  code``     | cod
+000077e0: 6520 6f66 2074 6865 2073 6571 7565 6e63  e of the sequenc
+000077f0: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+00007800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007810: 2020 2020 2020 2020 2020 7c0a 2b2d 2d2d            |.+---
+00007820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00007830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007860: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 6060  ----------+.| ``
+00007870: 666f 726d 6174 6572 6060 207c 2066 6f72  formater`` | for
+00007880: 6d61 7465 7220 6f66 2074 6865 2073 6571  mater of the seq
+00007890: 7565 6e63 6520 2020 2020 2020 2020 2020  uence           
+000078a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078b0: 2020 2020 2020 2020 2020 7c0a 2b2d 2d2d            |.+---
+000078c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+000078d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000078e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000078f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007900: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 0a4f 7468  ----------+..Oth
+00007910: 6572 2061 7474 7269 6275 7465 2066 6f72  er attribute for
+00007920: 2060 6043 6f6c 6f72 6060 3a0a 0a2b 2d2d   ``Color``:..+--
+00007930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+00007940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2050  -----------+.| P
+00007980: 6172 616d 2020 2020 2020 2020 2020 7c20  aram          | 
+00007990: 4465 7363 7269 7074 696f 6e20 2020 2020  Description     
+000079a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000079c0: 2020 2020 2020 2020 2020 207c 0a2b 3d3d             |.+==
+000079d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2b3d  ==============+=
+000079e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000079f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007a00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007a10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 0a7c 2060  ===========+.| `
+00007a20: 6073 697a 6560 6020 2020 2020 2020 7c20  `size``       | 
+00007a30: 636f 6c75 6d6e 206d 6178 2073 697a 6520  column max size 
+00007a40: 696e 2074 6865 2074 6162 6c65 2020 2020  in the table    
+00007a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a60: 2020 2020 2020 2020 2020 207c 0a2b 2d2d             |.+--
+00007a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+00007a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a 4f74  -----------+..Ot
+00007ac0: 6865 7220 6174 7472 6962 7574 6520 666f  her attribute fo
+00007ad0: 7220 6060 5061 7373 776f 7264 6060 3a0a  r ``Password``:.
+00007ae0: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+00007af0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00007b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007b10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00007b30: 0a7c 2050 6172 616d 2020 2020 2020 2020  .| Param        
+00007b40: 2020 2020 207c 2044 6573 6372 6970 7469       | Descripti
+00007b50: 6f6e 2020 2020 2020 2020 2020 2020 2020  on              
+00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b70: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007b80: 0a2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .+==============
+00007b90: 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d 3d3d  =====+==========
+00007ba0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007bb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007bc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b  ===============+
+00007bd0: 0a7c 2060 6073 697a 6560 6020 2020 2020  .| ``size``     
+00007be0: 2020 2020 207c 2070 6173 7377 6f72 6420       | password 
+00007bf0: 6d61 7820 7369 7a65 2069 6e20 7468 6520  max size in the 
+00007c00: 7461 626c 6520 2020 2020 2020 2020 2020  table           
+00007c10: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007c20: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+00007c30: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00007c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00007c70: 0a7c 2060 6063 7279 7074 5f63 6f6e 7465  .| ``crypt_conte
+00007c80: 7874 6060 207c 2073 6565 2074 6865 206f  xt`` | see the o
+00007c90: 7074 696f 6e20 666f 7220 7468 6520 7079  ption for the py
+00007ca0: 7468 6f6e 206c 6962 2060 7061 7373 6c69  thon lib `passli
+00007cb0: 6220 2020 2020 2020 2020 2020 2020 207c  b              |
+00007cc0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00007cd0: 2020 2020 207c 203c 6874 7470 733a 2f2f       | <https://
+00007ce0: 7061 7373 6c69 622e 7265 6164 7468 6564  passlib.readthed
+00007cf0: 6f63 732e 696f 2f65 6e2f 7374 6162 6c65  ocs.io/en/stable
+00007d00: 2f6c 6962 2f70 6173 736c 6962 2e63 6f7c  /lib/passlib.co|
+00007d10: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00007d20: 2020 2020 207c 206e 7465 7874 2e68 746d       | ntext.htm
+00007d30: 6c3e 605f 2020 2020 2020 2020 2020 2020  l>`_            
+00007d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d50: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007d60: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+00007d70: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00007d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00007db0: 0a0a 2e2e 7761 726e 696e 673a 3a0a 0a20  ....warning::.. 
+00007dc0: 2020 2054 6865 2050 6173 7377 6f72 6420     The Password 
+00007dd0: 636f 6c75 6d6e 2063 616e 2062 6520 666f  column can be fo
+00007de0: 756e 6420 7769 7468 2074 6865 2071 7565  und with the que
+00007df0: 7279 206d 6574 683a 0a0a 4f74 6865 7220  ry meth:..Other 
+00007e00: 6174 7472 6962 7574 6520 666f 7220 6060  attribute for ``
+00007e10: 5555 4944 6060 3a0a 0a2b 2d2d 2d2d 2d2d  UUID``:..+------
+00007e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
 00007e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007e40: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
+00007e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00007e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a  -------------+..
-00007e80: 2e2e 7761 726e 696e 673a 3a0a 0a20 2020  ..warning::..   
-00007e90: 2054 6865 2050 6173 7377 6f72 6420 636f   The Password co
-00007ea0: 6c75 6d6e 2063 616e 2062 6520 666f 756e  lumn can be foun
-00007eb0: 6420 7769 7468 2074 6865 2071 7565 7279  d with the query
-00007ec0: 206d 6574 683a 0a0a 4f74 6865 7220 6174   meth:..Other at
-00007ed0: 7472 6962 7574 6520 666f 7220 6060 5555  tribute for ``UU
-00007ee0: 4944 6060 3a0a 0a2b 2d2d 2d2d 2d2d 2d2d  ID``:..+--------
-00007ef0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00007f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007f10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007f30: 2d2d 2d2d 2d2b 0a7c 2050 6172 616d 2020  -----+.| Param  
-00007f40: 2020 2020 2020 2020 7c20 4465 7363 7269          | Descri
-00007f50: 7074 696f 6e20 2020 2020 2020 2020 2020  ption           
-00007f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f80: 2020 2020 207c 0a2b 3d3d 3d3d 3d3d 3d3d       |.+========
-00007f90: 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d  ========+=======
-00007fa0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007fb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007fc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007fd0: 3d3d 3d3d 3d2b 0a7c 2060 6062 696e 6172  =====+.| ``binar
-00007fe0: 7960 6020 2020 2020 7c20 5374 6f72 6573  y``     | Stores
-00007ff0: 2061 2055 5549 4420 696e 2074 6865 2064   a UUID in the d
-00008000: 6174 6162 6173 6520 6e61 7469 7665 6c79  atabase natively
-00008010: 2077 6865 6e20 6974 2063 616e 2061 6e64   when it can and
-00008020: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-00008030: 2020 2020 2020 2020 7c20 6661 6c6c 7320          | falls 
-00008040: 6261 636b 2074 6f20 6120 4249 4e41 5259  back to a BINARY
-00008050: 2831 3629 206f 7220 6120 4348 4152 2833  (16) or a CHAR(3
-00008060: 3229 2020 2020 2020 2020 2020 2020 2020  2)              
-00008070: 2020 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d       |.+--------
-00008080: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00008090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000080a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000080b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000080c0: 2d2d 2d2d 2d2b 0a0a 4f74 6865 7220 6174  -----+..Other at
-000080d0: 7472 6962 7574 6520 666f 7220 6060 4461  tribute for ``Da
-000080e0: 7465 5469 6d65 6060 2061 6e64 2060 6054  teTime`` and ``T
-000080f0: 696d 6553 7461 6d70 6060 3a0a 0a2b 2d2d  imeStamp``:..+--
-00008100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008110: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00008120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2050  -----------+.| P
-00008150: 6172 616d 2020 2020 2020 2020 2020 2020  aram            
-00008160: 2020 2020 7c20 4465 7363 7269 7074 696f      | Descriptio
-00008170: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00008180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008190: 2020 2020 2020 2020 2020 207c 0a2b 3d3d             |.+==
-000081a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000081b0: 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d  ====+===========
-000081c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000081d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000081e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 0a7c 2060  ===========+.| `
-000081f0: 6061 7574 6f5f 7570 6461 7465 6060 2020  `auto_update``  
-00008200: 2020 2020 7c20 426f 6f6c 6561 6e20 2864      | Boolean (d
-00008210: 6566 6175 6c74 3a20 2a2a 4661 6c73 652a  efault: **False*
-00008220: 2a29 2069 6620 5472 7565 2074 6865 2076  *) if True the v
-00008230: 616c 7565 2077 696c 6c20 207c 0a7c 2020  alue will  |.|  
-00008240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008250: 2020 2020 7c20 6265 2075 7064 6174 6520      | be update 
-00008260: 7768 656e 2074 6865 2073 6573 7369 6f6e  when the session
-00008270: 2069 7320 666c 7573 6865 6420 2020 2020   is flushed     
-00008280: 2020 2020 2020 2020 2020 207c 0a2b 2d2d             |.+--
-00008290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000082a0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-000082b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000082c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000082d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2060  -----------+.| `
-000082e0: 6064 6566 6175 6c74 5f74 696d 657a 6f6e  `default_timezon
-000082f0: 6560 6020 7c20 7469 6d65 7a6f 6e65 206f  e`` | timezone o
-00008300: 7220 7469 6d65 7a6f 6e65 2773 206e 616d  r timezone's nam
-00008310: 652c 2064 6566 696e 6520 7468 6520 7469  e, define the ti
-00008320: 6d65 7a6f 6e65 2074 6f20 207c 0a7c 2020  mezone to  |.|  
+00007e60: 2d2d 2d2d 2d2d 2d2b 0a7c 2050 6172 616d  -------+.| Param
+00007e70: 2020 2020 2020 2020 2020 7c20 4465 7363            | Desc
+00007e80: 7269 7074 696f 6e20 2020 2020 2020 2020  ription         
+00007e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007eb0: 2020 2020 2020 207c 0a2b 3d3d 3d3d 3d3d         |.+======
+00007ec0: 3d3d 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d  ==========+=====
+00007ed0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007ee0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007ef0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007f00: 3d3d 3d3d 3d3d 3d2b 0a7c 2060 6062 696e  =======+.| ``bin
+00007f10: 6172 7960 6020 2020 2020 7c20 5374 6f72  ary``     | Stor
+00007f20: 6573 2061 2055 5549 4420 696e 2074 6865  es a UUID in the
+00007f30: 2064 6174 6162 6173 6520 6e61 7469 7665   database native
+00007f40: 6c79 2077 6865 6e20 6974 2063 616e 2061  ly when it can a
+00007f50: 6e64 2020 2020 207c 0a7c 2020 2020 2020  nd     |.|      
+00007f60: 2020 2020 2020 2020 2020 7c20 6661 6c6c            | fall
+00007f70: 7320 6261 636b 2074 6f20 6120 4249 4e41  s back to a BINA
+00007f80: 5259 2831 3629 206f 7220 6120 4348 4152  RY(16) or a CHAR
+00007f90: 2833 3229 2020 2020 2020 2020 2020 2020  (32)            
+00007fa0: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+00007fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00007fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007fd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007ff0: 2d2d 2d2d 2d2d 2d2b 0a0a 4f74 6865 7220  -------+..Other 
+00008000: 6174 7472 6962 7574 6520 666f 7220 6060  attribute for ``
+00008010: 4461 7465 5469 6d65 6060 2061 6e64 2060  DateTime`` and `
+00008020: 6054 696d 6553 7461 6d70 6060 3a0a 0a2b  `TimeStamp``:..+
+00008030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008040: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00008050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
+00008080: 2050 6172 616d 2020 2020 2020 2020 2020   Param          
+00008090: 2020 2020 2020 7c20 4465 7363 7269 7074        | Descript
+000080a0: 696f 6e20 2020 2020 2020 2020 2020 2020  ion             
+000080b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080c0: 2020 2020 2020 2020 2020 2020 207c 0a2b               |.+
+000080d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000080e0: 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d  ======+=========
+000080f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00008100: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00008110: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 0a7c  =============+.|
+00008120: 2060 6061 7574 6f5f 7570 6461 7465 6060   ``auto_update``
+00008130: 2020 2020 2020 7c20 426f 6f6c 6561 6e20        | Boolean 
+00008140: 2864 6566 6175 6c74 3a20 2a2a 4661 6c73  (default: **Fals
+00008150: 652a 2a29 2069 6620 5472 7565 2074 6865  e**) if True the
+00008160: 2076 616c 7565 2077 696c 6c20 207c 0a7c   value will  |.|
+00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008180: 2020 2020 2020 7c20 6265 2075 7064 6174        | be updat
+00008190: 6520 7768 656e 2074 6865 2073 6573 7369  e when the sessi
+000081a0: 6f6e 2069 7320 666c 7573 6865 6420 2020  on is flushed   
+000081b0: 2020 2020 2020 2020 2020 2020 207c 0a2b               |.+
+000081c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000081d0: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+000081e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000081f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
+00008210: 2060 6064 6566 6175 6c74 5f74 696d 657a   ``default_timez
+00008220: 6f6e 6560 6020 7c20 7469 6d65 7a6f 6e65  one`` | timezone
+00008230: 206f 7220 7469 6d65 7a6f 6e65 2773 206e   or timezone's n
+00008240: 616d 652c 2064 6566 696e 6520 7468 6520  ame, define the 
+00008250: 7469 6d65 7a6f 6e65 2074 6f20 207c 0a7c  timezone to  |.|
+00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008270: 2020 2020 2020 7c20 6f6e 206e 6169 7665        | on naive
+00008280: 2064 6174 6574 696d 652e 2020 2020 2020   datetime.      
+00008290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082a0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082c0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+000082d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082f0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00008300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008310: 2020 2020 2020 7c20 2e2e 2077 6172 6e69        | .. warni
+00008320: 6e67 3a3a 2020 2020 2020 2020 2020 2020  ng::            
 00008330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008340: 2020 2020 7c20 6f6e 206e 6169 7665 2064      | on naive d
-00008350: 6174 6574 696d 652e 2020 2020 2020 2020  atetime.        
-00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008370: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-00008380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008390: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00008340: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00008350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008360: 2020 2020 2020 7c20 2020 2020 5468 6520        |     The 
+00008370: 6461 7465 7469 6d65 2077 6974 6820 616e  datetime with an
+00008380: 6f74 6865 7220 7469 6d65 7a6f 6e65 2064  other timezone d
+00008390: 6f6e 2774 2063 6861 6e67 6520 207c 0a7c  on't change  |.|
 000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083c0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083e0: 2020 2020 7c20 2e2e 2077 6172 6e69 6e67      | .. warning
-000083f0: 3a3a 2020 2020 2020 2020 2020 2020 2020  ::              
-00008400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008410: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+000083b0: 2020 2020 2020 7c20 2020 2020 616e 6420        |     and 
+000083c0: 6b65 6570 2074 6865 6972 206f 776e 2074  keep their own t
+000083d0: 696d 657a 6f6e 6520 2020 2020 2020 2020  imezone         
+000083e0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+000083f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008400: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00008410: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008430: 2020 2020 7c20 2020 2020 5468 6520 6461      |     The da
-00008440: 7465 7469 6d65 2077 6974 6820 616e 6f74  tetime with anot
-00008450: 6865 7220 7469 6d65 7a6f 6e65 2064 6f6e  her timezone don
-00008460: 2774 2063 6861 6e67 6520 207c 0a7c 2020  't change  |.|  
+00008430: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00008440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008450: 2020 2020 2020 7c20 3a3a 2020 2020 2020        | ::      
+00008460: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008480: 2020 2020 7c20 2020 2020 616e 6420 6b65      |     and ke
-00008490: 6570 2074 6865 6972 206f 776e 2074 696d  ep their own tim
-000084a0: 657a 6f6e 6520 2020 2020 2020 2020 2020  ezone           
-000084b0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00008480: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00008490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084a0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+000084b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000084c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084d0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+000084d0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008500: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-00008510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008520: 2020 2020 7c20 3a3a 2020 2020 2020 2020      | ::        
+000084f0: 2020 2020 2020 7c20 2020 2020 746f 6b79        |     toky
+00008500: 6f5f 747a 203d 2070 7974 7a2e 7469 6d65  o_tz = pytz.time
+00008510: 7a6f 6e65 2827 4173 6961 2f54 6f6b 796f  zone('Asia/Tokyo
+00008520: 2729 2020 2020 2020 2020 2020 207c 0a7c  ')           |.|
 00008530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008550: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00008540: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00008550: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008570: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00008570: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 00008580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085a0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00008590: 2020 2020 2020 7c20 2020 2020 4072 6567        |     @reg
+000085a0: 6973 7465 7228 4d6f 6465 6c29 2020 2020  ister(Model)    
 000085b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085c0: 2020 2020 7c20 2020 2020 746f 6b79 6f5f      |     tokyo_
-000085d0: 747a 203d 2070 7974 7a2e 7469 6d65 7a6f  tz = pytz.timezo
-000085e0: 6e65 2827 4173 6961 2f54 6f6b 796f 2729  ne('Asia/Tokyo')
-000085f0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+000085c0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+000085d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085e0: 2020 2020 2020 7c20 2020 2020 636c 6173        |     clas
+000085f0: 7320 4261 723a 2020 2020 2020 2020 2020  s Bar:          
 00008600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008610: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00008610: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 00008620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008640: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-00008650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008660: 2020 2020 7c20 2020 2020 4072 6567 6973      |     @regis
-00008670: 7465 7228 4d6f 6465 6c29 2020 2020 2020  ter(Model)      
-00008680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008690: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00008630: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00008640: 666f 6f20 3d20 4461 7465 5469 6d65 2864  foo = DateTime(d
+00008650: 6566 6175 6c74 5f74 696d 657a 6f6e 653d  efault_timezone=
+00008660: 746f 6b79 6f5f 747a 2920 2020 207c 0a7c  tokyo_tz)    |.|
+00008670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008680: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00008690: 2f2f 2020 2020 2020 2020 2020 2020 2020  //              
 000086a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086b0: 2020 2020 7c20 2020 2020 636c 6173 7320      |     class 
-000086c0: 4261 723a 2020 2020 2020 2020 2020 2020  Bar:            
-000086d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086e0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-000086f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008700: 2020 2020 7c20 2020 2020 2020 2020 666f      |         fo
-00008710: 6f20 3d20 4461 7465 5469 6d65 2864 6566  o = DateTime(def
-00008720: 6175 6c74 5f74 696d 657a 6f6e 653d 746f  ault_timezone=to
-00008730: 6b79 6f5f 747a 2920 2020 207c 0a7c 2020  kyo_tz)    |.|  
+000086b0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+000086c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086d0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+000086e0: 666f 6f20 3d20 4461 7465 5469 6d65 2864  foo = DateTime(d
+000086f0: 6566 6175 6c74 5f74 696d 657a 6f6e 653d  efault_timezone=
+00008700: 2741 7369 612f 546f 6b79 6f27 297c 0a7c  'Asia/Tokyo')|.|
+00008710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008720: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00008730: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008750: 2020 2020 7c20 2020 2020 2020 2020 2f2f      |         //
-00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008780: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-00008790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087a0: 2020 2020 7c20 2020 2020 2020 2020 666f      |         fo
-000087b0: 6f20 3d20 4461 7465 5469 6d65 2864 6566  o = DateTime(def
-000087c0: 6175 6c74 5f74 696d 657a 6f6e 653d 2741  ault_timezone='A
-000087d0: 7369 612f 546f 6b79 6f27 297c 0a7c 2020  sia/Tokyo')|.|  
-000087e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087f0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008820: 2020 2020 2020 2020 2020 207c 0a2b 2d2d             |.+--
-00008830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008840: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00008850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a 4f74  -----------+..Ot
-00008880: 6865 7220 6174 7472 6962 7574 6520 666f  her attribute fo
-00008890: 7220 6060 5068 6f6e 654e 756d 6265 7260  r ``PhoneNumber`
-000088a0: 603a 0a0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  `:..+-----------
-000088b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-000088c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000088d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000088e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000088f0: 2d2d 2b0a 7c20 5061 7261 6d20 2020 2020  --+.| Param     
-00008900: 2020 2020 2020 2020 2020 207c 2044 6573             | Des
-00008910: 6372 6970 7469 6f6e 2020 2020 2020 2020  cription        
-00008920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008940: 2020 7c0a 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d    |.+===========
-00008950: 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d  ===========+====
-00008960: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00008970: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00008980: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00008990: 3d3d 2b0a 7c20 6060 7265 6769 6f6e 6060  ==+.| ``region``
-000089a0: 2020 2020 2020 2020 2020 207c 2044 6566             | Def
-000089b0: 6175 6c74 2072 6567 696f 6e20 746f 2073  ault region to s
-000089c0: 6176 6520 7068 6f6e 6520 6e75 6d62 6572  ave phone number
-000089d0: 2028 4652 2920 2020 2020 2020 2020 2020   (FR)           
-000089e0: 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d    |.+-----------
-000089f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00008a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008a30: 2d2d 2b0a 7c20 6060 6d61 785f 6c65 6e67  --+.| ``max_leng
-00008a40: 7468 6060 2020 2020 2020 207c 206d 6178  th``       | max
-00008a50: 2073 697a 6520 6f66 2074 6865 2063 6f6c   size of the col
-00008a60: 756d 6e20 696e 2074 6865 2064 6174 6162  umn in the datab
-00008a70: 6173 6520 2832 3029 2020 2020 2020 2020  ase (20)        
-00008a80: 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d    |.+-----------
-00008a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00008aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008ad0: 2d2d 2b0a 0a52 656c 6174 696f 6e53 6869  --+..RelationShi
-00008ae0: 700a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  p.------------..
-00008af0: 546f 2064 6563 6c61 7265 2061 2060 6052  To declare a ``R
-00008b00: 656c 6174 696f 6e53 6869 7060 6020 696e  elationShip`` in
-00008b10: 2061 206d 6f64 656c 2c20 6164 6420 6120   a model, add a 
-00008b20: 5265 6c61 7469 6f6e 5368 6970 206f 6e20  RelationShip on 
-00008b30: 7468 6520 7461 626c 6520 6f66 0a74 6865  the table of.the
-00008b40: 206d 6f64 656c 2e3a 3a0a 0a20 2020 2066   model.::..    f
-00008b50: 726f 6d20 616e 7962 6c6f 6b2e 6465 636c  rom anyblok.decl
-00008b60: 6172 6174 696f 6e73 2069 6d70 6f72 7420  arations import 
-00008b70: 4465 636c 6172 6174 696f 6e73 0a20 2020  Declarations.   
-00008b80: 2066 726f 6d20 616e 7962 6c6f 6b2e 636f   from anyblok.co
-00008b90: 6c75 6d6e 2069 6d70 6f72 7420 496e 7465  lumn import Inte
-00008ba0: 6765 720a 2020 2020 6672 6f6d 2061 6e79  ger.    from any
-00008bb0: 626c 6f6b 2e72 656c 6174 696f 6e73 6869  blok.relationshi
-00008bc0: 7020 696d 706f 7274 204d 616e 7932 4f6e  p import Many2On
-00008bd0: 650a 0a0a 2020 2020 4044 6563 6c61 7261  e...    @Declara
-00008be0: 7469 6f6e 732e 7265 6769 7374 6572 2844  tions.register(D
-00008bf0: 6563 6c61 7261 7469 6f6e 2e4d 6f64 656c  eclaration.Model
-00008c00: 290a 2020 2020 636c 6173 7320 4d79 4d6f  ).    class MyMo
-00008c10: 6465 6c3a 0a0a 2020 2020 2020 2020 6964  del:..        id
-00008c20: 203d 2049 6e74 6567 6572 2870 7269 6d61   = Integer(prima
-00008c30: 7279 5f6b 6579 3d54 7275 6529 0a0a 0a20  ry_key=True)... 
-00008c40: 2020 2040 4465 636c 6172 6174 696f 6e73     @Declarations
-00008c50: 2e72 6567 6973 7465 7228 4465 636c 6172  .register(Declar
-00008c60: 6174 696f 6e2e 4d6f 6465 6c29 0a20 2020  ation.Model).   
-00008c70: 2063 6c61 7373 204d 794d 6f64 656c 323a   class MyModel2:
-00008c80: 0a0a 2020 2020 2020 2020 6964 203d 2049  ..        id = I
-00008c90: 6e74 6567 6572 2870 7269 6d61 7279 5f6b  nteger(primary_k
-00008ca0: 6579 3d54 7275 6529 0a20 2020 2020 2020  ey=True).       
-00008cb0: 206d 796d 6f64 656c 203d 204d 616e 7932   mymodel = Many2
-00008cc0: 4f6e 6528 6d6f 6465 6c3d 4465 636c 6172  One(model=Declar
-00008cd0: 6174 696f 6e2e 4d6f 6465 6c2e 4d79 4d6f  ation.Model.MyMo
-00008ce0: 6465 6c29 0a0a 2e2e 206e 6f74 653a 3a0a  del).... note::.
-00008cf0: 0a20 2020 2053 696e 6365 2074 6865 2076  .    Since the v
-00008d00: 6572 7369 6f6e 2030 2e34 2e30 2074 6865  ersion 0.4.0 the
-00008d10: 2060 6052 656c 6174 696f 6e53 6869 7060   ``RelationShip`
-00008d20: 6020 646f 6e27 7420 636f 6d65 2066 726f  ` don't come fro
-00008d30: 6d20 6060 4465 636c 6172 6174 696f 6e73  m ``Declarations
-00008d40: 6060 0a0a 4c69 7374 206f 6620 7468 6520  ``..List of the 
-00008d50: 5265 6c61 7469 6f6e 5368 6970 2074 7970  RelationShip typ
-00008d60: 653a 0a0a 2a20 6060 4f6e 6532 4f6e 6560  e:..* ``One2One`
-00008d70: 600a 2a20 6060 4d61 6e79 324f 6e65 6060  `.* ``Many2One``
-00008d80: 0a2a 2060 604f 6e65 324d 616e 7960 600a  .* ``One2Many``.
-00008d90: 2a20 6060 4d61 6e79 324d 616e 7960 600a  * ``Many2Many``.
-00008da0: 0a50 6172 616d 6574 6572 7320 6f66 2061  .Parameters of a
-00008db0: 2060 6052 656c 6174 696f 6e53 6869 7060   ``RelationShip`
-00008dc0: 603a 0a0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  `:..+-----------
-00008dd0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00008de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008e10: 2d2d 2b0a 7c20 5061 7261 6d20 2020 2020  --+.| Param     
-00008e20: 2020 2020 2020 2020 207c 2044 6573 6372           | Descr
-00008e30: 6970 7469 6f6e 2020 2020 2020 2020 2020  iption          
-00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008750: 2020 2020 2020 2020 2020 2020 207c 0a2b               |.+
+00008760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008770: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00008780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000087a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a  -------------+..
+000087b0: 4f74 6865 7220 6174 7472 6962 7574 6520  Other attribute 
+000087c0: 666f 7220 6060 5068 6f6e 654e 756d 6265  for ``PhoneNumbe
+000087d0: 7260 603a 0a0a 2b2d 2d2d 2d2d 2d2d 2d2d  r``:..+---------
+000087e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+000087f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008820: 2d2d 2d2d 2b0a 7c20 5061 7261 6d20 2020  ----+.| Param   
+00008830: 2020 2020 2020 2020 2020 2020 207c 2044               | D
+00008840: 6573 6372 6970 7469 6f6e 2020 2020 2020  escription      
+00008850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008870: 2020 2020 7c0a 2b3d 3d3d 3d3d 3d3d 3d3d      |.+=========
+00008880: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d  =============+==
+00008890: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000088a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000088b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000088c0: 3d3d 3d3d 2b0a 7c20 6060 7265 6769 6f6e  ====+.| ``region
+000088d0: 6060 2020 2020 2020 2020 2020 207c 2044  ``           | D
+000088e0: 6566 6175 6c74 2072 6567 696f 6e20 746f  efault region to
+000088f0: 2073 6176 6520 7068 6f6e 6520 6e75 6d62   save phone numb
+00008900: 6572 2028 4652 2920 2020 2020 2020 2020  er (FR)         
+00008910: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
+00008920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00008930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008960: 2d2d 2d2d 2b0a 7c20 6060 6d61 785f 6c65  ----+.| ``max_le
+00008970: 6e67 7468 6060 2020 2020 2020 207c 206d  ngth``       | m
+00008980: 6178 2073 697a 6520 6f66 2074 6865 2063  ax size of the c
+00008990: 6f6c 756d 6e20 696e 2074 6865 2064 6174  olumn in the dat
+000089a0: 6162 6173 6520 2832 3029 2020 2020 2020  abase (20)      
+000089b0: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
+000089c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+000089d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000089e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000089f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008a00: 2d2d 2d2d 2b0a 0a4f 7468 6572 2061 7474  ----+..Other att
+00008a10: 7269 6275 7465 2066 6f72 2060 6043 6f75  ribute for ``Cou
+00008a20: 6e74 7279 6060 3a0a 0a2b 2d2d 2d2d 2d2d  ntry``:..+------
+00008a30: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00008a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008a70: 2d2d 2d2d 2d2d 2d2b 0a7c 2050 6172 616d  -------+.| Param
+00008a80: 2020 2020 207c 2044 6573 6372 6970 7469       | Descripti
+00008a90: 6f6e 2020 2020 2020 2020 2020 2020 2020  on              
+00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ac0: 2020 2020 2020 207c 0a2b 3d3d 3d3d 3d3d         |.+======
+00008ad0: 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d 3d3d  =====+==========
+00008ae0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00008af0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00008b00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00008b10: 3d3d 3d3d 3d3d 3d2b 0a7c 2060 606d 6f64  =======+.| ``mod
+00008b20: 6560 6020 207c 2044 6566 696e 6520 7468  e``  | Define th
+00008b30: 6520 6d6f 6465 2062 7920 6465 6661 756c  e mode by defaul
+00008b40: 7420 746f 2073 746f 7265 2069 6e20 7468  t to store in th
+00008b50: 6520 4442 2028 6465 6661 756c 7420 616c  e DB (default al
+00008b60: 7068 615f 3229 207c 0a2b 2d2d 2d2d 2d2d  pha_2) |.+------
+00008b70: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00008b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008bb0: 2d2d 2d2d 2d2d 2d2b 0a0a 4f74 6865 7220  -------+..Other 
+00008bc0: 6174 7472 6962 7574 6520 666f 7220 6060  attribute for ``
+00008bd0: 4d6f 6465 6c53 656c 6563 7469 6f6e 6060  ModelSelection``
+00008be0: 3a0a 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :..+------------
+00008bf0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+00008c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008c30: 2d2b 0a7c 2050 6172 616d 2020 2020 2020  -+.| Param      
+00008c40: 2020 2020 7c20 4465 7363 7269 7074 696f      | Descriptio
+00008c50: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00008c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c80: 207c 0a2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   |.+============
+00008c90: 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d  ====+===========
+00008ca0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00008cb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00008cc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00008cd0: 3d2b 0a7c 2060 6076 616c 6964 6174 6f72  =+.| ``validator
+00008ce0: 6060 2020 7c20 6675 6e63 7469 6f6e 206f  ``  | function o
+00008cf0: 7220 6e61 6d65 206f 6620 7468 6520 6d65  r name of the me
+00008d00: 7468 6f64 206f 6e20 7468 6520 4d6f 6465  thod on the Mode
+00008d10: 6c2e 2074 6865 6972 2067 6f61 6c20 2020  l. their goal   
+00008d20: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00008d30: 2020 2020 7c20 6973 2074 6f20 6465 6669      | is to defi
+00008d40: 6e65 6420 7768 6963 6820 6d6f 6465 6c73  ned which models
+00008d50: 2063 616e 2062 6520 7573 6564 2e20 536f   can be used. So
+00008d60: 6d65 2066 756e 6374 696f 6e20 2020 2020  me function     
+00008d70: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00008d80: 2020 2020 7c20 6578 6973 7420 696e 2061      | exist in a
+00008d90: 6e79 626c 6f6b 2e63 6f6c 756d 6e3a 2020  nyblok.column:  
+00008da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008dc0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00008dd0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00008de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e10: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00008e20: 2020 2020 7c20 2a20 6d6f 6465 6c5f 7661      | * model_va
+00008e30: 6c69 6461 746f 725f 616c 6c3a 2041 6c6c  lidator_all: All
+00008e40: 206d 6f64 656c 7320 2020 2020 2020 2020   models         
 00008e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e60: 2020 7c0a 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d    |.+===========
-00008e70: 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d  =========+======
-00008e80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00008e90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00008ea0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00008eb0: 3d3d 2b0a 7c20 6060 6c61 6265 6c60 6020  ==+.| ``label`` 
-00008ec0: 2020 2020 2020 2020 207c 2054 6865 206c           | The l
-00008ed0: 6162 656c 206f 6620 7468 6520 636f 6c75  abel of the colu
-00008ee0: 6d6e 2020 2020 2020 2020 2020 2020 2020  mn              
-00008ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f00: 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d    |.+-----------
-00008f10: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00008f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008f50: 2d2d 2b0a 7c20 6060 6d6f 6465 6c60 6020  --+.| ``model`` 
-00008f60: 2020 2020 2020 2020 207c 2054 6865 2072           | The r
-00008f70: 656d 6f74 6520 6d6f 6465 6c20 2020 2020  emote model     
-00008f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fa0: 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d    |.+-----------
-00008fb0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00008fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008fd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008ff0: 2d2d 2b0a 7c20 6060 7265 6d6f 7465 5f63  --+.| ``remote_c
-00009000: 6f6c 756d 6e73 6060 207c 2054 6865 2063  olumns`` | The c
-00009010: 6f6c 756d 6e20 6e61 6d65 206f 6e20 7468  olumn name on th
-00009020: 6520 7265 6d6f 7465 206d 6f64 656c 2c20  e remote model, 
-00009030: 6966 206e 6f20 7265 6d6f 7465 2020 2020  if no remote    
-00009040: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-00009050: 2020 2020 2020 2020 207c 2063 6f6c 756d           | colum
-00009060: 6e73 2061 7265 2064 6566 696e 6564 2074  ns are defined t
-00009070: 6865 2072 656d 6f74 6520 636f 6c75 6d6e  he remote column
-00009080: 2077 696c 6c20 6265 2074 6865 2020 2020   will be the    
-00009090: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-000090a0: 2020 2020 2020 2020 207c 2070 7269 6d61           | prima
-000090b0: 7279 2063 6f6c 756d 6e20 6f66 2074 6865  ry column of the
-000090c0: 2072 656d 6f74 6520 6d6f 6465 6c20 2020   remote model   
+00008e60: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00008e70: 2020 2020 7c20 2a20 6d6f 6465 6c5f 7661      | * model_va
+00008e80: 6c69 6461 746f 725f 6973 5f73 716c 3a20  lidator_is_sql: 
+00008e90: 4f6e 6c79 2053 514c 206d 6f64 656c 7320  Only SQL models 
+00008ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008eb0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00008ec0: 2020 2020 7c20 2a20 6d6f 6465 6c5f 7661      | * model_va
+00008ed0: 6c69 6461 746f 725f 6973 5f6e 6f74 5f73  lidator_is_not_s
+00008ee0: 716c 3a20 4e6f 7420 7468 6520 5351 4c20  ql: Not the SQL 
+00008ef0: 6d6f 6465 6c73 2020 2020 2020 2020 2020  models          
+00008f00: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00008f10: 2020 2020 7c20 2a20 6d6f 6465 6c5f 7661      | * model_va
+00008f20: 6c69 6461 746f 725f 6973 5f76 6965 773a  lidator_is_view:
+00008f30: 204f 6e6c 7920 6d6f 6465 6c73 2077 6974   Only models wit
+00008f40: 6820 6661 6374 6f72 7920 7669 6577 2020  h factory view  
+00008f50: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00008f60: 2020 2020 7c20 2a20 6d6f 6465 6c5f 7661      | * model_va
+00008f70: 6c69 6461 746f 725f 6973 5f6e 6f74 5f76  lidator_is_not_v
+00008f80: 6965 773a 204e 6f74 2074 6865 206d 6f64  iew: Not the mod
+00008f90: 656c 2077 6974 6820 6661 6374 6f72 7920  el with factory 
+00008fa0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00008fb0: 2020 2020 7c20 2020 7669 6577 2020 2020      |   view    
+00008fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ff0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00009000: 2020 2020 7c20 2a20 6d6f 6465 6c5f 7661      | * model_va
+00009010: 6c69 6461 746f 725f 696e 5f6e 616d 6573  lidator_in_names
+00009020: 7061 6365 3a20 6669 6c74 6572 2062 7920  pace: filter by 
+00009030: 6e61 6d65 7370 6163 6520 2020 2020 2020  namespace       
+00009040: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00009050: 2020 2020 7c20 2a20 6d65 7267 655f 7661      | * merge_va
+00009060: 6c69 6461 746f 7273 3a20 446f 2061 2061  lidators: Do a a
+00009070: 6e64 2062 6574 7765 656e 2076 616c 6964  nd between valid
+00009080: 6174 6f72 7320 2020 2020 2020 2020 2020  ators           
+00009090: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+000090a0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+000090b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000090d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090e0: 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d    |.+-----------
-000090f0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+000090e0: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
+000090f0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
 00009100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00009110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00009120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009130: 2d2d 2b0a 0a50 6172 616d 6574 6572 7320  --+..Parameters 
-00009140: 6f66 2074 6865 2060 604f 6e65 324f 6e65  of the ``One2One
-00009150: 6060 2066 6965 6c64 3a0a 0a2b 2d2d 2d2d  `` field:..+----
-00009160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00009170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009130: 2d2b 0a0a 4f74 6865 7220 6174 7472 6962  -+..Other attrib
+00009140: 7574 6520 666f 7220 6060 4d6f 6465 6c46  ute for ``ModelF
+00009150: 6965 6c64 5365 6c65 6374 696f 6e60 603a  ieldSelection``:
+00009160: 0a0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..+-------------
+00009170: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
 00009180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00009190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000091a0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2050 6172  ---------+.| Par
-000091b0: 616d 2020 2020 2020 2020 2020 2020 207c  am             |
-000091c0: 2044 6573 6372 6970 7469 6f6e 2020 2020   Description    
-000091d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000091b0: 2b0a 7c20 5061 7261 6d20 2020 2020 2020  +.| Param       
+000091c0: 2020 2020 2020 2020 7c20 4465 7363 7269          | Descri
+000091d0: 7074 696f 6e20 2020 2020 2020 2020 2020  ption           
 000091e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091f0: 2020 2020 2020 2020 207c 0a2b 3d3d 3d3d           |.+====
-00009200: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b  ===============+
-00009210: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000091f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009200: 7c0a 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  |.+=============
+00009210: 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d 3d3d 3d3d  ========+=======
 00009220: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00009230: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00009240: 3d3d 3d3d 3d3d 3d3d 3d2b 0a7c 2060 6063  =========+.| ``c
-00009250: 6f6c 756d 6e5f 6e61 6d65 7360 6020 207c  olumn_names``  |
-00009260: 204e 616d 6520 6f66 2074 6865 206c 6f63   Name of the loc
-00009270: 616c 2063 6f6c 756d 6e2e 2020 2020 2020  al column.      
-00009280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009290: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-000092a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000092b0: 2049 6620 7468 6520 636f 6c75 6d6e 2064   If the column d
-000092c0: 6f65 736e 2774 2065 7869 7374 2074 6865  oesn't exist the
-000092d0: 6e20 7468 6973 2063 6f6c 756d 6e20 7769  n this column wi
-000092e0: 6c6c 2062 6520 2020 207c 0a7c 2020 2020  ll be    |.|    
-000092f0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00009300: 2063 7265 6174 6564 2e20 2020 2020 2020   created.       
-00009310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009330: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00009340: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00009350: 2049 6620 6e6f 2063 6f6c 756d 6e20 6e61   If no column na
-00009360: 6d65 2074 6865 6e20 7468 6520 6e61 6d65  me then the name
-00009370: 2077 696c 6c20 6265 2027 4d32 4f20 6e61   will be 'M2O na
-00009380: 6d65 2720 2b20 2020 207c 0a7c 2020 2020  me' +    |.|    
-00009390: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000093a0: 2027 5f27 202b 2027 6e61 6d65 206f 6620   '_' + 'name of 
-000093b0: 7468 6520 7265 6d6f 7465 2063 6f6c 756d  the remote colum
-000093c0: 6e27 2020 2020 2020 2020 2020 2020 2020  n'              
-000093d0: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
-000093e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-000093f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009420: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2060 606e  ---------+.| ``n
-00009430: 756c 6c61 626c 6560 6020 2020 2020 207c  ullable``      |
-00009440: 2049 6e64 6963 6174 6573 2069 6620 7468   Indicates if th
-00009450: 6520 636f 6c75 6d6e 206e 616d 6520 6973  e column name is
-00009460: 206e 756c 6c61 626c 6520 6f72 206e 6f74   nullable or not
-00009470: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
-00009480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00009490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000094a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000094b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000094c0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6062  ---------+.| ``b
-000094d0: 6163 6b72 6566 6060 2020 2020 2020 207c  ackref``       |
-000094e0: 2052 656d 6f74 6520 4f6e 6532 4f6e 6520   Remote One2One 
-000094f0: 6c69 6e6b 2077 6974 6820 7468 6520 636f  link with the co
-00009500: 6c75 6d6e 206e 616d 6520 2020 2020 2020  lumn name       
-00009510: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
-00009520: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00009530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009560: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6075  ---------+.| ``u
-00009570: 6e69 7175 6560 6020 2020 2020 2020 207c  nique``        |
-00009580: 2041 6464 2075 6e69 7175 6520 636f 6e73   Add unique cons
-00009590: 7472 6169 6e74 206f 6e20 7468 6520 6372  traint on the cr
-000095a0: 6561 7465 6420 636f 6c75 6d6e 2873 2920  eated column(s) 
-000095b0: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
-000095c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-000095d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000095e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000095f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009600: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6069  ---------+.| ``i
-00009610: 6e64 6578 6060 2020 2020 2020 2020 207c  ndex``         |
-00009620: 2041 6464 2069 6e64 6578 2063 6f6e 7374   Add index const
-00009630: 7261 696e 7420 6f6e 2074 6865 2063 7265  raint on the cre
-00009640: 6174 6564 2063 6f6c 756d 6e28 7329 2020  ated column(s)  
-00009650: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
-00009660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00009670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000096a0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6070  ---------+.| ``p
-000096b0: 7269 6d61 7279 5f6b 6579 6060 2020 207c  rimary_key``   |
-000096c0: 2054 6865 2063 7265 6174 6564 2063 6f6c   The created col
-000096d0: 756d 6e28 7329 2061 7265 2070 7269 6d61  umn(s) are prima
-000096e0: 7279 206b 6579 2020 2020 2020 2020 2020  ry key          
-000096f0: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
-00009700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00009710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009740: 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a 5061 7261  ---------+..Para
-00009750: 6d65 7465 7273 206f 6620 7468 6520 6060  meters of the ``
-00009760: 4d61 6e79 324f 6e65 6060 2066 6965 6c64  Many2One`` field
-00009770: 3a0a 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :..+------------
-00009780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-00009790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000097a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000097b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000097c0: 2d2b 0a7c 2050 6172 616d 6574 6572 2020  -+.| Parameter  
-000097d0: 2020 2020 2020 2020 2020 2020 207c 2044               | D
-000097e0: 6573 6372 6970 7469 6f6e 2020 2020 2020  escription      
-000097f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009810: 207c 0a2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   |.+============
-00009820: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d  =============+==
-00009830: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00009840: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00009850: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00009860: 3d2b 0a7c 2060 6063 6f6c 756d 6e5f 6e61  =+.| ``column_na
-00009870: 6d65 7360 6020 2020 2020 2020 207c 204e  mes``        | N
-00009880: 616d 6520 6f66 2074 6865 206c 6f63 616c  ame of the local
-00009890: 2063 6f6c 756d 6e2e 2020 2020 2020 2020   column.        
-000098a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098b0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-000098c0: 2020 2020 2020 2020 2020 2020 207c 2049               | I
-000098d0: 6620 7468 6520 636f 6c75 6d6e 2064 6f65  f the column doe
-000098e0: 736e 2774 2065 7869 7374 2074 6865 6e20  sn't exist then 
-000098f0: 7468 6973 2063 6f6c 756d 6e20 7769 6c6c  this column will
-00009900: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00009910: 2020 2020 2020 2020 2020 2020 207c 2062               | b
-00009920: 6520 6372 6561 7465 642e 2020 2020 2020  e created.      
-00009930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009950: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00009960: 2020 2020 2020 2020 2020 2020 207c 2049               | I
-00009970: 6620 6e6f 2063 6f6c 756d 6e20 6e61 6d65  f no column name
-00009980: 2074 6865 6e20 7468 6520 6e61 6d65 2077   then the name w
-00009990: 696c 6c20 6265 2020 2020 2020 2020 2020  ill be          
-000099a0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-000099b0: 2020 2020 2020 2020 2020 2020 207c 2027               | '
-000099c0: 4d32 4f20 6e61 6d65 2720 2b20 275f 2720  M2O name' + '_' 
-000099d0: 2b20 276e 616d 6520 6f66 2074 6865 2072  + 'name of the r
-000099e0: 656d 6f74 6520 636f 6c75 6d6e 2720 2020  emote column'   
-000099f0: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
-00009a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-00009a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009a40: 2d2b 0a7c 2060 606e 756c 6c61 626c 6560  -+.| ``nullable`
-00009a50: 6020 2020 2020 2020 2020 2020 207c 2049  `            | I
-00009a60: 6e64 6963 6174 6520 6966 2074 6865 2063  ndicate if the c
-00009a70: 6f6c 756d 6e20 6e61 6d65 2069 7320 6e75  olumn name is nu
-00009a80: 6c6c 6162 6c65 206f 7220 6e6f 7420 2020  llable or not   
-00009a90: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
-00009aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-00009ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009ae0: 2d2b 0a7c 2060 6075 6e69 7175 6560 6020  -+.| ``unique`` 
-00009af0: 2020 2020 2020 2020 2020 2020 207c 2041               | A
-00009b00: 6464 2075 6e69 7175 6520 636f 6e73 7472  dd unique constr
-00009b10: 6169 6e74 206f 6e20 7468 6520 6372 6561  aint on the crea
-00009b20: 7465 6420 636f 6c75 6d6e 2873 2920 2020  ted column(s)   
-00009b30: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
-00009b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-00009b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009b80: 2d2b 0a7c 2060 6069 6e64 6578 6060 2020  -+.| ``index``  
-00009b90: 2020 2020 2020 2020 2020 2020 207c 2041               | A
-00009ba0: 6464 2069 6e64 6578 2063 6f6e 7374 7261  dd index constra
-00009bb0: 696e 7420 6f6e 2074 6865 2063 7265 6174  int on the creat
-00009bc0: 6564 2063 6f6c 756d 6e28 7329 2020 2020  ed column(s)    
-00009bd0: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
-00009be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-00009bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009c20: 2d2b 0a7c 2060 6070 7269 6d61 7279 5f6b  -+.| ``primary_k
-00009c30: 6579 6060 2020 2020 2020 2020 207c 2054  ey``         | T
-00009c40: 6865 2063 7265 6174 6564 2063 6f6c 756d  he created colum
-00009c50: 6e28 7329 2061 7265 2070 7269 6d61 7279  n(s) are primary
-00009c60: 206b 6579 2020 2020 2020 2020 2020 2020   key            
-00009c70: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
-00009c80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-00009c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009cc0: 2d2b 0a7c 2060 606f 6e65 326d 616e 7960  -+.| ``one2many`
-00009cd0: 6020 2020 2020 2020 2020 2020 207c 204f  `            | O
-00009ce0: 7070 6f73 6974 6520 4f6e 6532 4d61 6e79  pposite One2Many
-00009cf0: 206c 696e 6b20 7769 7468 2074 6869 7320   link with this 
-00009d00: 4d61 6e79 326f 6e65 2020 2020 2020 2020  Many2one        
-00009d10: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
-00009d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-00009d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009d60: 2d2b 0a7c 2060 6066 6f72 6569 676e 5f6b  -+.| ``foreign_k
-00009d70: 6579 5f6f 7074 696f 6e73 6060 207c 2074  ey_options`` | t
-00009d80: 616b 6520 6120 6469 6374 2077 6974 6820  ake a dict with 
-00009d90: 7468 6520 6f70 7469 6f6e 2066 6f72 2063  the option for c
-00009da0: 7265 6174 6520 7468 6520 2020 2020 2020  reate the       
-00009db0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00009dc0: 2020 2020 2020 2020 2020 2020 207c 2066               | f
-00009dd0: 6f72 6569 676e 206b 6579 2020 2020 2020  oreign key      
-00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e00: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
-00009e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-00009e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009e50: 2d2b 0a0a 3a3a 0a0a 2020 2020 4d61 6e79  -+..::..    Many
-00009e60: 324f 6e65 286d 6f64 656c 3d54 6865 2e4d  2One(model=The.M
-00009e70: 6f64 656c 2c20 6e75 6c6c 6162 6c65 3d54  odel, nullable=T
-00009e80: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00009e90: 2020 666f 7265 6967 6e5f 6b65 795f 6f70    foreign_key_op
-00009ea0: 7469 6f6e 733d 7b27 6f6e 6465 6c65 7465  tions={'ondelete
-00009eb0: 273a 2027 6361 7363 6164 6527 7d29 0a0a  ': 'cascade'})..
-00009ec0: 0a0a 5061 7261 6d65 7465 7273 206f 6620  ..Parameters of 
-00009ed0: 7468 6520 6060 4f6e 6532 4d61 6e79 6060  the ``One2Many``
-00009ee0: 2066 6965 6c64 3a0a 0a2b 2d2d 2d2d 2d2d   field:..+------
-00009ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-00009f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009f10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009f30: 2d2d 2d2d 2d2d 2d2b 0a7c 2050 6172 616d  -------+.| Param
-00009f40: 6574 6572 2020 2020 2020 2020 207c 2044  eter         | D
-00009f50: 6573 6372 6970 7469 6f6e 2020 2020 2020  escription      
-00009f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f80: 2020 2020 2020 207c 0a2b 3d3d 3d3d 3d3d         |.+======
-00009f90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d  =============+==
-00009fa0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00009fb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00009fc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00009fd0: 3d3d 3d3d 3d3d 3d2b 0a7c 2060 6070 7269  =======+.| ``pri
-00009fe0: 6d61 7279 6a6f 696e 6060 2020 207c 204a  maryjoin``   | J
-00009ff0: 6f69 6e20 636f 6e64 6974 696f 6e20 6265  oin condition be
-0000a000: 7477 6565 6e20 7468 6520 7265 6c61 7469  tween the relati
-0000a010: 6f6e 7368 6970 2061 6e64 2074 6865 2072  onship and the r
-0000a020: 656d 6f74 6520 207c 0a7c 2020 2020 2020  emote  |.|      
-0000a030: 2020 2020 2020 2020 2020 2020 207c 2063               | c
-0000a040: 6f6c 756d 6e20 2020 2020 2020 2020 2020  olumn           
-0000a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009240: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00009250: 2b0a 7c20 6060 6d6f 6465 6c5f 7661 6c69  +.| ``model_vali
+00009260: 6461 746f 7260 6020 7c20 6675 6e63 7469  dator`` | functi
+00009270: 6f6e 206f 7220 6e61 6d65 206f 6620 7468  on or name of th
+00009280: 6520 6d65 7468 6f64 206f 6e20 7468 6520  e method on the 
+00009290: 4d6f 6465 6c2e 2074 6865 6972 2020 2020  Model. their    
+000092a0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+000092b0: 2020 2020 2020 2020 7c20 676f 616c 2069          | goal i
+000092c0: 7320 746f 2064 6566 696e 6564 2077 6869  s to defined whi
+000092d0: 6368 206d 6f64 656c 7320 6361 6e20 6265  ch models can be
+000092e0: 2075 7365 642e 2053 6f6d 6520 2020 2020   used. Some     
+000092f0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009300: 2020 2020 2020 2020 7c20 6675 6e63 7469          | functi
+00009310: 6f6e 2065 7869 7374 2069 6e20 616e 7962  on exist in anyb
+00009320: 6c6f 6b2e 636f 6c75 6d6e 3a20 2020 2020  lok.column:     
+00009330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009340: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009350: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00009360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009390: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+000093a0: 2020 2020 2020 2020 7c20 2a20 6d6f 6465          | * mode
+000093b0: 6c5f 7661 6c69 6461 746f 725f 616c 6c3a  l_validator_all:
+000093c0: 2041 6c6c 206d 6f64 656c 7320 2020 2020   All models     
+000093d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093e0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+000093f0: 2020 2020 2020 2020 7c20 2a20 6d6f 6465          | * mode
+00009400: 6c5f 7661 6c69 6461 746f 725f 6973 5f73  l_validator_is_s
+00009410: 716c 3a20 4f6e 6c79 2053 514c 206d 6f64  ql: Only SQL mod
+00009420: 656c 7320 2020 2020 2020 2020 2020 2020  els             
+00009430: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009440: 2020 2020 2020 2020 7c20 2a20 6d6f 6465          | * mode
+00009450: 6c5f 7661 6c69 6461 746f 725f 6973 5f6e  l_validator_is_n
+00009460: 6f74 5f73 716c 3a20 4e6f 7420 7468 6520  ot_sql: Not the 
+00009470: 5351 4c20 6d6f 6465 6c73 2020 2020 2020  SQL models      
+00009480: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009490: 2020 2020 2020 2020 7c20 2a20 6d6f 6465          | * mode
+000094a0: 6c5f 7661 6c69 6461 746f 725f 6973 5f76  l_validator_is_v
+000094b0: 6965 773a 204f 6e6c 7920 6d6f 6465 6c73  iew: Only models
+000094c0: 2077 6974 6820 6661 6374 6f72 7920 2020   with factory   
+000094d0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+000094e0: 2020 2020 2020 2020 7c20 2020 7669 6577          |   view
+000094f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009520: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009530: 2020 2020 2020 2020 7c20 2a20 6d6f 6465          | * mode
+00009540: 6c5f 7661 6c69 6461 746f 725f 6973 5f6e  l_validator_is_n
+00009550: 6f74 5f76 6965 773a 204e 6f74 2074 6865  ot_view: Not the
+00009560: 206d 6f64 656c 2077 6974 6820 2020 2020   model with     
+00009570: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009580: 2020 2020 2020 2020 7c20 2020 6661 6374          |   fact
+00009590: 6f72 7920 7669 6577 2020 2020 2020 2020  ory view        
+000095a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095c0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+000095d0: 2020 2020 2020 2020 7c20 2a20 6d6f 6465          | * mode
+000095e0: 6c5f 7661 6c69 6461 746f 725f 696e 5f6e  l_validator_in_n
+000095f0: 616d 6573 7061 6365 3a20 6669 6c74 6572  amespace: filter
+00009600: 2062 7920 6e61 6d65 7370 6163 6520 2020   by namespace   
+00009610: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009620: 2020 2020 2020 2020 7c20 2a20 6d65 7267          | * merg
+00009630: 655f 7661 6c69 6461 746f 7273 3a20 446f  e_validators: Do
+00009640: 2061 2061 6e64 2062 6574 7765 656e 2076   a and between v
+00009650: 616c 6964 6174 6f72 7320 2020 2020 2020  alidators       
+00009660: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009670: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00009680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096b0: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.+-------------
+000096c0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+000096d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000096e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000096f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009700: 2b0a 7c20 6060 6669 656c 645f 7661 6c69  +.| ``field_vali
+00009710: 6461 746f 7260 6020 7c20 6675 6e63 7469  dator`` | functi
+00009720: 6f6e 206f 7220 6e61 6d65 206f 6620 7468  on or name of th
+00009730: 6520 6d65 7468 6f64 206f 6e20 7468 6520  e method on the 
+00009740: 4d6f 6465 6c2e 2074 6865 6972 2020 2020  Model. their    
+00009750: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009760: 2020 2020 2020 2020 7c20 676f 616c 2069          | goal i
+00009770: 7320 746f 2064 6566 696e 6564 2077 6869  s to defined whi
+00009780: 6368 2066 6965 6c64 2063 616e 2062 6520  ch field can be 
+00009790: 7573 6564 2e20 536f 6d65 2020 2020 2020  used. Some      
+000097a0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+000097b0: 2020 2020 2020 2020 7c20 6675 6e63 7469          | functi
+000097c0: 6f6e 2065 7869 7374 2069 6e20 616e 7962  on exist in anyb
+000097d0: 6c6f 6b2e 636f 6c75 6d6e 3a20 2020 2020  lok.column:     
+000097e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097f0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009800: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009840: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009850: 2020 2020 2020 2020 7c20 2a20 6669 656c          | * fiel
+00009860: 645f 7661 6c69 6461 746f 725f 616c 6c3a  d_validator_all:
+00009870: 2041 6c6c 2066 6965 6c64 7320 6f6e 2074   All fields on t
+00009880: 6865 206d 6f64 656c 2020 2020 2020 2020  he model        
+00009890: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+000098a0: 2020 2020 2020 2020 7c20 2a20 6669 656c          | * fiel
+000098b0: 645f 7661 6c69 6461 746f 725f 6973 5f66  d_validator_is_f
+000098c0: 6965 6c64 3a20 4f6e 6c79 206e 6f20 5351  ield: Only no SQ
+000098d0: 4c20 6669 656c 6420 2020 2020 2020 2020  L field         
+000098e0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+000098f0: 2020 2020 2020 2020 7c20 2a20 6669 656c          | * fiel
+00009900: 645f 7661 6c69 6461 746f 725f 6973 5f6e  d_validator_is_n
+00009910: 6f74 5f66 6965 6c64 3a20 4e6f 7420 7468  ot_field: Not th
+00009920: 6520 5351 4c20 6669 656c 6473 2020 2020  e SQL fields    
+00009930: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009940: 2020 2020 2020 2020 7c20 2a20 6669 656c          | * fiel
+00009950: 645f 7661 6c69 6461 746f 725f 6973 5f63  d_validator_is_c
+00009960: 6f6c 756d 6e3a 204f 6e6c 7920 7468 6520  olumn: Only the 
+00009970: 436f 6c75 6d6e 2066 6965 6c64 2020 2020  Column field    
+00009980: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009990: 2020 2020 2020 2020 7c20 2a20 6669 656c          | * fiel
+000099a0: 645f 7661 6c69 6461 746f 725f 6973 5f6e  d_validator_is_n
+000099b0: 6f74 5f63 6f6c 756d 6e3a 204e 6f74 2074  ot_column: Not t
+000099c0: 6865 2043 6f6c 756d 6e20 6669 656c 6420  he Column field 
+000099d0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+000099e0: 2020 2020 2020 2020 7c20 2a20 6669 656c          | * fiel
+000099f0: 645f 7661 6c69 6461 746f 725f 6973 5f72  d_validator_is_r
+00009a00: 656c 6174 696f 6e73 6869 703a 204f 6e6c  elationship: Onl
+00009a10: 7920 7468 6520 2020 2020 2020 2020 2020  y the           
+00009a20: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009a30: 2020 2020 2020 2020 7c20 2020 7265 6c61          |   rela
+00009a40: 7469 6f6e 7373 6869 7020 284d 616e 7932  tionsship (Many2
+00009a50: 4f6e 652c 204f 6e65 324f 6e65 2c20 4f6e  One, One2One, On
+00009a60: 6532 4d61 6e79 2c20 2020 2020 2020 2020  e2Many,         
+00009a70: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009a80: 2020 2020 2020 2020 7c20 2020 4d61 6e79          |   Many
+00009a90: 324d 616e 7929 2020 2020 2020 2020 2020  2Many)          
+00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ac0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009ad0: 2020 2020 2020 2020 7c20 2a20 6669 656c          | * fiel
+00009ae0: 645f 7661 6c69 6461 746f 725f 6973 5f6e  d_validator_is_n
+00009af0: 6f74 5f72 656c 6174 696f 6e73 6869 703a  ot_relationship:
+00009b00: 204e 6f74 2074 6865 2020 2020 2020 2020   Not the        
+00009b10: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009b20: 2020 2020 2020 2020 7c20 2020 5265 6c61          |   Rela
+00009b30: 7469 6f6e 5368 6970 2020 2020 2020 2020  tionShip        
+00009b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b60: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009b70: 2020 2020 2020 2020 7c20 2a20 6669 656c          | * fiel
+00009b80: 645f 7661 6c69 6461 746f 725f 6973 5f6e  d_validator_is_n
+00009b90: 616d 6564 3a20 6669 6c74 6572 2062 7920  amed: filter by 
+00009ba0: 6e61 6d65 7320 6f66 2066 6965 6c64 2020  names of field  
+00009bb0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009bc0: 2020 2020 2020 2020 7c20 2a20 6669 656c          | * fiel
+00009bd0: 645f 7661 6c69 6461 746f 725f 6973 5f66  d_validator_is_f
+00009be0: 726f 6d5f 7479 7065 733a 2066 696c 7465  rom_types: filte
+00009bf0: 7220 6279 2046 6965 6c64 2020 2020 2020  r by Field      
+00009c00: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009c10: 2020 2020 2020 2020 7c20 2020 5479 7065          |   Type
+00009c20: 7320 2020 2020 2020 2020 2020 2020 2020  s               
+00009c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c50: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00009c60: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ca0: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.+-------------
+00009cb0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00009cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009cf0: 2b0a 0a52 656c 6174 696f 6e53 6869 700a  +..RelationShip.
+00009d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 546f  ------------..To
+00009d10: 2064 6563 6c61 7265 2061 2060 6052 656c   declare a ``Rel
+00009d20: 6174 696f 6e53 6869 7060 6020 696e 2061  ationShip`` in a
+00009d30: 206d 6f64 656c 2c20 6164 6420 6120 5265   model, add a Re
+00009d40: 6c61 7469 6f6e 5368 6970 206f 6e20 7468  lationShip on th
+00009d50: 6520 7461 626c 6520 6f66 0a74 6865 206d  e table of.the m
+00009d60: 6f64 656c 2e3a 3a0a 0a20 2020 2066 726f  odel.::..    fro
+00009d70: 6d20 616e 7962 6c6f 6b2e 6465 636c 6172  m anyblok.declar
+00009d80: 6174 696f 6e73 2069 6d70 6f72 7420 4465  ations import De
+00009d90: 636c 6172 6174 696f 6e73 0a20 2020 2066  clarations.    f
+00009da0: 726f 6d20 616e 7962 6c6f 6b2e 636f 6c75  rom anyblok.colu
+00009db0: 6d6e 2069 6d70 6f72 7420 496e 7465 6765  mn import Intege
+00009dc0: 720a 2020 2020 6672 6f6d 2061 6e79 626c  r.    from anybl
+00009dd0: 6f6b 2e72 656c 6174 696f 6e73 6869 7020  ok.relationship 
+00009de0: 696d 706f 7274 204d 616e 7932 4f6e 650a  import Many2One.
+00009df0: 0a0a 2020 2020 4044 6563 6c61 7261 7469  ..    @Declarati
+00009e00: 6f6e 732e 7265 6769 7374 6572 2844 6563  ons.register(Dec
+00009e10: 6c61 7261 7469 6f6e 2e4d 6f64 656c 290a  laration.Model).
+00009e20: 2020 2020 636c 6173 7320 4d79 4d6f 6465      class MyMode
+00009e30: 6c3a 0a0a 2020 2020 2020 2020 6964 203d  l:..        id =
+00009e40: 2049 6e74 6567 6572 2870 7269 6d61 7279   Integer(primary
+00009e50: 5f6b 6579 3d54 7275 6529 0a0a 0a20 2020  _key=True)...   
+00009e60: 2040 4465 636c 6172 6174 696f 6e73 2e72   @Declarations.r
+00009e70: 6567 6973 7465 7228 4465 636c 6172 6174  egister(Declarat
+00009e80: 696f 6e2e 4d6f 6465 6c29 0a20 2020 2063  ion.Model).    c
+00009e90: 6c61 7373 204d 794d 6f64 656c 323a 0a0a  lass MyModel2:..
+00009ea0: 2020 2020 2020 2020 6964 203d 2049 6e74          id = Int
+00009eb0: 6567 6572 2870 7269 6d61 7279 5f6b 6579  eger(primary_key
+00009ec0: 3d54 7275 6529 0a20 2020 2020 2020 206d  =True).        m
+00009ed0: 796d 6f64 656c 203d 204d 616e 7932 4f6e  ymodel = Many2On
+00009ee0: 6528 6d6f 6465 6c3d 4465 636c 6172 6174  e(model=Declarat
+00009ef0: 696f 6e2e 4d6f 6465 6c2e 4d79 4d6f 6465  ion.Model.MyMode
+00009f00: 6c29 0a0a 2e2e 206e 6f74 653a 3a0a 0a20  l).... note::.. 
+00009f10: 2020 2053 696e 6365 2074 6865 2076 6572     Since the ver
+00009f20: 7369 6f6e 2030 2e34 2e30 2074 6865 2060  sion 0.4.0 the `
+00009f30: 6052 656c 6174 696f 6e53 6869 7060 6020  `RelationShip`` 
+00009f40: 646f 6e27 7420 636f 6d65 2066 726f 6d20  don't come from 
+00009f50: 6060 4465 636c 6172 6174 696f 6e73 6060  ``Declarations``
+00009f60: 0a0a 4c69 7374 206f 6620 7468 6520 5265  ..List of the Re
+00009f70: 6c61 7469 6f6e 5368 6970 2074 7970 653a  lationShip type:
+00009f80: 0a0a 2a20 6060 4f6e 6532 4f6e 6560 600a  ..* ``One2One``.
+00009f90: 2a20 6060 4d61 6e79 324f 6e65 6060 0a2a  * ``Many2One``.*
+00009fa0: 2060 604f 6e65 324d 616e 7960 600a 2a20   ``One2Many``.* 
+00009fb0: 6060 4d61 6e79 324d 616e 7960 600a 0a50  ``Many2Many``..P
+00009fc0: 6172 616d 6574 6572 7320 6f66 2061 2060  arameters of a `
+00009fd0: 6052 656c 6174 696f 6e53 6869 7060 603a  `RelationShip``:
+00009fe0: 0a0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..+-------------
+00009ff0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+0000a000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a030: 2b0a 7c20 5061 7261 6d20 2020 2020 2020  +.| Param       
+0000a040: 2020 2020 2020 207c 2044 6573 6372 6970         | Descrip
+0000a050: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
 0000a060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a070: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
-0000a080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-0000a090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a0a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a0b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a0c0: 2d2d 2d2d 2d2d 2d2b 0a7c 2060 606d 616e  -------+.| ``man
-0000a0d0: 7932 6f6e 6560 6020 2020 2020 207c 204f  y2one``      | O
-0000a0e0: 7070 6f73 6974 6520 4d61 6e79 324f 6e65  pposite Many2One
-0000a0f0: 206c 696e 6b20 7769 7468 2074 6869 7320   link with this 
-0000a100: 4f6e 6532 4d61 6e79 2020 2020 2020 2020  One2Many        
-0000a110: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
-0000a120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-0000a130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a080: 7c0a 2b3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  |.+=============
+0000a090: 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d 3d3d 3d3d  =======+========
+0000a0a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000a0b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000a0c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000a0d0: 2b0a 7c20 6060 6c61 6265 6c60 6020 2020  +.| ``label``   
+0000a0e0: 2020 2020 2020 207c 2054 6865 206c 6162         | The lab
+0000a0f0: 656c 206f 6620 7468 6520 636f 6c75 6d6e  el of the column
+0000a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a120: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.+-------------
+0000a130: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
 0000a140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000a150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a160: 2d2d 2d2d 2d2d 2d2b 0a0a 2e2e 2077 6172  -------+.... war
-0000a170: 6e69 6e67 3a3a 0a0a 2020 2020 496e 2074  ning::..    In t
-0000a180: 6865 2063 6173 6520 7768 6572 6520 7477  he case where tw
-0000a190: 6f20 6f72 206d 6f72 6520 666f 7265 6967  o or more foreig
-0000a1a0: 6e20 6b65 7973 2069 7320 666f 756e 6420  n keys is found 
-0000a1b0: 746f 2074 6865 2073 616d 6520 7072 696d  to the same prim
-0000a1c0: 6172 7920 6b65 792c 0a20 2020 2074 6865  ary key,.    the
-0000a1d0: 6e20 7468 6520 7072 696d 6172 7920 6a6f  n the primary jo
-0000a1e0: 696e 2062 6563 6f6d 6520 6120 6060 6f72  in become a ``or
-0000a1f0: 6060 2062 6574 7765 656e 2074 6865 6d2e  `` between them.
-0000a200: 2059 6f75 206d 7573 7420 636f 6e73 6964   You must consid
-0000a210: 6572 6520 7468 6973 0a20 2020 2066 6965  ere this.    fie
-0000a220: 6c64 2061 7320 6120 7265 6164 6f6e 6c79  ld as a readonly
-0000a230: 2066 6965 6c64 2c20 6265 6361 7573 6520   field, because 
-0000a240: 5351 4c41 6c63 6865 6d79 2077 696c 6c20  SQLAlchemy will 
-0000a250: 6368 616e 6765 2074 6865 2062 6f74 6820  change the both 
-0000a260: 666f 7265 6967 6e20 6b65 790a 0a50 6172  foreign key..Par
-0000a270: 616d 6574 6572 7320 6f66 2074 6865 2060  ameters of the `
-0000a280: 604d 616e 7932 4d61 6e79 6060 2066 6965  `Many2Many`` fie
-0000a290: 6c64 3a0a 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d  ld:..+----------
-0000a2a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-0000a2b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a2c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a2d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a2e0: 2d2d 2d2b 0a7c 2050 6172 616d 6574 6572  ---+.| Parameter
-0000a2f0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000a300: 4465 7363 7269 7074 696f 6e20 2020 2020  Description     
-0000a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a330: 2020 207c 0a2b 3d3d 3d3d 3d3d 3d3d 3d3d     |.+==========
-0000a340: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2b3d  ==============+=
-0000a350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000a360: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000a370: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000a380: 3d3d 3d2b 0a7c 2060 606a 6f69 6e5f 7461  ===+.| ``join_ta
-0000a390: 626c 6560 6020 2020 2020 2020 2020 7c20  ble``         | 
-0000a3a0: 6d61 6e79 326d 616e 7920 696e 7465 726d  many2many interm
-0000a3b0: 6564 6961 7465 2074 6162 6c65 2062 6574  ediate table bet
-0000a3c0: 7765 656e 2062 6f74 6820 6d6f 6465 6c73  ween both models
-0000a3d0: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-0000a3e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-0000a3f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a420: 2d2d 2d2b 0a7c 2060 606a 6f69 6e5f 6d6f  ---+.| ``join_mo
-0000a430: 6465 6c60 6020 2020 2020 2020 2020 7c20  del``         | 
-0000a440: 6d61 6e79 326d 616e 7920 696e 7465 726d  many2many interm
-0000a450: 6564 6961 7465 2074 6162 6c65 2063 6f6d  ediate table com
-0000a460: 7075 7465 2066 726f 6d20 6120 4d6f 6465  pute from a Mode
-0000a470: 6c2c 207c 0a7c 2020 2020 2020 2020 2020  l, |.|          
-0000a480: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000a490: 5468 6973 2061 7474 7269 6275 7465 2069  This attribute i
-0000a4a0: 7320 7573 6564 2074 6f20 6275 696c 6420  s used to build 
-0000a4b0: 6120 7269 6368 204d 616e 7932 4d61 6e79  a rich Many2Many
-0000a4c0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000a4d0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a510: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000a520: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000a530: 2e2e 2077 6172 6e69 6e67 3a3a 2020 2020  .. warning::    
+0000a160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a170: 2b0a 7c20 6060 6d6f 6465 6c60 6020 2020  +.| ``model``   
+0000a180: 2020 2020 2020 207c 2054 6865 2072 656d         | The rem
+0000a190: 6f74 6520 6d6f 6465 6c20 2020 2020 2020  ote model       
+0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1c0: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.+-------------
+0000a1d0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+0000a1e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a1f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a210: 2b0a 7c20 6060 7265 6d6f 7465 5f63 6f6c  +.| ``remote_col
+0000a220: 756d 6e73 6060 207c 2054 6865 2063 6f6c  umns`` | The col
+0000a230: 756d 6e20 6e61 6d65 206f 6e20 7468 6520  umn name on the 
+0000a240: 7265 6d6f 7465 206d 6f64 656c 2c20 6966  remote model, if
+0000a250: 206e 6f20 7265 6d6f 7465 2020 2020 2020   no remote      
+0000a260: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+0000a270: 2020 2020 2020 207c 2063 6f6c 756d 6e73         | columns
+0000a280: 2061 7265 2064 6566 696e 6564 2074 6865   are defined the
+0000a290: 2072 656d 6f74 6520 636f 6c75 6d6e 2077   remote column w
+0000a2a0: 696c 6c20 6265 2074 6865 2020 2020 2020  ill be the      
+0000a2b0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+0000a2c0: 2020 2020 2020 207c 2070 7269 6d61 7279         | primary
+0000a2d0: 2063 6f6c 756d 6e20 6f66 2074 6865 2072   column of the r
+0000a2e0: 656d 6f74 6520 6d6f 6465 6c20 2020 2020  emote model     
+0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a300: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.+-------------
+0000a310: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+0000a320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a350: 2b0a 0a50 6172 616d 6574 6572 7320 6f66  +..Parameters of
+0000a360: 2074 6865 2060 604f 6e65 324f 6e65 6060   the ``One2One``
+0000a370: 2066 6965 6c64 3a0a 0a2b 2d2d 2d2d 2d2d   field:..+------
+0000a380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+0000a390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a3a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a3b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a3c0: 2d2d 2d2d 2d2d 2d2b 0a7c 2050 6172 616d  -------+.| Param
+0000a3d0: 2020 2020 2020 2020 2020 2020 207c 2044               | D
+0000a3e0: 6573 6372 6970 7469 6f6e 2020 2020 2020  escription      
+0000a3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a410: 2020 2020 2020 207c 0a2b 3d3d 3d3d 3d3d         |.+======
+0000a420: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d  =============+==
+0000a430: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000a440: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000a450: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000a460: 3d3d 3d3d 3d3d 3d2b 0a7c 2060 6063 6f6c  =======+.| ``col
+0000a470: 756d 6e5f 6e61 6d65 7360 6020 207c 204e  umn_names``  | N
+0000a480: 616d 6520 6f66 2074 6865 206c 6f63 616c  ame of the local
+0000a490: 2063 6f6c 756d 6e2e 2020 2020 2020 2020   column.        
+0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4b0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000a4c0: 2020 2020 2020 2020 2020 2020 207c 2049               | I
+0000a4d0: 6620 7468 6520 636f 6c75 6d6e 2064 6f65  f the column doe
+0000a4e0: 736e 2774 2065 7869 7374 2074 6865 6e20  sn't exist then 
+0000a4f0: 7468 6973 2063 6f6c 756d 6e20 7769 6c6c  this column will
+0000a500: 2062 6520 2020 207c 0a7c 2020 2020 2020   be    |.|      
+0000a510: 2020 2020 2020 2020 2020 2020 207c 2063               | c
+0000a520: 7265 6174 6564 2e20 2020 2020 2020 2020  reated.         
+0000a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a560: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000a570: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5b0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000a5c0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000a5d0: 2020 2020 416e 2065 7863 6570 7469 6f6e      An exception
-0000a5e0: 2069 7320 7261 6973 6564 2069 6620 7468   is raised if th
-0000a5f0: 6520 7461 626c 6520 636f 6d65 2066 726f  e table come fro
-0000a600: 6d20 207c 0a7c 2020 2020 2020 2020 2020  m  |.|          
-0000a610: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000a620: 2020 2020 6a6f 696e 5f74 6162 6c65 2061      join_table a
-0000a630: 6e64 206a 6f69 6e5f 6d6f 6465 6c20 6172  nd join_model ar
-0000a640: 6520 6469 6666 6572 656e 7420 2020 2020  e different     
-0000a650: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000a660: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a6a0: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-0000a6b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+0000a550: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000a560: 2020 2020 2020 2020 2020 2020 207c 2049               | I
+0000a570: 6620 6e6f 2063 6f6c 756d 6e20 6e61 6d65  f no column name
+0000a580: 2074 6865 6e20 7468 6520 6e61 6d65 2077   then the name w
+0000a590: 696c 6c20 6265 2027 4d32 4f20 6e61 6d65  ill be 'M2O name
+0000a5a0: 2720 2b20 2020 207c 0a7c 2020 2020 2020  ' +    |.|      
+0000a5b0: 2020 2020 2020 2020 2020 2020 207c 2027               | '
+0000a5c0: 5f27 202b 2027 6e61 6d65 206f 6620 7468  _' + 'name of th
+0000a5d0: 6520 7265 6d6f 7465 2063 6f6c 756d 6e27  e remote column'
+0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5f0: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+0000a600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+0000a610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a640: 2d2d 2d2d 2d2d 2d2b 0a7c 2060 606e 756c  -------+.| ``nul
+0000a650: 6c61 626c 6560 6020 2020 2020 207c 2049  lable``      | I
+0000a660: 6e64 6963 6174 6573 2069 6620 7468 6520  ndicates if the 
+0000a670: 636f 6c75 6d6e 206e 616d 6520 6973 206e  column name is n
+0000a680: 756c 6c61 626c 6520 6f72 206e 6f74 2020  ullable or not  
+0000a690: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+0000a6a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+0000a6b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000a6c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000a6d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a6e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a6f0: 2d2d 2d2b 0a7c 2060 606d 326d 5f72 656d  ---+.| ``m2m_rem
-0000a700: 6f74 655f 636f 6c75 6d6e 7360 6020 7c20  ote_columns`` | 
-0000a710: 436f 6c75 6d6e 206e 616d 6520 696e 2074  Column name in t
-0000a720: 6865 206a 6f69 6e20 7461 626c 6520 7768  he join table wh
-0000a730: 6963 6820 6861 7665 2067 6f74 2074 6865  ich have got the
-0000a740: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000a750: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000a760: 666f 7265 6967 6e20 6b65 7920 746f 2074  foreign key to t
-0000a770: 6865 2072 656d 6f74 6520 6d6f 6465 6c20  he remote model 
-0000a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a790: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-0000a7a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-0000a7b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a7c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a7d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a7e0: 2d2d 2d2b 0a7c 2060 606c 6f63 616c 5f63  ---+.| ``local_c
-0000a7f0: 6f6c 756d 6e73 6060 2020 2020 2020 7c20  olumns``      | 
-0000a800: 4e61 6d65 206f 6620 7468 6520 6c6f 6361  Name of the loca
-0000a810: 6c20 636f 6c75 6d6e 2077 6869 6368 2068  l column which h
-0000a820: 6f6c 6473 2074 6865 2066 6f72 6569 676e  olds the foreign
-0000a830: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000a840: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000a850: 6b65 7920 746f 2074 6865 206a 6f69 6e20  key to the join 
-0000a860: 7461 626c 652e 2020 2020 2020 2020 2020  table.          
-0000a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a880: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000a890: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000a8a0: 4966 2074 6865 2063 6f6c 756d 6e20 646f  If the column do
-0000a8b0: 6573 206e 6f74 2065 7869 7374 2074 6865  es not exist the
-0000a8c0: 6e20 7468 6973 2063 6f6c 756d 6e20 7769  n this column wi
-0000a8d0: 6c6c 207c 0a7c 2020 2020 2020 2020 2020  ll |.|          
-0000a8e0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000a8f0: 6265 2063 7265 6174 6564 2e20 2020 2020  be created.     
-0000a900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a920: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000a930: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000a940: 4966 206e 6f20 636f 6c75 6d6e 206e 616d  If no column nam
-0000a950: 6520 7468 656e 2074 6865 206e 616d 6520  e then the name 
-0000a960: 7769 6c6c 2062 6520 2774 6162 6c65 6e61  will be 'tablena
-0000a970: 6d65 277c 0a7c 2020 2020 2020 2020 2020  me'|.|          
-0000a980: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000a990: 2b20 275f 2720 2b20 6e61 6d65 206f 6620  + '_' + name of 
-0000a9a0: 7468 6520 7265 6c61 7469 6f6e 7368 6970  the relationship
-0000a9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9c0: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-0000a9d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-0000a9e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a9f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000aa00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000aa10: 2d2d 2d2b 0a7c 2060 606d 326d 5f6c 6f63  ---+.| ``m2m_loc
-0000aa20: 616c 5f63 6f6c 756d 6e73 6060 2020 7c20  al_columns``  | 
-0000aa30: 436f 6c75 6d6e 206e 616d 6520 696e 2074  Column name in t
-0000aa40: 6865 206a 6f69 6e20 7461 626c 6520 7768  he join table wh
-0000aa50: 6963 6820 686f 6c64 7320 7468 6520 2020  ich holds the   
-0000aa60: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000aa70: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000aa80: 666f 7265 6967 6e20 6b65 7920 746f 2074  foreign key to t
-0000aa90: 6865 206d 6f64 656c 2020 2020 2020 2020  he model        
-0000aaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aab0: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-0000aac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-0000aad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000aae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000aaf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ab00: 2d2d 2d2b 0a7c 2060 606d 616e 7932 6d61  ---+.| ``many2ma
-0000ab10: 6e79 6060 2020 2020 2020 2020 2020 7c20  ny``          | 
-0000ab20: 4f70 706f 7369 7465 204d 616e 7932 4d61  Opposite Many2Ma
-0000ab30: 6e79 206c 696e 6b20 7769 7468 2074 6869  ny link with thi
-0000ab40: 7320 7265 6c61 7469 6f6e 7368 6970 2020  s relationship  
-0000ab50: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-0000ab60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-0000ab70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ab80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ab90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000aba0: 2d2d 2d2b 0a7c 2060 6063 6f6d 7075 7465  ---+.| ``compute
-0000abb0: 5f6a 6f69 6e60 6020 2020 2020 2020 7c20  _join``       | 
-0000abc0: 466f 7263 6520 746f 2063 6f6d 7075 7465  Force to compute
-0000abd0: 2073 6563 6f6e 6461 7279 6a6f 696e 2061   secondaryjoin a
-0000abe0: 6e64 2070 7269 6d61 7279 6a6f 696e 2020  nd primaryjoin  
-0000abf0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000ac00: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000ac10: 496e 2074 6865 206d 6f73 7420 6361 7365  In the most case
-0000ac20: 2074 6869 7320 6973 2066 6f72 6269 6464   this is forbidd
-0000ac30: 656e 2062 6563 6175 7365 2069 7420 6973  en because it is
-0000ac40: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000ac50: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000ac60: 6461 6e67 656f 7572 6f75 732c 2054 6865  dangeourous, The
-0000ac70: 206f 6e6c 7920 6361 7365 2077 6865 7265   only case where
-0000ac80: 2074 6865 2063 6f6d 7075 7465 2069 7320   the compute is 
-0000ac90: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000aca0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000acb0: 7265 7175 6972 6564 2c20 6973 2077 6865  required, is whe
-0000acc0: 6e20 7468 6520 6d6f 6465 6c5f 6a6f 696e  n the model_join
-0000acd0: 2068 6176 6520 6d6f 7265 2074 6861 6e20   have more than 
-0000ace0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000acf0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000ad00: 6f6e 6520 7072 696d 6172 7920 6b65 7920  one primary key 
-0000ad10: 746f 2074 6865 206d 6169 6e20 6d6f 6465  to the main mode
-0000ad20: 6c20 666f 7220 7269 6368 2020 2020 2020  l for rich      
-0000ad30: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000ad40: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000ad50: 4d61 6e79 324d 616e 7920 2020 2020 2020  Many2Many       
-0000ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad80: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000ad90: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000adb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000add0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000ade0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000adf0: 2e2e 206e 6f74 653a 3a20 2020 2020 2020  .. note::       
-0000ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae20: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000ae30: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae70: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000ae80: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000ae90: 2020 2020 496e 2074 6865 2063 6173 6520      In the case 
-0000aea0: 7768 6572 6520 7468 6520 626f 7468 206d  where the both m
-0000aeb0: 6f64 656c 2061 7265 2074 6865 2073 616d  odel are the sam
-0000aec0: 6520 207c 0a7c 2020 2020 2020 2020 2020  e  |.|          
-0000aed0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000aee0: 2020 2020 7468 6973 206f 7074 696f 6e20      this option 
-0000aef0: 6973 2066 6f72 6365 6420 2020 2020 2020  is forced       
-0000af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af10: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0000af20: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0000af30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af60: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-0000af70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-0000af80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000af90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000afa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000afb0: 2d2d 2d2b 0a0a 2e2e 206e 6f74 653a 3a0a  ---+.... note::.
-0000afc0: 0a20 2020 2053 696e 6365 2030 2e34 2e30  .    Since 0.4.0
-0000afd0: 2c20 7768 656e 2074 6865 2072 656c 6174  , when the relat
-0000afe0: 696f 6e6e 616c 2074 6162 6c65 2069 7320  ionnal table is 
-0000aff0: 6372 6561 7465 6420 6279 2041 6e79 426c  created by AnyBl
-0000b000: 6f6b 2c20 7468 650a 2020 2020 6d32 6d5f  ok, the.    m2m_
-0000b010: 636f 6c75 6d6e 7320 6265 636f 6d6d 6520  columns becomme 
-0000b020: 666f 7265 6967 6e20 6b65 7973 0a0a 0a46  foreign keys...F
-0000b030: 6965 6c64 0a2d 2d2d 2d2d 0a0a 546f 2064  ield.-----..To d
-0000b040: 6563 6c61 7265 2061 2060 6046 6965 6c64  eclare a ``Field
-0000b050: 6060 2069 6e20 6120 6d6f 6465 6c2c 2061  `` in a model, a
-0000b060: 6464 2061 2046 6965 6c64 206f 6e20 7468  dd a Field on th
-0000b070: 6520 4d6f 6465 6c2c 2074 6869 7320 6973  e Model, this is
-0000b080: 206e 6f74 2061 0a53 514c 2063 6f6c 756d   not a.SQL colum
-0000b090: 6e2e 3a3a 0a0a 2020 2020 6672 6f6d 2061  n.::..    from a
-0000b0a0: 6e79 626c 6f6b 2e64 6563 6c61 7261 7469  nyblok.declarati
-0000b0b0: 6f6e 7320 696d 706f 7274 2044 6563 6c61  ons import Decla
-0000b0c0: 7261 7469 6f6e 730a 2020 2020 6672 6f6d  rations.    from
-0000b0d0: 2061 6e79 626c 6f6b 2e66 6965 6c64 2069   anyblok.field i
-0000b0e0: 6d70 6f72 7420 4675 6e63 7469 6f6e 0a20  mport Function. 
-0000b0f0: 2020 2066 726f 6d20 616e 7962 6c6f 6b2e     from anyblok.
-0000b100: 636f 6c75 6d6e 2069 6d70 6f72 7420 496e  column import In
-0000b110: 7465 6765 720a 0a0a 2020 2020 4044 6563  teger...    @Dec
-0000b120: 6c61 7261 7469 6f6e 732e 7265 6769 7374  larations.regist
-0000b130: 6572 2844 6563 6c61 7261 7469 6f6e 2e4d  er(Declaration.M
-0000b140: 6f64 656c 290a 2020 2020 636c 6173 7320  odel).    class 
-0000b150: 4d79 4d6f 6465 6c3a 0a0a 2020 2020 2020  MyModel:..      
-0000b160: 2020 6964 203d 2049 6e74 6567 6572 2870    id = Integer(p
-0000b170: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
-0000b180: 0a20 2020 2020 2020 2066 6972 7374 5f6e  .        first_n
-0000b190: 616d 6520 3d20 5374 7269 6e67 2829 0a20  ame = String(). 
-0000b1a0: 2020 2020 2020 206c 6173 745f 6e61 6d65         last_name
-0000b1b0: 203d 2053 7472 696e 6728 290a 2020 2020   = String().    
-0000b1c0: 2020 2020 6e61 6d65 203d 2046 756e 6374      name = Funct
-0000b1d0: 696f 6e28 6667 6574 3d27 6667 6574 272c  ion(fget='fget',
-0000b1e0: 2066 7365 743d 2766 7365 7427 2c20 6664   fset='fset', fd
-0000b1f0: 656c 3d27 6664 656c 272c 2066 6578 7072  el='fdel', fexpr
-0000b200: 3d27 6665 7870 7227 290a 0a20 2020 2020  ='fexpr')..     
-0000b210: 2020 2064 6566 2066 6765 7428 7365 6c66     def fget(self
-0000b220: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-0000b230: 6574 7572 6e20 277b 307d 207b 317d 272e  eturn '{0} {1}'.
-0000b240: 666f 726d 6174 2873 656c 662e 6669 7273  format(self.firs
-0000b250: 745f 6e61 6d65 2c20 7365 6c66 2e6c 6173  t_name, self.las
-0000b260: 745f 6e61 6d65 290a 0a20 2020 2020 2020  t_name)..       
-0000b270: 2064 6566 2066 7365 7428 7365 6c66 2c20   def fset(self, 
-0000b280: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
-0000b290: 2020 2020 7365 6c66 2e66 6972 7374 5f6e      self.first_n
-0000b2a0: 616d 652c 2073 656c 662e 6c61 7374 5f6e  ame, self.last_n
-0000b2b0: 616d 6520 3d20 7661 6c75 652e 7370 6c69  ame = value.spli
-0000b2c0: 7428 2720 272c 2031 290a 0a20 2020 2020  t(' ', 1)..     
-0000b2d0: 2020 2064 6566 2066 6465 6c28 7365 6c66     def fdel(self
-0000b2e0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000b2f0: 656c 662e 6669 7273 745f 6e61 6d65 203d  elf.first_name =
-0000b300: 2073 656c 662e 6c61 7374 5f6e 616d 6520   self.last_name 
-0000b310: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
-0000b320: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-0000b330: 2020 2020 2064 6566 2066 6578 7072 2863       def fexpr(c
-0000b340: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
-0000b350: 2072 6574 7572 6e20 6675 6e63 2e63 6f6e   return func.con
-0000b360: 6361 7428 636c 732e 6669 7273 745f 6e61  cat(cls.first_na
-0000b370: 6d65 2c20 2720 272c 2063 6c73 2e6c 6173  me, ' ', cls.las
-0000b380: 745f 6e61 6d65 290a 0a4c 6973 7420 6f66  t_name)..List of
-0000b390: 2074 6865 2060 6046 6965 6c64 6060 2074   the ``Field`` t
-0000b3a0: 7970 653a 0a0a 2a20 6060 4675 6e63 7469  ype:..* ``Functi
-0000b3b0: 6f6e 6060 0a2a 2060 604a 736f 6e52 656c  on``.* ``JsonRel
-0000b3c0: 6174 6564 6060 0a0a 5061 7261 6d65 7465  ated``..Paramete
-0000b3d0: 7273 2066 6f72 2060 6046 6965 6c64 2e46  rs for ``Field.F
-0000b3e0: 756e 6374 696f 6e60 600a 0a2b 2d2d 2d2d  unction``..+----
-0000b3f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-0000b400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b430: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2050 6172  ---------+.| Par
-0000b440: 616d 6574 6572 2020 2020 2020 2020 207c  ameter         |
-0000b450: 2044 6573 6372 6970 7469 6f6e 2020 2020   Description    
-0000b460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b480: 2020 2020 2020 2020 207c 0a2b 3d3d 3d3d           |.+====
-0000b490: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b  ===============+
-0000b4a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000b4b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000b4c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000b4d0: 3d3d 3d3d 3d3d 3d3d 3d2b 0a7c 2060 6066  =========+.| ``f
-0000b4e0: 6765 7460 6020 2020 2020 2020 2020 207c  get``          |
-0000b4f0: 206e 616d 6520 6f66 2074 6865 206d 6574   name of the met
-0000b500: 686f 6420 746f 2063 616c 6c20 746f 2067  hod to call to g
-0000b510: 6574 2074 6865 2076 616c 7565 206f 6620  et the value of 
-0000b520: 6669 656c 643a 3a20 207c 0a7c 2020 2020  field::  |.|    
-0000b530: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0000a6e0: 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6062 6163  -------+.| ``bac
+0000a6f0: 6b72 6566 6060 2020 2020 2020 207c 2052  kref``       | R
+0000a700: 656d 6f74 6520 4f6e 6532 4f6e 6520 6c69  emote One2One li
+0000a710: 6e6b 2077 6974 6820 7468 6520 636f 6c75  nk with the colu
+0000a720: 6d6e 206e 616d 6520 2020 2020 2020 2020  mn name         
+0000a730: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+0000a740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+0000a750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a780: 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6075 6e69  -------+.| ``uni
+0000a790: 7175 6560 6020 2020 2020 2020 207c 2041  que``        | A
+0000a7a0: 6464 2075 6e69 7175 6520 636f 6e73 7472  dd unique constr
+0000a7b0: 6169 6e74 206f 6e20 7468 6520 6372 6561  aint on the crea
+0000a7c0: 7465 6420 636f 6c75 6d6e 2873 2920 2020  ted column(s)   
+0000a7d0: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+0000a7e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+0000a7f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a820: 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6069 6e64  -------+.| ``ind
+0000a830: 6578 6060 2020 2020 2020 2020 207c 2041  ex``         | A
+0000a840: 6464 2069 6e64 6578 2063 6f6e 7374 7261  dd index constra
+0000a850: 696e 7420 6f6e 2074 6865 2063 7265 6174  int on the creat
+0000a860: 6564 2063 6f6c 756d 6e28 7329 2020 2020  ed column(s)    
+0000a870: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+0000a880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+0000a890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a8a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a8b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a8c0: 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6070 7269  -------+.| ``pri
+0000a8d0: 6d61 7279 5f6b 6579 6060 2020 207c 2054  mary_key``   | T
+0000a8e0: 6865 2063 7265 6174 6564 2063 6f6c 756d  he created colum
+0000a8f0: 6e28 7329 2061 7265 2070 7269 6d61 7279  n(s) are primary
+0000a900: 206b 6579 2020 2020 2020 2020 2020 2020   key            
+0000a910: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+0000a920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+0000a930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a960: 2d2d 2d2d 2d2d 2d2b 0a0a 5061 7261 6d65  -------+..Parame
+0000a970: 7465 7273 206f 6620 7468 6520 6060 4d61  ters of the ``Ma
+0000a980: 6e79 324f 6e65 6060 2066 6965 6c64 3a0a  ny2One`` field:.
+0000a990: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+0000a9a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+0000a9b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a9c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000a9d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+0000a9e0: 0a7c 2050 6172 616d 6574 6572 2020 2020  .| Parameter    
+0000a9f0: 2020 2020 2020 2020 2020 207c 2044 6573             | Des
+0000aa00: 6372 6970 7469 6f6e 2020 2020 2020 2020  cription        
+0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa20: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0000aa30: 0a2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .+==============
+0000aa40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d  ===========+====
+0000aa50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000aa60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000aa70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b  ===============+
+0000aa80: 0a7c 2060 6063 6f6c 756d 6e5f 6e61 6d65  .| ``column_name
+0000aa90: 7360 6020 2020 2020 2020 207c 204e 616d  s``        | Nam
+0000aaa0: 6520 6f66 2074 6865 206c 6f63 616c 2063  e of the local c
+0000aab0: 6f6c 756d 6e2e 2020 2020 2020 2020 2020  olumn.          
+0000aac0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0000aad0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+0000aae0: 2020 2020 2020 2020 2020 207c 2049 6620             | If 
+0000aaf0: 7468 6520 636f 6c75 6d6e 2064 6f65 736e  the column doesn
+0000ab00: 2774 2065 7869 7374 2074 6865 6e20 7468  't exist then th
+0000ab10: 6973 2063 6f6c 756d 6e20 7769 6c6c 207c  is column will |
+0000ab20: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+0000ab30: 2020 2020 2020 2020 2020 207c 2062 6520             | be 
+0000ab40: 6372 6561 7465 642e 2020 2020 2020 2020  created.        
+0000ab50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab60: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0000ab70: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+0000ab80: 2020 2020 2020 2020 2020 207c 2049 6620             | If 
+0000ab90: 6e6f 2063 6f6c 756d 6e20 6e61 6d65 2074  no column name t
+0000aba0: 6865 6e20 7468 6520 6e61 6d65 2077 696c  hen the name wil
+0000abb0: 6c20 6265 2020 2020 2020 2020 2020 207c  l be           |
+0000abc0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+0000abd0: 2020 2020 2020 2020 2020 207c 2027 4d32             | 'M2
+0000abe0: 4f20 6e61 6d65 2720 2b20 275f 2720 2b20  O name' + '_' + 
+0000abf0: 276e 616d 6520 6f66 2074 6865 2072 656d  'name of the rem
+0000ac00: 6f74 6520 636f 6c75 6d6e 2720 2020 207c  ote column'    |
+0000ac10: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+0000ac20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+0000ac30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ac40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ac50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+0000ac60: 0a7c 2060 606e 756c 6c61 626c 6560 6020  .| ``nullable`` 
+0000ac70: 2020 2020 2020 2020 2020 207c 2049 6e64             | Ind
+0000ac80: 6963 6174 6520 6966 2074 6865 2063 6f6c  icate if the col
+0000ac90: 756d 6e20 6e61 6d65 2069 7320 6e75 6c6c  umn name is null
+0000aca0: 6162 6c65 206f 7220 6e6f 7420 2020 207c  able or not    |
+0000acb0: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+0000acc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+0000acd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ace0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000acf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+0000ad00: 0a7c 2060 6075 6e69 7175 6560 6020 2020  .| ``unique``   
+0000ad10: 2020 2020 2020 2020 2020 207c 2041 6464             | Add
+0000ad20: 2075 6e69 7175 6520 636f 6e73 7472 6169   unique constrai
+0000ad30: 6e74 206f 6e20 7468 6520 6372 6561 7465  nt on the create
+0000ad40: 6420 636f 6c75 6d6e 2873 2920 2020 207c  d column(s)    |
+0000ad50: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+0000ad60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+0000ad70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ad80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ad90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+0000ada0: 0a7c 2060 6069 6e64 6578 6060 2020 2020  .| ``index``    
+0000adb0: 2020 2020 2020 2020 2020 207c 2041 6464             | Add
+0000adc0: 2069 6e64 6578 2063 6f6e 7374 7261 696e   index constrain
+0000add0: 7420 6f6e 2074 6865 2063 7265 6174 6564  t on the created
+0000ade0: 2063 6f6c 756d 6e28 7329 2020 2020 207c   column(s)     |
+0000adf0: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+0000ae00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+0000ae10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ae20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ae30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+0000ae40: 0a7c 2060 6070 7269 6d61 7279 5f6b 6579  .| ``primary_key
+0000ae50: 6060 2020 2020 2020 2020 207c 2054 6865  ``         | The
+0000ae60: 2063 7265 6174 6564 2063 6f6c 756d 6e28   created column(
+0000ae70: 7329 2061 7265 2070 7269 6d61 7279 206b  s) are primary k
+0000ae80: 6579 2020 2020 2020 2020 2020 2020 207c  ey             |
+0000ae90: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+0000aea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+0000aeb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000aec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000aed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+0000aee0: 0a7c 2060 606f 6e65 326d 616e 7960 6020  .| ``one2many`` 
+0000aef0: 2020 2020 2020 2020 2020 207c 204f 7070             | Opp
+0000af00: 6f73 6974 6520 4f6e 6532 4d61 6e79 206c  osite One2Many l
+0000af10: 696e 6b20 7769 7468 2074 6869 7320 4d61  ink with this Ma
+0000af20: 6e79 326f 6e65 2020 2020 2020 2020 207c  ny2one         |
+0000af30: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+0000af40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+0000af50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000af60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000af70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+0000af80: 0a7c 2060 6066 6f72 6569 676e 5f6b 6579  .| ``foreign_key
+0000af90: 5f6f 7074 696f 6e73 6060 207c 2074 616b  _options`` | tak
+0000afa0: 6520 6120 6469 6374 2077 6974 6820 7468  e a dict with th
+0000afb0: 6520 6f70 7469 6f6e 2066 6f72 2063 7265  e option for cre
+0000afc0: 6174 6520 7468 6520 2020 2020 2020 207c  ate the        |
+0000afd0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+0000afe0: 2020 2020 2020 2020 2020 207c 2066 6f72             | for
+0000aff0: 6569 676e 206b 6579 2020 2020 2020 2020  eign key        
+0000b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b010: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0000b020: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+0000b030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+0000b040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+0000b070: 0a0a 3a3a 0a0a 2020 2020 4d61 6e79 324f  ..::..    Many2O
+0000b080: 6e65 286d 6f64 656c 3d54 6865 2e4d 6f64  ne(model=The.Mod
+0000b090: 656c 2c20 6e75 6c6c 6162 6c65 3d54 7275  el, nullable=Tru
+0000b0a0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000b0b0: 666f 7265 6967 6e5f 6b65 795f 6f70 7469  foreign_key_opti
+0000b0c0: 6f6e 733d 7b27 6f6e 6465 6c65 7465 273a  ons={'ondelete':
+0000b0d0: 2027 6361 7363 6164 6527 7d29 0a0a 0a0a   'cascade'})....
+0000b0e0: 5061 7261 6d65 7465 7273 206f 6620 7468  Parameters of th
+0000b0f0: 6520 6060 4f6e 6532 4d61 6e79 6060 2066  e ``One2Many`` f
+0000b100: 6965 6c64 3a0a 0a2b 2d2d 2d2d 2d2d 2d2d  ield:..+--------
+0000b110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+0000b120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b150: 2d2d 2d2d 2d2b 0a7c 2050 6172 616d 6574  -----+.| Paramet
+0000b160: 6572 2020 2020 2020 2020 207c 2044 6573  er         | Des
+0000b170: 6372 6970 7469 6f6e 2020 2020 2020 2020  cription        
+0000b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1a0: 2020 2020 207c 0a2b 3d3d 3d3d 3d3d 3d3d       |.+========
+0000b1b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d 3d3d  ===========+====
+0000b1c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000b1d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000b1e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000b1f0: 3d3d 3d3d 3d2b 0a7c 2060 6070 7269 6d61  =====+.| ``prima
+0000b200: 7279 6a6f 696e 6060 2020 207c 204a 6f69  ryjoin``   | Joi
+0000b210: 6e20 636f 6e64 6974 696f 6e20 6265 7477  n condition betw
+0000b220: 6565 6e20 7468 6520 7265 6c61 7469 6f6e  een the relation
+0000b230: 7368 6970 2061 6e64 2074 6865 2072 656d  ship and the rem
+0000b240: 6f74 6520 207c 0a7c 2020 2020 2020 2020  ote  |.|        
+0000b250: 2020 2020 2020 2020 2020 207c 2063 6f6c             | col
+0000b260: 756d 6e20 2020 2020 2020 2020 2020 2020  umn             
+0000b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b290: 2020 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d       |.+--------
+0000b2a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+0000b2b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b2c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b2d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b2e0: 2d2d 2d2d 2d2b 0a7c 2060 606d 616e 7932  -----+.| ``many2
+0000b2f0: 6f6e 6560 6020 2020 2020 207c 204f 7070  one``      | Opp
+0000b300: 6f73 6974 6520 4d61 6e79 324f 6e65 206c  osite Many2One l
+0000b310: 696e 6b20 7769 7468 2074 6869 7320 4f6e  ink with this On
+0000b320: 6532 4d61 6e79 2020 2020 2020 2020 2020  e2Many          
+0000b330: 2020 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d       |.+--------
+0000b340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+0000b350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b380: 2d2d 2d2d 2d2b 0a0a 2e2e 2077 6172 6e69  -----+.... warni
+0000b390: 6e67 3a3a 0a0a 2020 2020 496e 2074 6865  ng::..    In the
+0000b3a0: 2063 6173 6520 7768 6572 6520 7477 6f20   case where two 
+0000b3b0: 6f72 206d 6f72 6520 666f 7265 6967 6e20  or more foreign 
+0000b3c0: 6b65 7973 2069 7320 666f 756e 6420 746f  keys is found to
+0000b3d0: 2074 6865 2073 616d 6520 7072 696d 6172   the same primar
+0000b3e0: 7920 6b65 792c 0a20 2020 2074 6865 6e20  y key,.    then 
+0000b3f0: 7468 6520 7072 696d 6172 7920 6a6f 696e  the primary join
+0000b400: 2062 6563 6f6d 6520 6120 6060 6f72 6060   become a ``or``
+0000b410: 2062 6574 7765 656e 2074 6865 6d2e 2059   between them. Y
+0000b420: 6f75 206d 7573 7420 636f 6e73 6964 6572  ou must consider
+0000b430: 6520 7468 6973 0a20 2020 2066 6965 6c64  e this.    field
+0000b440: 2061 7320 6120 7265 6164 6f6e 6c79 2066   as a readonly f
+0000b450: 6965 6c64 2c20 6265 6361 7573 6520 5351  ield, because SQ
+0000b460: 4c41 6c63 6865 6d79 2077 696c 6c20 6368  LAlchemy will ch
+0000b470: 616e 6765 2074 6865 2062 6f74 6820 666f  ange the both fo
+0000b480: 7265 6967 6e20 6b65 790a 0a50 6172 616d  reign key..Param
+0000b490: 6574 6572 7320 6f66 2074 6865 2060 604d  eters of the ``M
+0000b4a0: 616e 7932 4d61 6e79 6060 2066 6965 6c64  any2Many`` field
+0000b4b0: 3a0a 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :..+------------
+0000b4c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+0000b4d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b4e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b4f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b500: 2d2b 0a7c 2050 6172 616d 6574 6572 2020  -+.| Parameter  
+0000b510: 2020 2020 2020 2020 2020 2020 7c20 4465              | De
+0000b520: 7363 7269 7074 696f 6e20 2020 2020 2020  scription       
+0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b570: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0000b580: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0000b590: 2020 2064 6566 2066 6765 7428 7365 6c66     def fget(self
-0000b5a0: 293a 2020 2020 2020 2020 2020 2020 2020  ):              
-0000b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5c0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0000b5d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0000b5e0: 2020 2020 2020 2072 6574 7572 6e20 277b         return '{
-0000b5f0: 307d 207b 317d 272e 666f 726d 6174 2873  0} {1}'.format(s
-0000b600: 656c 662e 6669 7273 745f 6e61 6d65 2c20  elf.first_name, 
-0000b610: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0000b620: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000b650: 656c 662e 6c61 7374 5f6e 616d 6529 2020  elf.last_name)  
-0000b660: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0000b670: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6b0: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
-0000b6c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-0000b6d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b6e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b6f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b700: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6066  ---------+.| ``f
-0000b710: 7365 7460 6020 2020 2020 2020 2020 207c  set``          |
-0000b720: 206e 616d 6520 6f66 2074 6865 206d 6574   name of the met
-0000b730: 686f 6420 746f 2063 616c 6c20 746f 2073  hod to call to s
-0000b740: 6574 2074 6865 2076 616c 7565 206f 6620  et the value of 
-0000b750: 6669 656c 643a 3a20 207c 0a7c 2020 2020  field::  |.|    
-0000b760: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0000b550: 207c 0a2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   |.+============
+0000b560: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2b3d 3d3d  ============+===
+0000b570: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000b580: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000b590: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000b5a0: 3d2b 0a7c 2060 606a 6f69 6e5f 7461 626c  =+.| ``join_tabl
+0000b5b0: 6560 6020 2020 2020 2020 2020 7c20 6d61  e``         | ma
+0000b5c0: 6e79 326d 616e 7920 696e 7465 726d 6564  ny2many intermed
+0000b5d0: 6961 7465 2074 6162 6c65 2062 6574 7765  iate table betwe
+0000b5e0: 656e 2062 6f74 6820 6d6f 6465 6c73 2020  en both models  
+0000b5f0: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
+0000b600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+0000b610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b640: 2d2b 0a7c 2060 606a 6f69 6e5f 6d6f 6465  -+.| ``join_mode
+0000b650: 6c60 6020 2020 2020 2020 2020 7c20 6d61  l``         | ma
+0000b660: 6e79 326d 616e 7920 696e 7465 726d 6564  ny2many intermed
+0000b670: 6961 7465 2074 6162 6c65 2063 6f6d 7075  iate table compu
+0000b680: 7465 2066 726f 6d20 6120 4d6f 6465 6c2c  te from a Model,
+0000b690: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000b6a0: 2020 2020 2020 2020 2020 2020 7c20 5468              | Th
+0000b6b0: 6973 2061 7474 7269 6275 7465 2069 7320  is attribute is 
+0000b6c0: 7573 6564 2074 6f20 6275 696c 6420 6120  used to build a 
+0000b6d0: 7269 6368 204d 616e 7932 4d61 6e79 2020  rich Many2Many  
+0000b6e0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000b6f0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0000b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b730: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000b740: 2020 2020 2020 2020 2020 2020 7c20 2e2e              | ..
+0000b750: 2077 6172 6e69 6e67 3a3a 2020 2020 2020   warning::      
+0000b760: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7a0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0000b7b0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0000b7c0: 2020 2064 6566 2066 7365 7428 7365 6c66     def fset(self
-0000b7d0: 293a 2020 2020 2020 2020 2020 2020 2020  ):              
-0000b7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7f0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0000b800: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0000b810: 2020 2020 2020 2073 656c 662e 6669 7273         self.firs
-0000b820: 745f 6e61 6d65 2c20 7365 6c66 2e6c 6173  t_name, self.las
-0000b830: 745f 6e61 6d65 203d 2076 616c 7565 2e73  t_name = value.s
-0000b840: 706c 6974 2827 2027 2c7c 0a7c 2020 2020  plit(' ',|.|    
-0000b850: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0000b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b890: 2020 2020 2031 2920 207c 0a7c 2020 2020       1)  |.|    
-0000b8a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0000b780: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000b790: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0000b7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7d0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000b7e0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0000b7f0: 2020 416e 2065 7863 6570 7469 6f6e 2069    An exception i
+0000b800: 7320 7261 6973 6564 2069 6620 7468 6520  s raised if the 
+0000b810: 7461 626c 6520 636f 6d65 2066 726f 6d20  table come from 
+0000b820: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000b830: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0000b840: 2020 6a6f 696e 5f74 6162 6c65 2061 6e64    join_table and
+0000b850: 206a 6f69 6e5f 6d6f 6465 6c20 6172 6520   join_model are 
+0000b860: 6469 6666 6572 656e 7420 2020 2020 2020  different       
+0000b870: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000b880: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0000b890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8e0: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
-0000b8f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+0000b8c0: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
+0000b8d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+0000b8e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b8f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000b900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b930: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6066  ---------+.| ``f
-0000b940: 6465 6c60 6020 2020 2020 2020 2020 207c  del``          |
-0000b950: 206e 616d 6520 6f66 2074 6865 206d 6574   name of the met
-0000b960: 686f 6420 746f 2063 616c 6c20 746f 2064  hod to call to d
-0000b970: 656c 2074 6865 2076 616c 7565 206f 6620  el the value of 
-0000b980: 6669 656c 643a 3a20 207c 0a7c 2020 2020  field::  |.|    
-0000b990: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0000b910: 2d2b 0a7c 2060 606d 326d 5f72 656d 6f74  -+.| ``m2m_remot
+0000b920: 655f 636f 6c75 6d6e 7360 6020 7c20 436f  e_columns`` | Co
+0000b930: 6c75 6d6e 206e 616d 6520 696e 2074 6865  lumn name in the
+0000b940: 206a 6f69 6e20 7461 626c 6520 7768 6963   join table whic
+0000b950: 6820 6861 7665 2067 6f74 2074 6865 2020  h have got the  
+0000b960: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000b970: 2020 2020 2020 2020 2020 2020 7c20 666f              | fo
+0000b980: 7265 6967 6e20 6b65 7920 746f 2074 6865  reign key to the
+0000b990: 2072 656d 6f74 6520 6d6f 6465 6c20 2020   remote model   
 0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9d0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0000b9e0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0000b9f0: 2020 2064 6566 2066 6465 6c28 7365 6c66     def fdel(self
-0000ba00: 293a 2020 2020 2020 2020 2020 2020 2020  ):              
-0000ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba20: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0000ba30: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0000ba40: 2020 2020 2020 2073 656c 662e 6669 7273         self.firs
-0000ba50: 745f 6e61 6d65 203d 2073 656c 662e 6c61  t_name = self.la
-0000ba60: 7374 5f6e 616d 6520 3d20 4e6f 6e65 2020  st_name = None  
-0000ba70: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0000ba80: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0000b9b0: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
+0000b9c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+0000b9d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b9e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b9f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ba00: 2d2b 0a7c 2060 606c 6f63 616c 5f63 6f6c  -+.| ``local_col
+0000ba10: 756d 6e73 6060 2020 2020 2020 7c20 4e61  umns``      | Na
+0000ba20: 6d65 206f 6620 7468 6520 6c6f 6361 6c20  me of the local 
+0000ba30: 636f 6c75 6d6e 2077 6869 6368 2068 6f6c  column which hol
+0000ba40: 6473 2074 6865 2066 6f72 6569 676e 2020  ds the foreign  
+0000ba50: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000ba60: 2020 2020 2020 2020 2020 2020 7c20 6b65              | ke
+0000ba70: 7920 746f 2074 6865 206a 6f69 6e20 7461  y to the join ta
+0000ba80: 626c 652e 2020 2020 2020 2020 2020 2020  ble.            
 0000ba90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bac0: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
-0000bad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-0000bae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000baf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bb00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bb10: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6066  ---------+.| ``f
-0000bb20: 6578 7060 6020 2020 2020 2020 2020 207c  exp``          |
-0000bb30: 206e 616d 6520 6f66 2074 6865 2063 6c61   name of the cla
-0000bb40: 7373 206d 6574 686f 6420 746f 2063 616c  ss method to cal
-0000bb50: 6c20 746f 2066 696c 7465 7220 6f6e 2074  l to filter on t
-0000bb60: 6865 2020 2020 2020 207c 0a7c 2020 2020  he       |.|    
-0000bb70: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0000bb80: 2066 6965 6c64 3a3a 2020 2020 2020 2020   field::        
-0000bb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbb0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0000bbc0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0000baa0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000bab0: 2020 2020 2020 2020 2020 2020 7c20 4966              | If
+0000bac0: 2074 6865 2063 6f6c 756d 6e20 646f 6573   the column does
+0000bad0: 206e 6f74 2065 7869 7374 2074 6865 6e20   not exist then 
+0000bae0: 7468 6973 2063 6f6c 756d 6e20 7769 6c6c  this column will
+0000baf0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000bb00: 2020 2020 2020 2020 2020 2020 7c20 6265              | be
+0000bb10: 2063 7265 6174 6564 2e20 2020 2020 2020   created.       
+0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb40: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000bb50: 2020 2020 2020 2020 2020 2020 7c20 4966              | If
+0000bb60: 206e 6f20 636f 6c75 6d6e 206e 616d 6520   no column name 
+0000bb70: 7468 656e 2074 6865 206e 616d 6520 7769  then the name wi
+0000bb80: 6c6c 2062 6520 2774 6162 6c65 6e61 6d65  ll be 'tablename
+0000bb90: 277c 0a7c 2020 2020 2020 2020 2020 2020  '|.|            
+0000bba0: 2020 2020 2020 2020 2020 2020 7c20 2b20              | + 
+0000bbb0: 275f 2720 2b20 6e61 6d65 206f 6620 7468  '_' + name of th
+0000bbc0: 6520 7265 6c61 7469 6f6e 7368 6970 2020  e relationship  
 0000bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc00: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0000bc10: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0000bc20: 2020 2040 636c 6173 736d 6574 686f 6420     @classmethod 
-0000bc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc50: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0000bc60: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0000bc70: 2020 2064 6566 2066 6578 7028 7365 6c66     def fexp(self
-0000bc80: 293a 2020 2020 2020 2020 2020 2020 2020  ):              
-0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bca0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0000bcb0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0000bcc0: 2020 2020 2020 2072 6574 7572 6e20 6675         return fu
-0000bcd0: 6e63 2e63 6f6e 6361 7428 636c 732e 6669  nc.concat(cls.fi
-0000bce0: 7273 745f 6e61 6d65 2c20 2720 272c 2020  rst_name, ' ',  
-0000bcf0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0000bd00: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0000bd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd20: 2020 2020 2020 2020 2020 636c 732e 6c61            cls.la
-0000bd30: 7374 5f6e 616d 6529 2020 2020 2020 2020  st_name)        
-0000bd40: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0000bd50: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0000bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd90: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
-0000bda0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+0000bbe0: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
+0000bbf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+0000bc00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bc10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bc20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bc30: 2d2b 0a7c 2060 606d 326d 5f6c 6f63 616c  -+.| ``m2m_local
+0000bc40: 5f63 6f6c 756d 6e73 6060 2020 7c20 436f  _columns``  | Co
+0000bc50: 6c75 6d6e 206e 616d 6520 696e 2074 6865  lumn name in the
+0000bc60: 206a 6f69 6e20 7461 626c 6520 7768 6963   join table whic
+0000bc70: 6820 686f 6c64 7320 7468 6520 2020 2020  h holds the     
+0000bc80: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000bc90: 2020 2020 2020 2020 2020 2020 7c20 666f              | fo
+0000bca0: 7265 6967 6e20 6b65 7920 746f 2074 6865  reign key to the
+0000bcb0: 206d 6f64 656c 2020 2020 2020 2020 2020   model          
+0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcd0: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
+0000bce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+0000bcf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bd00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bd10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bd20: 2d2b 0a7c 2060 606d 616e 7932 6d61 6e79  -+.| ``many2many
+0000bd30: 6060 2020 2020 2020 2020 2020 7c20 4f70  ``          | Op
+0000bd40: 706f 7369 7465 204d 616e 7932 4d61 6e79  posite Many2Many
+0000bd50: 206c 696e 6b20 7769 7468 2074 6869 7320   link with this 
+0000bd60: 7265 6c61 7469 6f6e 7368 6970 2020 2020  relationship    
+0000bd70: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
+0000bd80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+0000bd90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bda0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000bdb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bdc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bdd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bde0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a 5061 7261  ---------+..Para
-0000bdf0: 6d65 7465 7273 2066 6f72 2060 6046 6965  meters for ``Fie
-0000be00: 6c64 2e4a 736f 6e52 656c 6174 6564 6060  ld.JsonRelated``
-0000be10: 0a0a 4465 6669 6e65 2073 6574 7465 722c  ..Define setter,
-0000be20: 2067 6574 7465 7220 666f 7220 6120 6b65   getter for a ke
-0000be30: 7920 696e 202a 2a43 6f6c 756d 6e2e 4a73  y in **Column.Js
-0000be40: 6f6e 2a2a 2c20 6974 2069 7320 6120 6865  on**, it is a he
-0000be50: 6c70 6572 2074 6f20 646f 2061 6e20 616c  lper to do an al
-0000be60: 6961 730a 6f66 2073 7065 6369 6669 6320  ias.of specific 
-0000be70: 656e 7472 7920 696e 2061 202a 2a43 6f6c  entry in a **Col
-0000be80: 756d 6e2e 4a73 6f6e 2a2a 2e0a 0a2b 2d2d  umn.Json**...+--
-0000be90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bea0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-0000beb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2050  -----------+.| P
-0000bee0: 6172 616d 6574 6572 2020 2020 2020 2020  arameter        
-0000bef0: 207c 2044 6573 6372 6970 7469 6f6e 2020   | Description  
-0000bf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf20: 2020 2020 2020 2020 2020 207c 0a2b 3d3d             |.+==
-0000bf30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000bf40: 3d2b 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  =+==============
-0000bf50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000bf60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000bf70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 0a7c 2060  ===========+.| `
-0000bf80: 606a 736f 6e5f 636f 6c75 6d6e 6060 2020  `json_column``  
-0000bf90: 207c 206e 616d 6520 6f66 2074 6865 206a   | name of the j
-0000bfa0: 736f 6e20 636f 6c75 6d6e 2069 6e20 7468  son column in th
-0000bfb0: 6520 4d6f 6465 6c20 2020 2020 2020 2020  e Model         
-0000bfc0: 2020 2020 2020 2020 2020 207c 0a2b 2d2d             |.+--
-0000bfd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bfe0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-0000bff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2060  -----------+.| `
-0000c020: 606b 6579 7360 6020 2020 2020 2020 2020  `keys``         
-0000c030: 207c 206c 6973 7420 6f66 2073 7472 696e   | list of strin
-0000c040: 672c 2072 6570 7265 7365 6e74 2074 6865  g, represent the
-0000c050: 2070 6174 6820 696e 206a 736f 6e20 746f   path in json to
-0000c060: 2073 746f 7265 2061 6e64 207c 0a7c 2020   store and |.|  
+0000bdc0: 2d2b 0a7c 2060 6063 6f6d 7075 7465 5f6a  -+.| ``compute_j
+0000bdd0: 6f69 6e60 6020 2020 2020 2020 7c20 466f  oin``       | Fo
+0000bde0: 7263 6520 746f 2063 6f6d 7075 7465 2073  rce to compute s
+0000bdf0: 6563 6f6e 6461 7279 6a6f 696e 2061 6e64  econdaryjoin and
+0000be00: 2070 7269 6d61 7279 6a6f 696e 2020 2020   primaryjoin    
+0000be10: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000be20: 2020 2020 2020 2020 2020 2020 7c20 496e              | In
+0000be30: 2074 6865 206d 6f73 7420 6361 7365 2074   the most case t
+0000be40: 6869 7320 6973 2066 6f72 6269 6464 656e  his is forbidden
+0000be50: 2062 6563 6175 7365 2069 7420 6973 2020   because it is  
+0000be60: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000be70: 2020 2020 2020 2020 2020 2020 7c20 6461              | da
+0000be80: 6e67 656f 7572 6f75 732c 2054 6865 206f  ngeourous, The o
+0000be90: 6e6c 7920 6361 7365 2077 6865 7265 2074  nly case where t
+0000bea0: 6865 2063 6f6d 7075 7465 2069 7320 2020  he compute is   
+0000beb0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000bec0: 2020 2020 2020 2020 2020 2020 7c20 7265              | re
+0000bed0: 7175 6972 6564 2c20 6973 2077 6865 6e20  quired, is when 
+0000bee0: 7468 6520 6d6f 6465 6c5f 6a6f 696e 2068  the model_join h
+0000bef0: 6176 6520 6d6f 7265 2074 6861 6e20 2020  ave more than   
+0000bf00: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000bf10: 2020 2020 2020 2020 2020 2020 7c20 6f6e              | on
+0000bf20: 6520 7072 696d 6172 7920 6b65 7920 746f  e primary key to
+0000bf30: 2074 6865 206d 6169 6e20 6d6f 6465 6c20   the main model 
+0000bf40: 666f 7220 7269 6368 2020 2020 2020 2020  for rich        
+0000bf50: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000bf60: 2020 2020 2020 2020 2020 2020 7c20 4d61              | Ma
+0000bf70: 6e79 324d 616e 7920 2020 2020 2020 2020  ny2Many         
+0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfa0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000bfb0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bff0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000c000: 2020 2020 2020 2020 2020 2020 7c20 2e2e              | ..
+0000c010: 206e 6f74 653a 3a20 2020 2020 2020 2020   note::         
+0000c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c040: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000c050: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0000c060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c080: 207c 2067 6574 2074 6865 2076 616c 7565   | get the value
-0000c090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0b0: 2020 2020 2020 2020 2020 207c 0a2b 2d2d             |.+--
-0000c0c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c0d0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-0000c0e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c0f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2060  -----------+.| `
-0000c110: 6067 6574 5f61 6461 7074 6572 6060 2020  `get_adapter``  
-0000c120: 207c 206d 6574 686f 6420 746f 2063 6f6e   | method to con
-0000c130: 7665 7274 2074 6865 2064 6174 6520 6166  vert the date af
-0000c140: 7465 7220 6765 7420 6974 2e20 5468 6973  ter get it. This
-0000c150: 2076 616c 7565 2020 2020 207c 0a7c 2020   value     |.|  
+0000c080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c090: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000c0a0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0000c0b0: 2020 496e 2074 6865 2063 6173 6520 7768    In the case wh
+0000c0c0: 6572 6520 7468 6520 626f 7468 206d 6f64  ere the both mod
+0000c0d0: 656c 2061 7265 2074 6865 2073 616d 6520  el are the same 
+0000c0e0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000c0f0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0000c100: 2020 7468 6973 206f 7074 696f 6e20 6973    this option is
+0000c110: 2066 6f72 6365 6420 2020 2020 2020 2020   forced         
+0000c120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c130: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0000c140: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0000c150: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c170: 207c 2063 616e 2062 6520 7468 6520 6e61   | can be the na
-0000c180: 6d65 206f 6620 6120 6d65 7468 6f64 206f  me of a method o
-0000c190: 6e20 7468 6520 6d6f 6465 6c20 2020 2020  n the model     
-0000c1a0: 2020 2020 2020 2020 2020 207c 0a2b 2d2d             |.+--
+0000c170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c180: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
+0000c190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+0000c1a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000c1b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c1c0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-0000c1d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c1e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c1f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2060  -----------+.| `
-0000c200: 6073 6574 5f61 6461 7074 6572 6060 2020  `set_adapter``  
-0000c210: 207c 206d 6574 686f 6420 746f 2063 6f6e   | method to con
-0000c220: 7665 7274 2074 6865 2064 6174 6520 6265  vert the date be
-0000c230: 666f 7265 2073 746f 7265 2069 742e 2054  fore store it. T
-0000c240: 6869 7320 7661 6c75 6520 207c 0a7c 2020  his value  |.|  
-0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c260: 207c 2063 616e 2062 6520 7468 6520 6e61   | can be the na
-0000c270: 6d65 206f 6620 6120 6d65 7468 6f64 206f  me of a method o
-0000c280: 6e20 7468 6520 6d6f 6465 6c20 2020 2020  n the model     
-0000c290: 2020 2020 2020 2020 2020 207c 0a2b 2d2d             |.+--
-0000c2a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c2b0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-0000c2c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c2d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c2e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a 4d69  -----------+..Mi
-0000c2f0: 7869 6e0a 2d2d 2d2d 2d0a 0a41 204d 6978  xin.-----..A Mix
-0000c300: 696e 206c 6f6f 6b73 206c 696b 6520 6120  in looks like a 
-0000c310: 4d6f 6465 6c2c 2062 7574 2068 6173 206e  Model, but has n
-0000c320: 6f20 7461 626c 6573 2e20 4120 4d69 7869  o tables. A Mixi
-0000c330: 6e20 6164 6473 2062 6568 6176 696f 7572  n adds behaviour
-0000c340: 2074 6f0a 6120 4d6f 6465 6c20 7769 7468   to.a Model with
-0000c350: 2050 7974 686f 6e20 696e 6865 7269 7461   Python inherita
-0000c360: 6e63 653a 3a0a 0a20 2020 2040 7265 6769  nce::..    @regi
-0000c370: 7374 6572 284d 6978 696e 290a 2020 2020  ster(Mixin).    
-0000c380: 636c 6173 7320 4d79 4d69 7869 6e3a 0a0a  class MyMixin:..
-0000c390: 2020 2020 2020 2020 6465 6620 666f 6f28          def foo(
-0000c3a0: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
-0000c3b0: 6173 730a 0a20 2020 2040 7265 6769 7374  ass..    @regist
-0000c3c0: 6572 284d 6f64 656c 290a 2020 2020 636c  er(Model).    cl
-0000c3d0: 6173 7320 4d79 4d6f 6465 6c28 4d69 7869  ass MyModel(Mixi
-0000c3e0: 6e2e 4d79 4d69 7869 6e29 3a0a 2020 2020  n.MyMixin):.    
-0000c3f0: 2020 2020 7061 7373 0a0a 2020 2020 2d2d      pass..    --
-0000c400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c420: 0a0a 2020 2020 6173 7365 7274 2068 6173  ..    assert has
-0000c430: 6174 7472 2872 6567 6973 7472 792e 4d79  attr(registry.My
-0000c440: 4d6f 6465 6c2c 2027 666f 6f27 290a 0a0a  Model, 'foo')...
-0000c450: 4966 2079 6f75 2069 6e68 6572 6974 2061  If you inherit a
-0000c460: 206d 6978 696e 2c20 616c 6c20 7468 6520   mixin, all the 
-0000c470: 6d6f 6465 6c73 2070 7265 7669 6f75 736c  models previousl
-0000c480: 7920 7573 696e 6720 7468 6520 6261 7365  y using the base
-0000c490: 206d 6978 696e 2061 6c73 6f20 6265 6e65   mixin also bene
-0000c4a0: 6669 740a 6672 6f6d 2074 6865 206f 7665  fit.from the ove
-0000c4b0: 726c 6f61 643a 3a0a 0a20 2020 2040 7265  rload::..    @re
-0000c4c0: 6769 7374 6572 284d 6978 696e 290a 2020  gister(Mixin).  
-0000c4d0: 2020 636c 6173 7320 4d79 4d69 7869 6e3a    class MyMixin:
-0000c4e0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-0000c4f0: 2020 2040 7265 6769 7374 6572 284d 6f64     @register(Mod
-0000c500: 656c 290a 2020 2020 636c 6173 7320 4d79  el).    class My
-0000c510: 4d6f 6465 6c28 4d69 7869 6e2e 4d79 4d69  Model(Mixin.MyMi
-0000c520: 7869 6e29 3a0a 2020 2020 2020 2020 7061  xin):.        pa
-0000c530: 7373 0a0a 2020 2020 4072 6567 6973 7465  ss..    @registe
-0000c540: 7228 4d69 7869 6e29 0a20 2020 2063 6c61  r(Mixin).    cla
-0000c550: 7373 204d 794d 6978 696e 3a0a 0a20 2020  ss MyMixin:..   
-0000c560: 2020 2020 2064 6566 2066 6f6f 2829 3a0a       def foo():.
-0000c570: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-0000c580: 0a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  ..    ----------
-0000c590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c5a0: 2d2d 2d2d 2d2d 2d2d 0a0a 2020 2020 6173  --------..    as
-0000c5b0: 7365 7274 2068 6173 6174 7472 2861 6e79  sert hasattr(any
-0000c5c0: 626c 6f6b 2e4d 794d 6f64 656c 2c20 2766  blok.MyModel, 'f
-0000c5d0: 6f6f 2729 0a0a 0a53 514c 2056 6965 770a  oo')...SQL View.
-0000c5e0: 2d2d 2d2d 2d2d 2d2d 0a0a 416e 2053 514c  --------..An SQL
-0000c5f0: 2076 6965 7720 6973 2061 206d 6f64 656c   view is a model
-0000c600: 2c20 7769 7468 2074 6865 2061 7267 756d  , with the argum
-0000c610: 656e 7420 6060 6661 6374 6f72 793d 616e  ent ``factory=an
-0000c620: 7962 6c6f 6b2e 6d6f 6465 6c2e 6661 6374  yblok.model.fact
-0000c630: 6f72 792e 5669 6577 4661 6374 6f72 7960  ory.ViewFactory`
-0000c640: 6020 696e 2074 6865 0a72 6567 6973 7465  ` in the.registe
-0000c650: 722e 2061 6e64 2074 6865 2063 6c61 7373  r. and the class
-0000c660: 6d65 7468 6f64 2060 6073 716c 616c 6368  method ``sqlalch
-0000c670: 656d 795f 7669 6577 5f64 6563 6c61 7261  emy_view_declara
-0000c680: 7469 6f6e 6060 3a3a 0a0a 2020 2020 6672  tion``::..    fr
-0000c690: 6f6d 2061 6e79 626c 6f6b 2e6d 6f64 656c  om anyblok.model
-0000c6a0: 2e66 6163 746f 7279 2069 6d70 6f72 7420  .factory import 
-0000c6b0: 5669 6577 4661 6374 6f72 790a 0a20 2020  ViewFactory..   
-0000c6c0: 2040 7265 6769 7374 6572 284d 6f64 656c   @register(Model
-0000c6d0: 290a 2020 2020 636c 6173 7320 5431 3a0a  ).    class T1:.
-0000c6e0: 2020 2020 2020 2020 6964 203d 2049 6e74          id = Int
-0000c6f0: 6567 6572 2870 7269 6d61 7279 5f6b 6579  eger(primary_key
-0000c700: 3d54 7275 6529 0a20 2020 2020 2020 2063  =True).        c
-0000c710: 6f64 6520 3d20 5374 7269 6e67 2829 0a20  ode = String(). 
-0000c720: 2020 2020 2020 2076 616c 203d 2049 6e74         val = Int
-0000c730: 6567 6572 2829 0a0a 2020 2020 4072 6567  eger()..    @reg
-0000c740: 6973 7465 7228 4d6f 6465 6c29 0a20 2020  ister(Model).   
-0000c750: 2063 6c61 7373 2054 323a 0a20 2020 2020   class T2:.     
-0000c760: 2020 2069 6420 3d20 496e 7465 6765 7228     id = Integer(
-0000c770: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
-0000c780: 290a 2020 2020 2020 2020 636f 6465 203d  ).        code =
-0000c790: 2053 7472 696e 6728 290a 2020 2020 2020   String().      
-0000c7a0: 2020 7661 6c20 3d20 496e 7465 6765 7228    val = Integer(
-0000c7b0: 290a 0a20 2020 2040 7265 6769 7374 6572  )..    @register
-0000c7c0: 284d 6f64 656c 2c20 6661 6374 6f72 793d  (Model, factory=
-0000c7d0: 5669 6577 4661 6374 6f72 7929 0a20 2020  ViewFactory).   
-0000c7e0: 2063 6c61 7373 2054 6573 7456 6965 773a   class TestView:
-0000c7f0: 0a20 2020 2020 2020 2063 6f64 6520 3d20  .        code = 
-0000c800: 5374 7269 6e67 2870 7269 6d61 7279 5f6b  String(primary_k
-0000c810: 6579 3d54 7275 6529 0a20 2020 2020 2020  ey=True).       
-0000c820: 2076 616c 3120 3d20 496e 7465 6765 7228   val1 = Integer(
-0000c830: 290a 2020 2020 2020 2020 7661 6c32 203d  ).        val2 =
-0000c840: 2049 6e74 6567 6572 2829 0a0a 2020 2020   Integer()..    
-0000c850: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-0000c860: 0a20 2020 2020 2020 2064 6566 2073 716c  .        def sql
-0000c870: 616c 6368 656d 795f 7669 6577 5f64 6563  alchemy_view_dec
-0000c880: 6c61 7261 7469 6f6e 2863 6c73 293a 0a20  laration(cls):. 
-0000c890: 2020 2020 2020 2020 2020 2022 2222 2054             """ T
-0000c8a0: 6869 7320 6d65 7468 6f64 206d 7573 7420  his method must 
-0000c8b0: 7265 7475 726e 2074 6865 2071 7565 7279  return the query
-0000c8c0: 206f 6620 7468 6520 7669 6577 2022 2222   of the view """
-0000c8d0: 0a20 2020 2020 2020 2020 2020 2054 3120  .            T1 
-0000c8e0: 3d20 636c 732e 616e 7962 6c6f 6b2e 5431  = cls.anyblok.T1
-0000c8f0: 0a20 2020 2020 2020 2020 2020 2054 3220  .            T2 
-0000c900: 3d20 636c 732e 616e 7962 6c6f 6b2e 5432  = cls.anyblok.T2
-0000c910: 0a20 2020 2020 2020 2020 2020 2071 7565  .            que
-0000c920: 7279 203d 2073 656c 6563 7428 5b54 312e  ry = select([T1.
-0000c930: 636f 6465 2e6c 6162 656c 2827 636f 6465  code.label('code
-0000c940: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-0000c950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c960: 5431 2e76 616c 2e6c 6162 656c 2827 7661  T1.val.label('va
-0000c970: 6c31 2729 2c0a 2020 2020 2020 2020 2020  l1'),.          
-0000c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c990: 2020 5432 2e76 616c 2e6c 6162 656c 2827    T2.val.label('
-0000c9a0: 7661 6c32 2729 5d29 0a20 2020 2020 2020  val2')]).       
-0000c9b0: 2020 2020 2072 6574 7572 6e20 7175 6572       return quer
-0000c9c0: 792e 7768 6572 6528 5431 2e63 6f64 6520  y.where(T1.code 
-0000c9d0: 3d3d 2054 322e 636f 6465 290a 0a0a 436f  == T2.code)...Co
-0000c9e0: 7265 0a2d 2d2d 2d0a 0a60 6043 6f72 6560  re.----..``Core`
-0000c9f0: 6020 6973 2061 206c 6f77 206c 6576 656c  ` is a low level
-0000ca00: 2073 6574 206f 6620 6465 636c 6172 6174   set of declarat
-0000ca10: 696f 6e73 2066 6f72 2061 6c6c 2074 6865  ions for all the
-0000ca20: 204d 6f64 656c 7320 6f66 2041 6e79 426c   Models of AnyBl
-0000ca30: 6f6b 2e20 6060 436f 7265 6060 2061 6464  ok. ``Core`` add
-0000ca40: 730a 6765 6e65 7261 6c20 6265 6861 7669  s.general behavi
-0000ca50: 6f75 7220 746f 2074 6865 2061 7070 6c69  our to the appli
-0000ca60: 6361 7469 6f6e 2e0a 0a2e 2e20 7761 726e  cation..... warn
-0000ca70: 696e 673a 3a0a 0a20 2020 2043 6f72 6520  ing::..    Core 
-0000ca80: 6361 6e20 6e6f 7420 696e 6865 7269 7420  can not inherit 
-0000ca90: 4d6f 6465 6c2c 204d 6978 696e 2c20 436f  Model, Mixin, Co
-0000caa0: 7265 2c20 6f72 206f 7468 6572 2064 6563  re, or other dec
-0000cab0: 6c61 7261 7469 6f6e 2074 7970 652e 0a0a  laration type...
-0000cac0: 4261 7365 0a7e 7e7e 7e0a 0a41 6464 2061  Base.~~~~..Add a
-0000cad0: 2062 6568 6176 696f 7572 2069 6e20 616c   behaviour in al
-0000cae0: 6c20 7468 6520 4d6f 6465 6c73 2c20 4561  l the Models, Ea
-0000caf0: 6368 204d 6f64 656c 2069 6e68 6572 6974  ch Model inherit
-0000cb00: 7320 4261 7365 2e20 466f 7220 696e 7374  s Base. For inst
-0000cb10: 616e 6365 2c20 7468 650a 6060 6669 7265  ance, the.``fire
-0000cb20: 6060 206d 6574 686f 6420 6f66 2074 6865  `` method of the
-0000cb30: 2065 7665 6e74 2063 6f6d 6520 6672 6f6d   event come from
-0000cb40: 2060 6043 6f72 652e 4261 7365 6060 2e0a   ``Core.Base``..
-0000cb50: 0a3a 3a0a 0a20 2020 2066 726f 6d20 616e  .::..    from an
-0000cb60: 7962 6c6f 6b20 696d 706f 7274 2044 6563  yblok import Dec
-0000cb70: 6c61 7261 7469 6f6e 730a 0a0a 2020 2020  larations...    
-0000cb80: 4044 6563 6c61 7261 7469 6f6e 732e 7265  @Declarations.re
-0000cb90: 6769 7374 6572 2844 6563 6c61 7261 7469  gister(Declarati
-0000cba0: 6f6e 732e 436f 7265 290a 2020 2020 636c  ons.Core).    cl
-0000cbb0: 6173 7320 4261 7365 3a0a 2020 2020 2020  ass Base:.      
-0000cbc0: 2020 7061 7373 0a0a 5371 6c42 6173 650a    pass..SqlBase.
-0000cbd0: 7e7e 7e7e 7e7e 7e0a 0a4f 6e6c 7920 7468  ~~~~~~~..Only th
-0000cbe0: 6520 4d6f 6465 6c73 2077 6974 6820 6060  e Models with ``
-0000cbf0: 4669 656c 6460 602c 2060 6043 6f6c 756d  Field``, ``Colum
-0000cc00: 6e60 602c 2060 6052 656c 6174 696f 6e53  n``, ``RelationS
-0000cc10: 6869 7060 6020 696e 6865 7269 7473 2060  hip`` inherits `
-0000cc20: 6043 6f72 652e 5371 6c42 6173 6560 602e  `Core.SqlBase``.
-0000cc30: 0a46 6f72 2069 6e73 7461 6e63 652c 2074  .For instance, t
-0000cc40: 6865 2060 6069 6e73 6572 7460 6020 6d65  he ``insert`` me
-0000cc50: 7468 6f64 206f 6e6c 7920 6d61 6b65 7320  thod only makes 
-0000cc60: 7365 6e73 6520 666f 7220 7468 6520 6060  sense for the ``
-0000cc70: 4d6f 6465 6c60 6020 7769 7468 2061 2074  Model`` with a t
-0000cc80: 6162 6c65 2e0a 0a3a 3a0a 0a20 2020 2066  able...::..    f
-0000cc90: 726f 6d20 616e 7962 6c6f 6b20 696d 706f  rom anyblok impo
-0000cca0: 7274 2044 6563 6c61 7261 7469 6f6e 730a  rt Declarations.
-0000ccb0: 0a0a 2020 2020 4044 6563 6c61 7261 7469  ..    @Declarati
-0000ccc0: 6f6e 732e 7265 6769 7374 6572 2844 6563  ons.register(Dec
-0000ccd0: 6c61 7261 7469 6f6e 732e 436f 7265 290a  larations.Core).
-0000cce0: 2020 2020 636c 6173 7320 5371 6c42 6173      class SqlBas
-0000ccf0: 653a 0a20 2020 2020 2020 2070 6173 730a  e:.        pass.
-0000cd00: 0a53 716c 5669 6577 4261 7365 0a7e 7e7e  .SqlViewBase.~~~
-0000cd10: 7e7e 7e7e 7e7e 7e7e 0a0a 4c69 6b65 2060  ~~~~~~~~..Like `
-0000cd20: 6053 716c 4261 7365 6060 2c20 6f6e 6c79  `SqlBase``, only
-0000cd30: 2074 6865 2060 6053 716c 5669 6577 6060   the ``SqlView``
-0000cd40: 2069 6e68 6572 6974 7320 7468 6973 2060   inherits this `
-0000cd50: 6043 6f72 6560 6020 636c 6173 732e 0a0a  `Core`` class...
-0000cd60: 3a3a 0a0a 2020 2020 6672 6f6d 2061 6e79  ::..    from any
-0000cd70: 626c 6f6b 2069 6d70 6f72 7420 4465 636c  blok import Decl
-0000cd80: 6172 6174 696f 6e73 0a0a 0a20 2020 2040  arations...    @
-0000cd90: 4465 636c 6172 6174 696f 6e73 2e72 6567  Declarations.reg
-0000cda0: 6973 7465 7228 4465 636c 6172 6174 696f  ister(Declaratio
-0000cdb0: 6e73 2e43 6f72 6529 0a20 2020 2063 6c61  ns.Core).    cla
-0000cdc0: 7373 2053 716c 5669 6577 4261 7365 3a0a  ss SqlViewBase:.
-0000cdd0: 2020 2020 2020 2020 7061 7373 0a0a 5175          pass..Qu
-0000cde0: 6572 790a 7e7e 7e7e 7e0a 0a4f 7665 726c  ery.~~~~~..Overl
-0000cdf0: 6f61 6473 2074 6865 2053 514c 416c 6368  oads the SQLAlch
-0000ce00: 656d 7920 6060 5175 6572 7960 6020 636c  emy ``Query`` cl
-0000ce10: 6173 732e 0a0a 3a3a 0a0a 2020 2020 6672  ass...::..    fr
-0000ce20: 6f6d 2061 6e79 626c 6f6b 2069 6d70 6f72  om anyblok impor
-0000ce30: 7420 4465 636c 6172 6174 696f 6e73 0a0a  t Declarations..
-0000ce40: 0a20 2020 2040 4465 636c 6172 6174 696f  .    @Declaratio
-0000ce50: 6e73 2e72 6567 6973 7465 7228 4465 636c  ns.register(Decl
-0000ce60: 6172 6174 696f 6e73 2e43 6f72 6529 0a20  arations.Core). 
-0000ce70: 2020 2063 6c61 7373 2051 7565 7279 0a20     class Query. 
-0000ce80: 2020 2020 2020 2070 6173 730a 0a53 6573         pass..Ses
-0000ce90: 7369 6f6e 0a7e 7e7e 7e7e 7e7e 0a0a 4f76  sion.~~~~~~~..Ov
-0000cea0: 6572 6c6f 6164 7320 7468 6520 5351 4c41  erloads the SQLA
-0000ceb0: 6c63 6865 6d79 2060 6053 6573 7369 6f6e  lchemy ``Session
-0000cec0: 6060 2063 6c61 7373 2e0a 0a3a 3a0a 0a20  `` class...::.. 
-0000ced0: 2020 2066 726f 6d20 616e 7962 6c6f 6b20     from anyblok 
-0000cee0: 696d 706f 7274 2044 6563 6c61 7261 7469  import Declarati
-0000cef0: 6f6e 730a 0a0a 2020 2020 4044 6563 6c61  ons...    @Decla
-0000cf00: 7261 7469 6f6e 732e 7265 6769 7374 6572  rations.register
-0000cf10: 2844 6563 6c61 7261 7469 6f6e 732e 436f  (Declarations.Co
-0000cf20: 7265 290a 2020 2020 636c 6173 7320 5365  re).    class Se
-0000cf30: 7373 696f 6e0a 2020 2020 2020 2020 7061  ssion.        pa
-0000cf40: 7373 0a0a 496e 7374 7275 6d65 6e74 6564  ss..Instrumented
-0000cf50: 4c69 7374 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  List.~~~~~~~~~~~
-0000cf60: 7e7e 7e7e 7e0a 0a3a 3a0a 0a20 2020 2066  ~~~~~..::..    f
-0000cf70: 726f 6d20 616e 7962 6c6f 6b20 696d 706f  rom anyblok impo
-0000cf80: 7274 2044 6563 6c61 7261 7469 6f6e 730a  rt Declarations.
-0000cf90: 0a0a 2020 2020 4044 6563 6c61 7261 7469  ..    @Declarati
-0000cfa0: 6f6e 732e 7265 6769 7374 6572 2844 6563  ons.register(Dec
-0000cfb0: 6c61 7261 7469 6f6e 732e 436f 7265 290a  larations.Core).
-0000cfc0: 2020 2020 636c 6173 7320 496e 7374 7275      class Instru
-0000cfd0: 6d65 6e74 6564 4c69 7374 0a20 2020 2020  mentedList.     
-0000cfe0: 2020 2070 6173 730a 0a60 6049 6e73 7472     pass..``Instr
-0000cff0: 756d 656e 7465 644c 6973 7460 6020 6973  umentedList`` is
-0000d000: 2074 6865 2063 6c61 7373 2072 6574 7572   the class retur
-0000d010: 6e65 6420 6279 2074 6865 2051 7565 7279  ned by the Query
-0000d020: 2066 6f72 2061 6c6c 2074 6865 206c 6973   for all the lis
-0000d030: 7420 7265 7375 6c74 0a6c 696b 653a 0a0a  t result.like:..
-0000d040: 2a20 7175 6572 792e 616c 6c28 290a 2a20  * query.all().* 
-0000d050: 7265 6c61 7469 6f6e 7368 6970 206c 6973  relationship lis
-0000d060: 7420 284d 616e 7932 4d61 6e79 2c20 4f6e  t (Many2Many, On
-0000d070: 6532 4d61 6e79 290a 0a41 6464 7320 736f  e2Many)..Adds so
-0000d080: 6d65 2066 6561 7475 7265 7320 6c69 6b65  me features like
-0000d090: 2067 6574 7469 6e67 2061 2073 7065 6369   getting a speci
-0000d0a0: 6669 6320 7072 6f70 6572 7479 206f 7220  fic property or 
-0000d0b0: 6361 6c6c 696e 6720 6120 6d65 7468 6f64  calling a method
-0000d0c0: 206f 6e20 616c 6c0a 7468 6520 656c 656d   on all.the elem
-0000d0d0: 656e 7473 206f 6620 7468 6520 6c69 7374  ents of the list
-0000d0e0: 3a3a 0a0a 2020 2020 4d79 4d6f 6465 6c2e  ::..    MyModel.
-0000d0f0: 7175 6572 7928 292e 616c 6c28 292e 666f  query().all().fo
-0000d100: 6f28 6261 7229 0a0a 5368 6172 696e 6720  o(bar)..Sharing 
-0000d110: 6120 7461 626c 6520 6265 7477 6565 6e20  a table between 
-0000d120: 6d6f 7265 2074 6861 6e20 6f6e 6520 6d6f  more than one mo
-0000d130: 6465 6c0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  del.------------
-0000d140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000d150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-0000d160: 0a53 514c 416c 6368 656d 7920 616c 6c6f  .SQLAlchemy allo
-0000d170: 7773 2074 776f 206d 6574 686f 6473 2074  ws two methods t
-0000d180: 6f20 7368 6172 6520 6120 7461 626c 6520  o share a table 
-0000d190: 6265 7477 6565 6e20 7477 6f20 6f72 206d  between two or m
-0000d1a0: 6f72 6520 6d61 7070 696e 670a 636c 6173  ore mapping.clas
-0000d1b0: 733a 0a0a 2a20 496e 6865 7269 7420 616e  s:..* Inherit an
-0000d1c0: 2053 514c 204d 6f64 656c 2069 6e20 6120   SQL Model in a 
-0000d1d0: 6e6f 6e2d 5351 4c20 4d6f 6465 6c3a 3a0a  non-SQL Model::.
-0000d1e0: 0a20 2020 2040 7265 6769 7374 6572 284d  .    @register(M
-0000d1f0: 6f64 656c 290a 2020 2020 636c 6173 7320  odel).    class 
-0000d200: 5465 7374 3a0a 2020 2020 2020 2020 6964  Test:.        id
-0000d210: 203d 2049 6e74 6567 6572 2870 7269 6d61   = Integer(prima
-0000d220: 7279 5f6b 6579 3d54 7275 6529 0a20 2020  ry_key=True).   
-0000d230: 2020 2020 206e 616d 6520 3d20 5374 7269       name = Stri
-0000d240: 6e67 2829 0a0a 2020 2020 4072 6567 6973  ng()..    @regis
-0000d250: 7465 7228 4d6f 6465 6c29 0a20 2020 2063  ter(Model).    c
-0000d260: 6c61 7373 2054 6573 7432 284d 6f64 656c  lass Test2(Model
-0000d270: 2e54 6573 7429 3a0a 2020 2020 2020 2020  .Test):.        
-0000d280: 7061 7373 0a0a 2020 2020 2d2d 2d2d 2d2d  pass..    ------
-0000d290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000d2a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000d2b0: 2d2d 0a0a 2020 2020 7431 203d 2054 6573  --..    t1 = Tes
-0000d2c0: 7431 2e69 6e73 6572 7428 6e61 6d65 3d27  t1.insert(name='
-0000d2d0: 666f 6f27 290a 2020 2020 6173 7365 7274  foo').    assert
-0000d2e0: 2054 6573 7432 2e71 7565 7279 2829 2e66   Test2.query().f
-0000d2f0: 696c 7465 7228 5465 7374 322e 6964 203d  ilter(Test2.id =
-0000d300: 3d20 7431 2e69 642c 0a20 2020 2020 2020  = t1.id,.       
+0000c1c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000c1d0: 2d2b 0a0a 2e2e 206e 6f74 653a 3a0a 0a20  -+.... note::.. 
+0000c1e0: 2020 2053 696e 6365 2030 2e34 2e30 2c20     Since 0.4.0, 
+0000c1f0: 7768 656e 2074 6865 2072 656c 6174 696f  when the relatio
+0000c200: 6e6e 616c 2074 6162 6c65 2069 7320 6372  nnal table is cr
+0000c210: 6561 7465 6420 6279 2041 6e79 426c 6f6b  eated by AnyBlok
+0000c220: 2c20 7468 650a 2020 2020 6d32 6d5f 636f  , the.    m2m_co
+0000c230: 6c75 6d6e 7320 6265 636f 6d6d 6520 666f  lumns becomme fo
+0000c240: 7265 6967 6e20 6b65 7973 0a0a 0a46 6965  reign keys...Fie
+0000c250: 6c64 0a2d 2d2d 2d2d 0a0a 546f 2064 6563  ld.-----..To dec
+0000c260: 6c61 7265 2061 2060 6046 6965 6c64 6060  lare a ``Field``
+0000c270: 2069 6e20 6120 6d6f 6465 6c2c 2061 6464   in a model, add
+0000c280: 2061 2046 6965 6c64 206f 6e20 7468 6520   a Field on the 
+0000c290: 4d6f 6465 6c2c 2074 6869 7320 6973 206e  Model, this is n
+0000c2a0: 6f74 2061 0a53 514c 2063 6f6c 756d 6e2e  ot a.SQL column.
+0000c2b0: 3a3a 0a0a 2020 2020 6672 6f6d 2061 6e79  ::..    from any
+0000c2c0: 626c 6f6b 2e64 6563 6c61 7261 7469 6f6e  blok.declaration
+0000c2d0: 7320 696d 706f 7274 2044 6563 6c61 7261  s import Declara
+0000c2e0: 7469 6f6e 730a 2020 2020 6672 6f6d 2061  tions.    from a
+0000c2f0: 6e79 626c 6f6b 2e66 6965 6c64 2069 6d70  nyblok.field imp
+0000c300: 6f72 7420 4675 6e63 7469 6f6e 0a20 2020  ort Function.   
+0000c310: 2066 726f 6d20 616e 7962 6c6f 6b2e 636f   from anyblok.co
+0000c320: 6c75 6d6e 2069 6d70 6f72 7420 496e 7465  lumn import Inte
+0000c330: 6765 720a 0a0a 2020 2020 4044 6563 6c61  ger...    @Decla
+0000c340: 7261 7469 6f6e 732e 7265 6769 7374 6572  rations.register
+0000c350: 2844 6563 6c61 7261 7469 6f6e 2e4d 6f64  (Declaration.Mod
+0000c360: 656c 290a 2020 2020 636c 6173 7320 4d79  el).    class My
+0000c370: 4d6f 6465 6c3a 0a0a 2020 2020 2020 2020  Model:..        
+0000c380: 6964 203d 2049 6e74 6567 6572 2870 7269  id = Integer(pri
+0000c390: 6d61 7279 5f6b 6579 3d54 7275 6529 0a20  mary_key=True). 
+0000c3a0: 2020 2020 2020 2066 6972 7374 5f6e 616d         first_nam
+0000c3b0: 6520 3d20 5374 7269 6e67 2829 0a20 2020  e = String().   
+0000c3c0: 2020 2020 206c 6173 745f 6e61 6d65 203d       last_name =
+0000c3d0: 2053 7472 696e 6728 290a 2020 2020 2020   String().      
+0000c3e0: 2020 6e61 6d65 203d 2046 756e 6374 696f    name = Functio
+0000c3f0: 6e28 6667 6574 3d27 6667 6574 272c 2066  n(fget='fget', f
+0000c400: 7365 743d 2766 7365 7427 2c20 6664 656c  set='fset', fdel
+0000c410: 3d27 6664 656c 272c 2066 6578 7072 3d27  ='fdel', fexpr='
+0000c420: 6665 7870 7227 290a 0a20 2020 2020 2020  fexpr')..       
+0000c430: 2064 6566 2066 6765 7428 7365 6c66 293a   def fget(self):
+0000c440: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000c450: 7572 6e20 277b 307d 207b 317d 272e 666f  urn '{0} {1}'.fo
+0000c460: 726d 6174 2873 656c 662e 6669 7273 745f  rmat(self.first_
+0000c470: 6e61 6d65 2c20 7365 6c66 2e6c 6173 745f  name, self.last_
+0000c480: 6e61 6d65 290a 0a20 2020 2020 2020 2064  name)..        d
+0000c490: 6566 2066 7365 7428 7365 6c66 2c20 7661  ef fset(self, va
+0000c4a0: 6c75 6529 3a0a 2020 2020 2020 2020 2020  lue):.          
+0000c4b0: 2020 7365 6c66 2e66 6972 7374 5f6e 616d    self.first_nam
+0000c4c0: 652c 2073 656c 662e 6c61 7374 5f6e 616d  e, self.last_nam
+0000c4d0: 6520 3d20 7661 6c75 652e 7370 6c69 7428  e = value.split(
+0000c4e0: 2720 272c 2031 290a 0a20 2020 2020 2020  ' ', 1)..       
+0000c4f0: 2064 6566 2066 6465 6c28 7365 6c66 293a   def fdel(self):
+0000c500: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c510: 662e 6669 7273 745f 6e61 6d65 203d 2073  f.first_name = s
+0000c520: 656c 662e 6c61 7374 5f6e 616d 6520 3d20  elf.last_name = 
+0000c530: 4e6f 6e65 0a0a 2020 2020 2020 2020 4063  None..        @c
+0000c540: 6c61 7373 6d65 7468 6f64 0a20 2020 2020  lassmethod.     
+0000c550: 2020 2064 6566 2066 6578 7072 2863 6c73     def fexpr(cls
+0000c560: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+0000c570: 6574 7572 6e20 6675 6e63 2e63 6f6e 6361  eturn func.conca
+0000c580: 7428 636c 732e 6669 7273 745f 6e61 6d65  t(cls.first_name
+0000c590: 2c20 2720 272c 2063 6c73 2e6c 6173 745f  , ' ', cls.last_
+0000c5a0: 6e61 6d65 290a 0a4c 6973 7420 6f66 2074  name)..List of t
+0000c5b0: 6865 2060 6046 6965 6c64 6060 2074 7970  he ``Field`` typ
+0000c5c0: 653a 0a0a 2a20 6060 4675 6e63 7469 6f6e  e:..* ``Function
+0000c5d0: 6060 0a2a 2060 604a 736f 6e52 656c 6174  ``.* ``JsonRelat
+0000c5e0: 6564 6060 0a0a 5061 7261 6d65 7465 7273  ed``..Parameters
+0000c5f0: 2066 6f72 2060 6046 6965 6c64 2e46 756e   for ``Field.Fun
+0000c600: 6374 696f 6e60 600a 0a2b 2d2d 2d2d 2d2d  ction``..+------
+0000c610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+0000c620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000c630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000c640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000c650: 2d2d 2d2d 2d2d 2d2b 0a7c 2050 6172 616d  -------+.| Param
+0000c660: 6574 6572 2020 2020 2020 2020 207c 2044  eter         | D
+0000c670: 6573 6372 6970 7469 6f6e 2020 2020 2020  escription      
+0000c680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6a0: 2020 2020 2020 207c 0a2b 3d3d 3d3d 3d3d         |.+======
+0000c6b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b 3d3d  =============+==
+0000c6c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000c6d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000c6e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000c6f0: 3d3d 3d3d 3d3d 3d2b 0a7c 2060 6066 6765  =======+.| ``fge
+0000c700: 7460 6020 2020 2020 2020 2020 207c 206e  t``          | n
+0000c710: 616d 6520 6f66 2074 6865 206d 6574 686f  ame of the metho
+0000c720: 6420 746f 2063 616c 6c20 746f 2067 6574  d to call to get
+0000c730: 2074 6865 2076 616c 7565 206f 6620 6669   the value of fi
+0000c740: 656c 643a 3a20 207c 0a7c 2020 2020 2020  eld::  |.|      
+0000c750: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000c760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c790: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000c7a0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000c7b0: 2064 6566 2066 6765 7428 7365 6c66 293a   def fget(self):
+0000c7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7e0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000c7f0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000c800: 2020 2020 2072 6574 7572 6e20 277b 307d       return '{0}
+0000c810: 207b 317d 272e 666f 726d 6174 2873 656c   {1}'.format(sel
+0000c820: 662e 6669 7273 745f 6e61 6d65 2c20 2020  f.first_name,   
+0000c830: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000c840: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c860: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000c870: 662e 6c61 7374 5f6e 616d 6529 2020 2020  f.last_name)    
+0000c880: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000c890: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000c8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8d0: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+0000c8e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+0000c8f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000c900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000c910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000c920: 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6066 7365  -------+.| ``fse
+0000c930: 7460 6020 2020 2020 2020 2020 207c 206e  t``          | n
+0000c940: 616d 6520 6f66 2074 6865 206d 6574 686f  ame of the metho
+0000c950: 6420 746f 2063 616c 6c20 746f 2073 6574  d to call to set
+0000c960: 2074 6865 2076 616c 7565 206f 6620 6669   the value of fi
+0000c970: 656c 643a 3a20 207c 0a7c 2020 2020 2020  eld::  |.|      
+0000c980: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9c0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000c9d0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000c9e0: 2064 6566 2066 7365 7428 7365 6c66 293a   def fset(self):
+0000c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca10: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000ca20: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000ca30: 2020 2020 2073 656c 662e 6669 7273 745f       self.first_
+0000ca40: 6e61 6d65 2c20 7365 6c66 2e6c 6173 745f  name, self.last_
+0000ca50: 6e61 6d65 203d 2076 616c 7565 2e73 706c  name = value.spl
+0000ca60: 6974 2827 2027 2c7c 0a7c 2020 2020 2020  it(' ',|.|      
+0000ca70: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000caa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cab0: 2020 2031 2920 207c 0a7c 2020 2020 2020     1)  |.|      
+0000cac0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000caf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb00: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+0000cb10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+0000cb20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000cb30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000cb40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000cb50: 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6066 6465  -------+.| ``fde
+0000cb60: 6c60 6020 2020 2020 2020 2020 207c 206e  l``          | n
+0000cb70: 616d 6520 6f66 2074 6865 206d 6574 686f  ame of the metho
+0000cb80: 6420 746f 2063 616c 6c20 746f 2064 656c  d to call to del
+0000cb90: 2074 6865 2076 616c 7565 206f 6620 6669   the value of fi
+0000cba0: 656c 643a 3a20 207c 0a7c 2020 2020 2020  eld::  |.|      
+0000cbb0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000cbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbf0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000cc00: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000cc10: 2064 6566 2066 6465 6c28 7365 6c66 293a   def fdel(self):
+0000cc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc40: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000cc50: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000cc60: 2020 2020 2073 656c 662e 6669 7273 745f       self.first_
+0000cc70: 6e61 6d65 203d 2073 656c 662e 6c61 7374  name = self.last
+0000cc80: 5f6e 616d 6520 3d20 4e6f 6e65 2020 2020  _name = None    
+0000cc90: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000cca0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000ccb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ccc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cce0: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+0000ccf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+0000cd00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000cd10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000cd20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000cd30: 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6066 6578  -------+.| ``fex
+0000cd40: 7060 6020 2020 2020 2020 2020 207c 206e  p``          | n
+0000cd50: 616d 6520 6f66 2074 6865 2063 6c61 7373  ame of the class
+0000cd60: 206d 6574 686f 6420 746f 2063 616c 6c20   method to call 
+0000cd70: 746f 2066 696c 7465 7220 6f6e 2074 6865  to filter on the
+0000cd80: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000cd90: 2020 2020 2020 2020 2020 2020 207c 2066               | f
+0000cda0: 6965 6c64 3a3a 2020 2020 2020 2020 2020  ield::          
+0000cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdd0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000cde0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce20: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000ce30: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000ce40: 2040 636c 6173 736d 6574 686f 6420 2020   @classmethod   
+0000ce50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce70: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000ce80: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000ce90: 2064 6566 2066 6578 7028 7365 6c66 293a   def fexp(self):
+0000cea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cec0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000ced0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000cee0: 2020 2020 2072 6574 7572 6e20 6675 6e63       return func
+0000cef0: 2e63 6f6e 6361 7428 636c 732e 6669 7273  .concat(cls.firs
+0000cf00: 745f 6e61 6d65 2c20 2720 272c 2020 2020  t_name, ' ',    
+0000cf10: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000cf20: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000cf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf40: 2020 2020 2020 2020 636c 732e 6c61 7374          cls.last
+0000cf50: 5f6e 616d 6529 2020 2020 2020 2020 2020  _name)          
+0000cf60: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000cf70: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000cf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfb0: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+0000cfc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+0000cfd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000cfe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000cff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d000: 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6066 7565  -------+.| ``fue
+0000d010: 7870 6060 2020 2020 2020 2020 207c 206e  xp``         | n
+0000d020: 616d 6520 6f66 2074 6865 2063 6c61 7373  ame of the class
+0000d030: 206d 6574 686f 6420 746f 2075 7064 6174   method to updat
+0000d040: 6520 7468 6520 6669 656c 6420 6672 6f6d  e the field from
+0000d050: 2071 7565 7279 207c 0a7c 2020 2020 2020   query |.|      
+0000d060: 2020 2020 2020 2020 2020 2020 207c 203a               | :
+0000d070: 3a20 2020 2020 2020 2020 2020 2020 2020  :               
+0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0a0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000d0b0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000d0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0f0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000d100: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000d110: 2040 636c 6173 736d 6574 686f 6420 2020   @classmethod   
+0000d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d140: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000d150: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000d160: 2064 6566 2066 7565 7870 2873 656c 6629   def fuexp(self)
+0000d170: 3a20 2020 2020 2020 2020 2020 2020 2020  :               
+0000d180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d190: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000d1a0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000d1b0: 2020 2020 2066 6e61 6d65 2c20 6c6e 616d       fname, lnam
+0000d1c0: 6520 3d20 7661 6c75 652e 7370 6c69 7428  e = value.split(
+0000d1d0: 2220 222c 2031 2920 2020 2020 2020 2020  " ", 1)         
+0000d1e0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000d1f0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000d200: 2020 2020 2072 6574 7572 6e20 5b20 2020       return [   
+0000d210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d230: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000d240: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000d250: 2020 2020 2020 2020 2028 636c 732e 6669           (cls.fi
+0000d260: 7273 745f 6e61 6d65 2c20 666e 616d 6529  rst_name, fname)
+0000d270: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
+0000d280: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000d290: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000d2a0: 2020 2020 2020 2020 2028 636c 732e 6c61           (cls.la
+0000d2b0: 7374 5f6e 616d 652c 206c 6e61 6d65 292c  st_name, lname),
+0000d2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2d0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000d2e0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000d2f0: 2020 2020 205d 2020 2020 2020 2020 2020       ]          
+0000d300: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000d310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d320: 2020 2020 2020 2020 2054 6573 7432 2e6e           Test2.n
-0000d330: 616d 6520 3d3d 2074 312e 6e61 6d65 292e  ame == t1.name).
-0000d340: 636f 756e 7428 2920 3d3d 2031 0a0a 2a20  count() == 1..* 
-0000d350: 5368 6172 6520 7468 6520 6060 5f5f 7461  Share the ``__ta
-0000d360: 626c 655f 5f60 602e 0a20 2020 2041 6e79  ble__``..    Any
-0000d370: 426c 6f6b 2063 616e 6e6f 7420 6769 7665  Blok cannot give
-0000d380: 2074 6865 2074 6162 6c65 2061 7420 7468   the table at th
-0000d390: 6520 6465 636c 6172 6174 696f 6e2c 2062  e declaration, b
-0000d3a0: 6563 6175 7365 2074 6865 2074 6162 6c65  ecause the table
-0000d3b0: 2064 6f65 7320 6e6f 740a 2020 2020 6578   does not.    ex
-0000d3c0: 6973 7420 7965 742e 2042 7574 2064 7572  ist yet. But dur
-0000d3d0: 696e 6720 7468 6520 6173 7365 6d62 6c79  ing the assembly
-0000d3e0: 2c20 6966 2074 6865 2074 6162 6c65 2065  , if the table e
-0000d3f0: 7869 7374 7320 616e 6420 7468 6520 6d6f  xists and the mo
-0000d400: 6465 6c0a 2020 2020 6861 7320 7468 6520  del.    has the 
-0000d410: 6e61 6d65 206f 6620 7468 6973 2074 6162  name of this tab
-0000d420: 6c65 2c20 416e 7942 6c6f 6b20 6469 7265  le, AnyBlok dire
-0000d430: 6374 6c79 206c 696e 6b73 2074 6865 2074  ctly links the t
-0000d440: 6162 6c65 2e20 546f 0a20 2020 2064 6566  able. To.    def
-0000d450: 696e 6520 7468 6520 7461 626c 6520 796f  ine the table yo
-0000d460: 7520 6d75 7374 2075 7365 2074 6865 206e  u must use the n
-0000d470: 616d 6564 2061 7267 756d 656e 7420 6060  amed argument ``
-0000d480: 7461 626c 656e 616d 6560 6020 696e 2074  tablename`` in t
-0000d490: 6865 0a20 2020 2060 6072 6567 6973 7465  he.    ``registe
-0000d4a0: 7260 600a 0a20 2020 203a 3a0a 0a20 2020  r``..    ::..   
-0000d4b0: 2020 2020 2040 7265 6769 7374 6572 284d       @register(M
-0000d4c0: 6f64 656c 290a 2020 2020 2020 2020 636c  odel).        cl
-0000d4d0: 6173 7320 5465 7374 3a0a 2020 2020 2020  ass Test:.      
-0000d4e0: 2020 2020 2020 6964 203d 2049 6e74 6567        id = Integ
-0000d4f0: 6572 2870 7269 6d61 7279 5f6b 6579 3d54  er(primary_key=T
-0000d500: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-0000d510: 206e 616d 6520 3d20 5374 7269 6e67 2829   name = String()
-0000d520: 0a0a 2020 2020 2020 2020 4072 6567 6973  ..        @regis
-0000d530: 7465 7228 4d6f 6465 6c2c 2074 6162 6c65  ter(Model, table
-0000d540: 6e61 6d65 3d4d 6f64 656c 2e54 6573 7429  name=Model.Test)
-0000d550: 0a20 2020 2020 2020 2063 6c61 7373 2054  .        class T
-0000d560: 6573 7432 3a0a 2020 2020 2020 2020 2020  est2:.          
-0000d570: 2020 6964 203d 2049 6e74 6567 6572 2870    id = Integer(p
-0000d580: 7269 6d61 7279 5f6b 6579 3d54 7275 6529  rimary_key=True)
-0000d590: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
-0000d5a0: 6520 3d20 5374 7269 6e67 2829 0a0a 2020  e = String()..  
-0000d5b0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+0000d320: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0000d330: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0000d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d370: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+0000d380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+0000d390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d3a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d3b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d3c0: 2d2d 2d2d 2d2d 2d2b 0a0a 5061 7261 6d65  -------+..Parame
+0000d3d0: 7465 7273 2066 6f72 2060 6046 6965 6c64  ters for ``Field
+0000d3e0: 2e4a 736f 6e52 656c 6174 6564 6060 0a0a  .JsonRelated``..
+0000d3f0: 4465 6669 6e65 2073 6574 7465 722c 2067  Define setter, g
+0000d400: 6574 7465 7220 666f 7220 6120 6b65 7920  etter for a key 
+0000d410: 696e 202a 2a43 6f6c 756d 6e2e 4a73 6f6e  in **Column.Json
+0000d420: 2a2a 2c20 6974 2069 7320 6120 6865 6c70  **, it is a help
+0000d430: 6572 2074 6f20 646f 2061 6e20 616c 6961  er to do an alia
+0000d440: 730a 6f66 2073 7065 6369 6669 6320 656e  s.of specific en
+0000d450: 7472 7920 696e 2061 202a 2a43 6f6c 756d  try in a **Colum
+0000d460: 6e2e 4a73 6f6e 2a2a 2e0a 0a2b 2d2d 2d2d  n.Json**...+----
+0000d470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+0000d480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d4a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d4b0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2050 6172  ---------+.| Par
+0000d4c0: 616d 6574 6572 2020 2020 2020 2020 207c  ameter         |
+0000d4d0: 2044 6573 6372 6970 7469 6f6e 2020 2020   Description    
+0000d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d500: 2020 2020 2020 2020 207c 0a2b 3d3d 3d3d           |.+====
+0000d510: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d2b  ===============+
+0000d520: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000d530: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000d540: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000d550: 3d3d 3d3d 3d3d 3d3d 3d2b 0a7c 2060 606a  =========+.| ``j
+0000d560: 736f 6e5f 636f 6c75 6d6e 6060 2020 207c  son_column``   |
+0000d570: 206e 616d 6520 6f66 2074 6865 206a 736f   name of the jso
+0000d580: 6e20 636f 6c75 6d6e 2069 6e20 7468 6520  n column in the 
+0000d590: 4d6f 6465 6c20 2020 2020 2020 2020 2020  Model           
+0000d5a0: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
+0000d5b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
 0000d5c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000d5d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-0000d5e0: 2020 2020 2020 2020 7431 203d 2054 6573          t1 = Tes
-0000d5f0: 7431 2e69 6e73 6572 7428 6e61 6d65 3d27  t1.insert(name='
-0000d600: 666f 6f27 290a 2020 2020 2020 2020 6173  foo').        as
-0000d610: 7365 7274 2054 6573 7432 2e71 7565 7279  sert Test2.query
-0000d620: 2829 2e66 696c 7465 7228 5465 7374 322e  ().filter(Test2.
-0000d630: 6964 203d 3d20 7431 2e69 642c 0a20 2020  id == t1.id,.   
-0000d640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d660: 2054 6573 7432 2e6e 616d 6520 3d3d 2074   Test2.name == t
-0000d670: 312e 6e61 6d65 292e 636f 756e 7428 2920  1.name).count() 
-0000d680: 3d3d 2031 0a0a 2020 2020 2e2e 2077 6172  == 1..    .. war
-0000d690: 6e69 6e67 3a3a 0a20 2020 2020 2020 2054  ning::.        T
-0000d6a0: 6865 7265 2061 7265 206e 6f20 6368 6563  here are no chec
-0000d6b0: 6b73 206f 6e20 7468 6520 6578 6973 7469  ks on the existi
-0000d6c0: 6e67 2063 6f6c 756d 6e73 2e0a 0a53 6861  ng columns...Sha
-0000d6d0: 7269 6e67 2061 2076 6965 7720 6265 7477  ring a view betw
-0000d6e0: 6565 6e20 6d6f 7265 2074 6861 6e20 6f6e  een more than on
-0000d6f0: 6520 6d6f 6465 6c0a 2d2d 2d2d 2d2d 2d2d  e model.--------
-0000d700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000d710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000d720: 2d2d 0a0a 5368 6172 696e 6720 6120 7669  --..Sharing a vi
-0000d730: 6577 2062 6574 7765 656e 2074 776f 204d  ew between two M
-0000d740: 6f64 656c 7320 6973 2074 6865 206d 6572  odels is the mer
-0000d750: 6765 2062 6574 7765 656e 3a0a 0a2a 2043  ge between:..* C
-0000d760: 7265 6174 696e 6720 6120 5669 6577 204d  reating a View M
-0000d770: 6f64 656c 0a2a 2053 6861 7269 6e67 2074  odel.* Sharing t
-0000d780: 6865 2073 616d 6520 7461 626c 6520 6265  he same table be
-0000d790: 7477 6565 6e20 6d6f 7265 2074 6861 6e20  tween more than 
-0000d7a0: 6f6e 6520 6d6f 6465 6c2e 0a0a 2e2e 2077  one model..... w
-0000d7b0: 6172 6e69 6e67 3a3a 0a0a 2020 2020 466f  arning::..    Fo
-0000d7c0: 7220 7468 6520 7669 6577 2079 6f75 206d  r the view you m
-0000d7d0: 7573 7420 7265 6469 6e65 6420 7468 6520  ust redined the 
-0000d7e0: 636f 6c75 6d6e 2069 6e20 7468 6520 4d6f  column in the Mo
-0000d7f0: 6465 6c20 636f 7272 6573 706f 6e64 696e  del correspondin
-0000d800: 6720 746f 2074 6865 2076 6965 770a 2020  g to the view.  
-0000d810: 2020 7769 7468 2069 6e68 6572 6974 616e    with inheritan
-0000d820: 6365 206f 7220 7369 6d70 6c65 2053 6861  ce or simple Sha
-0000d830: 7265 2062 7920 7461 626c 656e 616d 650a  re by tablename.
-0000d840: 0a53 7065 6369 6669 6320 6265 6861 7669  .Specific behavi
-0000d850: 6f75 720a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  our.------------
-0000d860: 2d2d 2d2d 2d2d 0a0a 416e 7942 6c6f 6b20  ------..AnyBlok 
-0000d870: 696d 706c 656d 656e 7473 2073 6f6d 6520  implements some 
-0000d880: 6661 6369 6c69 7469 6573 2074 6f20 6865  facilities to he
-0000d890: 6c70 2064 6576 656c 6f70 6572 730a 0a43  lp developers..C
-0000d8a0: 6f6c 756d 6e20 656e 6372 7970 7469 6f6e  olumn encryption
-0000d8b0: 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  .~~~~~~~~~~~~~~~
-0000d8c0: 7e7e 0a0a 596f 7520 6361 6e20 656e 6372  ~~..You can encr
-0000d8d0: 7970 7420 736f 6d65 2063 6f6c 756d 6e73  ypt some columns
-0000d8e0: 2074 6f20 7072 6f74 6563 7420 7468 656d   to protect them
-0000d8f0: 2e20 5468 6520 7079 7468 6f6e 2070 6163  . The python pac
-0000d900: 6b61 6765 2063 7279 7074 6f67 7261 7068  kage cryptograph
-0000d910: 790a 6d75 7374 2062 6520 696e 7374 616c  y.must be instal
-0000d920: 6c65 643a 3a0a 0a20 2020 2070 6970 2069  led::..    pip i
-0000d930: 6e73 7461 6c6c 2063 7279 7074 6f67 7261  nstall cryptogra
-0000d940: 7068 790a 0a55 7365 2074 6865 2065 6e63  phy..Use the enc
-0000d950: 7279 7074 5f6b 6579 2061 7474 7269 6275  rypt_key attribu
-0000d960: 7465 206f 6e20 7468 6520 636f 6c75 6d6e  te on the column
-0000d970: 2074 6f20 6465 6669 6e65 2074 6865 206b   to define the k
-0000d980: 6579 206f 6620 6372 7970 746f 6772 6170  ey of cryptograp
-0000d990: 6879 3a3a 0a0a 2020 2020 4072 6567 6973  hy::..    @regis
-0000d9a0: 7465 7228 4d6f 6465 6c29 0a20 2020 2063  ter(Model).    c
-0000d9b0: 6c61 7373 204d 794d 6f64 656c 3a0a 0a20  lass MyModel:.. 
-0000d9c0: 2020 2020 2020 2023 2064 6566 696e 6520         # define 
-0000d9d0: 7468 6520 7370 6563 6966 6963 2065 6e63  the specific enc
-0000d9e0: 7279 7074 5f6b 6579 0a20 2020 2020 2020  rypt_key.       
-0000d9f0: 2065 6e63 7279 7074 5f63 6f6c 756d 6e5f   encrypt_column_
-0000da00: 3120 3d20 5374 7269 6e67 2865 6e63 7279  1 = String(encry
-0000da10: 7074 5f6b 6579 3d27 5365 6372 6574 4b65  pt_key='SecretKe
-0000da20: 7927 290a 0a20 2020 2020 2020 2023 2055  y')..        # U
-0000da30: 7365 2074 6865 2064 6566 6175 6c74 2065  se the default e
-0000da40: 6e63 7279 7074 5f6b 6579 0a20 2020 2020  ncrypt_key.     
-0000da50: 2020 2065 6e63 7279 7074 5f63 6f6c 756d     encrypt_colum
-0000da60: 6e5f 3220 3d20 5374 7269 6e67 2865 6e63  n_2 = String(enc
-0000da70: 7279 7074 5f6b 6579 3d43 6f6e 6669 6775  rypt_key=Configu
-0000da80: 7261 7469 6f6e 2e67 6574 2827 6465 6661  ration.get('defa
-0000da90: 756c 745f 656e 6372 7970 745f 6b65 7927  ult_encrypt_key'
-0000daa0: 290a 2020 2020 2020 2020 656e 6372 7970  ).        encryp
-0000dab0: 745f 636f 6c75 6d6e 5f33 203d 2053 7472  t_column_3 = Str
-0000dac0: 696e 6728 656e 6372 7970 745f 6b65 793d  ing(encrypt_key=
-0000dad0: 5472 7565 290a 0a20 2020 2020 2020 2023  True)..        #
-0000dae0: 2055 7365 2074 6865 2063 6c61 7373 206d   Use the class m
-0000daf0: 6574 686f 6420 746f 2067 6574 2065 6e63  ethod to get enc
-0000db00: 7279 7074 5f6b 6579 0a20 2020 2020 2020  rypt_key.       
-0000db10: 2065 6e63 7279 7074 5f63 6f6c 756d 6e5f   encrypt_column_
-0000db20: 3120 3d20 5374 7269 6e67 2865 6e63 7279  1 = String(encry
-0000db30: 7074 5f6b 6579 3d27 6765 745f 656e 6372  pt_key='get_encr
-0000db40: 7970 745f 6b65 7927 290a 0a20 2020 2020  ypt_key')..     
-0000db50: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-0000db60: 2020 2020 2020 2020 6465 6620 6765 745f          def get_
-0000db70: 656e 6372 7970 745f 6b65 7928 636c 7329  encrypt_key(cls)
-0000db80: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000db90: 7475 726e 2027 5365 6372 6574 4b65 7927  turn 'SecretKey'
-0000dba0: 0a0a 5468 6520 656e 6372 7970 7469 6f6e  ..The encryption
-0000dbb0: 2077 6f72 6b73 2066 6f72 2061 6e79 2043   works for any C
-0000dbc0: 6f6c 756d 6e73 2e0a 0a45 6e76 6972 6f6e  olumns...Environ
-0000dbd0: 6d65 6e74 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  ment.~~~~~~~~~~~
-0000dbe0: 0a0a 5468 6520 456e 7669 726f 6e6d 656e  ..The Environmen
-0000dbf0: 7420 636f 6e74 6169 6e73 206e 6f6e 2070  t contains non p
-0000dc00: 6572 7369 7374 656e 7420 636f 6e74 6578  ersistent contex
-0000dc10: 7475 616c 2076 6172 6961 626c 6573 2e20  tual variables. 
-0000dc20: 4279 0a64 6566 6175 6c74 2c20 6974 2069  By.default, it i
-0000dc30: 7320 7374 6f72 6564 2069 6e20 7468 6520  s stored in the 
-0000dc40: 6375 7272 656e 7420 3a63 6c61 7373 3a60  current :class:`
-0000dc50: 5468 7265 6164 6020 6f62 6a65 6374 2c20  Thread` object, 
-0000dc60: 6275 7420 7468 6174 0a69 7320 616d 656e  but that.is amen
-0000dc70: 6461 626c 6520 2873 6565 203a 7265 663a  dable (see :ref:
-0000dc80: 6065 6e76 6972 6f6e 6d65 6e74 5f74 7970  `environment_typ
-0000dc90: 6573 6029 2e0a 0a55 7365 2074 6865 2063  es`)...Use the c
-0000dca0: 7572 7265 6e74 2065 6e76 6972 6f6e 6d65  urrent environme
-0000dcb0: 6e74 0a2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b  nt.+++++++++++++
-0000dcc0: 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 0a0a  ++++++++++++++..
-0000dcd0: 5468 6520 656e 7669 726f 6e6d 656e 7420  The environment 
-0000dce0: 6361 6e20 6265 2075 7365 6420 6672 6f6d  can be used from
-0000dcf0: 2077 6865 7265 6576 6572 2069 6e20 7468   whereever in th
-0000dd00: 6520 636f 6465 2e0a 0a47 656e 6572 6963  e code...Generic
-0000dd10: 2075 7365 0a2f 2f2f 2f2f 2f2f 2f2f 2f2f   use.///////////
-0000dd20: 0a0a 546f 2067 6574 206f 7220 7365 7420  ..To get or set 
-0000dd30: 7661 7269 6162 6c65 2069 6e20 656e 7669  variable in envi
-0000dd40: 726f 6e6d 656e 742c 2079 6f75 206d 7573  ronment, you mus
-0000dd50: 7420 696d 706f 7274 2074 6865 0a60 6045  t import the.``E
-0000dd60: 6e76 6972 6f6e 6d65 6e74 4d61 6e61 6765  nvironmentManage
-0000dd70: 7260 603a 3a0a 0a20 2020 2066 726f 6d20  r``::..    from 
-0000dd80: 616e 7962 6c6f 6b2e 656e 7669 726f 6e6d  anyblok.environm
-0000dd90: 656e 7420 696d 706f 7274 2045 6e76 6972  ent import Envir
-0000dda0: 6f6e 6d65 6e74 4d61 6e61 6765 720a 0a53  onmentManager..S
-0000ddb0: 6574 2061 2076 6172 6961 626c 653a 3a0a  et a variable::.
-0000ddc0: 0a20 2020 2045 6e76 6972 6f6e 6d65 6e74  .    Environment
-0000ddd0: 4d61 6e61 6765 722e 7365 7428 276d 7920  Manager.set('my 
-0000dde0: 7661 7269 6162 6c65 206e 616d 6527 2c20  variable name', 
-0000ddf0: 736f 6d65 5f76 616c 7565 290a 0a47 6574  some_value)..Get
-0000de00: 2061 2076 6172 6961 626c 653a 3a0a 0a20   a variable::.. 
-0000de10: 2020 2045 6e76 6972 6f6e 6d65 6e74 4d61     EnvironmentMa
-0000de20: 6e61 6765 722e 6765 7428 276d 7920 7661  nager.get('my va
-0000de30: 7269 6162 6c65 206e 616d 6527 2c20 6465  riable name', de
-0000de40: 6661 756c 743d 736f 6d65 5f64 6566 6175  fault=some_defau
-0000de50: 6c74 290a 0a55 7365 2066 726f 6d20 6120  lt)..Use from a 
-0000de60: 6060 4d6f 6465 6c60 600a 2f2f 2f2f 2f2f  ``Model``.//////
-0000de70: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 0a0a  //////////////..
-0000de80: 4120 636c 6173 732d 6c65 7665 6c20 6174  A class-level at
-0000de90: 7472 6962 7574 6520 6973 2070 7265 7365  tribute is prese
-0000dea0: 6e74 206f 6e20 616c 6c20 4d6f 6465 6c20  nt on all Model 
-0000deb0: 636c 6173 7365 7320 746f 2061 6363 6573  classes to acces
-0000dec0: 7320 7468 650a 456e 7669 726f 6e6d 656e  s the.Environmen
-0000ded0: 7420 7661 7269 6162 6c65 7320 636f 6e76  t variables conv
-0000dee0: 656e 6965 6e74 6c79 2e0a 0a54 6f20 6772  eniently...To gr
-0000def0: 6162 2074 6865 2045 6e76 6972 6f6e 6d65  ab the Environme
-0000df00: 6e74 4d61 6e61 6765 7220 6672 6f6d 2061  ntManager from a
-0000df10: 2060 604d 6f64 656c 6060 206d 6574 686f   ``Model`` metho
-0000df20: 642c 206a 7573 7420 7573 650a 6060 7365  d, just use.``se
-0000df30: 6c66 2e45 6e76 6060 2e20 466f 7220 6120  lf.Env``. For a 
-0000df40: 636c 6173 736d 6574 686f 642c 2074 6861  classmethod, tha
-0000df50: 7420 776f 756c 6420 6265 2061 7320 696e  t would be as in
-0000df60: 3a3a 0a0a 2020 2020 4063 6c61 7373 6d65  ::..    @classme
-0000df70: 7468 6f64 0a20 2020 2064 6566 206d 7963  thod.    def myc
-0000df80: 6c73 6d65 7468 2863 6c73 293a 0a20 2020  lsmeth(cls):.   
-0000df90: 2020 2065 6e76 203d 2063 6c73 2e45 6e76     env = cls.Env
-0000dfa0: 0a20 2020 2020 2028 2e2e 2e29 0a0a 5468  .      (...)..Th
-0000dfb0: 656e 2c20 6974 2773 2065 6173 7920 746f  en, it's easy to
-0000dfc0: 2067 6574 2061 6e64 2073 6574 2076 6172   get and set var
-0000dfd0: 6961 626c 6573 2e20 4865 7265 2773 2061  iables. Here's a
-0000dfe0: 6e20 6578 616d 706c 6520 6672 6f6d 2061  n example from a
-0000dff0: 204d 6f64 656c 0a69 6e73 7461 6e63 6520   Model.instance 
-0000e000: 6d65 7468 6f64 3a3a 0a0a 2020 2020 7365  method::..    se
-0000e010: 6c66 2e45 6e76 2e73 6574 2827 6d79 2076  lf.Env.set('my v
-0000e020: 6172 6961 626c 6520 6e61 6d65 272c 2073  ariable name', s
-0000e030: 6f6d 655f 7661 6c75 6529 0a20 2020 2073  ome_value).    s
-0000e040: 656c 662e 456e 762e 6765 7428 276d 7920  elf.Env.get('my 
-0000e050: 7661 7269 6162 6c65 206e 616d 6527 2c20  variable name', 
-0000e060: 6465 6661 756c 743d 736f 6d65 5f64 6566  default=some_def
-0000e070: 6175 6c74 5f76 616c 7565 290a 0a2e 2e20  ault_value).... 
-0000e080: 6e6f 7465 3a3a 2074 6865 2060 6045 6e76  note:: the ``Env
-0000e090: 6060 2061 7474 7269 6275 7465 2069 7320  `` attribute is 
-0000e0a0: 6163 7475 616c 6c79 2073 6574 2069 6e0a  actually set in.
-0000e0b0: 2020 2020 2020 2020 2020 6060 7265 6769            ``regi
-0000e0c0: 7374 7279 2e72 6567 6973 7472 795f 6261  stry.registry_ba
-0000e0d0: 7365 6060 2c20 7768 6963 6820 6973 2061  se``, which is a
-0000e0e0: 2063 6c61 7373 2064 796e 616d 6963 616c   class dynamical
-0000e0f0: 6c79 0a20 2020 2020 2020 2020 2067 656e  ly.          gen
-0000e100: 6572 6174 6564 2061 7420 7265 6769 7374  erated at regist
-0000e110: 7279 2063 7265 6174 696f 6e2c 2061 6e64  ry creation, and
-0000e120: 206f 6620 7768 6963 6820 616c 6c20 6173   of which all as
-0000e130: 7365 6d62 6c65 640a 2020 2020 2020 2020  sembled.        
-0000e140: 2020 636c 6173 7365 7320 7374 6f72 6564    classes stored
-0000e150: 2069 6e20 7468 6520 7265 6769 7374 7279   in the registry
-0000e160: 2069 6e68 6572 6974 2e0a 0a2e 2e20 5f65   inherit..... _e
-0000e170: 6e76 6972 6f6e 6d65 6e74 5f74 7970 6573  nvironment_types
-0000e180: 3a0a 0a44 6566 696e 6520 6120 6e65 7720  :..Define a new 
-0000e190: 656e 7669 726f 6e6d 656e 7420 7479 7065  environment type
-0000e1a0: 0a2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b  .+++++++++++++++
-0000e1b0: 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 0a0a  ++++++++++++++..
-0000e1c0: 4966 2079 6f75 2064 6f20 6e6f 7420 7761  If you do not wa
-0000e1d0: 6e74 2074 6f20 7374 6f63 6b20 7468 6520  nt to stock the 
-0000e1e0: 656e 7669 726f 6e6d 656e 7420 696e 2074  environment in t
-0000e1f0: 6865 2060 6054 6872 6561 6460 602c 2079  he ``Thread``, y
-0000e200: 6f75 2020 6d75 7374 0a69 6d70 6c65 6d65  ou  must.impleme
-0000e210: 6e74 2061 206e 6577 2074 7970 6520 6f66  nt a new type of
-0000e220: 2065 6e76 6972 6f6e 6d65 6e74 2e0a 0a54   environment...T
-0000e230: 6869 7320 7479 7065 2069 7320 6120 7369  his type is a si
-0000e240: 6d70 6c65 2063 6c61 7373 2077 6869 6368  mple class which
-0000e250: 2068 6176 6520 7468 6573 6573 2063 6c61   have theses cla
-0000e260: 7373 206d 6574 686f 6473 3a0a 0a2a 2073  ss methods:..* s
-0000e270: 636f 7065 645f 6675 6e63 7469 6f6e 5f66  coped_function_f
-0000e280: 6f72 5f73 6573 7369 6f6e 0a2a 2073 6574  or_session.* set
-0000e290: 7465 720a 2a20 6765 7474 6572 0a0a 3a3a  ter.* getter..::
-0000e2a0: 0a0a 2020 2020 4d79 456e 7669 726f 6e6d  ..    MyEnvironm
-0000e2b0: 656e 7443 6c61 7373 3a0a 0a20 2020 2020  entClass:..     
-0000e2c0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-0000e2d0: 2020 2020 2020 2020 6465 6620 7363 6f70          def scop
-0000e2e0: 6564 5f66 756e 6374 696f 6e5f 666f 725f  ed_function_for_
-0000e2f0: 7365 7373 696f 6e28 636c 7329 3a0a 2020  session(cls):.  
-0000e300: 2020 2020 2020 2020 2020 2e2e 2e0a 0a20            ..... 
-0000e310: 2020 2020 2020 2040 636c 6173 736d 6574         @classmet
-0000e320: 686f 640a 2020 2020 2020 2020 6465 6620  hod.        def 
-0000e330: 7365 7474 6572 2863 6c73 2c20 6b65 792c  setter(cls, key,
-0000e340: 2076 616c 7565 293a 0a20 2020 2020 2020   value):.       
-0000e350: 2020 2020 202e 2e2e 0a0a 2020 2020 2020       .....      
-0000e360: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-0000e370: 2020 2020 2020 2064 6566 2067 6574 7465         def gette
-0000e380: 7228 636c 732c 206b 6579 2c20 6465 6661  r(cls, key, defa
-0000e390: 756c 7429 3a0a 2020 2020 2020 2020 2020  ult):.          
-0000e3a0: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
-0000e3b0: 2020 7265 7475 726e 2076 616c 7565 0a0a    return value..
-0000e3c0: 4465 636c 6172 6520 796f 7572 2063 6c61  Declare your cla
-0000e3d0: 7373 2061 7320 7468 6520 456e 7669 726f  ss as the Enviro
-0000e3e0: 6e6d 656e 7420 636c 6173 733a 3a0a 0a20  nment class::.. 
-0000e3f0: 2020 2045 6e76 6972 6f6e 6d65 6e74 4d61     EnvironmentMa
-0000e400: 6e61 6765 722e 6465 6669 6e65 5f65 6e76  nager.define_env
-0000e410: 6972 6f6e 6d65 6e74 5f63 6c73 284d 7945  ironment_cls(MyE
-0000e420: 6e76 6972 6f6e 6d65 6e74 436c 6173 7329  nvironmentClass)
-0000e430: 0a0a 0a54 6865 2063 6c61 7373 6d65 7468  ...The classmeth
-0000e440: 6f64 2060 6073 636f 7065 645f 6675 6e63  od ``scoped_func
-0000e450: 7469 6f6e 5f66 6f72 5f73 6573 7369 6f6e  tion_for_session
-0000e460: 6060 2069 7320 7061 7373 6564 2061 7420  `` is passed at 
-0000e470: 5351 4c41 6c63 6865 6d79 0a60 6073 636f  SQLAlchemy.``sco
-0000e480: 7065 645f 7365 7373 696f 6e60 6020 6675  ped_session`` fu
-0000e490: 6e63 7469 6f6e 2060 7365 6520 3c68 7474  nction `see <htt
-0000e4a0: 703a 2f2f 646f 6373 2e73 716c 616c 6368  p://docs.sqlalch
-0000e4b0: 656d 792e 6f72 672f 656e 2f72 656c 5f30  emy.org/en/rel_0
-0000e4c0: 5f39 2f6f 726d 2f0a 636f 6e74 6578 7475  _9/orm/.contextu
-0000e4d0: 616c 2e68 746d 6c23 636f 6e74 6578 7475  al.html#contextu
-0000e4e0: 616c 2d74 6872 6561 642d 6c6f 6361 6c2d  al-thread-local-
-0000e4f0: 7365 7373 696f 6e73 3e60 5f0a 0a0a 4765  sessions>`_...Ge
-0000e500: 7420 7468 6520 7265 6769 7374 7279 0a7e  t the registry.~
-0000e510: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a  ~~~~~~~~~~~~~~~.
-0000e520: 0a59 6f75 2063 616e 2067 6574 2074 6865  .You can get the
-0000e530: 2072 6567 6973 7472 7920 696e 2061 6e79   registry in any
-0000e540: 206d 6574 686f 6420 6f66 204d 6f64 656c   method of Model
-0000e550: 7320 7769 7468 2074 6865 2061 7474 7269  s with the attri
-0000e560: 6275 7465 202a 2a61 6e79 626c 6f6b 2a2a  bute **anyblok**
-0000e570: 3a3a 0a0a 2020 2020 4d6f 6465 6c20 3d20  ::..    Model = 
-0000e580: 7365 6c66 2e61 6e79 626c 6f6b 2e53 7973  self.anyblok.Sys
-0000e590: 7465 6d2e 4d6f 6465 6c0a 2020 2020 6173  tem.Model.    as
-0000e5a0: 7365 7274 204d 6f64 656c 2e5f 5f72 6567  sert Model.__reg
-0000e5b0: 6973 7472 795f 6e61 6d65 5f5f 203d 3d20  istry_name__ == 
-0000e5c0: 274d 6f64 656c 2e53 7973 7465 6d2e 4d6f  'Model.System.Mo
-0000e5d0: 6465 6c27 0a0a 2e2e 2077 6172 6e69 6e67  del'.... warning
-0000e5e0: 3a3a 0a0a 2020 2053 696e 6365 2076 6572  ::..   Since ver
-0000e5f0: 7369 6f6e 2031 2e31 2e30 206f 6620 416e  sion 1.1.0 of An
-0000e600: 7942 6c6f 6b20 7468 6520 6174 7472 6962  yBlok the attrib
-0000e610: 7574 6520 2a2a 7265 6769 7374 7279 2a2a  ute **registry**
-0000e620: 2069 7320 7265 6e61 6d65 6420 2a2a 616e   is renamed **an
-0000e630: 7962 6c6f 6b2a 2a0a 0a0a 4361 6368 650a  yblok**...Cache.
-0000e640: 7e7e 7e7e 7e0a 0a54 6865 2063 6163 6865  ~~~~~..The cache
-0000e650: 2061 6c6c 6f77 7320 746f 2063 616c 6c20   allows to call 
-0000e660: 6120 6d65 7468 6f64 206d 6f72 6520 7468  a method more th
-0000e670: 616e 206f 6e63 6520 7769 7468 6f75 7420  an once without 
-0000e680: 6861 7669 6e67 2061 6e79 2064 6966 6665  having any diffe
-0000e690: 7265 6e63 650a 696e 2074 6865 2072 6573  rence.in the res
-0000e6a0: 756c 742e 2042 7574 2074 6865 2063 6163  ult. But the cac
-0000e6b0: 6865 206d 7573 7420 616c 736f 2064 6570  he must also dep
-0000e6c0: 656e 6420 6f6e 2074 6865 2072 6567 6973  end on the regis
-0000e6d0: 7472 7920 6461 7461 6261 7365 2061 6e64  try database and
-0000e6e0: 2074 6865 0a6d 6f64 656c 2e20 5468 6520   the.model. The 
-0000e6f0: 6361 6368 6520 6f66 2061 6e79 626c 6f6b  cache of anyblok
-0000e700: 2063 616e 2062 6520 7075 7420 6f6e 2061   can be put on a
-0000e710: 204d 6f64 656c 2c20 6120 436f 7265 206f   Model, a Core o
-0000e720: 7220 6120 4d69 7869 6e20 6d65 7468 6f64  r a Mixin method
-0000e730: 2e20 4966 0a74 6865 2063 6163 6865 2069  . If.the cache i
-0000e740: 7320 6f6e 2061 2043 6f72 6520 6f72 2061  s on a Core or a
-0000e750: 204d 6978 696e 2074 6865 6e20 7468 6520   Mixin then the 
-0000e760: 7573 6563 6173 6520 6465 7065 6e64 7320  usecase depends 
-0000e770: 6f6e 2074 6865 2072 6567 6973 7472 7920  on the registry 
-0000e780: 6e61 6d65 0a6f 6620 7468 6520 6173 7365  name.of the asse
-0000e790: 6d62 6c65 6420 6d6f 6465 6c2e 0a0a 5573  mbled model...Us
-0000e7a0: 6520 6060 6361 6368 6560 6020 6f72 2060  e ``cache`` or `
-0000e7b0: 6063 6c61 7373 6d65 7468 6f64 5f63 6163  `classmethod_cac
-0000e7c0: 6865 6060 2074 6f20 6170 706c 7920 6120  he`` to apply a 
-0000e7d0: 6361 6368 6520 6f6e 2061 206d 6574 686f  cache on a metho
-0000e7e0: 643a 3a0a 0a20 2020 2066 726f 6d20 616e  d::..    from an
-0000e7f0: 7962 6c6f 6b2e 6465 636c 6172 6174 696f  yblok.declaratio
-0000e800: 6e73 2069 6d70 6f72 7420 6361 6368 652c  ns import cache,
-0000e810: 2063 6c61 7373 6d65 7468 6f64 5f63 6163   classmethod_cac
-0000e820: 6865 0a0a 2e2e 2077 6172 6e69 6e67 3a3a  he.... warning::
-0000e830: 0a0a 2020 2020 6060 6361 6368 6560 6020  ..    ``cache`` 
-0000e840: 6465 7065 6e64 206f 6620 7468 6520 696e  depend of the in
-0000e850: 7374 616e 6365 2c20 6966 2079 6f75 2077  stance, if you w
-0000e860: 616e 7420 6164 6420 6120 6361 6368 6520  ant add a cache 
-0000e870: 666f 720a 2020 2020 616e 7920 696e 7374  for.    any inst
-0000e880: 616e 6365 2079 6f75 206d 7573 7420 7573  ance you must us
-0000e890: 6520 6060 636c 6173 736d 6574 686f 645f  e ``classmethod_
-0000e8a0: 6361 6368 6560 600a 0a43 6163 6865 2074  cache``..Cache t
-0000e8b0: 6865 206d 6574 686f 6420 6f66 2061 204d  he method of a M
-0000e8c0: 6f64 656c 3a3a 0a0a 2020 2020 4072 6567  odel::..    @reg
-0000e8d0: 6973 7465 7228 4d6f 6465 6c29 0a20 2020  ister(Model).   
-0000e8e0: 2063 6c61 7373 2046 6f6f 3a0a 0a20 2020   class Foo:..   
-0000e8f0: 2020 2020 2040 636c 6173 736d 6574 686f       @classmetho
-0000e900: 645f 6361 6368 6528 290a 2020 2020 2020  d_cache().      
-0000e910: 2020 6465 6620 6261 7228 636c 7329 3a0a    def bar(cls):.
-0000e920: 2020 2020 2020 2020 2020 2020 696d 706f              impo
-0000e930: 7274 2072 616e 646f 6d0a 2020 2020 2020  rt random.      
-0000e940: 2020 2020 2020 7265 7475 726e 2072 616e        return ran
-0000e950: 646f 6d2e 7261 6e64 6f6d 2829 0a0a 0a20  dom.random()... 
-0000e960: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-0000e970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000e980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2020  ------------..  
-0000e990: 2020 6173 7365 7274 2046 6f6f 2e62 6172    assert Foo.bar
-0000e9a0: 2829 203d 3d20 466f 6f2e 6261 7228 290a  () == Foo.bar().
-0000e9b0: 0a0a 4361 6368 6520 7468 6520 6d65 7468  ..Cache the meth
-0000e9c0: 6f64 2063 6f6d 696e 6720 6672 6f6d 2061  od coming from a
-0000e9d0: 204d 6978 696e 3a3a 0a0a 2020 2020 4072   Mixin::..    @r
-0000e9e0: 6567 6973 7465 7228 4d69 7869 6e29 0a20  egister(Mixin). 
-0000e9f0: 2020 2063 6c61 7373 204d 466f 6f3a 0a0a     class MFoo:..
-0000ea00: 2020 2020 2020 2020 4063 6c61 7373 6d65          @classme
-0000ea10: 7468 6f64 5f63 6163 6865 2829 0a20 2020  thod_cache().   
-0000ea20: 2020 2020 2064 6566 2062 6172 2863 6c73       def bar(cls
-0000ea30: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-0000ea40: 6d70 6f72 7420 7261 6e64 6f6d 0a20 2020  mport random.   
-0000ea50: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000ea60: 7261 6e64 6f6d 2e72 616e 646f 6d28 290a  random.random().
-0000ea70: 0a20 2020 2040 7265 6769 7374 6572 284d  .    @register(M
-0000ea80: 6f64 656c 290a 2020 2020 636c 6173 7320  odel).    class 
-0000ea90: 466f 6f28 4d69 7869 6e2e 4d46 6f6f 293a  Foo(Mixin.MFoo):
-0000eaa0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-0000eab0: 2020 2040 7265 6769 7374 6572 284d 6f64     @register(Mod
-0000eac0: 656c 290a 2020 2020 636c 6173 7320 466f  el).    class Fo
-0000ead0: 6f32 284d 6978 696e 2e4d 466f 6f29 3a0a  o2(Mixin.MFoo):.
-0000eae0: 2020 2020 2020 2020 7061 7373 0a0a 0a20          pass... 
-0000eaf0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-0000eb00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000eb10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2020  ------------..  
-0000eb20: 2020 6173 7365 7274 2046 6f6f 2e62 6172    assert Foo.bar
-0000eb30: 2829 203d 3d20 466f 6f2e 6261 7228 290a  () == Foo.bar().
-0000eb40: 2020 2020 6173 7365 7274 2046 6f6f 322e      assert Foo2.
-0000eb50: 6261 7228 2920 3d3d 2046 6f6f 322e 6261  bar() == Foo2.ba
-0000eb60: 7228 290a 2020 2020 6173 7365 7274 2046  r().    assert F
-0000eb70: 6f6f 2e62 6172 2829 2021 3d20 466f 6f32  oo.bar() != Foo2
-0000eb80: 2e62 6172 2829 0a0a 0a43 6163 6865 2074  .bar()...Cache t
-0000eb90: 6865 206d 6574 686f 6420 636f 6d69 6e67  he method coming
-0000eba0: 2066 726f 6d20 6120 4d69 7869 6e3a 3a0a   from a Mixin::.
-0000ebb0: 0a20 2020 2040 7265 6769 7374 6572 2843  .    @register(C
-0000ebc0: 6f72 6529 0a20 2020 2063 6c61 7373 2042  ore).    class B
-0000ebd0: 6173 650a 0a20 2020 2020 2020 2040 636c  ase..        @cl
-0000ebe0: 6173 736d 6574 686f 645f 6361 6368 6528  assmethod_cache(
-0000ebf0: 290a 2020 2020 2020 2020 6465 6620 6261  ).        def ba
-0000ec00: 7228 636c 7329 3a0a 2020 2020 2020 2020  r(cls):.        
-0000ec10: 2020 2020 696d 706f 7274 2072 616e 646f      import rando
-0000ec20: 6d0a 2020 2020 2020 2020 2020 2020 7265  m.            re
-0000ec30: 7475 726e 2072 616e 646f 6d2e 7261 6e64  turn random.rand
-0000ec40: 6f6d 2829 0a0a 2020 2020 4072 6567 6973  om()..    @regis
-0000ec50: 7465 7228 4d6f 6465 6c29 0a20 2020 2063  ter(Model).    c
-0000ec60: 6c61 7373 2046 6f6f 3a0a 2020 2020 2020  lass Foo:.      
-0000ec70: 2020 7061 7373 0a0a 2020 2020 4072 6567    pass..    @reg
-0000ec80: 6973 7465 7228 4d6f 6465 6c29 0a20 2020  ister(Model).   
-0000ec90: 2063 6c61 7373 2046 6f6f 323a 0a20 2020   class Foo2:.   
-0000eca0: 2020 2020 2070 6173 730a 0a0a 2020 2020       pass...    
-0000ecb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ecc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ecd0: 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020 2061  ---------..    a
-0000ece0: 7373 6572 7420 466f 6f2e 6261 7228 2920  ssert Foo.bar() 
-0000ecf0: 3d3d 2046 6f6f 2e62 6172 2829 0a20 2020  == Foo.bar().   
-0000ed00: 2061 7373 6572 7420 466f 6f32 2e62 6172   assert Foo2.bar
-0000ed10: 2829 203d 3d20 466f 6f32 2e62 6172 2829  () == Foo2.bar()
-0000ed20: 0a20 2020 2061 7373 6572 7420 466f 6f2e  .    assert Foo.
-0000ed30: 6261 7228 2920 213d 2046 6f6f 322e 6261  bar() != Foo2.ba
-0000ed40: 7228 290a 0a45 7665 6e74 0a7e 7e7e 7e7e  r()..Event.~~~~~
-0000ed50: 0a0a 5369 6d70 6c65 2069 6d70 6c65 6d65  ..Simple impleme
-0000ed60: 6e74 6174 696f 6e20 6f66 2061 2073 796e  ntation of a syn
-0000ed70: 6368 726f 6e6f 7573 2060 6065 7665 6e74  chronous ``event
-0000ed80: 6060 2066 6f72 2041 6e79 426c 6f6b 206f  `` for AnyBlok o
-0000ed90: 7220 5351 4c41 6c63 6865 6d79 3a3a 0a0a  r SQLAlchemy::..
-0000eda0: 0a20 2020 2040 7265 6769 7374 6572 284d  .    @register(M
-0000edb0: 6f64 656c 290a 2020 2020 636c 6173 7320  odel).    class 
-0000edc0: 4576 656e 743a 0a20 2020 2020 2020 2070  Event:.        p
-0000edd0: 6173 730a 0a20 2020 2040 7265 6769 7374  ass..    @regist
-0000ede0: 6572 284d 6f64 656c 290a 2020 2020 636c  er(Model).    cl
-0000edf0: 6173 7320 5465 7374 3a0a 0a20 2020 2020  ass Test:..     
-0000ee00: 2020 2020 2020 2078 203d 2030 0a0a 2020         x = 0..  
-0000ee10: 2020 2020 2020 2020 2020 406c 6973 7465            @liste
-0000ee20: 6e28 4d6f 6465 6c2e 4576 656e 742c 2027  n(Model.Event, '
-0000ee30: 6669 7265 6576 656e 7427 290a 2020 2020  fireevent').    
-0000ee40: 2020 2020 2020 2020 6465 6620 6d79 5f65          def my_e
-0000ee50: 7665 6e74 2863 6c73 2c20 613d 312c 2062  vent(cls, a=1, b
-0000ee60: 3d31 293a 0a20 2020 2020 2020 2020 2020  =1):.           
-0000ee70: 2020 2020 2063 6c73 2e78 203d 2061 202a       cls.x = a *
-0000ee80: 2062 0a0a 2020 2020 2d2d 2d2d 2d2d 2d2d   b..    --------
-0000ee90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000eea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000eeb0: 2d2d 2d2d 2d0a 0a20 2020 2072 6567 6973  -----..    regis
-0000eec0: 7472 792e 4576 656e 742e 6669 7265 2827  try.Event.fire('
-0000eed0: 6669 7265 6576 656e 7427 2c20 613d 3229  fireevent', a=2)
-0000eee0: 0a20 2020 2061 7373 6572 7420 7265 6769  .    assert regi
-0000eef0: 7374 7279 2e54 6573 742e 7820 3d3d 2032  stry.Test.x == 2
-0000ef00: 0a0a 2e2e 206e 6f74 653a 3a0a 0a20 2020  .... note::..   
-0000ef10: 2054 6865 2064 6563 6f72 6174 6564 206d   The decorated m
-0000ef20: 6574 686f 6420 6973 2073 6565 6e20 6173  ethod is seen as
-0000ef30: 2061 2063 6c61 7373 6d65 7468 6f64 0a0a   a classmethod..
-0000ef40: 5468 6973 2041 5049 2067 6976 6573 3a0a  This API gives:.
-0000ef50: 0a2a 2061 2064 6563 6f72 6174 6f72 2060  .* a decorator `
-0000ef60: 606c 6973 7465 6e60 6020 7768 6963 6820  `listen`` which 
-0000ef70: 6269 6e64 7320 7468 6520 6465 636f 7261  binds the decora
-0000ef80: 7465 6420 6d65 7468 6f64 2074 6f20 7468  ted method to th
-0000ef90: 6520 6576 656e 742e 0a2a 2060 6066 6972  e event..* ``fir
-0000efa0: 6560 6020 6d65 7468 6f64 2077 6974 6820  e`` method with 
-0000efb0: 7468 6520 666f 6c6c 6f77 696e 6720 7061  the following pa
-0000efc0: 7261 6d65 7465 7273 2028 4f6e 6c79 2066  rameters (Only f
-0000efd0: 6f72 2041 6e79 426c 6f6b 2065 7665 6e74  or AnyBlok event
-0000efe0: 293a 0a20 2020 202d 2060 6065 7665 6e74  ):.    - ``event
-0000eff0: 6060 3a20 7374 7269 6e67 206e 616d 6520  ``: string name 
-0000f000: 6f66 2074 6865 2065 7665 6e74 0a20 2020  of the event.   
-0000f010: 202d 2060 602a 6172 6773 6060 3a20 706f   - ``*args``: po
-0000f020: 7369 7469 6f6e 6e61 6c20 6172 6775 6d65  sitionnal argume
-0000f030: 6e74 7320 746f 2070 6173 7320 6174 7420  nts to pass att 
-0000f040: 7468 6520 6465 636f 7261 7465 6420 6d65  the decorated me
-0000f050: 7468 6f64 0a20 2020 202d 2060 602a 2a6b  thod.    - ``**k
-0000f060: 7761 7267 7360 603a 206e 616d 6564 2061  wargs``: named a
-0000f070: 7267 756d 656e 7420 746f 2070 6173 7320  rgument to pass 
-0000f080: 6174 2074 6865 2064 6563 6f72 6174 6564  at the decorated
-0000f090: 206d 6574 686f 640a 0a49 7420 6973 2070   method..It is p
-0000f0a0: 6f73 7369 626c 6520 746f 206f 7665 726c  ossible to overl
-0000f0b0: 6f61 6420 616e 2065 7869 7374 696e 6720  oad an existing 
-0000f0c0: 6576 656e 7420 6c69 7374 656e 6572 2c20  event listener, 
-0000f0d0: 6a75 7374 2062 7920 6f76 6572 6c6f 6164  just by overload
-0000f0e0: 696e 6720 7468 650a 6465 636f 7261 7465  ing the.decorate
-0000f0f0: 6420 6d65 7468 6f64 3a3a 0a0a 2020 2020  d method::..    
-0000f100: 4072 6567 6973 7465 7228 4d6f 6465 6c29  @register(Model)
-0000f110: 0a20 2020 2063 6c61 7373 2054 6573 743a  .    class Test:
-0000f120: 0a0a 2020 2020 2020 2020 4063 6c61 7373  ..        @class
-0000f130: 6d65 7468 6f64 0a20 2020 2020 2020 2064  method.        d
-0000f140: 6566 206d 795f 6576 656e 7428 636c 732c  ef my_event(cls,
-0000f150: 202a 2a6b 7761 7267 293a 0a20 2020 2020   **kwarg):.     
-0000f160: 2020 2020 2020 2072 6573 203d 2073 7570         res = sup
-0000f170: 6572 2854 6573 742c 2063 6c73 292e 6d79  er(Test, cls).my
-0000f180: 5f65 7665 6e74 282a 2a6b 7761 7267 7329  _event(**kwargs)
-0000f190: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000f1a0: 7572 6e20 7265 7320 2a20 320a 0a20 2020  urn res * 2..   
-0000f1b0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-0000f1c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000f1d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-0000f1e0: 2020 2020 7265 6769 7374 7279 2e45 7665      registry.Eve
-0000f1f0: 6e74 2e66 6972 6528 2766 6972 6565 7665  nt.fire('fireeve
-0000f200: 6e74 272c 2061 3d32 290a 2020 2020 6173  nt', a=2).    as
-0000f210: 7365 7274 2072 6567 6973 7472 792e 5465  sert registry.Te
-0000f220: 7374 2e78 203d 3d20 340a 0a2e 2e20 7761  st.x == 4.... wa
-0000f230: 726e 696e 673a 3a0a 0a20 2020 2054 6865  rning::..    The
-0000f240: 206f 7665 726c 6f61 6420 646f 6573 206e   overload does n
-0000f250: 6f74 2074 616b 6520 7468 6520 6060 6c69  ot take the ``li
-0000f260: 7374 656e 6060 2064 6563 6f72 6174 6f72  sten`` decorator
-0000f270: 2062 7574 2074 6865 0a20 2020 2063 6c61   but the.    cla
-0000f280: 7373 6d65 7468 6f64 2064 6563 6f72 6174  ssmethod decorat
-0000f290: 6f72 2c20 6265 6361 7573 6520 7468 6520  or, because the 
-0000f2a0: 6d65 7468 6f64 206e 616d 6520 6973 2061  method name is a
-0000f2b0: 6c72 6561 6479 2073 6565 6e20 6173 2061  lready seen as a
-0000f2c0: 6e0a 2020 2020 6576 656e 7420 6c69 7374  n.    event list
-0000f2d0: 656e 6572 0a0a 536f 6d65 206f 6620 7468  ener..Some of th
-0000f2e0: 6520 4174 7472 6962 7574 6520 6576 656e  e Attribute even
-0000f2f0: 7473 206f 6620 7468 6520 4d61 7070 6572  ts of the Mapper
-0000f300: 2065 7665 6e74 7320 6172 6520 696d 706c   events are impl
-0000f310: 656d 656e 7465 642e 2053 6565 2074 6865  emented. See the
-0000f320: 0a53 514c 416c 6368 656d 7920 4f52 4d20  .SQLAlchemy ORM 
-0000f330: 4576 656e 7473 2068 7474 703a 2f2f 646f  Events http://do
-0000f340: 6373 2e73 716c 616c 6368 656d 792e 6f72  cs.sqlalchemy.or
-0000f350: 672f 656e 2f6c 6174 6573 742f 6f72 6d2f  g/en/latest/orm/
-0000f360: 6576 656e 7473 2e68 746d 6c23 6f72 6d2d  events.html#orm-
-0000f370: 6576 656e 7473 0a0a 596f 7520 6d61 7920  events..You may 
-0000f380: 616c 736f 2061 6464 2061 2063 6c61 7373  also add a class
-0000f390: 6d65 7468 6f64 2077 6974 6820 7468 6520  method with the 
-0000f3a0: 6e61 6d65 2060 6065 7665 6e74 2074 7970  name ``event typ
-0000f3b0: 6520 2b20 275f 6f72 6d5f 6576 656e 7427  e + '_orm_event'
-0000f3c0: 6060 2e20 5468 6520 6576 656e 7420 7769  ``. The event wi
-0000f3d0: 6c6c 2062 6520 6175 746f 6d61 7469 636c  ll be automaticl
-0000f3e0: 790a 6372 6561 7465 2077 6974 6820 6f6e  y.create with on
-0000f3f0: 2074 6865 204d 6f64 656c 2061 6e64 2074   the Model and t
-0000f400: 6865 2065 7665 6e74 2074 7970 6520 7769  he event type wi
-0000f410: 7468 6f75 7420 6172 6775 6d65 6e74 733a  thout arguments:
-0000f420: 3a0a 0a20 2020 2040 7265 6769 7374 6572  :..    @register
-0000f430: 284d 6f64 656c 290a 2020 2020 636c 6173  (Model).    clas
-0000f440: 7320 5465 7374 3a0a 0a20 2020 2020 2020  s Test:..       
-0000f450: 2020 2020 2078 203d 2030 0a0a 2020 2020       x = 0..    
-0000f460: 2020 2020 2020 2020 4063 6c61 7373 6d65          @classme
-0000f470: 7468 6f64 0a20 2020 2020 2020 2020 2020  thod.           
-0000f480: 2064 6566 2061 6674 6572 5f69 6e73 6572   def after_inser
-0000f490: 745f 6f72 6d5f 6576 656e 7428 636c 732c  t_orm_event(cls,
-0000f4a0: 206d 6170 7065 722c 2063 6f6e 6e65 6374   mapper, connect
-0000f4b0: 696f 6e2c 2074 6172 6765 7429 3a0a 2020  ion, target):.  
-0000f4c0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000f4d0: 6361 6c6c 2077 6865 6e20 6120 6e65 7720  call when a new 
-0000f4e0: 696e 7374 616e 6365 206f 6620 5465 7374  instance of Test
-0000f4f0: 2069 7320 6164 6465 6420 696e 2074 6865   is added in the
-0000f500: 2073 6573 7369 6f6e 0a20 2020 2020 2020   session.       
-0000f510: 2020 2020 2020 2020 2070 6173 730a 0a20           pass.. 
-0000f520: 2020 2020 2020 2020 2020 2040 6c69 7374             @list
-0000f530: 656e 2827 4d6f 6465 6c2e 5465 7374 272c  en('Model.Test',
-0000f540: 2027 6166 7465 725f 696e 7365 7274 2729   'after_insert')
-0000f550: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-0000f560: 2061 6e6f 7468 6572 5f6f 726d 5f65 7665   another_orm_eve
-0000f570: 6e74 2863 6c73 2c20 6d61 7070 6572 2c20  nt(cls, mapper, 
-0000f580: 636f 6e6e 6563 7469 6f6e 2c20 7461 7267  connection, targ
-0000f590: 6574 293a 0a20 2020 2020 2020 2020 2020  et):.           
-0000f5a0: 2020 2020 2023 2069 7420 6973 2074 6865       # it is the
-0000f5b0: 2073 616d 6520 6566 6665 6374 2061 7320   same effect as 
-0000f5c0: 6060 6166 7465 725f 696e 7365 7274 5f6f  ``after_insert_o
-0000f5d0: 726d 5f65 7665 6e74 6060 2c0a 2020 2020  rm_event``,.    
-0000f5e0: 2020 2020 2020 2020 2020 2020 2320 6974              # it
-0000f5f0: 2069 7320 6361 6c6c 2061 6674 6572 2074   is call after t
-0000f600: 6865 2061 6464 206f 6620 6120 6e65 7720  he add of a new 
-0000f610: 696e 7374 616e 6365 2069 6e20 7468 6520  instance in the 
-0000f620: 7365 7373 696f 6e0a 0a0a 4879 6272 6964  session...Hybrid
-0000f630: 206d 6574 686f 640a 7e7e 7e7e 7e7e 7e7e   method.~~~~~~~~
-0000f640: 7e7e 7e7e 7e0a 0a46 6163 696c 6974 7920  ~~~~~..Facility 
-0000f650: 746f 2063 7265 6174 6520 616e 2053 514c  to create an SQL
-0000f660: 416c 6368 656d 7920 6879 6272 6964 206d  Alchemy hybrid m
-0000f670: 6574 686f 642e 2053 6565 2074 6869 7320  ethod. See this 
-0000f680: 7061 6765 3a0a 6874 7470 3a2f 2f64 6f63  page:.http://doc
-0000f690: 732e 7371 6c61 6c63 6865 6d79 2e6f 7267  s.sqlalchemy.org
-0000f6a0: 2f65 6e2f 6c61 7465 7374 2f6f 726d 2f65  /en/latest/orm/e
-0000f6b0: 7874 656e 7369 6f6e 732f 6879 6272 6964  xtensions/hybrid
-0000f6c0: 2e68 746d 6c23 6d6f 6475 6c65 2d73 716c  .html#module-sql
-0000f6d0: 616c 6368 656d 792e 6578 742e 6879 6272  alchemy.ext.hybr
-0000f6e0: 6964 0a0a 416e 7942 6c6f 6b20 616c 6c6f  id..AnyBlok allo
-0000f6f0: 7773 2074 6f20 6465 6669 6e65 2061 2068  ws to define a h
-0000f700: 7962 7269 645f 6d65 7468 6f64 2077 6869  ybrid_method whi
-0000f710: 6368 2063 616e 2062 6520 6f76 6572 6c6f  ch can be overlo
-0000f720: 6164 6564 2c20 6265 6361 7573 6520 7468  aded, because th
-0000f730: 650a 7265 616c 2073 716c 616c 6368 656d  e.real sqlalchem
-0000f740: 7920 6465 636f 7261 746f 7220 6973 2061  y decorator is a
-0000f750: 7070 6c69 6564 2061 6674 6572 2061 7373  pplied after ass
-0000f760: 656d 626c 696e 6720 696e 2074 6865 206c  embling in the l
-0000f770: 6173 7420 6f76 6572 6c6f 6164 0a6f 6620  ast overload.of 
-0000f780: 7468 6520 6465 636f 7261 7465 6420 6d65  the decorated me
-0000f790: 7468 6f64 3a3a 0a0a 2020 2020 6672 6f6d  thod::..    from
-0000f7a0: 2061 6e79 626c 6f6b 2e64 6563 6c61 7261   anyblok.declara
-0000f7b0: 7469 6f6e 7320 696d 706f 7274 2068 7962  tions import hyb
-0000f7c0: 7269 645f 6d65 7468 6f64 0a0a 2020 2020  rid_method..    
-0000f7d0: 4072 6567 6973 7465 7228 4d6f 6465 6c29  @register(Model)
-0000f7e0: 0a20 2020 2063 6c61 7373 2054 6573 743a  .    class Test:
-0000f7f0: 0a0a 2020 2020 2020 2020 4068 7962 7269  ..        @hybri
-0000f800: 645f 6d65 7468 6f64 0a20 2020 2020 2020  d_method.       
-0000f810: 2064 6566 206d 795f 6879 6272 6964 5f6d   def my_hybrid_m
-0000f820: 6574 686f 6428 7365 6c66 293a 0a20 2020  ethod(self):.   
-0000f830: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000f840: 2e2e 2e0a 0a50 7265 2d63 6f6d 6d69 7420  .....Pre-commit 
-0000f850: 686f 6f6b 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  hook.~~~~~~~~~~~
-0000f860: 7e7e 7e7e 0a0a 4974 2069 7320 706f 7373  ~~~~..It is poss
-0000f870: 6962 6c65 2074 6f20 6361 6c6c 2073 7065  ible to call spe
-0000f880: 6369 6669 6320 636c 6173 736d 6574 686f  cific classmetho
-0000f890: 6473 206a 7573 7420 6265 666f 7265 2074  ds just before t
-0000f8a0: 6865 2063 6f6d 6d69 7420 6f66 2074 6865  he commit of the
-0000f8b0: 0a73 6573 7369 6f6e 3a3a 0a0a 2020 2020  .session::..    
-0000f8c0: 4072 6567 6973 7465 7228 4d6f 6465 6c29  @register(Model)
-0000f8d0: 0a20 2020 2063 6c61 7373 2054 6573 743a  .    class Test:
-0000f8e0: 0a0a 2020 2020 2020 2020 6964 203d 2049  ..        id = I
-0000f8f0: 6e74 6567 6572 2870 7269 6d61 7279 5f6b  nteger(primary_k
-0000f900: 6579 3d54 7275 6529 0a20 2020 2020 2020  ey=True).       
-0000f910: 2076 616c 203d 2049 6e74 6567 6572 2864   val = Integer(d
-0000f920: 6566 6175 6c74 3d30 290a 0a20 2020 2020  efault=0)..     
-0000f930: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-0000f940: 2020 2020 2020 2020 6465 6620 6d65 7468          def meth
-0000f950: 6f64 3263 616c 6c5f 6a75 7374 5f62 6566  od2call_just_bef
-0000f960: 6f72 655f 7468 655f 636f 6d6d 6974 2863  ore_the_commit(c
-0000f970: 6c73 2c20 2a61 2c20 2a2a 6b77 293a 0a20  ls, *a, **kw):. 
-0000f980: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-0000f990: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-0000f9a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000f9b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000f9c0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2020 2020  ----------..    
-0000f9d0: 7265 6769 7374 7279 2e54 6573 742e 7072  registry.Test.pr
-0000f9e0: 6563 6f6d 6d69 745f 686f 6f6b 2827 6d65  ecommit_hook('me
-0000f9f0: 7468 6f64 3263 616c 6c5f 6a75 7374 5f62  thod2call_just_b
-0000fa00: 6566 6f72 655f 7468 655f 636f 6d6d 6974  efore_the_commit
-0000fa10: 272c 202a 612c 202a 2a6b 7729 0a0a 506f  ', *a, **kw)..Po
-0000fa20: 7374 2d63 6f6d 6d69 7420 686f 6f6b 0a7e  st-commit hook.~
-0000fa30: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a  ~~~~~~~~~~~~~~~.
-0000fa40: 0a49 7420 6973 2070 6f73 7369 626c 6520  .It is possible 
-0000fa50: 746f 2063 616c 6c20 7370 6563 6966 6963  to call specific
-0000fa60: 2063 6c61 7373 6d65 7468 6f64 7320 6a75   classmethods ju
-0000fa70: 7374 2061 6674 6572 2074 6865 2063 6f6d  st after the com
-0000fa80: 6d69 7420 6f66 2074 6865 0a73 6573 7369  mit of the.sessi
-0000fa90: 6f6e 3a3a 0a0a 2020 2020 4072 6567 6973  on::..    @regis
-0000faa0: 7465 7228 4d6f 6465 6c29 0a20 2020 2063  ter(Model).    c
-0000fab0: 6c61 7373 2054 6573 743a 0a0a 2020 2020  lass Test:..    
-0000fac0: 2020 2020 6964 203d 2049 6e74 6567 6572      id = Integer
-0000fad0: 2870 7269 6d61 7279 5f6b 6579 3d54 7275  (primary_key=Tru
-0000fae0: 6529 0a20 2020 2020 2020 2076 616c 203d  e).        val =
-0000faf0: 2049 6e74 6567 6572 2864 6566 6175 6c74   Integer(default
-0000fb00: 3d30 290a 0a20 2020 2020 2020 2040 636c  =0)..        @cl
-0000fb10: 6173 736d 6574 686f 640a 2020 2020 2020  assmethod.      
-0000fb20: 2020 6465 6620 6d65 7468 6f64 3263 616c    def method2cal
-0000fb30: 6c5f 6a75 7374 5f61 6674 6572 5f74 6865  l_just_after_the
-0000fb40: 5f63 6f6d 6d69 7428 636c 732c 202a 612c  _commit(cls, *a,
-0000fb50: 202a 2a6b 7729 3a0a 2020 2020 2020 2020   **kw):.        
-0000fb60: 2020 2020 7061 7373 0a0a 2020 2020 2d2d      pass..    --
-0000fb70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000fb80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000fb90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000fba0: 2d2d 2d0a 0a20 2020 2072 6567 6973 7472  ---..    registr
-0000fbb0: 792e 5465 7374 2e70 6f73 7463 6f6d 6d69  y.Test.postcommi
-0000fbc0: 745f 686f 6f6b 2827 6d65 7468 6f64 3263  t_hook('method2c
-0000fbd0: 616c 6c5f 6a75 7374 5f61 6674 6572 5f74  all_just_after_t
-0000fbe0: 6865 5f63 6f6d 6d69 7427 2c20 2a61 2c20  he_commit', *a, 
-0000fbf0: 2a2a 6b77 290a 0a0a 416c 6961 7365 640a  **kw)...Aliased.
-0000fc00: 7e7e 7e7e 7e7e 7e0a 0a46 6163 696c 6974  ~~~~~~~..Facilit
-0000fc10: 7920 746f 2063 7265 6174 6520 616e 2053  y to create an S
-0000fc20: 514c 2061 6c69 6173 2066 6f72 2074 6865  QL alias for the
-0000fc30: 2053 514c 2071 7565 7279 2062 7920 7468   SQL query by th
-0000fc40: 6520 4f52 4d3a 3a0a 0a20 2020 2073 656c  e ORM::..    sel
-0000fc50: 6563 7420 2a20 6672 6f6d 206d 795f 7461  ect * from my_ta
-0000fc60: 626c 6520 7468 655f 7461 626c 655f 616c  ble the_table_al
-0000fc70: 6961 732e 0a0a 5468 6973 2066 6163 696c  ias...This facil
-0000fc80: 6974 7920 6973 2067 6976 656e 2062 7920  ity is given by 
-0000fc90: 5351 4c41 6c63 6865 6d79 2c20 616e 6420  SQLAlchemy, and 
-0000fca0: 616e 7962 6c6f 6b20 6164 6473 2074 6869  anyblok adds thi
-0000fcb0: 7320 6675 6e63 7469 6f6e 6e61 6c69 7479  s functionnality
-0000fcc0: 0a64 6972 6563 746c 7920 696e 2074 6865  .directly in the
-0000fcd0: 204d 6f64 656c 3a3a 0a0a 2020 2020 426c   Model::..    Bl
-0000fce0: 6f6b 416c 6961 7365 6420 3d20 7265 6769  okAliased = regi
-0000fcf0: 7374 7279 2e53 7973 7465 6d2e 426c 6f6b  stry.System.Blok
-0000fd00: 2e61 6c69 6173 6564 2829 0a0a 2e2e 206e  .aliased().... n
-0000fd10: 6f74 653a 3a20 5365 6520 7468 6973 2070  ote:: See this p
-0000fd20: 6167 653a 0a20 2020 2068 7474 703a 2f2f  age:.    http://
-0000fd30: 646f 6373 2e73 716c 616c 6368 656d 792e  docs.sqlalchemy.
-0000fd40: 6f72 672f 656e 2f6c 6174 6573 742f 6f72  org/en/latest/or
-0000fd50: 6d2f 7175 6572 792e 6874 6d6c 2373 716c  m/query.html#sql
-0000fd60: 616c 6368 656d 792e 6f72 6d2e 616c 6961  alchemy.orm.alia
-0000fd70: 7365 640a 2020 2020 746f 206b 6e6f 7720  sed.    to know 
-0000fd80: 7468 6520 7061 7261 6d65 7465 7273 206f  the parameters o
-0000fd90: 6620 7468 6520 6060 616c 6961 7365 6460  f the ``aliased`
-0000fda0: 6020 6d65 7468 6f64 0a0a 2020 2020 2e2e  ` method..    ..
-0000fdb0: 2077 6172 6e69 6e67 3a3a 2054 6865 2066   warning:: The f
-0000fdc0: 6972 7374 2061 7267 2069 7320 616c 7265  irst arg is alre
-0000fdd0: 6164 7920 7061 7373 6564 2062 7920 416e  ady passed by An
-0000fde0: 7942 6c6f 6b0a 0a20 2020 202e 2e20 7761  yBlok..    .. wa
-0000fdf0: 726e 696e 673a 3a20 4f6e 6c79 2074 6869  rning:: Only thi
-0000fe00: 7320 6d65 7468 6f64 2067 6976 6520 7468  s method give th
-0000fe10: 6520 7265 6769 7374 7279 2069 6e74 6f20  e registry into 
-0000fe20: 7468 6520 616c 6961 732c 2064 6f6e 2774  the alias, don't
-0000fe30: 2069 6d70 6f72 7420 2a2a 7371 6c61 6c63   import **sqlalc
-0000fe40: 6865 6d79 2e6f 726d 2e61 6c69 6173 6564  hemy.orm.aliased
-0000fe50: 2a2a 0a0a 4765 7420 7468 6520 6375 7272  **..Get the curr
-0000fe60: 656e 7420 656e 7669 726f 6e6d 656e 740a  ent environment.
-0000fe70: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-0000fe80: 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 0a54 6865  ~~~~~~~~~~~..The
-0000fe90: 2063 7572 7265 6e74 2065 6e76 6972 6f6e   current environ
-0000fea0: 6d65 6e74 2069 7320 7361 7665 6420 696e  ment is saved in
-0000feb0: 2074 6865 206d 6169 6e20 7468 7265 6164   the main thread
-0000fec0: 2e20 596f 7520 6361 6e20 6164 6420 6120  . You can add a 
-0000fed0: 7661 6c75 6520 746f 0a74 6865 2063 7572  value to.the cur
-0000fee0: 7265 6e74 2045 6e76 6972 6f6e 6d65 6e74  rent Environment
-0000fef0: 3a3a 0a0a 2020 2020 7365 6c66 2e45 6e76  ::..    self.Env
-0000ff00: 2e73 6574 2827 4d79 2076 6172 272c 2027  .set('My var', '
-0000ff10: 6f6e 6520 7661 6c75 6527 290a 0a59 6f75  one value')..You
-0000ff20: 2063 616e 2067 6574 2061 2076 616c 7565   can get a value
-0000ff30: 2066 726f 6d20 7468 6520 6375 7272 656e   from the curren
-0000ff40: 7420 456e 7669 726f 6e6d 656e 743a 3a0a  t Environment::.
-0000ff50: 0a20 2020 206d 7976 616c 7565 203d 2073  .    myvalue = s
-0000ff60: 656c 662e 456e 762e 6765 7428 274d 7920  elf.Env.get('My 
-0000ff70: 7661 7227 2c20 6465 6661 756c 3d22 4d79  var', defaul="My
-0000ff80: 2064 6566 6175 6c74 2076 616c 7565 2229   default value")
-0000ff90: 0a0a 2e2e 206e 6f74 653a 3a0a 0a20 2020  .... note::..   
-0000ffa0: 2054 6865 2065 6e76 6972 6f6e 6d65 6e74   The environment
-0000ffb0: 2069 7320 6173 2061 2064 6963 7420 7468   is as a dict th
-0000ffc0: 6520 7661 6c75 6520 6361 6e20 6265 2061  e value can be a
-0000ffd0: 6e20 696e 7374 616e 6365 206f 6620 616e  n instance of an
-0000ffe0: 7920 7479 7065 0a0a 496e 6974 6961 6c69  y type..Initiali
-0000fff0: 7a65 2073 6f6d 6520 6461 7461 2062 7920  ze some data by 
-00010000: 656e 7472 7920 706f 696e 740a 7e7e 7e7e  entry point.~~~~
-00010010: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00010020: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a  ~~~~~~~~~~~~~~~.
-00010030: 0a74 6865 2065 6e74 7279 2070 6f69 6e74  .the entry point
-00010040: 2060 6061 6e79 626c 6f6b 2e69 6e69 7460   ``anyblok.init`
-00010050: 6020 616c 6c6f 7720 746f 2064 6566 696e  ` allow to defin
-00010060: 6520 6675 6e63 7469 6f6e 2c20 6060 c3ac  e function, ``..
-00010070: 6e69 745f 6675 6e63 7469 6f6e 6060 0a69  nit_function``.i
-00010080: 6e20 7468 6973 2065 7861 6d70 6c65 3a3a  n this example::
-00010090: 0a0a 2020 2020 7365 7475 7028 0a20 2020  ..    setup(.   
-000100a0: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
-000100b0: 2065 6e74 7279 5f70 6f69 6e74 733d 7b0a   entry_points={.
-000100c0: 2020 2020 2020 2020 2020 2020 2761 6e79              'any
-000100d0: 626c 6f6b 2e69 6e69 7427 3a20 5b0a 2020  blok.init': [.  
-000100e0: 2020 2020 2020 2020 2020 2020 2020 276d                'm
-000100f0: 795f 6675 6e63 7469 6f6e 3d70 6174 683a  y_function=path:
-00010100: 696e 6974 5f66 756e 6374 696f 6e27 2c0a  init_function',.
-00010110: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
-00010120: 2020 2020 2020 207d 2c0a 2020 2020 290a         },.    ).
-00010130: 0a49 6e20 7468 6520 7061 7468 2074 6865  .In the path the
-00010140: 2069 6e69 745f 6675 6e63 7469 6f6e 206d   init_function m
-00010150: 7573 7420 6265 2064 6566 696e 6564 3a3a  ust be defined::
-00010160: 0a0a 2020 2020 6465 6620 696e 6974 5f66  ..    def init_f
-00010170: 756e 6374 696f 6e28 756e 6974 7465 7374  unction(unittest
-00010180: 3d46 616c 7365 293a 0a20 2020 2020 2020  =False):.       
-00010190: 202e 2e2e 0a0a 2e2e 7761 726e 696e 673a   .......warning:
-000101a0: 3a0a 0a20 2020 2055 7365 2075 6e69 7474  :..    Use unitt
-000101b0: 6573 7420 7061 7261 6d65 7465 7220 746f  est parameter to
-000101c0: 2064 6566 696e 6564 2069 6620 7468 6520   defined if the 
-000101d0: 6675 6e63 7469 6f6e 206d 7573 7420 6265  function must be
-000101e0: 2063 616c 6c0a 2020 2020 6f72 206e 6f74   call.    or not
-000101f0: 0a0a 4d61 6b65 2065 6173 696c 7920 5265  ..Make easily Re
-00010200: 6164 4f6e 6c79 206d 6f64 656c 0a7e 7e7e  adOnly model.~~~
-00010210: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
-00010220: 7e7e 7e7e 7e7e 7e0a 0a49 6e20 736f 6d6d  ~~~~~~~..In somm
-00010230: 6520 6361 7365 2079 6f75 2077 616e 7420  e case you want 
-00010240: 7468 6174 2079 6f75 7220 6d6f 6465 6c20  that your model 
-00010250: 6973 3a0a 0a2a 2072 6561 646f 6e6c 793a  is:..* readonly:
-00010260: 204e 6f20 6d6f 6469 6669 6361 7469 6f6e   No modification
-00010270: 2c20 4e6f 2064 656c 6574 696f 6e3a 3a0a  , No deletion::.
-00010280: 0a20 2020 2020 2040 7265 6769 7374 6572  .      @register
-00010290: 282e 2e2e 290a 2020 2020 2020 636c 6173  (...).      clas
-000102a0: 7320 4d79 4d6f 6465 6c28 4d69 7869 6e2e  s MyModel(Mixin.
-000102b0: 5265 6164 4f6e 6c79 293a 0a20 2020 2020  ReadOnly):.     
-000102c0: 2020 202e 2e2e 0a0a 2a20 666f 7262 6964     .....* forbid
-000102d0: 206d 6f64 6966 6963 6174 696f 6e3a 204e   modification: N
-000102e0: 6f20 6d6f 6469 6669 6361 7469 6f6e 2062  o modification b
-000102f0: 7574 2063 616e 2064 656c 6574 653a 3a0a  ut can delete::.
-00010300: 0a20 2020 2020 2040 7265 6769 7374 6572  .      @register
-00010310: 282e 2e2e 290a 2020 2020 2020 636c 6173  (...).      clas
-00010320: 7320 4d79 4d6f 6465 6c28 4d69 7869 6e2e  s MyModel(Mixin.
-00010330: 466f 7262 6964 5570 6461 7465 293a 0a20  ForbidUpdate):. 
-00010340: 2020 2020 2020 202e 2e2e 0a0a 2a20 666f         .....* fo
-00010350: 7262 6964 2064 656c 6574 696f 6e3a 204e  rbid deletion: N
-00010360: 6f20 6465 6c65 7469 6f6e 2062 7574 2063  o deletion but c
-00010370: 616e 206d 6f64 6966 793a 3a0a 0a20 2020  an modify::..   
-00010380: 2020 2040 7265 6769 7374 6572 282e 2e2e     @register(...
-00010390: 290a 2020 2020 2020 636c 6173 7320 4d79  ).      class My
-000103a0: 4d6f 6465 6c28 4d69 7869 6e2e 466f 7262  Model(Mixin.Forb
-000103b0: 6964 4465 6c65 7465 293a 0a20 2020 2020  idDelete):.     
-000103c0: 2020 202e 2e2e 0a0a 0a50 6c75 6769 6e0a     ......Plugin.
-000103d0: 2d2d 2d2d 2d2d 0a0a 506c 7567 696e 2069  ------..Plugin i
-000103e0: 7320 7573 6564 2066 6f72 2074 6865 206c  s used for the l
-000103f0: 6f77 206c 6576 656c 2c20 6974 2069 7320  ow level, it is 
-00010400: 6e6f 7420 7573 6520 696e 2074 6865 2062  not use in the b
-00010410: 6c6f 6b73 2c20 6265 6361 7573 6520 7468  loks, because th
-00010420: 6520 6d6f 6465 6c0a 6361 6e20 6265 206f  e model.can be o
-00010430: 7665 726c 6f61 6420 6279 2074 6865 2064  verload by the d
-00010440: 6563 6c61 7261 7469 6f6e 2e0a 0a44 6566  eclaration...Def
-00010450: 696e 6520 6120 6e65 7720 706c 7567 696e  ine a new plugin
-00010460: 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  .~~~~~~~~~~~~~~~
-00010470: 7e7e 7e7e 0a0a 4120 706c 7567 696e 2063  ~~~~..A plugin c
-00010480: 616e 2062 6520 6120 636c 6173 7320 6f72  an be a class or
-00010490: 2061 2066 756e 6374 696f 6e3a 3a0a 0a20   a function::.. 
-000104a0: 2020 2063 6c61 7373 204d 7950 6c75 6769     class MyPlugi
-000104b0: 6e3a 0a20 2020 2020 2020 2070 6173 730a  n:.        pass.
-000104c0: 0a41 6464 2074 6865 2070 6c75 6769 6e20  .Add the plugin 
-000104d0: 6465 6669 6e69 7469 6f6e 2069 6e20 7468  definition in th
-000104e0: 6520 636f 6e66 6967 7572 6174 696f 6e3a  e configuration:
-000104f0: 3a0a 0a20 2020 2040 436f 6e66 6967 7572  :..    @Configur
-00010500: 6174 696f 6e2e 6164 6428 2770 6c75 6769  ation.add('plugi
-00010510: 6e73 2729 0a20 2020 2064 6566 2061 6464  ns').    def add
-00010520: 5f70 6c75 6769 6e73 2873 656c 662c 2067  _plugins(self, g
-00010530: 726f 7570 290a 2020 2020 2020 2020 6772  roup).        gr
-00010540: 6f75 702e 6164 645f 6172 6775 6d65 6e74  oup.add_argument
-00010550: 2827 2d2d 6d79 2d6f 7074 696f 6e27 2c20  ('--my-option', 
-00010560: 6465 7374 3d27 706c 7567 696e 5f6e 616d  dest='plugin_nam
-00010570: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
-00010580: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00010590: 7970 653d 416e 7942 6c6f 6b50 6c75 6769  ype=AnyBlokPlugi
-000105a0: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
-000105b0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-000105c0: 6661 756c 743d 2770 6174 683a 4d79 506c  fault='path:MyPl
-000105d0: 7567 696e 2729 0a0a 5573 6520 7468 6520  ugin')..Use the 
-000105e0: 706c 7567 696e 3a3a 0a0a 2020 2020 706c  plugin::..    pl
-000105f0: 7567 696e 203d 2043 6f6e 6669 6775 7261  ugin = Configura
-00010600: 7469 6f6e 2e67 6574 2827 706c 7567 696e  tion.get('plugin
-00010610: 5f6e 616d 6527 290a 0a0a 2a2a 616e 7962  _name')...**anyb
-00010620: 6c6f 6b2e 6d6f 6465 6c2e 706c 7567 696e  lok.model.plugin
-00010630: 2a2a 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  **.-------------
-00010640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a54 6869  -----------..Thi
-00010650: 7320 6120 686f 6f6b 2074 6f20 6164 6420  s a hook to add 
-00010660: 6e65 7720 6665 6174 7572 6520 696e 204d  new feature in M
-00010670: 6f64 656c 2c20 7468 6973 2069 7320 616c  odel, this is al
-00010680: 7265 6164 7920 7573 6520 666f 723a 0a0a  ready use for:..
-00010690: 2a20 6879 6272 6964 5f6d 6574 686f 640a  * hybrid_method.
-000106a0: 2a20 7461 626c 6520 616e 6420 6d61 7070  * table and mapp
-000106b0: 6572 2061 7267 730a 2a20 6576 656e 740a  er args.* event.
-000106c0: 2a20 5371 6c61 6c63 6865 6d79 2065 7665  * Sqlalchemy eve
-000106d0: 6e74 0a2a 2063 6163 6865 202f 2063 6c61  nt.* cache / cla
-000106e0: 7373 6d65 7468 6f64 5f63 6163 6865 0a0a  ssmethod_cache..
-000106f0: 5374 6172 7420 6279 2069 6d70 6c65 6d65  Start by impleme
-00010700: 6e74 696e 6720 7468 6520 706c 7567 696e  nting the plugin
-00010710: 2028 7365 650a 3a63 6c61 7373 3a60 4d6f   (see.:class:`Mo
-00010720: 6465 6c50 6c75 6769 6e42 6173 6520 3c61  delPluginBase <a
-00010730: 6e79 626c 6f6b 2e6d 6f64 656c 2e70 6c75  nyblok.model.plu
-00010740: 6769 6e73 2e4d 6f64 656c 506c 7567 696e  gins.ModelPlugin
-00010750: 4261 7365 3e60 293a 3a0a 0a20 2020 2066  Base>`)::..    f
-00010760: 726f 6d20 616e 7962 6c6f 6b2e 6d6f 6465  rom anyblok.mode
-00010770: 6c2e 706c 7567 696e 7320 696d 706f 7274  l.plugins import
-00010780: 204d 6f64 656c 506c 7567 696e 4261 7365   ModelPluginBase
-00010790: 0a0a 2020 2020 636c 6173 7320 4d79 506c  ..    class MyPl
-000107a0: 7567 696e 284d 6f64 656c 506c 7567 696e  ugin(ModelPlugin
-000107b0: 4261 7365 293a 0a20 2020 2020 2020 202e  Base):.        .
-000107c0: 2e2e 0a0a 0a54 6865 6e2c 2064 6563 6c61  .....Then, decla
-000107d0: 7265 2069 7420 696e 2060 6073 6574 7570  re it in ``setup
-000107e0: 2e70 7960 603a 3a0a 0a20 2020 2073 6574  .py``::..    set
-000107f0: 7570 280a 2020 2020 2020 2020 2e2e 2e0a  up(.        ....
-00010800: 2020 2020 2020 2020 656e 7472 795f 706f          entry_po
-00010810: 696e 7473 3d7b 0a20 2020 2020 2020 2020  ints={.         
-00010820: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
-00010830: 2020 2027 616e 7962 6c6f 6b2e 6d6f 6465     'anyblok.mode
-00010840: 6c2e 706c 7567 696e 273a 205b 0a20 2020  l.plugin': [.   
-00010850: 2020 2020 2020 2020 2020 2020 2027 6d79               'my
-00010860: 706c 7567 696e 3d70 6174 683a 4d79 506c  plugin=path:MyPl
-00010870: 7567 696e 272c 0a20 2020 2020 2020 2020  ugin',.         
-00010880: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
-00010890: 2020 2e2e 2e0a 2020 2020 2020 2020 7d2c    ....        },
-000108a0: 0a20 2020 2020 2020 202e 2e2e 0a20 2020  .        ....   
-000108b0: 2029 0a0a 0a2a 2a61 6e79 626c 6f6b 2e6d   )...**anyblok.m
-000108c0: 6f64 656c 2e66 6163 746f 7279 2a2a 0a2d  odel.factory**.-
-000108d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000108e0: 2d2d 2d2d 2d2d 2d2d 0a0a 5468 6973 2066  --------..This f
-000108f0: 6163 746f 7279 2069 7320 7573 6564 2074  actory is used t
-00010900: 6f3a 0a0a 2a20 6769 7665 2074 6865 2063  o:..* give the c
-00010910: 6f72 6520 636c 6173 7365 7320 6e65 6564  ore classes need
-00010920: 2074 6f20 6275 696c 6420 7468 6520 6d6f   to build the mo
-00010930: 6465 6c0a 2a20 6275 696c 6420 7468 6520  del.* build the 
-00010940: 6d6f 6465 6c0a 0a53 7461 7274 2062 7920  model..Start by 
-00010950: 696d 706c 656d 656e 7469 6e67 2074 6865  implementing the
-00010960: 2066 6163 746f 7279 2028 7365 650a 3a63   factory (see.:c
-00010970: 6c61 7373 3a60 4261 7365 4661 6374 6f72  lass:`BaseFactor
-00010980: 7920 3c61 6e79 626c 6f6b 2e6d 6f64 656c  y <anyblok.model
-00010990: 2e74 6163 746f 7279 2e42 6173 6546 6163  .tactory.BaseFac
-000109a0: 746f 7279 3e60 293a 3a0a 0a20 2020 2066  tory>`)::..    f
-000109b0: 726f 6d20 616e 7962 6c6f 6b2e 6d6f 6465  rom anyblok.mode
-000109c0: 6c2e 6661 6374 6f72 7920 696d 706f 7274  l.factory import
-000109d0: 2042 6173 6546 6163 746f 7279 0a0a 2020   BaseFactory..  
-000109e0: 2020 636c 6173 7320 4d79 4661 6374 6f72    class MyFactor
-000109f0: 7928 4261 7365 4661 6374 6f72 7929 3a0a  y(BaseFactory):.
-00010a00: 0a20 2020 2020 2020 2064 6566 2069 6e73  .        def ins
-00010a10: 6572 745f 636f 7265 5f62 6173 6573 2873  ert_core_bases(s
-00010a20: 656c 662c 2062 6173 6573 2c20 7072 6f70  elf, bases, prop
-00010a30: 6572 7469 6573 293a 0a20 2020 2020 2020  erties):.       
-00010a40: 2020 2020 202e 2e2e 0a0a 2020 2020 2020       .....      
-00010a50: 2020 6465 6620 6275 696c 645f 6d6f 6465    def build_mode
-00010a60: 6c28 7365 6c66 2c20 6d6f 6465 6c6e 616d  l(self, modelnam
-00010a70: 652c 2062 6173 6573 2c20 7072 6f70 6572  e, bases, proper
-00010a80: 7469 6573 293a 0a20 2020 2020 2020 2020  ties):.         
-00010a90: 2020 202e 2e2e 0a0a 496e 2079 6f75 7220     .....In your 
-00010aa0: 626c 6f6b 7320 796f 7520 6361 6e20 7573  bloks you can us
-00010ab0: 6520 796f 7572 2066 6163 746f 7279 3a3a  e your factory::
-00010ac0: 0a0a 2020 2020 4072 6567 6973 7465 7228  ..    @register(
-00010ad0: 4d6f 6465 6c2c 2066 6163 746f 7279 3d4d  Model, factory=M
-00010ae0: 7946 6163 746f 7279 290a 2020 2020 636c  yFactory).    cl
-00010af0: 6173 7320 4d79 4d6f 6465 6c3a 0a20 2020  ass MyModel:.   
-00010b00: 2020 2020 202e 2e2e 0a0a 2a2a 456e 6769       .....**Engi
-00010b10: 6e65 2773 2065 7665 6e74 732a 2a0a 2d2d  ne's events**.--
-00010b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00010b30: 2d0a 0a54 6865 2065 6e67 696e 6527 7320  -..The engine's 
-00010b40: 6576 656e 7473 2069 7320 7573 6564 2074  events is used t
-00010b50: 6f20 6465 6669 6e65 2073 716c 616c 6368  o define sqlalch
-00010b60: 656d 7920 6576 656e 7420 6c69 7374 656e  emy event listen
-00010b70: 6572 206f 6e20 656e 6769 6e65 0a0a 7468  er on engine..th
-00010b80: 6973 2065 7665 6e74 2069 7320 6465 636c  is event is decl
-00010b90: 6172 6564 2062 7920 656e 7472 7970 6f69  ared by entrypoi
-00010ba0: 6e74 3a0a 0a2a 202a 2a61 6e79 626c 6f6b  nt:..* **anyblok
-00010bb0: 2e65 6e67 696e 652e 6576 656e 742a 2a20  .engine.event** 
-00010bc0: 3a20 466f 7220 616c 6c20 6469 616c 6563  : For all dialec
-00010bd0: 7473 0a2a 202a 2a61 6e79 626c 6f6b 2e65  ts.* **anyblok.e
-00010be0: 6e67 696e 652e 6576 656e 742e 706f 7374  ngine.event.post
-00010bf0: 6772 6573 2a2a 203a 206f 6e6c 7920 666f  gres** : only fo
-00010c00: 7220 706f 7374 6772 6573 716c 0a2a 202a  r postgresql.* *
-00010c10: 2a61 6e79 626c 6f6b 2e65 6e67 696e 652e  *anyblok.engine.
-00010c20: 6576 656e 742e 6d79 7371 6c2a 2a20 3a20  event.mysql** : 
-00010c30: 6f6e 6c79 2066 6f72 204d 7953 514c 0a2a  only for MySQL.*
-00010c40: 202a 2a61 6e79 626c 6f6b 2e65 6e67 696e   **anyblok.engin
-00010c50: 652e 6576 656e 742e 6d73 7371 6c2a 2a20  e.event.mssql** 
-00010c60: 3a20 6f6e 6c79 2066 6f72 204d 7353 514c  : only for MsSQL
-00010c70: 0a0a 4578 656d 706c 6520 7769 7468 2074  ..Exemple with t
-00010c80: 6865 202a 2a6d 7973 716c 5f6e 6f5f 6175  he **mysql_no_au
-00010c90: 746f 636f 6d6d 6974 2a2a 206c 6973 7465  tocommit** liste
-00010ca0: 6e65 720a 0a2a 2a61 6e79 626c 6f6b 2e65  ner..**anyblok.e
-00010cb0: 7665 6e74 2a2a 3a3a 0a0a 2020 2066 726f  vent**::..   fro
-00010cc0: 6d20 7371 6c61 6c63 6865 6d79 2069 6d70  m sqlalchemy imp
-00010cd0: 6f72 7420 6576 656e 740a 0a0a 2020 2064  ort event...   d
-00010ce0: 6566 206d 7973 716c 5f6e 6f5f 6175 746f  ef mysql_no_auto
-00010cf0: 636f 6d6d 6974 2865 6e67 696e 6529 3a0a  commit(engine):.
-00010d00: 0a20 2020 2020 2020 6465 6620 6d79 7371  .       def mysq
-00010d10: 6c5f 7365 745f 6e6f 5f61 7574 6f63 6f6d  l_set_no_autocom
-00010d20: 6d69 7428 6462 6170 695f 636f 6e2c 2063  mit(dbapi_con, c
-00010d30: 6f6e 6e65 6374 696f 6e5f 7265 636f 7264  onnection_record
-00010d40: 293a 0a20 2020 2020 2020 2020 2020 6375  ):.           cu
-00010d50: 7220 3d20 6462 6170 695f 636f 6e2e 6375  r = dbapi_con.cu
-00010d60: 7273 6f72 2829 0a20 2020 2020 2020 2020  rsor().         
-00010d70: 2020 6375 722e 6578 6563 7574 6528 2253    cur.execute("S
-00010d80: 4554 2061 7574 6f63 6f6d 6d69 743d 303b  ET autocommit=0;
-00010d90: 2229 0a20 2020 2020 2020 2020 2020 6375  ").           cu
-00010da0: 722e 6578 6563 7574 6528 2253 4554 2053  r.execute("SET S
-00010db0: 4553 5349 4f4e 2073 716c 5f6d 6f64 653d  ESSION sql_mode=
-00010dc0: 2754 5241 4449 5449 4f4e 414c 273b 2229  'TRADITIONAL';")
-00010dd0: 0a20 2020 2020 2020 2020 2020 6375 7220  .           cur 
-00010de0: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2065  = None..       e
-00010df0: 7665 6e74 2e6c 6973 7465 6e28 656e 6769  vent.listen(engi
-00010e00: 6e65 2c20 2763 6f6e 6e65 6374 272c 206d  ne, 'connect', m
-00010e10: 7973 716c 5f73 6574 5f6e 6f5f 6175 746f  ysql_set_no_auto
-00010e20: 636f 6d6d 6974 290a 0a0a 2a2a 7365 7475  commit)...**setu
-00010e30: 702e 7079 2a2a 3a3a 0a0a 2020 2073 6574  p.py**::..   set
-00010e40: 7570 280a 2020 2020 2020 2065 6e74 7279  up(.       entry
-00010e50: 5f70 6f69 6e74 733d 7b0a 2020 2020 2020  _points={.      
-00010e60: 2020 2020 2027 616e 7962 6c6f 6b2e 656e       'anyblok.en
-00010e70: 6769 6e65 2e65 7665 6e74 2e6d 7973 716c  gine.event.mysql
-00010e80: 273a 205b 0a20 2020 2020 2020 2020 2020  ': [.           
-00010e90: 2020 2020 276d 7973 716c 2d6e 6f2d 6175      'mysql-no-au
-00010ea0: 746f 636f 6d6d 6974 3d61 6e79 626c 6f6b  tocommit=anyblok
-00010eb0: 2e65 7665 6e74 3a6d 7973 716c 5f6e 6f5f  .event:mysql_no_
-00010ec0: 6175 746f 636f 6d6d 6974 272c 0a20 2020  autocommit',.   
-00010ed0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00010ee0: 2020 7d2c 0a20 2020 290a 0a2e 2e20 6e6f    },.   ).... no
-00010ef0: 7465 3a3a 0a0a 2020 2054 6865 2053 514c  te::..   The SQL
-00010f00: 416c 6368 656d 7920 6465 6375 6d65 6e74  Alchemy decument
-00010f10: 6174 696f 6e20 666f 7220 7468 6520 6063  ation for the `c
-00010f20: 6f72 6520 6576 656e 7420 3c68 7474 7073  ore event <https
-00010f30: 3a2f 2f64 6f63 732e 7371 6c61 6c63 6865  ://docs.sqlalche
-00010f40: 6d79 2e6f 7267 2f65 6e2f 3134 2f63 6f72  my.org/en/14/cor
-00010f50: 652f 6576 656e 7473 2e68 746d 6c3f 6869  e/events.html?hi
-00010f60: 6768 6c69 6768 743d 6576 656e 7423 636f  ghlight=event#co
-00010f70: 6e6e 6563 7469 6f6e 2d70 6f6f 6c2d 6576  nnection-pool-ev
-00010f80: 656e 7473 3e60 5f0a 0a2a 2a53 6573 7369  ents>`_..**Sessi
-00010f90: 6f6e 2773 2065 7665 6e74 732a 2a0a 2d2d  on's events**.--
-00010fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00010fb0: 2d2d 0a0a 5468 6520 656e 6769 6e65 2773  --..The engine's
-00010fc0: 2065 7665 6e74 7320 6973 2075 7365 6420   events is used 
-00010fd0: 746f 2064 6566 696e 6520 7371 6c61 6c63  to define sqlalc
-00010fe0: 6865 6d79 2065 7665 6e74 206c 6973 7465  hemy event liste
-00010ff0: 6e65 7220 6f6e 2065 6e67 696e 650a 0a74  ner on engine..t
-00011000: 6869 7320 6576 656e 7420 6973 2064 6563  his event is dec
-00011010: 6c61 7265 6420 6279 2065 6e74 7279 706f  lared by entrypo
-00011020: 696e 743a 0a0a 2a20 2a2a 616e 7962 6c6f  int:..* **anyblo
-00011030: 6b2e 7365 7373 696f 6e2e 6576 656e 742a  k.session.event*
-00011040: 2a20 3a20 466f 7220 616c 6c20 6469 616c  * : For all dial
-00011050: 6563 7473 0a2a 202a 2a61 6e79 626c 6f6b  ects.* **anyblok
-00011060: 2e73 6573 7369 6f6e 2e65 7665 6e74 2e70  .session.event.p
-00011070: 6f73 7467 7265 7371 6c2a 2a20 3a20 6f6e  ostgresql** : on
-00011080: 6c79 2066 6f72 2070 6f73 7467 7265 7371  ly for postgresq
-00011090: 6c0a 2a20 2a2a 616e 7962 6c6f 6b2e 7365  l.* **anyblok.se
-000110a0: 7373 696f 6e2e 6576 656e 742e 6d79 7371  ssion.event.mysq
-000110b0: 6c2a 2a20 3a20 6f6e 6c79 2066 6f72 204d  l** : only for M
-000110c0: 7953 514c 0a2a 202a 2a61 6e79 626c 6f6b  ySQL.* **anyblok
-000110d0: 2e73 6573 7369 6f6e 2e65 7665 6e74 2e6d  .session.event.m
-000110e0: 7373 716c 2a2a 203a 206f 6e6c 7920 666f  ssql** : only fo
-000110f0: 7220 4d73 5351 4c0a 0a45 7865 6d70 6c65  r MsSQL..Exemple
-00011100: 0a0a 6d65 7468 6f64 3a3a 0a0a 2020 2066  ..method::..   f
-00011110: 726f 6d20 7371 6c61 6c63 6865 6d79 2069  rom sqlalchemy i
-00011120: 6d70 6f72 7420 6576 656e 740a 0a0a 2020  mport event...  
-00011130: 2064 6566 2064 6f5f 736f 6d65 7468 696e   def do_somethin
-00011140: 6728 7365 7373 696f 6e29 3a0a 0a20 2020  g(session):..   
-00011150: 2020 2020 6465 6620 736f 6d65 7468 696e      def somethin
-00011160: 6728 7365 7373 2c20 7472 616e 7361 6374  g(sess, transact
-00011170: 696f 6e2c 2063 6f6e 6e65 6374 696f 6e29  ion, connection)
-00011180: 3a0a 2020 2020 2020 2020 2020 2070 6173  :.           pas
-00011190: 730a 0a20 2020 2020 2020 6576 656e 742e  s..       event.
-000111a0: 6c69 7374 656e 2873 6573 7369 6f6e 2c20  listen(session, 
-000111b0: 2761 6674 6572 5f62 6567 696e 272c 2073  'after_begin', s
-000111c0: 6f6d 6574 6869 6e67 290a 0a0a 2a2a 7365  omething)...**se
-000111d0: 7475 702e 7079 2a2a 3a3a 0a0a 2020 2073  tup.py**::..   s
-000111e0: 6574 7570 280a 2020 2020 2020 2065 6e74  etup(.       ent
-000111f0: 7279 5f70 6f69 6e74 733d 7b0a 2020 2020  ry_points={.    
-00011200: 2020 2020 2020 2027 616e 7962 6c6f 6b2e         'anyblok.
-00011210: 7365 7373 696f 6e2e 6576 656e 7427 3a20  session.event': 
-00011220: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00011230: 2027 646f 2d73 6f6d 6574 6869 6e67 3d70   'do-something=p
-00011240: 6174 683a 646f 5f73 6f6d 6574 6869 6e67  ath:do_something
-00011250: 272c 0a20 2020 2020 2020 2020 2020 5d2c  ',.           ],
-00011260: 0a20 2020 2020 2020 7d2c 0a20 2020 290a  .       },.   ).
-00011270: 0a2e 2e20 6e6f 7465 3a3a 0a0a 2020 2054  ... note::..   T
-00011280: 6865 2053 514c 416c 6368 656d 7920 6465  he SQLAlchemy de
-00011290: 6375 6d65 6e74 6174 696f 6e20 666f 7220  cumentation for 
-000112a0: 7468 6520 6073 6573 7369 6f6e 2065 7665  the `session eve
-000112b0: 6e74 7320 3c68 7474 7073 3a2f 2f64 6f63  nts <https://doc
-000112c0: 732e 7371 6c61 6c63 6865 6d79 2e6f 7267  s.sqlalchemy.org
-000112d0: 2f65 6e2f 3134 2f6f 726d 2f65 7665 6e74  /en/14/orm/event
-000112e0: 732e 6874 6d6c 2373 6573 7369 6f6e 2d65  s.html#session-e
-000112f0: 7665 6e74 733e 605f 0a                   vents>`_.
+0000d5d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d5e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d5f0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2060 606b  ---------+.| ``k
+0000d600: 6579 7360 6020 2020 2020 2020 2020 207c  eys``          |
+0000d610: 206c 6973 7420 6f66 2073 7472 696e 672c   list of string,
+0000d620: 2072 6570 7265 7365 6e74 2074 6865 2070   represent the p
+0000d630: 6174 6820 696e 206a 736f 6e20 746f 2073  ath in json to s
+0000d640: 746f 7265 2061 6e64 207c 0a7c 2020 2020  tore and |.|    
+0000d650: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0000d660: 2067 6574 2074 6865 2076 616c 7565 2020   get the value  
+0000d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d690: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
+0000d6a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+0000d6b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d6c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d6d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d6e0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6067  ---------+.| ``g
+0000d6f0: 6574 5f61 6461 7074 6572 6060 2020 207c  et_adapter``   |
+0000d700: 206d 6574 686f 6420 746f 2063 6f6e 7665   method to conve
+0000d710: 7274 2074 6865 2064 6174 6520 6166 7465  rt the date afte
+0000d720: 7220 6765 7420 6974 2e20 5468 6973 2076  r get it. This v
+0000d730: 616c 7565 2020 2020 207c 0a7c 2020 2020  alue     |.|    
+0000d740: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0000d750: 2063 616e 2062 6520 7468 6520 6e61 6d65   can be the name
+0000d760: 206f 6620 6120 6d65 7468 6f64 206f 6e20   of a method on 
+0000d770: 7468 6520 6d6f 6465 6c20 2020 2020 2020  the model       
+0000d780: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
+0000d790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+0000d7a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d7b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d7c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d7d0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2060 6073  ---------+.| ``s
+0000d7e0: 6574 5f61 6461 7074 6572 6060 2020 207c  et_adapter``   |
+0000d7f0: 206d 6574 686f 6420 746f 2063 6f6e 7665   method to conve
+0000d800: 7274 2074 6865 2064 6174 6520 6265 666f  rt the date befo
+0000d810: 7265 2073 746f 7265 2069 742e 2054 6869  re store it. Thi
+0000d820: 7320 7661 6c75 6520 207c 0a7c 2020 2020  s value  |.|    
+0000d830: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0000d840: 2063 616e 2062 6520 7468 6520 6e61 6d65   can be the name
+0000d850: 206f 6620 6120 6d65 7468 6f64 206f 6e20   of a method on 
+0000d860: 7468 6520 6d6f 6465 6c20 2020 2020 2020  the model       
+0000d870: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
+0000d880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+0000d890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d8a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d8b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d8c0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a 4d69 7869  ---------+..Mixi
+0000d8d0: 6e0a 2d2d 2d2d 2d0a 0a41 204d 6978 696e  n.-----..A Mixin
+0000d8e0: 206c 6f6f 6b73 206c 696b 6520 6120 4d6f   looks like a Mo
+0000d8f0: 6465 6c2c 2062 7574 2068 6173 206e 6f20  del, but has no 
+0000d900: 7461 626c 6573 2e20 4120 4d69 7869 6e20  tables. A Mixin 
+0000d910: 6164 6473 2062 6568 6176 696f 7572 2074  adds behaviour t
+0000d920: 6f0a 6120 4d6f 6465 6c20 7769 7468 2050  o.a Model with P
+0000d930: 7974 686f 6e20 696e 6865 7269 7461 6e63  ython inheritanc
+0000d940: 653a 3a0a 0a20 2020 2040 7265 6769 7374  e::..    @regist
+0000d950: 6572 284d 6978 696e 290a 2020 2020 636c  er(Mixin).    cl
+0000d960: 6173 7320 4d79 4d69 7869 6e3a 0a0a 2020  ass MyMixin:..  
+0000d970: 2020 2020 2020 6465 6620 666f 6f28 293a        def foo():
+0000d980: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
+0000d990: 730a 0a20 2020 2040 7265 6769 7374 6572  s..    @register
+0000d9a0: 284d 6f64 656c 290a 2020 2020 636c 6173  (Model).    clas
+0000d9b0: 7320 4d79 4d6f 6465 6c28 4d69 7869 6e2e  s MyModel(Mixin.
+0000d9c0: 4d79 4d69 7869 6e29 3a0a 2020 2020 2020  MyMixin):.      
+0000d9d0: 2020 7061 7373 0a0a 2020 2020 2d2d 2d2d    pass..    ----
+0000d9e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d9f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
+0000da00: 2020 2020 6173 7365 7274 2068 6173 6174      assert hasat
+0000da10: 7472 2872 6567 6973 7472 792e 4d79 4d6f  tr(registry.MyMo
+0000da20: 6465 6c2c 2027 666f 6f27 290a 0a0a 4966  del, 'foo')...If
+0000da30: 2079 6f75 2069 6e68 6572 6974 2061 206d   you inherit a m
+0000da40: 6978 696e 2c20 616c 6c20 7468 6520 6d6f  ixin, all the mo
+0000da50: 6465 6c73 2070 7265 7669 6f75 736c 7920  dels previously 
+0000da60: 7573 696e 6720 7468 6520 6261 7365 206d  using the base m
+0000da70: 6978 696e 2061 6c73 6f20 6265 6e65 6669  ixin also benefi
+0000da80: 740a 6672 6f6d 2074 6865 206f 7665 726c  t.from the overl
+0000da90: 6f61 643a 3a0a 0a20 2020 2040 7265 6769  oad::..    @regi
+0000daa0: 7374 6572 284d 6978 696e 290a 2020 2020  ster(Mixin).    
+0000dab0: 636c 6173 7320 4d79 4d69 7869 6e3a 0a20  class MyMixin:. 
+0000dac0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+0000dad0: 2040 7265 6769 7374 6572 284d 6f64 656c   @register(Model
+0000dae0: 290a 2020 2020 636c 6173 7320 4d79 4d6f  ).    class MyMo
+0000daf0: 6465 6c28 4d69 7869 6e2e 4d79 4d69 7869  del(Mixin.MyMixi
+0000db00: 6e29 3a0a 2020 2020 2020 2020 7061 7373  n):.        pass
+0000db10: 0a0a 2020 2020 4072 6567 6973 7465 7228  ..    @register(
+0000db20: 4d69 7869 6e29 0a20 2020 2063 6c61 7373  Mixin).    class
+0000db30: 204d 794d 6978 696e 3a0a 0a20 2020 2020   MyMixin:..     
+0000db40: 2020 2064 6566 2066 6f6f 2829 3a0a 2020     def foo():.  
+0000db50: 2020 2020 2020 2020 2020 7061 7373 0a0a            pass..
+0000db60: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+0000db70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000db80: 2d2d 2d2d 2d2d 0a0a 2020 2020 6173 7365  ------..    asse
+0000db90: 7274 2068 6173 6174 7472 2861 6e79 626c  rt hasattr(anybl
+0000dba0: 6f6b 2e4d 794d 6f64 656c 2c20 2766 6f6f  ok.MyModel, 'foo
+0000dbb0: 2729 0a0a 0a53 514c 2056 6965 770a 2d2d  ')...SQL View.--
+0000dbc0: 2d2d 2d2d 2d2d 0a0a 416e 2053 514c 2076  ------..An SQL v
+0000dbd0: 6965 7720 6973 2061 206d 6f64 656c 2c20  iew is a model, 
+0000dbe0: 7769 7468 2074 6865 2061 7267 756d 656e  with the argumen
+0000dbf0: 7420 6060 6661 6374 6f72 793d 616e 7962  t ``factory=anyb
+0000dc00: 6c6f 6b2e 6d6f 6465 6c2e 6661 6374 6f72  lok.model.factor
+0000dc10: 792e 5669 6577 4661 6374 6f72 7960 6020  y.ViewFactory`` 
+0000dc20: 696e 2074 6865 0a72 6567 6973 7465 722e  in the.register.
+0000dc30: 2061 6e64 2074 6865 2063 6c61 7373 6d65   and the classme
+0000dc40: 7468 6f64 2060 6073 716c 616c 6368 656d  thod ``sqlalchem
+0000dc50: 795f 7669 6577 5f64 6563 6c61 7261 7469  y_view_declarati
+0000dc60: 6f6e 6060 3a3a 0a0a 2020 2020 6672 6f6d  on``::..    from
+0000dc70: 2061 6e79 626c 6f6b 2e6d 6f64 656c 2e66   anyblok.model.f
+0000dc80: 6163 746f 7279 2069 6d70 6f72 7420 5669  actory import Vi
+0000dc90: 6577 4661 6374 6f72 790a 0a20 2020 2040  ewFactory..    @
+0000dca0: 7265 6769 7374 6572 284d 6f64 656c 290a  register(Model).
+0000dcb0: 2020 2020 636c 6173 7320 5431 3a0a 2020      class T1:.  
+0000dcc0: 2020 2020 2020 6964 203d 2049 6e74 6567        id = Integ
+0000dcd0: 6572 2870 7269 6d61 7279 5f6b 6579 3d54  er(primary_key=T
+0000dce0: 7275 6529 0a20 2020 2020 2020 2063 6f64  rue).        cod
+0000dcf0: 6520 3d20 5374 7269 6e67 2829 0a20 2020  e = String().   
+0000dd00: 2020 2020 2076 616c 203d 2049 6e74 6567       val = Integ
+0000dd10: 6572 2829 0a0a 2020 2020 4072 6567 6973  er()..    @regis
+0000dd20: 7465 7228 4d6f 6465 6c29 0a20 2020 2063  ter(Model).    c
+0000dd30: 6c61 7373 2054 323a 0a20 2020 2020 2020  lass T2:.       
+0000dd40: 2069 6420 3d20 496e 7465 6765 7228 7072   id = Integer(pr
+0000dd50: 696d 6172 795f 6b65 793d 5472 7565 290a  imary_key=True).
+0000dd60: 2020 2020 2020 2020 636f 6465 203d 2053          code = S
+0000dd70: 7472 696e 6728 290a 2020 2020 2020 2020  tring().        
+0000dd80: 7661 6c20 3d20 496e 7465 6765 7228 290a  val = Integer().
+0000dd90: 0a20 2020 2040 7265 6769 7374 6572 284d  .    @register(M
+0000dda0: 6f64 656c 2c20 6661 6374 6f72 793d 5669  odel, factory=Vi
+0000ddb0: 6577 4661 6374 6f72 7929 0a20 2020 2063  ewFactory).    c
+0000ddc0: 6c61 7373 2054 6573 7456 6965 773a 0a20  lass TestView:. 
+0000ddd0: 2020 2020 2020 2063 6f64 6520 3d20 5374         code = St
+0000dde0: 7269 6e67 2870 7269 6d61 7279 5f6b 6579  ring(primary_key
+0000ddf0: 3d54 7275 6529 0a20 2020 2020 2020 2076  =True).        v
+0000de00: 616c 3120 3d20 496e 7465 6765 7228 290a  al1 = Integer().
+0000de10: 2020 2020 2020 2020 7661 6c32 203d 2049          val2 = I
+0000de20: 6e74 6567 6572 2829 0a0a 2020 2020 2020  nteger()..      
+0000de30: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+0000de40: 2020 2020 2020 2064 6566 2073 716c 616c         def sqlal
+0000de50: 6368 656d 795f 7669 6577 5f64 6563 6c61  chemy_view_decla
+0000de60: 7261 7469 6f6e 2863 6c73 293a 0a20 2020  ration(cls):.   
+0000de70: 2020 2020 2020 2020 2022 2222 2054 6869           """ Thi
+0000de80: 7320 6d65 7468 6f64 206d 7573 7420 7265  s method must re
+0000de90: 7475 726e 2074 6865 2071 7565 7279 206f  turn the query o
+0000dea0: 6620 7468 6520 7669 6577 2022 2222 0a20  f the view """. 
+0000deb0: 2020 2020 2020 2020 2020 2054 3120 3d20             T1 = 
+0000dec0: 636c 732e 616e 7962 6c6f 6b2e 5431 0a20  cls.anyblok.T1. 
+0000ded0: 2020 2020 2020 2020 2020 2054 3220 3d20             T2 = 
+0000dee0: 636c 732e 616e 7962 6c6f 6b2e 5432 0a20  cls.anyblok.T2. 
+0000def0: 2020 2020 2020 2020 2020 2071 7565 7279             query
+0000df00: 203d 2073 656c 6563 7428 5b54 312e 636f   = select([T1.co
+0000df10: 6465 2e6c 6162 656c 2827 636f 6465 2729  de.label('code')
+0000df20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000df30: 2020 2020 2020 2020 2020 2020 2020 5431                T1
+0000df40: 2e76 616c 2e6c 6162 656c 2827 7661 6c31  .val.label('val1
+0000df50: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+0000df60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df70: 5432 2e76 616c 2e6c 6162 656c 2827 7661  T2.val.label('va
+0000df80: 6c32 2729 5d29 0a20 2020 2020 2020 2020  l2')]).         
+0000df90: 2020 2072 6574 7572 6e20 7175 6572 792e     return query.
+0000dfa0: 7768 6572 6528 5431 2e63 6f64 6520 3d3d  where(T1.code ==
+0000dfb0: 2054 322e 636f 6465 290a 0a0a 436f 7265   T2.code)...Core
+0000dfc0: 0a2d 2d2d 2d0a 0a60 6043 6f72 6560 6020  .----..``Core`` 
+0000dfd0: 6973 2061 206c 6f77 206c 6576 656c 2073  is a low level s
+0000dfe0: 6574 206f 6620 6465 636c 6172 6174 696f  et of declaratio
+0000dff0: 6e73 2066 6f72 2061 6c6c 2074 6865 204d  ns for all the M
+0000e000: 6f64 656c 7320 6f66 2041 6e79 426c 6f6b  odels of AnyBlok
+0000e010: 2e20 6060 436f 7265 6060 2061 6464 730a  . ``Core`` adds.
+0000e020: 6765 6e65 7261 6c20 6265 6861 7669 6f75  general behaviou
+0000e030: 7220 746f 2074 6865 2061 7070 6c69 6361  r to the applica
+0000e040: 7469 6f6e 2e0a 0a2e 2e20 7761 726e 696e  tion..... warnin
+0000e050: 673a 3a0a 0a20 2020 2043 6f72 6520 6361  g::..    Core ca
+0000e060: 6e20 6e6f 7420 696e 6865 7269 7420 4d6f  n not inherit Mo
+0000e070: 6465 6c2c 204d 6978 696e 2c20 436f 7265  del, Mixin, Core
+0000e080: 2c20 6f72 206f 7468 6572 2064 6563 6c61  , or other decla
+0000e090: 7261 7469 6f6e 2074 7970 652e 0a0a 4261  ration type...Ba
+0000e0a0: 7365 0a7e 7e7e 7e0a 0a41 6464 2061 2062  se.~~~~..Add a b
+0000e0b0: 6568 6176 696f 7572 2069 6e20 616c 6c20  ehaviour in all 
+0000e0c0: 7468 6520 4d6f 6465 6c73 2c20 4561 6368  the Models, Each
+0000e0d0: 204d 6f64 656c 2069 6e68 6572 6974 7320   Model inherits 
+0000e0e0: 4261 7365 2e20 466f 7220 696e 7374 616e  Base. For instan
+0000e0f0: 6365 2c20 7468 650a 6060 6669 7265 6060  ce, the.``fire``
+0000e100: 206d 6574 686f 6420 6f66 2074 6865 2065   method of the e
+0000e110: 7665 6e74 2063 6f6d 6520 6672 6f6d 2060  vent come from `
+0000e120: 6043 6f72 652e 4261 7365 6060 2e0a 0a3a  `Core.Base``...:
+0000e130: 3a0a 0a20 2020 2066 726f 6d20 616e 7962  :..    from anyb
+0000e140: 6c6f 6b20 696d 706f 7274 2044 6563 6c61  lok import Decla
+0000e150: 7261 7469 6f6e 730a 0a0a 2020 2020 4044  rations...    @D
+0000e160: 6563 6c61 7261 7469 6f6e 732e 7265 6769  eclarations.regi
+0000e170: 7374 6572 2844 6563 6c61 7261 7469 6f6e  ster(Declaration
+0000e180: 732e 436f 7265 290a 2020 2020 636c 6173  s.Core).    clas
+0000e190: 7320 4261 7365 3a0a 2020 2020 2020 2020  s Base:.        
+0000e1a0: 7061 7373 0a0a 5371 6c42 6173 650a 7e7e  pass..SqlBase.~~
+0000e1b0: 7e7e 7e7e 7e0a 0a4f 6e6c 7920 7468 6520  ~~~~~..Only the 
+0000e1c0: 4d6f 6465 6c73 2077 6974 6820 6060 4669  Models with ``Fi
+0000e1d0: 656c 6460 602c 2060 6043 6f6c 756d 6e60  eld``, ``Column`
+0000e1e0: 602c 2060 6052 656c 6174 696f 6e53 6869  `, ``RelationShi
+0000e1f0: 7060 6020 696e 6865 7269 7473 2060 6043  p`` inherits ``C
+0000e200: 6f72 652e 5371 6c42 6173 6560 602e 0a46  ore.SqlBase``..F
+0000e210: 6f72 2069 6e73 7461 6e63 652c 2074 6865  or instance, the
+0000e220: 2060 6069 6e73 6572 7460 6020 6d65 7468   ``insert`` meth
+0000e230: 6f64 206f 6e6c 7920 6d61 6b65 7320 7365  od only makes se
+0000e240: 6e73 6520 666f 7220 7468 6520 6060 4d6f  nse for the ``Mo
+0000e250: 6465 6c60 6020 7769 7468 2061 2074 6162  del`` with a tab
+0000e260: 6c65 2e0a 0a3a 3a0a 0a20 2020 2066 726f  le...::..    fro
+0000e270: 6d20 616e 7962 6c6f 6b20 696d 706f 7274  m anyblok import
+0000e280: 2044 6563 6c61 7261 7469 6f6e 730a 0a0a   Declarations...
+0000e290: 2020 2020 4044 6563 6c61 7261 7469 6f6e      @Declaration
+0000e2a0: 732e 7265 6769 7374 6572 2844 6563 6c61  s.register(Decla
+0000e2b0: 7261 7469 6f6e 732e 436f 7265 290a 2020  rations.Core).  
+0000e2c0: 2020 636c 6173 7320 5371 6c42 6173 653a    class SqlBase:
+0000e2d0: 0a20 2020 2020 2020 2070 6173 730a 0a53  .        pass..S
+0000e2e0: 716c 5669 6577 4261 7365 0a7e 7e7e 7e7e  qlViewBase.~~~~~
+0000e2f0: 7e7e 7e7e 7e7e 0a0a 4c69 6b65 2060 6053  ~~~~~~..Like ``S
+0000e300: 716c 4261 7365 6060 2c20 6f6e 6c79 2074  qlBase``, only t
+0000e310: 6865 2060 6053 716c 5669 6577 6060 2069  he ``SqlView`` i
+0000e320: 6e68 6572 6974 7320 7468 6973 2060 6043  nherits this ``C
+0000e330: 6f72 6560 6020 636c 6173 732e 0a0a 3a3a  ore`` class...::
+0000e340: 0a0a 2020 2020 6672 6f6d 2061 6e79 626c  ..    from anybl
+0000e350: 6f6b 2069 6d70 6f72 7420 4465 636c 6172  ok import Declar
+0000e360: 6174 696f 6e73 0a0a 0a20 2020 2040 4465  ations...    @De
+0000e370: 636c 6172 6174 696f 6e73 2e72 6567 6973  clarations.regis
+0000e380: 7465 7228 4465 636c 6172 6174 696f 6e73  ter(Declarations
+0000e390: 2e43 6f72 6529 0a20 2020 2063 6c61 7373  .Core).    class
+0000e3a0: 2053 716c 5669 6577 4261 7365 3a0a 2020   SqlViewBase:.  
+0000e3b0: 2020 2020 2020 7061 7373 0a0a 5175 6572        pass..Quer
+0000e3c0: 790a 7e7e 7e7e 7e0a 0a4f 7665 726c 6f61  y.~~~~~..Overloa
+0000e3d0: 6473 2074 6865 2053 514c 416c 6368 656d  ds the SQLAlchem
+0000e3e0: 7920 6060 5175 6572 7960 6020 636c 6173  y ``Query`` clas
+0000e3f0: 732e 0a0a 3a3a 0a0a 2020 2020 6672 6f6d  s...::..    from
+0000e400: 2061 6e79 626c 6f6b 2069 6d70 6f72 7420   anyblok import 
+0000e410: 4465 636c 6172 6174 696f 6e73 0a0a 0a20  Declarations... 
+0000e420: 2020 2040 4465 636c 6172 6174 696f 6e73     @Declarations
+0000e430: 2e72 6567 6973 7465 7228 4465 636c 6172  .register(Declar
+0000e440: 6174 696f 6e73 2e43 6f72 6529 0a20 2020  ations.Core).   
+0000e450: 2063 6c61 7373 2051 7565 7279 0a20 2020   class Query.   
+0000e460: 2020 2020 2070 6173 730a 0a49 6e73 7472       pass..Instr
+0000e470: 756d 656e 7465 644c 6973 740a 7e7e 7e7e  umentedList.~~~~
+0000e480: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 3a3a  ~~~~~~~~~~~~..::
+0000e490: 0a0a 2020 2020 6672 6f6d 2061 6e79 626c  ..    from anybl
+0000e4a0: 6f6b 2069 6d70 6f72 7420 4465 636c 6172  ok import Declar
+0000e4b0: 6174 696f 6e73 0a0a 0a20 2020 2040 4465  ations...    @De
+0000e4c0: 636c 6172 6174 696f 6e73 2e72 6567 6973  clarations.regis
+0000e4d0: 7465 7228 4465 636c 6172 6174 696f 6e73  ter(Declarations
+0000e4e0: 2e43 6f72 6529 0a20 2020 2063 6c61 7373  .Core).    class
+0000e4f0: 2049 6e73 7472 756d 656e 7465 644c 6973   InstrumentedLis
+0000e500: 740a 2020 2020 2020 2020 7061 7373 0a0a  t.        pass..
+0000e510: 6060 496e 7374 7275 6d65 6e74 6564 4c69  ``InstrumentedLi
+0000e520: 7374 6060 2069 7320 7468 6520 636c 6173  st`` is the clas
+0000e530: 7320 7265 7475 726e 6564 2062 7920 7468  s returned by th
+0000e540: 6520 5175 6572 7920 666f 7220 616c 6c20  e Query for all 
+0000e550: 7468 6520 6c69 7374 2072 6573 756c 740a  the list result.
+0000e560: 6c69 6b65 3a0a 0a2a 2071 7565 7279 2e61  like:..* query.a
+0000e570: 6c6c 2829 0a2a 2072 656c 6174 696f 6e73  ll().* relations
+0000e580: 6869 7020 6c69 7374 2028 4d61 6e79 324d  hip list (Many2M
+0000e590: 616e 792c 204f 6e65 324d 616e 7929 0a0a  any, One2Many)..
+0000e5a0: 4164 6473 2073 6f6d 6520 6665 6174 7572  Adds some featur
+0000e5b0: 6573 206c 696b 6520 6765 7474 696e 6720  es like getting 
+0000e5c0: 6120 7370 6563 6966 6963 2070 726f 7065  a specific prope
+0000e5d0: 7274 7920 6f72 2063 616c 6c69 6e67 2061  rty or calling a
+0000e5e0: 206d 6574 686f 6420 6f6e 2061 6c6c 0a74   method on all.t
+0000e5f0: 6865 2065 6c65 6d65 6e74 7320 6f66 2074  he elements of t
+0000e600: 6865 206c 6973 743a 3a0a 0a20 2020 204d  he list::..    M
+0000e610: 794d 6f64 656c 2e71 7565 7279 2829 2e61  yModel.query().a
+0000e620: 6c6c 2829 2e66 6f6f 2862 6172 290a 0a53  ll().foo(bar)..S
+0000e630: 6861 7269 6e67 2061 2074 6162 6c65 2062  haring a table b
+0000e640: 6574 7765 656e 206d 6f72 6520 7468 616e  etween more than
+0000e650: 206f 6e65 206d 6f64 656c 0a2d 2d2d 2d2d   one model.-----
+0000e660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000e670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000e680: 2d2d 2d2d 2d2d 0a0a 5351 4c41 6c63 6865  ------..SQLAlche
+0000e690: 6d79 2061 6c6c 6f77 7320 7477 6f20 6d65  my allows two me
+0000e6a0: 7468 6f64 7320 746f 2073 6861 7265 2061  thods to share a
+0000e6b0: 2074 6162 6c65 2062 6574 7765 656e 2074   table between t
+0000e6c0: 776f 206f 7220 6d6f 7265 206d 6170 7069  wo or more mappi
+0000e6d0: 6e67 0a63 6c61 7373 3a0a 0a2a 2049 6e68  ng.class:..* Inh
+0000e6e0: 6572 6974 2061 6e20 5351 4c20 4d6f 6465  erit an SQL Mode
+0000e6f0: 6c20 696e 2061 206e 6f6e 2d53 514c 204d  l in a non-SQL M
+0000e700: 6f64 656c 3a3a 0a0a 2020 2020 4072 6567  odel::..    @reg
+0000e710: 6973 7465 7228 4d6f 6465 6c29 0a20 2020  ister(Model).   
+0000e720: 2063 6c61 7373 2054 6573 743a 0a20 2020   class Test:.   
+0000e730: 2020 2020 2069 6420 3d20 496e 7465 6765       id = Intege
+0000e740: 7228 7072 696d 6172 795f 6b65 793d 5472  r(primary_key=Tr
+0000e750: 7565 290a 2020 2020 2020 2020 6e61 6d65  ue).        name
+0000e760: 203d 2053 7472 696e 6728 290a 0a20 2020   = String()..   
+0000e770: 2040 7265 6769 7374 6572 284d 6f64 656c   @register(Model
+0000e780: 290a 2020 2020 636c 6173 7320 5465 7374  ).    class Test
+0000e790: 3228 4d6f 6465 6c2e 5465 7374 293a 0a20  2(Model.Test):. 
+0000e7a0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+0000e7b0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+0000e7c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000e7d0: 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020 2074  ---------..    t
+0000e7e0: 3120 3d20 5465 7374 312e 696e 7365 7274  1 = Test1.insert
+0000e7f0: 286e 616d 653d 2766 6f6f 2729 0a20 2020  (name='foo').   
+0000e800: 2061 7373 6572 7420 5465 7374 322e 7175   assert Test2.qu
+0000e810: 6572 7928 292e 6669 6c74 6572 2854 6573  ery().filter(Tes
+0000e820: 7432 2e69 6420 3d3d 2074 312e 6964 2c0a  t2.id == t1.id,.
+0000e830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e850: 5465 7374 322e 6e61 6d65 203d 3d20 7431  Test2.name == t1
+0000e860: 2e6e 616d 6529 2e63 6f75 6e74 2829 203d  .name).count() =
+0000e870: 3d20 310a 0a2a 2053 6861 7265 2074 6865  = 1..* Share the
+0000e880: 2060 605f 5f74 6162 6c65 5f5f 6060 2e0a   ``__table__``..
+0000e890: 2020 2020 416e 7942 6c6f 6b20 6361 6e6e      AnyBlok cann
+0000e8a0: 6f74 2067 6976 6520 7468 6520 7461 626c  ot give the tabl
+0000e8b0: 6520 6174 2074 6865 2064 6563 6c61 7261  e at the declara
+0000e8c0: 7469 6f6e 2c20 6265 6361 7573 6520 7468  tion, because th
+0000e8d0: 6520 7461 626c 6520 646f 6573 206e 6f74  e table does not
+0000e8e0: 0a20 2020 2065 7869 7374 2079 6574 2e20  .    exist yet. 
+0000e8f0: 4275 7420 6475 7269 6e67 2074 6865 2061  But during the a
+0000e900: 7373 656d 626c 792c 2069 6620 7468 6520  ssembly, if the 
+0000e910: 7461 626c 6520 6578 6973 7473 2061 6e64  table exists and
+0000e920: 2074 6865 206d 6f64 656c 0a20 2020 2068   the model.    h
+0000e930: 6173 2074 6865 206e 616d 6520 6f66 2074  as the name of t
+0000e940: 6869 7320 7461 626c 652c 2041 6e79 426c  his table, AnyBl
+0000e950: 6f6b 2064 6972 6563 746c 7920 6c69 6e6b  ok directly link
+0000e960: 7320 7468 6520 7461 626c 652e 2054 6f0a  s the table. To.
+0000e970: 2020 2020 6465 6669 6e65 2074 6865 2074      define the t
+0000e980: 6162 6c65 2079 6f75 206d 7573 7420 7573  able you must us
+0000e990: 6520 7468 6520 6e61 6d65 6420 6172 6775  e the named argu
+0000e9a0: 6d65 6e74 2060 6074 6162 6c65 6e61 6d65  ment ``tablename
+0000e9b0: 6060 2069 6e20 7468 650a 2020 2020 6060  `` in the.    ``
+0000e9c0: 7265 6769 7374 6572 6060 0a0a 2020 2020  register``..    
+0000e9d0: 3a3a 0a0a 2020 2020 2020 2020 4072 6567  ::..        @reg
+0000e9e0: 6973 7465 7228 4d6f 6465 6c29 0a20 2020  ister(Model).   
+0000e9f0: 2020 2020 2063 6c61 7373 2054 6573 743a       class Test:
+0000ea00: 0a20 2020 2020 2020 2020 2020 2069 6420  .            id 
+0000ea10: 3d20 496e 7465 6765 7228 7072 696d 6172  = Integer(primar
+0000ea20: 795f 6b65 793d 5472 7565 290a 2020 2020  y_key=True).    
+0000ea30: 2020 2020 2020 2020 6e61 6d65 203d 2053          name = S
+0000ea40: 7472 696e 6728 290a 0a20 2020 2020 2020  tring()..       
+0000ea50: 2040 7265 6769 7374 6572 284d 6f64 656c   @register(Model
+0000ea60: 2c20 7461 626c 656e 616d 653d 4d6f 6465  , tablename=Mode
+0000ea70: 6c2e 5465 7374 290a 2020 2020 2020 2020  l.Test).        
+0000ea80: 636c 6173 7320 5465 7374 323a 0a20 2020  class Test2:.   
+0000ea90: 2020 2020 2020 2020 2069 6420 3d20 496e           id = In
+0000eaa0: 7465 6765 7228 7072 696d 6172 795f 6b65  teger(primary_ke
+0000eab0: 793d 5472 7565 290a 2020 2020 2020 2020  y=True).        
+0000eac0: 2020 2020 6e61 6d65 203d 2053 7472 696e      name = Strin
+0000ead0: 6728 290a 0a20 2020 2020 2020 202d 2d2d  g()..        ---
+0000eae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000eaf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000eb00: 2d2d 2d2d 2d0a 0a20 2020 2020 2020 2074  -----..        t
+0000eb10: 3120 3d20 5465 7374 312e 696e 7365 7274  1 = Test1.insert
+0000eb20: 286e 616d 653d 2766 6f6f 2729 0a20 2020  (name='foo').   
+0000eb30: 2020 2020 2061 7373 6572 7420 5465 7374       assert Test
+0000eb40: 322e 7175 6572 7928 292e 6669 6c74 6572  2.query().filter
+0000eb50: 2854 6573 7432 2e69 6420 3d3d 2074 312e  (Test2.id == t1.
+0000eb60: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+0000eb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb80: 2020 2020 2020 2020 5465 7374 322e 6e61          Test2.na
+0000eb90: 6d65 203d 3d20 7431 2e6e 616d 6529 2e63  me == t1.name).c
+0000eba0: 6f75 6e74 2829 203d 3d20 310a 0a20 2020  ount() == 1..   
+0000ebb0: 202e 2e20 7761 726e 696e 673a 3a0a 2020   .. warning::.  
+0000ebc0: 2020 2020 2020 5468 6572 6520 6172 6520        There are 
+0000ebd0: 6e6f 2063 6865 636b 7320 6f6e 2074 6865  no checks on the
+0000ebe0: 2065 7869 7374 696e 6720 636f 6c75 6d6e   existing column
+0000ebf0: 732e 0a0a 5368 6172 696e 6720 6120 7669  s...Sharing a vi
+0000ec00: 6577 2062 6574 7765 656e 206d 6f72 6520  ew between more 
+0000ec10: 7468 616e 206f 6e65 206d 6f64 656c 0a2d  than one model.-
+0000ec20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ec30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ec40: 2d2d 2d2d 2d2d 2d2d 2d0a 0a53 6861 7269  ---------..Shari
+0000ec50: 6e67 2061 2076 6965 7720 6265 7477 6565  ng a view betwee
+0000ec60: 6e20 7477 6f20 4d6f 6465 6c73 2069 7320  n two Models is 
+0000ec70: 7468 6520 6d65 7267 6520 6265 7477 6565  the merge betwee
+0000ec80: 6e3a 0a0a 2a20 4372 6561 7469 6e67 2061  n:..* Creating a
+0000ec90: 2056 6965 7720 4d6f 6465 6c0a 2a20 5368   View Model.* Sh
+0000eca0: 6172 696e 6720 7468 6520 7361 6d65 2074  aring the same t
+0000ecb0: 6162 6c65 2062 6574 7765 656e 206d 6f72  able between mor
+0000ecc0: 6520 7468 616e 206f 6e65 206d 6f64 656c  e than one model
+0000ecd0: 2e0a 0a2e 2e20 7761 726e 696e 673a 3a0a  ..... warning::.
+0000ece0: 0a20 2020 2046 6f72 2074 6865 2076 6965  .    For the vie
+0000ecf0: 7720 796f 7520 6d75 7374 2072 6564 696e  w you must redin
+0000ed00: 6564 2074 6865 2063 6f6c 756d 6e20 696e  ed the column in
+0000ed10: 2074 6865 204d 6f64 656c 2063 6f72 7265   the Model corre
+0000ed20: 7370 6f6e 6469 6e67 2074 6f20 7468 6520  sponding to the 
+0000ed30: 7669 6577 0a20 2020 2077 6974 6820 696e  view.    with in
+0000ed40: 6865 7269 7461 6e63 6520 6f72 2073 696d  heritance or sim
+0000ed50: 706c 6520 5368 6172 6520 6279 2074 6162  ple Share by tab
+0000ed60: 6c65 6e61 6d65 0a0a 5370 6563 6966 6963  lename..Specific
+0000ed70: 2062 6568 6176 696f 7572 0a2d 2d2d 2d2d   behaviour.-----
+0000ed80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a41  -------------..A
+0000ed90: 6e79 426c 6f6b 2069 6d70 6c65 6d65 6e74  nyBlok implement
+0000eda0: 7320 736f 6d65 2066 6163 696c 6974 6965  s some facilitie
+0000edb0: 7320 746f 2068 656c 7020 6465 7665 6c6f  s to help develo
+0000edc0: 7065 7273 0a0a 436f 6c75 6d6e 2065 6e63  pers..Column enc
+0000edd0: 7279 7074 696f 6e0a 7e7e 7e7e 7e7e 7e7e  ryption.~~~~~~~~
+0000ede0: 7e7e 7e7e 7e7e 7e7e 7e0a 0a59 6f75 2063  ~~~~~~~~~..You c
+0000edf0: 616e 2065 6e63 7279 7074 2073 6f6d 6520  an encrypt some 
+0000ee00: 636f 6c75 6d6e 7320 746f 2070 726f 7465  columns to prote
+0000ee10: 6374 2074 6865 6d2e 2054 6865 2070 7974  ct them. The pyt
+0000ee20: 686f 6e20 7061 636b 6167 6520 6372 7970  hon package cryp
+0000ee30: 746f 6772 6170 6879 0a6d 7573 7420 6265  tography.must be
+0000ee40: 2069 6e73 7461 6c6c 6564 3a3a 0a0a 2020   installed::..  
+0000ee50: 2020 7069 7020 696e 7374 616c 6c20 6372    pip install cr
+0000ee60: 7970 746f 6772 6170 6879 0a0a 5573 6520  yptography..Use 
+0000ee70: 7468 6520 656e 6372 7970 745f 6b65 7920  the encrypt_key 
+0000ee80: 6174 7472 6962 7574 6520 6f6e 2074 6865  attribute on the
+0000ee90: 2063 6f6c 756d 6e20 746f 2064 6566 696e   column to defin
+0000eea0: 6520 7468 6520 6b65 7920 6f66 2063 7279  e the key of cry
+0000eeb0: 7074 6f67 7261 7068 793a 3a0a 0a20 2020  ptography::..   
+0000eec0: 2040 7265 6769 7374 6572 284d 6f64 656c   @register(Model
+0000eed0: 290a 2020 2020 636c 6173 7320 4d79 4d6f  ).    class MyMo
+0000eee0: 6465 6c3a 0a0a 2020 2020 2020 2020 2320  del:..        # 
+0000eef0: 6465 6669 6e65 2074 6865 2073 7065 6369  define the speci
+0000ef00: 6669 6320 656e 6372 7970 745f 6b65 790a  fic encrypt_key.
+0000ef10: 2020 2020 2020 2020 656e 6372 7970 745f          encrypt_
+0000ef20: 636f 6c75 6d6e 5f31 203d 2053 7472 696e  column_1 = Strin
+0000ef30: 6728 656e 6372 7970 745f 6b65 793d 2753  g(encrypt_key='S
+0000ef40: 6563 7265 744b 6579 2729 0a0a 2020 2020  ecretKey')..    
+0000ef50: 2020 2020 2320 5573 6520 7468 6520 6465      # Use the de
+0000ef60: 6661 756c 7420 656e 6372 7970 745f 6b65  fault encrypt_ke
+0000ef70: 790a 2020 2020 2020 2020 656e 6372 7970  y.        encryp
+0000ef80: 745f 636f 6c75 6d6e 5f32 203d 2053 7472  t_column_2 = Str
+0000ef90: 696e 6728 656e 6372 7970 745f 6b65 793d  ing(encrypt_key=
+0000efa0: 436f 6e66 6967 7572 6174 696f 6e2e 6765  Configuration.ge
+0000efb0: 7428 2764 6566 6175 6c74 5f65 6e63 7279  t('default_encry
+0000efc0: 7074 5f6b 6579 2729 0a20 2020 2020 2020  pt_key').       
+0000efd0: 2065 6e63 7279 7074 5f63 6f6c 756d 6e5f   encrypt_column_
+0000efe0: 3320 3d20 5374 7269 6e67 2865 6e63 7279  3 = String(encry
+0000eff0: 7074 5f6b 6579 3d54 7275 6529 0a0a 2020  pt_key=True)..  
+0000f000: 2020 2020 2020 2320 5573 6520 7468 6520        # Use the 
+0000f010: 636c 6173 7320 6d65 7468 6f64 2074 6f20  class method to 
+0000f020: 6765 7420 656e 6372 7970 745f 6b65 790a  get encrypt_key.
+0000f030: 2020 2020 2020 2020 656e 6372 7970 745f          encrypt_
+0000f040: 636f 6c75 6d6e 5f31 203d 2053 7472 696e  column_1 = Strin
+0000f050: 6728 656e 6372 7970 745f 6b65 793d 2767  g(encrypt_key='g
+0000f060: 6574 5f65 6e63 7279 7074 5f6b 6579 2729  et_encrypt_key')
+0000f070: 0a0a 2020 2020 2020 2020 4063 6c61 7373  ..        @class
+0000f080: 6d65 7468 6f64 0a20 2020 2020 2020 2064  method.        d
+0000f090: 6566 2067 6574 5f65 6e63 7279 7074 5f6b  ef get_encrypt_k
+0000f0a0: 6579 2863 6c73 293a 0a20 2020 2020 2020  ey(cls):.       
+0000f0b0: 2020 2020 2072 6574 7572 6e20 2753 6563       return 'Sec
+0000f0c0: 7265 744b 6579 270a 0a54 6865 2065 6e63  retKey'..The enc
+0000f0d0: 7279 7074 696f 6e20 776f 726b 7320 666f  ryption works fo
+0000f0e0: 7220 616e 7920 436f 6c75 6d6e 732e 0a0a  r any Columns...
+0000f0f0: 456e 7669 726f 6e6d 656e 740a 7e7e 7e7e  Environment.~~~~
+0000f100: 7e7e 7e7e 7e7e 7e0a 0a54 6865 2045 6e76  ~~~~~~~..The Env
+0000f110: 6972 6f6e 6d65 6e74 2063 6f6e 7461 696e  ironment contain
+0000f120: 7320 6e6f 6e20 7065 7273 6973 7465 6e74  s non persistent
+0000f130: 2063 6f6e 7465 7874 7561 6c20 7661 7269   contextual vari
+0000f140: 6162 6c65 732e 2042 790a 6465 6661 756c  ables. By.defaul
+0000f150: 742c 2069 7420 6973 2073 746f 7265 6420  t, it is stored 
+0000f160: 696e 2074 6865 2063 7572 7265 6e74 203a  in the current :
+0000f170: 636c 6173 733a 6054 6872 6561 6460 206f  class:`Thread` o
+0000f180: 626a 6563 742c 2062 7574 2074 6861 740a  bject, but that.
+0000f190: 6973 2061 6d65 6e64 6162 6c65 2028 7365  is amendable (se
+0000f1a0: 6520 3a72 6566 3a60 656e 7669 726f 6e6d  e :ref:`environm
+0000f1b0: 656e 745f 7479 7065 7360 292e 0a0a 5573  ent_types`)...Us
+0000f1c0: 6520 7468 6520 6375 7272 656e 7420 656e  e the current en
+0000f1d0: 7669 726f 6e6d 656e 740a 2b2b 2b2b 2b2b  vironment.++++++
+0000f1e0: 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b  ++++++++++++++++
+0000f1f0: 2b2b 2b2b 2b0a 0a54 6865 2065 6e76 6972  +++++..The envir
+0000f200: 6f6e 6d65 6e74 2063 616e 2062 6520 7573  onment can be us
+0000f210: 6564 2066 726f 6d20 7768 6572 6565 7665  ed from whereeve
+0000f220: 7220 696e 2074 6865 2063 6f64 652e 0a0a  r in the code...
+0000f230: 4765 6e65 7269 6320 7573 650a 2f2f 2f2f  Generic use.////
+0000f240: 2f2f 2f2f 2f2f 2f0a 0a54 6f20 6765 7420  ///////..To get 
+0000f250: 6f72 2073 6574 2076 6172 6961 626c 6520  or set variable 
+0000f260: 696e 2065 6e76 6972 6f6e 6d65 6e74 2c20  in environment, 
+0000f270: 796f 7520 6d75 7374 2069 6d70 6f72 7420  you must import 
+0000f280: 7468 650a 6060 456e 7669 726f 6e6d 656e  the.``Environmen
+0000f290: 744d 616e 6167 6572 6060 3a3a 0a0a 2020  tManager``::..  
+0000f2a0: 2020 6672 6f6d 2061 6e79 626c 6f6b 2e65    from anyblok.e
+0000f2b0: 6e76 6972 6f6e 6d65 6e74 2069 6d70 6f72  nvironment impor
+0000f2c0: 7420 456e 7669 726f 6e6d 656e 744d 616e  t EnvironmentMan
+0000f2d0: 6167 6572 0a0a 5365 7420 6120 7661 7269  ager..Set a vari
+0000f2e0: 6162 6c65 3a3a 0a0a 2020 2020 456e 7669  able::..    Envi
+0000f2f0: 726f 6e6d 656e 744d 616e 6167 6572 2e73  ronmentManager.s
+0000f300: 6574 2827 6d79 2076 6172 6961 626c 6520  et('my variable 
+0000f310: 6e61 6d65 272c 2073 6f6d 655f 7661 6c75  name', some_valu
+0000f320: 6529 0a0a 4765 7420 6120 7661 7269 6162  e)..Get a variab
+0000f330: 6c65 3a3a 0a0a 2020 2020 456e 7669 726f  le::..    Enviro
+0000f340: 6e6d 656e 744d 616e 6167 6572 2e67 6574  nmentManager.get
+0000f350: 2827 6d79 2076 6172 6961 626c 6520 6e61  ('my variable na
+0000f360: 6d65 272c 2064 6566 6175 6c74 3d73 6f6d  me', default=som
+0000f370: 655f 6465 6661 756c 7429 0a0a 5573 6520  e_default)..Use 
+0000f380: 6672 6f6d 2061 2060 604d 6f64 656c 6060  from a ``Model``
+0000f390: 0a2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  .///////////////
+0000f3a0: 2f2f 2f2f 2f0a 0a41 2063 6c61 7373 2d6c  /////..A class-l
+0000f3b0: 6576 656c 2061 7474 7269 6275 7465 2069  evel attribute i
+0000f3c0: 7320 7072 6573 656e 7420 6f6e 2061 6c6c  s present on all
+0000f3d0: 204d 6f64 656c 2063 6c61 7373 6573 2074   Model classes t
+0000f3e0: 6f20 6163 6365 7373 2074 6865 0a45 6e76  o access the.Env
+0000f3f0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+0000f400: 6573 2063 6f6e 7665 6e69 656e 746c 792e  es conveniently.
+0000f410: 0a0a 546f 2067 7261 6220 7468 6520 456e  ..To grab the En
+0000f420: 7669 726f 6e6d 656e 744d 616e 6167 6572  vironmentManager
+0000f430: 2066 726f 6d20 6120 6060 4d6f 6465 6c60   from a ``Model`
+0000f440: 6020 6d65 7468 6f64 2c20 6a75 7374 2075  ` method, just u
+0000f450: 7365 0a60 6073 656c 662e 456e 7660 602e  se.``self.Env``.
+0000f460: 2046 6f72 2061 2063 6c61 7373 6d65 7468   For a classmeth
+0000f470: 6f64 2c20 7468 6174 2077 6f75 6c64 2062  od, that would b
+0000f480: 6520 6173 2069 6e3a 3a0a 0a20 2020 2040  e as in::..    @
+0000f490: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+0000f4a0: 6465 6620 6d79 636c 736d 6574 6828 636c  def myclsmeth(cl
+0000f4b0: 7329 3a0a 2020 2020 2020 656e 7620 3d20  s):.      env = 
+0000f4c0: 636c 732e 456e 760a 2020 2020 2020 282e  cls.Env.      (.
+0000f4d0: 2e2e 290a 0a54 6865 6e2c 2069 7427 7320  ..)..Then, it's 
+0000f4e0: 6561 7379 2074 6f20 6765 7420 616e 6420  easy to get and 
+0000f4f0: 7365 7420 7661 7269 6162 6c65 732e 2048  set variables. H
+0000f500: 6572 6527 7320 616e 2065 7861 6d70 6c65  ere's an example
+0000f510: 2066 726f 6d20 6120 4d6f 6465 6c0a 696e   from a Model.in
+0000f520: 7374 616e 6365 206d 6574 686f 643a 3a0a  stance method::.
+0000f530: 0a20 2020 2073 656c 662e 456e 762e 7365  .    self.Env.se
+0000f540: 7428 276d 7920 7661 7269 6162 6c65 206e  t('my variable n
+0000f550: 616d 6527 2c20 736f 6d65 5f76 616c 7565  ame', some_value
+0000f560: 290a 2020 2020 7365 6c66 2e45 6e76 2e67  ).    self.Env.g
+0000f570: 6574 2827 6d79 2076 6172 6961 626c 6520  et('my variable 
+0000f580: 6e61 6d65 272c 2064 6566 6175 6c74 3d73  name', default=s
+0000f590: 6f6d 655f 6465 6661 756c 745f 7661 6c75  ome_default_valu
+0000f5a0: 6529 0a0a 2e2e 206e 6f74 653a 3a20 7468  e).... note:: th
+0000f5b0: 6520 6060 456e 7660 6020 6174 7472 6962  e ``Env`` attrib
+0000f5c0: 7574 6520 6973 2061 6374 7561 6c6c 7920  ute is actually 
+0000f5d0: 7365 7420 696e 0a20 2020 2020 2020 2020  set in.         
+0000f5e0: 2060 6072 6567 6973 7472 792e 7265 6769   ``registry.regi
+0000f5f0: 7374 7279 5f62 6173 6560 602c 2077 6869  stry_base``, whi
+0000f600: 6368 2069 7320 6120 636c 6173 7320 6479  ch is a class dy
+0000f610: 6e61 6d69 6361 6c6c 790a 2020 2020 2020  namically.      
+0000f620: 2020 2020 6765 6e65 7261 7465 6420 6174      generated at
+0000f630: 2072 6567 6973 7472 7920 6372 6561 7469   registry creati
+0000f640: 6f6e 2c20 616e 6420 6f66 2077 6869 6368  on, and of which
+0000f650: 2061 6c6c 2061 7373 656d 626c 6564 0a20   all assembled. 
+0000f660: 2020 2020 2020 2020 2063 6c61 7373 6573           classes
+0000f670: 2073 746f 7265 6420 696e 2074 6865 2072   stored in the r
+0000f680: 6567 6973 7472 7920 696e 6865 7269 742e  egistry inherit.
+0000f690: 0a0a 2e2e 205f 656e 7669 726f 6e6d 656e  .... _environmen
+0000f6a0: 745f 7479 7065 733a 0a0a 4465 6669 6e65  t_types:..Define
+0000f6b0: 2061 206e 6577 2065 6e76 6972 6f6e 6d65   a new environme
+0000f6c0: 6e74 2074 7970 650a 2b2b 2b2b 2b2b 2b2b  nt type.++++++++
+0000f6d0: 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b  ++++++++++++++++
+0000f6e0: 2b2b 2b2b 2b0a 0a49 6620 796f 7520 646f  +++++..If you do
+0000f6f0: 206e 6f74 2077 616e 7420 746f 2073 746f   not want to sto
+0000f700: 636b 2074 6865 2065 6e76 6972 6f6e 6d65  ck the environme
+0000f710: 6e74 2069 6e20 7468 6520 6060 5468 7265  nt in the ``Thre
+0000f720: 6164 6060 2c20 796f 7520 206d 7573 740a  ad``, you  must.
+0000f730: 696d 706c 656d 656e 7420 6120 6e65 7720  implement a new 
+0000f740: 7479 7065 206f 6620 656e 7669 726f 6e6d  type of environm
+0000f750: 656e 742e 0a0a 5468 6973 2074 7970 6520  ent...This type 
+0000f760: 6973 2061 2073 696d 706c 6520 636c 6173  is a simple clas
+0000f770: 7320 7768 6963 6820 6861 7665 2074 6865  s which have the
+0000f780: 7365 7320 636c 6173 7320 6d65 7468 6f64  ses class method
+0000f790: 733a 0a0a 2a20 7363 6f70 6564 5f66 756e  s:..* scoped_fun
+0000f7a0: 6374 696f 6e5f 666f 725f 7365 7373 696f  ction_for_sessio
+0000f7b0: 6e0a 2a20 7365 7474 6572 0a2a 2067 6574  n.* setter.* get
+0000f7c0: 7465 720a 0a3a 3a0a 0a20 2020 204d 7945  ter..::..    MyE
+0000f7d0: 6e76 6972 6f6e 6d65 6e74 436c 6173 733a  nvironmentClass:
+0000f7e0: 0a0a 2020 2020 2020 2020 4063 6c61 7373  ..        @class
+0000f7f0: 6d65 7468 6f64 0a20 2020 2020 2020 2064  method.        d
+0000f800: 6566 2073 636f 7065 645f 6675 6e63 7469  ef scoped_functi
+0000f810: 6f6e 5f66 6f72 5f73 6573 7369 6f6e 2863  on_for_session(c
+0000f820: 6c73 293a 0a20 2020 2020 2020 2020 2020  ls):.           
+0000f830: 202e 2e2e 0a0a 2020 2020 2020 2020 4063   .....        @c
+0000f840: 6c61 7373 6d65 7468 6f64 0a20 2020 2020  lassmethod.     
+0000f850: 2020 2064 6566 2073 6574 7465 7228 636c     def setter(cl
+0000f860: 732c 206b 6579 2c20 7661 6c75 6529 3a0a  s, key, value):.
+0000f870: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
+0000f880: 0a20 2020 2020 2020 2040 636c 6173 736d  .        @classm
+0000f890: 6574 686f 640a 2020 2020 2020 2020 6465  ethod.        de
+0000f8a0: 6620 6765 7474 6572 2863 6c73 2c20 6b65  f getter(cls, ke
+0000f8b0: 792c 2064 6566 6175 6c74 293a 0a20 2020  y, default):.   
+0000f8c0: 2020 2020 2020 2020 202e 2e2e 0a20 2020           ....   
+0000f8d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000f8e0: 7661 6c75 650a 0a44 6563 6c61 7265 2079  value..Declare y
+0000f8f0: 6f75 7220 636c 6173 7320 6173 2074 6865  our class as the
+0000f900: 2045 6e76 6972 6f6e 6d65 6e74 2063 6c61   Environment cla
+0000f910: 7373 3a3a 0a0a 2020 2020 456e 7669 726f  ss::..    Enviro
+0000f920: 6e6d 656e 744d 616e 6167 6572 2e64 6566  nmentManager.def
+0000f930: 696e 655f 656e 7669 726f 6e6d 656e 745f  ine_environment_
+0000f940: 636c 7328 4d79 456e 7669 726f 6e6d 656e  cls(MyEnvironmen
+0000f950: 7443 6c61 7373 290a 0a0a 5468 6520 636c  tClass)...The cl
+0000f960: 6173 736d 6574 686f 6420 6060 7363 6f70  assmethod ``scop
+0000f970: 6564 5f66 756e 6374 696f 6e5f 666f 725f  ed_function_for_
+0000f980: 7365 7373 696f 6e60 6020 6973 2070 6173  session`` is pas
+0000f990: 7365 6420 6174 2053 514c 416c 6368 656d  sed at SQLAlchem
+0000f9a0: 790a 6060 7363 6f70 6564 5f73 6573 7369  y.``scoped_sessi
+0000f9b0: 6f6e 6060 2066 756e 6374 696f 6e20 6073  on`` function `s
+0000f9c0: 6565 203c 6874 7470 3a2f 2f64 6f63 732e  ee <http://docs.
+0000f9d0: 7371 6c61 6c63 6865 6d79 2e6f 7267 2f65  sqlalchemy.org/e
+0000f9e0: 6e2f 7265 6c5f 305f 392f 6f72 6d2f 0a63  n/rel_0_9/orm/.c
+0000f9f0: 6f6e 7465 7874 7561 6c2e 6874 6d6c 2363  ontextual.html#c
+0000fa00: 6f6e 7465 7874 7561 6c2d 7468 7265 6164  ontextual-thread
+0000fa10: 2d6c 6f63 616c 2d73 6573 7369 6f6e 733e  -local-sessions>
+0000fa20: 605f 0a0a 0a47 6574 2074 6865 2072 6567  `_...Get the reg
+0000fa30: 6973 7472 790a 7e7e 7e7e 7e7e 7e7e 7e7e  istry.~~~~~~~~~~
+0000fa40: 7e7e 7e7e 7e7e 0a0a 596f 7520 6361 6e20  ~~~~~~..You can 
+0000fa50: 6765 7420 7468 6520 7265 6769 7374 7279  get the registry
+0000fa60: 2069 6e20 616e 7920 6d65 7468 6f64 206f   in any method o
+0000fa70: 6620 4d6f 6465 6c73 2077 6974 6820 7468  f Models with th
+0000fa80: 6520 6174 7472 6962 7574 6520 2a2a 616e  e attribute **an
+0000fa90: 7962 6c6f 6b2a 2a3a 3a0a 0a20 2020 204d  yblok**::..    M
+0000faa0: 6f64 656c 203d 2073 656c 662e 616e 7962  odel = self.anyb
+0000fab0: 6c6f 6b2e 5379 7374 656d 2e4d 6f64 656c  lok.System.Model
+0000fac0: 0a20 2020 2061 7373 6572 7420 4d6f 6465  .    assert Mode
+0000fad0: 6c2e 5f5f 7265 6769 7374 7279 5f6e 616d  l.__registry_nam
+0000fae0: 655f 5f20 3d3d 2027 4d6f 6465 6c2e 5379  e__ == 'Model.Sy
+0000faf0: 7374 656d 2e42 6c6f 6b27 0a0a 2e2e 2077  stem.Blok'.... w
+0000fb00: 6172 6e69 6e67 3a3a 0a0a 2020 2053 696e  arning::..   Sin
+0000fb10: 6365 2076 6572 7369 6f6e 2031 2e31 2e30  ce version 1.1.0
+0000fb20: 206f 6620 416e 7942 6c6f 6b20 7468 6520   of AnyBlok the 
+0000fb30: 6174 7472 6962 7574 6520 2a2a 7265 6769  attribute **regi
+0000fb40: 7374 7279 2a2a 2069 7320 7265 6e61 6d65  stry** is rename
+0000fb50: 6420 2a2a 616e 7962 6c6f 6b2a 2a0a 0a0a  d **anyblok**...
+0000fb60: 4361 6368 650a 7e7e 7e7e 7e0a 0a54 6865  Cache.~~~~~..The
+0000fb70: 2063 6163 6865 2061 6c6c 6f77 7320 746f   cache allows to
+0000fb80: 2063 616c 6c20 6120 6d65 7468 6f64 206d   call a method m
+0000fb90: 6f72 6520 7468 616e 206f 6e63 6520 7769  ore than once wi
+0000fba0: 7468 6f75 7420 6861 7669 6e67 2061 6e79  thout having any
+0000fbb0: 2064 6966 6665 7265 6e63 650a 696e 2074   difference.in t
+0000fbc0: 6865 2072 6573 756c 742e 2042 7574 2074  he result. But t
+0000fbd0: 6865 2063 6163 6865 206d 7573 7420 616c  he cache must al
+0000fbe0: 736f 2064 6570 656e 6420 6f6e 2074 6865  so depend on the
+0000fbf0: 2072 6567 6973 7472 7920 6461 7461 6261   registry databa
+0000fc00: 7365 2061 6e64 2074 6865 0a6d 6f64 656c  se and the.model
+0000fc10: 2e20 5468 6520 6361 6368 6520 6f66 2061  . The cache of a
+0000fc20: 6e79 626c 6f6b 2063 616e 2062 6520 7075  nyblok can be pu
+0000fc30: 7420 6f6e 2061 204d 6f64 656c 2c20 6120  t on a Model, a 
+0000fc40: 436f 7265 206f 7220 6120 4d69 7869 6e20  Core or a Mixin 
+0000fc50: 6d65 7468 6f64 2e20 4966 0a74 6865 2063  method. If.the c
+0000fc60: 6163 6865 2069 7320 6f6e 2061 2043 6f72  ache is on a Cor
+0000fc70: 6520 6f72 2061 204d 6978 696e 2074 6865  e or a Mixin the
+0000fc80: 6e20 7468 6520 7573 6563 6173 6520 6465  n the usecase de
+0000fc90: 7065 6e64 7320 6f6e 2074 6865 2072 6567  pends on the reg
+0000fca0: 6973 7472 7920 6e61 6d65 0a6f 6620 7468  istry name.of th
+0000fcb0: 6520 6173 7365 6d62 6c65 6420 6d6f 6465  e assembled mode
+0000fcc0: 6c2e 0a0a 5573 6520 6060 6361 6368 6560  l...Use ``cache`
+0000fcd0: 6020 6f72 2060 6063 6c61 7373 6d65 7468  ` or ``classmeth
+0000fce0: 6f64 5f63 6163 6865 6060 2074 6f20 6170  od_cache`` to ap
+0000fcf0: 706c 7920 6120 6361 6368 6520 6f6e 2061  ply a cache on a
+0000fd00: 206d 6574 686f 643a 3a0a 0a20 2020 2066   method::..    f
+0000fd10: 726f 6d20 616e 7962 6c6f 6b2e 6465 636c  rom anyblok.decl
+0000fd20: 6172 6174 696f 6e73 2069 6d70 6f72 7420  arations import 
+0000fd30: 6361 6368 652c 2063 6c61 7373 6d65 7468  cache, classmeth
+0000fd40: 6f64 5f63 6163 6865 0a0a 2e2e 2077 6172  od_cache.... war
+0000fd50: 6e69 6e67 3a3a 0a0a 2020 2020 6060 6361  ning::..    ``ca
+0000fd60: 6368 6560 6020 6465 7065 6e64 206f 6620  che`` depend of 
+0000fd70: 7468 6520 696e 7374 616e 6365 2c20 6966  the instance, if
+0000fd80: 2079 6f75 2077 616e 7420 6164 6420 6120   you want add a 
+0000fd90: 6361 6368 6520 666f 720a 2020 2020 616e  cache for.    an
+0000fda0: 7920 696e 7374 616e 6365 2079 6f75 206d  y instance you m
+0000fdb0: 7573 7420 7573 6520 6060 636c 6173 736d  ust use ``classm
+0000fdc0: 6574 686f 645f 6361 6368 6560 600a 0a43  ethod_cache``..C
+0000fdd0: 6163 6865 2074 6865 206d 6574 686f 6420  ache the method 
+0000fde0: 6f66 2061 204d 6f64 656c 3a3a 0a0a 2020  of a Model::..  
+0000fdf0: 2020 4072 6567 6973 7465 7228 4d6f 6465    @register(Mode
+0000fe00: 6c29 0a20 2020 2063 6c61 7373 2046 6f6f  l).    class Foo
+0000fe10: 3a0a 0a20 2020 2020 2020 2040 636c 6173  :..        @clas
+0000fe20: 736d 6574 686f 645f 6361 6368 6528 290a  smethod_cache().
+0000fe30: 2020 2020 2020 2020 6465 6620 6261 7228          def bar(
+0000fe40: 636c 7329 3a0a 2020 2020 2020 2020 2020  cls):.          
+0000fe50: 2020 696d 706f 7274 2072 616e 646f 6d0a    import random.
+0000fe60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000fe70: 726e 2072 616e 646f 6d2e 7261 6e64 6f6d  rn random.random
+0000fe80: 2829 0a0a 0a20 2020 202d 2d2d 2d2d 2d2d  ()...    -------
+0000fe90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000fea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000feb0: 2d2d 0a0a 2020 2020 6173 7365 7274 2046  --..    assert F
+0000fec0: 6f6f 2e62 6172 2829 203d 3d20 466f 6f2e  oo.bar() == Foo.
+0000fed0: 6261 7228 290a 0a0a 4361 6368 6520 7468  bar()...Cache th
+0000fee0: 6520 6d65 7468 6f64 2063 6f6d 696e 6720  e method coming 
+0000fef0: 6672 6f6d 2061 204d 6978 696e 3a3a 0a0a  from a Mixin::..
+0000ff00: 2020 2020 4072 6567 6973 7465 7228 4d69      @register(Mi
+0000ff10: 7869 6e29 0a20 2020 2063 6c61 7373 204d  xin).    class M
+0000ff20: 466f 6f3a 0a0a 2020 2020 2020 2020 4063  Foo:..        @c
+0000ff30: 6c61 7373 6d65 7468 6f64 5f63 6163 6865  lassmethod_cache
+0000ff40: 2829 0a20 2020 2020 2020 2064 6566 2062  ().        def b
+0000ff50: 6172 2863 6c73 293a 0a20 2020 2020 2020  ar(cls):.       
+0000ff60: 2020 2020 2069 6d70 6f72 7420 7261 6e64       import rand
+0000ff70: 6f6d 0a20 2020 2020 2020 2020 2020 2072  om.            r
+0000ff80: 6574 7572 6e20 7261 6e64 6f6d 2e72 616e  eturn random.ran
+0000ff90: 646f 6d28 290a 0a20 2020 2040 7265 6769  dom()..    @regi
+0000ffa0: 7374 6572 284d 6f64 656c 290a 2020 2020  ster(Model).    
+0000ffb0: 636c 6173 7320 466f 6f28 4d69 7869 6e2e  class Foo(Mixin.
+0000ffc0: 4d46 6f6f 293a 0a20 2020 2020 2020 2070  MFoo):.        p
+0000ffd0: 6173 730a 0a20 2020 2040 7265 6769 7374  ass..    @regist
+0000ffe0: 6572 284d 6f64 656c 290a 2020 2020 636c  er(Model).    cl
+0000fff0: 6173 7320 466f 6f32 284d 6978 696e 2e4d  ass Foo2(Mixin.M
+00010000: 466f 6f29 3a0a 2020 2020 2020 2020 7061  Foo):.        pa
+00010010: 7373 0a0a 0a20 2020 202d 2d2d 2d2d 2d2d  ss...    -------
+00010020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00010030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00010040: 2d2d 0a0a 2020 2020 6173 7365 7274 2046  --..    assert F
+00010050: 6f6f 2e62 6172 2829 203d 3d20 466f 6f2e  oo.bar() == Foo.
+00010060: 6261 7228 290a 2020 2020 6173 7365 7274  bar().    assert
+00010070: 2046 6f6f 322e 6261 7228 2920 3d3d 2046   Foo2.bar() == F
+00010080: 6f6f 322e 6261 7228 290a 2020 2020 6173  oo2.bar().    as
+00010090: 7365 7274 2046 6f6f 2e62 6172 2829 2021  sert Foo.bar() !
+000100a0: 3d20 466f 6f32 2e62 6172 2829 0a0a 0a43  = Foo2.bar()...C
+000100b0: 6163 6865 2074 6865 206d 6574 686f 6420  ache the method 
+000100c0: 636f 6d69 6e67 2066 726f 6d20 6120 4d69  coming from a Mi
+000100d0: 7869 6e3a 3a0a 0a20 2020 2040 7265 6769  xin::..    @regi
+000100e0: 7374 6572 2843 6f72 6529 0a20 2020 2063  ster(Core).    c
+000100f0: 6c61 7373 2042 6173 650a 0a20 2020 2020  lass Base..     
+00010100: 2020 2040 636c 6173 736d 6574 686f 645f     @classmethod_
+00010110: 6361 6368 6528 290a 2020 2020 2020 2020  cache().        
+00010120: 6465 6620 6261 7228 636c 7329 3a0a 2020  def bar(cls):.  
+00010130: 2020 2020 2020 2020 2020 696d 706f 7274            import
+00010140: 2072 616e 646f 6d0a 2020 2020 2020 2020   random.        
+00010150: 2020 2020 7265 7475 726e 2072 616e 646f      return rando
+00010160: 6d2e 7261 6e64 6f6d 2829 0a0a 2020 2020  m.random()..    
+00010170: 4072 6567 6973 7465 7228 4d6f 6465 6c29  @register(Model)
+00010180: 0a20 2020 2063 6c61 7373 2046 6f6f 3a0a  .    class Foo:.
+00010190: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000101a0: 2020 4072 6567 6973 7465 7228 4d6f 6465    @register(Mode
+000101b0: 6c29 0a20 2020 2063 6c61 7373 2046 6f6f  l).    class Foo
+000101c0: 323a 0a20 2020 2020 2020 2070 6173 730a  2:.        pass.
+000101d0: 0a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  ..    ----------
+000101e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000101f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+00010200: 0a20 2020 2061 7373 6572 7420 466f 6f2e  .    assert Foo.
+00010210: 6261 7228 2920 3d3d 2046 6f6f 2e62 6172  bar() == Foo.bar
+00010220: 2829 0a20 2020 2061 7373 6572 7420 466f  ().    assert Fo
+00010230: 6f32 2e62 6172 2829 203d 3d20 466f 6f32  o2.bar() == Foo2
+00010240: 2e62 6172 2829 0a20 2020 2061 7373 6572  .bar().    asser
+00010250: 7420 466f 6f2e 6261 7228 2920 213d 2046  t Foo.bar() != F
+00010260: 6f6f 322e 6261 7228 290a 0a45 7665 6e74  oo2.bar()..Event
+00010270: 0a7e 7e7e 7e7e 0a0a 5369 6d70 6c65 2069  .~~~~~..Simple i
+00010280: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
+00010290: 2061 2073 796e 6368 726f 6e6f 7573 2060   a synchronous `
+000102a0: 6065 7665 6e74 6060 2066 6f72 2041 6e79  `event`` for Any
+000102b0: 426c 6f6b 206f 7220 5351 4c41 6c63 6865  Blok or SQLAlche
+000102c0: 6d79 3a3a 0a0a 0a20 2020 2040 7265 6769  my::...    @regi
+000102d0: 7374 6572 284d 6f64 656c 290a 2020 2020  ster(Model).    
+000102e0: 636c 6173 7320 4576 656e 743a 0a20 2020  class Event:.   
+000102f0: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
+00010300: 7265 6769 7374 6572 284d 6f64 656c 290a  register(Model).
+00010310: 2020 2020 636c 6173 7320 5465 7374 3a0a      class Test:.
+00010320: 0a20 2020 2020 2020 2020 2020 2078 203d  .            x =
+00010330: 2030 0a0a 2020 2020 2020 2020 2020 2020   0..            
+00010340: 406c 6973 7465 6e28 4d6f 6465 6c2e 4576  @listen(Model.Ev
+00010350: 656e 742c 2027 6669 7265 6576 656e 7427  ent, 'fireevent'
+00010360: 290a 2020 2020 2020 2020 2020 2020 6465  ).            de
+00010370: 6620 6d79 5f65 7665 6e74 2863 6c73 2c20  f my_event(cls, 
+00010380: 613d 312c 2062 3d31 293a 0a20 2020 2020  a=1, b=1):.     
+00010390: 2020 2020 2020 2020 2020 2063 6c73 2e78             cls.x
+000103a0: 203d 2061 202a 2062 0a0a 2020 2020 2d2d   = a * b..    --
+000103b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000103c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000103d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020  -----------..   
+000103e0: 2072 6567 6973 7472 792e 4576 656e 742e   registry.Event.
+000103f0: 6669 7265 2827 6669 7265 6576 656e 7427  fire('fireevent'
+00010400: 2c20 613d 3229 0a20 2020 2061 7373 6572  , a=2).    asser
+00010410: 7420 7265 6769 7374 7279 2e54 6573 742e  t registry.Test.
+00010420: 7820 3d3d 2032 0a0a 2e2e 206e 6f74 653a  x == 2.... note:
+00010430: 3a0a 0a20 2020 2054 6865 2064 6563 6f72  :..    The decor
+00010440: 6174 6564 206d 6574 686f 6420 6973 2073  ated method is s
+00010450: 6565 6e20 6173 2061 2063 6c61 7373 6d65  een as a classme
+00010460: 7468 6f64 0a0a 5468 6973 2041 5049 2067  thod..This API g
+00010470: 6976 6573 3a0a 0a2a 2061 2064 6563 6f72  ives:..* a decor
+00010480: 6174 6f72 2060 606c 6973 7465 6e60 6020  ator ``listen`` 
+00010490: 7768 6963 6820 6269 6e64 7320 7468 6520  which binds the 
+000104a0: 6465 636f 7261 7465 6420 6d65 7468 6f64  decorated method
+000104b0: 2074 6f20 7468 6520 6576 656e 742e 0a2a   to the event..*
+000104c0: 2060 6066 6972 6560 6020 6d65 7468 6f64   ``fire`` method
+000104d0: 2077 6974 6820 7468 6520 666f 6c6c 6f77   with the follow
+000104e0: 696e 6720 7061 7261 6d65 7465 7273 2028  ing parameters (
+000104f0: 4f6e 6c79 2066 6f72 2041 6e79 426c 6f6b  Only for AnyBlok
+00010500: 2065 7665 6e74 293a 0a20 2020 202d 2060   event):.    - `
+00010510: 6065 7665 6e74 6060 3a20 7374 7269 6e67  `event``: string
+00010520: 206e 616d 6520 6f66 2074 6865 2065 7665   name of the eve
+00010530: 6e74 0a20 2020 202d 2060 602a 6172 6773  nt.    - ``*args
+00010540: 6060 3a20 706f 7369 7469 6f6e 6e61 6c20  ``: positionnal 
+00010550: 6172 6775 6d65 6e74 7320 746f 2070 6173  arguments to pas
+00010560: 7320 6174 7420 7468 6520 6465 636f 7261  s att the decora
+00010570: 7465 6420 6d65 7468 6f64 0a20 2020 202d  ted method.    -
+00010580: 2060 602a 2a6b 7761 7267 7360 603a 206e   ``**kwargs``: n
+00010590: 616d 6564 2061 7267 756d 656e 7420 746f  amed argument to
+000105a0: 2070 6173 7320 6174 2074 6865 2064 6563   pass at the dec
+000105b0: 6f72 6174 6564 206d 6574 686f 640a 0a49  orated method..I
+000105c0: 7420 6973 2070 6f73 7369 626c 6520 746f  t is possible to
+000105d0: 206f 7665 726c 6f61 6420 616e 2065 7869   overload an exi
+000105e0: 7374 696e 6720 6576 656e 7420 6c69 7374  sting event list
+000105f0: 656e 6572 2c20 6a75 7374 2062 7920 6f76  ener, just by ov
+00010600: 6572 6c6f 6164 696e 6720 7468 650a 6465  erloading the.de
+00010610: 636f 7261 7465 6420 6d65 7468 6f64 3a3a  corated method::
+00010620: 0a0a 2020 2020 4072 6567 6973 7465 7228  ..    @register(
+00010630: 4d6f 6465 6c29 0a20 2020 2063 6c61 7373  Model).    class
+00010640: 2054 6573 743a 0a0a 2020 2020 2020 2020   Test:..        
+00010650: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+00010660: 2020 2020 2064 6566 206d 795f 6576 656e       def my_even
+00010670: 7428 636c 732c 202a 2a6b 7761 7267 293a  t(cls, **kwarg):
+00010680: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00010690: 203d 2073 7570 6572 2854 6573 742c 2063   = super(Test, c
+000106a0: 6c73 292e 6d79 5f65 7665 6e74 282a 2a6b  ls).my_event(**k
+000106b0: 7761 7267 7329 0a20 2020 2020 2020 2020  wargs).         
+000106c0: 2020 2072 6574 7572 6e20 7265 7320 2a20     return res * 
+000106d0: 320a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  2..    ---------
+000106e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000106f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00010700: 2d2d 2d2d 0a0a 2020 2020 7265 6769 7374  ----..    regist
+00010710: 7279 2e45 7665 6e74 2e66 6972 6528 2766  ry.Event.fire('f
+00010720: 6972 6565 7665 6e74 272c 2061 3d32 290a  ireevent', a=2).
+00010730: 2020 2020 6173 7365 7274 2072 6567 6973      assert regis
+00010740: 7472 792e 5465 7374 2e78 203d 3d20 340a  try.Test.x == 4.
+00010750: 0a2e 2e20 7761 726e 696e 673a 3a0a 0a20  ... warning::.. 
+00010760: 2020 2054 6865 206f 7665 726c 6f61 6420     The overload 
+00010770: 646f 6573 206e 6f74 2074 616b 6520 7468  does not take th
+00010780: 6520 6060 6c69 7374 656e 6060 2064 6563  e ``listen`` dec
+00010790: 6f72 6174 6f72 2062 7574 2074 6865 0a20  orator but the. 
+000107a0: 2020 2063 6c61 7373 6d65 7468 6f64 2064     classmethod d
+000107b0: 6563 6f72 6174 6f72 2c20 6265 6361 7573  ecorator, becaus
+000107c0: 6520 7468 6520 6d65 7468 6f64 206e 616d  e the method nam
+000107d0: 6520 6973 2061 6c72 6561 6479 2073 6565  e is already see
+000107e0: 6e20 6173 2061 6e0a 2020 2020 6576 656e  n as an.    even
+000107f0: 7420 6c69 7374 656e 6572 0a0a 536f 6d65  t listener..Some
+00010800: 206f 6620 7468 6520 4174 7472 6962 7574   of the Attribut
+00010810: 6520 6576 656e 7473 206f 6620 7468 6520  e events of the 
+00010820: 4d61 7070 6572 2065 7665 6e74 7320 6172  Mapper events ar
+00010830: 6520 696d 706c 656d 656e 7465 642e 2053  e implemented. S
+00010840: 6565 2074 6865 0a53 514c 416c 6368 656d  ee the.SQLAlchem
+00010850: 7920 4f52 4d20 4576 656e 7473 2068 7474  y ORM Events htt
+00010860: 703a 2f2f 646f 6373 2e73 716c 616c 6368  p://docs.sqlalch
+00010870: 656d 792e 6f72 672f 656e 2f6c 6174 6573  emy.org/en/lates
+00010880: 742f 6f72 6d2f 6576 656e 7473 2e68 746d  t/orm/events.htm
+00010890: 6c23 6f72 6d2d 6576 656e 7473 0a0a 596f  l#orm-events..Yo
+000108a0: 7520 6d61 7920 616c 736f 2061 6464 2061  u may also add a
+000108b0: 2063 6c61 7373 6d65 7468 6f64 2077 6974   classmethod wit
+000108c0: 6820 7468 6520 6e61 6d65 2060 6065 7665  h the name ``eve
+000108d0: 6e74 2074 7970 6520 2b20 275f 6f72 6d5f  nt type + '_orm_
+000108e0: 6576 656e 7427 6060 2e20 5468 6520 6576  event'``. The ev
+000108f0: 656e 7420 7769 6c6c 2062 6520 6175 746f  ent will be auto
+00010900: 6d61 7469 636c 790a 6372 6561 7465 2077  maticly.create w
+00010910: 6974 6820 6f6e 2074 6865 204d 6f64 656c  ith on the Model
+00010920: 2061 6e64 2074 6865 2065 7665 6e74 2074   and the event t
+00010930: 7970 6520 7769 7468 6f75 7420 6172 6775  ype without argu
+00010940: 6d65 6e74 733a 3a0a 0a20 2020 2040 7265  ments::..    @re
+00010950: 6769 7374 6572 284d 6f64 656c 290a 2020  gister(Model).  
+00010960: 2020 636c 6173 7320 5465 7374 3a0a 0a20    class Test:.. 
+00010970: 2020 2020 2020 2020 2020 2078 203d 2030             x = 0
+00010980: 0a0a 2020 2020 2020 2020 2020 2020 4063  ..            @c
+00010990: 6c61 7373 6d65 7468 6f64 0a20 2020 2020  lassmethod.     
+000109a0: 2020 2020 2020 2064 6566 2061 6674 6572         def after
+000109b0: 5f69 6e73 6572 745f 6f72 6d5f 6576 656e  _insert_orm_even
+000109c0: 7428 636c 732c 206d 6170 7065 722c 2063  t(cls, mapper, c
+000109d0: 6f6e 6e65 6374 696f 6e2c 2074 6172 6765  onnection, targe
+000109e0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+000109f0: 2020 2020 2320 6361 6c6c 2077 6865 6e20      # call when 
+00010a00: 6120 6e65 7720 696e 7374 616e 6365 206f  a new instance o
+00010a10: 6620 5465 7374 2069 7320 6164 6465 6420  f Test is added 
+00010a20: 696e 2074 6865 2073 6573 7369 6f6e 0a20  in the session. 
+00010a30: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00010a40: 6173 730a 0a20 2020 2020 2020 2020 2020  ass..           
+00010a50: 2040 6c69 7374 656e 2827 4d6f 6465 6c2e   @listen('Model.
+00010a60: 5465 7374 272c 2027 6166 7465 725f 696e  Test', 'after_in
+00010a70: 7365 7274 2729 0a20 2020 2020 2020 2020  sert').         
+00010a80: 2020 2064 6566 2061 6e6f 7468 6572 5f6f     def another_o
+00010a90: 726d 5f65 7665 6e74 2863 6c73 2c20 6d61  rm_event(cls, ma
+00010aa0: 7070 6572 2c20 636f 6e6e 6563 7469 6f6e  pper, connection
+00010ab0: 2c20 7461 7267 6574 293a 0a20 2020 2020  , target):.     
+00010ac0: 2020 2020 2020 2020 2020 2023 2069 7420             # it 
+00010ad0: 6973 2074 6865 2073 616d 6520 6566 6665  is the same effe
+00010ae0: 6374 2061 7320 6060 6166 7465 725f 696e  ct as ``after_in
+00010af0: 7365 7274 5f6f 726d 5f65 7665 6e74 6060  sert_orm_event``
+00010b00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010b10: 2020 2320 6974 2069 7320 6361 6c6c 2061    # it is call a
+00010b20: 6674 6572 2074 6865 2061 6464 206f 6620  fter the add of 
+00010b30: 6120 6e65 7720 696e 7374 616e 6365 2069  a new instance i
+00010b40: 6e20 7468 6520 7365 7373 696f 6e0a 0a0a  n the session...
+00010b50: 4879 6272 6964 206d 6574 686f 640a 7e7e  Hybrid method.~~
+00010b60: 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 0a46 6163  ~~~~~~~~~~~..Fac
+00010b70: 696c 6974 7920 746f 2063 7265 6174 6520  ility to create 
+00010b80: 616e 2053 514c 416c 6368 656d 7920 6879  an SQLAlchemy hy
+00010b90: 6272 6964 206d 6574 686f 642e 2053 6565  brid method. See
+00010ba0: 2074 6869 7320 7061 6765 3a0a 6874 7470   this page:.http
+00010bb0: 3a2f 2f64 6f63 732e 7371 6c61 6c63 6865  ://docs.sqlalche
+00010bc0: 6d79 2e6f 7267 2f65 6e2f 6c61 7465 7374  my.org/en/latest
+00010bd0: 2f6f 726d 2f65 7874 656e 7369 6f6e 732f  /orm/extensions/
+00010be0: 6879 6272 6964 2e68 746d 6c23 6d6f 6475  hybrid.html#modu
+00010bf0: 6c65 2d73 716c 616c 6368 656d 792e 6578  le-sqlalchemy.ex
+00010c00: 742e 6879 6272 6964 0a0a 416e 7942 6c6f  t.hybrid..AnyBlo
+00010c10: 6b20 616c 6c6f 7773 2074 6f20 6465 6669  k allows to defi
+00010c20: 6e65 2061 2068 7962 7269 645f 6d65 7468  ne a hybrid_meth
+00010c30: 6f64 2077 6869 6368 2063 616e 2062 6520  od which can be 
+00010c40: 6f76 6572 6c6f 6164 6564 2c20 6265 6361  overloaded, beca
+00010c50: 7573 6520 7468 650a 7265 616c 2073 716c  use the.real sql
+00010c60: 616c 6368 656d 7920 6465 636f 7261 746f  alchemy decorato
+00010c70: 7220 6973 2061 7070 6c69 6564 2061 6674  r is applied aft
+00010c80: 6572 2061 7373 656d 626c 696e 6720 696e  er assembling in
+00010c90: 2074 6865 206c 6173 7420 6f76 6572 6c6f   the last overlo
+00010ca0: 6164 0a6f 6620 7468 6520 6465 636f 7261  ad.of the decora
+00010cb0: 7465 6420 6d65 7468 6f64 3a3a 0a0a 2020  ted method::..  
+00010cc0: 2020 6672 6f6d 2061 6e79 626c 6f6b 2e64    from anyblok.d
+00010cd0: 6563 6c61 7261 7469 6f6e 7320 696d 706f  eclarations impo
+00010ce0: 7274 2068 7962 7269 645f 6d65 7468 6f64  rt hybrid_method
+00010cf0: 0a0a 2020 2020 4072 6567 6973 7465 7228  ..    @register(
+00010d00: 4d6f 6465 6c29 0a20 2020 2063 6c61 7373  Model).    class
+00010d10: 2054 6573 743a 0a0a 2020 2020 2020 2020   Test:..        
+00010d20: 4068 7962 7269 645f 6d65 7468 6f64 0a20  @hybrid_method. 
+00010d30: 2020 2020 2020 2064 6566 206d 795f 6879         def my_hy
+00010d40: 6272 6964 5f6d 6574 686f 6428 7365 6c66  brid_method(self
+00010d50: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00010d60: 6574 7572 6e20 2e2e 2e0a 0a50 7265 2d63  eturn .....Pre-c
+00010d70: 6f6d 6d69 7420 686f 6f6b 0a7e 7e7e 7e7e  ommit hook.~~~~~
+00010d80: 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 4974 2069  ~~~~~~~~~~..It i
+00010d90: 7320 706f 7373 6962 6c65 2074 6f20 6361  s possible to ca
+00010da0: 6c6c 2073 7065 6369 6669 6320 636c 6173  ll specific clas
+00010db0: 736d 6574 686f 6473 206a 7573 7420 6265  smethods just be
+00010dc0: 666f 7265 2074 6865 2063 6f6d 6d69 7420  fore the commit 
+00010dd0: 6f66 2074 6865 0a73 6573 7369 6f6e 3a3a  of the.session::
+00010de0: 0a0a 2020 2020 4072 6567 6973 7465 7228  ..    @register(
+00010df0: 4d6f 6465 6c29 0a20 2020 2063 6c61 7373  Model).    class
+00010e00: 2054 6573 743a 0a0a 2020 2020 2020 2020   Test:..        
+00010e10: 6964 203d 2049 6e74 6567 6572 2870 7269  id = Integer(pri
+00010e20: 6d61 7279 5f6b 6579 3d54 7275 6529 0a20  mary_key=True). 
+00010e30: 2020 2020 2020 2076 616c 203d 2049 6e74         val = Int
+00010e40: 6567 6572 2864 6566 6175 6c74 3d30 290a  eger(default=0).
+00010e50: 0a20 2020 2020 2020 2040 636c 6173 736d  .        @classm
+00010e60: 6574 686f 640a 2020 2020 2020 2020 6465  ethod.        de
+00010e70: 6620 6d65 7468 6f64 3263 616c 6c5f 6a75  f method2call_ju
+00010e80: 7374 5f62 6566 6f72 655f 7468 655f 636f  st_before_the_co
+00010e90: 6d6d 6974 2863 6c73 2c20 2a61 2c20 2a2a  mmit(cls, *a, **
+00010ea0: 6b77 293a 0a20 2020 2020 2020 2020 2020  kw):.           
+00010eb0: 2070 6173 730a 0a20 2020 202d 2d2d 2d2d   pass..    -----
+00010ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00010ed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00010ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00010ef0: 0a0a 2020 2020 7265 6769 7374 7279 2e54  ..    registry.T
+00010f00: 6573 742e 7072 6563 6f6d 6d69 745f 686f  est.precommit_ho
+00010f10: 6f6b 2827 6d65 7468 6f64 3263 616c 6c5f  ok('method2call_
+00010f20: 6a75 7374 5f62 6566 6f72 655f 7468 655f  just_before_the_
+00010f30: 636f 6d6d 6974 272c 202a 612c 202a 2a6b  commit', *a, **k
+00010f40: 7729 0a0a 506f 7374 2d63 6f6d 6d69 7420  w)..Post-commit 
+00010f50: 686f 6f6b 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e  hook.~~~~~~~~~~~
+00010f60: 7e7e 7e7e 7e0a 0a49 7420 6973 2070 6f73  ~~~~~..It is pos
+00010f70: 7369 626c 6520 746f 2063 616c 6c20 7370  sible to call sp
+00010f80: 6563 6966 6963 2063 6c61 7373 6d65 7468  ecific classmeth
+00010f90: 6f64 7320 6a75 7374 2061 6674 6572 2074  ods just after t
+00010fa0: 6865 2063 6f6d 6d69 7420 6f66 2074 6865  he commit of the
+00010fb0: 0a73 6573 7369 6f6e 3a3a 0a0a 2020 2020  .session::..    
+00010fc0: 4072 6567 6973 7465 7228 4d6f 6465 6c29  @register(Model)
+00010fd0: 0a20 2020 2063 6c61 7373 2054 6573 743a  .    class Test:
+00010fe0: 0a0a 2020 2020 2020 2020 6964 203d 2049  ..        id = I
+00010ff0: 6e74 6567 6572 2870 7269 6d61 7279 5f6b  nteger(primary_k
+00011000: 6579 3d54 7275 6529 0a20 2020 2020 2020  ey=True).       
+00011010: 2076 616c 203d 2049 6e74 6567 6572 2864   val = Integer(d
+00011020: 6566 6175 6c74 3d30 290a 0a20 2020 2020  efault=0)..     
+00011030: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00011040: 2020 2020 2020 2020 6465 6620 6d65 7468          def meth
+00011050: 6f64 3263 616c 6c5f 6a75 7374 5f61 6674  od2call_just_aft
+00011060: 6572 5f74 6865 5f63 6f6d 6d69 7428 636c  er_the_commit(cl
+00011070: 732c 202a 612c 202a 2a6b 7729 3a0a 2020  s, *a, **kw):.  
+00011080: 2020 2020 2020 2020 2020 7061 7373 0a0a            pass..
+00011090: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+000110a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000110b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000110c0: 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2020 2072  ---------..    r
+000110d0: 6567 6973 7472 792e 5465 7374 2e70 6f73  egistry.Test.pos
+000110e0: 7463 6f6d 6d69 745f 686f 6f6b 2827 6d65  tcommit_hook('me
+000110f0: 7468 6f64 3263 616c 6c5f 6a75 7374 5f61  thod2call_just_a
+00011100: 6674 6572 5f74 6865 5f63 6f6d 6d69 7427  fter_the_commit'
+00011110: 2c20 2a61 2c20 2a2a 6b77 290a 0a0a 416c  , *a, **kw)...Al
+00011120: 6961 7365 640a 7e7e 7e7e 7e7e 7e0a 0a46  iased.~~~~~~~..F
+00011130: 6163 696c 6974 7920 746f 2063 7265 6174  acility to creat
+00011140: 6520 616e 2053 514c 2061 6c69 6173 2066  e an SQL alias f
+00011150: 6f72 2074 6865 2053 514c 2071 7565 7279  or the SQL query
+00011160: 2062 7920 7468 6520 4f52 4d3a 3a0a 0a20   by the ORM::.. 
+00011170: 2020 2073 656c 6563 7420 2a20 6672 6f6d     select * from
+00011180: 206d 795f 7461 626c 6520 7468 655f 7461   my_table the_ta
+00011190: 626c 655f 616c 6961 732e 0a0a 5468 6973  ble_alias...This
+000111a0: 2066 6163 696c 6974 7920 6973 2067 6976   facility is giv
+000111b0: 656e 2062 7920 5351 4c41 6c63 6865 6d79  en by SQLAlchemy
+000111c0: 2c20 616e 6420 616e 7962 6c6f 6b20 6164  , and anyblok ad
+000111d0: 6473 2074 6869 7320 6675 6e63 7469 6f6e  ds this function
+000111e0: 6e61 6c69 7479 0a64 6972 6563 746c 7920  nality.directly 
+000111f0: 696e 2074 6865 204d 6f64 656c 3a3a 0a0a  in the Model::..
+00011200: 2020 2020 426c 6f6b 416c 6961 7365 6420      BlokAliased 
+00011210: 3d20 7265 6769 7374 7279 2e53 7973 7465  = registry.Syste
+00011220: 6d2e 426c 6f6b 2e61 6c69 6173 6564 2829  m.Blok.aliased()
+00011230: 0a0a 2e2e 206e 6f74 653a 3a20 5365 6520  .... note:: See 
+00011240: 7468 6973 2070 6167 653a 0a20 2020 2068  this page:.    h
+00011250: 7474 703a 2f2f 646f 6373 2e73 716c 616c  ttp://docs.sqlal
+00011260: 6368 656d 792e 6f72 672f 656e 2f6c 6174  chemy.org/en/lat
+00011270: 6573 742f 6f72 6d2f 7175 6572 792e 6874  est/orm/query.ht
+00011280: 6d6c 2373 716c 616c 6368 656d 792e 6f72  ml#sqlalchemy.or
+00011290: 6d2e 616c 6961 7365 640a 2020 2020 746f  m.aliased.    to
+000112a0: 206b 6e6f 7720 7468 6520 7061 7261 6d65   know the parame
+000112b0: 7465 7273 206f 6620 7468 6520 6060 616c  ters of the ``al
+000112c0: 6961 7365 6460 6020 6d65 7468 6f64 0a0a  iased`` method..
+000112d0: 2020 2020 2e2e 2077 6172 6e69 6e67 3a3a      .. warning::
+000112e0: 2054 6865 2066 6972 7374 2061 7267 2069   The first arg i
+000112f0: 7320 616c 7265 6164 7920 7061 7373 6564  s already passed
+00011300: 2062 7920 416e 7942 6c6f 6b0a 0a20 2020   by AnyBlok..   
+00011310: 202e 2e20 7761 726e 696e 673a 3a20 4f6e   .. warning:: On
+00011320: 6c79 2074 6869 7320 6d65 7468 6f64 2067  ly this method g
+00011330: 6976 6520 7468 6520 7265 6769 7374 7279  ive the registry
+00011340: 2069 6e74 6f20 7468 6520 616c 6961 732c   into the alias,
+00011350: 2064 6f6e 2774 2069 6d70 6f72 7420 2a2a   don't import **
+00011360: 7371 6c61 6c63 6865 6d79 2e6f 726d 2e61  sqlalchemy.orm.a
+00011370: 6c69 6173 6564 2a2a 0a0a 4765 7420 7468  liased**..Get th
+00011380: 6520 6375 7272 656e 7420 656e 7669 726f  e current enviro
+00011390: 6e6d 656e 740a 7e7e 7e7e 7e7e 7e7e 7e7e  nment.~~~~~~~~~~
+000113a0: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+000113b0: 7e0a 0a54 6865 2063 7572 7265 6e74 2065  ~..The current e
+000113c0: 6e76 6972 6f6e 6d65 6e74 2069 7320 7361  nvironment is sa
+000113d0: 7665 6420 696e 2074 6865 206d 6169 6e20  ved in the main 
+000113e0: 7468 7265 6164 2e20 596f 7520 6361 6e20  thread. You can 
+000113f0: 6164 6420 6120 7661 6c75 6520 746f 0a74  add a value to.t
+00011400: 6865 2063 7572 7265 6e74 2045 6e76 6972  he current Envir
+00011410: 6f6e 6d65 6e74 3a3a 0a0a 2020 2020 7365  onment::..    se
+00011420: 6c66 2e45 6e76 2e73 6574 2827 4d79 2076  lf.Env.set('My v
+00011430: 6172 272c 2027 6f6e 6520 7661 6c75 6527  ar', 'one value'
+00011440: 290a 0a59 6f75 2063 616e 2067 6574 2061  )..You can get a
+00011450: 2076 616c 7565 2066 726f 6d20 7468 6520   value from the 
+00011460: 6375 7272 656e 7420 456e 7669 726f 6e6d  current Environm
+00011470: 656e 743a 3a0a 0a20 2020 206d 7976 616c  ent::..    myval
+00011480: 7565 203d 2073 656c 662e 456e 762e 6765  ue = self.Env.ge
+00011490: 7428 274d 7920 7661 7227 2c20 6465 6661  t('My var', defa
+000114a0: 756c 3d22 4d79 2064 6566 6175 6c74 2076  ul="My default v
+000114b0: 616c 7565 2229 0a0a 2e2e 206e 6f74 653a  alue").... note:
+000114c0: 3a0a 0a20 2020 2054 6865 2065 6e76 6972  :..    The envir
+000114d0: 6f6e 6d65 6e74 2069 7320 6173 2061 2064  onment is as a d
+000114e0: 6963 7420 7468 6520 7661 6c75 6520 6361  ict the value ca
+000114f0: 6e20 6265 2061 6e20 696e 7374 616e 6365  n be an instance
+00011500: 206f 6620 616e 7920 7479 7065 0a0a 496e   of any type..In
+00011510: 6974 6961 6c69 7a65 2073 6f6d 6520 6461  itialize some da
+00011520: 7461 2062 7920 656e 7472 7920 706f 696e  ta by entry poin
+00011530: 740a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  t.~~~~~~~~~~~~~~
+00011540: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  ~~~~~~~~~~~~~~~~
+00011550: 7e7e 7e7e 7e0a 0a74 6865 2065 6e74 7279  ~~~~~..the entry
+00011560: 2070 6f69 6e74 2060 6061 6e79 626c 6f6b   point ``anyblok
+00011570: 2e69 6e69 7460 6020 616c 6c6f 7720 746f  .init`` allow to
+00011580: 2064 6566 696e 6520 6675 6e63 7469 6f6e   define function
+00011590: 2c20 6060 c3ac 6e69 745f 6675 6e63 7469  , ``..nit_functi
+000115a0: 6f6e 6060 0a69 6e20 7468 6973 2065 7861  on``.in this exa
+000115b0: 6d70 6c65 3a3a 0a0a 2020 2020 7365 7475  mple::..    setu
+000115c0: 7028 0a20 2020 2020 2020 202e 2e2e 0a20  p(.        .... 
+000115d0: 2020 2020 2020 2065 6e74 7279 5f70 6f69         entry_poi
+000115e0: 6e74 733d 7b0a 2020 2020 2020 2020 2020  nts={.          
+000115f0: 2020 2761 6e79 626c 6f6b 2e69 6e69 7427    'anyblok.init'
+00011600: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
+00011610: 2020 2020 276d 795f 6675 6e63 7469 6f6e      'my_function
+00011620: 3d70 6174 683a 696e 6974 5f66 756e 6374  =path:init_funct
+00011630: 696f 6e27 2c0a 2020 2020 2020 2020 2020  ion',.          
+00011640: 2020 5d2c 0a20 2020 2020 2020 207d 2c0a    ],.        },.
+00011650: 2020 2020 290a 0a49 6e20 7468 6520 7061      )..In the pa
+00011660: 7468 2074 6865 2069 6e69 745f 6675 6e63  th the init_func
+00011670: 7469 6f6e 206d 7573 7420 6265 2064 6566  tion must be def
+00011680: 696e 6564 3a3a 0a0a 2020 2020 6465 6620  ined::..    def 
+00011690: 696e 6974 5f66 756e 6374 696f 6e28 756e  init_function(un
+000116a0: 6974 7465 7374 3d46 616c 7365 293a 0a20  ittest=False):. 
+000116b0: 2020 2020 2020 202e 2e2e 0a0a 2e2e 7761         .......wa
+000116c0: 726e 696e 673a 3a0a 0a20 2020 2055 7365  rning::..    Use
+000116d0: 2075 6e69 7474 6573 7420 7061 7261 6d65   unittest parame
+000116e0: 7465 7220 746f 2064 6566 696e 6564 2069  ter to defined i
+000116f0: 6620 7468 6520 6675 6e63 7469 6f6e 206d  f the function m
+00011700: 7573 7420 6265 2063 616c 6c0a 2020 2020  ust be call.    
+00011710: 6f72 206e 6f74 0a0a 4d61 6b65 2065 6173  or not..Make eas
+00011720: 696c 7920 5265 6164 4f6e 6c79 206d 6f64  ily ReadOnly mod
+00011730: 656c 0a7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e  el.~~~~~~~~~~~~~
+00011740: 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 7e0a 0a49  ~~~~~~~~~~~~~..I
+00011750: 6e20 736f 6d6d 6520 6361 7365 2079 6f75  n somme case you
+00011760: 2077 616e 7420 7468 6174 2079 6f75 7220   want that your 
+00011770: 6d6f 6465 6c20 6973 3a0a 0a2a 2072 6561  model is:..* rea
+00011780: 646f 6e6c 793a 204e 6f20 6d6f 6469 6669  donly: No modifi
+00011790: 6361 7469 6f6e 2c20 4e6f 2064 656c 6574  cation, No delet
+000117a0: 696f 6e3a 3a0a 0a20 2020 2020 2040 7265  ion::..      @re
+000117b0: 6769 7374 6572 282e 2e2e 290a 2020 2020  gister(...).    
+000117c0: 2020 636c 6173 7320 4d79 4d6f 6465 6c28    class MyModel(
+000117d0: 4d69 7869 6e2e 5265 6164 4f6e 6c79 293a  Mixin.ReadOnly):
+000117e0: 0a20 2020 2020 2020 202e 2e2e 0a0a 2a20  .        .....* 
+000117f0: 666f 7262 6964 206d 6f64 6966 6963 6174  forbid modificat
+00011800: 696f 6e3a 204e 6f20 6d6f 6469 6669 6361  ion: No modifica
+00011810: 7469 6f6e 2062 7574 2063 616e 2064 656c  tion but can del
+00011820: 6574 653a 3a0a 0a20 2020 2020 2040 7265  ete::..      @re
+00011830: 6769 7374 6572 282e 2e2e 290a 2020 2020  gister(...).    
+00011840: 2020 636c 6173 7320 4d79 4d6f 6465 6c28    class MyModel(
+00011850: 4d69 7869 6e2e 466f 7262 6964 5570 6461  Mixin.ForbidUpda
+00011860: 7465 293a 0a20 2020 2020 2020 202e 2e2e  te):.        ...
+00011870: 0a0a 2a20 666f 7262 6964 2064 656c 6574  ..* forbid delet
+00011880: 696f 6e3a 204e 6f20 6465 6c65 7469 6f6e  ion: No deletion
+00011890: 2062 7574 2063 616e 206d 6f64 6966 793a   but can modify:
+000118a0: 3a0a 0a20 2020 2020 2040 7265 6769 7374  :..      @regist
+000118b0: 6572 282e 2e2e 290a 2020 2020 2020 636c  er(...).      cl
+000118c0: 6173 7320 4d79 4d6f 6465 6c28 4d69 7869  ass MyModel(Mixi
+000118d0: 6e2e 466f 7262 6964 4465 6c65 7465 293a  n.ForbidDelete):
+000118e0: 0a20 2020 2020 2020 202e 2e2e 0a0a 0a50  .        ......P
+000118f0: 6c75 6769 6e0a 2d2d 2d2d 2d2d 0a0a 506c  lugin.------..Pl
+00011900: 7567 696e 2069 7320 7573 6564 2066 6f72  ugin is used for
+00011910: 2074 6865 206c 6f77 206c 6576 656c 2c20   the low level, 
+00011920: 6974 2069 7320 6e6f 7420 7573 6520 696e  it is not use in
+00011930: 2074 6865 2062 6c6f 6b73 2c20 6265 6361   the bloks, beca
+00011940: 7573 6520 7468 6520 6d6f 6465 6c0a 6361  use the model.ca
+00011950: 6e20 6265 206f 7665 726c 6f61 6420 6279  n be overload by
+00011960: 2074 6865 2064 6563 6c61 7261 7469 6f6e   the declaration
+00011970: 2e0a 0a44 6566 696e 6520 6120 6e65 7720  ...Define a new 
+00011980: 706c 7567 696e 0a7e 7e7e 7e7e 7e7e 7e7e  plugin.~~~~~~~~~
+00011990: 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a 4120 706c  ~~~~~~~~~~..A pl
+000119a0: 7567 696e 2063 616e 2062 6520 6120 636c  ugin can be a cl
+000119b0: 6173 7320 6f72 2061 2066 756e 6374 696f  ass or a functio
+000119c0: 6e3a 3a0a 0a20 2020 2063 6c61 7373 204d  n::..    class M
+000119d0: 7950 6c75 6769 6e3a 0a20 2020 2020 2020  yPlugin:.       
+000119e0: 2070 6173 730a 0a41 6464 2074 6865 2070   pass..Add the p
+000119f0: 6c75 6769 6e20 6465 6669 6e69 7469 6f6e  lugin definition
+00011a00: 2069 6e20 7468 6520 636f 6e66 6967 7572   in the configur
+00011a10: 6174 696f 6e3a 3a0a 0a20 2020 2040 436f  ation::..    @Co
+00011a20: 6e66 6967 7572 6174 696f 6e2e 6164 6428  nfiguration.add(
+00011a30: 2770 6c75 6769 6e73 2729 0a20 2020 2064  'plugins').    d
+00011a40: 6566 2061 6464 5f70 6c75 6769 6e73 2873  ef add_plugins(s
+00011a50: 656c 662c 2067 726f 7570 290a 2020 2020  elf, group).    
+00011a60: 2020 2020 6772 6f75 702e 6164 645f 6172      group.add_ar
+00011a70: 6775 6d65 6e74 2827 2d2d 6d79 2d6f 7074  gument('--my-opt
+00011a80: 696f 6e27 2c20 6465 7374 3d27 706c 7567  ion', dest='plug
+00011a90: 696e 5f6e 616d 6527 2c0a 2020 2020 2020  in_name',.      
+00011aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ab0: 2020 2020 2074 7970 653d 416e 7942 6c6f       type=AnyBlo
+00011ac0: 6b50 6c75 6769 6e2c 0a20 2020 2020 2020  kPlugin,.       
+00011ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ae0: 2020 2020 6465 6661 756c 743d 2770 6174      default='pat
+00011af0: 683a 4d79 506c 7567 696e 2729 0a0a 5573  h:MyPlugin')..Us
+00011b00: 6520 7468 6520 706c 7567 696e 3a3a 0a0a  e the plugin::..
+00011b10: 2020 2020 706c 7567 696e 203d 2043 6f6e      plugin = Con
+00011b20: 6669 6775 7261 7469 6f6e 2e67 6574 2827  figuration.get('
+00011b30: 706c 7567 696e 5f6e 616d 6527 290a 0a0a  plugin_name')...
+00011b40: 2a2a 616e 7962 6c6f 6b2e 6d6f 6465 6c2e  **anyblok.model.
+00011b50: 706c 7567 696e 2a2a 0a2d 2d2d 2d2d 2d2d  plugin**.-------
+00011b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011b70: 2d0a 0a54 6869 7320 6120 686f 6f6b 2074  -..This a hook t
+00011b80: 6f20 6164 6420 6e65 7720 6665 6174 7572  o add new featur
+00011b90: 6520 696e 204d 6f64 656c 2c20 7468 6973  e in Model, this
+00011ba0: 2069 7320 616c 7265 6164 7920 7573 6520   is already use 
+00011bb0: 666f 723a 0a0a 2a20 6879 6272 6964 5f6d  for:..* hybrid_m
+00011bc0: 6574 686f 640a 2a20 7461 626c 6520 616e  ethod.* table an
+00011bd0: 6420 6d61 7070 6572 2061 7267 730a 2a20  d mapper args.* 
+00011be0: 6576 656e 740a 2a20 5371 6c61 6c63 6865  event.* Sqlalche
+00011bf0: 6d79 2065 7665 6e74 0a2a 2063 6163 6865  my event.* cache
+00011c00: 202f 2063 6c61 7373 6d65 7468 6f64 5f63   / classmethod_c
+00011c10: 6163 6865 0a0a 5374 6172 7420 6279 2069  ache..Start by i
+00011c20: 6d70 6c65 6d65 6e74 696e 6720 7468 6520  mplementing the 
+00011c30: 706c 7567 696e 2028 7365 650a 3a63 6c61  plugin (see.:cla
+00011c40: 7373 3a60 4d6f 6465 6c50 6c75 6769 6e42  ss:`ModelPluginB
+00011c50: 6173 6520 3c61 6e79 626c 6f6b 2e6d 6f64  ase <anyblok.mod
+00011c60: 656c 2e70 6c75 6769 6e73 2e4d 6f64 656c  el.plugins.Model
+00011c70: 506c 7567 696e 4261 7365 3e60 293a 3a0a  PluginBase>`)::.
+00011c80: 0a20 2020 2066 726f 6d20 616e 7962 6c6f  .    from anyblo
+00011c90: 6b2e 6d6f 6465 6c2e 706c 7567 696e 7320  k.model.plugins 
+00011ca0: 696d 706f 7274 204d 6f64 656c 506c 7567  import ModelPlug
+00011cb0: 696e 4261 7365 0a0a 2020 2020 636c 6173  inBase..    clas
+00011cc0: 7320 4d79 506c 7567 696e 284d 6f64 656c  s MyPlugin(Model
+00011cd0: 506c 7567 696e 4261 7365 293a 0a20 2020  PluginBase):.   
+00011ce0: 2020 2020 202e 2e2e 0a0a 0a54 6865 6e2c       ......Then,
+00011cf0: 2064 6563 6c61 7265 2069 7420 696e 2060   declare it in `
+00011d00: 6073 6574 7570 2e70 7960 603a 3a0a 0a20  `setup.py``::.. 
+00011d10: 2020 2073 6574 7570 280a 2020 2020 2020     setup(.      
+00011d20: 2020 2e2e 2e0a 2020 2020 2020 2020 656e    ....        en
+00011d30: 7472 795f 706f 696e 7473 3d7b 0a20 2020  try_points={.   
+00011d40: 2020 2020 2020 2020 202e 2e2e 0a20 2020           ....   
+00011d50: 2020 2020 2020 2020 2027 616e 7962 6c6f           'anyblo
+00011d60: 6b2e 6d6f 6465 6c2e 706c 7567 696e 273a  k.model.plugin':
+00011d70: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00011d80: 2020 2027 6d79 706c 7567 696e 3d70 6174     'myplugin=pat
+00011d90: 683a 4d79 506c 7567 696e 272c 0a20 2020  h:MyPlugin',.   
+00011da0: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+00011db0: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
+00011dc0: 2020 2020 7d2c 0a20 2020 2020 2020 202e      },.        .
+00011dd0: 2e2e 0a20 2020 2029 0a0a 0a2a 2a61 6e79  ...    )...**any
+00011de0: 626c 6f6b 2e6d 6f64 656c 2e66 6163 746f  blok.model.facto
+00011df0: 7279 2a2a 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ry**.-----------
+00011e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
+00011e10: 5468 6973 2066 6163 746f 7279 2069 7320  This factory is 
+00011e20: 7573 6564 2074 6f3a 0a0a 2a20 6769 7665  used to:..* give
+00011e30: 2074 6865 2063 6f72 6520 636c 6173 7365   the core classe
+00011e40: 7320 6e65 6564 2074 6f20 6275 696c 6420  s need to build 
+00011e50: 7468 6520 6d6f 6465 6c0a 2a20 6275 696c  the model.* buil
+00011e60: 6420 7468 6520 6d6f 6465 6c0a 0a53 7461  d the model..Sta
+00011e70: 7274 2062 7920 696d 706c 656d 656e 7469  rt by implementi
+00011e80: 6e67 2074 6865 2066 6163 746f 7279 2028  ng the factory (
+00011e90: 7365 650a 3a63 6c61 7373 3a60 4261 7365  see.:class:`Base
+00011ea0: 4661 6374 6f72 7920 3c61 6e79 626c 6f6b  Factory <anyblok
+00011eb0: 2e6d 6f64 656c 2e74 6163 746f 7279 2e42  .model.tactory.B
+00011ec0: 6173 6546 6163 746f 7279 3e60 293a 3a0a  aseFactory>`)::.
+00011ed0: 0a20 2020 2066 726f 6d20 616e 7962 6c6f  .    from anyblo
+00011ee0: 6b2e 6d6f 6465 6c2e 6661 6374 6f72 7920  k.model.factory 
+00011ef0: 696d 706f 7274 2042 6173 6546 6163 746f  import BaseFacto
+00011f00: 7279 0a0a 2020 2020 636c 6173 7320 4d79  ry..    class My
+00011f10: 4661 6374 6f72 7928 4261 7365 4661 6374  Factory(BaseFact
+00011f20: 6f72 7929 3a0a 0a20 2020 2020 2020 2064  ory):..        d
+00011f30: 6566 2069 6e73 6572 745f 636f 7265 5f62  ef insert_core_b
+00011f40: 6173 6573 2873 656c 662c 2062 6173 6573  ases(self, bases
+00011f50: 2c20 7072 6f70 6572 7469 6573 293a 0a20  , properties):. 
+00011f60: 2020 2020 2020 2020 2020 202e 2e2e 0a0a             .....
+00011f70: 2020 2020 2020 2020 6465 6620 6275 696c          def buil
+00011f80: 645f 6d6f 6465 6c28 7365 6c66 2c20 6d6f  d_model(self, mo
+00011f90: 6465 6c6e 616d 652c 2062 6173 6573 2c20  delname, bases, 
+00011fa0: 7072 6f70 6572 7469 6573 293a 0a20 2020  properties):.   
+00011fb0: 2020 2020 2020 2020 202e 2e2e 0a0a 496e           .....In
+00011fc0: 2079 6f75 7220 626c 6f6b 7320 796f 7520   your bloks you 
+00011fd0: 6361 6e20 7573 6520 796f 7572 2066 6163  can use your fac
+00011fe0: 746f 7279 3a3a 0a0a 2020 2020 4072 6567  tory::..    @reg
+00011ff0: 6973 7465 7228 4d6f 6465 6c2c 2066 6163  ister(Model, fac
+00012000: 746f 7279 3d4d 7946 6163 746f 7279 290a  tory=MyFactory).
+00012010: 2020 2020 636c 6173 7320 4d79 4d6f 6465      class MyMode
+00012020: 6c3a 0a20 2020 2020 2020 202e 2e2e 0a0a  l:.        .....
+00012030: 2a2a 456e 6769 6e65 2773 2065 7665 6e74  **Engine's event
+00012040: 732a 2a0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  s**.------------
+00012050: 2d2d 2d2d 2d2d 2d0a 0a54 6865 2065 6e67  -------..The eng
+00012060: 696e 6527 7320 6576 656e 7473 2069 7320  ine's events is 
+00012070: 7573 6564 2074 6f20 6465 6669 6e65 2073  used to define s
+00012080: 716c 616c 6368 656d 7920 6576 656e 7420  qlalchemy event 
+00012090: 6c69 7374 656e 6572 206f 6e20 656e 6769  listener on engi
+000120a0: 6e65 0a0a 7468 6973 2065 7665 6e74 2069  ne..this event i
+000120b0: 7320 6465 636c 6172 6564 2062 7920 656e  s declared by en
+000120c0: 7472 7970 6f69 6e74 3a0a 0a2a 202a 2a61  trypoint:..* **a
+000120d0: 6e79 626c 6f6b 2e65 6e67 696e 652e 6576  nyblok.engine.ev
+000120e0: 656e 742a 2a20 3a20 466f 7220 616c 6c20  ent** : For all 
+000120f0: 6469 616c 6563 7473 0a2a 202a 2a61 6e79  dialects.* **any
+00012100: 626c 6f6b 2e65 6e67 696e 652e 6576 656e  blok.engine.even
+00012110: 742e 706f 7374 6772 6573 2a2a 203a 206f  t.postgres** : o
+00012120: 6e6c 7920 666f 7220 706f 7374 6772 6573  nly for postgres
+00012130: 716c 0a2a 202a 2a61 6e79 626c 6f6b 2e65  ql.* **anyblok.e
+00012140: 6e67 696e 652e 6576 656e 742e 6d79 7371  ngine.event.mysq
+00012150: 6c2a 2a20 3a20 6f6e 6c79 2066 6f72 204d  l** : only for M
+00012160: 7953 514c 0a2a 202a 2a61 6e79 626c 6f6b  ySQL.* **anyblok
+00012170: 2e65 6e67 696e 652e 6576 656e 742e 6d73  .engine.event.ms
+00012180: 7371 6c2a 2a20 3a20 6f6e 6c79 2066 6f72  sql** : only for
+00012190: 204d 7353 514c 0a0a 4578 656d 706c 6520   MsSQL..Exemple 
+000121a0: 7769 7468 2074 6865 202a 2a6d 7973 716c  with the **mysql
+000121b0: 5f6e 6f5f 6175 746f 636f 6d6d 6974 2a2a  _no_autocommit**
+000121c0: 206c 6973 7465 6e65 720a 0a2a 2a61 6e79   listener..**any
+000121d0: 626c 6f6b 2e65 7665 6e74 2a2a 3a3a 0a0a  blok.event**::..
+000121e0: 2020 2066 726f 6d20 7371 6c61 6c63 6865     from sqlalche
+000121f0: 6d79 2069 6d70 6f72 7420 6576 656e 740a  my import event.
+00012200: 0a0a 2020 2064 6566 206d 7973 716c 5f6e  ..   def mysql_n
+00012210: 6f5f 6175 746f 636f 6d6d 6974 2865 6e67  o_autocommit(eng
+00012220: 696e 6529 3a0a 0a20 2020 2020 2020 6465  ine):..       de
+00012230: 6620 6d79 7371 6c5f 7365 745f 6e6f 5f61  f mysql_set_no_a
+00012240: 7574 6f63 6f6d 6d69 7428 6462 6170 695f  utocommit(dbapi_
+00012250: 636f 6e2c 2063 6f6e 6e65 6374 696f 6e5f  con, connection_
+00012260: 7265 636f 7264 293a 0a20 2020 2020 2020  record):.       
+00012270: 2020 2020 6375 7220 3d20 6462 6170 695f      cur = dbapi_
+00012280: 636f 6e2e 6375 7273 6f72 2829 0a20 2020  con.cursor().   
+00012290: 2020 2020 2020 2020 6375 722e 6578 6563          cur.exec
+000122a0: 7574 6528 2253 4554 2061 7574 6f63 6f6d  ute("SET autocom
+000122b0: 6d69 743d 303b 2229 0a20 2020 2020 2020  mit=0;").       
+000122c0: 2020 2020 6375 722e 6578 6563 7574 6528      cur.execute(
+000122d0: 2253 4554 2053 4553 5349 4f4e 2073 716c  "SET SESSION sql
+000122e0: 5f6d 6f64 653d 2754 5241 4449 5449 4f4e  _mode='TRADITION
+000122f0: 414c 273b 2229 0a20 2020 2020 2020 2020  AL';").         
+00012300: 2020 6375 7220 3d20 4e6f 6e65 0a0a 2020    cur = None..  
+00012310: 2020 2020 2065 7665 6e74 2e6c 6973 7465       event.liste
+00012320: 6e28 656e 6769 6e65 2c20 2763 6f6e 6e65  n(engine, 'conne
+00012330: 6374 272c 206d 7973 716c 5f73 6574 5f6e  ct', mysql_set_n
+00012340: 6f5f 6175 746f 636f 6d6d 6974 290a 0a0a  o_autocommit)...
+00012350: 2a2a 7365 7475 702e 7079 2a2a 3a3a 0a0a  **setup.py**::..
+00012360: 2020 2073 6574 7570 280a 2020 2020 2020     setup(.      
+00012370: 2065 6e74 7279 5f70 6f69 6e74 733d 7b0a   entry_points={.
+00012380: 2020 2020 2020 2020 2020 2027 616e 7962             'anyb
+00012390: 6c6f 6b2e 656e 6769 6e65 2e65 7665 6e74  lok.engine.event
+000123a0: 2e6d 7973 716c 273a 205b 0a20 2020 2020  .mysql': [.     
+000123b0: 2020 2020 2020 2020 2020 276d 7973 716c            'mysql
+000123c0: 2d6e 6f2d 6175 746f 636f 6d6d 6974 3d61  -no-autocommit=a
+000123d0: 6e79 626c 6f6b 2e65 7665 6e74 3a6d 7973  nyblok.event:mys
+000123e0: 716c 5f6e 6f5f 6175 746f 636f 6d6d 6974  ql_no_autocommit
+000123f0: 272c 0a20 2020 2020 2020 2020 2020 5d2c  ',.           ],
+00012400: 0a20 2020 2020 2020 7d2c 0a20 2020 290a  .       },.   ).
+00012410: 0a2e 2e20 6e6f 7465 3a3a 0a0a 2020 2054  ... note::..   T
+00012420: 6865 2053 514c 416c 6368 656d 7920 6465  he SQLAlchemy de
+00012430: 6375 6d65 6e74 6174 696f 6e20 666f 7220  cumentation for 
+00012440: 7468 6520 6063 6f72 6520 6576 656e 7420  the `core event 
+00012450: 3c68 7474 7073 3a2f 2f64 6f63 732e 7371  <https://docs.sq
+00012460: 6c61 6c63 6865 6d79 2e6f 7267 2f65 6e2f  lalchemy.org/en/
+00012470: 3134 2f63 6f72 652f 6576 656e 7473 2e68  14/core/events.h
+00012480: 746d 6c3f 6869 6768 6c69 6768 743d 6576  tml?highlight=ev
+00012490: 656e 7423 636f 6e6e 6563 7469 6f6e 2d70  ent#connection-p
+000124a0: 6f6f 6c2d 6576 656e 7473 3e60 5f0a 0a2a  ool-events>`_..*
+000124b0: 2a53 6573 7369 6f6e 2773 2065 7665 6e74  *Session's event
+000124c0: 732a 2a0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  s**.------------
+000124d0: 2d2d 2d2d 2d2d 2d2d 0a0a 5468 6520 656e  --------..The en
+000124e0: 6769 6e65 2773 2065 7665 6e74 7320 6973  gine's events is
+000124f0: 2075 7365 6420 746f 2064 6566 696e 6520   used to define 
+00012500: 7371 6c61 6c63 6865 6d79 2065 7665 6e74  sqlalchemy event
+00012510: 206c 6973 7465 6e65 7220 6f6e 2065 6e67   listener on eng
+00012520: 696e 650a 0a74 6869 7320 6576 656e 7420  ine..this event 
+00012530: 6973 2064 6563 6c61 7265 6420 6279 2065  is declared by e
+00012540: 6e74 7279 706f 696e 743a 0a0a 2a20 2a2a  ntrypoint:..* **
+00012550: 616e 7962 6c6f 6b2e 7365 7373 696f 6e2e  anyblok.session.
+00012560: 6576 656e 742a 2a20 3a20 466f 7220 616c  event** : For al
+00012570: 6c20 6469 616c 6563 7473 0a2a 202a 2a61  l dialects.* **a
+00012580: 6e79 626c 6f6b 2e73 6573 7369 6f6e 2e65  nyblok.session.e
+00012590: 7665 6e74 2e70 6f73 7467 7265 7371 6c2a  vent.postgresql*
+000125a0: 2a20 3a20 6f6e 6c79 2066 6f72 2070 6f73  * : only for pos
+000125b0: 7467 7265 7371 6c0a 2a20 2a2a 616e 7962  tgresql.* **anyb
+000125c0: 6c6f 6b2e 7365 7373 696f 6e2e 6576 656e  lok.session.even
+000125d0: 742e 6d79 7371 6c2a 2a20 3a20 6f6e 6c79  t.mysql** : only
+000125e0: 2066 6f72 204d 7953 514c 0a2a 202a 2a61   for MySQL.* **a
+000125f0: 6e79 626c 6f6b 2e73 6573 7369 6f6e 2e65  nyblok.session.e
+00012600: 7665 6e74 2e6d 7373 716c 2a2a 203a 206f  vent.mssql** : o
+00012610: 6e6c 7920 666f 7220 4d73 5351 4c0a 0a45  nly for MsSQL..E
+00012620: 7865 6d70 6c65 0a0a 6d65 7468 6f64 3a3a  xemple..method::
+00012630: 0a0a 2020 2066 726f 6d20 7371 6c61 6c63  ..   from sqlalc
+00012640: 6865 6d79 2069 6d70 6f72 7420 6576 656e  hemy import even
+00012650: 740a 0a0a 2020 2064 6566 2064 6f5f 736f  t...   def do_so
+00012660: 6d65 7468 696e 6728 7365 7373 696f 6e29  mething(session)
+00012670: 3a0a 0a20 2020 2020 2020 6465 6620 736f  :..       def so
+00012680: 6d65 7468 696e 6728 7365 7373 2c20 7472  mething(sess, tr
+00012690: 616e 7361 6374 696f 6e2c 2063 6f6e 6e65  ansaction, conne
+000126a0: 6374 696f 6e29 3a0a 2020 2020 2020 2020  ction):.        
+000126b0: 2020 2070 6173 730a 0a20 2020 2020 2020     pass..       
+000126c0: 6576 656e 742e 6c69 7374 656e 2873 6573  event.listen(ses
+000126d0: 7369 6f6e 2c20 2761 6674 6572 5f62 6567  sion, 'after_beg
+000126e0: 696e 272c 2073 6f6d 6574 6869 6e67 290a  in', something).
+000126f0: 0a0a 2a2a 7365 7475 702e 7079 2a2a 3a3a  ..**setup.py**::
+00012700: 0a0a 2020 2073 6574 7570 280a 2020 2020  ..   setup(.    
+00012710: 2020 2065 6e74 7279 5f70 6f69 6e74 733d     entry_points=
+00012720: 7b0a 2020 2020 2020 2020 2020 2027 616e  {.           'an
+00012730: 7962 6c6f 6b2e 7365 7373 696f 6e2e 6576  yblok.session.ev
+00012740: 656e 7427 3a20 5b0a 2020 2020 2020 2020  ent': [.        
+00012750: 2020 2020 2020 2027 646f 2d73 6f6d 6574         'do-somet
+00012760: 6869 6e67 3d70 6174 683a 646f 5f73 6f6d  hing=path:do_som
+00012770: 6574 6869 6e67 272c 0a20 2020 2020 2020  ething',.       
+00012780: 2020 2020 5d2c 0a20 2020 2020 2020 7d2c      ],.       },
+00012790: 0a20 2020 290a 0a2e 2e20 6e6f 7465 3a3a  .   ).... note::
+000127a0: 0a0a 2020 2054 6865 2053 514c 416c 6368  ..   The SQLAlch
+000127b0: 656d 7920 6465 6375 6d65 6e74 6174 696f  emy decumentatio
+000127c0: 6e20 666f 7220 7468 6520 6073 6573 7369  n for the `sessi
+000127d0: 6f6e 2065 7665 6e74 7320 3c68 7474 7073  on events <https
+000127e0: 3a2f 2f64 6f63 732e 7371 6c61 6c63 6865  ://docs.sqlalche
+000127f0: 6d79 2e6f 7267 2f65 6e2f 3134 2f6f 726d  my.org/en/14/orm
+00012800: 2f65 7665 6e74 732e 6874 6d6c 2373 6573  /events.html#ses
+00012810: 7369 6f6e 2d65 7665 6e74 733e 605f 0a    sion-events>`_.
```

### Comparing `AnyBlok-2.0.0/doc/ROADMAP.rst` & `AnyBlok-2.1.0/doc/ROADMAP.rst`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/doc/advanced_topics.rst` & `AnyBlok-2.1.0/doc/advanced_topics.rst`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/doc/basic_usage.rst` & `AnyBlok-2.1.0/doc/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/doc/builtin_bloks.rst` & `AnyBlok-2.1.0/doc/builtin_bloks.rst`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/doc/index.rst` & `AnyBlok-2.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/doc/internals.rst` & `AnyBlok-2.1.0/doc/internals.rst`

 * *Files identical despite different names*

### Comparing `AnyBlok-2.0.0/pyproject.toml` & `AnyBlok-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "AnyBlok"
 description = "Anyblok is a dynamic injection blok framework"
 authors = [
     { name = "Jean-Sébastien Suzanne", email = "jssuzanne@anybox.fr" },
 ]
-version = "2.0.0"
+version = "2.1.0"
 license = { text = "MPL2" }
 requires-python = ">=3.7"
 dependencies = [
     'sqlalchemy >= 2.0',
     'sqlalchemy-utils >= 0.40',
     'sqlalchemy-views >= 0.3.2',
     'packaging',
```

