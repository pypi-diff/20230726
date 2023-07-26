# Comparing `tmp/dagshub-0.3.0.post3.tar.gz` & `tmp/dagshub-0.3.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagshub-0.3.0.post3.tar", last modified: Mon Jul 24 13:01:32 2023, max compression
+gzip compressed data, was "dagshub-0.3.0.post4.tar", last modified: Wed Jul 26 12:44:52 2023, max compression
```

## Comparing `dagshub-0.3.0.post3.tar` & `dagshub-0.3.0.post4.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.766531 dagshub-0.3.0.post3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-24 13:01:32.766531 dagshub-0.3.0.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.746530 dagshub-0.3.0.post3/dagshub/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.750530 dagshub-0.3.0.post3/dagshub/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/auth/token_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/auth/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.754531 dagshub-0.3.0.post3/dagshub/common/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.754531 dagshub-0.3.0.post3/dagshub/common/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11849 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/api/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/api/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/rich_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/common/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.754531 dagshub-0.3.0.post3/dagshub/data_engine/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.754531 dagshub-0.3.0.post3/dagshub/data_engine/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/annotation/voxel_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.758531 dagshub-0.3.0.post3/dagshub/data_engine/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/data_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.758531 dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.758531 dagshub-0.3.0.post3/dagshub/data_engine/client/query_builder/
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/client/query_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/datasources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/data_engine/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/model/datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    25813 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/model/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/model/datasource_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/model/query_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.742530 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    42241 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/
--rw-r--r--   0 runner    (1001) docker     (123)   180750 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/fiftyone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/voxel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/fastai/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/fastai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/fastai/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/keras/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/keras/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/notebook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.762531 dagshub-0.3.0.post3/dagshub/pytorch_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/pytorch_lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/pytorch_lightning/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/pytorch_lightning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.766531 dagshub-0.3.0.post3/dagshub/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/streaming/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/streaming/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    39148 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/streaming/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/streaming/mount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.766531 dagshub-0.3.0.post3/dagshub/upload/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/upload/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    22616 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/dagshub/upload/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.750530 dagshub-0.3.0.post3/dagshub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-07-24 13:01:32.000000 dagshub-0.3.0.post3/dagshub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-24 13:01:32.000000 dagshub-0.3.0.post3/dagshub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:01:32.000000 dagshub-0.3.0.post3/dagshub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 13:01:32.000000 dagshub-0.3.0.post3/dagshub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-24 13:01:32.000000 dagshub-0.3.0.post3/dagshub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 13:01:32.000000 dagshub-0.3.0.post3/dagshub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:01:32.766531 dagshub-0.3.0.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:01:32.766531 dagshub-0.3.0.post3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/tests/test_dagshub_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-24 13:01:11.000000 dagshub-0.3.0.post3/tests/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.552173 dagshub-0.3.0.post4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-26 12:44:52.552173 dagshub-0.3.0.post4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.528173 dagshub-0.3.0.post4/dagshub/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.532173 dagshub-0.3.0.post4/dagshub/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/auth/token_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/auth/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.532173 dagshub-0.3.0.post4/dagshub/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.532173 dagshub-0.3.0.post4/dagshub/common/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/api/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/api/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/rich_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/common/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.532173 dagshub-0.3.0.post4/dagshub/data_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.536173 dagshub-0.3.0.post4/dagshub/data_engine/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/annotation/voxel_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.536173 dagshub-0.3.0.post4/dagshub/data_engine/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/data_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.536173 dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.536173 dagshub-0.3.0.post4/dagshub/data_engine/client/query_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/client/query_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/datasources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.540173 dagshub-0.3.0.post4/dagshub/data_engine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/model/datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26149 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/model/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/model/datasource_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/model/query_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.540173 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.524173 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.540173 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.540173 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    42241 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.540173 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)   180750 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/fiftyone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.544173 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/voxel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.544173 dagshub-0.3.0.post4/dagshub/fastai/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/fastai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/fastai/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.544173 dagshub-0.3.0.post4/dagshub/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/keras/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.544173 dagshub-0.3.0.post4/dagshub/pytorch_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/pytorch_lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/pytorch_lightning/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/pytorch_lightning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.548173 dagshub-0.3.0.post4/dagshub/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/streaming/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/streaming/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39148 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/streaming/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/streaming/mount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.552173 dagshub-0.3.0.post4/dagshub/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/upload/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25355 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/dagshub/upload/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.528173 dagshub-0.3.0.post4/dagshub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-26 12:44:52.000000 dagshub-0.3.0.post4/dagshub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-26 12:44:52.000000 dagshub-0.3.0.post4/dagshub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:44:52.000000 dagshub-0.3.0.post4/dagshub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-26 12:44:52.000000 dagshub-0.3.0.post4/dagshub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-26 12:44:52.000000 dagshub-0.3.0.post4/dagshub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 12:44:52.000000 dagshub-0.3.0.post4/dagshub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:44:52.552173 dagshub-0.3.0.post4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:44:52.552173 dagshub-0.3.0.post4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/tests/test_dagshub_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-26 12:44:34.000000 dagshub-0.3.0.post4/tests/test_misc.py
```

### Comparing `dagshub-0.3.0.post3/LICENSE` & `dagshub-0.3.0.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/PKG-INFO` & `dagshub-0.3.0.post4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagshub
-Version: 0.3.0.post3
+Version: 0.3.0.post4
 Summary: DagsHub client libraries
 Home-page: https://github.com/DagsHub/client
 Author: DagsHub
 Author-email: contact@dagshub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,14 +53,15 @@
 
 For more details on the different functions of the client, check out the docs segments:
 1. [Installation & Setup](https://github.com/DagsHub/client/blob/master/docs/index.md#installation-and-setup)
 2. [Data Streaming](https://github.com/DagsHub/client/blob/master/docs/index.md#data-streaming)
 3. [Data Upload](https://github.com/DagsHub/client/blob/master/docs/index.md#data-upload)
 4. [Experiment Tracking](https://github.com/DagsHub/client/blob/master/docs/index.md#experiment-tracking-logger)
     1. [Autologging](https://github.com/DagsHub/client/blob/master/docs/index.md#autologging-integrations-with-ml-frameworks)
+5. [Data Engine](https://github.com/DagsHub/client/blob/master/docs/data_engine.md)
 
 Some functionality is supported only in Python.
 
 To read about some of the awesome use cases for Direct Data Access, check out
 the [relevant doc page](https://dagshub.com/docs/feature_guide/direct_data_access/#use-cases).
 
 ## Installation
@@ -90,8 +91,13 @@
 
 ## Next Steps
 You can dive into the expanded [documentation](docs/index.md), to learn more about data streaming, data upload and
 experiment tracking with DagsHub
 
 ---
 
+
+### Analytics
+To improve your experience, we collect analytics on client usage. If you want to disable analytics collection,
+set the `DAGSHUB_DISABLE_ANALYTICS` environment variable to any value.
+
 Made with 🐶 by [DagsHub](https://dagshub.com/).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dagshub Version: 0.3.0.post3 Summary: DagsHub
+Metadata-Version: 2.1 Name: dagshub Version: 0.3.0.post4 Summary: DagsHub
 client libraries Home-page: https://github.com/DagsHub/client Author: DagsHub
 Author-email: contact@dagshub.com Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE [![DagsHub Client](https://github.com/DagsHub/
 client/raw/master/dagshub_github.png)](https://dagshub.com)
    **** ð Launching Streaming and Upload of DVC versioned Data ð ****
@@ -48,16 +48,17 @@
 client, check out the docs segments: 1. [Installation & Setup](https://
 github.com/DagsHub/client/blob/master/docs/index.md#installation-and-setup) 2.
 [Data Streaming](https://github.com/DagsHub/client/blob/master/docs/
 index.md#data-streaming) 3. [Data Upload](https://github.com/DagsHub/client/
 blob/master/docs/index.md#data-upload) 4. [Experiment Tracking](https://
 github.com/DagsHub/client/blob/master/docs/index.md#experiment-tracking-logger)
 1. [Autologging](https://github.com/DagsHub/client/blob/master/docs/
-index.md#autologging-integrations-with-ml-frameworks) Some functionality is
-supported only in Python. To read about some of the awesome use cases for
+index.md#autologging-integrations-with-ml-frameworks) 5. [Data Engine](https://
+github.com/DagsHub/client/blob/master/docs/data_engine.md) Some functionality
+is supported only in Python. To read about some of the awesome use cases for
 Direct Data Access, check out the [relevant doc page](https://dagshub.com/docs/
 feature_guide/direct_data_access/#use-cases). ## Installation ```bash pip
 install dagshub ``` Direct Data Access (DDA) functionality requires
 authentication, which you can easily do by running the following command in
 your terminal: ```bash dagshub login ``` ## Quickstart for Data Streaming The
 easiest way to start using DagsHub is via the Python Hooks method. To do this:
 1. Your DagsHub project, 2. Copy the following 2 lines of code into your Python
@@ -65,8 +66,11 @@
 install_hooks install_hooks() ``` 3. Thatâs it! You now have streaming access
 to all your project files. **ð¤© Check out this colab to see an example of
 this Data Streaming work end to end:** [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1CtBmcDtZnxZKVIhNvPagX-8UFWHZ5HAg?usp=sharing)
 ## Next Steps You can dive into the expanded [documentation](docs/index.md), to
 learn more about data streaming, data upload and experiment tracking with
-DagsHub --- Made with ð¶ by [DagsHub](https://dagshub.com/).
+DagsHub --- ### Analytics To improve your experience, we collect analytics on
+client usage. If you want to disable analytics collection, set the
+`DAGSHUB_DISABLE_ANALYTICS` environment variable to any value. Made with ð¶
+by [DagsHub](https://dagshub.com/).
```

### Comparing `dagshub-0.3.0.post3/README.md` & `dagshub-0.3.0.post4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 For more details on the different functions of the client, check out the docs segments:
 1. [Installation & Setup](https://github.com/DagsHub/client/blob/master/docs/index.md#installation-and-setup)
 2. [Data Streaming](https://github.com/DagsHub/client/blob/master/docs/index.md#data-streaming)
 3. [Data Upload](https://github.com/DagsHub/client/blob/master/docs/index.md#data-upload)
 4. [Experiment Tracking](https://github.com/DagsHub/client/blob/master/docs/index.md#experiment-tracking-logger)
     1. [Autologging](https://github.com/DagsHub/client/blob/master/docs/index.md#autologging-integrations-with-ml-frameworks)
+5. [Data Engine](https://github.com/DagsHub/client/blob/master/docs/data_engine.md)
 
 Some functionality is supported only in Python.
 
 To read about some of the awesome use cases for Direct Data Access, check out
 the [relevant doc page](https://dagshub.com/docs/feature_guide/direct_data_access/#use-cases).
 
 ## Installation
@@ -76,8 +77,13 @@
 
 ## Next Steps
 You can dive into the expanded [documentation](docs/index.md), to learn more about data streaming, data upload and
 experiment tracking with DagsHub
 
 ---
 
+
+### Analytics
+To improve your experience, we collect analytics on client usage. If you want to disable analytics collection,
+set the `DAGSHUB_DISABLE_ANALYTICS` environment variable to any value.
+
 Made with 🐶 by [DagsHub](https://dagshub.com/).
```

#### html2text {}

```diff
@@ -43,16 +43,17 @@
 client, check out the docs segments: 1. [Installation & Setup](https://
 github.com/DagsHub/client/blob/master/docs/index.md#installation-and-setup) 2.
 [Data Streaming](https://github.com/DagsHub/client/blob/master/docs/
 index.md#data-streaming) 3. [Data Upload](https://github.com/DagsHub/client/
 blob/master/docs/index.md#data-upload) 4. [Experiment Tracking](https://
 github.com/DagsHub/client/blob/master/docs/index.md#experiment-tracking-logger)
 1. [Autologging](https://github.com/DagsHub/client/blob/master/docs/
-index.md#autologging-integrations-with-ml-frameworks) Some functionality is
-supported only in Python. To read about some of the awesome use cases for
+index.md#autologging-integrations-with-ml-frameworks) 5. [Data Engine](https://
+github.com/DagsHub/client/blob/master/docs/data_engine.md) Some functionality
+is supported only in Python. To read about some of the awesome use cases for
 Direct Data Access, check out the [relevant doc page](https://dagshub.com/docs/
 feature_guide/direct_data_access/#use-cases). ## Installation ```bash pip
 install dagshub ``` Direct Data Access (DDA) functionality requires
 authentication, which you can easily do by running the following command in
 your terminal: ```bash dagshub login ``` ## Quickstart for Data Streaming The
 easiest way to start using DagsHub is via the Python Hooks method. To do this:
 1. Your DagsHub project, 2. Copy the following 2 lines of code into your Python
@@ -60,8 +61,11 @@
 install_hooks install_hooks() ``` 3. Thatâs it! You now have streaming access
 to all your project files. **ð¤© Check out this colab to see an example of
 this Data Streaming work end to end:** [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1CtBmcDtZnxZKVIhNvPagX-8UFWHZ5HAg?usp=sharing)
 ## Next Steps You can dive into the expanded [documentation](docs/index.md), to
 learn more about data streaming, data upload and experiment tracking with
-DagsHub --- Made with ð¶ by [DagsHub](https://dagshub.com/).
+DagsHub --- ### Analytics To improve your experience, we collect analytics on
+client usage. If you want to disable analytics collection, set the
+`DAGSHUB_DISABLE_ANALYTICS` environment variable to any value. Made with ð¶
+by [DagsHub](https://dagshub.com/).
```

### Comparing `dagshub-0.3.0.post3/dagshub/auth/oauth.py` & `dagshub-0.3.0.post4/dagshub/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/auth/token_auth.py` & `dagshub-0.3.0.post4/dagshub/auth/token_auth.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/auth/tokens.py` & `dagshub-0.3.0.post4/dagshub/auth/tokens.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/common/analytics.py` & `dagshub-0.3.0.post4/dagshub/common/analytics.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,17 +15,17 @@
         event_data = {}
     event_data["event"] = event_name
     if repo is not None:
         if type(repo) is int:
             event_data["repo_id"] = repo
         else:
             event_data["repo_id"] = repo.id
-    t = Thread(target=_send, args=(event_data,), daemon=True)
+    host = config.host
+    token = config.token or get_token(host=host)
+    t = Thread(target=_send, args=(event_data, host, token), daemon=True)
     t.start()
 
 
-def _send(event_data: Dict[str, Any]):
-    host = config.host
-    token = config.token or get_token(host=host)
+def _send(event_data: Dict[str, Any], host: str, token: str):
     url = f"{host}/api/internal/trackAnalyticsEvent"
 
     http_request("POST", url, data=event_data, auth=HTTPBearerAuth(token))
```

### Comparing `dagshub-0.3.0.post3/dagshub/common/api/repo.py` & `dagshub-0.3.0.post4/dagshub/common/api/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,14 +223,18 @@
     def default_branch(self) -> str:
         return self.get_repo_info().default_branch
 
     @cached_property
     def id(self) -> int:
         return self.get_repo_info().id
 
+    @cached_property
+    def is_mirror(self) -> bool:
+        return self.get_repo_info().mirror
+
     @property
     def full_name(self) -> str:
         return f"{self.owner}/{self.repo_name}"
 
     def last_commit(self, branch: Optional[str] = None) -> CommitAPIResponse:
         if branch is None:
             branch = self.default_branch
```

### Comparing `dagshub-0.3.0.post3/dagshub/common/api/responses.py` & `dagshub-0.3.0.post4/dagshub/common/api/responses.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/common/cli.py` & `dagshub-0.3.0.post4/dagshub/common/cli.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/common/config.py` & `dagshub-0.3.0.post4/dagshub/common/config.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/common/download.py` & `dagshub-0.3.0.post4/dagshub/common/download.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/common/helpers.py` & `dagshub-0.3.0.post4/dagshub/common/helpers.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/common/init.py` & `dagshub-0.3.0.post4/dagshub/common/init.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                                Please run this command in a git repository.')
 
     if url and (repo_name or repo_owner):
         repo_name, repo_owner = None, None
 
     if not url:
         if repo_name is not None and repo_owner is not None:
-            url = urllib.parse.urljoin(host, f'{repo_owner}/{repo_name}')
+            url = urllib.parse.urljoin(f'{host}/', f'{repo_owner}/{repo_name}')
         elif dvc:
             for remote in git.Repo(root).remotes:
                 if host in remote.url:
                     url = remote.url[:-4]
     if not url:
         raise ValueError('No host remote found! Please specify the remote using the url variable, or --url argument.')
     elif url[-4] == '.':
@@ -65,15 +65,15 @@
                           to the repository with --url or a pair of --repo-owner and --repo-name')
 
     # Setup authentication
     token = config.token or get_token(host=host)
     bearer = HTTPBearerAuth(token)
 
     # Configure repository
-    res = http_request("GET", urllib.parse.urljoin(host, config.REPO_INFO_URL.format(
+    res = http_request("GET", urllib.parse.urljoin(f'{host}/', config.REPO_INFO_URL.format(
         owner=repo_owner,
         reponame=repo_name)), auth=bearer)
     if res.status_code == 404:
         create_repo(repo_name)
 
     # Configure MLFlow
     if mlflow:
```

### Comparing `dagshub-0.3.0.post3/dagshub/common/logging_util.py` & `dagshub-0.3.0.post4/dagshub/common/logging_util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/common/util.py` & `dagshub-0.3.0.post4/dagshub/common/util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/annotation/voxel_conversion.py` & `dagshub-0.3.0.post4/dagshub/data_engine/annotation/voxel_conversion.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/client/data_client.py` & `dagshub-0.3.0.post4/dagshub/data_engine/client/data_client.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/client/gql_mutations.py` & `dagshub-0.3.0.post4/dagshub/data_engine/client/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/client/gql_queries.py` & `dagshub-0.3.0.post4/dagshub/data_engine/client/gql_queries.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/base.py` & `dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/base.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/tf.py` & `dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/tf.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/client/loaders/torch.py` & `dagshub-0.3.0.post4/dagshub/data_engine/client/loaders/torch.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/client/models.py` & `dagshub-0.3.0.post4/dagshub/data_engine/client/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,14 +55,17 @@
     valueType: MetadataFieldType = field(
         metadata=config(
             encoder=lambda val: val.value
         )
     )
     multiple: bool
 
+    def __repr__(self):
+        return f"{self.name} ({self.valueType.value})"
+
 
 @dataclass
 class DatasourceResult:
     id: Union[str, int]
     name: str
     rootUrl: str
     integrationStatus: IntegrationStatus
```

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/client/query_builder/__init__.py` & `dagshub-0.3.0.post4/dagshub/data_engine/client/query_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/datasets.py` & `dagshub-0.3.0.post4/dagshub/data_engine/datasets.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/datasources.py` & `dagshub-0.3.0.post4/dagshub/data_engine/datasources.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/model/datapoint.py` & `dagshub-0.3.0.post4/dagshub/data_engine/model/datapoint.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/model/datasource.py` & `dagshub-0.3.0.post4/dagshub/data_engine/model/datasource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import base64
 import gzip
 import json
 import logging
-import time
-
 import math
 import os.path
+import time
 import webbrowser
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Any, Dict, List, Optional, TYPE_CHECKING, Union, Set, ContextManager
 
 import rich.progress
 from dataclasses_json import dataclass_json, config
 from pathvalidate import sanitize_filepath
 
-from dagshub.common import rich_console
 import dagshub.common.config
+from dagshub.common import rich_console
 from dagshub.common.analytics import send_analytics_event
 from dagshub.common.helpers import prompt_user, http_request, log_message
 from dagshub.common.rich_util import get_rich_progress
 from dagshub.common.util import lazy_load, multi_urljoin
 from dagshub.data_engine.client.models import PreprocessingStatus, MetadataFieldType, MetadataFieldSchema, \
     autogenerated_columns
 from dagshub.data_engine.model.datapoint import Datapoint
-from dagshub.data_engine.model.errors import WrongOperatorError, WrongOrderError, DatasetFieldComparisonError
+from dagshub.data_engine.model.errors import WrongOperatorError, WrongOrderError, DatasetFieldComparisonError, \
+    FieldNotFoundError
 from dagshub.data_engine.model.query import DatasourceQuery, _metadataTypeLookup, _metadataTypeLookupReverse
 
 if TYPE_CHECKING:
     from dagshub.data_engine.model.query_result import QueryResult
     from dagshub.data_engine.model.datasource_state import DatasourceState
     import fiftyone as fo
     import pandas
@@ -380,15 +380,15 @@
             webbrowser.open_new_tab(link)
         return link
 
     def _launch_annotation_workspace(self):
         try:
             start_workspace_url = multi_urljoin(self.source.repoApi.annotations_url, "start")
             http_request("POST", start_workspace_url, auth=self.source.repoApi.auth)
-        except: # noqa
+        except:  # noqa
             pass
 
     def wait_until_ready(self, max_wait_time=300, fail_on_timeout=True):
         """
        Blocks until the datasource preprocessing is complete
 
        Args:
@@ -419,18 +419,25 @@
                     else:
                         logger.warning(
                             f"Time limit of {max_wait_time} seconds reached before processing was completed.")
                         return
 
                 time.sleep(1)
 
+    def has_field(self, field_name: str):
+        fields = (f.name for f in self.fields)
+        return field_name in fields
+
     def __repr__(self):
         res = f"Datasource {self.source.name}"
         res += f"\n\tRepo: {self.source.repo}, path: {self.source.path}"
         res += f"\n\t{self._query}"
+        res += "\n\tFields:"
+        for f in self.fields:
+            res += f"\n\t\t{f}"
         return res + "\n"
 
     """ FUNCTIONS RELATED TO QUERYING
     These are functions that overload operators on the DataSet, so you can do pandas-like filtering
         ds = Dataset(...)
         queried_ds = ds[ds["value"] == 5]
     """
@@ -439,18 +446,20 @@
         # Slicing - get items from the slice
         if type(other) is slice:
             return self.sample(other.start, other.stop)
 
         # Otherwise we're doing querying
         new_ds = self.__deepcopy__()
         if type(other) is str:
+            if not self.has_field(other):
+                raise FieldNotFoundError(other)
             new_ds._query = DatasourceQuery(other)
             return new_ds
         else:
-            # "index" is a dataset with a query - compose with "and"
+            # "index" is a datasource with a query - compose with "and"
             # Example:
             #   ds = Dataset()
             #   filtered_ds = ds[ds["aaa"] > 5]
             #   filtered_ds2 = filtered_ds[filtered_ds["bbb"] < 4]
             if self._query.is_empty:
                 new_ds._query = other._query
                 return new_ds
```

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/model/datasource_state.py` & `dagshub-0.3.0.post4/dagshub/data_engine/model/datasource_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,16 @@
     _revision: Optional[str] = field(init=False, default=None)
 
     def __post_init__(self):
         self.client = DataClient(self.repo)
         self.repoApi = RepoAPI(self.repo)
         if hasattr(self, "source_type") and self.source_type == DatasourceType.REPOSITORY:
             self.revision = self.path_parts()["revision"]
+        if not hasattr(self, "metadata_fields"):
+            self.metadata_fields = []
 
     @property
     def revision(self) -> str:
         """Used for repository sources, provides branch/revision from which to download files"""
         if self._revision is None:
             logger.warning("Revision wasn't set, assuming default repo branch")
             self.revision = self.repoApi.default_branch
```

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/model/errors.py` & `dagshub-0.3.0.post4/dagshub/data_engine/model/errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,23 @@
                "Querying only supports comparisons with primitives (int/str/float)"
 
 
 class WrongOperatorError(Exception):
     pass
 
 
+class FieldNotFoundError(Exception):
+    def __init__(self, field: str):
+        super().__init__()
+        self.field = field
+
+    def __str__(self):
+        return f"Field {self.field} does not exist on this datasource"
+
+
 class DatasourceAlreadyExistsError(Exception):
     def __init__(self, datasource):
         super().__init__()
         self.datasource = datasource
 
     def __str__(self):
         return f"Datasource with name {self.datasource.name} already exists in repository {self.datasource.repo}"
```

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/model/query.py` & `dagshub-0.3.0.post4/dagshub/data_engine/model/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,16 +62,16 @@
             # If it's ds["column"] then the root node is just the column name
             self._column_filter = column_or_query
         elif column_or_query is not None:
             self._operand_tree.create_node(column_or_query)
 
     def __repr__(self):
         if self.is_empty:
-            return "<Query: empty>"
-        return f"<Query: {self.to_dict()}>"
+            return "Query: empty"
+        return f"Query: {self.to_dict()}"
 
     @property
     def column_filter(self) -> Optional[str]:
         return self._column_filter
 
     def compose(self, op: str, other: Optional[Union[str, int, float, "DatasourceQuery", "Datasource"]]):
         if self._column_filter is not None:
```

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/model/query_result.py` & `dagshub-0.3.0.post4/dagshub/data_engine/model/query_result.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/app.py` & `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/app.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/models.py` & `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/models.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg` & `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js` & `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/annotation.py` & `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/annotation.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/datasource.py` & `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/datasource.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/util.py` & `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/routes/voxel.py` & `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/routes/voxel.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/server.py` & `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/server.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/data_engine/voxel_plugin_server/utils.py` & `dagshub-0.3.0.post4/dagshub/data_engine/voxel_plugin_server/utils.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/fastai/logger.py` & `dagshub-0.3.0.post4/dagshub/fastai/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/keras/logger.py` & `dagshub-0.3.0.post4/dagshub/keras/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/logger.py` & `dagshub-0.3.0.post4/dagshub/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/notebook.py` & `dagshub-0.3.0.post4/dagshub/notebook.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/pytorch_lightning/logger.py` & `dagshub-0.3.0.post4/dagshub/pytorch_lightning/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/streaming/dataclasses.py` & `dagshub-0.3.0.post4/dagshub/streaming/dataclasses.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/streaming/filesystem.py` & `dagshub-0.3.0.post4/dagshub/streaming/filesystem.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/streaming/mount.py` & `dagshub-0.3.0.post4/dagshub/streaming/mount.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/upload/errors.py` & `dagshub-0.3.0.post4/dagshub/upload/errors.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/dagshub/upload/wrapper.py` & `dagshub-0.3.0.post4/dagshub/upload/wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import fnmatch
 import json
 import logging
 import os
 import posixpath
+import time
 import urllib
 from http import HTTPStatus
 from io import IOBase
 from pathlib import Path
-from typing import Union, Tuple, BinaryIO, Dict
+from typing import Union, Tuple, BinaryIO, Dict, Optional
 
 import httpx
 import rich.progress
+import rich.status
 
 import dagshub.auth
 from dagshub.auth.token_auth import HTTPBearerAuth
 from dagshub.common import config, rich_console
 from dagshub.common.api.repo import RepoAPI
 from dagshub.common.helpers import log_message
 from dagshub.upload.errors import determine_upload_api_error
@@ -178,14 +180,17 @@
     def __init__(
         self, owner, name, username=None, password=None, token=None, branch=None
     ):
 
         """
         Repo class constructor. If branch is not provided, then default branch is used.
 
+        WARNING: this class is not thread safe.
+        Uploading files in parallel can lead to unexpected outcomes
+
         :param owner (str): Store the username of the user who owns this repository
         :param name (str): Identify the repository
         :param username (str): Set the username to none if it is not provided
         :param password (str): Set the password to none if it is not provided
         :param token (str): Set the token
         :param branch (str): Set the branch to the default branch
         :return: The object of the class
@@ -198,14 +203,18 @@
         self.username = username or config.username
         self.password = password or config.password
         self.token = token or config.token
         self.branch = branch
 
         self._api = RepoAPI(f"{owner}/{name}", host=self.host, auth=self.auth)
 
+        # For mirror uploading: store the last revision for which we uploaded
+        # When the last revision changes, that means the sync has been complete and we can upload a new batch
+        self._last_upload_revision: Optional[str] = None
+
         if self.branch is None:
             logger.debug("Branch wasn't provided. Fetching default branch...")
             self.branch = self._api.default_branch
         logger.debug(f"Set branch: {self.branch}")
 
     def upload(
         self,
@@ -277,27 +286,33 @@
         if new_branch is not None:
             data.update(
                 {
                     "commit_choice": "commit-to-new-branch",
                     "new_branch_name": new_branch,
                 }
             )
+        # elif self._api.is_mirror:
+        #     # If not uploading to a new branch, and we're in a mirror - wait for the sync to complete
+        #     self._poll_mirror_up_to_date()
 
         if force:
             data["last_commit"] = self._api.last_commit_sha(self.branch)
 
         log_message(f'Uploading files ({len(files)}) to "{self._api.full_name}"...', logger)
         res = s.put(
             self.get_request_url(directory_path),
             data=data,
             files=[("files", file) for file in files],
             auth=self.auth,
             timeout=None,
         )
         self._log_upload_details(data, res, files)
+        # 204 means nothing was added, so if we're in the mirror we can upload the next batch immediately
+        if new_branch is None and self._api.is_mirror and res.status_code == 204:
+            self._last_upload_revision = None
 
     @staticmethod
     def _log_upload_details(data, res, files):
         """
         The _log_upload_details function logs the request URL, data, and files.
         It then logs the response status code and content.
         If the response is not 200(OK), or 204(NoContent) it raises an error.
@@ -317,17 +332,54 @@
             f"Files:\n{json.dumps(list(map(str, files)), indent=4)}"
         )
 
         if res.status_code == HTTPStatus.OK:
             log_message("Upload finished successfully!", logger)
         elif res.status_code == HTTPStatus.NO_CONTENT:
             log_message("Upload successful, content was identical and no new commit was created", logger)
+        elif res.status_code < 400:
+            log_message(f"Got unknown successful status code {res.status_code}")
         else:
             raise determine_upload_api_error(res)
 
+    def _poll_mirror_up_to_date(self):
+        """
+        Synchronization lock for the mirrored repository uploading
+        Since the upload is being done "through" DagsHub,
+            and we rely on the change first showing up on the original repo, then being synced back to us,
+            there is a possibility of uploading a new batch before the sync has been completed,
+            during which the DagsHub repo is out of date with the original mirror.
+        This is a client-side fix made to mitigate this.
+        We poll for the change in the revision and compare it to the revision we had when we last uploaded
+        When the revision changes, that means the sync has been completed and we can upload a new batch
+        """
+        if not self._api.is_mirror:
+            return
+        # Initial state - assume we can upload
+        if self._last_upload_revision is None:
+            self._last_upload_revision = self._api.last_commit_sha(self.branch)
+            return
+
+        poll_interval = 1.0  # seconds
+        poll_timeout = 600.0
+        start_time = time.time()
+
+        with rich.status.Status("Waiting for the mirror to sync", console=rich_console):
+            while True:
+                new_revision = self._api.last_commit_sha(self.branch)
+                if new_revision == self._last_upload_revision:
+                    if time.time() - start_time > poll_timeout:
+                        logger.warning(f"Timed out while polling for a mirror sync finishing after {poll_timeout} s. "
+                                       f"Trying to push anyway, which might not work.")
+                        return
+                    time.sleep(poll_interval)
+                else:
+                    self._last_upload_revision = new_revision
+                    return
+
     @property
     def auth(self):
         """
         The auth function is used to authenticate the user with the dagshub API.
             It takes in a username and password, or token as arguments. If both are provided,
             it will use the username and password combination to
             get a token from dagshub's authentication server.
```

### Comparing `dagshub-0.3.0.post3/dagshub.egg-info/PKG-INFO` & `dagshub-0.3.0.post4/dagshub.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagshub
-Version: 0.3.0.post3
+Version: 0.3.0.post4
 Summary: DagsHub client libraries
 Home-page: https://github.com/DagsHub/client
 Author: DagsHub
 Author-email: contact@dagshub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,14 +53,15 @@
 
 For more details on the different functions of the client, check out the docs segments:
 1. [Installation & Setup](https://github.com/DagsHub/client/blob/master/docs/index.md#installation-and-setup)
 2. [Data Streaming](https://github.com/DagsHub/client/blob/master/docs/index.md#data-streaming)
 3. [Data Upload](https://github.com/DagsHub/client/blob/master/docs/index.md#data-upload)
 4. [Experiment Tracking](https://github.com/DagsHub/client/blob/master/docs/index.md#experiment-tracking-logger)
     1. [Autologging](https://github.com/DagsHub/client/blob/master/docs/index.md#autologging-integrations-with-ml-frameworks)
+5. [Data Engine](https://github.com/DagsHub/client/blob/master/docs/data_engine.md)
 
 Some functionality is supported only in Python.
 
 To read about some of the awesome use cases for Direct Data Access, check out
 the [relevant doc page](https://dagshub.com/docs/feature_guide/direct_data_access/#use-cases).
 
 ## Installation
@@ -90,8 +91,13 @@
 
 ## Next Steps
 You can dive into the expanded [documentation](docs/index.md), to learn more about data streaming, data upload and
 experiment tracking with DagsHub
 
 ---
 
+
+### Analytics
+To improve your experience, we collect analytics on client usage. If you want to disable analytics collection,
+set the `DAGSHUB_DISABLE_ANALYTICS` environment variable to any value.
+
 Made with 🐶 by [DagsHub](https://dagshub.com/).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dagshub Version: 0.3.0.post3 Summary: DagsHub
+Metadata-Version: 2.1 Name: dagshub Version: 0.3.0.post4 Summary: DagsHub
 client libraries Home-page: https://github.com/DagsHub/client Author: DagsHub
 Author-email: contact@dagshub.com Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE [![DagsHub Client](https://github.com/DagsHub/
 client/raw/master/dagshub_github.png)](https://dagshub.com)
    **** ð Launching Streaming and Upload of DVC versioned Data ð ****
@@ -48,16 +48,17 @@
 client, check out the docs segments: 1. [Installation & Setup](https://
 github.com/DagsHub/client/blob/master/docs/index.md#installation-and-setup) 2.
 [Data Streaming](https://github.com/DagsHub/client/blob/master/docs/
 index.md#data-streaming) 3. [Data Upload](https://github.com/DagsHub/client/
 blob/master/docs/index.md#data-upload) 4. [Experiment Tracking](https://
 github.com/DagsHub/client/blob/master/docs/index.md#experiment-tracking-logger)
 1. [Autologging](https://github.com/DagsHub/client/blob/master/docs/
-index.md#autologging-integrations-with-ml-frameworks) Some functionality is
-supported only in Python. To read about some of the awesome use cases for
+index.md#autologging-integrations-with-ml-frameworks) 5. [Data Engine](https://
+github.com/DagsHub/client/blob/master/docs/data_engine.md) Some functionality
+is supported only in Python. To read about some of the awesome use cases for
 Direct Data Access, check out the [relevant doc page](https://dagshub.com/docs/
 feature_guide/direct_data_access/#use-cases). ## Installation ```bash pip
 install dagshub ``` Direct Data Access (DDA) functionality requires
 authentication, which you can easily do by running the following command in
 your terminal: ```bash dagshub login ``` ## Quickstart for Data Streaming The
 easiest way to start using DagsHub is via the Python Hooks method. To do this:
 1. Your DagsHub project, 2. Copy the following 2 lines of code into your Python
@@ -65,8 +66,11 @@
 install_hooks install_hooks() ``` 3. Thatâs it! You now have streaming access
 to all your project files. **ð¤© Check out this colab to see an example of
 this Data Streaming work end to end:** [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1CtBmcDtZnxZKVIhNvPagX-8UFWHZ5HAg?usp=sharing)
 ## Next Steps You can dive into the expanded [documentation](docs/index.md), to
 learn more about data streaming, data upload and experiment tracking with
-DagsHub --- Made with ð¶ by [DagsHub](https://dagshub.com/).
+DagsHub --- ### Analytics To improve your experience, we collect analytics on
+client usage. If you want to disable analytics collection, set the
+`DAGSHUB_DISABLE_ANALYTICS` environment variable to any value. Made with ð¶
+by [DagsHub](https://dagshub.com/).
```

### Comparing `dagshub-0.3.0.post3/dagshub.egg-info/SOURCES.txt` & `dagshub-0.3.0.post4/dagshub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/setup.py` & `dagshub-0.3.0.post4/setup.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/tests/test_dagshub_logger.py` & `dagshub-0.3.0.post4/tests/test_dagshub_logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.0.post3/tests/test_misc.py` & `dagshub-0.3.0.post4/tests/test_misc.py`

 * *Files identical despite different names*

