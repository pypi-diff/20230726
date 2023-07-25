# Comparing `tmp/dominodatalab_data-5.7.0.tar.gz` & `tmp/dominodatalab_data-5.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dominodatalab_data-5.7.0.tar", max compression
+gzip compressed data, was "dominodatalab_data-5.7.1.tar", max compression
```

## Comparing `dominodatalab_data-5.7.0.tar` & `dominodatalab_data-5.7.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0    10891 2022-12-13 21:08:46.883572 dominodatalab_data-5.7.0/LICENSE
--rw-r--r--   0        0        0     5982 2023-06-30 18:10:37.170554 dominodatalab_data-5.7.0/README.md
--rw-r--r--   0        0        0      102 2022-12-13 21:08:46.888200 dominodatalab_data-5.7.0/datasource_api_client/__init__.py
--rw-r--r--   0        0        0       47 2022-12-13 21:08:46.888449 dominodatalab_data-5.7.0/datasource_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-13 21:08:46.888635 dominodatalab_data-5.7.0/datasource_api_client/api/datasource/__init__.py
--rw-r--r--   0        0        0     4143 2023-06-21 23:24:10.676184 dominodatalab_data-5.7.0/datasource_api_client/api/datasource/get_datasource_by_name.py
--rw-r--r--   0        0        0        0 2022-12-13 21:08:46.889007 dominodatalab_data-5.7.0/datasource_api_client/api/proxy/__init__.py
--rw-r--r--   0        0        0     3381 2022-12-13 21:08:46.889155 dominodatalab_data-5.7.0/datasource_api_client/api/proxy/get_key_url.py
--rw-r--r--   0        0        0     3434 2022-12-13 21:08:46.889278 dominodatalab_data-5.7.0/datasource_api_client/api/proxy/list_keys.py
--rw-r--r--   0        0        0     2204 2022-12-13 21:08:46.889429 dominodatalab_data-5.7.0/datasource_api_client/api/proxy/log_metric.py
--rw-r--r--   0        0        0     1661 2022-12-13 21:08:46.889565 dominodatalab_data-5.7.0/datasource_api_client/client.py
--rw-r--r--   0        0        0      695 2022-12-13 21:08:46.889828 dominodatalab_data-5.7.0/datasource_api_client/models/__init__.py
--rw-r--r--   0        0        0     1173 2022-12-13 21:08:46.890343 dominodatalab_data-5.7.0/datasource_api_client/models/datasource_config.py
--rw-r--r--   0        0        0     4708 2022-12-13 21:08:46.890492 dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto.py
--rw-r--r--   0        0        0     1199 2022-12-13 21:08:46.890641 dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto_added_by.py
--rw-r--r--   0        0        0      428 2023-01-20 00:18:54.638950 dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto_auth_type.py
--rw-r--r--   0        0        0      712 2023-01-20 00:18:54.639696 dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto_data_source_type.py
--rw-r--r--   0        0        0      170 2022-12-13 21:08:46.891095 dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto_status.py
--rw-r--r--   0        0        0     1905 2022-12-13 21:08:46.891294 dominodatalab_data-5.7.0/datasource_api_client/models/datasource_owner_info.py
--rw-r--r--   0        0        0     1498 2022-12-13 21:08:46.891428 dominodatalab_data-5.7.0/datasource_api_client/models/error_response.py
--rw-r--r--   0        0        0     3569 2022-12-13 21:08:46.891567 dominodatalab_data-5.7.0/datasource_api_client/models/key_request.py
--rw-r--r--   0        0        0     3880 2022-12-13 21:08:46.891715 dominodatalab_data-5.7.0/datasource_api_client/models/list_request.py
--rw-r--r--   0        0        0      153 2022-12-13 21:08:46.891858 dominodatalab_data-5.7.0/datasource_api_client/models/log_metric_m.py
--rw-r--r--   0        0        0      239 2022-12-13 21:08:46.891994 dominodatalab_data-5.7.0/datasource_api_client/models/log_metric_t.py
--rw-r--r--   0        0        0     2084 2022-12-13 21:08:46.892129 dominodatalab_data-5.7.0/datasource_api_client/models/proxy_error_response.py
--rw-r--r--   0        0        0      939 2022-12-13 21:08:46.892280 dominodatalab_data-5.7.0/datasource_api_client/types.py
--rw-r--r--   0        0        0      369 2022-12-13 21:08:46.893659 dominodatalab_data-5.7.0/domino_data/__init__.py
--rw-r--r--   0        0        0        0 2022-12-13 21:08:46.893983 dominodatalab_data-5.7.0/domino_data/_feature_store/__init__.py
--rw-r--r--   0        0        0     3801 2023-02-06 21:42:31.303590 dominodatalab_data-5.7.0/domino_data/_feature_store/client.py
--rw-r--r--   0        0        0      684 2022-12-13 21:08:46.894282 dominodatalab_data-5.7.0/domino_data/_feature_store/exceptions.py
--rw-r--r--   0        0        0     2966 2023-01-04 19:29:57.407758 dominodatalab_data-5.7.0/domino_data/_feature_store/git.py
--rw-r--r--   0        0        0      683 2023-01-04 19:29:57.408054 dominodatalab_data-5.7.0/domino_data/_feature_store/logging.py
--rw-r--r--   0        0        0     1223 2023-01-04 19:29:57.408553 dominodatalab_data-5.7.0/domino_data/_feature_store/run.py
--rw-r--r--   0        0        0     8180 2023-02-06 21:42:31.304886 dominodatalab_data-5.7.0/domino_data/_feature_store/sync.py
--rw-r--r--   0        0        0     4527 2022-12-13 21:08:46.894894 dominodatalab_data-5.7.0/domino_data/auth.py
--rw-r--r--   0        0        0    10464 2023-02-06 21:42:28.586341 dominodatalab_data-5.7.0/domino_data/configuration_gen.py
--rw-r--r--   0        0        0    27063 2023-06-30 22:30:47.388304 dominodatalab_data-5.7.0/domino_data/data_sources.py
--rw-r--r--   0        0        0      894 2023-01-04 19:29:57.409242 dominodatalab_data-5.7.0/domino_data/logging.py
--rw-r--r--   0        0        0        0 2022-12-13 21:08:46.895616 dominodatalab_data-5.7.0/domino_data/py.typed
--rw-r--r--   0        0        0        0 2022-12-13 21:08:46.895810 dominodatalab_data-5.7.0/domino_data/training_sets/__init__.py
--rw-r--r--   0        0        0    13955 2022-12-13 21:08:46.895997 dominodatalab_data-5.7.0/domino_data/training_sets/client.py
--rw-r--r--   0        0        0     3588 2022-12-13 21:08:46.896143 dominodatalab_data-5.7.0/domino_data/training_sets/model.py
--rw-r--r--   0        0        0     2550 2023-06-30 22:30:47.388714 dominodatalab_data-5.7.0/domino_data/transfer.py
--rw-r--r--   0        0        0      104 2022-12-13 21:08:46.896371 dominodatalab_data-5.7.0/feature_store_api_client/__init__.py
--rw-r--r--   0        0        0       47 2022-12-13 21:08:46.896618 dominodatalab_data-5.7.0/feature_store_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-13 21:08:46.896866 dominodatalab_data-5.7.0/feature_store_api_client/api/default/__init__.py
--rw-r--r--   0        0        0     2657 2022-12-13 21:08:46.897016 dominodatalab_data-5.7.0/feature_store_api_client/api/default/get.py
--rw-r--r--   0        0        0     2861 2022-12-13 21:08:46.897152 dominodatalab_data-5.7.0/feature_store_api_client/api/default/get_feature_view_name_store.py
--rw-r--r--   0        0        0     3383 2022-12-13 21:08:46.897295 dominodatalab_data-5.7.0/feature_store_api_client/api/default/post.py
--rw-r--r--   0        0        0     1870 2022-12-13 21:08:46.897427 dominodatalab_data-5.7.0/feature_store_api_client/api/default/post_featureview.py
--rw-r--r--   0        0        0     3215 2022-12-13 21:08:46.897553 dominodatalab_data-5.7.0/feature_store_api_client/api/default/post_lock.py
--rw-r--r--   0        0        0     3144 2022-12-13 21:08:46.897705 dominodatalab_data-5.7.0/feature_store_api_client/api/default/post_unlock.py
--rw-r--r--   0        0        0     1822 2022-12-13 21:08:46.897860 dominodatalab_data-5.7.0/feature_store_api_client/client.py
--rw-r--r--   0        0        0     1443 2023-02-06 21:42:31.307225 dominodatalab_data-5.7.0/feature_store_api_client/models/__init__.py
--rw-r--r--   0        0        0     2002 2022-12-13 21:08:46.898606 dominodatalab_data-5.7.0/feature_store_api_client/models/auth_config.py
--rw-r--r--   0        0        0     1513 2022-12-13 21:08:46.898839 dominodatalab_data-5.7.0/feature_store_api_client/models/auth_config_fields.py
--rw-r--r--   0        0        0     1166 2022-12-13 21:08:46.898998 dominodatalab_data-5.7.0/feature_store_api_client/models/auth_config_meta.py
--rw-r--r--   0        0        0      170 2022-12-13 21:08:46.899130 dominodatalab_data-5.7.0/feature_store_api_client/models/auth_field_name.py
--rw-r--r--   0        0        0      197 2022-12-13 21:08:46.899246 dominodatalab_data-5.7.0/feature_store_api_client/models/auth_type.py
--rw-r--r--   0        0        0      668 2022-12-13 21:08:46.899363 dominodatalab_data-5.7.0/feature_store_api_client/models/config_field_name.py
--rw-r--r--   0        0        0     2987 2022-12-13 21:08:46.899487 dominodatalab_data-5.7.0/feature_store_api_client/models/create_feature_store_request.py
--rw-r--r--   0        0        0     1323 2022-12-13 21:08:46.899636 dominodatalab_data-5.7.0/feature_store_api_client/models/create_feature_store_request_offline_store_config.py
--rw-r--r--   0        0        0     1832 2022-12-13 21:08:46.899849 dominodatalab_data-5.7.0/feature_store_api_client/models/entity.py
--rw-r--r--   0        0        0     1721 2023-02-06 21:42:31.308456 dominodatalab_data-5.7.0/feature_store_api_client/models/feature.py
--rw-r--r--   0        0        0     3878 2022-12-13 21:08:46.900117 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_store.py
--rw-r--r--   0        0        0     1252 2022-12-13 21:08:46.900229 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_store_offline_store_config.py
--rw-r--r--   0        0        0      175 2022-12-13 21:08:46.900333 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_store_sync_result.py
--rw-r--r--   0        0        0     1148 2023-02-06 21:42:31.309808 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_tags.py
--rw-r--r--   0        0        0     3863 2022-12-13 21:08:46.900460 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view.py
--rw-r--r--   0        0        0     3261 2023-02-06 21:42:31.311302 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view_request.py
--rw-r--r--   0        0        0     1209 2022-12-13 21:08:46.900686 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view_request_tags.py
--rw-r--r--   0        0        0     1171 2022-12-13 21:08:46.901421 dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view_tags.py
--rw-r--r--   0        0        0     2968 2022-12-13 21:08:46.901544 dominodatalab_data-5.7.0/feature_store_api_client/models/field.py
--rw-r--r--   0        0        0      340 2022-12-13 21:08:46.901657 dominodatalab_data-5.7.0/feature_store_api_client/models/git_provider_name.py
--rw-r--r--   0        0        0     2405 2022-12-13 21:08:46.901774 dominodatalab_data-5.7.0/feature_store_api_client/models/lock_feature_store_request.py
--rw-r--r--   0        0        0     1750 2022-12-13 21:08:46.901882 dominodatalab_data-5.7.0/feature_store_api_client/models/metadata.py
--rw-r--r--   0        0        0     2552 2022-12-13 21:08:46.901982 dominodatalab_data-5.7.0/feature_store_api_client/models/offline_store_config.py
--rw-r--r--   0        0        0     1556 2022-12-13 21:08:46.902065 dominodatalab_data-5.7.0/feature_store_api_client/models/offline_store_config_fields.py
--rw-r--r--   0        0        0      219 2022-12-13 21:08:46.902164 dominodatalab_data-5.7.0/feature_store_api_client/models/offline_store_type.py
--rw-r--r--   0        0        0     1895 2022-12-13 21:08:46.902282 dominodatalab_data-5.7.0/feature_store_api_client/models/unlock_feature_store_request.py
--rw-r--r--   0        0        0     2459 2023-02-06 21:42:31.312038 dominodatalab_data-5.7.0/feature_store_api_client/models/upsert_feature_views_request.py
--rw-r--r--   0        0        0      939 2022-12-13 21:08:46.902477 dominodatalab_data-5.7.0/feature_store_api_client/types.py
--rw-r--r--   0        0        0     3831 2023-06-30 22:49:15.478754 dominodatalab_data-5.7.0/pyproject.toml
--rw-r--r--   0        0        0      103 2022-12-13 21:08:46.910476 dominodatalab_data-5.7.0/training_set_api_client/__init__.py
--rw-r--r--   0        0        0       47 2022-12-13 21:08:46.910619 dominodatalab_data-5.7.0/training_set_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-13 21:08:46.910785 dominodatalab_data-5.7.0/training_set_api_client/api/default/__init__.py
--rw-r--r--   0        0        0     1441 2022-12-13 21:08:46.910908 dominodatalab_data-5.7.0/training_set_api_client/api/default/delete_training_set_name.py
--rw-r--r--   0        0        0     1576 2022-12-13 21:08:46.911013 dominodatalab_data-5.7.0/training_set_api_client/api/default/delete_training_set_name_number.py
--rw-r--r--   0        0        0     2242 2022-12-13 21:08:46.911099 dominodatalab_data-5.7.0/training_set_api_client/api/default/get_training_set_name.py
--rw-r--r--   0        0        0     2525 2022-12-13 21:08:46.911182 dominodatalab_data-5.7.0/training_set_api_client/api/default/get_training_set_name_number.py
--rw-r--r--   0        0        0     3679 2022-12-13 21:08:46.911276 dominodatalab_data-5.7.0/training_set_api_client/api/default/post_find.py
--rw-r--r--   0        0        0     2832 2022-12-13 21:08:46.911364 dominodatalab_data-5.7.0/training_set_api_client/api/default/post_training_set_name.py
--rw-r--r--   0        0        0     3801 2022-12-13 21:08:46.911452 dominodatalab_data-5.7.0/training_set_api_client/api/default/post_version_find.py
--rw-r--r--   0        0        0     2716 2022-12-13 21:08:46.911584 dominodatalab_data-5.7.0/training_set_api_client/api/default/put_training_set_name.py
--rw-r--r--   0        0        0     3049 2022-12-13 21:08:46.911684 dominodatalab_data-5.7.0/training_set_api_client/api/default/put_training_set_name_number.py
--rw-r--r--   0        0        0     1661 2022-12-13 21:08:46.911774 dominodatalab_data-5.7.0/training_set_api_client/client.py
--rw-r--r--   0        0        0     1139 2022-12-13 21:08:46.911917 dominodatalab_data-5.7.0/training_set_api_client/models/__init__.py
--rw-r--r--   0        0        0     3301 2022-12-13 21:08:46.912007 dominodatalab_data-5.7.0/training_set_api_client/models/create_training_set_version_request.py
--rw-r--r--   0        0        0     1280 2022-12-13 21:08:46.912105 dominodatalab_data-5.7.0/training_set_api_client/models/create_training_set_version_request_meta.py
--rw-r--r--   0        0        0     1995 2022-12-13 21:08:46.912303 dominodatalab_data-5.7.0/training_set_api_client/models/monitoring_meta.py
--rw-r--r--   0        0        0     2411 2022-12-13 21:08:46.912407 dominodatalab_data-5.7.0/training_set_api_client/models/training_set.py
--rw-r--r--   0        0        0     2010 2022-12-13 21:08:46.912513 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_filter.py
--rw-r--r--   0        0        0     1204 2022-12-13 21:08:46.912628 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_filter_meta.py
--rw-r--r--   0        0        0     1171 2022-12-13 21:08:46.912764 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_meta.py
--rw-r--r--   0        0        0     4472 2022-12-13 21:08:46.912863 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version.py
--rw-r--r--   0        0        0     2545 2022-12-13 21:08:46.912963 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_filter.py
--rw-r--r--   0        0        0     1242 2022-12-13 21:08:46.913081 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_filter_meta.py
--rw-r--r--   0        0        0     1303 2022-12-13 21:08:46.913192 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_filter_training_set_meta.py
--rw-r--r--   0        0        0     1209 2022-12-13 21:08:46.913297 dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_meta.py
--rw-r--r--   0        0        0     1844 2022-12-13 21:08:46.913396 dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_request.py
--rw-r--r--   0        0        0     1242 2022-12-13 21:08:46.913504 dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_request_meta.py
--rw-r--r--   0        0        0     3070 2022-12-13 21:08:46.913600 dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_version_request.py
--rw-r--r--   0        0        0     1280 2022-12-13 21:08:46.913689 dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_version_request_meta.py
--rw-r--r--   0        0        0      984 2022-12-13 21:08:46.913773 dominodatalab_data-5.7.0/training_set_api_client/types.py
--rw-r--r--   0        0        0     7310 1970-01-01 00:00:00.000000 dominodatalab_data-5.7.0/PKG-INFO
+-rw-r--r--   0        0        0    10891 2022-12-13 21:08:46.883572 dominodatalab_data-5.7.1/LICENSE
+-rw-r--r--   0        0        0     5982 2023-07-20 22:48:08.992771 dominodatalab_data-5.7.1/README.md
+-rw-r--r--   0        0        0      102 2022-12-13 21:08:46.888200 dominodatalab_data-5.7.1/datasource_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2022-12-13 21:08:46.888449 dominodatalab_data-5.7.1/datasource_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-13 21:08:46.888635 dominodatalab_data-5.7.1/datasource_api_client/api/datasource/__init__.py
+-rw-r--r--   0        0        0     4143 2023-07-25 21:18:01.766650 dominodatalab_data-5.7.1/datasource_api_client/api/datasource/get_datasource_by_name.py
+-rw-r--r--   0        0        0        0 2022-12-13 21:08:46.889007 dominodatalab_data-5.7.1/datasource_api_client/api/proxy/__init__.py
+-rw-r--r--   0        0        0     3381 2023-07-25 21:18:01.766907 dominodatalab_data-5.7.1/datasource_api_client/api/proxy/get_key_url.py
+-rw-r--r--   0        0        0     3434 2023-07-25 21:18:01.767159 dominodatalab_data-5.7.1/datasource_api_client/api/proxy/list_keys.py
+-rw-r--r--   0        0        0     2204 2023-07-25 21:18:01.767451 dominodatalab_data-5.7.1/datasource_api_client/api/proxy/log_metric.py
+-rw-r--r--   0        0        0     1661 2023-07-25 21:18:01.767728 dominodatalab_data-5.7.1/datasource_api_client/client.py
+-rw-r--r--   0        0        0      695 2022-12-13 21:08:46.889828 dominodatalab_data-5.7.1/datasource_api_client/models/__init__.py
+-rw-r--r--   0        0        0     1173 2022-12-13 21:08:46.890343 dominodatalab_data-5.7.1/datasource_api_client/models/datasource_config.py
+-rw-r--r--   0        0        0     4708 2022-12-13 21:08:46.890492 dominodatalab_data-5.7.1/datasource_api_client/models/datasource_dto.py
+-rw-r--r--   0        0        0     1199 2022-12-13 21:08:46.890641 dominodatalab_data-5.7.1/datasource_api_client/models/datasource_dto_added_by.py
+-rw-r--r--   0        0        0      428 2023-07-20 22:48:08.995331 dominodatalab_data-5.7.1/datasource_api_client/models/datasource_dto_auth_type.py
+-rw-r--r--   0        0        0      712 2023-07-25 21:18:01.768820 dominodatalab_data-5.7.1/datasource_api_client/models/datasource_dto_data_source_type.py
+-rw-r--r--   0        0        0      170 2022-12-13 21:08:46.891095 dominodatalab_data-5.7.1/datasource_api_client/models/datasource_dto_status.py
+-rw-r--r--   0        0        0     1905 2022-12-13 21:08:46.891294 dominodatalab_data-5.7.1/datasource_api_client/models/datasource_owner_info.py
+-rw-r--r--   0        0        0     1498 2022-12-13 21:08:46.891428 dominodatalab_data-5.7.1/datasource_api_client/models/error_response.py
+-rw-r--r--   0        0        0     3569 2022-12-13 21:08:46.891567 dominodatalab_data-5.7.1/datasource_api_client/models/key_request.py
+-rw-r--r--   0        0        0     3880 2023-07-25 21:18:01.769075 dominodatalab_data-5.7.1/datasource_api_client/models/list_request.py
+-rw-r--r--   0        0        0      153 2022-12-13 21:08:46.891858 dominodatalab_data-5.7.1/datasource_api_client/models/log_metric_m.py
+-rw-r--r--   0        0        0      239 2022-12-13 21:08:46.891994 dominodatalab_data-5.7.1/datasource_api_client/models/log_metric_t.py
+-rw-r--r--   0        0        0     2084 2022-12-13 21:08:46.892129 dominodatalab_data-5.7.1/datasource_api_client/models/proxy_error_response.py
+-rw-r--r--   0        0        0      939 2023-07-20 22:48:08.996991 dominodatalab_data-5.7.1/datasource_api_client/types.py
+-rw-r--r--   0        0        0      369 2022-12-13 21:08:46.893659 dominodatalab_data-5.7.1/domino_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 22:48:08.998268 dominodatalab_data-5.7.1/domino_data/_feature_store/__init__.py
+-rw-r--r--   0        0        0     3801 2023-07-20 22:48:08.998880 dominodatalab_data-5.7.1/domino_data/_feature_store/client.py
+-rw-r--r--   0        0        0      684 2023-07-20 22:48:08.999044 dominodatalab_data-5.7.1/domino_data/_feature_store/exceptions.py
+-rw-r--r--   0        0        0     2966 2023-07-20 22:48:08.999763 dominodatalab_data-5.7.1/domino_data/_feature_store/git.py
+-rw-r--r--   0        0        0      683 2023-07-20 22:48:09.000218 dominodatalab_data-5.7.1/domino_data/_feature_store/logging.py
+-rw-r--r--   0        0        0     1223 2023-07-20 22:48:09.000513 dominodatalab_data-5.7.1/domino_data/_feature_store/run.py
+-rw-r--r--   0        0        0     8180 2023-07-20 22:48:09.000922 dominodatalab_data-5.7.1/domino_data/_feature_store/sync.py
+-rw-r--r--   0        0        0     4527 2023-07-20 22:48:09.001175 dominodatalab_data-5.7.1/domino_data/auth.py
+-rw-r--r--   0        0        0    10464 2023-07-25 21:18:01.770172 dominodatalab_data-5.7.1/domino_data/configuration_gen.py
+-rw-r--r--   0        0        0    27063 2023-07-25 21:18:01.771520 dominodatalab_data-5.7.1/domino_data/data_sources.py
+-rw-r--r--   0        0        0      894 2023-01-04 19:29:57.409242 dominodatalab_data-5.7.1/domino_data/logging.py
+-rw-r--r--   0        0        0        0 2022-12-13 21:08:46.895616 dominodatalab_data-5.7.1/domino_data/py.typed
+-rw-r--r--   0        0        0        0 2022-12-13 21:08:46.895810 dominodatalab_data-5.7.1/domino_data/training_sets/__init__.py
+-rw-r--r--   0        0        0    13955 2023-07-20 22:48:09.003049 dominodatalab_data-5.7.1/domino_data/training_sets/client.py
+-rw-r--r--   0        0        0     3588 2022-12-13 21:08:46.896143 dominodatalab_data-5.7.1/domino_data/training_sets/model.py
+-rw-r--r--   0        0        0     2566 2023-07-25 17:05:35.878259 dominodatalab_data-5.7.1/domino_data/transfer.py
+-rw-r--r--   0        0        0      104 2023-07-20 22:48:09.003666 dominodatalab_data-5.7.1/feature_store_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-20 22:48:09.003784 dominodatalab_data-5.7.1/feature_store_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 22:48:09.003861 dominodatalab_data-5.7.1/feature_store_api_client/api/default/__init__.py
+-rw-r--r--   0        0        0     2657 2023-07-20 22:48:09.003992 dominodatalab_data-5.7.1/feature_store_api_client/api/default/get.py
+-rw-r--r--   0        0        0     2861 2023-07-20 22:48:09.004103 dominodatalab_data-5.7.1/feature_store_api_client/api/default/get_feature_view_name_store.py
+-rw-r--r--   0        0        0     3383 2023-07-20 22:48:09.004198 dominodatalab_data-5.7.1/feature_store_api_client/api/default/post.py
+-rw-r--r--   0        0        0     1870 2023-07-20 22:48:09.004458 dominodatalab_data-5.7.1/feature_store_api_client/api/default/post_featureview.py
+-rw-r--r--   0        0        0     3215 2023-07-20 22:48:09.004596 dominodatalab_data-5.7.1/feature_store_api_client/api/default/post_lock.py
+-rw-r--r--   0        0        0     3144 2023-07-20 22:48:09.004720 dominodatalab_data-5.7.1/feature_store_api_client/api/default/post_unlock.py
+-rw-r--r--   0        0        0     1822 2023-07-20 22:48:09.004825 dominodatalab_data-5.7.1/feature_store_api_client/client.py
+-rw-r--r--   0        0        0     1443 2023-07-20 22:48:09.005377 dominodatalab_data-5.7.1/feature_store_api_client/models/__init__.py
+-rw-r--r--   0        0        0     2002 2023-07-20 22:48:09.005624 dominodatalab_data-5.7.1/feature_store_api_client/models/auth_config.py
+-rw-r--r--   0        0        0     1513 2023-07-20 22:48:09.005775 dominodatalab_data-5.7.1/feature_store_api_client/models/auth_config_fields.py
+-rw-r--r--   0        0        0     1166 2023-07-20 22:48:09.005907 dominodatalab_data-5.7.1/feature_store_api_client/models/auth_config_meta.py
+-rw-r--r--   0        0        0      170 2023-07-20 22:48:09.006010 dominodatalab_data-5.7.1/feature_store_api_client/models/auth_field_name.py
+-rw-r--r--   0        0        0      197 2023-07-20 22:48:09.006118 dominodatalab_data-5.7.1/feature_store_api_client/models/auth_type.py
+-rw-r--r--   0        0        0      668 2023-07-20 22:48:09.006253 dominodatalab_data-5.7.1/feature_store_api_client/models/config_field_name.py
+-rw-r--r--   0        0        0     2987 2023-07-20 22:48:09.006367 dominodatalab_data-5.7.1/feature_store_api_client/models/create_feature_store_request.py
+-rw-r--r--   0        0        0     1323 2023-07-20 22:48:09.006521 dominodatalab_data-5.7.1/feature_store_api_client/models/create_feature_store_request_offline_store_config.py
+-rw-r--r--   0        0        0     1832 2023-07-20 22:48:09.006662 dominodatalab_data-5.7.1/feature_store_api_client/models/entity.py
+-rw-r--r--   0        0        0     1721 2023-07-20 22:48:09.007150 dominodatalab_data-5.7.1/feature_store_api_client/models/feature.py
+-rw-r--r--   0        0        0     3878 2023-07-20 22:48:09.007262 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_store.py
+-rw-r--r--   0        0        0     1252 2023-07-20 22:48:09.007374 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_store_offline_store_config.py
+-rw-r--r--   0        0        0      175 2023-07-20 22:48:09.007477 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_store_sync_result.py
+-rw-r--r--   0        0        0     1148 2023-07-20 22:48:09.007807 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_tags.py
+-rw-r--r--   0        0        0     3863 2023-07-20 22:48:09.007951 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view.py
+-rw-r--r--   0        0        0     3261 2023-07-20 22:48:09.008381 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view_request.py
+-rw-r--r--   0        0        0     1209 2023-07-20 22:48:09.008486 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view_request_tags.py
+-rw-r--r--   0        0        0     1171 2023-07-20 22:48:09.008653 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view_tags.py
+-rw-r--r--   0        0        0     2968 2023-07-20 22:48:09.008787 dominodatalab_data-5.7.1/feature_store_api_client/models/field.py
+-rw-r--r--   0        0        0      340 2023-07-20 22:48:09.008914 dominodatalab_data-5.7.1/feature_store_api_client/models/git_provider_name.py
+-rw-r--r--   0        0        0     2405 2023-07-20 22:48:09.009041 dominodatalab_data-5.7.1/feature_store_api_client/models/lock_feature_store_request.py
+-rw-r--r--   0        0        0     1750 2023-07-20 22:48:09.009149 dominodatalab_data-5.7.1/feature_store_api_client/models/metadata.py
+-rw-r--r--   0        0        0     2552 2023-07-20 22:48:09.009252 dominodatalab_data-5.7.1/feature_store_api_client/models/offline_store_config.py
+-rw-r--r--   0        0        0     1556 2023-07-20 22:48:09.009349 dominodatalab_data-5.7.1/feature_store_api_client/models/offline_store_config_fields.py
+-rw-r--r--   0        0        0      219 2023-07-20 22:48:09.009470 dominodatalab_data-5.7.1/feature_store_api_client/models/offline_store_type.py
+-rw-r--r--   0        0        0     1895 2023-07-20 22:48:09.009577 dominodatalab_data-5.7.1/feature_store_api_client/models/unlock_feature_store_request.py
+-rw-r--r--   0        0        0     2459 2023-07-20 22:48:09.009897 dominodatalab_data-5.7.1/feature_store_api_client/models/upsert_feature_views_request.py
+-rw-r--r--   0        0        0      939 2023-07-20 22:48:09.009999 dominodatalab_data-5.7.1/feature_store_api_client/types.py
+-rw-r--r--   0        0        0     3858 2023-07-25 22:13:15.765438 dominodatalab_data-5.7.1/pyproject.toml
+-rw-r--r--   0        0        0      103 2022-12-13 21:08:46.910476 dominodatalab_data-5.7.1/training_set_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2022-12-13 21:08:46.910619 dominodatalab_data-5.7.1/training_set_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-13 21:08:46.910785 dominodatalab_data-5.7.1/training_set_api_client/api/default/__init__.py
+-rw-r--r--   0        0        0     1441 2022-12-13 21:08:46.910908 dominodatalab_data-5.7.1/training_set_api_client/api/default/delete_training_set_name.py
+-rw-r--r--   0        0        0     1576 2022-12-13 21:08:46.911013 dominodatalab_data-5.7.1/training_set_api_client/api/default/delete_training_set_name_number.py
+-rw-r--r--   0        0        0     2242 2022-12-13 21:08:46.911099 dominodatalab_data-5.7.1/training_set_api_client/api/default/get_training_set_name.py
+-rw-r--r--   0        0        0     2525 2022-12-13 21:08:46.911182 dominodatalab_data-5.7.1/training_set_api_client/api/default/get_training_set_name_number.py
+-rw-r--r--   0        0        0     3679 2022-12-13 21:08:46.911276 dominodatalab_data-5.7.1/training_set_api_client/api/default/post_find.py
+-rw-r--r--   0        0        0     2832 2022-12-13 21:08:46.911364 dominodatalab_data-5.7.1/training_set_api_client/api/default/post_training_set_name.py
+-rw-r--r--   0        0        0     3801 2022-12-13 21:08:46.911452 dominodatalab_data-5.7.1/training_set_api_client/api/default/post_version_find.py
+-rw-r--r--   0        0        0     2716 2022-12-13 21:08:46.911584 dominodatalab_data-5.7.1/training_set_api_client/api/default/put_training_set_name.py
+-rw-r--r--   0        0        0     3049 2022-12-13 21:08:46.911684 dominodatalab_data-5.7.1/training_set_api_client/api/default/put_training_set_name_number.py
+-rw-r--r--   0        0        0     1661 2022-12-13 21:08:46.911774 dominodatalab_data-5.7.1/training_set_api_client/client.py
+-rw-r--r--   0        0        0     1139 2022-12-13 21:08:46.911917 dominodatalab_data-5.7.1/training_set_api_client/models/__init__.py
+-rw-r--r--   0        0        0     3301 2022-12-13 21:08:46.912007 dominodatalab_data-5.7.1/training_set_api_client/models/create_training_set_version_request.py
+-rw-r--r--   0        0        0     1280 2022-12-13 21:08:46.912105 dominodatalab_data-5.7.1/training_set_api_client/models/create_training_set_version_request_meta.py
+-rw-r--r--   0        0        0     1995 2022-12-13 21:08:46.912303 dominodatalab_data-5.7.1/training_set_api_client/models/monitoring_meta.py
+-rw-r--r--   0        0        0     2411 2022-12-13 21:08:46.912407 dominodatalab_data-5.7.1/training_set_api_client/models/training_set.py
+-rw-r--r--   0        0        0     2010 2022-12-13 21:08:46.912513 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_filter.py
+-rw-r--r--   0        0        0     1204 2022-12-13 21:08:46.912628 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_filter_meta.py
+-rw-r--r--   0        0        0     1171 2022-12-13 21:08:46.912764 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_meta.py
+-rw-r--r--   0        0        0     4472 2022-12-13 21:08:46.912863 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version.py
+-rw-r--r--   0        0        0     2545 2022-12-13 21:08:46.912963 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_filter.py
+-rw-r--r--   0        0        0     1242 2022-12-13 21:08:46.913081 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_filter_meta.py
+-rw-r--r--   0        0        0     1303 2022-12-13 21:08:46.913192 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_filter_training_set_meta.py
+-rw-r--r--   0        0        0     1209 2022-12-13 21:08:46.913297 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_meta.py
+-rw-r--r--   0        0        0     1844 2022-12-13 21:08:46.913396 dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_request.py
+-rw-r--r--   0        0        0     1242 2022-12-13 21:08:46.913504 dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_request_meta.py
+-rw-r--r--   0        0        0     3070 2022-12-13 21:08:46.913600 dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_version_request.py
+-rw-r--r--   0        0        0     1280 2022-12-13 21:08:46.913689 dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_version_request_meta.py
+-rw-r--r--   0        0        0      984 2022-12-13 21:08:46.913773 dominodatalab_data-5.7.1/training_set_api_client/types.py
+-rw-r--r--   0        0        0     7352 1970-01-01 00:00:00.000000 dominodatalab_data-5.7.1/PKG-INFO
```

### Comparing `dominodatalab_data-5.7.0/LICENSE` & `dominodatalab_data-5.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/README.md` & `dominodatalab_data-5.7.1/README.md`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/api/datasource/get_datasource_by_name.py` & `dominodatalab_data-5.7.1/datasource_api_client/api/datasource/get_datasource_by_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/api/proxy/get_key_url.py` & `dominodatalab_data-5.7.1/datasource_api_client/api/proxy/get_key_url.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/api/proxy/list_keys.py` & `dominodatalab_data-5.7.1/datasource_api_client/api/proxy/list_keys.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/api/proxy/log_metric.py` & `dominodatalab_data-5.7.1/datasource_api_client/api/proxy/log_metric.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/client.py` & `dominodatalab_data-5.7.1/datasource_api_client/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/models/__init__.py` & `dominodatalab_data-5.7.1/datasource_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/models/datasource_config.py` & `dominodatalab_data-5.7.1/datasource_api_client/models/datasource_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto.py` & `dominodatalab_data-5.7.1/datasource_api_client/models/datasource_dto.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto_added_by.py` & `dominodatalab_data-5.7.1/datasource_api_client/models/datasource_dto_added_by.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/models/datasource_dto_data_source_type.py` & `dominodatalab_data-5.7.1/datasource_api_client/models/datasource_dto_data_source_type.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/models/datasource_owner_info.py` & `dominodatalab_data-5.7.1/datasource_api_client/models/datasource_owner_info.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/models/error_response.py` & `dominodatalab_data-5.7.1/datasource_api_client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/models/key_request.py` & `dominodatalab_data-5.7.1/datasource_api_client/models/key_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/models/list_request.py` & `dominodatalab_data-5.7.1/datasource_api_client/models/list_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/models/proxy_error_response.py` & `dominodatalab_data-5.7.1/datasource_api_client/models/proxy_error_response.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/datasource_api_client/types.py` & `dominodatalab_data-5.7.1/datasource_api_client/types.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/domino_data/_feature_store/client.py` & `dominodatalab_data-5.7.1/domino_data/_feature_store/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/domino_data/_feature_store/exceptions.py` & `dominodatalab_data-5.7.1/domino_data/_feature_store/exceptions.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/domino_data/_feature_store/git.py` & `dominodatalab_data-5.7.1/domino_data/_feature_store/git.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/domino_data/_feature_store/logging.py` & `dominodatalab_data-5.7.1/domino_data/_feature_store/logging.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/domino_data/_feature_store/run.py` & `dominodatalab_data-5.7.1/domino_data/_feature_store/run.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/domino_data/_feature_store/sync.py` & `dominodatalab_data-5.7.1/domino_data/_feature_store/sync.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/domino_data/auth.py` & `dominodatalab_data-5.7.1/domino_data/auth.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/domino_data/configuration_gen.py` & `dominodatalab_data-5.7.1/domino_data/configuration_gen.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/domino_data/data_sources.py` & `dominodatalab_data-5.7.1/domino_data/data_sources.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/domino_data/logging.py` & `dominodatalab_data-5.7.1/domino_data/logging.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/domino_data/training_sets/client.py` & `dominodatalab_data-5.7.1/domino_data/training_sets/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/domino_data/training_sets/model.py` & `dominodatalab_data-5.7.1/domino_data/training_sets/model.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/domino_data/transfer.py` & `dominodatalab_data-5.7.1/domino_data/transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,11 +73,11 @@
 
         buffer = io.BytesIO()
         shutil.copyfileobj(res, buffer)
 
         buffer.seek(0)
         with self._lock:
             self.destination.seek(block[0])
-            shutil.copyfileobj(buffer, self.destination)
+            shutil.copyfileobj(buffer, self.destination)  # type: ignore
 
         buffer.close()
         res.release_connection()
```

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/api/default/get.py` & `dominodatalab_data-5.7.1/feature_store_api_client/api/default/get.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/api/default/get_feature_view_name_store.py` & `dominodatalab_data-5.7.1/feature_store_api_client/api/default/get_feature_view_name_store.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/api/default/post.py` & `dominodatalab_data-5.7.1/feature_store_api_client/api/default/post.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/api/default/post_featureview.py` & `dominodatalab_data-5.7.1/feature_store_api_client/api/default/post_featureview.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/api/default/post_lock.py` & `dominodatalab_data-5.7.1/feature_store_api_client/api/default/post_lock.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/api/default/post_unlock.py` & `dominodatalab_data-5.7.1/feature_store_api_client/api/default/post_unlock.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/client.py` & `dominodatalab_data-5.7.1/feature_store_api_client/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/__init__.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/auth_config.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/auth_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/auth_config_fields.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/auth_config_fields.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/auth_config_meta.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/auth_config_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/config_field_name.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/config_field_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/create_feature_store_request.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/create_feature_store_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/create_feature_store_request_offline_store_config.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/create_feature_store_request_offline_store_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/entity.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/entity.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/feature.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/feature.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/feature_store.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/feature_store.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/feature_store_offline_store_config.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/feature_store_offline_store_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/feature_tags.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/feature_tags.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view_request.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view_request_tags.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view_request_tags.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/feature_view_tags.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view_tags.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/field.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/field.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/lock_feature_store_request.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/lock_feature_store_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/metadata.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/metadata.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/offline_store_config.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/offline_store_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/offline_store_config_fields.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/offline_store_config_fields.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/unlock_feature_store_request.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/unlock_feature_store_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/models/upsert_feature_views_request.py` & `dominodatalab_data-5.7.1/feature_store_api_client/models/upsert_feature_views_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/feature_store_api_client/types.py` & `dominodatalab_data-5.7.1/feature_store_api_client/types.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/pyproject.toml` & `dominodatalab_data-5.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dominodatalab-data"
-version = "5.7.0"
+version = "5.7.1"
 description = "Domino Data API for interacting with Domino Data features"
 readme = "README.md"
 authors = [
     "Gabriel Haim <gabriel.haim@dominodatalab.com>",
     "Aaron Read <aaron.read@dominodatalab.com>",
 ]
 license = "Apache Software License 2.0"
@@ -36,24 +36,25 @@
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
 
-[tool.poetry.group.main.dependencies]
+[tool.poetry.dependencies]
 python = "^3.8"
 pandas = ">=1.3.0"
 httpx = "^0.23.0"
 attrs = ">=20.1.0,<22.0.0"
 python-dateutil = "^2.8.0"
 pyarrow = "^8.0.0"
 loguru = "^0.5.3"
 backoff = "^1.11.1"
 bson = "^0.5.10"
+urllib3 = "^1.26.16"
 
 [tool.poetry.group.dev.dependencies]
 Sphinx = "^5.3.0"
 bandit = "^1.7.5"
 black = {version = "^22.12.0", allow-prereleases = true}
 darglint = "^1.8.1"
 flake8 = "^4.0.1"
@@ -69,16 +70,17 @@
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 pytest-recording = "^0.12.2"
 pyupgrade = "^2.38.4"
 respx = "^0.20.1"
 safety = "^2.3.5"
 sphinx-rtd-theme = "^1.2.2"
-types-PyYAML = "^6.0.12.10"
-types-python-dateutil = "^2.8.19.13"
+types-PyYAML = "^6.0.12.11"
+types-python-dateutil = "^2.8.19.14"
+vcrpy = "^5.0.0"
 
 [tool.poetry.group.featurestore.dependencies]
 feast = "^0.29.0"
 GitPython = "^3.1.31"
 
 [tool.black]
 # https://github.com/psf/black
```

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/api/default/delete_training_set_name.py` & `dominodatalab_data-5.7.1/training_set_api_client/api/default/delete_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/api/default/delete_training_set_name_number.py` & `dominodatalab_data-5.7.1/training_set_api_client/api/default/delete_training_set_name_number.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/api/default/get_training_set_name.py` & `dominodatalab_data-5.7.1/training_set_api_client/api/default/get_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/api/default/get_training_set_name_number.py` & `dominodatalab_data-5.7.1/training_set_api_client/api/default/get_training_set_name_number.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/api/default/post_find.py` & `dominodatalab_data-5.7.1/training_set_api_client/api/default/post_find.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/api/default/post_training_set_name.py` & `dominodatalab_data-5.7.1/training_set_api_client/api/default/post_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/api/default/post_version_find.py` & `dominodatalab_data-5.7.1/training_set_api_client/api/default/post_version_find.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/api/default/put_training_set_name.py` & `dominodatalab_data-5.7.1/training_set_api_client/api/default/put_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/api/default/put_training_set_name_number.py` & `dominodatalab_data-5.7.1/training_set_api_client/api/default/put_training_set_name_number.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/client.py` & `dominodatalab_data-5.7.1/training_set_api_client/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/__init__.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/create_training_set_version_request.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/create_training_set_version_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/create_training_set_version_request_meta.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/create_training_set_version_request_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/monitoring_meta.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/monitoring_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/training_set.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/training_set.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_filter.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_filter.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_filter_meta.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_filter_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_meta.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_filter.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_filter.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_filter_meta.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_filter_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_filter_training_set_meta.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_filter_training_set_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/training_set_version_meta.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_request.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_request_meta.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_request_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_version_request.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_version_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/models/update_training_set_version_request_meta.py` & `dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_version_request_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/training_set_api_client/types.py` & `dominodatalab_data-5.7.1/training_set_api_client/types.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.0/PKG-INFO` & `dominodatalab_data-5.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dominodatalab-data
-Version: 5.7.0
+Version: 5.7.1
 Summary: Domino Data API for interacting with Domino Data features
 Home-page: https://github.com/dominodatalab/domino-data
 License: Apache Software License 2.0
 Author: Gabriel Haim
 Author-email: gabriel.haim@dominodatalab.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,14 +22,15 @@
 Requires-Dist: backoff (>=1.11.1,<2.0.0)
 Requires-Dist: bson (>=0.5.10,<0.6.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Requires-Dist: pandas (>=1.3.0)
 Requires-Dist: pyarrow (>=8.0.0,<9.0.0)
 Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
+Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Repository, https://github.com/dominodatalab/domino-data
 Description-Content-Type: text/markdown
 
 # Domino Data API
 
 <div align="center">
```

