# Comparing `tmp/flask-rest-jsonapi-next-0.40.0.tar.gz` & `tmp/flask-rest-jsonapi-next-0.41.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-rest-jsonapi-next-0.40.0.tar", last modified: Fri Jul 21 17:53:07 2023, max compression
+gzip compressed data, was "flask-rest-jsonapi-next-0.41.0.tar", last modified: Wed Jul 26 13:38:39 2023, max compression
```

## Comparing `flask-rest-jsonapi-next-0.40.0.tar` & `flask-rest-jsonapi-next-0.41.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.873710 flask-rest-jsonapi-next-0.40.0/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-21 17:53:07.873710 flask-rest-jsonapi-next-0.40.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.865710 flask-rest-jsonapi-next-0.40.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/data_layer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/filtering.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/flask-rest-jsonapi-next.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.865710 flask-rest-jsonapi-next-0.40.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    60801 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/img/schema.png
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/include_related_objects.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/logical_data_abstraction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/oauth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/pagination.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/permission.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25464 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/resource_manager.rst
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/routing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/sorting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/sparse_fieldsets.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/docs/sqlalchemy_2x_support.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.865710 flask-rest-jsonapi-next-0.40.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/examples/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/examples/api_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 17:53:07.873710 flask-rest-jsonapi-next-0.40.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.861710 flask-rest-jsonapi-next-0.40.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37548 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/alchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13929 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/filtering/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/filtering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/filtering/alchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/error_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/errors_as_json_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/flask_rest_jsonapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/marshamallow.py
--rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/werkzeug.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/querystring.py
--rw-r--r--   0 runner    (1001) docker     (123)    22299 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-21 17:53:07.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-21 17:53:07.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:53:07.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:53:07.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-21 17:53:07.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 17:53:07.000000 flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/content_type_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.869710 flask-rest-jsonapi-next-0.40.0/tests/factories/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/flask_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.873710 flask-rest-jsonapi-next-0.40.0/tests/factories/models/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/computer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/person_single_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/person_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/models/string_json_attribute_person.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:53:07.873710 flask-rest-jsonapi-next-0.40.0/tests/factories/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/resources/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/resources/computer.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/resources/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/resources/person.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/factories/resources/string_json_attribute_person.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/querystring_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/resource_detail_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/resource_list_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/resource_relationship_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/sqlalchemy_data_layer_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-21 17:52:57.000000 flask-rest-jsonapi-next-0.40.0/tests/sqlalchemy_filtering_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:39.807026 flask-rest-jsonapi-next-0.41.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-26 13:38:39.807026 flask-rest-jsonapi-next-0.41.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:39.799026 flask-rest-jsonapi-next-0.41.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/data_layer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/filtering.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/flask-rest-jsonapi-next.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:39.799026 flask-rest-jsonapi-next-0.41.0/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    60801 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/img/schema.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/include_related_objects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/logical_data_abstraction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/oauth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/pagination.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/permission.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25464 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/resource_manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/routing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/sorting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/sparse_fieldsets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/docs/sqlalchemy_2x_support.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:39.799026 flask-rest-jsonapi-next-0.41.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/examples/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/examples/api_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:38:39.807026 flask-rest-jsonapi-next-0.41.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:39.795025 flask-rest-jsonapi-next-0.41.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:39.799026 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:39.803026 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/data_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/data_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37548 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/data_layers/alchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13929 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/data_layers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:39.803026 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/data_layers/filtering/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/data_layers/filtering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/data_layers/filtering/alchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:39.803026 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/error_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/errors_as_json_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:39.803026 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/flask_rest_jsonapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/marshamallow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/werkzeug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22299 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:39.803026 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-26 13:38:39.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-26 13:38:39.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:38:39.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:38:39.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-26 13:38:39.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-26 13:38:39.000000 flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:39.803026 flask-rest-jsonapi-next-0.41.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/content_type_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:39.803026 flask-rest-jsonapi-next-0.41.0/tests/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/flask_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:39.803026 flask-rest-jsonapi-next-0.41.0/tests/factories/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/models/computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/models/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/models/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/models/person_single_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/models/person_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/models/string_json_attribute_person.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:38:39.807026 flask-rest-jsonapi-next-0.41.0/tests/factories/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/resources/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/resources/computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/resources/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/resources/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/factories/resources/string_json_attribute_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/querystring_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/resource_detail_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/resource_list_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/resource_relationship_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/sqlalchemy_data_layer_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-26 13:38:29.000000 flask-rest-jsonapi-next-0.41.0/tests/sqlalchemy_filtering_spec.py
```

### Comparing `flask-rest-jsonapi-next-0.40.0/CHANGELOG.md` & `flask-rest-jsonapi-next-0.41.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # CHANGELOG
 
+## 0.410.0 (2023-07-26)
+
+- fix: don't log stacktrace for common exceptions
+- fix: defend from empty filters
+
 ## 0.40.0 (2023-07-21)
 
 - removed restriction on SQLAlchemy version, library now works with SQLAlchemy 2.x
   - working with SQLAlchemy 2.x layer requires some changes in client code, otherwise
     there might be performance penalties
   - added docs section on SQLAlchemy 2.x usage
 - tested with psycopg 3
```

### Comparing `flask-rest-jsonapi-next-0.40.0/LICENSE` & `flask-rest-jsonapi-next-0.41.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/PKG-INFO` & `flask-rest-jsonapi-next-0.41.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rest-jsonapi-next
-Version: 0.40.0
+Version: 0.41.0
 Summary: Flask extension to create REST web api according to JSONAPI 1.0 specification with Flask, Marshmallow and data provider of your choice (SQLAlchemy, MongoDB, ...)
 Author: original miLibris/flask-rest-jsonapi contributors
 Maintainer-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-rest-jsonapi-next
 Project-URL: Documentation, https://flask-rest-jsonapi-next.readthedocs.io/en/latest/
 Keywords: web,api,rest,jsonapi,flask,sqlalchemy,marshmallow
```

### Comparing `flask-rest-jsonapi-next-0.40.0/README.md` & `flask-rest-jsonapi-next-0.41.0/README.md`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/Makefile` & `flask-rest-jsonapi-next-0.41.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/conf.py` & `flask-rest-jsonapi-next-0.41.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "flask-rest-jsonapi-next"
 copyright = "2016-2021 miLibris; 2021-... miLibris, tadams42"
 author = "tadams42"
-release = "0.40.0"
+release = "0.41.0"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
```

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/data_layer.rst` & `flask-rest-jsonapi-next-0.41.0/docs/data_layer.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/errors.rst` & `flask-rest-jsonapi-next-0.41.0/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/features.rst` & `flask-rest-jsonapi-next-0.41.0/docs/features.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/filtering.rst` & `flask-rest-jsonapi-next-0.41.0/docs/filtering.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/flask-rest-jsonapi-next.rst` & `flask-rest-jsonapi-next-0.41.0/docs/flask-rest-jsonapi-next.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/img/schema.png` & `flask-rest-jsonapi-next-0.41.0/docs/img/schema.png`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/include_related_objects.rst` & `flask-rest-jsonapi-next-0.41.0/docs/include_related_objects.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/index.rst` & `flask-rest-jsonapi-next-0.41.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/installation.rst` & `flask-rest-jsonapi-next-0.41.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/logical_data_abstraction.rst` & `flask-rest-jsonapi-next-0.41.0/docs/logical_data_abstraction.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/make.bat` & `flask-rest-jsonapi-next-0.41.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/oauth.rst` & `flask-rest-jsonapi-next-0.41.0/docs/oauth.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/pagination.rst` & `flask-rest-jsonapi-next-0.41.0/docs/pagination.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/permission.rst` & `flask-rest-jsonapi-next-0.41.0/docs/permission.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/quickstart.rst` & `flask-rest-jsonapi-next-0.41.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/resource_manager.rst` & `flask-rest-jsonapi-next-0.41.0/docs/resource_manager.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/routing.rst` & `flask-rest-jsonapi-next-0.41.0/docs/routing.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/sorting.rst` & `flask-rest-jsonapi-next-0.41.0/docs/sorting.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/sparse_fieldsets.rst` & `flask-rest-jsonapi-next-0.41.0/docs/sparse_fieldsets.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/docs/sqlalchemy_2x_support.rst` & `flask-rest-jsonapi-next-0.41.0/docs/sqlalchemy_2x_support.rst`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/examples/api.py` & `flask-rest-jsonapi-next-0.41.0/examples/api.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/examples/api_nested.py` & `flask-rest-jsonapi-next-0.41.0/examples/api_nested.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/pyproject.toml` & `flask-rest-jsonapi-next-0.41.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 # setuptools v64 was first to support `pip install -e` for packages defined using
 # pyproject.toml (older versions support this, but only for setup.py projects)
 requires = ["setuptools>=64", "wheel"]
 
 [project]
 name = "flask-rest-jsonapi-next"
-version = "0.40.0"
+version = "0.41.0"
 description = "Flask extension to create REST web api according to JSONAPI 1.0 specification with Flask, Marshmallow and data provider of your choice (SQLAlchemy, MongoDB, ...)"
 readme = "README.md"
 classifiers = [
 	"Framework :: Flask",
 	"Programming Language :: Python :: 3",
 	"Programming Language :: Python :: 3.7",
 	"Programming Language :: Python :: 3.8",
```

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/api.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/api.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/alchemy.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/data_layers/alchemy.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/base.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/data_layers/base.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/data_layers/filtering/alchemy.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/data_layers/filtering/alchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,19 @@
     """Apply filters from filters information to base query
 
     :param DeclarativeMeta model: the model of the node
     :param dict filter_info: current node filter information
     :param Resource resource: the resource
     """
     filters = []
+
     for filter_ in filter_info:
-        filters.append(Node(model, filter_, resource, resource.schema).resolve())
+        resolved = Node(model, filter_, resource, resource.schema).resolve()
+        if resolved is not None:
+            filters.append(resolved)
 
     return filters
 
 
 class Node(object):
     """Helper to recursively create filters with sqlalchemy according to filter querystring parameter"""
 
@@ -57,25 +60,25 @@
                 value = {self.filter_["name"].split("__")[1]: value}
 
             if isinstance(value, dict):
                 return getattr(self.column, self.operator)(**value)
             else:
                 return getattr(self.column, self.operator)(value)
 
-        if "or" in self.filter_:
+        if "or" in self.filter_ and self.filter_["or"]:
             return or_(
                 Node(self.model, filt, self.resource, self.schema).resolve()
                 for filt in self.filter_["or"]
             )
-        if "and" in self.filter_:
+        if "and" in self.filter_ and self.filter_["and"]:
             return and_(
                 Node(self.model, filt, self.resource, self.schema).resolve()
                 for filt in self.filter_["and"]
             )
-        if "not" in self.filter_:
+        if "not" in self.filter_ and self.filter_["not"]:
             return not_(
                 Node(
                     self.model, self.filter_["not"], self.resource, self.schema
                 ).resolve()
             )
 
     @property
```

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/decorators.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/decorators.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/error_formatters.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/error_formatters.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/errors_as_json_api.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/errors_as_json_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from typing import Callable, Optional, Type, Union
 
 import flask
 from werkzeug.exceptions import default_exceptions
+from marshmallow import ValidationError
 
 from .error_formatters import error_response_from
 
 logger = logging.getLogger(__name__)
 
 
 class ErrorsAsJsonApi:
@@ -52,23 +53,22 @@
         """
         (app or flask.current_app).register_error_handler(
             exception_or_code, handler or cls._std_handler
         )
 
     @classmethod
     def _std_handler(cls, error):
-        if error in {401, 403, 405} or isinstance(
-            error,
-            (default_exceptions[401], default_exceptions[403], default_exceptions[405]),
+        if isinstance(error, ValidationError):
+            logger.error(f"ValidationError: {error}", exc_info=False)
+        elif error == 405 or isinstance(error, default_exceptions[405]):
+            logger.error(f"{error} ", exc_info=False)
+        elif error in {401, 403} or isinstance(
+            error, (default_exceptions[401], default_exceptions[403])
         ):
-            logger.debug(
-                "Exception bubbled to top level handler and was returned as HTTP "
-                "JSON response.",
-                exc_info=True,
-            )
+            logger.error(f"Authentication {error}", exc_info=False)
         else:
             logger.error(
                 "Exception bubbled to top level handler and was returned as HTTP "
                 "JSON response.",
                 exc_info=True,
             )
```

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/base.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/base.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/marshamallow.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/marshamallow.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/sqlalchemy.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/exception_converters/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/error_responses/exceptions.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/error_responses/exceptions.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/exceptions.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/exceptions.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/pagination.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/pagination.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/querystring.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/querystring.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/resource.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/resource.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next/schema.py` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next/schema.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/PKG-INFO` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rest-jsonapi-next
-Version: 0.40.0
+Version: 0.41.0
 Summary: Flask extension to create REST web api according to JSONAPI 1.0 specification with Flask, Marshmallow and data provider of your choice (SQLAlchemy, MongoDB, ...)
 Author: original miLibris/flask-rest-jsonapi contributors
 Maintainer-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-rest-jsonapi-next
 Project-URL: Documentation, https://flask-rest-jsonapi-next.readthedocs.io/en/latest/
 Keywords: web,api,rest,jsonapi,flask,sqlalchemy,marshmallow
```

### Comparing `flask-rest-jsonapi-next-0.40.0/src/flask_rest_jsonapi_next.egg-info/SOURCES.txt` & `flask-rest-jsonapi-next-0.41.0/src/flask_rest_jsonapi_next.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/content_type_spec.py` & `flask-rest-jsonapi-next-0.41.0/tests/content_type_spec.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/factories/flask_app.py` & `flask-rest-jsonapi-next-0.41.0/tests/factories/flask_app.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/factories/models/computer.py` & `flask-rest-jsonapi-next-0.41.0/tests/factories/models/computer.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/factories/models/db.py` & `flask-rest-jsonapi-next-0.41.0/tests/factories/models/db.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/factories/models/fixtures.py` & `flask-rest-jsonapi-next-0.41.0/tests/factories/models/fixtures.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/factories/models/person.py` & `flask-rest-jsonapi-next-0.41.0/tests/factories/models/person.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/factories/models/person_single_tag.py` & `flask-rest-jsonapi-next-0.41.0/tests/factories/models/person_single_tag.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/factories/models/person_tag.py` & `flask-rest-jsonapi-next-0.41.0/tests/factories/models/person_tag.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/factories/models/string_json_attribute_person.py` & `flask-rest-jsonapi-next-0.41.0/tests/factories/models/string_json_attribute_person.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/factories/resources/computer.py` & `flask-rest-jsonapi-next-0.41.0/tests/factories/resources/computer.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/factories/resources/person.py` & `flask-rest-jsonapi-next-0.41.0/tests/factories/resources/person.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/factories/resources/string_json_attribute_person.py` & `flask-rest-jsonapi-next-0.41.0/tests/factories/resources/string_json_attribute_person.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/querystring_spec.py` & `flask-rest-jsonapi-next-0.41.0/tests/querystring_spec.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/resource_detail_spec.py` & `flask-rest-jsonapi-next-0.41.0/tests/resource_detail_spec.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/resource_list_spec.py` & `flask-rest-jsonapi-next-0.41.0/tests/resource_list_spec.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/resource_relationship_spec.py` & `flask-rest-jsonapi-next-0.41.0/tests/resource_relationship_spec.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/resource_spec.py` & `flask-rest-jsonapi-next-0.41.0/tests/resource_spec.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/sqlalchemy_data_layer_spec.py` & `flask-rest-jsonapi-next-0.41.0/tests/sqlalchemy_data_layer_spec.py`

 * *Files identical despite different names*

### Comparing `flask-rest-jsonapi-next-0.40.0/tests/sqlalchemy_filtering_spec.py` & `flask-rest-jsonapi-next-0.41.0/tests/sqlalchemy_filtering_spec.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,7 +29,17 @@
         n.model = person_model
         n.filter_["op"] = ""
         n.operator
     with pytest.raises(InvalidFilters):
         n.related_model
     with pytest.raises(InvalidFilters):
         n.related_schema
+
+
+def test_Node_empty_filter(person_model, person_schema):
+    for filt in [
+        {"and": []},
+        {"or": []},
+        {"not": []},
+    ]:
+        resolved = Node(person_model, filt, None, person_schema).resolve()
+        assert resolved is None
```

