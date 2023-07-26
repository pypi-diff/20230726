# Comparing `tmp/gql-3.5.0b4.tar.gz` & `tmp/gql-3.5.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gql-3.5.0b4.tar", last modified: Sat May  6 19:36:59 2023, max compression
+gzip compressed data, was "gql-3.5.0b5.tar", last modified: Wed Jul 26 10:15:24 2023, max compression
```

## Comparing `gql-3.5.0b4.tar` & `gql-3.5.0b5.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.502615 gql-3.5.0b4/
--rw-r--r--   0 runner    (1001) docker     (122)      603 2023-05-06 19:36:54.000000 gql-3.5.0b4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-06 19:36:54.000000 gql-3.5.0b4/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)     4069 2023-05-06 19:36:54.000000 gql-3.5.0b4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-06 19:36:54.000000 gql-3.5.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      464 2023-05-06 19:36:54.000000 gql-3.5.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      875 2023-05-06 19:36:54.000000 gql-3.5.0b4/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     6203 2023-05-06 19:36:59.502615 gql-3.5.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4276 2023-05-06 19:36:54.000000 gql-3.5.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.474614 gql-3.5.0b4/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.474614 gql-3.5.0b4/docs/advanced/
--rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/advanced/async_advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/advanced/async_permanent_session.rst
--rw-r--r--   0 runner    (1001) docker     (122)    11000 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/advanced/dsl_module.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3143 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/advanced/error_handling.rst
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/advanced/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/advanced/local_schema.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/advanced/logging.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.478614 gql-3.5.0b4/docs/async/
--rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/async/async_intro.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1251 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/async/async_usage.rst
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/async/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.478614 gql-3.5.0b4/docs/code_examples/
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/aiohttp_async.py
--rw-r--r--   0 runner    (1001) docker     (122)     1783 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/aiohttp_async_dsl.py
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/aiohttp_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.478614 gql-3.5.0b4/docs/code_examples/appsync/
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/appsync/mutation_api_key.py
--rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/appsync/mutation_iam.py
--rw-r--r--   0 runner    (1001) docker     (122)     1254 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/appsync/subscription_api_key.py
--rw-r--r--   0 runner    (1001) docker     (122)      941 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/appsync/subscription_iam.py
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/console_async.py
--rw-r--r--   0 runner    (1001) docker     (122)     2033 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/fastapi_async.py
--rw-r--r--   0 runner    (1001) docker     (122)      788 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/httpx_async.py
--rw-r--r--   0 runner    (1001) docker     (122)      377 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/httpx_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)      734 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/phoenix_channel_async.py
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/reconnecting_mutation_http.py
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/reconnecting_mutation_ws.py
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/reconnecting_subscription.py
--rw-r--r--   0 runner    (1001) docker     (122)      433 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/requests_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/requests_sync_dsl.py
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/websockets_async.py
--rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.478614 gql-3.5.0b4/docs/gql-cli/
--rw-r--r--   0 runner    (1001) docker     (122)     2057 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/gql-cli/intro.rst
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4166 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.482615 gql-3.5.0b4/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/client.rst
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/dsl.rst
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/gql.rst
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport.rst
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_aiohttp.rst
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_appsync_auth.rst
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_appsync_websockets.rst
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_httpx.rst
--rw-r--r--   0 runner    (1001) docker     (122)      229 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_phoenix_channel_websockets.rst
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_requests.rst
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_websockets.rst
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_websockets_base.rst
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.482615 gql-3.5.0b4/docs/transports/
--rw-r--r--   0 runner    (1001) docker     (122)     1474 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/aiohttp.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5965 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/appsync.rst
--rw-r--r--   0 runner    (1001) docker     (122)      301 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/async_transports.rst
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/httpx.rst
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/httpx_async.rst
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/phoenix.rst
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/requests.rst
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/sync_transports.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5481 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/websockets.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.486615 gql-3.5.0b4/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/basic_usage.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10061 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/custom_scalars_and_enums.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5898 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/file_upload.rst
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/headers.rst
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/subscriptions.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/validation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      790 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/variables.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.486615 gql-3.5.0b4/gql/
--rw-r--r--   0 runner    (1001) docker     (122)      463 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16695 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    52066 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    36033 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/dsl.py
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/gql.py
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.490615 gql-3.5.0b4/gql/transport/
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13451 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (122)     7515 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/appsync_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/appsync_websockets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/async_transport.py
--rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    10440 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/httpx.py
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/local_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)    15179 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/phoenix_channel_websockets.py
--rw-r--r--   0 runner    (1001) docker     (122)    10021 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/requests.py
--rw-r--r--   0 runner    (1001) docker     (122)      991 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/transport.py
--rw-r--r--   0 runner    (1001) docker     (122)    19190 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/websockets.py
--rw-r--r--   0 runner    (1001) docker     (122)    24466 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/websockets_base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.490615 gql-3.5.0b4/gql/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3165 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utilities/build_client_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     3865 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utilities/get_introspection_query_ast.py
--rw-r--r--   0 runner    (1001) docker     (122)    14304 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utilities/parse_result.py
--rw-r--r--   0 runner    (1001) docker     (122)     4261 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utilities/serialize_variable_values.py
--rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utilities/update_schema_enum.py
--rw-r--r--   0 runner    (1001) docker     (122)     2280 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utilities/update_schema_scalars.py
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.490615 gql-3.5.0b4/gql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6203 2023-05-06 19:36:59.000000 gql-3.5.0b4/gql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-05-06 19:36:59.000000 gql-3.5.0b4/gql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 19:36:59.000000 gql-3.5.0b4/gql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-06 19:36:59.000000 gql-3.5.0b4/gql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 19:36:59.000000 gql-3.5.0b4/gql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-05-06 19:36:59.000000 gql-3.5.0b4/gql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-05-06 19:36:59.000000 gql-3.5.0b4/gql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-05-06 19:36:59.502615 gql-3.5.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3262 2023-05-06 19:36:54.000000 gql-3.5.0b4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.494614 gql-3.5.0b4/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15031 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.498615 gql-3.5.0b4/tests/custom_scalars/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/custom_scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6593 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/custom_scalars/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (122)     6960 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/custom_scalars/test_enum_colors.py
--rw-r--r--   0 runner    (1001) docker     (122)     5153 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/custom_scalars/test_json.py
--rw-r--r--   0 runner    (1001) docker     (122)    20717 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/custom_scalars/test_money.py
--rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/custom_scalars/test_parse_results.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.498615 gql-3.5.0b4/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.498615 gql-3.5.0b4/tests/fixtures/aws/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      885 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/aws/fake_credentials.py
--rw-r--r--   0 runner    (1001) docker     (122)      604 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/aws/fake_request.py
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/aws/fake_session.py
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/aws/fake_signer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.498615 gql-3.5.0b4/tests/fixtures/graphql/
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/graphql/sample.graphql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.498615 gql-3.5.0b4/tests/fixtures/vcr_cassettes/
--rw-r--r--   0 runner    (1001) docker     (122)     5340 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/vcr_cassettes/client.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    78820 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/vcr_cassettes/queries.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.498615 gql-3.5.0b4/tests/nested_input/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/nested_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/nested_input/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/nested_input/test_nested_input.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.502615 gql-3.5.0b4/tests/starwars/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     7990 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)    23843 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/test_dsl.py
--rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (122)     3587 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/test_parse_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     7529 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/test_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     2594 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (122)     5441 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (122)    43147 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3320 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_aiohttp_online.py
--rw-r--r--   0 runner    (1001) docker     (122)     6588 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_appsync_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_appsync_http.py
--rw-r--r--   0 runner    (1001) docker     (122)    23922 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_appsync_websockets.py
--rw-r--r--   0 runner    (1001) docker     (122)     7303 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_async_client_validation.py
--rw-r--r--   0 runner    (1001) docker     (122)    12020 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     7011 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     7525 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_graphqlws_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    27257 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_graphqlws_subscription.py
--rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_http_async_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)    26413 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_httpx.py
--rw-r--r--   0 runner    (1001) docker     (122)    38462 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_httpx_async.py
--rw-r--r--   0 runner    (1001) docker     (122)     3320 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_httpx_online.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_localhost.cnf
--rw-r--r--   0 runner    (1001) docker     (122)     2908 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_localhost.pem
--rw-r--r--   0 runner    (1001) docker     (122)    15131 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_phoenix_channel_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4079 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_phoenix_channel_query.py
--rw-r--r--   0 runner    (1001) docker     (122)    12704 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_phoenix_channel_subscription.py
--rw-r--r--   0 runner    (1001) docker     (122)    26692 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (122)     3517 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (122)    11402 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_websocket_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     6236 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_websocket_online.py
--rw-r--r--   0 runner    (1001) docker     (122)    17431 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_websocket_query.py
--rw-r--r--   0 runner    (1001) docker     (122)    18656 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_websocket_subscription.py
--rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-05-06 19:36:54.000000 gql-3.5.0b4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.706527 gql-3.5.0b5/
+-rw-r--r--   0 runner    (1001) docker     (122)      603 2023-07-26 10:15:21.000000 gql-3.5.0b5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-26 10:15:21.000000 gql-3.5.0b5/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     4069 2023-07-26 10:15:21.000000 gql-3.5.0b5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-07-26 10:15:21.000000 gql-3.5.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      464 2023-07-26 10:15:21.000000 gql-3.5.0b5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      875 2023-07-26 10:15:21.000000 gql-3.5.0b5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-07-26 10:15:24.706527 gql-3.5.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4342 2023-07-26 10:15:21.000000 gql-3.5.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.690527 gql-3.5.0b5/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.690527 gql-3.5.0b5/docs/advanced/
+-rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/advanced/async_advanced_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/advanced/async_permanent_session.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11000 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/advanced/dsl_module.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3143 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/advanced/error_handling.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/advanced/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/advanced/local_schema.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/advanced/logging.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.690527 gql-3.5.0b5/docs/async/
+-rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/async/async_intro.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1251 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/async/async_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/async/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.694527 gql-3.5.0b5/docs/code_examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/aiohttp_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1783 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/aiohttp_async_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/aiohttp_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.694527 gql-3.5.0b5/docs/code_examples/appsync/
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/appsync/mutation_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/appsync/mutation_iam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1254 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/appsync/subscription_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (122)      941 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/appsync/subscription_iam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/console_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2033 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/fastapi_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/httpx_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)      377 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/httpx_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)      734 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/phoenix_channel_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/reconnecting_mutation_http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/reconnecting_mutation_ws.py
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/reconnecting_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/requests_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/requests_sync_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/code_examples/websockets_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.694527 gql-3.5.0b5/docs/gql-cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     2057 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/gql-cli/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4166 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.694527 gql-3.5.0b5/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/modules/client.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/modules/dsl.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/modules/gql.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/modules/transport.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/modules/transport_aiohttp.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/modules/transport_appsync_auth.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/modules/transport_appsync_websockets.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/modules/transport_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/modules/transport_httpx.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/modules/transport_phoenix_channel_websockets.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/modules/transport_requests.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/modules/transport_websockets.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/modules/transport_websockets_base.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/modules/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.694527 gql-3.5.0b5/docs/transports/
+-rw-r--r--   0 runner    (1001) docker     (122)     1474 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/transports/aiohttp.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5965 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/transports/appsync.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/transports/async_transports.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/transports/httpx.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/transports/httpx_async.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/transports/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/transports/phoenix.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/transports/requests.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/transports/sync_transports.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5481 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/transports/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.698526 gql-3.5.0b5/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/usage/basic_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10061 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/usage/custom_scalars_and_enums.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/usage/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5898 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/usage/file_upload.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/usage/headers.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/usage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/usage/subscriptions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/usage/validation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-07-26 10:15:21.000000 gql-3.5.0b5/docs/usage/variables.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.698526 gql-3.5.0b5/gql/
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16695 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52066 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36033 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/dsl.py
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/gql.py
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.702527 gql-3.5.0b5/gql/transport/
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13451 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/transport/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7515 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/transport/appsync_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/transport/appsync_websockets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/transport/async_transport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/transport/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10440 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/transport/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/transport/local_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15179 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/transport/phoenix_channel_websockets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10853 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/transport/requests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/transport/transport.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19190 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/transport/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24466 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/transport/websockets_base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.702527 gql-3.5.0b5/gql/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3165 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/utilities/build_client_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3865 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/utilities/get_introspection_query_ast.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14304 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/utilities/parse_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4261 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/utilities/serialize_variable_values.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/utilities/update_schema_enum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2280 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/utilities/update_schema_scalars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-07-26 10:15:21.000000 gql-3.5.0b5/gql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.698526 gql-3.5.0b5/gql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-07-26 10:15:24.000000 gql-3.5.0b5/gql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-07-26 10:15:24.000000 gql-3.5.0b5/gql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 10:15:24.000000 gql-3.5.0b5/gql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-26 10:15:24.000000 gql-3.5.0b5/gql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 10:15:24.000000 gql-3.5.0b5/gql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-07-26 10:15:24.000000 gql-3.5.0b5/gql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-07-26 10:15:24.000000 gql-3.5.0b5/gql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-07-26 10:15:24.706527 gql-3.5.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-07-26 10:15:21.000000 gql-3.5.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.702527 gql-3.5.0b5/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15031 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.706527 gql-3.5.0b5/tests/custom_scalars/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/custom_scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6593 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/custom_scalars/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6960 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/custom_scalars/test_enum_colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5153 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/custom_scalars/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20717 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/custom_scalars/test_money.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/custom_scalars/test_parse_results.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.706527 gql-3.5.0b5/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.706527 gql-3.5.0b5/tests/fixtures/aws/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/fixtures/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/fixtures/aws/fake_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/fixtures/aws/fake_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/fixtures/aws/fake_session.py
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/fixtures/aws/fake_signer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.706527 gql-3.5.0b5/tests/fixtures/graphql/
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/fixtures/graphql/sample.graphql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.706527 gql-3.5.0b5/tests/fixtures/vcr_cassettes/
+-rw-r--r--   0 runner    (1001) docker     (122)     5340 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/fixtures/vcr_cassettes/client.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    78820 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/fixtures/vcr_cassettes/queries.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.706527 gql-3.5.0b5/tests/nested_input/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/nested_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/nested_input/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/nested_input/test_nested_input.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:24.706527 gql-3.5.0b5/tests/starwars/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/starwars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/starwars/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7990 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/starwars/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23843 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/starwars/test_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/starwars/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3587 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/starwars/test_parse_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7529 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/starwars/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/starwars/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5441 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/starwars/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43147 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3320 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_aiohttp_online.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6588 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_appsync_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_appsync_http.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23922 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_appsync_websockets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7303 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_async_client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12020 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7011 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7525 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_graphqlws_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27257 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_graphqlws_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_http_async_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26413 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38462 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_httpx_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3320 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_httpx_online.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_localhost.cnf
+-rw-r--r--   0 runner    (1001) docker     (122)     2908 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_localhost.pem
+-rw-r--r--   0 runner    (1001) docker     (122)    15131 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_phoenix_channel_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4079 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_phoenix_channel_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12704 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_phoenix_channel_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26692 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3517 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11402 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_websocket_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6236 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_websocket_online.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17431 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_websocket_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18656 2023-07-26 10:15:21.000000 gql-3.5.0b5/tests/test_websocket_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-07-26 10:15:21.000000 gql-3.5.0b5/tox.ini
```

### Comparing `gql-3.5.0b4/.readthedocs.yaml` & `gql-3.5.0b5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/CONTRIBUTING.md` & `gql-3.5.0b5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/LICENSE` & `gql-3.5.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/Makefile` & `gql-3.5.0b5/Makefile`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/PKG-INFO` & `gql-3.5.0b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gql
-Version: 3.5.0b4
+Version: 3.5.0b5
 Summary: GraphQL client for Python
 Home-page: https://github.com/graphql-python/gql
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Description: # GQL
         
@@ -51,15 +51,18 @@
         * [gql-cli script](https://gql.readthedocs.io/en/latest/gql-cli/intro.html) to execute GraphQL queries or download schemas from the command line
         * [DSL module](https://gql.readthedocs.io/en/latest/advanced/dsl_module.html) to compose GraphQL queries dynamically
         
         ## Installation
         
         You can install GQL with all the optional dependencies using pip:
         
-            pip install gql[all]
+        ```bash
+        # Quotes may be required on certain shells such as zsh.
+        pip install "gql[all]"
+        ```
         
         > **NOTE**: See also [the documentation](https://gql.readthedocs.io/en/latest/intro.html#less-dependencies) to install GQL with less extra dependencies depending on the transports you would like to use or for alternative installation methods.
         
         ## Usage
         
         ### Basic usage
```

### Comparing `gql-3.5.0b4/README.md` & `gql-3.5.0b5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,18 @@
 * [gql-cli script](https://gql.readthedocs.io/en/latest/gql-cli/intro.html) to execute GraphQL queries or download schemas from the command line
 * [DSL module](https://gql.readthedocs.io/en/latest/advanced/dsl_module.html) to compose GraphQL queries dynamically
 
 ## Installation
 
 You can install GQL with all the optional dependencies using pip:
 
-    pip install gql[all]
+```bash
+# Quotes may be required on certain shells such as zsh.
+pip install "gql[all]"
+```
 
 > **NOTE**: See also [the documentation](https://gql.readthedocs.io/en/latest/intro.html#less-dependencies) to install GQL with less extra dependencies depending on the transports you would like to use or for alternative installation methods.
 
 ## Usage
 
 ### Basic usage
```

### Comparing `gql-3.5.0b4/docs/Makefile` & `gql-3.5.0b5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/advanced/async_advanced_usage.rst` & `gql-3.5.0b5/docs/advanced/async_advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/advanced/async_permanent_session.rst` & `gql-3.5.0b5/docs/advanced/async_permanent_session.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/advanced/dsl_module.rst` & `gql-3.5.0b5/docs/advanced/dsl_module.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/advanced/error_handling.rst` & `gql-3.5.0b5/docs/advanced/error_handling.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/advanced/local_schema.rst` & `gql-3.5.0b5/docs/advanced/local_schema.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/advanced/logging.rst` & `gql-3.5.0b5/docs/advanced/logging.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/async/async_intro.rst` & `gql-3.5.0b5/docs/async/async_intro.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/async/async_usage.rst` & `gql-3.5.0b5/docs/async/async_usage.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/aiohttp_async.py` & `gql-3.5.0b5/docs/code_examples/aiohttp_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/aiohttp_async_dsl.py` & `gql-3.5.0b5/docs/code_examples/aiohttp_async_dsl.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/aiohttp_sync.py` & `gql-3.5.0b5/docs/code_examples/aiohttp_sync.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/appsync/mutation_api_key.py` & `gql-3.5.0b5/docs/code_examples/appsync/mutation_api_key.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/appsync/mutation_iam.py` & `gql-3.5.0b5/docs/code_examples/appsync/mutation_iam.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/appsync/subscription_api_key.py` & `gql-3.5.0b5/docs/code_examples/appsync/subscription_api_key.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/appsync/subscription_iam.py` & `gql-3.5.0b5/docs/code_examples/appsync/subscription_iam.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/console_async.py` & `gql-3.5.0b5/docs/code_examples/console_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/fastapi_async.py` & `gql-3.5.0b5/docs/code_examples/fastapi_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/httpx_async.py` & `gql-3.5.0b5/docs/code_examples/httpx_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/phoenix_channel_async.py` & `gql-3.5.0b5/docs/code_examples/phoenix_channel_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/reconnecting_mutation_http.py` & `gql-3.5.0b5/docs/code_examples/reconnecting_mutation_http.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/reconnecting_mutation_ws.py` & `gql-3.5.0b5/docs/code_examples/reconnecting_mutation_ws.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/reconnecting_subscription.py` & `gql-3.5.0b5/docs/code_examples/reconnecting_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/requests_sync_dsl.py` & `gql-3.5.0b5/docs/code_examples/requests_sync_dsl.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/code_examples/websockets_async.py` & `gql-3.5.0b5/docs/code_examples/websockets_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/conf.py` & `gql-3.5.0b5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/gql-cli/intro.rst` & `gql-3.5.0b5/docs/gql-cli/intro.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/intro.rst` & `gql-3.5.0b5/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/make.bat` & `gql-3.5.0b5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/transports/aiohttp.rst` & `gql-3.5.0b5/docs/transports/aiohttp.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/transports/appsync.rst` & `gql-3.5.0b5/docs/transports/appsync.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/transports/httpx_async.rst` & `gql-3.5.0b5/docs/transports/httpx_async.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/transports/phoenix.rst` & `gql-3.5.0b5/docs/transports/phoenix.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/transports/websockets.rst` & `gql-3.5.0b5/docs/transports/websockets.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/usage/basic_usage.rst` & `gql-3.5.0b5/docs/usage/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/usage/custom_scalars_and_enums.rst` & `gql-3.5.0b5/docs/usage/custom_scalars_and_enums.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/usage/extensions.rst` & `gql-3.5.0b5/docs/usage/extensions.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/usage/file_upload.rst` & `gql-3.5.0b5/docs/usage/file_upload.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/usage/subscriptions.rst` & `gql-3.5.0b5/docs/usage/subscriptions.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/usage/validation.rst` & `gql-3.5.0b5/docs/usage/validation.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/docs/usage/variables.rst` & `gql-3.5.0b5/docs/usage/variables.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/cli.py` & `gql-3.5.0b5/gql/cli.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/client.py` & `gql-3.5.0b5/gql/client.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/dsl.py` & `gql-3.5.0b5/gql/dsl.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/gql.py` & `gql-3.5.0b5/gql/gql.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/transport/aiohttp.py` & `gql-3.5.0b5/gql/transport/aiohttp.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/transport/appsync_auth.py` & `gql-3.5.0b5/gql/transport/appsync_auth.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/transport/appsync_websockets.py` & `gql-3.5.0b5/gql/transport/appsync_websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/transport/async_transport.py` & `gql-3.5.0b5/gql/transport/async_transport.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/transport/exceptions.py` & `gql-3.5.0b5/gql/transport/exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/transport/httpx.py` & `gql-3.5.0b5/gql/transport/httpx.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/transport/local_schema.py` & `gql-3.5.0b5/gql/transport/local_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         **kwargs,
     ) -> AsyncGenerator[ExecutionResult, None]:
         """Send a subscription and receive the results using an async generator
 
         The results are sent as an ExecutionResult object
         """
 
-        subscribe_result = await subscribe(self.schema, document, *args, **kwargs)
+        subscribe_result = subscribe(self.schema, document, *args, **kwargs)
 
         if isinstance(subscribe_result, ExecutionResult):
             yield subscribe_result
 
         else:
             async for result in subscribe_result:
                 yield result
```

### Comparing `gql-3.5.0b4/gql/transport/phoenix_channel_websockets.py` & `gql-3.5.0b5/gql/transport/phoenix_channel_websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/transport/requests.py` & `gql-3.5.0b5/gql/transport/requests.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import io
 import json
 import logging
-from typing import Any, Dict, Optional, Tuple, Type, Union
+from typing import Any, Collection, Dict, Optional, Tuple, Type, Union
 
 import requests
 from graphql import DocumentNode, ExecutionResult, print_ast
 from requests.adapters import HTTPAdapter, Retry
 from requests.auth import AuthBase
 from requests.cookies import RequestsCookieJar
 from requests_toolbelt.multipart.encoder import MultipartEncoder
@@ -27,26 +27,29 @@
     """:ref:`Sync Transport <sync_transports>` used to execute GraphQL queries
     on remote servers.
 
     The transport uses the requests library to send HTTP POST requests.
     """
 
     file_classes: Tuple[Type[Any], ...] = (io.IOBase,)
+    _default_retry_codes = (429, 500, 502, 503, 504)
 
     def __init__(
         self,
         url: str,
         headers: Optional[Dict[str, Any]] = None,
         cookies: Optional[Union[Dict[str, Any], RequestsCookieJar]] = None,
         auth: Optional[AuthBase] = None,
         use_json: bool = True,
         timeout: Optional[int] = None,
         verify: Union[bool, str] = True,
         retries: int = 0,
         method: str = "POST",
+        retry_backoff_factor: float = 0.1,
+        retry_status_forcelist: Collection[int] = _default_retry_codes,
         **kwargs: Any,
     ):
         """Initialize the transport with the given request parameters.
 
         :param url: The GraphQL server URL.
         :param headers: Dictionary of HTTP Headers to send with the :class:`Request`
             (Default: None).
@@ -58,14 +61,21 @@
             (Default: True).
         :param timeout: Specifies a default timeout for requests (Default: None).
         :param verify: Either a boolean, in which case it controls whether we verify
             the server's TLS certificate, or a string, in which case it must be a path
             to a CA bundle to use. (Default: True).
         :param retries: Pre-setup of the requests' Session for performing retries
         :param method: HTTP method used for requests. (Default: POST).
+        :param retry_backoff_factor: A backoff factor to apply between attempts after
+            the second try. urllib3 will sleep for:
+            {backoff factor} * (2 ** ({number of previous retries}))
+        :param retry_status_forcelist: A set of integer HTTP status codes that we
+            should force a retry on. A retry is initiated if the request method is
+            in allowed_methods and the response status code is in status_forcelist.
+            (Default: [429, 500, 502, 503, 504])
         :param kwargs: Optional arguments that ``request`` takes.
             These can be seen at the `requests`_ source code or the official `docs`_
 
         .. _requests: https://github.com/psf/requests/blob/master/requests/api.py
         .. _docs: https://requests.readthedocs.io/en/master/
         """
         self.url = url
@@ -73,14 +83,16 @@
         self.cookies = cookies
         self.auth = auth
         self.use_json = use_json
         self.default_timeout = timeout
         self.verify = verify
         self.retries = retries
         self.method = method
+        self.retry_backoff_factor = retry_backoff_factor
+        self.retry_status_forcelist = retry_status_forcelist
         self.kwargs = kwargs
 
         self.session = None
 
         self.response_headers = None
 
     def connect(self):
@@ -91,16 +103,16 @@
             self.session = requests.Session()
 
             # If we specified some retries, we provide a predefined retry-logic
             if self.retries > 0:
                 adapter = HTTPAdapter(
                     max_retries=Retry(
                         total=self.retries,
-                        backoff_factor=0.1,
-                        status_forcelist=[500, 502, 503, 504],
+                        backoff_factor=self.retry_backoff_factor,
+                        status_forcelist=self.retry_status_forcelist,
                         allowed_methods=None,
                     )
                 )
                 for prefix in "http://", "https://":
                     self.session.mount(prefix, adapter)
         else:
             raise TransportAlreadyConnected("Transport is already connected")
```

### Comparing `gql-3.5.0b4/gql/transport/transport.py` & `gql-3.5.0b5/gql/transport/transport.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/transport/websockets.py` & `gql-3.5.0b5/gql/transport/websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/transport/websockets_base.py` & `gql-3.5.0b5/gql/transport/websockets_base.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/utilities/__init__.py` & `gql-3.5.0b5/gql/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/utilities/build_client_schema.py` & `gql-3.5.0b5/gql/utilities/build_client_schema.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/utilities/get_introspection_query_ast.py` & `gql-3.5.0b5/gql/utilities/get_introspection_query_ast.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/utilities/parse_result.py` & `gql-3.5.0b5/gql/utilities/parse_result.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/utilities/serialize_variable_values.py` & `gql-3.5.0b5/gql/utilities/serialize_variable_values.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/utilities/update_schema_enum.py` & `gql-3.5.0b5/gql/utilities/update_schema_enum.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/utilities/update_schema_scalars.py` & `gql-3.5.0b5/gql/utilities/update_schema_scalars.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql/utils.py` & `gql-3.5.0b5/gql/utils.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql.egg-info/PKG-INFO` & `gql-3.5.0b5/gql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gql
-Version: 3.5.0b4
+Version: 3.5.0b5
 Summary: GraphQL client for Python
 Home-page: https://github.com/graphql-python/gql
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Description: # GQL
         
@@ -51,15 +51,18 @@
         * [gql-cli script](https://gql.readthedocs.io/en/latest/gql-cli/intro.html) to execute GraphQL queries or download schemas from the command line
         * [DSL module](https://gql.readthedocs.io/en/latest/advanced/dsl_module.html) to compose GraphQL queries dynamically
         
         ## Installation
         
         You can install GQL with all the optional dependencies using pip:
         
-            pip install gql[all]
+        ```bash
+        # Quotes may be required on certain shells such as zsh.
+        pip install "gql[all]"
+        ```
         
         > **NOTE**: See also [the documentation](https://gql.readthedocs.io/en/latest/intro.html#less-dependencies) to install GQL with less extra dependencies depending on the transports you would like to use or for alternative installation methods.
         
         ## Usage
         
         ### Basic usage
```

### Comparing `gql-3.5.0b4/gql.egg-info/SOURCES.txt` & `gql-3.5.0b5/gql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/gql.egg-info/requires.txt` & `gql-3.5.0b5/gql.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-graphql-core<3.4,>=3.3.0a2
+graphql-core<3.4,>=3.3.0a3
 yarl<2.0,>=1.6
 backoff<3.0,>=1.11.1
 
 [aiohttp]
-aiohttp<3.9.0,>=3.8.0
+aiohttp<4,>=3.8.0
 
 [all]
-aiohttp<3.9.0,>=3.8.0
+aiohttp<4,>=3.8.0
 requests<3,>=2.26
 requests_toolbelt<1,>=0.9.1
 urllib3<2,>=1.26
 httpx<1,>=0.23.1
-websockets<11,>=10
+websockets<12,>=10
 botocore<2,>=1.21
 
 [botocore]
 botocore<2,>=1.21
 
 [dev]
-aiohttp<3.9.0,>=3.8.0
+aiohttp<4,>=3.8.0
 requests<3,>=2.26
 requests_toolbelt<1,>=0.9.1
 urllib3<2,>=1.26
 httpx<1,>=0.23.1
-websockets<11,>=10
+websockets<12,>=10
 botocore<2,>=1.21
 black==22.3.0
 check-manifest<1,>=0.42
 flake8==3.8.1
 isort==4.3.21
 mypy==0.910
 sphinx<6,>=5.3.0
@@ -50,20 +50,20 @@
 
 [requests]
 requests<3,>=2.26
 requests_toolbelt<1,>=0.9.1
 urllib3<2,>=1.26
 
 [test]
-aiohttp<3.9.0,>=3.8.0
+aiohttp<4,>=3.8.0
 requests<3,>=2.26
 requests_toolbelt<1,>=0.9.1
 urllib3<2,>=1.26
 httpx<1,>=0.23.1
-websockets<11,>=10
+websockets<12,>=10
 botocore<2,>=1.21
 parse==1.15.0
 pytest==6.2.5
 pytest-asyncio==0.16.0
 pytest-console-scripts==1.3.1
 pytest-cov==3.0.0
 mock==4.0.2
@@ -77,8 +77,8 @@
 pytest-console-scripts==1.3.1
 pytest-cov==3.0.0
 mock==4.0.2
 vcrpy==4.0.2
 aiofiles
 
 [websockets]
-websockets<11,>=10
+websockets<12,>=10
```

### Comparing `gql-3.5.0b4/setup.py` & `gql-3.5.0b5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from setuptools import setup, find_packages
 
 install_requires = [
-    "graphql-core>=3.3.0a2,<3.4",
+    "graphql-core>=3.3.0a3,<3.4",
     "yarl>=1.6,<2.0",
     "backoff>=1.11.1,<3.0",
 ]
 
 console_scripts = [
     "gql-cli=gql.cli:gql_cli",
 ]
@@ -34,29 +34,29 @@
     "sphinx-argparse==0.2.5",
     "types-aiofiles",
     "types-mock",
     "types-requests",
 ] + tests_requires
 
 install_aiohttp_requires = [
-    "aiohttp>=3.8.0,<3.9.0",
+    "aiohttp>=3.8.0,<4",
 ]
 
 install_requests_requires = [
     "requests>=2.26,<3",
     "requests_toolbelt>=0.9.1,<1",
     "urllib3>=1.26,<2",
 ]
 
 install_httpx_requires = [
     "httpx>=0.23.1,<1",
 ]
 
 install_websockets_requires = [
-    "websockets>=10,<11",
+    "websockets>=10,<12",
 ]
 
 install_botocore_requires = [
     "botocore>=1.21,<2",
 ]
 
 install_all_requires = (
```

### Comparing `gql-3.5.0b4/tests/conftest.py` & `gql-3.5.0b5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/custom_scalars/test_datetime.py` & `gql-3.5.0b5/tests/custom_scalars/test_datetime.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/custom_scalars/test_enum_colors.py` & `gql-3.5.0b5/tests/custom_scalars/test_enum_colors.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/custom_scalars/test_json.py` & `gql-3.5.0b5/tests/custom_scalars/test_json.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/custom_scalars/test_money.py` & `gql-3.5.0b5/tests/custom_scalars/test_money.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/custom_scalars/test_parse_results.py` & `gql-3.5.0b5/tests/custom_scalars/test_parse_results.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/fixtures/aws/fake_credentials.py` & `gql-3.5.0b5/tests/fixtures/aws/fake_credentials.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/fixtures/aws/fake_request.py` & `gql-3.5.0b5/tests/fixtures/aws/fake_request.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/fixtures/aws/fake_session.py` & `gql-3.5.0b5/tests/fixtures/aws/fake_session.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/fixtures/aws/fake_signer.py` & `gql-3.5.0b5/tests/fixtures/aws/fake_signer.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/fixtures/vcr_cassettes/client.yaml` & `gql-3.5.0b5/tests/fixtures/vcr_cassettes/client.yaml`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/fixtures/vcr_cassettes/queries.yaml` & `gql-3.5.0b5/tests/fixtures/vcr_cassettes/queries.yaml`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/nested_input/schema.py` & `gql-3.5.0b5/tests/nested_input/schema.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/nested_input/test_nested_input.py` & `gql-3.5.0b5/tests/nested_input/test_nested_input.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/starwars/fixtures.py` & `gql-3.5.0b5/tests/starwars/fixtures.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/starwars/schema.py` & `gql-3.5.0b5/tests/starwars/schema.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/starwars/test_dsl.py` & `gql-3.5.0b5/tests/starwars/test_dsl.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/starwars/test_introspection.py` & `gql-3.5.0b5/tests/starwars/test_introspection.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/starwars/test_parse_results.py` & `gql-3.5.0b5/tests/starwars/test_parse_results.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/starwars/test_query.py` & `gql-3.5.0b5/tests/starwars/test_query.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/starwars/test_subscription.py` & `gql-3.5.0b5/tests/starwars/test_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     ]
 
     subs = gql(subscription_str)
 
     params = {"ep": "JEDI"}
     expected = [{**review, "episode": "JEDI"} for review in reviews[6]]
 
-    ai = await subscribe(StarWarsSchema, subs, variable_values=params)
+    ai = subscribe(StarWarsSchema, subs, variable_values=params)
 
     result = [result.data["reviewAdded"] async for result in ai]
 
     assert result == expected
 
 
 @pytest.mark.asyncio
```

### Comparing `gql-3.5.0b4/tests/starwars/test_validation.py` & `gql-3.5.0b5/tests/starwars/test_validation.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_aiohttp.py` & `gql-3.5.0b5/tests/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_aiohttp_online.py` & `gql-3.5.0b5/tests/test_aiohttp_online.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_appsync_auth.py` & `gql-3.5.0b5/tests/test_appsync_auth.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_appsync_http.py` & `gql-3.5.0b5/tests/test_appsync_http.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_appsync_websockets.py` & `gql-3.5.0b5/tests/test_appsync_websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_async_client_validation.py` & `gql-3.5.0b5/tests/test_async_client_validation.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_cli.py` & `gql-3.5.0b5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_client.py` & `gql-3.5.0b5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_graphqlws_exceptions.py` & `gql-3.5.0b5/tests/test_graphqlws_exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_graphqlws_subscription.py` & `gql-3.5.0b5/tests/test_graphqlws_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_http_async_sync.py` & `gql-3.5.0b5/tests/test_http_async_sync.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_httpx.py` & `gql-3.5.0b5/tests/test_httpx.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_httpx_async.py` & `gql-3.5.0b5/tests/test_httpx_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_httpx_online.py` & `gql-3.5.0b5/tests/test_httpx_online.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_localhost.pem` & `gql-3.5.0b5/tests/test_localhost.pem`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_phoenix_channel_exceptions.py` & `gql-3.5.0b5/tests/test_phoenix_channel_exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_phoenix_channel_query.py` & `gql-3.5.0b5/tests/test_phoenix_channel_query.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_phoenix_channel_subscription.py` & `gql-3.5.0b5/tests/test_phoenix_channel_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_requests.py` & `gql-3.5.0b5/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_transport.py` & `gql-3.5.0b5/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_websocket_exceptions.py` & `gql-3.5.0b5/tests/test_websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_websocket_online.py` & `gql-3.5.0b5/tests/test_websocket_online.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_websocket_query.py` & `gql-3.5.0b5/tests/test_websocket_query.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tests/test_websocket_subscription.py` & `gql-3.5.0b5/tests/test_websocket_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b4/tox.ini` & `gql-3.5.0b5/tox.ini`

 * *Files identical despite different names*

