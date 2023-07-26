# Comparing `tmp/APIFlask-1.3.1.tar.gz` & `tmp/APIFlask-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "APIFlask-1.3.1.tar", last modified: Mon Mar 27 13:35:51 2023, max compression
+gzip compressed data, was "APIFlask-2.0.0.tar", last modified: Wed Jul 26 00:36:24 2023, max compression
```

## Comparing `APIFlask-1.3.1.tar` & `APIFlask-2.0.0.tar`

### file list

```diff
@@ -1,100 +1,102 @@
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.837678 APIFlask-1.3.1/
--rw-r--r--   0 greyli    (1000) greyli    (1000)    24964 2023-03-27 13:34:42.000000 APIFlask-1.3.1/CHANGES.md
--rw-r--r--   0 greyli    (1000) greyli    (1000)     1064 2023-03-18 02:53:33.000000 APIFlask-1.3.1/LICENSE
--rw-r--r--   0 greyli    (1000) greyli    (1000)      207 2023-03-18 02:53:33.000000 APIFlask-1.3.1/MANIFEST.in
--rw-r--r--   0 greyli    (1000) greyli    (1000)     3712 2023-03-18 02:53:33.000000 APIFlask-1.3.1/NOTICE
--rw-r--r--   0 greyli    (1000) greyli    (1000)    10116 2023-03-27 13:35:51.837678 APIFlask-1.3.1/PKG-INFO
--rw-r--r--   0 greyli    (1000) greyli    (1000)     8695 2023-03-27 13:34:17.000000 APIFlask-1.3.1/README.md
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.827678 APIFlask-1.3.1/examples/
--rw-r--r--   0 greyli    (1000) greyli    (1000)     3805 2023-03-18 09:32:50.000000 APIFlask-1.3.1/examples/README.md
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.827678 APIFlask-1.3.1/examples/auth/
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.827678 APIFlask-1.3.1/examples/auth/basic_auth/
--rw-r--r--   0 greyli    (1000) greyli    (1000)      624 2023-03-18 02:53:33.000000 APIFlask-1.3.1/examples/auth/basic_auth/app.py
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.827678 APIFlask-1.3.1/examples/auth/token_auth/
--rw-r--r--   0 greyli    (1000) greyli    (1000)     1516 2023-03-18 02:53:33.000000 APIFlask-1.3.1/examples/auth/token_auth/app.py
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.827678 APIFlask-1.3.1/examples/base_response/
--rw-r--r--   0 greyli    (1000) greyli    (1000)     2287 2023-03-18 02:53:33.000000 APIFlask-1.3.1/examples/base_response/app.py
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.827678 APIFlask-1.3.1/examples/basic/
--rw-r--r--   0 greyli    (1000) greyli    (1000)     1595 2023-03-27 12:34:54.000000 APIFlask-1.3.1/examples/basic/app.py
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.827678 APIFlask-1.3.1/examples/blueprint_tags/
--rwxr-xr-x   0 greyli    (1000) greyli    (1000)     2320 2023-03-18 02:53:33.000000 APIFlask-1.3.1/examples/blueprint_tags/app.py
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.827678 APIFlask-1.3.1/examples/cbv/
--rw-r--r--   0 greyli    (1000) greyli    (1000)     1977 2023-03-18 02:53:33.000000 APIFlask-1.3.1/examples/cbv/app.py
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.827678 APIFlask-1.3.1/examples/dataclass/
--rw-r--r--   0 greyli    (1000) greyli    (1000)     1895 2023-03-18 02:53:33.000000 APIFlask-1.3.1/examples/dataclass/app.py
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.827678 APIFlask-1.3.1/examples/openapi/
--rwxr-xr-x   0 greyli    (1000) greyli    (1000)     5615 2023-03-18 02:53:33.000000 APIFlask-1.3.1/examples/openapi/app.py
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.827678 APIFlask-1.3.1/examples/orm/
--rw-r--r--   0 greyli    (1000) greyli    (1000)     2002 2023-03-18 02:53:33.000000 APIFlask-1.3.1/examples/orm/app.py
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.827678 APIFlask-1.3.1/examples/pagination/
--rw-r--r--   0 greyli    (1000) greyli    (1000)     1649 2023-03-18 02:53:33.000000 APIFlask-1.3.1/examples/pagination/app.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)       56 2023-03-18 02:53:33.000000 APIFlask-1.3.1/examples/requirements.txt
--rw-r--r--   0 greyli    (1000) greyli    (1000)     5384 2023-03-18 02:53:33.000000 APIFlask-1.3.1/examples/test_examples.py
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.827678 APIFlask-1.3.1/requirements/
--rw-r--r--   0 greyli    (1000) greyli    (1000)     1065 2023-03-18 09:32:50.000000 APIFlask-1.3.1/requirements/dev.txt
--rw-r--r--   0 greyli    (1000) greyli    (1000)     1681 2023-03-18 09:32:50.000000 APIFlask-1.3.1/requirements/docs.txt
--rw-r--r--   0 greyli    (1000) greyli    (1000)     1042 2023-03-18 09:32:50.000000 APIFlask-1.3.1/requirements/examples.txt
--rw-r--r--   0 greyli    (1000) greyli    (1000)     1245 2023-03-18 09:32:50.000000 APIFlask-1.3.1/requirements/tests.txt
--rw-r--r--   0 greyli    (1000) greyli    (1000)      299 2023-03-18 09:32:50.000000 APIFlask-1.3.1/requirements/typing.txt
--rw-r--r--   0 greyli    (1000) greyli    (1000)     2509 2023-03-27 13:35:51.837678 APIFlask-1.3.1/setup.cfg
--rw-r--r--   0 greyli    (1000) greyli    (1000)      558 2023-03-27 12:46:27.000000 APIFlask-1.3.1/setup.py
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.827678 APIFlask-1.3.1/src/
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.827678 APIFlask-1.3.1/src/APIFlask.egg-info/
--rw-r--r--   0 greyli    (1000) greyli    (1000)    10116 2023-03-27 13:35:51.000000 APIFlask-1.3.1/src/APIFlask.egg-info/PKG-INFO
--rw-r--r--   0 greyli    (1000) greyli    (1000)     2000 2023-03-27 13:35:51.000000 APIFlask-1.3.1/src/APIFlask.egg-info/SOURCES.txt
--rw-r--r--   0 greyli    (1000) greyli    (1000)        1 2023-03-27 13:35:51.000000 APIFlask-1.3.1/src/APIFlask.egg-info/dependency_links.txt
--rw-r--r--   0 greyli    (1000) greyli    (1000)      101 2023-03-27 13:35:51.000000 APIFlask-1.3.1/src/APIFlask.egg-info/entry_points.txt
--rw-r--r--   0 greyli    (1000) greyli    (1000)      189 2023-03-27 13:35:51.000000 APIFlask-1.3.1/src/APIFlask.egg-info/requires.txt
--rw-r--r--   0 greyli    (1000) greyli    (1000)        9 2023-03-27 13:35:51.000000 APIFlask-1.3.1/src/APIFlask.egg-info/top_level.txt
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.837678 APIFlask-1.3.1/src/apiflask/
--rw-r--r--   0 greyli    (1000) greyli    (1000)      593 2023-03-27 13:34:49.000000 APIFlask-1.3.1/src/apiflask/__init__.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)    52854 2023-03-27 13:34:17.000000 APIFlask-1.3.1/src/apiflask/app.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     2494 2023-03-18 02:53:33.000000 APIFlask-1.3.1/src/apiflask/blueprint.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     1388 2023-03-18 02:53:33.000000 APIFlask-1.3.1/src/apiflask/commands.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     4839 2023-03-18 09:32:50.000000 APIFlask-1.3.1/src/apiflask/exceptions.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     4385 2023-03-18 02:53:33.000000 APIFlask-1.3.1/src/apiflask/fields.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     3017 2023-03-18 02:53:33.000000 APIFlask-1.3.1/src/apiflask/helpers.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     6882 2023-03-18 09:32:50.000000 APIFlask-1.3.1/src/apiflask/openapi.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)        0 2023-03-18 02:53:33.000000 APIFlask-1.3.1/src/apiflask/py.typed
--rw-r--r--   0 greyli    (1000) greyli    (1000)     4778 2023-03-18 02:53:33.000000 APIFlask-1.3.1/src/apiflask/route.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)    22706 2023-03-18 09:32:50.000000 APIFlask-1.3.1/src/apiflask/scaffold.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     2200 2023-03-18 02:53:33.000000 APIFlask-1.3.1/src/apiflask/schemas.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     5881 2023-03-18 09:32:50.000000 APIFlask-1.3.1/src/apiflask/security.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     3118 2023-03-18 09:32:50.000000 APIFlask-1.3.1/src/apiflask/settings.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     2477 2023-03-18 02:53:33.000000 APIFlask-1.3.1/src/apiflask/types.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     8155 2023-03-18 09:32:50.000000 APIFlask-1.3.1/src/apiflask/ui_templates.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)      626 2023-03-18 02:53:33.000000 APIFlask-1.3.1/src/apiflask/validators.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     6861 2023-03-18 02:53:33.000000 APIFlask-1.3.1/src/apiflask/views.py
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.837678 APIFlask-1.3.1/tests/
--rw-r--r--   0 greyli    (1000) greyli    (1000)        0 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/__init__.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)      428 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/conftest.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     1452 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/schemas.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     9055 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_app.py
-drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-03-27 13:35:51.837678 APIFlask-1.3.1/tests/test_apps/
--rw-r--r--   0 greyli    (1000) greyli    (1000)        0 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_apps/__init__.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     2779 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_async.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     4533 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_base_response.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     2142 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_blueprint.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     2432 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_commands.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     7279 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_decorator_auth_required.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     9423 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_decorator_doc.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)    11775 2023-03-18 09:32:50.000000 APIFlask-1.3.1/tests/test_decorator_input.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     9386 2023-03-18 09:32:50.000000 APIFlask-1.3.1/tests/test_decorator_output.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     1064 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_decorators.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     4071 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_exceptions.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     2313 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_fields.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     1664 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_helpers.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     7500 2023-03-18 09:32:50.000000 APIFlask-1.3.1/tests/test_openapi_basic.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     4869 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_openapi_blueprint.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     3254 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_openapi_info.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     7963 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_openapi_paths.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     4492 2023-03-18 09:32:50.000000 APIFlask-1.3.1/tests/test_openapi_security.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     4756 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_openapi_tags.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     6632 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_route.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     3780 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_security.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     5539 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_settings_api_docs.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)    11252 2023-03-18 09:32:50.000000 APIFlask-1.3.1/tests/test_settings_auto_behaviour.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     4683 2023-03-18 09:32:50.000000 APIFlask-1.3.1/tests/test_settings_openapi_fields.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     2188 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_settings_openapi_spec.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)     5363 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tests/test_settings_response_customization.py
--rw-r--r--   0 greyli    (1000) greyli    (1000)      661 2023-03-18 02:53:33.000000 APIFlask-1.3.1/tox.ini
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    26285 2023-07-26 00:33:03.000000 APIFlask-2.0.0/CHANGES.md
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1064 2023-03-18 02:53:33.000000 APIFlask-2.0.0/LICENSE
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      207 2023-03-18 02:53:33.000000 APIFlask-2.0.0/MANIFEST.in
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     3712 2023-03-18 02:53:33.000000 APIFlask-2.0.0/NOTICE
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    10388 2023-07-26 00:36:24.484555 APIFlask-2.0.0/PKG-INFO
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     8858 2023-07-26 00:26:54.000000 APIFlask-2.0.0/README.md
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/examples/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     3805 2023-07-15 10:14:48.000000 APIFlask-2.0.0/examples/README.md
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/examples/auth/
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/examples/auth/basic_auth/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      624 2023-03-18 02:53:33.000000 APIFlask-2.0.0/examples/auth/basic_auth/app.py
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/examples/auth/token_auth/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1516 2023-03-18 02:53:33.000000 APIFlask-2.0.0/examples/auth/token_auth/app.py
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/examples/base_response/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2346 2023-07-15 15:10:37.000000 APIFlask-2.0.0/examples/base_response/app.py
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/examples/basic/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1654 2023-07-22 04:41:21.000000 APIFlask-2.0.0/examples/basic/app.py
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/examples/blueprint_tags/
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     2294 2023-07-15 15:10:37.000000 APIFlask-2.0.0/examples/blueprint_tags/app.py
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/examples/cbv/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2033 2023-07-15 15:10:37.000000 APIFlask-2.0.0/examples/cbv/app.py
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/examples/dataclass/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1961 2023-07-15 15:10:37.000000 APIFlask-2.0.0/examples/dataclass/app.py
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/examples/openapi/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    53248 2023-07-22 03:04:05.000000 APIFlask-2.0.0/examples/openapi/.coverage
+-rwxr-xr-x   0 greyli    (1000) greyli    (1000)     5478 2023-07-18 14:47:48.000000 APIFlask-2.0.0/examples/openapi/app.py
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/examples/orm/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2070 2023-07-15 15:21:33.000000 APIFlask-2.0.0/examples/orm/app.py
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/examples/pagination/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1699 2023-07-15 15:21:33.000000 APIFlask-2.0.0/examples/pagination/app.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)       56 2023-03-18 02:53:33.000000 APIFlask-2.0.0/examples/requirements.txt
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     5384 2023-03-18 02:53:33.000000 APIFlask-2.0.0/examples/test_examples.py
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/requirements/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1064 2023-07-15 15:21:33.000000 APIFlask-2.0.0/requirements/dev.txt
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1673 2023-07-15 15:21:33.000000 APIFlask-2.0.0/requirements/docs.txt
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1074 2023-07-15 15:21:33.000000 APIFlask-2.0.0/requirements/examples.txt
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1651 2023-07-15 15:21:33.000000 APIFlask-2.0.0/requirements/tests.txt
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      299 2023-07-15 15:21:33.000000 APIFlask-2.0.0/requirements/typing.txt
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2625 2023-07-26 00:36:24.484555 APIFlask-2.0.0/setup.cfg
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      503 2023-07-15 15:21:33.000000 APIFlask-2.0.0/setup.py
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/src/
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/src/APIFlask.egg-info/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    10388 2023-07-26 00:36:24.000000 APIFlask-2.0.0/src/APIFlask.egg-info/PKG-INFO
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2049 2023-07-26 00:36:24.000000 APIFlask-2.0.0/src/APIFlask.egg-info/SOURCES.txt
+-rw-r--r--   0 greyli    (1000) greyli    (1000)        1 2023-07-26 00:36:24.000000 APIFlask-2.0.0/src/APIFlask.egg-info/dependency_links.txt
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      101 2023-07-26 00:36:24.000000 APIFlask-2.0.0/src/APIFlask.egg-info/entry_points.txt
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      142 2023-07-26 00:36:24.000000 APIFlask-2.0.0/src/APIFlask.egg-info/requires.txt
+-rw-r--r--   0 greyli    (1000) greyli    (1000)        9 2023-07-26 00:36:24.000000 APIFlask-2.0.0/src/APIFlask.egg-info/top_level.txt
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/src/apiflask/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      687 2023-07-26 00:29:21.000000 APIFlask-2.0.0/src/apiflask/__init__.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    49430 2023-07-25 01:43:43.000000 APIFlask-2.0.0/src/apiflask/app.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2494 2023-07-24 14:14:06.000000 APIFlask-2.0.0/src/apiflask/blueprint.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1388 2023-03-18 02:53:33.000000 APIFlask-2.0.0/src/apiflask/commands.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     4849 2023-06-15 13:08:29.000000 APIFlask-2.0.0/src/apiflask/exceptions.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     4432 2023-07-15 15:10:37.000000 APIFlask-2.0.0/src/apiflask/fields.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     3017 2023-03-18 02:53:33.000000 APIFlask-2.0.0/src/apiflask/helpers.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     7128 2023-07-17 15:03:25.000000 APIFlask-2.0.0/src/apiflask/openapi.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)        0 2023-03-18 02:53:33.000000 APIFlask-2.0.0/src/apiflask/py.typed
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     4186 2023-07-15 15:10:37.000000 APIFlask-2.0.0/src/apiflask/route.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    22380 2023-07-23 03:56:05.000000 APIFlask-2.0.0/src/apiflask/scaffold.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     3983 2023-07-17 15:03:25.000000 APIFlask-2.0.0/src/apiflask/schemas.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     5881 2023-03-18 09:32:50.000000 APIFlask-2.0.0/src/apiflask/security.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     3118 2023-03-18 09:32:50.000000 APIFlask-2.0.0/src/apiflask/settings.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2477 2023-03-18 02:53:33.000000 APIFlask-2.0.0/src/apiflask/types.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     8155 2023-07-24 14:14:06.000000 APIFlask-2.0.0/src/apiflask/ui_templates.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      626 2023-03-18 02:53:33.000000 APIFlask-2.0.0/src/apiflask/validators.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)       86 2023-07-15 15:10:37.000000 APIFlask-2.0.0/src/apiflask/views.py
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/tests/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)        0 2023-03-18 02:53:33.000000 APIFlask-2.0.0/tests/__init__.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      428 2023-03-18 02:53:33.000000 APIFlask-2.0.0/tests/conftest.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1596 2023-07-23 03:56:05.000000 APIFlask-2.0.0/tests/schemas.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     9200 2023-07-15 15:10:37.000000 APIFlask-2.0.0/tests/test_app.py
+drwxr-xr-x   0 greyli    (1000) greyli    (1000)        0 2023-07-26 00:36:24.484555 APIFlask-2.0.0/tests/test_apps/
+-rw-r--r--   0 greyli    (1000) greyli    (1000)        0 2023-03-18 02:53:33.000000 APIFlask-2.0.0/tests/test_apps/__init__.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2625 2023-07-15 15:10:37.000000 APIFlask-2.0.0/tests/test_async.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     4533 2023-03-18 02:53:33.000000 APIFlask-2.0.0/tests/test_base_response.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2139 2023-07-15 15:10:37.000000 APIFlask-2.0.0/tests/test_blueprint.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2432 2023-03-18 02:53:33.000000 APIFlask-2.0.0/tests/test_commands.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     7276 2023-07-15 15:10:37.000000 APIFlask-2.0.0/tests/test_decorator_auth_required.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    12116 2023-07-23 03:56:05.000000 APIFlask-2.0.0/tests/test_decorator_doc.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    11701 2023-07-18 14:47:48.000000 APIFlask-2.0.0/tests/test_decorator_input.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     9423 2023-07-16 05:03:17.000000 APIFlask-2.0.0/tests/test_decorator_output.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      411 2023-07-23 03:56:05.000000 APIFlask-2.0.0/tests/test_decorators.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     4071 2023-03-18 02:53:33.000000 APIFlask-2.0.0/tests/test_exceptions.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2303 2023-07-15 15:10:37.000000 APIFlask-2.0.0/tests/test_fields.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1664 2023-03-18 02:53:33.000000 APIFlask-2.0.0/tests/test_helpers.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     7459 2023-07-23 03:56:05.000000 APIFlask-2.0.0/tests/test_openapi_basic.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     4457 2023-07-23 03:56:05.000000 APIFlask-2.0.0/tests/test_openapi_blueprint.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     3254 2023-03-18 02:53:33.000000 APIFlask-2.0.0/tests/test_openapi_info.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     8026 2023-07-15 15:10:37.000000 APIFlask-2.0.0/tests/test_openapi_paths.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     4492 2023-03-18 09:32:50.000000 APIFlask-2.0.0/tests/test_openapi_security.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     4581 2023-07-03 14:11:24.000000 APIFlask-2.0.0/tests/test_openapi_tags.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     6307 2023-07-15 15:10:37.000000 APIFlask-2.0.0/tests/test_route.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     1531 2023-07-17 15:03:25.000000 APIFlask-2.0.0/tests/test_schemas.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     3780 2023-03-18 02:53:33.000000 APIFlask-2.0.0/tests/test_security.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     5752 2023-07-23 03:56:05.000000 APIFlask-2.0.0/tests/test_settings_api_docs.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)    11249 2023-07-15 15:10:37.000000 APIFlask-2.0.0/tests/test_settings_auto_behaviour.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     4683 2023-03-18 09:32:50.000000 APIFlask-2.0.0/tests/test_settings_openapi_fields.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     2188 2023-03-18 02:53:33.000000 APIFlask-2.0.0/tests/test_settings_openapi_spec.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)     5356 2023-07-17 15:03:25.000000 APIFlask-2.0.0/tests/test_settings_response_customization.py
+-rw-r--r--   0 greyli    (1000) greyli    (1000)      668 2023-07-26 00:26:33.000000 APIFlask-2.0.0/tox.ini
```

### Comparing `APIFlask-1.3.1/CHANGES.md` & `APIFlask-2.0.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+## Version 2.0.0
+
+Released: 2023/7/26<br>Codename: Gongqing
+
+Please see the [migration guide](/migration_guide/#migrate-to-apiflask-2x) for APIFlask 2.0.0 version.
+
+- Drop Python 3.7 support.
+- Drop Flask 1.x support ([issue #442][issue_442]).
+- Only pass keyword arguments to the view function. The argument name
+  of the parsed data from `app.input()` will be `{location}_data` or the
+  value of `arg_name` ([issue #427][issue_427]).
+- Add `FileSchema` to generate OpenAPI file response ([issue #447][issue_447]).
+- Support using `{}` to represent not only empty body (204) but also empty schema.
+  Use `{}` or `EmptySchema` will not set the status code to 204 anymore.
+- Remove the previously deprecated code:
+    - The `tag` parameter in `@app.doc`.
+    - The `role` parameter in `@app.auth_required`.
+    - The `redoc_path` parameter in `apiflask.APIFlask` and the `/redoc` path.
+- Support setting a complete response OpenAPI spec throught the `app.doc(responses)`
+  parameter (i.e. `responses={400: {'description': '', 'content': ...}}`)
+  ([issue #327][issue_327]).
+
+[issue_327]: https://github.com/apiflask/apiflask/issues/327
+[issue_427]: https://github.com/apiflask/apiflask/issues/427
+[issue_442]: https://github.com/apiflask/apiflask/issues/442
+[issue_447]: https://github.com/apiflask/apiflask/issues/447
+
+
 ## Version 1.3.1
 
 Released: 2023/3/27
 
 - Fix the import error when calling `apispec.yaml_utils.dict_to_yaml`
   ([issue #419][issue_419]).
 
@@ -120,15 +148,15 @@
 
 - Add a versioned docs for 1.x releases (https://v1.apiflask.com).
 - Allow the view function to return a list as JSON response ([issue #321][issue_321]).
 - Add new docs UI support: RapiDoc, RapiPDF, and Elements ([pr #308][pr_308]).
 - Add a `docs_ui` parameter to APIFlask to set the API docs UI (can be
   `swagger-ui` (default), `redoc`, `rapidoc`, and `rapipdf`).
 - Deprecate the separate docs path `/redoc` and the `redoc_path` parameter.
-- Add the following configuration variables for new docs supprt:
+- Add the following configuration variables for new docs support:
     - `ELEMENTS_JS`
     - `ELEMENTS_CSS`
     - `ELEMENTS_LAYOUT`
     - `ELEMENTS_CONFIG`
     - `RAPIDOC_JS`
     - `RAPIDOC_THEME`
     - `RAPIDOC_CONFIG`
```

### Comparing `APIFlask-1.3.1/LICENSE` & `APIFlask-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/NOTICE` & `APIFlask-2.0.0/NOTICE`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/PKG-INFO` & `APIFlask-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: APIFlask
-Version: 1.3.1
+Version: 2.0.0
 Summary: A lightweight web API framework based on Flask and marshmallow-code projects.
 Home-page: https://apiflask.com
 Author: Grey Li
 Author-email: withlihui@gmail.com
 License: MIT
 Project-URL: Documentation, https://apiflask.com/docs
 Project-URL: Source, https://github.com/apiflask/apiflask
 Project-URL: Changelog, https://apiflask.com/changelog
 Project-URL: Issue Tracker, https://github.com/apiflask/apiflask/issues
+Project-URL: Donate, https://opencollective.com/apiflask
 Keywords: flask,marshmallow,openapi
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: async
 Provides-Extra: dotenv
 Provides-Extra: yaml
 License-File: LICENSE
 License-File: NOTICE
 
@@ -52,16 +54,16 @@
 - Automatic interactive API documentation
 - API authentication support (with [Flask-HTTPAuth](https://github.com/miguelgrinberg/flask-httpauth))
 - Automatic JSON response for HTTP errors
 
 
 ## Requirements
 
-- Python 3.7+
-- Flask 1.1.0+
+- Python 3.8+
+- Flask 2.0+
 
 
 ## Installation
 
 For Linux and macOS:
 
 ```bash
@@ -81,14 +83,20 @@
 - Documentation: <https://apiflask.com/docs>
 - PyPI Releases: <https://pypi.python.org/pypi/APIFlask>
 - Change Log: <https://apiflask.com/changelog>
 - Source Code: <https://github.com/apiflask/apiflask>
 - Issue Tracker: <https://github.com/apiflask/apiflask/issues>
 - Discussion: <https://github.com/apiflask/apiflask/discussions>
 - Twitter: <https://twitter.com/apiflask>
+- Open Collective: <https://opencollective.com/apiflask>
+
+
+## Donate
+
+If you find APIFlask useful, please consider [donating](https://opencollective.com/apiflask) today. Your donation keeps APIFlask maintained and evolving.
 
 
 ## Example
 
 ```python
 from apiflask import APIFlask, Schema, abort
 from apiflask.fields import Integer, String
@@ -128,32 +136,32 @@
     # APIFlask will serialize the object into JSON format
     return pets[pet_id]
 
 
 @app.patch('/pets/<int:pet_id>')
 @app.input(PetIn(partial=True))
 @app.output(PetOut)
-def update_pet(pet_id, data):
+def update_pet(pet_id, json_data):
     # the validated and parsed input data will
     # be injected into the view function as a dict
     if pet_id > len(pets) - 1:
         abort(404)
-    for attr, value in data.items():
+    for attr, value in json_data.items():
         pets[pet_id][attr] = value
     return pets[pet_id]
 ```
 
 <details>
 <summary>You can also use class-based views based on <code>MethodView</code></summary>
 
 ```python
 from apiflask import APIFlask, Schema, abort
 from apiflask.fields import Integer, String
 from apiflask.validators import Length, OneOf
-from apiflask.views import MethodView
+from flask.views import MethodView
 
 app = APIFlask(__name__)
 
 pets = [
     {'id': 0, 'name': 'Kitty', 'category': 'cat'},
     {'id': 1, 'name': 'Coco', 'category': 'dog'}
 ]
@@ -184,30 +192,30 @@
         """Get a pet"""
         if pet_id > len(pets) - 1:
             abort(404)
         return pets[pet_id]
 
     @app.input(PetIn(partial=True))
     @app.output(PetOut)
-    def patch(self, pet_id, data):
+    def patch(self, pet_id, json_data):
         """Update a pet"""
         if pet_id > len(pets) - 1:
             abort(404)
-        for attr, value in data.items():
+        for attr, value in json_data.items():
             pets[pet_id][attr] = value
         return pets[pet_id]
 
 
 app.add_url_rule('/', view_func=Hello.as_view('hello'))
 app.add_url_rule('/pets/<int:pet_id>', view_func=Pet.as_view('pet'))
 ```
 </details>
 
 <details>
-<summary>Or use <code>async def</code> with Flask 2.0</summary>
+<summary>Or use <code>async def</code></summary>
 
 ```bash
 $ pip install -U "apiflask[async]"
 ```
 
 ```python
 import asyncio
@@ -270,35 +278,36 @@
 
 ## Relationship with Flask
 
 APIFlask is a thin wrapper on top of Flask. You only need to remember the following differences (see *[Migrating from Flask](https://apiflask.com/migrating)* for more details):
 
 - When creating an application instance, use `APIFlask` instead of `Flask`.
 - When creating a blueprint instance, use `APIBlueprint` instead of `Blueprint`.
-- When creating a class-based view, use `apiflask.views.MethodView` instead of `flask.views.MethodView`.
 - The `abort()` function from APIFlask (`apiflask.abort`) returns JSON error response.
 
 For a minimal Flask application:
 
 ```python
-from flask import Flask, request, escape
+from flask import Flask, request
+from markupsafe import escape
 
 app = Flask(__name__)
 
 @app.route('/')
 def hello():
     name = request.args.get('name', 'Human')
     return f'Hello, {escape(name)}'
 ```
 
 Now change to APIFlask:
 
 ```python
 from apiflask import APIFlask  # step one
-from flask import request, escape
+from flask import request
+from markupsafe import escape
 
 app = APIFlask(__name__)  # step two
 
 @app.route('/')
 def hello():
     name = request.args.get('name', 'Human')
     return f'Hello, {escape(name)}'
```

### Comparing `APIFlask-1.3.1/README.md` & `APIFlask-2.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 - Automatic interactive API documentation
 - API authentication support (with [Flask-HTTPAuth](https://github.com/miguelgrinberg/flask-httpauth))
 - Automatic JSON response for HTTP errors
 
 
 ## Requirements
 
-- Python 3.7+
-- Flask 1.1.0+
+- Python 3.8+
+- Flask 2.0+
 
 
 ## Installation
 
 For Linux and macOS:
 
 ```bash
@@ -45,14 +45,20 @@
 - Documentation: <https://apiflask.com/docs>
 - PyPI Releases: <https://pypi.python.org/pypi/APIFlask>
 - Change Log: <https://apiflask.com/changelog>
 - Source Code: <https://github.com/apiflask/apiflask>
 - Issue Tracker: <https://github.com/apiflask/apiflask/issues>
 - Discussion: <https://github.com/apiflask/apiflask/discussions>
 - Twitter: <https://twitter.com/apiflask>
+- Open Collective: <https://opencollective.com/apiflask>
+
+
+## Donate
+
+If you find APIFlask useful, please consider [donating](https://opencollective.com/apiflask) today. Your donation keeps APIFlask maintained and evolving.
 
 
 ## Example
 
 ```python
 from apiflask import APIFlask, Schema, abort
 from apiflask.fields import Integer, String
@@ -92,32 +98,32 @@
     # APIFlask will serialize the object into JSON format
     return pets[pet_id]
 
 
 @app.patch('/pets/<int:pet_id>')
 @app.input(PetIn(partial=True))
 @app.output(PetOut)
-def update_pet(pet_id, data):
+def update_pet(pet_id, json_data):
     # the validated and parsed input data will
     # be injected into the view function as a dict
     if pet_id > len(pets) - 1:
         abort(404)
-    for attr, value in data.items():
+    for attr, value in json_data.items():
         pets[pet_id][attr] = value
     return pets[pet_id]
 ```
 
 <details>
 <summary>You can also use class-based views based on <code>MethodView</code></summary>
 
 ```python
 from apiflask import APIFlask, Schema, abort
 from apiflask.fields import Integer, String
 from apiflask.validators import Length, OneOf
-from apiflask.views import MethodView
+from flask.views import MethodView
 
 app = APIFlask(__name__)
 
 pets = [
     {'id': 0, 'name': 'Kitty', 'category': 'cat'},
     {'id': 1, 'name': 'Coco', 'category': 'dog'}
 ]
@@ -148,30 +154,30 @@
         """Get a pet"""
         if pet_id > len(pets) - 1:
             abort(404)
         return pets[pet_id]
 
     @app.input(PetIn(partial=True))
     @app.output(PetOut)
-    def patch(self, pet_id, data):
+    def patch(self, pet_id, json_data):
         """Update a pet"""
         if pet_id > len(pets) - 1:
             abort(404)
-        for attr, value in data.items():
+        for attr, value in json_data.items():
             pets[pet_id][attr] = value
         return pets[pet_id]
 
 
 app.add_url_rule('/', view_func=Hello.as_view('hello'))
 app.add_url_rule('/pets/<int:pet_id>', view_func=Pet.as_view('pet'))
 ```
 </details>
 
 <details>
-<summary>Or use <code>async def</code> with Flask 2.0</summary>
+<summary>Or use <code>async def</code></summary>
 
 ```bash
 $ pip install -U "apiflask[async]"
 ```
 
 ```python
 import asyncio
@@ -234,35 +240,36 @@
 
 ## Relationship with Flask
 
 APIFlask is a thin wrapper on top of Flask. You only need to remember the following differences (see *[Migrating from Flask](https://apiflask.com/migrating)* for more details):
 
 - When creating an application instance, use `APIFlask` instead of `Flask`.
 - When creating a blueprint instance, use `APIBlueprint` instead of `Blueprint`.
-- When creating a class-based view, use `apiflask.views.MethodView` instead of `flask.views.MethodView`.
 - The `abort()` function from APIFlask (`apiflask.abort`) returns JSON error response.
 
 For a minimal Flask application:
 
 ```python
-from flask import Flask, request, escape
+from flask import Flask, request
+from markupsafe import escape
 
 app = Flask(__name__)
 
 @app.route('/')
 def hello():
     name = request.args.get('name', 'Human')
     return f'Hello, {escape(name)}'
 ```
 
 Now change to APIFlask:
 
 ```python
 from apiflask import APIFlask  # step one
-from flask import request, escape
+from flask import request
+from markupsafe import escape
 
 app = APIFlask(__name__)  # step two
 
 @app.route('/')
 def hello():
     name = request.args.get('name', 'Human')
     return f'Hello, {escape(name)}'
```

### Comparing `APIFlask-1.3.1/examples/README.md` & `APIFlask-2.0.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/examples/auth/basic_auth/app.py` & `APIFlask-2.0.0/examples/auth/basic_auth/app.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/examples/auth/token_auth/app.py` & `APIFlask-2.0.0/examples/auth/token_auth/app.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/examples/base_response/app.py` & `APIFlask-2.0.0/examples/basic/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,13 @@
 from apiflask import APIFlask, Schema, abort
-from apiflask.fields import Integer, String, Field
+from apiflask.fields import Integer, String
 from apiflask.validators import Length, OneOf
 
 app = APIFlask(__name__)
 
-
-class BaseResponse(Schema):
-    data = Field()  # the data key
-    message = String()
-    code = Integer()
-
-
-app.config['BASE_RESPONSE_SCHEMA'] = BaseResponse
-# the data key should match the data field name in the base response schema
-# defaults to "data"
-app.config['BASE_RESPONSE_DATA_KEY '] = 'data'
-
 pets = [
     {'id': 0, 'name': 'Kitty', 'category': 'cat'},
     {'id': 1, 'name': 'Coco', 'category': 'dog'},
     {'id': 2, 'name': 'Flash', 'category': 'cat'}
 ]
 
 
@@ -32,71 +20,50 @@
     id = Integer()
     name = String()
     category = String()
 
 
 @app.get('/')
 def say_hello():
-    data = {'message': 'Hello!'}
-    return {
-        'data': data,
-        'message': 'Success!',
-        'code': 200
-    }
+    return {'message': 'Hello!'}
 
 
 @app.get('/pets/<int:pet_id>')
 @app.output(PetOut)
 def get_pet(pet_id):
     if pet_id > len(pets) - 1 or pets[pet_id].get('deleted'):
         abort(404)
-    return {
-        'data': pets[pet_id],
-        'message': 'Success!',
-        'code': 200,
-    }
+    return pets[pet_id]
 
 
 @app.get('/pets')
-@app.output(PetOut(many=True))
+@app.output(PetOut(many=True), content_type='image/png')
 def get_pets():
-    return {
-        'data': pets,
-        'message': 'Success!',
-        'code': 200,
-    }
+    return pets
 
 
 @app.post('/pets')
-@app.input(PetIn)
+@app.input(PetIn, location='json')
 @app.output(PetOut, status_code=201)
-def create_pet(data):
+def create_pet(json_data):
     pet_id = len(pets)
-    data['id'] = pet_id
-    pets.append(data)
-    return {
-        'data': pets[pet_id],
-        'message': 'Pet created.',
-        'code': 201
-    }
+    json_data['id'] = pet_id
+    pets.append(json_data)
+    return pets[pet_id]
 
 
 @app.patch('/pets/<int:pet_id>')
-@app.input(PetIn(partial=True))
+@app.input(PetIn(partial=True), location='json')
 @app.output(PetOut)
-def update_pet(pet_id, data):
+def update_pet(pet_id, json_data):
     if pet_id > len(pets) - 1:
         abort(404)
-    for attr, value in data.items():
+    for attr, value in json_data.items():
         pets[pet_id][attr] = value
-    return {
-        'data': pets[pet_id],
-        'message': 'Pet updated.',
-        'code': 200
-    }
+    return pets[pet_id]
 
 
 @app.delete('/pets/<int:pet_id>')
 @app.output({}, status_code=204)
 def delete_pet(pet_id):
     if pet_id > len(pets) - 1:
         abort(404)
```

### Comparing `APIFlask-1.3.1/examples/basic/app.py` & `APIFlask-2.0.0/examples/dataclass/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,82 @@
-from apiflask import APIFlask, Schema, abort
-from apiflask.fields import Integer, String
+from dataclasses import field
+
+from marshmallow_dataclass import dataclass
+from apiflask import APIFlask, abort
 from apiflask.validators import Length, OneOf
 
 app = APIFlask(__name__)
 
+
+@dataclass
+class PetIn:
+    name: str = field(
+        metadata={'required': True, 'validate': Length(min=1, max=10)}
+    )
+    category: str = field(
+        metadata={'required': True, 'validate': OneOf(['cat', 'dog'])}
+    )
+
+
+@dataclass
+class PetOut:
+    id: int
+    name: str
+    category: str
+
+
 pets = [
     {'id': 0, 'name': 'Kitty', 'category': 'cat'},
     {'id': 1, 'name': 'Coco', 'category': 'dog'},
     {'id': 2, 'name': 'Flash', 'category': 'cat'}
 ]
 
 
-class PetIn(Schema):
-    name = String(required=True, validate=Length(0, 10))
-    category = String(required=True, validate=OneOf(['dog', 'cat']))
-
-
-class PetOut(Schema):
-    id = Integer()
-    name = String()
-    category = String()
-
-
 @app.get('/')
 def say_hello():
     return {'message': 'Hello!'}
 
 
 @app.get('/pets/<int:pet_id>')
-@app.output(PetOut)
+@app.output(PetOut.Schema)
 def get_pet(pet_id):
     if pet_id > len(pets) - 1 or pets[pet_id].get('deleted'):
         abort(404)
     return pets[pet_id]
 
 
 @app.get('/pets')
-@app.output(PetOut(many=True), content_type='image/png')
+@app.output(PetOut.Schema(many=True))
 def get_pets():
     return pets
 
 
 @app.post('/pets')
-@app.input(PetIn)
-@app.output(PetOut, status_code=201)
-def create_pet(data):
+@app.input(PetIn.Schema, location='json', arg_name='pet')
+@app.output(PetOut.Schema, status_code=201)
+def create_pet(pet: PetIn):
     pet_id = len(pets)
-    data['id'] = pet_id
-    pets.append(data)
+    pets.append({
+        'id': pet_id,
+        'name': pet.name,
+        'category': pet.category
+    })
     return pets[pet_id]
 
 
+# partial=True is not supported in marshmallow-dataclass currently
+# https://github.com/lovasoa/marshmallow_dataclass/issues/169
 @app.patch('/pets/<int:pet_id>')
-@app.input(PetIn(partial=True))
-@app.output(PetOut)
-def update_pet(pet_id, data):
+@app.input(PetIn.Schema, location='json', arg_name='pet')
+@app.output(PetOut.Schema)
+def update_pet(pet_id, pet: PetIn):
     if pet_id > len(pets) - 1:
         abort(404)
-    for attr, value in data.items():
-        pets[pet_id][attr] = value
+    pets[pet_id]['name'] = pet.name
+    pets[pet_id]['category'] = pet.category
     return pets[pet_id]
 
 
 @app.delete('/pets/<int:pet_id>')
 @app.output({}, status_code=204)
 def delete_pet(pet_id):
     if pet_id > len(pets) - 1:
```

### Comparing `APIFlask-1.3.1/examples/blueprint_tags/app.py` & `APIFlask-2.0.0/examples/blueprint_tags/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-from apiflask import APIFlask, APIBlueprint, Schema, abort
-from apiflask.fields import Integer, String
-from apiflask.validators import Length, OneOf
-
-app = APIFlask(__name__)
-hello_bp = APIBlueprint('hello', __name__)  # tag name will be "Hello"
-pet_bp = APIBlueprint('pet', __name__)  # tag name will be "Pet"
-
-# The default tag is the blueprint name in title form. If you need to set a custom tag name:
-# hello_bp = APIBlueprint('hello', __name__, tag='NoHello')
-
-# If you need to set the tag "description" or "externalDocs", just pass a dict:
-# hello_bp = APIBlueprint('hello', __name__, tag={'name': 'Hello', 'description': '...'})
-# pet_bp = APIBlueprint('pet', __name__, tag={'name': 'Pet', 'description': '...'})
-
-pets = [
-    {'id': 0, 'name': 'Kitty', 'category': 'cat'},
-    {'id': 1, 'name': 'Coco', 'category': 'dog'},
-    {'id': 2, 'name': 'Flash', 'category': 'cat'}
-]
-
-
-class PetIn(Schema):
-    name = String(required=True, validate=Length(0, 10))
-    category = String(required=True, validate=OneOf(['dog', 'cat']))
-
-
-class PetOut(Schema):
-    id = Integer()
-    name = String()
-    category = String()
-
-
-@hello_bp.get('/')
-def say_hello():
-    return {'message': 'Hello!'}
-
-
-@pet_bp.get('/pets/<int:pet_id>')
-@pet_bp.output(PetOut)
-def get_pet(pet_id):
-    if pet_id > len(pets) - 1 or pets[pet_id].get('deleted'):
-        abort(404)
-    return pets[pet_id]
-
-
-@pet_bp.get('/pets')
-@pet_bp.output(PetOut(many=True))
-def get_pets():
-    return pets
-
-
-@pet_bp.post('/pets')
-@pet_bp.input(PetIn)
-@pet_bp.output(PetOut, status_code=201)
-def create_pet(data):
-    pet_id = len(pets)
-    data['id'] = pet_id
-    pets.append(data)
-    return pets[pet_id]
-
-
-@pet_bp.patch('/pets/<int:pet_id>')
-@pet_bp.input(PetIn(partial=True))
-@pet_bp.output(PetOut)
-def update_pet(pet_id, data):
-    if pet_id > len(pets) - 1:
-        abort(404)
-    for attr, value in data.items():
-        pets[pet_id][attr] = value
-    return pets[pet_id]
-
-
-@pet_bp.delete('/pets/<int:pet_id>')
-@pet_bp.output({}, status_code=204)
-def delete_pet(pet_id):
-    if pet_id > len(pets) - 1:
-        abort(404)
-    pets[pet_id]['deleted'] = True
-    pets[pet_id]['name'] = 'Ghost'
-    return ''
-
-
-app.register_blueprint(hello_bp)
-app.register_blueprint(pet_bp)
+from apiflask import APIFlask, APIBlueprint, Schema, abort
+from apiflask.fields import Integer, String
+from apiflask.validators import Length, OneOf
+
+app = APIFlask(__name__)
+hello_bp = APIBlueprint('hello', __name__)  # tag name will be "Hello"
+pet_bp = APIBlueprint('pet', __name__)  # tag name will be "Pet"
+
+# The default tag is the blueprint name in title form. If you need to set a custom tag name:
+# hello_bp = APIBlueprint('hello', __name__, tag='NoHello')
+
+# If you need to set the tag "description" or "externalDocs", just pass a dict:
+# hello_bp = APIBlueprint('hello', __name__, tag={'name': 'Hello', 'description': '...'})
+# pet_bp = APIBlueprint('pet', __name__, tag={'name': 'Pet', 'description': '...'})
+
+pets = [
+    {'id': 0, 'name': 'Kitty', 'category': 'cat'},
+    {'id': 1, 'name': 'Coco', 'category': 'dog'},
+    {'id': 2, 'name': 'Flash', 'category': 'cat'}
+]
+
+
+class PetIn(Schema):
+    name = String(required=True, validate=Length(0, 10))
+    category = String(required=True, validate=OneOf(['dog', 'cat']))
+
+
+class PetOut(Schema):
+    id = Integer()
+    name = String()
+    category = String()
+
+
+@hello_bp.get('/')
+def say_hello():
+    return {'message': 'Hello!'}
+
+
+@pet_bp.get('/pets/<int:pet_id>')
+@pet_bp.output(PetOut)
+def get_pet(pet_id):
+    if pet_id > len(pets) - 1 or pets[pet_id].get('deleted'):
+        abort(404)
+    return pets[pet_id]
+
+
+@pet_bp.get('/pets')
+@pet_bp.output(PetOut(many=True))
+def get_pets():
+    return pets
+
+
+@pet_bp.post('/pets')
+@pet_bp.input(PetIn, location='json')
+@pet_bp.output(PetOut, status_code=201)
+def create_pet(json_data):
+    pet_id = len(pets)
+    json_data['id'] = pet_id
+    pets.append(json_data)
+    return pets[pet_id]
+
+
+@pet_bp.patch('/pets/<int:pet_id>')
+@pet_bp.input(PetIn(partial=True), location='json')
+@pet_bp.output(PetOut)
+def update_pet(pet_id, json_data):
+    if pet_id > len(pets) - 1:
+        abort(404)
+    for attr, value in json_data.items():
+        pets[pet_id][attr] = value
+    return pets[pet_id]
+
+
+@pet_bp.delete('/pets/<int:pet_id>')
+@pet_bp.output({}, status_code=204)
+def delete_pet(pet_id):
+    if pet_id > len(pets) - 1:
+        abort(404)
+    pets[pet_id]['deleted'] = True
+    pets[pet_id]['name'] = 'Ghost'
+    return ''
+
+
+app.register_blueprint(hello_bp)
+app.register_blueprint(pet_bp)
```

### Comparing `APIFlask-1.3.1/examples/cbv/app.py` & `APIFlask-2.0.0/examples/cbv/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from apiflask import APIFlask, Schema, abort
 from apiflask.fields import Integer, String
 from apiflask.validators import Length, OneOf
-from apiflask.views import MethodView
+from flask.views import MethodView
 
 app = APIFlask(__name__)
 
 pets = [
     {'id': 0, 'name': 'Kitty', 'category': 'cat'},
     {'id': 1, 'name': 'Coco', 'category': 'dog'},
     {'id': 2, 'name': 'Flash', 'category': 'cat'}
@@ -34,21 +34,21 @@
     @app.output(PetOut)
     def get(self, pet_id):
         """Get a pet"""
         if pet_id > len(pets) - 1 or pets[pet_id].get('deleted'):
             abort(404)
         return pets[pet_id]
 
-    @app.input(PetIn(partial=True))
+    @app.input(PetIn(partial=True), location='json')
     @app.output(PetOut)
-    def patch(self, pet_id, data):
+    def patch(self, pet_id, json_data):
         """Update a pet"""
         if pet_id > len(pets) - 1:
             abort(404)
-        for attr, value in data.items():
+        for attr, value in json_data.items():
             pets[pet_id][attr] = value
         return pets[pet_id]
 
     @app.output({}, status_code=204)
     def delete(self, pet_id):
         """Delete a pet"""
         if pet_id > len(pets) - 1:
@@ -61,20 +61,20 @@
 class Pets(MethodView):
 
     @app.output(PetOut(many=True))
     def get(self):
         """Get all pets"""
         return pets
 
-    @app.input(PetIn)
+    @app.input(PetIn, location='json')
     @app.output(PetOut, status_code=201)
-    def post(self, data):
+    def post(self, json_data):
         """Create a pet"""
         pet_id = len(pets)
-        data['id'] = pet_id
-        pets.append(data)
+        json_data['id'] = pet_id
+        pets.append(json_data)
         return pets[pet_id]
 
 
 app.add_url_rule('/', view_func=Hello.as_view('hello'))
 app.add_url_rule('/pets/<int:pet_id>', view_func=Pet.as_view('pet'))
 app.add_url_rule('/pets', view_func=Pets.as_view('pets'))
```

### Comparing `APIFlask-1.3.1/examples/openapi/app.py` & `APIFlask-2.0.0/examples/openapi/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-from apiflask import APIFlask, Schema, abort
-from apiflask.fields import Integer, String
-from apiflask.validators import Length, OneOf
-
-# set openapi.info.title and openapi.info.version
-app = APIFlask(__name__, title='Pet API', version='1.0')
-
-# All the OpenAPI field config can be set with the corresponding attributes of the app instance:
-# app.description = '...'
-
-# openapi.info.description
-app.config['DESCRIPTION'] = """
-The description for this API. It can be very long and **Markdown** is supported.
-
-In this example, the tags is manually set. However, in a real world application, it will be
-enough to use the automatic tags feature based on blueprint, see the example for blueprint
-tags under the "examples/blueprint_tags" folder:
-
-```
-$ cd ..
-$ cd blueprint_tags
-$ flask run
-```
-
-The source can be found at [examples/blueprint_tags/app.py][_blueprint_tags].
-
-[_blueprint_tags]: https://github.com/apiflask/apiflask/tree/main/examples/blueprint_tags/app.py
-"""
-
-# openapi.info.contact
-app.config['CONTACT'] = {
-    'name': 'API Support',
-    'url': 'https://greyli.com/en',
-    'email': 'withlihui@gmail.com'
-}
-
-# openapi.info.license
-app.config['LICENSE'] = {
-    'name': 'MIT',
-    'url': 'https://opensource.org/licenses/MIT'
-}
-
-# openapi.info.termsOfService
-app.config['TERMS_OF_SERVICE'] = 'http://example.com'
-
-# The four info fields above can be set with the INFO key:
-# app.config['INFO'] = {
-#     'description': '...',
-#     'termsOfService': 'http://example.com',
-#     'contact': {
-#         'name': 'API Support',
-#         'url': 'http://www.example.com/support',
-#         'email': 'support@example.com'
-#     },
-#     'license': {
-#          'name': 'Apache 2.0',
-#          'url': 'http://www.apache.org/licenses/LICENSE-2.0.html'
-#      }
-# }
-
-# openapi.tags
-app.config['TAGS'] = [
-    {'name': 'Hello', 'description': 'The description of the **Hello** tag.'},
-    {'name': 'Pet', 'description': 'The description of the **Pet** tag.'}
-]
-
-# If you don't need to set tag "description" or tag "externalDocs", just pass a list a string:
-# app.config['TAGS'] = ['Hello', 'Pet']
-
-# openapi.servers
-app.config['SERVERS'] = [
-    {
-        'name': 'Development Server',
-        'url': 'http://localhost:5000'
-    },
-    {
-        'name': 'Production Server',
-        'url': 'http://api.example.com'
-    },
-    {
-        'name': 'Testing Server',
-        'url': 'http://test.example.com'
-    }
-]
-
-# openapi.externalDocs
-app.config['EXTERNAL_DOCS'] = {
-    'description': 'Find more info here',
-    'url': 'https://apiflask.com/docs'
-}
-
-pets = [
-    {'id': 0, 'name': 'Kitty', 'category': 'cat'},
-    {'id': 1, 'name': 'Coco', 'category': 'dog'},
-    {'id': 2, 'name': 'Flash', 'category': 'cat'}
-]
-
-
-class PetIn(Schema):
-    name = String(
-        required=True,
-        validate=Length(0, 10),
-        metadata={'title': 'Pet Name', 'description': 'The name of the pet.'}
-    )
-    category = String(
-        required=True,
-        validate=OneOf(['dog', 'cat']),
-        metadata={'title': 'Pet Category', 'description': 'The category of the pet.'}
-    )
-
-
-class PetOut(Schema):
-    id = Integer(metadata={'title': 'Pet ID', 'description': 'The ID of the pet.'})
-    name = String(metadata={'title': 'Pet Name', 'description': 'The name of the pet.'})
-    category = String(metadata={'title': 'Pet Category', 'description': 'The category of the pet.'})
-
-
-@app.get('/')
-@app.doc(tags=['Hello'])
-def say_hello():
-    """Just Say Hello
-
-    It will always return a greeting like this:
-    ```
-    {'message': 'Hello!'}
-    ```
-    """
-    return {'message': 'Hello!'}
-
-
-@app.get('/pets/<int:pet_id>')
-@app.output(PetOut, description='The pet with given ID')
-@app.doc(tags=['Pet'], operation_id='getPet')
-def get_pet(pet_id):
-    """Get a Pet
-
-    Get a pet with specific ID.
-    """
-    if pet_id > len(pets) - 1 or pets[pet_id].get('deleted'):
-        abort(404)
-    return pets[pet_id]
-
-
-@app.get('/pets')
-@app.output(PetOut(many=True), description='A list of pets')
-@app.doc(tags=['Pet'])
-def get_pets():
-    """Get All Pet
-
-    Get all pets in the database.
-    """
-    return pets
-
-
-@app.post('/pets')
-@app.input(PetIn)
-@app.output(
-    PetOut,
-    201,
-    description='The pet you just created',
-    links={'getPetById': {
-        'operationId': 'getPet',
-        'parameters': {
-            'pet_id': '$response.body#/id'
-        }
-    }}
-)
-@app.doc(tags=['Pet'])
-def create_pet(data):
-    """Create a Pet
-
-    Create a pet with given data. The created pet will be returned.
-    """
-    pet_id = len(pets)
-    data['id'] = pet_id
-    pets.append(data)
-    return pets[pet_id]
-
-
-@app.patch('/pets/<int:pet_id>')
-@app.input(PetIn(partial=True))
-@app.output(PetOut, description='The updated pet')
-@app.doc(tags=['Pet'])
-def update_pet(pet_id, data):
-    """Update a Pet
-
-    Update a pet with given data, the valid fields are `name` and `category`.
-    """
-    if pet_id > len(pets) - 1:
-        abort(404)
-    for attr, value in data.items():
-        pets[pet_id][attr] = value
-    return pets[pet_id]
-
-
-@app.delete('/pets/<int:pet_id>')
-@app.output({}, status_code=204, description='Empty')
-@app.doc(tags=['Pet'])
-def delete_pet(pet_id):
-    """Delete a Pet
-
-    Delete a pet with specific ID. The deleted pet will be renamed to `"Ghost"`.
-    """
-    if pet_id > len(pets) - 1:
-        abort(404)
-    pets[pet_id]['deleted'] = True
-    pets[pet_id]['name'] = 'Ghost'
-    return ''
+from apiflask import APIFlask, Schema, abort
+from apiflask.fields import Integer, String
+from apiflask.validators import Length, OneOf
+
+# set openapi.info.title and openapi.info.version
+app = APIFlask(__name__, title='Pet API', version='1.0')
+
+# All the OpenAPI field config can be set with the corresponding attributes of the app instance:
+# app.description = '...'
+
+# openapi.info.description
+app.config['DESCRIPTION'] = """
+The description for this API. It can be very long and **Markdown** is supported.
+
+In this example, the tags is manually set. However, in a real world application, it will be
+enough to use the automatic tags feature based on blueprint, see the example for blueprint
+tags under the "examples/blueprint_tags" folder:
+
+```
+$ cd ..
+$ cd blueprint_tags
+$ flask run
+```
+
+The source can be found at [examples/blueprint_tags/app.py][_blueprint_tags].
+
+[_blueprint_tags]: https://github.com/apiflask/apiflask/tree/main/examples/blueprint_tags/app.py
+"""
+
+# openapi.info.contact
+app.config['CONTACT'] = {
+    'name': 'API Support',
+    'url': 'https://greyli.com/en',
+    'email': 'withlihui@gmail.com'
+}
+
+# openapi.info.license
+app.config['LICENSE'] = {
+    'name': 'MIT',
+    'url': 'https://opensource.org/licenses/MIT'
+}
+
+# openapi.info.termsOfService
+app.config['TERMS_OF_SERVICE'] = 'http://example.com'
+
+# The four info fields above can be set with the INFO key:
+# app.config['INFO'] = {
+#     'description': '...',
+#     'termsOfService': 'http://example.com',
+#     'contact': {
+#         'name': 'API Support',
+#         'url': 'http://www.example.com/support',
+#         'email': 'support@example.com'
+#     },
+#     'license': {
+#          'name': 'Apache 2.0',
+#          'url': 'http://www.apache.org/licenses/LICENSE-2.0.html'
+#      }
+# }
+
+# openapi.tags
+app.config['TAGS'] = [
+    {'name': 'Hello', 'description': 'The description of the **Hello** tag.'},
+    {'name': 'Pet', 'description': 'The description of the **Pet** tag.'}
+]
+
+# If you don't need to set tag "description" or tag "externalDocs", just pass a list a string:
+# app.config['TAGS'] = ['Hello', 'Pet']
+
+# openapi.servers
+app.config['SERVERS'] = [
+    {
+        'name': 'Development Server',
+        'url': 'http://localhost:5000'
+    },
+    {
+        'name': 'Production Server',
+        'url': 'http://api.example.com'
+    },
+    {
+        'name': 'Testing Server',
+        'url': 'http://test.example.com'
+    }
+]
+
+# openapi.externalDocs
+app.config['EXTERNAL_DOCS'] = {
+    'description': 'Find more info here',
+    'url': 'https://apiflask.com/docs'
+}
+
+pets = [
+    {'id': 0, 'name': 'Kitty', 'category': 'cat'},
+    {'id': 1, 'name': 'Coco', 'category': 'dog'},
+    {'id': 2, 'name': 'Flash', 'category': 'cat'}
+]
+
+
+class PetIn(Schema):
+    name = String(
+        required=True,
+        validate=Length(0, 10),
+        metadata={'title': 'Pet Name', 'description': 'The name of the pet.'}
+    )
+    category = String(
+        required=True,
+        validate=OneOf(['dog', 'cat']),
+        metadata={'title': 'Pet Category', 'description': 'The category of the pet.'}
+    )
+
+
+class PetOut(Schema):
+    id = Integer(metadata={'title': 'Pet ID', 'description': 'The ID of the pet.'})
+    name = String(metadata={'title': 'Pet Name', 'description': 'The name of the pet.'})
+    category = String(metadata={'title': 'Pet Category', 'description': 'The category of the pet.'})
+
+
+@app.get('/')
+@app.doc(tags=['Hello'])
+def say_hello():
+    """Just Say Hello
+
+    It will always return a greeting like this:
+    ```
+    {'message': 'Hello!'}
+    ```
+    """
+    return {'message': 'Hello!'}
+
+
+@app.get('/pets/<int:pet_id>')
+@app.output(PetOut, description='The pet with given ID')
+@app.doc(tags=['Pet'], operation_id='getPet')
+def get_pet(pet_id):
+    """Get a Pet
+
+    Get a pet with specific ID.
+    """
+    if pet_id > len(pets) - 1 or pets[pet_id].get('deleted'):
+        abort(404)
+    return pets[pet_id]
+
+
+@app.get('/pets')
+@app.output(PetOut(many=True), description='A list of pets')
+@app.doc(tags=['Pet'])
+def get_pets():
+    """Get All Pet
+
+    Get all pets in the database.
+    """
+    return pets
+
+
+@app.post('/pets')
+@app.input(PetIn, location='json')
+@app.output(
+    PetOut,
+    status_code=201,
+    description='The pet you just created',
+    links={'getPetById': {
+        'operationId': 'getPet',
+        'parameters': {
+            'pet_id': '$response.body#/id'
+        }
+    }}
+)
+@app.doc(tags=['Pet'])
+def create_pet(json_data):
+    """Create a Pet
+
+    Create a pet with given data. The created pet will be returned.
+    """
+    pet_id = len(pets)
+    json_data['id'] = pet_id
+    pets.append(json_data)
+    return pets[pet_id]
+
+
+@app.patch('/pets/<int:pet_id>')
+@app.input(PetIn(partial=True), location='json')
+@app.output(PetOut, description='The updated pet')
+@app.doc(tags=['Pet'])
+def update_pet(pet_id, json_data):
+    """Update a Pet
+
+    Update a pet with given data, the valid fields are `name` and `category`.
+    """
+    if pet_id > len(pets) - 1:
+        abort(404)
+    for attr, value in json_data.items():
+        pets[pet_id][attr] = value
+    return pets[pet_id]
+
+
+@app.delete('/pets/<int:pet_id>')
+@app.output({}, status_code=204, description='Empty')
+@app.doc(tags=['Pet'])
+def delete_pet(pet_id):
+    """Delete a Pet
+
+    Delete a pet with specific ID. The deleted pet will be renamed to `"Ghost"`.
+    """
+    if pet_id > len(pets) - 1:
+        abort(404)
+    pets[pet_id]['deleted'] = True
+    pets[pet_id]['name'] = 'Ghost'
+    return ''
```

### Comparing `APIFlask-1.3.1/examples/orm/app.py` & `APIFlask-2.0.0/examples/orm/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 class PetModel(db.Model):
     id = db.Column(db.Integer, primary_key=True)
     name = db.Column(db.String(10))
     category = db.Column(db.String(10))
 
 
-@app.before_first_request
 def init_database():
     db.create_all()
 
     pets = [
         {'name': 'Kitty', 'category': 'cat'},
         {'name': 'Coco', 'category': 'dog'},
         {'name': 'Flash', 'category': 'cat'}
@@ -46,44 +45,48 @@
 def say_hello():
     return {'message': 'Hello!'}
 
 
 @app.get('/pets/<int:pet_id>')
 @app.output(PetOut)
 def get_pet(pet_id):
-    return PetModel.query.get_or_404(pet_id)
+    return db.get_or_404(PetModel, pet_id)
 
 
 @app.get('/pets')
 @app.output(PetOut(many=True))
 def get_pets():
     return PetModel.query.all()
 
 
 @app.post('/pets')
-@app.input(PetIn)
+@app.input(PetIn, location='json')
 @app.output(PetOut, status_code=201)
-def create_pet(data):
-    pet = PetModel(**data)
+def create_pet(json_data):
+    pet = PetModel(**json_data)
     db.session.add(pet)
     db.session.commit()
     return pet
 
 
 @app.patch('/pets/<int:pet_id>')
-@app.input(PetIn(partial=True))
+@app.input(PetIn(partial=True), location='json')
 @app.output(PetOut)
-def update_pet(pet_id, data):
-    pet = PetModel.query.get_or_404(pet_id)
-    for attr, value in data.items():
+def update_pet(pet_id, json_data):
+    pet = db.get_or_404(PetModel, pet_id)
+    for attr, value in json_data.items():
         setattr(pet, attr, value)
     db.session.commit()
     return pet
 
 
 @app.delete('/pets/<int:pet_id>')
 @app.output({}, status_code=204)
 def delete_pet(pet_id):
-    pet = PetModel.query.get_or_404(pet_id)
+    pet = db.get_or_404(PetModel, pet_id)
     db.session.delete(pet)
     db.session.commit()
     return ''
+
+
+with app.app_context():
+    init_database()
```

### Comparing `APIFlask-1.3.1/examples/pagination/app.py` & `APIFlask-2.0.0/examples/base_response/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,105 @@
-import random
-
-from flask_sqlalchemy import SQLAlchemy
-from apiflask import APIFlask, Schema, PaginationSchema, pagination_builder
-from apiflask.fields import Integer, String, List, Nested
-from apiflask.validators import Range
+from apiflask import APIFlask, Schema, abort
+from apiflask.fields import Integer, String, Field
+from apiflask.validators import Length, OneOf
 
 app = APIFlask(__name__)
-app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite:///:memory:'
-app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
-
-db = SQLAlchemy(app)
-
-
-class PetModel(db.Model):
-    id = db.Column(db.Integer, primary_key=True)
-    name = db.Column(db.String(10))
-    category = db.Column(db.String(10))
-
-
-@app.before_first_request
-def init_database():
-    db.create_all()
-    for i in range(1, 101):
-        name = f'Pet {i}'
-        category = random.choice(['dog', 'cat'])
-        pet = PetModel(name=name, category=category)
-        db.session.add(pet)
-    db.session.commit()
 
 
-class PetQuery(Schema):
-    page = Integer(load_default=1)
-    per_page = Integer(load_default=20, validate=Range(max=30))
+class BaseResponse(Schema):
+    data = Field()  # the data key
+    message = String()
+    code = Integer()
+
+
+app.config['BASE_RESPONSE_SCHEMA'] = BaseResponse
+# the data key should match the data field name in the base response schema
+# defaults to "data"
+app.config['BASE_RESPONSE_DATA_KEY '] = 'data'
+
+pets = [
+    {'id': 0, 'name': 'Kitty', 'category': 'cat'},
+    {'id': 1, 'name': 'Coco', 'category': 'dog'},
+    {'id': 2, 'name': 'Flash', 'category': 'cat'}
+]
+
+
+class PetIn(Schema):
+    name = String(required=True, validate=Length(0, 10))
+    category = String(required=True, validate=OneOf(['dog', 'cat']))
 
 
 class PetOut(Schema):
     id = Integer()
     name = String()
     category = String()
 
 
-class PetsOut(Schema):
-    pets = List(Nested(PetOut))
-    pagination = Nested(PaginationSchema)
-
-
 @app.get('/')
 def say_hello():
-    return {'message': 'Hello!'}
+    data = {'message': 'Hello!'}
+    return {
+        'data': data,
+        'message': 'Success!',
+        'code': 200
+    }
 
 
 @app.get('/pets/<int:pet_id>')
 @app.output(PetOut)
 def get_pet(pet_id):
-    return PetModel.query.get_or_404(pet_id)
+    if pet_id > len(pets) - 1 or pets[pet_id].get('deleted'):
+        abort(404)
+    return {
+        'data': pets[pet_id],
+        'message': 'Success!',
+        'code': 200,
+    }
 
 
 @app.get('/pets')
-@app.input(PetQuery, location='query')
-@app.output(PetsOut)
-def get_pets(query):
-    pagination = PetModel.query.paginate(
-        page=query['page'],
-        per_page=query['per_page']
-    )
-    pets = pagination.items
+@app.output(PetOut(many=True))
+def get_pets():
     return {
-        'pets': pets,
-        'pagination': pagination_builder(pagination)
+        'data': pets,
+        'message': 'Success!',
+        'code': 200,
     }
+
+
+@app.post('/pets')
+@app.input(PetIn, location='json')
+@app.output(PetOut, status_code=201)
+def create_pet(json_data):
+    pet_id = len(pets)
+    json_data['id'] = pet_id
+    pets.append(json_data)
+    return {
+        'data': pets[pet_id],
+        'message': 'Pet created.',
+        'code': 201
+    }
+
+
+@app.patch('/pets/<int:pet_id>')
+@app.input(PetIn(partial=True), location='json')
+@app.output(PetOut)
+def update_pet(pet_id, json_data):
+    if pet_id > len(pets) - 1:
+        abort(404)
+    for attr, value in json_data.items():
+        pets[pet_id][attr] = value
+    return {
+        'data': pets[pet_id],
+        'message': 'Pet updated.',
+        'code': 200
+    }
+
+
+@app.delete('/pets/<int:pet_id>')
+@app.output({}, status_code=204)
+def delete_pet(pet_id):
+    if pet_id > len(pets) - 1:
+        abort(404)
+    pets[pet_id]['deleted'] = True
+    pets[pet_id]['name'] = 'Ghost'
+    return ''
```

### Comparing `APIFlask-1.3.1/examples/test_examples.py` & `APIFlask-2.0.0/examples/test_examples.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/requirements/dev.txt` & `APIFlask-2.0.0/requirements/dev.txt`

 * *Files 24% similar despite different names*

```diff
@@ -7,49 +7,49 @@
 #
 -r docs.txt
 -r examples.txt
 -r tests.txt
 -r typing.txt
 build==0.10.0
     # via pip-tools
-cachetools==5.3.0
+cachetools==5.3.1
     # via tox
 cfgv==3.3.1
     # via pre-commit
 chardet==5.1.0
     # via tox
 distlib==0.3.6
     # via virtualenv
-filelock==3.10.0
+filelock==3.12.2
     # via
     #   tox
     #   virtualenv
-identify==2.5.21
+identify==2.5.24
     # via pre-commit
-nodeenv==1.7.0
+nodeenv==1.8.0
     # via pre-commit
-pip-compile-multi==2.6.2
+pip-compile-multi==2.6.3
     # via -r requirements/dev.in
-pip-tools==6.12.3
+pip-tools==7.0.0
     # via pip-compile-multi
-platformdirs==3.1.1
+platformdirs==3.8.1
     # via
     #   tox
     #   virtualenv
-pre-commit==3.2.0
+pre-commit==3.3.3
     # via -r requirements/dev.in
-pyproject-api==1.5.1
+pyproject-api==1.5.3
     # via tox
 pyproject-hooks==1.0.0
     # via build
 toposort==1.10
     # via pip-compile-multi
-tox==4.4.7
+tox==4.6.4
     # via -r requirements/dev.in
-virtualenv==20.21.0
+virtualenv==20.24.0
     # via
     #   pre-commit
     #   tox
 wheel==0.40.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `APIFlask-1.3.1/requirements/docs.txt` & `APIFlask-2.0.0/requirements/docs.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,83 +1,85 @@
-# SHA1:ef596ae778adb45f338de10aecbc5fdcea757811
+# SHA1:56a1feae5bc5e5f7fdcfa63e6f6628efdacd917c
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.2.0
     # via requests
-click==8.1.3
+click==8.1.5
     # via mkdocs
 colorama==0.4.6
-    # via mkdocs-material
+    # via
+    #   griffe
+    #   mkdocs-material
 ghp-import==2.1.0
     # via mkdocs
+griffe==0.32.1
+    # via mkdocstrings-python
 idna==3.4
     # via requests
 jinja2==3.1.2
     # via
     #   mkdocs
     #   mkdocs-material
     #   mkdocstrings
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
     #   pymdown-extensions
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   mkdocstrings
 mergedeep==1.3.4
     # via mkdocs
-mkdocs==1.4.2
+mkdocs==1.4.3
     # via
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
 mkdocs-autorefs==0.4.1
     # via mkdocstrings
-mkdocs-material==9.1.3
+mkdocs-material==9.1.18
     # via -r requirements/docs.in
 mkdocs-material-extensions==1.1.1
     # via mkdocs-material
-mkdocstrings[python-legacy]==0.20.0
+mkdocstrings==0.22.0
     # via
     #   -r requirements/docs.in
-    #   mkdocstrings-python-legacy
-mkdocstrings-python-legacy==0.2.3
-    # via mkdocstrings
-packaging==23.0
+    #   mkdocstrings-python
+mkdocstrings-python==1.2.0
+    # via -r requirements/docs.in
+packaging==23.1
     # via mkdocs
-pygments==2.14.0
+pygments==2.15.1
     # via mkdocs-material
-pymdown-extensions==9.10
+pymdown-extensions==10.1
     # via
     #   mkdocs-material
     #   mkdocstrings
 python-dateutil==2.8.2
     # via ghp-import
-pytkdocs==0.16.1
-    # via mkdocstrings-python-legacy
 pyyaml==6.0
     # via
     #   mkdocs
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
-regex==2022.10.31
+regex==2023.6.3
     # via mkdocs-material
-requests==2.28.2
+requests==2.31.0
     # via mkdocs-material
 six==1.16.0
     # via python-dateutil
-urllib3==1.26.15
+urllib3==2.0.3
     # via requests
-watchdog==2.3.1
+watchdog==3.0.0
     # via mkdocs
```

### Comparing `APIFlask-1.3.1/requirements/examples.txt` & `APIFlask-2.0.0/requirements/examples.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 # SHA1:381712aa8983e6e5324445a24e0fb8cf1ab21d6d
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-authlib==1.2.0
+authlib==1.2.1
     # via -r requirements/examples.in
+blinker==1.6.2
+    # via flask
 cffi==1.15.1
     # via cryptography
-click==8.1.3
+click==8.1.5
     # via flask
-cryptography==39.0.2
+cryptography==41.0.2
     # via authlib
-flask==2.2.3
+flask==2.3.2
     # via flask-sqlalchemy
-flask-sqlalchemy==3.0.3
+flask-sqlalchemy==3.0.5
     # via -r requirements/examples.in
 greenlet==2.0.2
     # via sqlalchemy
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
-markupsafe==2.1.2
+markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
 marshmallow==3.19.0
     # via marshmallow-dataclass
-marshmallow-dataclass==8.5.12
+marshmallow-dataclass==8.5.14
     # via -r requirements/examples.in
 mypy-extensions==1.0.0
     # via typing-inspect
-packaging==23.0
+packaging==23.1
     # via marshmallow
 pycparser==2.21
     # via cffi
-sqlalchemy==2.0.6
+sqlalchemy==2.0.19
     # via flask-sqlalchemy
-typing-extensions==4.5.0
+typing-extensions==4.7.1
     # via
     #   marshmallow-dataclass
     #   sqlalchemy
     #   typing-inspect
-typing-inspect==0.8.0
+typing-inspect==0.9.0
     # via marshmallow-dataclass
-werkzeug==2.2.3
+werkzeug==2.3.6
     # via flask
```

### Comparing `APIFlask-1.3.1/setup.cfg` & `APIFlask-2.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -10,36 +10,38 @@
 platforms = any
 url = https://apiflask.com
 project_urls = 
 	Documentation = https://apiflask.com/docs
 	Source = https://github.com/apiflask/apiflask
 	Changelog = https://apiflask.com/changelog
 	Issue Tracker = https://github.com/apiflask/apiflask/issues
+	Donate = https://opencollective.com/apiflask
 keywords = flask, marshmallow, openapi
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Web Environment
 	Framework :: Flask
 	Intended Audience :: Developers
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 	Topic :: Internet :: WWW/HTTP :: WSGI
 	Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 	Topic :: Software Development :: Libraries :: Application Frameworks
 
 [options]
 packages = find:
 package_dir = = src
 include_package_data = true
-python_requires = >= 3.7
+python_requires = >= 3.8
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	apiflask = flask.cli:main
@@ -55,14 +57,15 @@
 ignore = 
 	W503
 max-line-length = 100
 per-file-ignores = 
 	src/apiflask/__init__.py: F401
 	src/apiflask/fields.py: F401
 	src/apiflask/validators.py: F401
+	src/apiflask/views.py: F401
 	src/apiflask/ui_templates.py: E501, B950
 exclude = 
 	.*
 	*.txt
 	*.md
 	__pycache__
```

### Comparing `APIFlask-1.3.1/src/APIFlask.egg-info/PKG-INFO` & `APIFlask-2.0.0/src/APIFlask.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: APIFlask
-Version: 1.3.1
+Version: 2.0.0
 Summary: A lightweight web API framework based on Flask and marshmallow-code projects.
 Home-page: https://apiflask.com
 Author: Grey Li
 Author-email: withlihui@gmail.com
 License: MIT
 Project-URL: Documentation, https://apiflask.com/docs
 Project-URL: Source, https://github.com/apiflask/apiflask
 Project-URL: Changelog, https://apiflask.com/changelog
 Project-URL: Issue Tracker, https://github.com/apiflask/apiflask/issues
+Project-URL: Donate, https://opencollective.com/apiflask
 Keywords: flask,marshmallow,openapi
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: async
 Provides-Extra: dotenv
 Provides-Extra: yaml
 License-File: LICENSE
 License-File: NOTICE
 
@@ -52,16 +54,16 @@
 - Automatic interactive API documentation
 - API authentication support (with [Flask-HTTPAuth](https://github.com/miguelgrinberg/flask-httpauth))
 - Automatic JSON response for HTTP errors
 
 
 ## Requirements
 
-- Python 3.7+
-- Flask 1.1.0+
+- Python 3.8+
+- Flask 2.0+
 
 
 ## Installation
 
 For Linux and macOS:
 
 ```bash
@@ -81,14 +83,20 @@
 - Documentation: <https://apiflask.com/docs>
 - PyPI Releases: <https://pypi.python.org/pypi/APIFlask>
 - Change Log: <https://apiflask.com/changelog>
 - Source Code: <https://github.com/apiflask/apiflask>
 - Issue Tracker: <https://github.com/apiflask/apiflask/issues>
 - Discussion: <https://github.com/apiflask/apiflask/discussions>
 - Twitter: <https://twitter.com/apiflask>
+- Open Collective: <https://opencollective.com/apiflask>
+
+
+## Donate
+
+If you find APIFlask useful, please consider [donating](https://opencollective.com/apiflask) today. Your donation keeps APIFlask maintained and evolving.
 
 
 ## Example
 
 ```python
 from apiflask import APIFlask, Schema, abort
 from apiflask.fields import Integer, String
@@ -128,32 +136,32 @@
     # APIFlask will serialize the object into JSON format
     return pets[pet_id]
 
 
 @app.patch('/pets/<int:pet_id>')
 @app.input(PetIn(partial=True))
 @app.output(PetOut)
-def update_pet(pet_id, data):
+def update_pet(pet_id, json_data):
     # the validated and parsed input data will
     # be injected into the view function as a dict
     if pet_id > len(pets) - 1:
         abort(404)
-    for attr, value in data.items():
+    for attr, value in json_data.items():
         pets[pet_id][attr] = value
     return pets[pet_id]
 ```
 
 <details>
 <summary>You can also use class-based views based on <code>MethodView</code></summary>
 
 ```python
 from apiflask import APIFlask, Schema, abort
 from apiflask.fields import Integer, String
 from apiflask.validators import Length, OneOf
-from apiflask.views import MethodView
+from flask.views import MethodView
 
 app = APIFlask(__name__)
 
 pets = [
     {'id': 0, 'name': 'Kitty', 'category': 'cat'},
     {'id': 1, 'name': 'Coco', 'category': 'dog'}
 ]
@@ -184,30 +192,30 @@
         """Get a pet"""
         if pet_id > len(pets) - 1:
             abort(404)
         return pets[pet_id]
 
     @app.input(PetIn(partial=True))
     @app.output(PetOut)
-    def patch(self, pet_id, data):
+    def patch(self, pet_id, json_data):
         """Update a pet"""
         if pet_id > len(pets) - 1:
             abort(404)
-        for attr, value in data.items():
+        for attr, value in json_data.items():
             pets[pet_id][attr] = value
         return pets[pet_id]
 
 
 app.add_url_rule('/', view_func=Hello.as_view('hello'))
 app.add_url_rule('/pets/<int:pet_id>', view_func=Pet.as_view('pet'))
 ```
 </details>
 
 <details>
-<summary>Or use <code>async def</code> with Flask 2.0</summary>
+<summary>Or use <code>async def</code></summary>
 
 ```bash
 $ pip install -U "apiflask[async]"
 ```
 
 ```python
 import asyncio
@@ -270,35 +278,36 @@
 
 ## Relationship with Flask
 
 APIFlask is a thin wrapper on top of Flask. You only need to remember the following differences (see *[Migrating from Flask](https://apiflask.com/migrating)* for more details):
 
 - When creating an application instance, use `APIFlask` instead of `Flask`.
 - When creating a blueprint instance, use `APIBlueprint` instead of `Blueprint`.
-- When creating a class-based view, use `apiflask.views.MethodView` instead of `flask.views.MethodView`.
 - The `abort()` function from APIFlask (`apiflask.abort`) returns JSON error response.
 
 For a minimal Flask application:
 
 ```python
-from flask import Flask, request, escape
+from flask import Flask, request
+from markupsafe import escape
 
 app = Flask(__name__)
 
 @app.route('/')
 def hello():
     name = request.args.get('name', 'Human')
     return f'Hello, {escape(name)}'
 ```
 
 Now change to APIFlask:
 
 ```python
 from apiflask import APIFlask  # step one
-from flask import request, escape
+from flask import request
+from markupsafe import escape
 
 app = APIFlask(__name__)  # step two
 
 @app.route('/')
 def hello():
     name = request.args.get('name', 'Human')
     return f'Hello, {escape(name)}'
```

### Comparing `APIFlask-1.3.1/src/APIFlask.egg-info/SOURCES.txt` & `APIFlask-2.0.0/src/APIFlask.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 examples/auth/basic_auth/app.py
 examples/auth/token_auth/app.py
 examples/base_response/app.py
 examples/basic/app.py
 examples/blueprint_tags/app.py
 examples/cbv/app.py
 examples/dataclass/app.py
+examples/openapi/.coverage
 examples/openapi/app.py
 examples/orm/app.py
 examples/pagination/app.py
 requirements/dev.txt
 requirements/docs.txt
 requirements/examples.txt
 requirements/tests.txt
@@ -67,14 +68,15 @@
 tests/test_openapi_basic.py
 tests/test_openapi_blueprint.py
 tests/test_openapi_info.py
 tests/test_openapi_paths.py
 tests/test_openapi_security.py
 tests/test_openapi_tags.py
 tests/test_route.py
+tests/test_schemas.py
 tests/test_security.py
 tests/test_settings_api_docs.py
 tests/test_settings_auto_behaviour.py
 tests/test_settings_openapi_fields.py
 tests/test_settings_openapi_spec.py
 tests/test_settings_response_customization.py
 tests/test_apps/__init__.py
```

### Comparing `APIFlask-1.3.1/src/apiflask/__init__.py` & `APIFlask-2.0.0/src/apiflask/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,13 +2,15 @@
 from . import validators as validators
 from .app import APIFlask as APIFlask
 from .blueprint import APIBlueprint as APIBlueprint
 from .exceptions import abort as abort
 from .exceptions import HTTPError as HTTPError
 from .helpers import get_reason_phrase as get_reason_phrase
 from .helpers import pagination_builder as pagination_builder
+from .schemas import EmptySchema as EmptySchema
+from .schemas import FileSchema as FileSchema
 from .schemas import PaginationSchema as PaginationSchema
 from .schemas import Schema as Schema
 from .security import HTTPBasicAuth as HTTPBasicAuth
 from .security import HTTPTokenAuth as HTTPTokenAuth
 
-__version__ = '1.3.1'
+__version__ = '2.0.0'
```

### Comparing `APIFlask-1.3.1/src/apiflask/app.py` & `APIFlask-2.0.0/src/apiflask/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,23 @@
 import inspect
 import json
 import re
-import sys
 import typing as t
 import warnings
 
-# temp fix for https://github.com/django/asgiref/issues/143
-if sys.platform == 'win32' and (3, 8, 0) <= sys.version_info < (3, 9, 0):  # pragma: no cover
-    import asyncio
-    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())  # pragma: no cover
-
 from apispec import APISpec
 from apispec import BasePlugin
 from apispec.ext.marshmallow import MarshmallowPlugin
 from flask import Blueprint
 from flask import Flask
 from flask import has_request_context
 from flask import jsonify
 from flask import render_template_string
 from flask import request
 from flask.config import ConfigAttribute
-try:
-    from flask.globals import request_ctx  # type: ignore
-except ImportError:  # pragma: no cover
-    from flask.globals import _request_ctx_stack
-    request_ctx = None  # type: ignore
-from flask.wrappers import Response
 
 with warnings.catch_warnings():
     warnings.simplefilter('ignore')
     from flask_marshmallow import fields
     try:
         from flask_marshmallow import sqla
     except ImportError:
@@ -56,15 +44,14 @@
 from .openapi import default_response
 from .openapi import get_tag
 from .openapi import get_operation_tags
 from .openapi import get_path_summary
 from .openapi import get_auth_name
 from .openapi import get_argument
 from .openapi import get_security_and_security_schemes
-from .ui_templates import redoc_template
 from .ui_templates import ui_templates
 from .ui_templates import swagger_ui_oauth2_redirect_template
 from .scaffold import APIScaffold
 
 
 @route_patch
 class APIFlask(APIScaffold, Flask):
@@ -274,15 +261,14 @@
         import_name: str,
         title: str = 'APIFlask',
         version: str = '0.1.0',
         spec_path: t.Optional[str] = '/openapi.json',
         docs_path: t.Optional[str] = '/docs',
         docs_oauth2_redirect_path: t.Optional[str] = '/docs/oauth2-redirect',
         docs_ui: str = 'swagger-ui',
-        redoc_path: t.Optional[str] = '/redoc',
         openapi_blueprint_url_prefix: t.Optional[str] = None,
         json_errors: bool = True,
         enable_openapi: bool = True,
         spec_plugins: t.Optional[t.List[BasePlugin]] = None,
         static_url_path: t.Optional[str] = None,
         static_folder: str = 'static',
         static_host: t.Optional[str] = None,
@@ -305,27 +291,29 @@
             spec_path: The path to OpenAPI Spec documentation. It
                 defaults to `/openapi.json`, if the path ends with `.yaml`
                 or `.yml`, the YAML format of the OAS will be returned.
             docs_path: The path to API UI documentation, defaults to `/docs`.
             docs_ui: The UI of API documentation, one of `swagger-ui` (default), `redoc`,
                 `elements`, `rapidoc`, and `rapipdf`.
             docs_oauth2_redirect_path: The path to Swagger UI OAuth redirect.
-            redoc_path: Deprecated since 1.1, set `APIFlask(docs_ui='redoc')` to use Redoc.
-                The path to Redoc documentation, defaults to `/redoc`.
             openapi_blueprint_url_prefix: The url prefix of the OpenAPI blueprint. This
                 prefix will append before all the OpenAPI-related paths (`sepc_path`,
                 `docs_path`, etc.), defaults to `None`.
             json_errors: If `True`, APIFlask will return a JSON response for HTTP errors.
             enable_openapi: If `False`, will disable OpenAPI spec and API docs views.
             spec_plugins: List of apispec-compatible plugins (subclasses of `apispec.BasePlugin`),
                 defaults to `None`. The `MarshmallowPlugin` for apispec is already included
                 by default, so it doesn't need to be provided here.
 
         Other keyword arguments are directly passed to `flask.Flask`.
 
+        *Version changed: 2.0.0*
+
+        - Remove the deprecated `redoc_path` parameter.
+
         *Version changed: 1.2.0*
 
         - Add `spec_plugins` parameter.
 
         *Version changed: 1.1.0*
 
         - Add `docs_ui` parameter.
@@ -351,15 +339,14 @@
         self.config.from_object('apiflask.settings')
 
         self.title = title
         self.version = version
         self.spec_path = spec_path
         self.docs_ui = docs_ui
         self.docs_path = docs_path
-        self.redoc_path = redoc_path
         self.docs_oauth2_redirect_path = docs_oauth2_redirect_path
         self.openapi_blueprint_url_prefix = openapi_blueprint_url_prefix
         self.enable_openapi = enable_openapi
         self.json_errors = json_errors
 
         self.spec_callback: t.Optional[SpecCallbackType] = None
         self.error_callback: ErrorCallbackType = self._error_handler
@@ -399,70 +386,14 @@
             error = HTTPError(
                 e.code,
                 message=e.name,
                 headers=headers
             )
             return self.error_callback(error)
 
-    def dispatch_request(self) -> ResponseReturnValueType:  # type: ignore
-        """Overwrite the default dispatch method in Flask.
-
-        With this overwrite, view arguments are passed as positional
-        arguments so that the view function can intuitively accept the
-        parameters (i.e., from top to bottom, from left to right).
-
-        Examples:
-
-        ```python
-        @app.get('/pets/<name>/<int:pet_id>/<age>')  # -> name, pet_id, age
-        @app.input(Query)  # -> query
-        @app.output(Pet)  # -> pet
-        def get_pet(name, pet_id, age, query, pet):
-            pass
-        ```
-
-        From Flask, see the NOTICE file for license information.
-
-        *Version added: 0.2.0*
-        """
-        req = request_ctx.request if request_ctx else _request_ctx_stack.top.request  # type: ignore
-        if req.routing_exception is not None:
-            self.raise_routing_exception(req)
-        rule = req.url_rule
-        # if we provide automatic options for this URL and the
-        # request came with the OPTIONS method, reply automatically
-        if (  # pragma: no cover
-            getattr(rule, 'provide_automatic_options', False)
-            and req.method == 'OPTIONS'
-        ):
-            return self.make_default_options_response()  # pragma: no cover
-        # otherwise dispatch to the handler for that endpoint
-        view_function = self.view_functions[rule.endpoint]
-        if hasattr(self, 'ensure_sync'):  # pragma: no cover
-            view_function = self.ensure_sync(view_function)
-        if rule.endpoint == 'static' or hasattr(view_function, '_only_kwargs'):
-            # app static route only accepts keyword arguments, see flask#3762
-            # view classes created by Flask only accept keyword arguments
-            return view_function(**req.view_args)  # type: ignore
-        else:
-            return view_function(*req.view_args.values())  # type: ignore
-
-    # TODO: remove this function when we dropped the Flask 1.x support
-    # the list return values are supported in Flask 2.2
-    def make_response(self, rv) -> Response:
-        """Patch the make_response form Flask to allow returning list as JSON.
-
-        *Version added: 1.1.0*
-        """
-        if isinstance(rv, list):
-            rv = jsonify(rv)
-        elif isinstance(rv, tuple) and isinstance(rv[0], list):
-            rv = (jsonify(rv[0]), *rv[1:])
-        return super().make_response(rv)
-
     @staticmethod
     def _error_handler(
         error: HTTPError
     ) -> ResponseReturnValueType:
         """The default error handler.
 
         Arguments:
@@ -564,18 +495,15 @@
         - Apply this error processor to normal HTTP errors even when
           `json_error` is set to `False` when creating `APIFlask` instance.
 
         *Version changed: 0.7.0*
 
         - Support registering an async callback function.
         """
-        if hasattr(self, 'ensure_sync'):  # pragma: no cover
-            self.error_callback = self.ensure_sync(f)
-        else:  # pragma: no cover
-            self.error_callback = f
+        self.error_callback = self.ensure_sync(f)
         self._apply_error_callback_to_werkzeug_errors()
         return f
 
     def _register_openapi_blueprint(self) -> None:
         """Register a blueprint for OpenAPI support.
 
         The name of the blueprint is "openapi". This blueprint will hold the view
@@ -624,32 +552,16 @@
 
             if self.docs_ui == 'swagger-ui':
                 if self.docs_oauth2_redirect_path:
                     @bp.route(self.docs_oauth2_redirect_path)
                     def swagger_ui_oauth_redirect() -> str:
                         return render_template_string(swagger_ui_oauth2_redirect_template)
 
-        if self.redoc_path:
-            @bp.route(self.redoc_path)
-            def redoc():
-                warnings.warn(
-                    'The `/redoc` path and `redoc_path` parameter is deprecated '
-                    'and will be removed in 2.0, Set `APIFlask(docs_ui="redoc")` '
-                    'to use Redoc and then visit "/docs" instead.',
-                    UserWarning,
-                    stacklevel=2,
-                )
-                return render_template_string(
-                    redoc_template,
-                    title=self.title,
-                    version=self.version
-                )
-
         if self.enable_openapi and (
-            self.spec_path or self.docs_path or self.redoc_path
+            self.spec_path or self.docs_path
         ):
             self.register_blueprint(bp)
 
     def _get_spec(
         self,
         spec_format: t.Optional[str] = None,
         force_update: bool = False
@@ -744,18 +656,15 @@
         - `'json'` -> dict
         - `'yaml'` -> string
 
         *Version Changed: 0.7.0*
 
         - Support registering an async callback function.
         """
-        if hasattr(self, 'ensure_sync'):  # pragma: no cover
-            self.spec_callback = self.ensure_sync(f)
-        else:  # pragma: no cover
-            self.spec_callback = f
+        self.spec_callback = self.ensure_sync(f)
         return f
 
     @property
     def spec(self) -> t.Union[dict, str]:
         """Get the current OAS document file.
 
         This property will call `app._get_spec()` method and set the
@@ -766,15 +675,21 @@
         - Generate the spec on every call.
         """
         return self._get_spec(force_update=True)
 
     @staticmethod
     def _schema_name_resolver(schema: t.Type[Schema]) -> str:
         """Default schema name resovler."""
+        # some schema are passed through the `doc(responses=...)`
+        # we need to make sure the schema is an instance of `Schema`
+        if isinstance(schema, type):  # pragma: no cover
+            schema = schema()  # type: ignore
+
         name = schema.__class__.__name__
+
         if name.endswith('Schema'):
             name = name[:-6] or name
         if schema.partial:
             name += 'Update'
         return name
 
     def _make_info(self) -> dict:
@@ -1144,35 +1059,43 @@
                     add_response_with_schema(
                         spec, operation, '404', schema, 'HTTPError', description
                     )
 
                 if view_func._spec.get('responses'):
                     responses: t.Union[t.List[int], t.Dict[int, str]] \
                         = view_func._spec.get('responses')
+                    # turn status_code list to dict {status_code: reason_phrase}
                     if isinstance(responses, list):
                         responses: t.Dict[int, str] = {}  # type: ignore
                         for status_code in view_func._spec.get('responses'):
                             responses[  # type: ignore
                                 status_code
                             ] = get_reason_phrase(int(status_code), '')
-                    for status_code, description in responses.items():  # type: ignore
+                    for status_code, value in responses.items():  # type: ignore
                         status_code: str = str(status_code)  # type: ignore
+                        # custom complete response spec
+                        if isinstance(value, dict):
+                            operation['responses'][status_code] = value
+                            continue
+                        else:
+                            description = value
+                        # overwrite existing response description
                         if status_code in operation['responses']:
                             if not isinstance(
                                 view_func._spec.get('responses'), list
                             ):  # pragma: no cover
                                 operation['responses'][status_code]['description'] = description
                             continue
+                        # add error response schema for error responses
                         if status_code.startswith('4') or status_code.startswith('5'):
-                            # add error response schema for error responses
                             schema: SchemaType = self.config['HTTP_ERROR_SCHEMA']  # type: ignore
                             add_response_with_schema(
                                 spec, operation, status_code, schema, 'HTTPError', description
                             )
-                        else:
+                        else:  # add default response for other responses
                             add_response(operation, status_code, {}, description)
 
                 # requestBody
                 if view_func._spec.get('body'):
                     content_type = view_func._spec.get('content_type', 'application/json')
                     operation['requestBody'] = {
                         'content': {
@@ -1247,11 +1170,10 @@
 
         for path, operations in paths.items():
             # sort by method before adding them to the spec
             sorted_operations: t.Dict[str, t.Any] = {}
             for method in ['get', 'post', 'put', 'patch', 'delete']:
                 if method in operations:
                     sorted_operations[method] = operations[method]
-            # TODO: remove the type ignore comment when apispec 5.3.0 released
-            spec.path(path=path, operations=sorted_operations)  # type: ignore
+            spec.path(path=path, operations=sorted_operations)
 
         return spec
```

### Comparing `APIFlask-1.3.1/src/apiflask/blueprint.py` & `APIFlask-2.0.0/src/apiflask/blueprint.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/src/apiflask/commands.py` & `APIFlask-2.0.0/src/apiflask/commands.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/src/apiflask/exceptions.py` & `APIFlask-2.0.0/src/apiflask/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class HTTPError(Exception):
     """The exception to end the request handling and return an JSON error response.
 
     Examples:
 
     ```python
     from apiflask import APIFlask, HTTPError
-    from flask import escape
+    from markupsafe import escape
 
     app = APIFlask(__name__)
 
     @app.get('/<name>')
     def hello(name):
         if name == 'Foo':
             raise HTTPError(404, 'This man is missing.')
@@ -106,15 +106,15 @@
 
     Similar to Flask's `abort`, but returns a JSON response.
 
     Examples:
 
     ```python
     from apiflask import APIFlask, abort
-    from flask import escape
+    from markupsafe import escape
 
     app = APIFlask(__name__)
 
     @app.get('/<name>')
     def hello(name):
         if name == 'Foo':
             abort(404, 'This man is missing.')
```

### Comparing `APIFlask-1.3.1/src/apiflask/fields.py` & `APIFlask-2.0.0/src/apiflask/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 
     class Image(Schema):
         image = File()
 
 
     @app.post('/images')
     @app.input(Image, location='files')
-    def upload_image(data):
-        f = data['image']
+    def upload_image(files):
+        f = files['image']
         # use `secure_filename` to clean the filename, notice it will only keep ascii characters
         filename = secure_filename(f.filename)
         f.save(os.path.join(the_path_to_uploads, filename))
 
         return {'message': f'file {filename} saved.'}
     ```
     The file object is an instance of `werkzeug.datastructures.FileStorage`, see more details in the
@@ -81,17 +81,17 @@
 
     class ProfileIn(Schema):
         name = String()
         avatar = File()
 
     @app.post('/profiles')
     @app.input(ProfileIn, location='form_and_files')
-    def create_profile(data):
-        avatar_file = data['avatar']
-        name = data['name']
+    def create_profile(form_and_files_data):
+        avatar_file = form_and_files_data['avatar']
+        name = form_and_files_data['name']
 
         # use `secure_filename` to clean the filename, notice it will only keep ascii characters
         avatar_filename = secure_filename(avatar_file.filename)
         avatar_file.save(os.path.join(the_path_to_uploads, avatar_filename))
 
         profile = Profile(name=name, avatar_filename=avatar_filename)
         # ...
```

### Comparing `APIFlask-1.3.1/src/apiflask/helpers.py` & `APIFlask-2.0.0/src/apiflask/helpers.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/src/apiflask/openapi.py` & `APIFlask-2.0.0/src/apiflask/openapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import typing as t
 
 from apispec import APISpec
 
 from .exceptions import _bad_schema_message
+from .schemas import EmptySchema
+from .schemas import FileSchema
 from .security import HTTPBasicAuth
 from .security import HTTPTokenAuth
 from .types import HTTPAuthType
 from .types import OpenAPISchemaType
 from .types import SchemaType
 
 if t.TYPE_CHECKING:  # pragma: no cover
@@ -174,14 +176,18 @@
 
     *Version changed: 0.10.0*
 
     - Add `links` parameter.
     """
     operation['responses'][status_code] = {}
     if status_code != '204':
+        if isinstance(schema, FileSchema):
+            schema = {'type': schema.type, 'format': schema.format}
+        elif isinstance(schema, EmptySchema):
+            schema = {}
         operation['responses'][status_code]['content'] = {
             content_type: {
                 'schema': schema
             }
         }
     operation['responses'][status_code]['description'] = description
     if example is not None:
```

### Comparing `APIFlask-1.3.1/src/apiflask/route.py` & `APIFlask-2.0.0/src/apiflask/route.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 import typing as t
 
-from flask.views import MethodView as FlaskMethodView
-from flask.views import View as FlaskView
-
 from .openapi import get_path_description
 from .openapi import get_path_summary
 from .types import ViewClassType
 from .types import ViewFuncOrClassType
 from .types import ViewFuncType
 from .views import MethodView
 
@@ -90,24 +87,14 @@
                 # skip View-based class
                 view_func._spec = {'hide': True}  # type: ignore
             else:
                 # record spec for MethodView class
                 if hasattr(self, 'enable_openapi') and self.enable_openapi:
                     view_func = record_spec_for_view_class(view_func, view_class)  # type: ignore
 
-            # view func created by Flask's View only accpets keyword arguments
-            if issubclass(view_class, FlaskView):
-                view_func._only_kwargs = True  # type: ignore
-
-            if issubclass(view_class, FlaskMethodView):
-                raise RuntimeError(
-                    'APIFlask only supports generating OpenAPI spec for view classes created '
-                    'with apiflask.views.MethodView (`from apiflask.views import MethodView`).',
-                )
-
         super(cls, self).add_url_rule(
             rule,
             endpoint,
             view_func,
             provide_automatic_options=provide_automatic_options,
             **options
         )
```

### Comparing `APIFlask-1.3.1/src/apiflask/scaffold.py` & `APIFlask-2.0.0/src/apiflask/scaffold.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import typing as t
-import warnings
 from collections.abc import Mapping as ABCMapping
 from functools import wraps
 
-import flask
 from flask import current_app
 from flask import jsonify
 from flask import Response
 from marshmallow import ValidationError as MarshmallowValidationError
 from webargs.flaskparser import FlaskParser as BaseFlaskParser
 from webargs.multidictproxy import MultiDictProxy
 
@@ -29,14 +27,15 @@
 
 class FlaskParser(BaseFlaskParser):
     """Overwrite the default `webargs.FlaskParser.handle_error`.
 
     Update the default status code and the error description from related
     configuration variables.
     """
+    USE_ARGS_POSITIONAL = False
 
     def handle_error(  # type: ignore
         self,
         error: MarshmallowValidationError,
         req: RequestType,
         schema: Schema,
         *,
@@ -75,15 +74,15 @@
     if not hasattr(f, '_spec'):
         f._spec = {}
     for key, value in kwargs.items():
         f._spec[key] = value
 
 
 def _ensure_sync(f):
-    if flask.__version__ < '2.' or hasattr(f, '_sync_ensured'):
+    if hasattr(f, '_sync_ensured'):
         return f
 
     @wraps(f)
     def wrapper(*args, **kwargs):
         return current_app.ensure_sync(f)(*args, **kwargs)
 
     wrapper._sync_ensured = True
@@ -140,15 +139,14 @@
     def delete(self, rule: str, **options: t.Any):
         """Shortcut for `app.route(methods=['DELETE'])`."""
         return self._method_route('DELETE', rule, options)
 
     def auth_required(
         self,
         auth: HTTPAuthType,
-        role: t.Optional[str] = None,
         roles: t.Optional[list] = None,
         optional: t.Optional[str] = None
     ) -> t.Callable[[DecoratedType], DecoratedType]:
         """Protect a view with provided authentication settings.
 
         > Be sure to put it under the routes decorators (i.e., `app.route`, `app.get`,
         `app.post`, etc.).
@@ -167,89 +165,84 @@
             return 'Hello'!
         ```
 
         Arguments:
             auth: The `auth` object, an instance of
                 [`HTTPBasicAuth`][apiflask.security.HTTPBasicAuth]
                 or [`HTTPTokenAuth`][apiflask.security.HTTPTokenAuth].
-            role: Deprecated since 1.0, use `roles` instead.
             roles: The selected roles to allow to visit this view, accepts a list of role names.
                 See [Flask-HTTPAuth's documentation][_role]{target:_blank} for more details.
                 [_role]: https://flask-httpauth.readthedocs.io/en/latest/#user-roles
             optional: Set to `True` to allow the view to execute even the authentication
                 information is not included with the request, in which case the attribute
                 `auth.current_user` will be `None`.
 
+        *Version changed: 2.0.0*
+
+        - Remove the deprecated `role` parameter.
+
         *Version changed: 1.0.0*
 
         - The `role` parameter is deprecated.
 
         *Version changed: 0.12.0*
 
         - Move to `APIFlask` and `APIBlueprint` classes.
 
         *Version changed: 0.4.0*
 
         - Add parameter `roles`.
         """
-        _roles = None
-        if role is not None:
-            warnings.warn(
-                'The `role` parameter is deprecated and will be removed in 1.1, '
-                'use `roles` and always pass a list instead.',
-                DeprecationWarning,
-                stacklevel=3,
-            )
-            _roles = [role]
-        elif roles is not None:
-            _roles = roles
-
         def decorator(f):
             f = _ensure_sync(f)
-            _annotate(f, auth=auth, roles=_roles or [])
-            return auth.login_required(role=_roles, optional=optional)(f)
+            _annotate(f, auth=auth, roles=roles or [])
+            return auth.login_required(role=roles, optional=optional)(f)
         return decorator
 
     def input(
         self,
         schema: SchemaType,
         location: str = 'json',
+        arg_name: t.Optional[str] = None,
         schema_name: t.Optional[str] = None,
         example: t.Optional[t.Any] = None,
         examples: t.Optional[t.Dict[str, t.Any]] = None,
         **kwargs: t.Any
     ) -> t.Callable[[DecoratedType], DecoratedType]:
         """Add input settings for view functions.
 
+        If the validation passed, the data will be injected into the view
+        function as a keyword argument in the form of `dict` and named `{location}_data`.
+        Otherwise, an error response with the detail of the validation result will be
+        returned.
+
         > Be sure to put it under the routes decorators (i.e., `app.route`, `app.get`,
         `app.post`, etc.).
 
-        If the validation passed, the data will inject into view
-        function as a positional argument in the form of `dict`. Otherwise,
-        an error response with the detail of the validation result will be returned.
-
         Examples:
 
         ```python
         from apiflask import APIFlask
 
         app = APIFlask(__name__)
 
         @app.get('/')
-        @app.input(PetIn)
-        def hello(parsed_and_validated_input_data):
-            print(parsed_and_validated_input_data)
+        @app.input(PetIn, location='json')
+        def hello(json_data):
+            print(json_data)
             return 'Hello'!
         ```
 
         Arguments:
             schema: The marshmallow schema of the input data.
             location: The location of the input data, one of `'json'` (default),
                 `'files'`, `'form'`, `'cookies'`, `'headers'`, `'query'`
                 (same as `'querystring'`).
+            arg_name: The name of the argument passed to the view function,
+                defaults to `{location}_data`.
             schema_name: The schema name for dict schema, only needed when you pass
                 a schema dict (e.g., `{'name': String(required=True)}`) for `json`
                 location.
             example: The example data in dict for request body, you should use either
                 `example` or `examples`, not both.
             examples: Multiple examples for request body, you should pass a dict
                 that contains multiple examples. Example:
@@ -263,14 +256,19 @@
                     'example bar': {
                         'summary': 'an example of bar',
                         'value': {'name': 'bar', 'id': 2}
                     },
                 }
                 ```
 
+        *Version changed: 2.0.0*
+
+        - Always pass parsed data to view function as a keyword argument.
+          The argument name will be in the form of `{location}_data`.
+
         *Version changed: 1.0*
 
         - Ensure only one input body location was used.
         - Add `form_and_files` and `json_or_form` (from webargs) location.
         - Rewrite `files` to act as `form_and_files`.
         - Use correct request content type for `form` and `files`.
 
@@ -317,15 +315,20 @@
             else:
                 if not hasattr(f, '_spec') or f._spec.get('args') is None:
                     _annotate(f, args=[])
                 if location == 'path':
                     _annotate(f, omit_default_path_parameters=True)
                 # TODO: Support set example for request parameters
                 f._spec['args'].append((schema, location))
-            return use_args(schema, location=location, **kwargs)(f)
+            return use_args(
+                schema,
+                location=location,
+                arg_name=arg_name or f'{location}_data',
+                **kwargs
+            )(f)
         return decorator
 
     def output(
         self,
         schema: SchemaType,
         status_code: int = 200,
         description: t.Optional[str] = None,
@@ -399,14 +402,18 @@
                 ```
 
                 See the [docs](https://apiflask.com/openapi/#response-links) for more details
                 about setting response links.
 
             content_type: The content/media type of the response. It defautls to `application/json`.
 
+        *Version changed: 2.0.0*
+
+        - Don't change the status code to 204 for EmptySchema.
+
         *Version changed: 1.3.0*
 
         - Add parameter `content_type`.
 
         *Version changed: 0.12.0*
 
         - Move to APIFlask and APIBlueprint classes.
@@ -434,17 +441,14 @@
         if schema == {}:
             schema = EmptySchema
         if isinstance(schema, ABCMapping):
             schema = _generate_schema_from_mapping(schema, schema_name)
         if isinstance(schema, type):  # pragma: no cover
             schema = schema()
 
-        if isinstance(schema, EmptySchema):
-            status_code = 204
-
         def decorator(f):
             f = _ensure_sync(f)
             _annotate(f, response={
                 'schema': schema,
                 'status_code': status_code,
                 'description': description,
                 'example': example,
@@ -506,15 +510,14 @@
             return _response
         return decorator
 
     def doc(
         self,
         summary: t.Optional[str] = None,
         description: t.Optional[str] = None,
-        tag: t.Optional[str] = None,
         tags: t.Optional[t.List[str]] = None,
         responses: t.Optional[t.Union[t.List[int], t.Dict[int, str]]] = None,
         deprecated: t.Optional[bool] = None,
         hide: t.Optional[bool] = None,
         operation_id: t.Optional[str] = None,
         security: t.Optional[t.Union[str, t.List[t.Union[str, t.Dict[str, list]]]]] = None,
     ) -> t.Callable[[DecoratedType], DecoratedType]:
@@ -544,15 +547,14 @@
 
                 ```
                 @app.doc(summary='blah') > the first line of docstring > the view function name
                 ```
 
             description: The description of this endpoint. If not set, the lines after the empty
                 line of the docstring will be used.
-            tag: Deprecated since 1.0, use `tags` instead.
             tags: A list of tag names of this endpoint, map the tags you passed in the `app.tags`
                 attribute. If `app.tags` is not set, the blueprint name will be used as tag name.
             responses: The other responses for this view function, accepts a dict in a format
                 of `{404: 'Not Found'}` or a list of status code (`[404, 418]`). If pass a dict,
                 and a response with the same status code is already exist, the existing
                 description will be overwritten.
             deprecated: Flag this endpoint as deprecated in API docs.
@@ -561,14 +563,18 @@
                 `True` to enable the auto-generating of operationId (in the format of
                 `{method}_{endpoint}`).
             security: The `security` used for this endpoint. Match the security info specified in
                 the `SECURITY_SCHEMES` configuration. If you don't need specify the scopes, just
                 pass a security name (equals to `[{'foo': []}]`) or a list of security names (equals
                 to `[{'foo': []}, {'bar': []}]`).
 
+        *Version changed: 2.0.0*
+
+        - Remove the deprecated `tag` parameter.
+
         *Version changed: 1.0*
 
         - Add `security` parameter to support customizing security info.
         - The `role` parameter is deprecated.
 
         *Version changed: 0.12.0*
 
@@ -589,33 +595,21 @@
         *Version changed: 0.3.0*
 
         - Change the default value of `deprecated` from `None` to `False`.
         - Rename parameter `tags` to `tag`.
 
         *Version added: 0.2.0*
         """
-        _tags = None
-        if tag is not None:
-            warnings.warn(
-                'The `tag` parameter is deprecated and will be removed in 1.1, '
-                'use `tags` and always pass a list instead.',
-                DeprecationWarning,
-                stacklevel=2,
-            )
-            _tags = [tag]
-        elif tags is not None:
-            _tags = tags
-
         def decorator(f):
             f = _ensure_sync(f)
             _annotate(
                 f,
                 summary=summary,
                 description=description,
-                tags=_tags,
+                tags=tags,
                 responses=responses,
                 deprecated=deprecated,
                 hide=hide,
                 operation_id=operation_id,
                 security=security,
             )
             return f
```

### Comparing `APIFlask-1.3.1/src/apiflask/security.py` & `APIFlask-2.0.0/src/apiflask/security.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/src/apiflask/settings.py` & `APIFlask-2.0.0/src/apiflask/settings.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/src/apiflask/types.py` & `APIFlask-2.0.0/src/apiflask/types.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/src/apiflask/ui_templates.py` & `APIFlask-2.0.0/src/apiflask/ui_templates.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/src/apiflask/validators.py` & `APIFlask-2.0.0/src/apiflask/validators.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/tests/schemas.py` & `APIFlask-2.0.0/tests/schemas.py`

 * *Files 13% similar despite different names*

```diff
@@ -76,7 +76,13 @@
     status_code = String(required=True)
     message = String(required=True)
 
 
 class HTTPError(Schema):
     status_code = String(required=True)
     message = String(required=True)
+
+
+class CustomHTTPError(Schema):
+    status_code = String(required=True)
+    message = String(required=True)
+    custom = String(required=True)
```

### Comparing `APIFlask-1.3.1/tests/test_app.py` & `APIFlask-2.0.0/tests/test_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pytest
 from apispec import BasePlugin
 from flask import Blueprint
+from flask.views import MethodView
 from openapi_spec_validator import validate_spec
 
 from .schemas import Bar
 from .schemas import Foo
 from .schemas import Pagination
 from apiflask import APIBlueprint
 from apiflask import APIFlask
 from apiflask import Schema
 from apiflask.fields import Integer
 from apiflask.fields import String
-from apiflask.views import MethodView
 
 
 def test_app_init(app):
     assert app
     assert hasattr(app, 'import_name')
     assert hasattr(app, 'title')
     assert 'TAGS' in app.config
@@ -70,29 +70,29 @@
         bar = String(required=True)
 
     class Pet(Schema):
         name = String(required=True)
         age = Integer(dump_default=123)
 
     @app.post('/pets/<int:pet_id>/toys/<int:toy_id>')
-    @app.input(Query, location='query')
-    @app.input(Pagination, location='query')
-    @app.input(Pet)
-    def pets(pet_id, toy_id, query, pagination, body):
+    @app.input(Query, location='query', arg_name='query')
+    @app.input(Pagination, location='query', arg_name='pagination')
+    @app.input(Pet, location='json')
+    def pets(pet_id, toy_id, query, pagination, json_data):
         return {'pet_id': pet_id, 'toy_id': toy_id,
-                'foo': query['foo'], 'bar': query['bar'], 'pagination': pagination, **body}
+                'foo': query['foo'], 'bar': query['bar'], 'pagination': pagination, **json_data}
 
     @app.route('/animals/<int:pet_id>/toys/<int:toy_id>')
     class Animals(MethodView):
-        @app.input(Query, location='query')
-        @app.input(Pagination, location='query')
-        @app.input(Pet)
-        def post(self, pet_id, toy_id, query, pagination, body):
+        @app.input(Query, location='query', arg_name='query')
+        @app.input(Pagination, location='query', arg_name='pagination')
+        @app.input(Pet, location='json')
+        def post(self, pet_id, toy_id, query, pagination, json_data):
             return {'pet_id': pet_id, 'toy_id': toy_id,
-                    'foo': query['foo'], 'bar': query['bar'], 'pagination': pagination, **body}
+                    'foo': query['foo'], 'bar': query['bar'], 'pagination': pagination, **json_data}
 
     rv = client.post('/pets/1/toys/3?foo=yes&bar=no',
                      json={'name': 'dodge', 'age': 5})
     assert rv.status_code == 200
     assert rv.json['pet_id'] == 1
     assert rv.json['toy_id'] == 3
     assert rv.json['foo'] == 'yes'
@@ -189,16 +189,16 @@
     assert '/spam' in rv.json['paths']
 
 
 def test_dispatch_static_request(app, client):
     # positional arguments
     @app.get('/mystatic/<int:pet_id>')
     @app.input(Foo)
-    def mystatic(pet_id, foo):  # endpoint: mystatic
-        return {'pet_id': pet_id, 'foo': foo}
+    def mystatic(pet_id, json_data):  # endpoint: mystatic
+        return {'pet_id': pet_id, 'foo': json_data}
 
     # positional arguments
     # blueprint static route accepts both keyword/positional arguments
     bp = APIBlueprint('foo', __name__, static_folder='static')
     app.register_blueprint(bp, url_prefix='/foo')
 
     rv = client.get('/mystatic/2', json={'id': 1, 'name': 'foo'})
```

### Comparing `APIFlask-1.3.1/tests/test_async.py` & `APIFlask-2.0.0/tests/test_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,13 @@
-import pytest
 from openapi_spec_validator import validate_spec
 
 from .schemas import Foo
 from apiflask import HTTPTokenAuth
 
 
-@pytest.fixture(autouse=True)
-def skip_async_test(app):
-    if not hasattr(app, 'ensure_sync'):
-        pytest.skip('This test requires Flask 2.0 or higher')
-
-
 def test_async_view(app, client):
 
     @app.get('/')
     async def index():
         return {'message': 'hello'}
 
     rv = client.get('/')
@@ -70,16 +63,16 @@
     assert rv.json['echo'] == 1234
 
 
 def test_input_on_async_view(app, client):
 
     @app.post('/')
     @app.input(Foo)
-    async def index(data):
-        return data
+    async def index(json_data):
+        return json_data
 
     data = {'id': 1, 'name': 'foo'}
     rv = client.post('/', json=data)
     assert rv.status_code == 200
     assert rv.json == data
 
 
@@ -105,14 +98,14 @@
 
 def test_async_doc_input_and_output_decorator(app, client):
 
     @app.post('/')
     @app.doc(summary='Test Root Endpoint')
     @app.input(Foo)
     @app.output(Foo)
-    async def index(data):
-        return data
+    async def index(json_data):
+        return json_data
 
     payload = {'id': 1, 'name': 'foo'}
     rv = client.post('/', json=payload)
     assert rv.status_code == 200
     assert rv.json == payload
```

### Comparing `APIFlask-1.3.1/tests/test_base_response.py` & `APIFlask-2.0.0/tests/test_base_response.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/tests/test_blueprint.py` & `APIFlask-2.0.0/tests/test_blueprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from flask.views import MethodView
 from openapi_spec_validator import validate_spec
 
 from apiflask import APIBlueprint
 from apiflask.security import HTTPBasicAuth
 from apiflask.security import HTTPTokenAuth
-from apiflask.views import MethodView
 
 
 def test_blueprint_object():
     bp = APIBlueprint('test', __name__)
     assert bp.name == 'test'
     assert hasattr(bp, 'tag')
     assert bp.tag is None
```

### Comparing `APIFlask-1.3.1/tests/test_commands.py` & `APIFlask-2.0.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/tests/test_decorator_auth_required.py` & `APIFlask-2.0.0/tests/test_decorator_auth_required.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from flask.views import MethodView
 from openapi_spec_validator import validate_spec
 
 from apiflask import APIBlueprint
 from apiflask.security import HTTPBasicAuth
 from apiflask.security import HTTPTokenAuth
-from apiflask.views import MethodView
 
 
 def test_auth_required(app, client):
     auth = HTTPBasicAuth()
 
     @auth.verify_password
     def verify_password(username, password):
```

### Comparing `APIFlask-1.3.1/tests/test_decorator_doc.py` & `APIFlask-2.0.0/tests/test_decorator_doc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
+from flask.views import MethodView
 from openapi_spec_validator import validate_spec
 
+from .schemas import CustomHTTPError
 from .schemas import Foo
-from apiflask.views import MethodView
 
 
 def test_doc_summary_and_description(app, client):
     @app.route('/foo')
     @app.doc(summary='summary from doc decorator')
     def foo():
         pass
@@ -199,14 +200,101 @@
     assert rv.json['paths']['/bar']['get']['responses'][
         '404']['description'] == 'Not Found'
     assert '500' in rv.json['paths']['/bar']['get']['responses']
     assert rv.json['paths']['/bar']['get']['responses'][
         '500']['description'] == 'Internal Server Error'
 
 
+def test_doc_responses_custom_spec(app, client):
+    response_spec = {
+        'description': 'Success',
+        'content': {
+            'application/json': {
+                'schema': {
+                    'type': 'object',
+                    'properties': {
+                        'data': {
+                            'type': 'object',
+                            'properties': {
+                                'id': {'type': 'integer'},
+                                'name': {'type': 'string'},
+                            }
+                        }
+                    }
+                }
+            }
+        }
+    }
+
+    @app.get('/foo')
+    @app.input(Foo)
+    @app.output(Foo)
+    @app.doc(responses={
+        200: response_spec
+    })
+    def foo():
+        return {'message': 'Hello!'}
+
+    @app.get('/bar')
+    @app.doc(responses={
+        200: {
+            'description': 'Success',
+            'content': {
+                'application/json': {
+                    'schema': Foo
+                }
+            }
+        },
+        400: {
+            'description': 'Error',
+            'content': {
+                'application/json': {
+                    'schema': CustomHTTPError
+                }
+            }
+        },
+        404: {
+            'description': 'Error',
+            'content': {
+                'application/json': {
+                    'schema': CustomHTTPError()
+                }
+            }
+        }
+    })
+    def say_hello():
+        return {'message': 'Hello!'}
+
+    rv = client.get('/openapi.json')
+    assert rv.status_code == 200
+    validate_spec(rv.json)
+    assert '200' in rv.json['paths']['/foo']['get']['responses']
+    assert rv.json['paths']['/foo']['get']['responses']['200'] == response_spec
+
+    assert '200' in rv.json['paths']['/bar']['get']['responses']
+    assert '400' in rv.json['paths']['/bar']['get']['responses']
+    assert '404' in rv.json['paths']['/bar']['get']['responses']
+    assert rv.json['paths']['/bar']['get']['responses'][
+        '200']['description'] == 'Success'
+    assert rv.json['paths']['/bar']['get']['responses'][
+        '400']['description'] == 'Error'
+    assert rv.json['paths']['/bar']['get']['responses'][
+        '400']['content']['application/json']['schema'] == {
+            '$ref': '#/components/schemas/CustomHTTPError'}
+    assert rv.json['components']['schemas']['CustomHTTPError'] == {
+        'type': 'object',
+        'properties': {
+            'status_code': {'type': 'string'},
+            'message': {'type': 'string'},
+            'custom': {'type': 'string'},
+        },
+        'required': ['custom', 'message', 'status_code'],
+    }
+
+
 def test_doc_responses_with_methodview(app, client):
     @app.route('/foo')
     class FooAPI(MethodView):
         @app.input(Foo)
         @app.output(Foo)
         @app.doc(responses={200: 'success', 400: 'bad', 404: 'not found', 500: 'server error'})
         def get(self):
```

### Comparing `APIFlask-1.3.1/tests/test_decorator_input.py` & `APIFlask-2.0.0/tests/test_decorator_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import io
 
 import pytest
+from flask.views import MethodView
 from openapi_spec_validator import validate_spec
 from werkzeug.datastructures import FileStorage
 
 from .schemas import Bar
 from .schemas import EnumPathParameter
 from .schemas import Files
 from .schemas import Foo
 from .schemas import Form
 from .schemas import FormAndFiles
 from apiflask.fields import String
-from apiflask.views import MethodView
 
 
 def test_input(app, client):
     @app.route('/foo', methods=['POST'])
     @app.input(Foo)
-    def foo(schema):
-        return schema
+    def foo(json_data):
+        return json_data
 
     @app.route('/bar')
     class Bar(MethodView):
         @app.input(Foo)
-        def post(self, data):
-            return data
+        def post(self, json_data):
+            return json_data
 
     for rule in ['/foo', '/bar']:
         rv = client.post(rule)
         assert rv.status_code == 422
         assert rv.json == {
             'detail': {
                 'json': {'name': ['Missing data for required field.']}
@@ -58,18 +58,18 @@
         validate_spec(rv.json)
         assert rv.json['paths'][rule]['post']['requestBody'][
             'content']['application/json']['schema']['$ref'] == '#/components/schemas/Foo'
 
 
 def test_input_with_query_location(app, client):
     @app.route('/foo', methods=['POST'])
-    @app.input(Foo, location='query')
-    @app.input(Bar, location='query')
-    def foo(schema, schema2):
-        return {'name': schema['name'], 'name2': schema2['name2']}
+    @app.input(Foo, location='query', arg_name='foo')
+    @app.input(Bar, location='query', arg_name='bar')
+    def foo(foo, bar):
+        return {'name': foo['name'], 'name2': bar['name2']}
 
     rv = client.post('/foo')
     assert rv.status_code == 422
     assert rv.json == {
         'detail': {
             'query': {'name': ['Missing data for required field.']}
         },
@@ -121,17 +121,15 @@
         data = {}
         if 'image' in files_data and isinstance(files_data['image'], FileStorage):
             data['image'] = True
         return data
 
     rv = client.get('/openapi.json')
     assert rv.status_code == 200
-    # TODO: Failed validating 'oneOf' in schema
-    # https://github.com/p1c2u/openapi-spec-validator/issues/113
-    # validate_spec(rv.json)
+    validate_spec(rv.json)
     assert 'multipart/form-data' in rv.json['paths']['/']['post']['requestBody']['content']
     assert rv.json['paths']['/']['post']['requestBody'][
         'content']['multipart/form-data']['schema']['$ref'] == '#/components/schemas/Files'
     assert 'image' in rv.json['components']['schemas']['Files']['properties']
     assert rv.json['components']['schemas']['Files']['properties']['image']['type'] == 'string'
     assert rv.json['components']['schemas']['Files']['properties']['image']['format'] == 'binary'
 
@@ -145,27 +143,25 @@
     assert rv.status_code == 200
     assert rv.json == {'image': True}
 
 
 def test_input_with_form_and_files_location(app, client):
     @app.post('/')
     @app.input(FormAndFiles, location='form_and_files')
-    def index(form_data):
+    def index(form_and_files_data):
         data = {}
-        if 'name' in form_data:
+        if 'name' in form_and_files_data:
             data['name'] = True
-        if 'image' in form_data and isinstance(form_data['image'], FileStorage):
+        if 'image' in form_and_files_data and isinstance(form_and_files_data['image'], FileStorage):
             data['image'] = True
         return data
 
     rv = client.get('/openapi.json')
     assert rv.status_code == 200
-    # TODO: Failed validating 'oneOf' in schema
-    # https://github.com/p1c2u/openapi-spec-validator/issues/113
-    # validate_spec(rv.json)
+    validate_spec(rv.json)
     assert 'multipart/form-data' in rv.json['paths']['/']['post']['requestBody']['content']
     assert rv.json['paths']['/']['post']['requestBody'][
         'content']['multipart/form-data']['schema']['$ref'] == '#/components/schemas/FormAndFiles'
     assert 'name' in rv.json['components']['schemas']['FormAndFiles']['properties']
     assert 'image' in rv.json['components']['schemas']['FormAndFiles']['properties']
     assert rv.json['components']['schemas']['FormAndFiles']['properties']['image'][
         'type'] == 'string'
@@ -180,22 +176,20 @@
     assert rv.status_code == 200
     assert rv.json == {'name': True, 'image': True}
 
 
 def test_input_with_path_location(app, client):
     @app.get('/<image_type>')
     @app.input(EnumPathParameter, location='path')
-    def index(image_type, _):
+    def index(image_type, path_data):
         return {'image_type': image_type}
 
     rv = client.get('/openapi.json')
     assert rv.status_code == 200
-    # TODO: Failed validating 'oneOf' in schema
-    # https://github.com/p1c2u/openapi-spec-validator/issues/113
-    # validate_spec(rv.json)
+    validate_spec(rv.json)
     assert '/{image_type}' in rv.json['paths']
     assert len(rv.json['paths']['/{image_type}']['get']['parameters']) == 1
     assert rv.json['paths']['/{image_type}']['get']['parameters'][0]['in'] == 'path'
     assert rv.json['paths']['/{image_type}']['get']['parameters'][0]['name'] == 'image_type'
     assert rv.json['paths']['/{image_type}']['get']['parameters'][0]['schema'] == {
         'type': 'string',
         'enum': ['jpg', 'png', 'tiff', 'webp'],
@@ -222,46 +216,48 @@
     ['form_and_files', 'files'],
     ['json_or_form', 'json'],
     ['json_or_form', 'files'],
     ['json_or_form', 'form'],
     ['json_or_form', 'form_and_files'],
 ])
 def test_multiple_input_body_location(app, locations):
+    arg_name_1 = f'{locations[0]}_data'  # noqa: F841
+    arg_name_2 = f'{locations[1]}_data'  # noqa: F841
     with pytest.raises(RuntimeError):
         @app.route('/foo')
-        @app.input(Foo, locations[0])
-        @app.input(Bar, locations[1])
-        def foo(query):
+        @app.input(Foo, location=locations[0])
+        @app.input(Bar, location=locations[1])
+        def foo(arg_name_1, arg_name_2):
             pass
 
 
 def test_input_with_dict_schema(app, client):
     dict_schema = {
         'name': String(required=True)
     }
 
     @app.get('/foo')
-    @app.input(dict_schema, 'query')
-    def foo(query):
-        return query
+    @app.input(dict_schema, location='query')
+    def foo(query_data):
+        return query_data
 
     @app.post('/bar')
     @app.input(dict_schema, schema_name='MyName')
-    def bar(body):
-        return body
+    def bar(json_data):
+        return json_data
 
     @app.post('/baz')
     @app.input(dict_schema)
-    def baz(body):
-        return body
+    def baz(json_data):
+        return json_data
 
     @app.post('/spam')
     @app.input(dict_schema)
-    def spam(body):
-        return body
+    def spam(json_data):
+        return json_data
 
     rv = client.get('/foo')
     assert rv.status_code == 422
     assert rv.json == {
         'detail': {
             'query': {'name': ['Missing data for required field.']}
         },
```

### Comparing `APIFlask-1.3.1/tests/test_decorator_output.py` & `APIFlask-2.0.0/tests/test_decorator_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from dataclasses import dataclass
 
 from flask import make_response
+from flask.views import MethodView
 from openapi_spec_validator import validate_spec
 
 from .schemas import Foo
 from .schemas import Query
 from apiflask import Schema
 from apiflask.fields import Field
 from apiflask.fields import String
-from apiflask.views import MethodView
 
 
 def test_output(app, client):
     @app.route('/foo')
     @app.output(Foo)
     def foo():
         return {'name': 'bar'}
@@ -21,20 +21,20 @@
     @app.output(Foo, status_code=201)
     def bar():
         return {'name': 'foo'}
 
     @app.route('/baz')
     @app.input(Query, location='query')
     @app.output(Foo, status_code=201)
-    def baz(query):
-        if query['id'] == 1:
+    def baz(query_data):
+        if query_data['id'] == 1:
             return {'name': 'baz'}, 202
-        elif query['id'] == 2:
+        elif query_data['id'] == 2:
             return {'name': 'baz'}, {'Location': '/baz'}
-        elif query['id'] == 3:
+        elif query_data['id'] == 3:
             return {'name': 'baz'}, 202, {'Location': '/baz'}
         return ({'name': 'baz'},)
 
     rv = client.get('/foo')
     assert rv.status_code == 200
     assert rv.json == {'id': 123, 'name': 'bar'}
 
@@ -72,20 +72,20 @@
 
         @app.output(Foo, status_code=201)
         def post(self):
             return {'name': 'foo'}
 
         @app.input(Query, location='query')
         @app.output(Foo, status_code=201)
-        def delete(self, query):
-            if query['id'] == 1:
+        def delete(self, query_data):
+            if query_data['id'] == 1:
                 return {'name': 'baz'}, 202
-            elif query['id'] == 2:
+            elif query_data['id'] == 2:
                 return {'name': 'baz'}, {'Location': '/baz'}
-            elif query['id'] == 3:
+            elif query_data['id'] == 3:
                 return {'name': 'baz'}, 202, {'Location': '/baz'}
             return ({'name': 'baz'},)
 
     rv = client.get('/')
     assert rv.status_code == 200
     assert rv.json == {'id': 123, 'name': 'bar'}
```

### Comparing `APIFlask-1.3.1/tests/test_exceptions.py` & `APIFlask-2.0.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/tests/test_fields.py` & `APIFlask-2.0.0/tests/test_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     assert rv.status_code == 422
     assert rv.json['detail']['files']['image'] == ['Not a valid file.']
 
 
 def test_multiple_file_field(app, client):
     @app.post('/')
     @app.input(FilesList, location='files')
-    def index(files_list_data):
+    def index(files_data):
         data = {'images': True}
-        for f in files_list_data['images']:
+        for f in files_data['images']:
             if not isinstance(f, FileStorage):
                 data['images'] = False
         return data
 
     rv = client.post(
         '/',
         data={
```

### Comparing `APIFlask-1.3.1/tests/test_helpers.py` & `APIFlask-2.0.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/tests/test_openapi_basic.py` & `APIFlask-2.0.0/tests/test_openapi_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
     app.register_blueprint(bp)
 
     spec = app._get_spec()
     assert '/static' not in spec['paths']
     assert '/foo/static' not in spec['paths']
     assert '/docs' not in spec['paths']
     assert '/openapi.json' not in spec['paths']
-    assert '/redoc' not in spec['paths']
     assert '/docs/oauth2-redirect' not in spec['paths']
 
 
 def test_spec_bypass_methods(app):
 
     class Foo:
         def bar(self):
```

### Comparing `APIFlask-1.3.1/tests/test_openapi_blueprint.py` & `APIFlask-2.0.0/tests/test_openapi_blueprint.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,33 +3,32 @@
 from apiflask import APIFlask
 
 
 def test_openapi_blueprint(app):
     assert 'openapi' in app.blueprints
     rules = list(app.url_map.iter_rules())
     bp_endpoints = [rule.endpoint for rule in rules if rule.endpoint.startswith('openapi')]
-    assert len(bp_endpoints) == 4
+    assert len(bp_endpoints) == 3
     assert 'openapi.spec' in bp_endpoints
     assert 'openapi.docs' in bp_endpoints
     assert 'openapi.swagger_ui_oauth_redirect' in bp_endpoints
-    assert 'openapi.redoc' in bp_endpoints
 
-    app = APIFlask(__name__, spec_path=None, docs_path=None, redoc_path=None)
+    app = APIFlask(__name__, spec_path=None, docs_path=None)
     assert 'openapi' not in app.blueprints
 
 
 def test_spec_path(app):
     assert app.spec_path
 
     app = APIFlask(__name__, spec_path=None)
     assert app.spec_path is None
     assert 'openapi' in app.blueprints
     rules = list(app.url_map.iter_rules())
     bp_endpoints = [rule.endpoint for rule in rules if rule.endpoint.startswith('openapi')]
-    assert len(bp_endpoints) == 3
+    assert len(bp_endpoints) == 2
     assert 'openapi.spec' not in bp_endpoints
 
 
 @pytest.mark.parametrize('spec_path', ['/spec.yaml', '/spec.yml'])
 def test_yaml_spec(spec_path):
     app = APIFlask(__name__, spec_path=spec_path)
     app.config['SPEC_FORMAT'] = 'yaml'
@@ -45,15 +44,15 @@
     assert app.docs_path
 
     app = APIFlask(__name__, docs_path=None)
     assert app.docs_path is None
 
     rules = list(app.url_map.iter_rules())
     bp_endpoints = [rule.endpoint for rule in rules if rule.endpoint.startswith('openapi')]
-    assert len(bp_endpoints) == 2
+    assert len(bp_endpoints) == 1
     assert 'openapi.docs' not in bp_endpoints
     assert 'openapi.swagger_ui_oauth_redirect' not in bp_endpoints
 
 
 def test_docs_oauth2_redirect_path(client):
     rv = client.get('/docs/oauth2-redirect')
     assert rv.status_code == 200
@@ -71,34 +70,22 @@
     assert b'oauth2RedirectUrl: "/docs/oauth2/redirect"' in rv.data
 
     app = APIFlask(__name__, docs_oauth2_redirect_path=None)
     assert app.docs_oauth2_redirect_path is None
 
     rules = list(app.url_map.iter_rules())
     bp_endpoints = [rule.endpoint for rule in rules if rule.endpoint.startswith('openapi')]
-    assert len(bp_endpoints) == 3
+    assert len(bp_endpoints) == 2
     assert 'openapi.docs' in bp_endpoints
     assert 'openapi.swagger_ui_oauth_redirect' not in bp_endpoints
     rv = app.test_client().get('/docs')
     assert rv.status_code == 200
     assert b'oauth2RedirectUrl' not in rv.data
 
 
-def test_redoc_path(app):
-    assert app.redoc_path
-
-    app = APIFlask(__name__, redoc_path=None)
-    assert app.redoc_path is None
-
-    rules = list(app.url_map.iter_rules())
-    bp_endpoints = [rule.endpoint for rule in rules if rule.endpoint.startswith('openapi')]
-    assert len(bp_endpoints) == 3
-    assert 'openapi.redoc' not in bp_endpoints
-
-
 def test_disable_openapi_with_enable_openapi_arg(app):
     assert app.enable_openapi
 
     app = APIFlask(__name__, enable_openapi=False)
     assert app.enable_openapi is False
 
     rules = list(app.url_map.iter_rules())
```

### Comparing `APIFlask-1.3.1/tests/test_openapi_info.py` & `APIFlask-2.0.0/tests/test_openapi_info.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/tests/test_openapi_paths.py` & `APIFlask-2.0.0/tests/test_openapi_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         'parameters'][2]['schema']['type'] == 'number'
 
 
 def test_path_arguments_order(app, client):
     @app.route('/<foo>/bar')
     @app.input(Query, location='query')
     @app.output(Foo)
-    def path_and_query(foo, query):
+    def path_and_query(foo, query_data):
         pass
 
     @app.route('/<foo>/<bar>')
     @app.output(Foo)
     def two_path_variables(foo, bar):
         pass
 
@@ -173,26 +173,26 @@
         'parameters'][1]['name'] == 'bar'
 
 
 def test_parameters_registration(app, client):
     @app.route('/foo')
     @app.input(Query, location='query')
     @app.output(Foo)
-    def foo(query):
+    def foo(query_data):
         pass
 
     @app.route('/bar')
-    @app.input(Query, location='query')
-    @app.input(Pagination, location='query')
+    @app.input(Query, location='query', arg_name='query')
+    @app.input(Pagination, location='query', arg_name='pagination')
     @app.input(Header, location='headers')
-    def bar(query, pagination, header):
+    def bar(query, pagination, headers_data):
         return {
             'query': query['id'],
             'pagination': pagination,
-            'foo': header['foo']
+            'foo': headers_data['foo']
         }
 
     rv = client.get('/openapi.json')
     assert rv.status_code == 200
     validate_spec(rv.json)
     assert '/foo' in rv.json['paths']
     assert '/bar' in rv.json['paths']
```

### Comparing `APIFlask-1.3.1/tests/test_openapi_security.py` & `APIFlask-2.0.0/tests/test_openapi_security.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/tests/test_openapi_tags.py` & `APIFlask-2.0.0/tests/test_openapi_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 import pytest
 from openapi_spec_validator import validate_spec
 
 from apiflask import APIBlueprint
 
 
-def skip_flask1():
-    if not hasattr(APIBlueprint, 'register_blueprint'):
-        pytest.skip('This test requires Flask 2.0 or higher')
-
-
 def test_tags(app, client):
     assert app.tags is None
     app.tags = [
         {
             'name': 'foo',
             'description': 'some description for foo',
             'externalDocs': {
@@ -88,15 +83,14 @@
     assert rv.status_code == 200
     validate_spec(rv.json)
     assert rv.json['tags']
     assert {'name': 'Foo'} in rv.json['tags']
 
 
 def test_auto_tag_from_nesting_blueprints(app, client):
-    skip_flask1()
 
     parent_bp = APIBlueprint('parent', __name__)
     child_bp = APIBlueprint('child', __name__)
     parent_bp.register_blueprint(child_bp)
     app.register_blueprint(parent_bp)
 
     rv = client.get('/openapi.json')
@@ -135,15 +129,14 @@
     rv = client.get('/openapi.json')
     assert rv.status_code == 200
     validate_spec(rv.json)
     assert rv.json['paths']['/']['get']['tags'] == ['test']
 
 
 def test_path_tags_with_nesting_blueprints(app, client):
-    skip_flask1()
 
     parent_bp = APIBlueprint('parent', __name__, url_prefix='/parent')
     child_bp = APIBlueprint('child', __name__, url_prefix='/child')
 
     @parent_bp.get('/')
     def foo():
         pass
```

### Comparing `APIFlask-1.3.1/tests/test_route.py` & `APIFlask-2.0.0/tests/test_route.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import pytest
-from flask.views import MethodView as FlaskMethodView
-from flask.views import View as FlaskView
+from flask.views import MethodView
+from flask.views import View
 from openapi_spec_validator import validate_spec
 
 from .schemas import Foo
 from apiflask import APIBlueprint
 from apiflask import HTTPTokenAuth
-from apiflask.views import MethodView
-from apiflask.views import View
 
 
 @pytest.mark.parametrize('method', ['get', 'post', 'put', 'patch', 'delete'])
 def test_route_shortcuts(app, client, method):
     route_method = getattr(app, method)
     client_method = getattr(client, method)
 
@@ -213,15 +211,15 @@
 
     rv = client.get('/openapi.json')
     assert rv.status_code == 200
     validate_spec(rv.json)
     assert rv.json['paths']['/']['get']
 
 
-@pytest.mark.parametrize('view_class', [View, FlaskView])
+@pytest.mark.parametrize('view_class', [View])
 def test_add_url_rule_skip_collecting_spec_from_view_class(app, client, view_class):
     class Foo(view_class):
         def dispatch_request(self):
             return 'Hello'
 
     app.add_url_rule('/foo', view_func=Foo.as_view('foo'))
 
@@ -229,22 +227,14 @@
     assert rv.status_code == 200
     assert '/foo' not in rv.json['paths']
 
     rv = client.get('/foo')
     assert rv.status_code == 200
 
 
-def test_runtime_error_on_flask_methodview_class(app):
-    with pytest.raises(RuntimeError):
-        class Foo(FlaskMethodView):
-            pass
-
-        app.add_url_rule('/foo', view_func=Foo.as_view('foo'))
-
-
 def test_empty_methodview_class(app, client):
     class Foo(MethodView):
         pass
 
     app.add_url_rule('/foo', view_func=Foo.as_view('foo'))
     rv = client.get('/openapi.json')
     assert rv.status_code == 200
```

### Comparing `APIFlask-1.3.1/tests/test_security.py` & `APIFlask-2.0.0/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/tests/test_settings_api_docs.py` & `APIFlask-2.0.0/tests/test_settings_api_docs.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,37 +8,43 @@
 
     rv = client.get('/docs')
     assert rv.status_code == 200
     assert b'href="/my-favicon.png"' in rv.data
 
 
 @pytest.mark.parametrize('config_value', [True, False])
-def test_docs_use_google_font(app, client, config_value):
+def test_docs_use_google_font(client, config_value):
+    app = APIFlask(__name__, docs_ui='redoc')
     app.config['REDOC_USE_GOOGLE_FONT'] = config_value
+    client = app.test_client()
 
-    rv = client.get('/redoc')
+    rv = client.get('/docs')
     assert rv.status_code == 200
     assert bool(b'fonts.googleapis.com' in rv.data) is config_value
 
 
-def test_redoc_standalone_js(app, client):
+def test_redoc_standalone_js(client):
+    app = APIFlask(__name__, docs_ui='redoc')
     app.config['REDOC_STANDALONE_JS'] = 'https://cdn.example.com/redoc.js'
+    client = app.test_client()
 
-    rv = client.get('/redoc')
+    rv = client.get('/docs')
     assert rv.status_code == 200
     assert b'src="https://cdn.example.com/redoc.js"' in rv.data
 
 
 @pytest.mark.parametrize('config_value', [
     {}, {'disableSearch': True, 'hideLoading': True}
 ])
-def test_redoc_config(app, client, config_value):
+def test_redoc_config(client, config_value):
+    app = APIFlask(__name__, docs_ui='redoc')
     app.config['REDOC_CONFIG'] = config_value
+    client = app.test_client()
 
-    rv = client.get('/redoc')
+    rv = client.get('/docs')
     assert rv.status_code == 200
     if config_value == {}:
         assert b'{},' in rv.data
     else:
         assert b'"disableSearch": true' in rv.data
         assert b'"hideLoading": true' in rv.data
```

### Comparing `APIFlask-1.3.1/tests/test_settings_auto_behaviour.py` & `APIFlask-2.0.0/tests/test_settings_auto_behaviour.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
+from flask.views import MethodView
 from openapi_spec_validator import validate_spec
 
 from .schemas import Foo
 from .schemas import Query
 from apiflask import APIBlueprint
 from apiflask.security import HTTPBasicAuth
-from apiflask.views import MethodView
 
 
 def test_auto_tags(app, client):
     bp = APIBlueprint('foo', __name__)
     app.config['AUTO_TAGS'] = False
 
     @bp.get('/')
```

### Comparing `APIFlask-1.3.1/tests/test_settings_openapi_fields.py` & `APIFlask-2.0.0/tests/test_settings_openapi_fields.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/tests/test_settings_openapi_spec.py` & `APIFlask-2.0.0/tests/test_settings_openapi_spec.py`

 * *Files identical despite different names*

### Comparing `APIFlask-1.3.1/tests/test_settings_response_customization.py` & `APIFlask-2.0.0/tests/test_settings_response_customization.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     @app.get('/bar')
     @app.output(Foo, status_code=201)
     def create():
         pass
 
     @app.get('/baz')
-    @app.output(EmptySchema)  # 204
+    @app.output(EmptySchema)
     def no_schema():
         pass
 
     @app.get('/spam')
     @app.output(Foo, status_code=206)
     def spam():
         pass
@@ -41,15 +41,15 @@
     assert rv.status_code == 200
     validate_spec(rv.json)
     assert rv.json['paths']['/foo']['get']['responses'][
         '200']['description'] == 'Success'
     assert rv.json['paths']['/bar']['get']['responses'][
         '201']['description'] == 'Success'
     assert rv.json['paths']['/baz']['get']['responses'][
-        '204']['description'] == 'Success'
+        '200']['description'] == 'Success'
     assert rv.json['paths']['/spam']['get']['responses'][
         '206']['description'] == 'Success'
     assert rv.json['paths']['/eggs/{id}']['get']['responses'][
         '404']['description'] == 'Egg not found'
 
 
 def test_validation_error_status_code_and_description(app, client):
```

### Comparing `APIFlask-1.3.1/tox.ini` & `APIFlask-2.0.0/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 [tox]
 envlist =
-    py3{11,10,9,8,7},pypy3{8,7}
-    py310-min
-    py37-dev
+    py3{11,10,9,8}
+    pypy310
+    minimal
     style
     typing
     docs
-    flask1
 skip_missing_interpreters = True
 
 [testenv]
 deps =
     -r requirements/tests.txt
     -r requirements/examples.txt
 commands =
     pytest -v
 
+# test with minimal dependencies
+# make sure no extra dependencies are introduced
+[testenv:minimal]
+deps =
+    -e .
+commands =
+    python -c "from apiflask import APIFlask"
+
 [testenv:style]
 deps = pre-commit
 skip_install = true
 commands =
     pre-commit run --all-files
 
 [testenv:docs]
 deps = -r requirements/docs.txt
 whitelist_externals = mkdocs
 commands = mkdocs build
 
 [testenv:typing]
 deps = -r requirements/typing.txt
 commands = mypy
-
-[testenv:flask1]
-deps =
-    -r requirements/tests.txt
-    flask == 1.1.4
-    markupsafe == 2.0.1
-commands =
-    pytest -v {posargs: tests}
```

