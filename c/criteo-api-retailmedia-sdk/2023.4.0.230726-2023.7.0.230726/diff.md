# Comparing `tmp/criteo-api-retailmedia-sdk-2023.4.0.230726.tar.gz` & `tmp/criteo-api-retailmedia-sdk-2023.7.0.230726.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criteo-api-retailmedia-sdk-2023.4.0.230726.tar", last modified: Wed Jul 26 09:57:01 2023, max compression
+gzip compressed data, was "criteo-api-retailmedia-sdk-2023.7.0.230726.tar", last modified: Wed Jul 26 09:57:14 2023, max compression
```

## Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726.tar` & `criteo-api-retailmedia-sdk-2023.7.0.230726.tar`

### file list

```diff
@@ -1,219 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:01.122664 criteo-api-retailmedia-sdk-2023.4.0.230726/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-26 09:57:01.122664 criteo-api-retailmedia-sdk-2023.4.0.230726/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:01.062664 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-26 09:57:01.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-07-26 09:57:01.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:57:01.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 09:57:01.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 09:57:01.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:01.066664 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:01.070664 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/api/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21710 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/api/analytics_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/api/audience_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   369289 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/api/campaign_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/api/gateway_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39220 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/api_client_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:01.070664 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16722 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/criteo_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/criteo_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/criteo_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/flow_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:01.122664 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/add_to_basket_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11868 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/application_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/application_summary_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12514 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/application_summary_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/asset_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12332 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/asset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/auction_line_item_create_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12773 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/auction_line_item_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/auction_line_item_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/auction_line_item_update_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/audience_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11836 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/audience_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/audience_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11582 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/bad_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/balance202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/campaign_attributes_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    18458 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/category202204.py
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/category202204_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/choice_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/choice_variable_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/choice_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/color_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/common_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/common_line_item_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/common_line_item_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/common_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/common_status_code_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/common_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    13465 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_user_behavior_segment_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/creative202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/creative202110_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/creative202210.py
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/creative202210_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/creative202210_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/creative_create_model202207.py
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/creative_update_model202207.py
--rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/customer_list_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/editable_campaign_attributes_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/envelope_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/envelope_report_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    16676 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_auction_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    15320 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_create_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_audience_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_audience_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_balance202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_common_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_keyword_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_line_item_capping202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_line_item_page202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_line_item_page_category202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    16309 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_create_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_promoted_product202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_retailer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_retailer_pages202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_store_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_store_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/files_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    12744 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/files_variables_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/get_page_of_audiences_by_account_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/hyperlink_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/input_resource_of_auction_line_item_create_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/input_resource_of_preferred_line_item_create_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12133 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_account_and_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12948 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    13156 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_retailer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_request_of_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12892 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/keyword_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/keyword_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11793 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/map_string.py
--rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/page_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/page_type_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/post_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/preferred_line_item_create_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/preferred_line_item_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/problem_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/promoted_product202110_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/promoted_product202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/put_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    15943 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/report_request_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/report_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/report_status_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_balance202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_balance_campaign202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_category202204.py
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_common_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_creative202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_creative202210.py
--rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_promoted_product202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12445 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keyword_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_input_keywords_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keyword_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_problem_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12910 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_resource_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11890 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/section.py
--rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/store_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/store_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/store_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/template_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/template_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/template_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/template_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11589 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/text_variable_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11476 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/text_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/user_behavior_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/user_behavior_details_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12114 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_keyword_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    82565 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:01.122664 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/models/
--rw-r--r--   0 runner    (1001) docker     (123)    21283 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14242 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 09:57:01.122664 criteo-api-retailmedia-sdk-2023.4.0.230726/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:01.122664 criteo-api-retailmedia-sdk-2023.4.0.230726/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230726/test/test_gateway_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:14.690614 criteo-api-retailmedia-sdk-2023.7.0.230726/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-26 09:57:14.690614 criteo-api-retailmedia-sdk-2023.7.0.230726/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16773 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:14.662614 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-26 09:57:14.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15284 2023-07-26 09:57:14.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:57:14.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 09:57:14.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 09:57:14.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:14.666614 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:14.666614 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/api/analytics_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/api/audience_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   369289 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/api/campaign_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/api/gateway_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39252 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/api_client_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:14.666614 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16722 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/criteo_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/criteo_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/criteo_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/flow_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:14.690614 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/add_to_basket_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11868 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/add_to_basket_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/add_to_basket_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/application_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/application_summary_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12514 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/application_summary_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/asset_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12332 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/asset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/async_report_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/auction_line_item_create_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12773 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/auction_line_item_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/auction_line_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/auction_line_item_update_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/audience_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11836 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/audience_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/audience_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/balance202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/balance_campaign202110_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/balance_campaign202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/campaign_attributes_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/campaign_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/campaign_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/campaign_report_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18458 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/category202204.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/category202204_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/choice_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/choice_variable_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/choice_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/color_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/common_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/common_line_item_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/common_line_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/common_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/common_status_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/common_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13465 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_v2_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_v2_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_v2_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_user_behavior_segment_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/creative202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/creative202110_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/creative202210.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/creative202210_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/creative202210_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/creative_create_model202207.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/creative_update_model202207.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11538 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/customer_list_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/editable_campaign_attributes_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/export_report_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/export_report_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_add_to_basket_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_add_to_basket_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16676 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_auction_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15320 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_auction_line_item_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_auction_line_item_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11662 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_audience_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_audience_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14390 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_balance202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_common_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_keyword_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_line_item_capping202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_line_item_page202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_line_item_page_category202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16309 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_preferred_line_item202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_preferred_line_item_create_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_preferred_line_item_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_promoted_product202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_retailer_pages202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_store_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_store_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/files_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12744 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/files_variables_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/get_page_of_audiences_by_account_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/hyperlink_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/input_resource_of_auction_line_item_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/input_resource_of_preferred_line_item_create_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12133 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_account_and_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_page_response_of_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12948 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_page_response_of_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13156 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_page_response_of_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_page_response_of_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_request_of_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_single_response_of_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_single_response_of_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12892 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_single_response_of_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/keyword_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/keyword_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11793 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/line_item_bid_multipliers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/line_item_bid_multipliers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16441 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/line_item_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/line_item_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/line_item_report_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/page_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/page_type_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/post_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/preferred_line_item202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/preferred_line_item202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/preferred_line_item_create_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/preferred_line_item_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/promoted_product202110_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/promoted_product202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/put_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/report_data_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11924 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/report_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/report_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_auction_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_auction_line_item_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_balance202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_balance_campaign202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_category202204.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_common_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_creative202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12129 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_creative202210.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_preferred_line_item202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_preferred_line_item_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_promoted_product202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12445 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_audience_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_audience_v2_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_audience_v2_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_audience_v2_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_add_remove_keyword_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_add_remove_keywords_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_add_remove_keywords_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_add_remove_keywords_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12109 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_input_keywords_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_keyword_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_keywords_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_keywords_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_keywords_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_proposal_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_proposal_status_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12910 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_proposal_status_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_resource_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_set_bid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_set_bids_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11890 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_set_bids_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_set_bids_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12996 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12018 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/status_response_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/store_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/store_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/store_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/template_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/template_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/template_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/template_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11589 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/text_variable_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11476 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/text_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/user_behavior_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/user_behavior_details_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12114 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/value_type_resource_of_add_to_basket_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/value_type_resource_of_audience_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/value_type_resource_of_audience_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/value_type_resource_of_keyword_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/value_type_resource_of_store_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/value_type_resource_of_store_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82565 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:14.690614 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    21809 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14242 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 09:57:14.690614 criteo-api-retailmedia-sdk-2023.7.0.230726/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:57:14.690614 criteo-api-retailmedia-sdk-2023.7.0.230726/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-26 09:54:50.000000 criteo-api-retailmedia-sdk-2023.7.0.230726/test/test_gateway_api.py
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/PKG-INFO` & `criteo-api-retailmedia-sdk-2023.7.0.230726/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-retailmedia-sdk
-Version: 2023.4.0.230726
+Version: 2023.7.0.230726
 Summary: Criteo API SDK
 Home-page: https://github.com/criteo/criteo-api-python-sdk
 Author: Criteo
 Author-email: 
 Keywords: Criteo,OpenAPI-Generator,Criteo API SDK
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,21 +20,21 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-retailmedia-sdk==2023.04.0.230726
+pip install criteo-api-retailmedia-sdk==2023.07.0.230726
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230726`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.07.0.230726`)
 
 Then import the package:
 ```python
-import criteo_api_retailmedia_v2023_04
+import criteo_api_retailmedia_v2023_07
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/README.md` & `criteo-api-retailmedia-sdk-2023.7.0.230726/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,45 +4,45 @@
 API Client Libraries can facilitate your use of the Criteo API allowing you to build unique and customized solutions to serve your businesses and clients.
 These libraries can reduce the amount of code you need to write in order to start accessing Criteo programmatically. They also can help expedite troubleshooting, should you encounter any issues.
 
 More information: [https://developers.criteo.com/](https://developers.criteo.com/)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- Package version: 2023.04.0.230726
+- Package version: 2023.07.0.230726
 
 ## Requirements
 
 Python 2.7 and 3.5+
 
 ## Installation & Usage
 ### pip install
 
 ```sh
-pip install criteo-api-retailmedia-sdk==2023.04.0.230726
+pip install criteo-api-retailmedia-sdk==2023.07.0.230726
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230726`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.07.0.230726`)
 
 Then import the package:
 ```python
-import criteo_api_retailmedia_v2023_04
+import criteo_api_retailmedia_v2023_07
 ```
 
 ### Manual Installation using [Setuptools](http://pypi.python.org/pypi/setuptools)
 
 Download the code or clone the repository locally, then execute the following command:
 
 ```sh
 python setup.py install --user
 ```
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
-import criteo_api_retailmedia_v2023_04
+import criteo_api_retailmedia_v2023_07
 ```
 
 ## Example
 There are multiple examples for the different OAuth flows that the SDK supports.
 - See [test/example_application_with_client_credentials.py](test/example_application_with_client_credentials.py) for an example with Client Credentials.
 - See [test/example_application_with_auth_code.py](test/example_application_with_auth_code.py) for an example with Authorization Code.
 Once you follow the authorization code flow, you will have a refresh token that has to be used to regenerate access token for future usage. 
@@ -65,26 +65,29 @@
  - [AddToBasketTarget202110Response](docs/AddToBasketTarget202110Response.md)
  - [ApplicationSummaryModel](docs/ApplicationSummaryModel.md)
  - [ApplicationSummaryModelResource](docs/ApplicationSummaryModelResource.md)
  - [ApplicationSummaryModelResponse](docs/ApplicationSummaryModelResponse.md)
  - [Asset](docs/Asset.md)
  - [AssetResource](docs/AssetResource.md)
  - [AssetResponse](docs/AssetResponse.md)
+ - [AsyncReportResponse](docs/AsyncReportResponse.md)
  - [AuctionLineItemCreateModelRequest](docs/AuctionLineItemCreateModelRequest.md)
  - [AuctionLineItemPagedListResponse](docs/AuctionLineItemPagedListResponse.md)
  - [AuctionLineItemResponse](docs/AuctionLineItemResponse.md)
  - [AuctionLineItemUpdateModelRequest](docs/AuctionLineItemUpdateModelRequest.md)
  - [AudienceIdsUpdateModel202110Request](docs/AudienceIdsUpdateModel202110Request.md)
  - [AudienceTarget202110Request](docs/AudienceTarget202110Request.md)
  - [AudienceTarget202110Response](docs/AudienceTarget202110Response.md)
- - [BadRequest](docs/BadRequest.md)
  - [Balance202110PagedListResponse](docs/Balance202110PagedListResponse.md)
  - [BalanceCampaign202110ListRequest](docs/BalanceCampaign202110ListRequest.md)
  - [BalanceCampaign202110PagedListResponse](docs/BalanceCampaign202110PagedListResponse.md)
  - [CampaignAttributesV202301](docs/CampaignAttributesV202301.md)
+ - [CampaignReport](docs/CampaignReport.md)
+ - [CampaignReportRequest](docs/CampaignReportRequest.md)
+ - [CampaignReportResource](docs/CampaignReportResource.md)
  - [CampaignV202301](docs/CampaignV202301.md)
  - [Category202204](docs/Category202204.md)
  - [Category202204ListResponse](docs/Category202204ListResponse.md)
  - [ChoiceOption](docs/ChoiceOption.md)
  - [ChoiceVariableSpecification](docs/ChoiceVariableSpecification.md)
  - [ChoiceVariableValue](docs/ChoiceVariableValue.md)
  - [ColorVariableValue](docs/ColorVariableValue.md)
@@ -109,17 +112,16 @@
  - [Creative202210](docs/Creative202210.md)
  - [Creative202210ListResponse](docs/Creative202210ListResponse.md)
  - [Creative202210Response](docs/Creative202210Response.md)
  - [CreativeCreateModel202207](docs/CreativeCreateModel202207.md)
  - [CreativeUpdateModel202207](docs/CreativeUpdateModel202207.md)
  - [CustomerListDetails](docs/CustomerListDetails.md)
  - [EditableCampaignAttributesV202301](docs/EditableCampaignAttributesV202301.md)
- - [EnvelopeReportRequest](docs/EnvelopeReportRequest.md)
- - [EnvelopeReportStatus](docs/EnvelopeReportStatus.md)
- - [Error](docs/Error.md)
+ - [ExportReportColumn](docs/ExportReportColumn.md)
+ - [ExportReportMetaData](docs/ExportReportMetaData.md)
  - [ExternalAccount](docs/ExternalAccount.md)
  - [ExternalAddToBasketIdsUpdateModel202110](docs/ExternalAddToBasketIdsUpdateModel202110.md)
  - [ExternalAddToBasketTarget202110](docs/ExternalAddToBasketTarget202110.md)
  - [ExternalAuctionLineItem](docs/ExternalAuctionLineItem.md)
  - [ExternalAuctionLineItemCreateModel](docs/ExternalAuctionLineItemCreateModel.md)
  - [ExternalAuctionLineItemUpdateModel](docs/ExternalAuctionLineItemUpdateModel.md)
  - [ExternalAudienceIdsUpdateModel202110](docs/ExternalAudienceIdsUpdateModel202110.md)
@@ -165,30 +167,31 @@
  - [JsonApiSingleResponseOfCatalogStatus](docs/JsonApiSingleResponseOfCatalogStatus.md)
  - [JsonApiSingleResponseOfLineItemBidMultipliers](docs/JsonApiSingleResponseOfLineItemBidMultipliers.md)
  - [KeywordTarget202110Request](docs/KeywordTarget202110Request.md)
  - [KeywordTarget202110Response](docs/KeywordTarget202110Response.md)
  - [LineItemBidMultipliers](docs/LineItemBidMultipliers.md)
  - [LineItemBidMultipliersRequest](docs/LineItemBidMultipliersRequest.md)
  - [LineItemBidMultipliersResponse](docs/LineItemBidMultipliersResponse.md)
- - [MapString](docs/MapString.md)
+ - [LineItemReport](docs/LineItemReport.md)
+ - [LineItemReportRequest](docs/LineItemReportRequest.md)
+ - [LineItemReportResource](docs/LineItemReportResource.md)
  - [PageMetadata](docs/PageMetadata.md)
  - [PageTypeEnvironment](docs/PageTypeEnvironment.md)
  - [PostCampaignV202301](docs/PostCampaignV202301.md)
  - [PreferredLineItem202110PagedListResponse](docs/PreferredLineItem202110PagedListResponse.md)
  - [PreferredLineItem202110Response](docs/PreferredLineItem202110Response.md)
  - [PreferredLineItemCreateModel202110Request](docs/PreferredLineItemCreateModel202110Request.md)
  - [PreferredLineItemUpdateModel202110Request](docs/PreferredLineItemUpdateModel202110Request.md)
  - [ProblemDetails](docs/ProblemDetails.md)
  - [PromotedProduct202110ListRequest](docs/PromotedProduct202110ListRequest.md)
  - [PromotedProduct202110PagedListResponse](docs/PromotedProduct202110PagedListResponse.md)
  - [PutCampaignV202301](docs/PutCampaignV202301.md)
- - [ReportRequest](docs/ReportRequest.md)
- - [ReportRequestAttributes](docs/ReportRequestAttributes.md)
- - [ReportStatus](docs/ReportStatus.md)
- - [ReportStatusAttributes](docs/ReportStatusAttributes.md)
+ - [ReportDataResponseResource](docs/ReportDataResponseResource.md)
+ - [ReportOutcome](docs/ReportOutcome.md)
+ - [ReportResponse](docs/ReportResponse.md)
  - [ResourceOfAuctionLineItem](docs/ResourceOfAuctionLineItem.md)
  - [ResourceOfAuctionLineItemUpdateModel](docs/ResourceOfAuctionLineItemUpdateModel.md)
  - [ResourceOfBalance202110](docs/ResourceOfBalance202110.md)
  - [ResourceOfBalanceCampaign202110](docs/ResourceOfBalanceCampaign202110.md)
  - [ResourceOfCategory202204](docs/ResourceOfCategory202204.md)
  - [ResourceOfCommonLineItem](docs/ResourceOfCommonLineItem.md)
  - [ResourceOfCreative202110](docs/ResourceOfCreative202110.md)
@@ -219,14 +222,16 @@
  - [RetailMediaExternalv1ProposalStatusModelResponse](docs/RetailMediaExternalv1ProposalStatusModelResponse.md)
  - [RetailMediaExternalv1ResourceOutcome](docs/RetailMediaExternalv1ResourceOutcome.md)
  - [RetailMediaExternalv1SetBidModel](docs/RetailMediaExternalv1SetBidModel.md)
  - [RetailMediaExternalv1SetBidsModel](docs/RetailMediaExternalv1SetBidsModel.md)
  - [RetailMediaExternalv1SetBidsModelRequest](docs/RetailMediaExternalv1SetBidsModelRequest.md)
  - [RetailMediaExternalv1SetBidsModelResource](docs/RetailMediaExternalv1SetBidsModelResource.md)
  - [Section](docs/Section.md)
+ - [StatusResponse](docs/StatusResponse.md)
+ - [StatusResponseResource](docs/StatusResponseResource.md)
  - [StoreIdsUpdateModel202110Request](docs/StoreIdsUpdateModel202110Request.md)
  - [StoreTarget202110Request](docs/StoreTarget202110Request.md)
  - [StoreTarget202110Response](docs/StoreTarget202110Response.md)
  - [Template](docs/Template.md)
  - [TemplateListResponse](docs/TemplateListResponse.md)
  - [TemplateResponse](docs/TemplateResponse.md)
  - [TemplateVariable](docs/TemplateVariable.md)
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_sdk.egg-info/PKG-INFO` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-retailmedia-sdk
-Version: 2023.4.0.230726
+Version: 2023.7.0.230726
 Summary: Criteo API SDK
 Home-page: https://github.com/criteo/criteo-api-python-sdk
 Author: Criteo
 Author-email: 
 Keywords: Criteo,OpenAPI-Generator,Criteo API SDK
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,21 +20,21 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-retailmedia-sdk==2023.04.0.230726
+pip install criteo-api-retailmedia-sdk==2023.07.0.230726
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230726`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.07.0.230726`)
 
 Then import the package:
 ```python
-import criteo_api_retailmedia_v2023_04
+import criteo_api_retailmedia_v2023_07
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,209 +2,214 @@
 setup.cfg
 setup.py
 criteo_api_retailmedia_sdk.egg-info/PKG-INFO
 criteo_api_retailmedia_sdk.egg-info/SOURCES.txt
 criteo_api_retailmedia_sdk.egg-info/dependency_links.txt
 criteo_api_retailmedia_sdk.egg-info/requires.txt
 criteo_api_retailmedia_sdk.egg-info/top_level.txt
-criteo_api_retailmedia_v2023_04/__init__.py
-criteo_api_retailmedia_v2023_04/api_client.py
-criteo_api_retailmedia_v2023_04/api_client_builder.py
-criteo_api_retailmedia_v2023_04/configuration.py
-criteo_api_retailmedia_v2023_04/criteo_api_client.py
-criteo_api_retailmedia_v2023_04/criteo_auth.py
-criteo_api_retailmedia_v2023_04/criteo_rest.py
-criteo_api_retailmedia_v2023_04/exceptions.py
-criteo_api_retailmedia_v2023_04/flow_constants.py
-criteo_api_retailmedia_v2023_04/model_utils.py
-criteo_api_retailmedia_v2023_04/rest.py
-criteo_api_retailmedia_v2023_04/api/__init__.py
-criteo_api_retailmedia_v2023_04/api/analytics_api.py
-criteo_api_retailmedia_v2023_04/api/audience_api.py
-criteo_api_retailmedia_v2023_04/api/campaign_api.py
-criteo_api_retailmedia_v2023_04/api/gateway_api.py
-criteo_api_retailmedia_v2023_04/apis/__init__.py
-criteo_api_retailmedia_v2023_04/model/__init__.py
-criteo_api_retailmedia_v2023_04/model/add_to_basket_ids_update_model202110_request.py
-criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_request.py
-criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_response.py
-criteo_api_retailmedia_v2023_04/model/application_summary_model.py
-criteo_api_retailmedia_v2023_04/model/application_summary_model_resource.py
-criteo_api_retailmedia_v2023_04/model/application_summary_model_response.py
-criteo_api_retailmedia_v2023_04/model/asset.py
-criteo_api_retailmedia_v2023_04/model/asset_resource.py
-criteo_api_retailmedia_v2023_04/model/asset_response.py
-criteo_api_retailmedia_v2023_04/model/auction_line_item_create_model_request.py
-criteo_api_retailmedia_v2023_04/model/auction_line_item_paged_list_response.py
-criteo_api_retailmedia_v2023_04/model/auction_line_item_response.py
-criteo_api_retailmedia_v2023_04/model/auction_line_item_update_model_request.py
-criteo_api_retailmedia_v2023_04/model/audience_ids_update_model202110_request.py
-criteo_api_retailmedia_v2023_04/model/audience_target202110_request.py
-criteo_api_retailmedia_v2023_04/model/audience_target202110_response.py
-criteo_api_retailmedia_v2023_04/model/bad_request.py
-criteo_api_retailmedia_v2023_04/model/balance202110_paged_list_response.py
-criteo_api_retailmedia_v2023_04/model/balance_campaign202110_list_request.py
-criteo_api_retailmedia_v2023_04/model/balance_campaign202110_paged_list_response.py
-criteo_api_retailmedia_v2023_04/model/campaign_attributes_v202301.py
-criteo_api_retailmedia_v2023_04/model/campaign_v202301.py
-criteo_api_retailmedia_v2023_04/model/category202204.py
-criteo_api_retailmedia_v2023_04/model/category202204_list_response.py
-criteo_api_retailmedia_v2023_04/model/choice_option.py
-criteo_api_retailmedia_v2023_04/model/choice_variable_specification.py
-criteo_api_retailmedia_v2023_04/model/choice_variable_value.py
-criteo_api_retailmedia_v2023_04/model/color_variable_value.py
-criteo_api_retailmedia_v2023_04/model/common_error.py
-criteo_api_retailmedia_v2023_04/model/common_line_item_paged_list_response.py
-criteo_api_retailmedia_v2023_04/model/common_line_item_response.py
-criteo_api_retailmedia_v2023_04/model/common_problem.py
-criteo_api_retailmedia_v2023_04/model/common_status_code_response.py
-criteo_api_retailmedia_v2023_04/model/common_warning.py
-criteo_api_retailmedia_v2023_04/model/create_retail_media_audience.py
-criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_attributes.py
-criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_body.py
-criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_request.py
-criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_response.py
-criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2.py
-criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_attributes.py
-criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_data.py
-criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_request.py
-criteo_api_retailmedia_v2023_04/model/create_user_behavior_segment_v2.py
-criteo_api_retailmedia_v2023_04/model/creative202110.py
-criteo_api_retailmedia_v2023_04/model/creative202110_list_response.py
-criteo_api_retailmedia_v2023_04/model/creative202210.py
-criteo_api_retailmedia_v2023_04/model/creative202210_list_response.py
-criteo_api_retailmedia_v2023_04/model/creative202210_response.py
-criteo_api_retailmedia_v2023_04/model/creative_create_model202207.py
-criteo_api_retailmedia_v2023_04/model/creative_update_model202207.py
-criteo_api_retailmedia_v2023_04/model/customer_list_details.py
-criteo_api_retailmedia_v2023_04/model/editable_campaign_attributes_v202301.py
-criteo_api_retailmedia_v2023_04/model/envelope_report_request.py
-criteo_api_retailmedia_v2023_04/model/envelope_report_status.py
-criteo_api_retailmedia_v2023_04/model/error.py
-criteo_api_retailmedia_v2023_04/model/external_account.py
-criteo_api_retailmedia_v2023_04/model/external_add_to_basket_ids_update_model202110.py
-criteo_api_retailmedia_v2023_04/model/external_add_to_basket_target202110.py
-criteo_api_retailmedia_v2023_04/model/external_auction_line_item.py
-criteo_api_retailmedia_v2023_04/model/external_auction_line_item_create_model.py
-criteo_api_retailmedia_v2023_04/model/external_auction_line_item_update_model.py
-criteo_api_retailmedia_v2023_04/model/external_audience_ids_update_model202110.py
-criteo_api_retailmedia_v2023_04/model/external_audience_target202110.py
-criteo_api_retailmedia_v2023_04/model/external_balance202110.py
-criteo_api_retailmedia_v2023_04/model/external_brand.py
-criteo_api_retailmedia_v2023_04/model/external_catalog_request.py
-criteo_api_retailmedia_v2023_04/model/external_catalog_status.py
-criteo_api_retailmedia_v2023_04/model/external_common_line_item.py
-criteo_api_retailmedia_v2023_04/model/external_keyword_target202110.py
-criteo_api_retailmedia_v2023_04/model/external_line_item_capping202110.py
-criteo_api_retailmedia_v2023_04/model/external_line_item_page202110.py
-criteo_api_retailmedia_v2023_04/model/external_line_item_page_category202110.py
-criteo_api_retailmedia_v2023_04/model/external_preferred_line_item202110.py
-criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_create_model202110.py
-criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_update_model202110.py
-criteo_api_retailmedia_v2023_04/model/external_promoted_product202110.py
-criteo_api_retailmedia_v2023_04/model/external_retailer.py
-criteo_api_retailmedia_v2023_04/model/external_retailer_pages202110.py
-criteo_api_retailmedia_v2023_04/model/external_store_ids_update_model202110.py
-criteo_api_retailmedia_v2023_04/model/external_store_target202110.py
-criteo_api_retailmedia_v2023_04/model/files_variable_value.py
-criteo_api_retailmedia_v2023_04/model/files_variables_specification.py
-criteo_api_retailmedia_v2023_04/model/get_page_of_audiences_by_account_id_response.py
-criteo_api_retailmedia_v2023_04/model/hyperlink_variable_value.py
-criteo_api_retailmedia_v2023_04/model/input_resource_of_auction_line_item_create_model.py
-criteo_api_retailmedia_v2023_04/model/input_resource_of_preferred_line_item_create_model202110.py
-criteo_api_retailmedia_v2023_04/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
-criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_account_and_account.py
-criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
-criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
-criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
-criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
-criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
-criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
-criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
-criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_account.py
-criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_brand.py
-criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_campaign_v202301.py
-criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_retailer.py
-criteo_api_retailmedia_v2023_04/model/json_api_request_of_catalog_request.py
-criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_campaign_v202301.py
-criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_catalog_status.py
-criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_line_item_bid_multipliers.py
-criteo_api_retailmedia_v2023_04/model/keyword_target202110_request.py
-criteo_api_retailmedia_v2023_04/model/keyword_target202110_response.py
-criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers.py
-criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_request.py
-criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_response.py
-criteo_api_retailmedia_v2023_04/model/map_string.py
-criteo_api_retailmedia_v2023_04/model/page_metadata.py
-criteo_api_retailmedia_v2023_04/model/page_type_environment.py
-criteo_api_retailmedia_v2023_04/model/post_campaign_v202301.py
-criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_paged_list_response.py
-criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_response.py
-criteo_api_retailmedia_v2023_04/model/preferred_line_item_create_model202110_request.py
-criteo_api_retailmedia_v2023_04/model/preferred_line_item_update_model202110_request.py
-criteo_api_retailmedia_v2023_04/model/problem_details.py
-criteo_api_retailmedia_v2023_04/model/promoted_product202110_list_request.py
-criteo_api_retailmedia_v2023_04/model/promoted_product202110_paged_list_response.py
-criteo_api_retailmedia_v2023_04/model/put_campaign_v202301.py
-criteo_api_retailmedia_v2023_04/model/report_request.py
-criteo_api_retailmedia_v2023_04/model/report_request_attributes.py
-criteo_api_retailmedia_v2023_04/model/report_status.py
-criteo_api_retailmedia_v2023_04/model/report_status_attributes.py
-criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item.py
-criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item_update_model.py
-criteo_api_retailmedia_v2023_04/model/resource_of_balance202110.py
-criteo_api_retailmedia_v2023_04/model/resource_of_balance_campaign202110.py
-criteo_api_retailmedia_v2023_04/model/resource_of_category202204.py
-criteo_api_retailmedia_v2023_04/model/resource_of_common_line_item.py
-criteo_api_retailmedia_v2023_04/model/resource_of_creative202110.py
-criteo_api_retailmedia_v2023_04/model/resource_of_creative202210.py
-criteo_api_retailmedia_v2023_04/model/resource_of_line_item_bid_multipliers.py
-criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item202110.py
-criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item_update_model202110.py
-criteo_api_retailmedia_v2023_04/model/resource_of_promoted_product202110.py
-criteo_api_retailmedia_v2023_04/model/resource_of_template.py
-criteo_api_retailmedia_v2023_04/model/retail_media_audience.py
-criteo_api_retailmedia_v2023_04/model/retail_media_audience_attributes.py
-criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2.py
-criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_attributes.py
-criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_list_response.py
-criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_response.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keyword_model.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_request.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_resource.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_input_keywords_model.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keyword_data_model.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_resource.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_response.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_problem_details.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_resource.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_response.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_resource_outcome.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bid_model.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_request.py
-criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_resource.py
-criteo_api_retailmedia_v2023_04/model/section.py
-criteo_api_retailmedia_v2023_04/model/store_ids_update_model202110_request.py
-criteo_api_retailmedia_v2023_04/model/store_target202110_request.py
-criteo_api_retailmedia_v2023_04/model/store_target202110_response.py
-criteo_api_retailmedia_v2023_04/model/template.py
-criteo_api_retailmedia_v2023_04/model/template_list_response.py
-criteo_api_retailmedia_v2023_04/model/template_response.py
-criteo_api_retailmedia_v2023_04/model/template_variable.py
-criteo_api_retailmedia_v2023_04/model/template_variable_value.py
-criteo_api_retailmedia_v2023_04/model/text_variable_specification.py
-criteo_api_retailmedia_v2023_04/model/text_variable_value.py
-criteo_api_retailmedia_v2023_04/model/user_behavior_details.py
-criteo_api_retailmedia_v2023_04/model/user_behavior_details_v2.py
-criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
-criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_target202110.py
-criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_ids_update_model202110.py
-criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_target202110.py
-criteo_api_retailmedia_v2023_04/model/value_type_resource_of_keyword_target202110.py
-criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_ids_update_model202110.py
-criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_target202110.py
-criteo_api_retailmedia_v2023_04/models/__init__.py
+criteo_api_retailmedia_v2023_07/__init__.py
+criteo_api_retailmedia_v2023_07/api_client.py
+criteo_api_retailmedia_v2023_07/api_client_builder.py
+criteo_api_retailmedia_v2023_07/configuration.py
+criteo_api_retailmedia_v2023_07/criteo_api_client.py
+criteo_api_retailmedia_v2023_07/criteo_auth.py
+criteo_api_retailmedia_v2023_07/criteo_rest.py
+criteo_api_retailmedia_v2023_07/exceptions.py
+criteo_api_retailmedia_v2023_07/flow_constants.py
+criteo_api_retailmedia_v2023_07/model_utils.py
+criteo_api_retailmedia_v2023_07/rest.py
+criteo_api_retailmedia_v2023_07/api/__init__.py
+criteo_api_retailmedia_v2023_07/api/analytics_api.py
+criteo_api_retailmedia_v2023_07/api/audience_api.py
+criteo_api_retailmedia_v2023_07/api/campaign_api.py
+criteo_api_retailmedia_v2023_07/api/gateway_api.py
+criteo_api_retailmedia_v2023_07/apis/__init__.py
+criteo_api_retailmedia_v2023_07/model/__init__.py
+criteo_api_retailmedia_v2023_07/model/add_to_basket_ids_update_model202110_request.py
+criteo_api_retailmedia_v2023_07/model/add_to_basket_target202110_request.py
+criteo_api_retailmedia_v2023_07/model/add_to_basket_target202110_response.py
+criteo_api_retailmedia_v2023_07/model/application_summary_model.py
+criteo_api_retailmedia_v2023_07/model/application_summary_model_resource.py
+criteo_api_retailmedia_v2023_07/model/application_summary_model_response.py
+criteo_api_retailmedia_v2023_07/model/asset.py
+criteo_api_retailmedia_v2023_07/model/asset_resource.py
+criteo_api_retailmedia_v2023_07/model/asset_response.py
+criteo_api_retailmedia_v2023_07/model/async_report_response.py
+criteo_api_retailmedia_v2023_07/model/auction_line_item_create_model_request.py
+criteo_api_retailmedia_v2023_07/model/auction_line_item_paged_list_response.py
+criteo_api_retailmedia_v2023_07/model/auction_line_item_response.py
+criteo_api_retailmedia_v2023_07/model/auction_line_item_update_model_request.py
+criteo_api_retailmedia_v2023_07/model/audience_ids_update_model202110_request.py
+criteo_api_retailmedia_v2023_07/model/audience_target202110_request.py
+criteo_api_retailmedia_v2023_07/model/audience_target202110_response.py
+criteo_api_retailmedia_v2023_07/model/balance202110_paged_list_response.py
+criteo_api_retailmedia_v2023_07/model/balance_campaign202110_list_request.py
+criteo_api_retailmedia_v2023_07/model/balance_campaign202110_paged_list_response.py
+criteo_api_retailmedia_v2023_07/model/campaign_attributes_v202301.py
+criteo_api_retailmedia_v2023_07/model/campaign_report.py
+criteo_api_retailmedia_v2023_07/model/campaign_report_request.py
+criteo_api_retailmedia_v2023_07/model/campaign_report_resource.py
+criteo_api_retailmedia_v2023_07/model/campaign_v202301.py
+criteo_api_retailmedia_v2023_07/model/category202204.py
+criteo_api_retailmedia_v2023_07/model/category202204_list_response.py
+criteo_api_retailmedia_v2023_07/model/choice_option.py
+criteo_api_retailmedia_v2023_07/model/choice_variable_specification.py
+criteo_api_retailmedia_v2023_07/model/choice_variable_value.py
+criteo_api_retailmedia_v2023_07/model/color_variable_value.py
+criteo_api_retailmedia_v2023_07/model/common_error.py
+criteo_api_retailmedia_v2023_07/model/common_line_item_paged_list_response.py
+criteo_api_retailmedia_v2023_07/model/common_line_item_response.py
+criteo_api_retailmedia_v2023_07/model/common_problem.py
+criteo_api_retailmedia_v2023_07/model/common_status_code_response.py
+criteo_api_retailmedia_v2023_07/model/common_warning.py
+criteo_api_retailmedia_v2023_07/model/create_retail_media_audience.py
+criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_attributes.py
+criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_body.py
+criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_request.py
+criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_response.py
+criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_v2.py
+criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_v2_attributes.py
+criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_v2_data.py
+criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_v2_request.py
+criteo_api_retailmedia_v2023_07/model/create_user_behavior_segment_v2.py
+criteo_api_retailmedia_v2023_07/model/creative202110.py
+criteo_api_retailmedia_v2023_07/model/creative202110_list_response.py
+criteo_api_retailmedia_v2023_07/model/creative202210.py
+criteo_api_retailmedia_v2023_07/model/creative202210_list_response.py
+criteo_api_retailmedia_v2023_07/model/creative202210_response.py
+criteo_api_retailmedia_v2023_07/model/creative_create_model202207.py
+criteo_api_retailmedia_v2023_07/model/creative_update_model202207.py
+criteo_api_retailmedia_v2023_07/model/customer_list_details.py
+criteo_api_retailmedia_v2023_07/model/editable_campaign_attributes_v202301.py
+criteo_api_retailmedia_v2023_07/model/export_report_column.py
+criteo_api_retailmedia_v2023_07/model/export_report_meta_data.py
+criteo_api_retailmedia_v2023_07/model/external_account.py
+criteo_api_retailmedia_v2023_07/model/external_add_to_basket_ids_update_model202110.py
+criteo_api_retailmedia_v2023_07/model/external_add_to_basket_target202110.py
+criteo_api_retailmedia_v2023_07/model/external_auction_line_item.py
+criteo_api_retailmedia_v2023_07/model/external_auction_line_item_create_model.py
+criteo_api_retailmedia_v2023_07/model/external_auction_line_item_update_model.py
+criteo_api_retailmedia_v2023_07/model/external_audience_ids_update_model202110.py
+criteo_api_retailmedia_v2023_07/model/external_audience_target202110.py
+criteo_api_retailmedia_v2023_07/model/external_balance202110.py
+criteo_api_retailmedia_v2023_07/model/external_brand.py
+criteo_api_retailmedia_v2023_07/model/external_catalog_request.py
+criteo_api_retailmedia_v2023_07/model/external_catalog_status.py
+criteo_api_retailmedia_v2023_07/model/external_common_line_item.py
+criteo_api_retailmedia_v2023_07/model/external_keyword_target202110.py
+criteo_api_retailmedia_v2023_07/model/external_line_item_capping202110.py
+criteo_api_retailmedia_v2023_07/model/external_line_item_page202110.py
+criteo_api_retailmedia_v2023_07/model/external_line_item_page_category202110.py
+criteo_api_retailmedia_v2023_07/model/external_preferred_line_item202110.py
+criteo_api_retailmedia_v2023_07/model/external_preferred_line_item_create_model202110.py
+criteo_api_retailmedia_v2023_07/model/external_preferred_line_item_update_model202110.py
+criteo_api_retailmedia_v2023_07/model/external_promoted_product202110.py
+criteo_api_retailmedia_v2023_07/model/external_retailer.py
+criteo_api_retailmedia_v2023_07/model/external_retailer_pages202110.py
+criteo_api_retailmedia_v2023_07/model/external_store_ids_update_model202110.py
+criteo_api_retailmedia_v2023_07/model/external_store_target202110.py
+criteo_api_retailmedia_v2023_07/model/files_variable_value.py
+criteo_api_retailmedia_v2023_07/model/files_variables_specification.py
+criteo_api_retailmedia_v2023_07/model/get_page_of_audiences_by_account_id_response.py
+criteo_api_retailmedia_v2023_07/model/hyperlink_variable_value.py
+criteo_api_retailmedia_v2023_07/model/input_resource_of_auction_line_item_create_model.py
+criteo_api_retailmedia_v2023_07/model/input_resource_of_preferred_line_item_create_model202110.py
+criteo_api_retailmedia_v2023_07/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
+criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_account_and_account.py
+criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
+criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
+criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
+criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
+criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
+criteo_api_retailmedia_v2023_07/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
+criteo_api_retailmedia_v2023_07/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
+criteo_api_retailmedia_v2023_07/model/json_api_page_response_of_account.py
+criteo_api_retailmedia_v2023_07/model/json_api_page_response_of_brand.py
+criteo_api_retailmedia_v2023_07/model/json_api_page_response_of_campaign_v202301.py
+criteo_api_retailmedia_v2023_07/model/json_api_page_response_of_retailer.py
+criteo_api_retailmedia_v2023_07/model/json_api_request_of_catalog_request.py
+criteo_api_retailmedia_v2023_07/model/json_api_single_response_of_campaign_v202301.py
+criteo_api_retailmedia_v2023_07/model/json_api_single_response_of_catalog_status.py
+criteo_api_retailmedia_v2023_07/model/json_api_single_response_of_line_item_bid_multipliers.py
+criteo_api_retailmedia_v2023_07/model/keyword_target202110_request.py
+criteo_api_retailmedia_v2023_07/model/keyword_target202110_response.py
+criteo_api_retailmedia_v2023_07/model/line_item_bid_multipliers.py
+criteo_api_retailmedia_v2023_07/model/line_item_bid_multipliers_request.py
+criteo_api_retailmedia_v2023_07/model/line_item_bid_multipliers_response.py
+criteo_api_retailmedia_v2023_07/model/line_item_report.py
+criteo_api_retailmedia_v2023_07/model/line_item_report_request.py
+criteo_api_retailmedia_v2023_07/model/line_item_report_resource.py
+criteo_api_retailmedia_v2023_07/model/page_metadata.py
+criteo_api_retailmedia_v2023_07/model/page_type_environment.py
+criteo_api_retailmedia_v2023_07/model/post_campaign_v202301.py
+criteo_api_retailmedia_v2023_07/model/preferred_line_item202110_paged_list_response.py
+criteo_api_retailmedia_v2023_07/model/preferred_line_item202110_response.py
+criteo_api_retailmedia_v2023_07/model/preferred_line_item_create_model202110_request.py
+criteo_api_retailmedia_v2023_07/model/preferred_line_item_update_model202110_request.py
+criteo_api_retailmedia_v2023_07/model/problem_details.py
+criteo_api_retailmedia_v2023_07/model/promoted_product202110_list_request.py
+criteo_api_retailmedia_v2023_07/model/promoted_product202110_paged_list_response.py
+criteo_api_retailmedia_v2023_07/model/put_campaign_v202301.py
+criteo_api_retailmedia_v2023_07/model/report_data_response_resource.py
+criteo_api_retailmedia_v2023_07/model/report_outcome.py
+criteo_api_retailmedia_v2023_07/model/report_response.py
+criteo_api_retailmedia_v2023_07/model/resource_of_auction_line_item.py
+criteo_api_retailmedia_v2023_07/model/resource_of_auction_line_item_update_model.py
+criteo_api_retailmedia_v2023_07/model/resource_of_balance202110.py
+criteo_api_retailmedia_v2023_07/model/resource_of_balance_campaign202110.py
+criteo_api_retailmedia_v2023_07/model/resource_of_category202204.py
+criteo_api_retailmedia_v2023_07/model/resource_of_common_line_item.py
+criteo_api_retailmedia_v2023_07/model/resource_of_creative202110.py
+criteo_api_retailmedia_v2023_07/model/resource_of_creative202210.py
+criteo_api_retailmedia_v2023_07/model/resource_of_line_item_bid_multipliers.py
+criteo_api_retailmedia_v2023_07/model/resource_of_preferred_line_item202110.py
+criteo_api_retailmedia_v2023_07/model/resource_of_preferred_line_item_update_model202110.py
+criteo_api_retailmedia_v2023_07/model/resource_of_promoted_product202110.py
+criteo_api_retailmedia_v2023_07/model/resource_of_template.py
+criteo_api_retailmedia_v2023_07/model/retail_media_audience.py
+criteo_api_retailmedia_v2023_07/model/retail_media_audience_attributes.py
+criteo_api_retailmedia_v2023_07/model/retail_media_audience_v2.py
+criteo_api_retailmedia_v2023_07/model/retail_media_audience_v2_attributes.py
+criteo_api_retailmedia_v2023_07/model/retail_media_audience_v2_list_response.py
+criteo_api_retailmedia_v2023_07/model/retail_media_audience_v2_response.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_add_remove_keyword_model.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_add_remove_keywords_model.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_add_remove_keywords_model_request.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_add_remove_keywords_model_resource.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_input_keywords_model.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_keyword_data_model.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_keywords_model.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_keywords_model_resource.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_keywords_model_response.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_problem_details.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_proposal_status_model.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_proposal_status_model_resource.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_proposal_status_model_response.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_resource_outcome.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_set_bid_model.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_set_bids_model.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_set_bids_model_request.py
+criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_set_bids_model_resource.py
+criteo_api_retailmedia_v2023_07/model/section.py
+criteo_api_retailmedia_v2023_07/model/status_response.py
+criteo_api_retailmedia_v2023_07/model/status_response_resource.py
+criteo_api_retailmedia_v2023_07/model/store_ids_update_model202110_request.py
+criteo_api_retailmedia_v2023_07/model/store_target202110_request.py
+criteo_api_retailmedia_v2023_07/model/store_target202110_response.py
+criteo_api_retailmedia_v2023_07/model/template.py
+criteo_api_retailmedia_v2023_07/model/template_list_response.py
+criteo_api_retailmedia_v2023_07/model/template_response.py
+criteo_api_retailmedia_v2023_07/model/template_variable.py
+criteo_api_retailmedia_v2023_07/model/template_variable_value.py
+criteo_api_retailmedia_v2023_07/model/text_variable_specification.py
+criteo_api_retailmedia_v2023_07/model/text_variable_value.py
+criteo_api_retailmedia_v2023_07/model/user_behavior_details.py
+criteo_api_retailmedia_v2023_07/model/user_behavior_details_v2.py
+criteo_api_retailmedia_v2023_07/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
+criteo_api_retailmedia_v2023_07/model/value_type_resource_of_add_to_basket_target202110.py
+criteo_api_retailmedia_v2023_07/model/value_type_resource_of_audience_ids_update_model202110.py
+criteo_api_retailmedia_v2023_07/model/value_type_resource_of_audience_target202110.py
+criteo_api_retailmedia_v2023_07/model/value_type_resource_of_keyword_target202110.py
+criteo_api_retailmedia_v2023_07/model/value_type_resource_of_store_ids_update_model202110.py
+criteo_api_retailmedia_v2023_07/model/value_type_resource_of_store_target202110.py
+criteo_api_retailmedia_v2023_07/models/__init__.py
 test/test_gateway_api.py
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/__init__.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "2023.04.0.230726"
+__version__ = "2023.07.0.230726"
 
 # import ApiClient
-from criteo_api_retailmedia_v2023_04.api_client import ApiClient
-from criteo_api_retailmedia_v2023_04.criteo_api_client import CriteoApiClient
-from criteo_api_retailmedia_v2023_04.api_client_builder import ApiClientBuilder
-from criteo_api_retailmedia_v2023_04 import flow_constants
+from criteo_api_retailmedia_v2023_07.api_client import ApiClient
+from criteo_api_retailmedia_v2023_07.criteo_api_client import CriteoApiClient
+from criteo_api_retailmedia_v2023_07.api_client_builder import ApiClientBuilder
+from criteo_api_retailmedia_v2023_07 import flow_constants
 
 # import Configuration
-from criteo_api_retailmedia_v2023_04.configuration import Configuration
+from criteo_api_retailmedia_v2023_07.configuration import Configuration
 
 # import exceptions
-from criteo_api_retailmedia_v2023_04.exceptions import OpenApiException
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
-from criteo_api_retailmedia_v2023_04.exceptions import ApiTypeError
-from criteo_api_retailmedia_v2023_04.exceptions import ApiValueError
-from criteo_api_retailmedia_v2023_04.exceptions import ApiKeyError
-from criteo_api_retailmedia_v2023_04.exceptions import ApiException
+from criteo_api_retailmedia_v2023_07.exceptions import OpenApiException
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiTypeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiValueError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiKeyError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiException
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/api/analytics_api.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/api/analytics_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,273 +1,287 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_retailmedia_v2023_04.model.bad_request import BadRequest
-from criteo_api_retailmedia_v2023_04.model.envelope_report_request import EnvelopeReportRequest
-from criteo_api_retailmedia_v2023_04.model.envelope_report_status import EnvelopeReportStatus
+from criteo_api_retailmedia_v2023_07.model.async_report_response import AsyncReportResponse
+from criteo_api_retailmedia_v2023_07.model.campaign_report_request import CampaignReportRequest
+from criteo_api_retailmedia_v2023_07.model.line_item_report_request import LineItemReportRequest
+from criteo_api_retailmedia_v2023_07.model.report_outcome import ReportOutcome
+from criteo_api_retailmedia_v2023_07.model.report_response import ReportResponse
 
 
 class AnalyticsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
-        self.get_report_output_endpoint = _Endpoint(
+        self.generate_campaign_reports_endpoint = _Endpoint(
             settings={
-                'response_type': (str,),
+                'response_type': (ReportResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/reports/{reportId}/output',
-                'operation_id': 'get_report_output',
-                'http_method': 'GET',
+                'endpoint_path': '/2023-07/retail-media/reports/campaigns',
+                'operation_id': 'generate_campaign_reports',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'report_id',
+                    'campaign_report_request',
                 ],
                 'required': [
-                    'report_id',
+                    'campaign_report_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'report_id':
-                        (str,),
+                    'campaign_report_request':
+                        (CampaignReportRequest,),
                 },
                 'attribute_map': {
-                    'report_id': 'reportId',
                 },
                 'location_map': {
-                    'report_id': 'path',
+                    'campaign_report_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/octet-stream'
+                    'text/plain',
+                    'application/json',
+                    'text/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json',
+                    'text/json',
+                    'application/*+json'
+                ]
             },
             api_client=api_client
         )
-        self.get_report_status_endpoint = _Endpoint(
+        self.generate_line_items_reports_endpoint = _Endpoint(
             settings={
-                'response_type': (EnvelopeReportStatus,),
+                'response_type': (ReportResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/reports/{reportId}/status',
-                'operation_id': 'get_report_status',
-                'http_method': 'GET',
+                'endpoint_path': '/2023-07/retail-media/reports/line-items',
+                'operation_id': 'generate_line_items_reports',
+                'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'report_id',
+                    'line_item_report_request',
                 ],
                 'required': [
-                    'report_id',
+                    'line_item_report_request',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'report_id':
-                        (str,),
+                    'line_item_report_request':
+                        (LineItemReportRequest,),
                 },
                 'attribute_map': {
-                    'report_id': 'reportId',
                 },
                 'location_map': {
-                    'report_id': 'path',
+                    'line_item_report_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/json'
+                    'text/plain',
+                    'application/json',
+                    'text/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json',
+                    'text/json',
+                    'application/*+json'
+                ]
             },
             api_client=api_client
         )
-        self.request_campaign_report_endpoint = _Endpoint(
+        self.get_async_export_output_endpoint = _Endpoint(
             settings={
-                'response_type': (EnvelopeReportStatus,),
+                'response_type': (str,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/reports/campaigns',
-                'operation_id': 'request_campaign_report',
-                'http_method': 'POST',
+                'endpoint_path': '/2023-07/retail-media/reports/{reportId}/output',
+                'operation_id': 'get_async_export_output',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'envelope_report_request',
+                    'report_id',
                 ],
                 'required': [
-                    'envelope_report_request',
+                    'report_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'envelope_report_request':
-                        (EnvelopeReportRequest,),
+                    'report_id':
+                        (str,),
                 },
                 'attribute_map': {
+                    'report_id': 'reportId',
                 },
                 'location_map': {
-                    'envelope_report_request': 'body',
+                    'report_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/json'
+                    'text/plain',
+                    'application/json',
+                    'text/json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.request_line_item_report_endpoint = _Endpoint(
+        self.get_async_export_status_endpoint = _Endpoint(
             settings={
-                'response_type': (EnvelopeReportStatus,),
+                'response_type': (AsyncReportResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/reports/line-items',
-                'operation_id': 'request_line_item_report',
-                'http_method': 'POST',
+                'endpoint_path': '/2023-07/retail-media/reports/{reportId}/status',
+                'operation_id': 'get_async_export_status',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'envelope_report_request',
+                    'report_id',
                 ],
                 'required': [
-                    'envelope_report_request',
+                    'report_id',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'envelope_report_request':
-                        (EnvelopeReportRequest,),
+                    'report_id':
+                        (str,),
                 },
                 'attribute_map': {
+                    'report_id': 'reportId',
                 },
                 'location_map': {
-                    'envelope_report_request': 'body',
+                    'report_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/json'
+                    'text/plain',
+                    'application/json',
+                    'text/json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
 
-    def get_report_output(
+    def generate_campaign_reports(
         self,
-        report_id,
+        campaign_report_request,
         **kwargs
     ):
-        """get_report_output  # noqa: E501
+        """generate_campaign_reports  # noqa: E501
 
-        Request the report output  # noqa: E501
+        Return a Campaign Report  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_report_output(report_id, async_req=True)
+        >>> thread = api.generate_campaign_reports(campaign_report_request, async_req=True)
         >>> result = thread.get()
 
         Args:
-            report_id (str): report id
+            campaign_report_request (CampaignReportRequest):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -294,15 +308,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            str
+            ReportResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -323,34 +337,34 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['report_id'] = \
-            report_id
-        return self.get_report_output_endpoint.call_with_http_info(**kwargs)
+        kwargs['campaign_report_request'] = \
+            campaign_report_request
+        return self.generate_campaign_reports_endpoint.call_with_http_info(**kwargs)
 
-    def get_report_status(
+    def generate_line_items_reports(
         self,
-        report_id,
+        line_item_report_request,
         **kwargs
     ):
-        """get_report_status  # noqa: E501
+        """generate_line_items_reports  # noqa: E501
 
-        Get the status of the report  # noqa: E501
+        Return a Line Item Report  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_report_status(report_id, async_req=True)
+        >>> thread = api.generate_line_items_reports(line_item_report_request, async_req=True)
         >>> result = thread.get()
 
         Args:
-            report_id (str): report id
+            line_item_report_request (LineItemReportRequest):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -377,15 +391,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            EnvelopeReportStatus
+            ReportResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -406,34 +420,34 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['report_id'] = \
-            report_id
-        return self.get_report_status_endpoint.call_with_http_info(**kwargs)
+        kwargs['line_item_report_request'] = \
+            line_item_report_request
+        return self.generate_line_items_reports_endpoint.call_with_http_info(**kwargs)
 
-    def request_campaign_report(
+    def get_async_export_output(
         self,
-        envelope_report_request,
+        report_id,
         **kwargs
     ):
-        """request_campaign_report  # noqa: E501
+        """get_async_export_output  # noqa: E501
 
-        Request a campaign report  # noqa: E501
+        Return the output of an async report  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.request_campaign_report(envelope_report_request, async_req=True)
+        >>> thread = api.get_async_export_output(report_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            envelope_report_request (EnvelopeReportRequest): Envelope of the request
+            report_id (str): The ID of the report to retrieve
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -460,15 +474,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            EnvelopeReportStatus
+            str
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -489,34 +503,34 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['envelope_report_request'] = \
-            envelope_report_request
-        return self.request_campaign_report_endpoint.call_with_http_info(**kwargs)
+        kwargs['report_id'] = \
+            report_id
+        return self.get_async_export_output_endpoint.call_with_http_info(**kwargs)
 
-    def request_line_item_report(
+    def get_async_export_status(
         self,
-        envelope_report_request,
+        report_id,
         **kwargs
     ):
-        """request_line_item_report  # noqa: E501
+        """get_async_export_status  # noqa: E501
 
-        Request a line item report  # noqa: E501
+        Return the status of an async report  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.request_line_item_report(envelope_report_request, async_req=True)
+        >>> thread = api.get_async_export_status(report_id, async_req=True)
         >>> result = thread.get()
 
         Args:
-            envelope_report_request (EnvelopeReportRequest): Envelope of the request
+            report_id (str): The ID of the report to retrieve
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -543,15 +557,15 @@
             _request_auths (list): set to override the auth_settings for an a single
                 request; this effectively ignores the authentication
                 in the spec for a single request.
                 Default is None
             async_req (bool): execute request asynchronously
 
         Returns:
-            EnvelopeReportStatus
+            AsyncReportResponse
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -572,11 +586,11 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
-        kwargs['envelope_report_request'] = \
-            envelope_report_request
-        return self.request_line_item_report_endpoint.call_with_http_info(**kwargs)
+        kwargs['report_id'] = \
+            report_id
+        return self.get_async_export_status_endpoint.call_with_http_info(**kwargs)
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/api/audience_api.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/api/audience_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_retailmedia_v2023_04.model.common_status_code_response import CommonStatusCodeResponse
-from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_request import CreateRetailMediaAudienceRequest
-from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_response import CreateRetailMediaAudienceResponse
-from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2_request import CreateRetailMediaAudienceV2Request
-from criteo_api_retailmedia_v2023_04.model.get_page_of_audiences_by_account_id_response import GetPageOfAudiencesByAccountIdResponse
-from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2_list_response import RetailMediaAudienceV2ListResponse
-from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2_response import RetailMediaAudienceV2Response
+from criteo_api_retailmedia_v2023_07.model.common_status_code_response import CommonStatusCodeResponse
+from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_request import CreateRetailMediaAudienceRequest
+from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_response import CreateRetailMediaAudienceResponse
+from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_v2_request import CreateRetailMediaAudienceV2Request
+from criteo_api_retailmedia_v2023_07.model.get_page_of_audiences_by_account_id_response import GetPageOfAudiencesByAccountIdResponse
+from criteo_api_retailmedia_v2023_07.model.retail_media_audience_v2_list_response import RetailMediaAudienceV2ListResponse
+from criteo_api_retailmedia_v2023_07.model.retail_media_audience_v2_response import RetailMediaAudienceV2Response
 
 
 class AudienceApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -44,15 +44,15 @@
         self.create_audience_endpoint = _Endpoint(
             settings={
                 'response_type': (CreateRetailMediaAudienceResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/accounts/{accountId}/audiences',
+                'endpoint_path': '/2023-07/retail-media/accounts/{accountId}/audiences',
                 'operation_id': 'create_audience',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -103,15 +103,15 @@
         self.create_retail_media_audience_v2_endpoint = _Endpoint(
             settings={
                 'response_type': (RetailMediaAudienceV2Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/v2/accounts/{accountId}/audiences',
+                'endpoint_path': '/2023-07/retail-media/v2/accounts/{accountId}/audiences',
                 'operation_id': 'create_retail_media_audience_v2',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -162,15 +162,15 @@
         self.get_audiences_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (GetPageOfAudiencesByAccountIdResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/accounts/{accountId}/audiences',
+                'endpoint_path': '/2023-07/retail-media/accounts/{accountId}/audiences',
                 'operation_id': 'get_audiences_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -230,15 +230,15 @@
         self.get_retail_media_audience_v2_list_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (RetailMediaAudienceV2ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/v2/accounts/{accountId}/audiences',
+                'endpoint_path': '/2023-07/retail-media/v2/accounts/{accountId}/audiences',
                 'operation_id': 'get_retail_media_audience_v2_list_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/api/campaign_api.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/api/campaign_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,84 +1,84 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_retailmedia_v2023_04.model.add_to_basket_ids_update_model202110_request import AddToBasketIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2023_04.model.add_to_basket_target202110_request import AddToBasketTarget202110Request
-from criteo_api_retailmedia_v2023_04.model.add_to_basket_target202110_response import AddToBasketTarget202110Response
-from criteo_api_retailmedia_v2023_04.model.asset_response import AssetResponse
-from criteo_api_retailmedia_v2023_04.model.auction_line_item_create_model_request import AuctionLineItemCreateModelRequest
-from criteo_api_retailmedia_v2023_04.model.auction_line_item_paged_list_response import AuctionLineItemPagedListResponse
-from criteo_api_retailmedia_v2023_04.model.auction_line_item_response import AuctionLineItemResponse
-from criteo_api_retailmedia_v2023_04.model.auction_line_item_update_model_request import AuctionLineItemUpdateModelRequest
-from criteo_api_retailmedia_v2023_04.model.audience_ids_update_model202110_request import AudienceIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2023_04.model.audience_target202110_request import AudienceTarget202110Request
-from criteo_api_retailmedia_v2023_04.model.audience_target202110_response import AudienceTarget202110Response
-from criteo_api_retailmedia_v2023_04.model.balance202110_paged_list_response import Balance202110PagedListResponse
-from criteo_api_retailmedia_v2023_04.model.balance_campaign202110_list_request import BalanceCampaign202110ListRequest
-from criteo_api_retailmedia_v2023_04.model.balance_campaign202110_paged_list_response import BalanceCampaign202110PagedListResponse
-from criteo_api_retailmedia_v2023_04.model.category202204 import Category202204
-from criteo_api_retailmedia_v2023_04.model.category202204_list_response import Category202204ListResponse
-from criteo_api_retailmedia_v2023_04.model.common_line_item_paged_list_response import CommonLineItemPagedListResponse
-from criteo_api_retailmedia_v2023_04.model.common_line_item_response import CommonLineItemResponse
-from criteo_api_retailmedia_v2023_04.model.creative202110_list_response import Creative202110ListResponse
-from criteo_api_retailmedia_v2023_04.model.creative202210_list_response import Creative202210ListResponse
-from criteo_api_retailmedia_v2023_04.model.creative202210_response import Creative202210Response
-from criteo_api_retailmedia_v2023_04.model.creative_create_model202207 import CreativeCreateModel202207
-from criteo_api_retailmedia_v2023_04.model.creative_update_model202207 import CreativeUpdateModel202207
-from criteo_api_retailmedia_v2023_04.model.external_retailer_pages202110 import ExternalRetailerPages202110
-from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_account import JsonApiPageResponseOfAccount
-from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_brand import JsonApiPageResponseOfBrand
-from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_campaign_v202301 import JsonApiPageResponseOfCampaignV202301
-from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_retailer import JsonApiPageResponseOfRetailer
-from criteo_api_retailmedia_v2023_04.model.json_api_request_of_catalog_request import JsonApiRequestOfCatalogRequest
-from criteo_api_retailmedia_v2023_04.model.json_api_single_response_of_campaign_v202301 import JsonApiSingleResponseOfCampaignV202301
-from criteo_api_retailmedia_v2023_04.model.json_api_single_response_of_catalog_status import JsonApiSingleResponseOfCatalogStatus
-from criteo_api_retailmedia_v2023_04.model.json_api_single_response_of_line_item_bid_multipliers import JsonApiSingleResponseOfLineItemBidMultipliers
-from criteo_api_retailmedia_v2023_04.model.keyword_target202110_request import KeywordTarget202110Request
-from criteo_api_retailmedia_v2023_04.model.keyword_target202110_response import KeywordTarget202110Response
-from criteo_api_retailmedia_v2023_04.model.line_item_bid_multipliers_request import LineItemBidMultipliersRequest
-from criteo_api_retailmedia_v2023_04.model.line_item_bid_multipliers_response import LineItemBidMultipliersResponse
-from criteo_api_retailmedia_v2023_04.model.post_campaign_v202301 import PostCampaignV202301
-from criteo_api_retailmedia_v2023_04.model.preferred_line_item202110_paged_list_response import PreferredLineItem202110PagedListResponse
-from criteo_api_retailmedia_v2023_04.model.preferred_line_item202110_response import PreferredLineItem202110Response
-from criteo_api_retailmedia_v2023_04.model.preferred_line_item_create_model202110_request import PreferredLineItemCreateModel202110Request
-from criteo_api_retailmedia_v2023_04.model.preferred_line_item_update_model202110_request import PreferredLineItemUpdateModel202110Request
-from criteo_api_retailmedia_v2023_04.model.promoted_product202110_list_request import PromotedProduct202110ListRequest
-from criteo_api_retailmedia_v2023_04.model.promoted_product202110_paged_list_response import PromotedProduct202110PagedListResponse
-from criteo_api_retailmedia_v2023_04.model.put_campaign_v202301 import PutCampaignV202301
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_add_remove_keywords_model_request import RetailMediaExternalv1AddRemoveKeywordsModelRequest
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_keywords_model_response import RetailMediaExternalv1KeywordsModelResponse
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_proposal_status_model_response import RetailMediaExternalv1ProposalStatusModelResponse
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_resource_outcome import RetailMediaExternalv1ResourceOutcome
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_set_bids_model_request import RetailMediaExternalv1SetBidsModelRequest
-from criteo_api_retailmedia_v2023_04.model.store_ids_update_model202110_request import StoreIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2023_04.model.store_target202110_request import StoreTarget202110Request
-from criteo_api_retailmedia_v2023_04.model.store_target202110_response import StoreTarget202110Response
-from criteo_api_retailmedia_v2023_04.model.template_list_response import TemplateListResponse
-from criteo_api_retailmedia_v2023_04.model.template_response import TemplateResponse
+from criteo_api_retailmedia_v2023_07.model.add_to_basket_ids_update_model202110_request import AddToBasketIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2023_07.model.add_to_basket_target202110_request import AddToBasketTarget202110Request
+from criteo_api_retailmedia_v2023_07.model.add_to_basket_target202110_response import AddToBasketTarget202110Response
+from criteo_api_retailmedia_v2023_07.model.asset_response import AssetResponse
+from criteo_api_retailmedia_v2023_07.model.auction_line_item_create_model_request import AuctionLineItemCreateModelRequest
+from criteo_api_retailmedia_v2023_07.model.auction_line_item_paged_list_response import AuctionLineItemPagedListResponse
+from criteo_api_retailmedia_v2023_07.model.auction_line_item_response import AuctionLineItemResponse
+from criteo_api_retailmedia_v2023_07.model.auction_line_item_update_model_request import AuctionLineItemUpdateModelRequest
+from criteo_api_retailmedia_v2023_07.model.audience_ids_update_model202110_request import AudienceIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2023_07.model.audience_target202110_request import AudienceTarget202110Request
+from criteo_api_retailmedia_v2023_07.model.audience_target202110_response import AudienceTarget202110Response
+from criteo_api_retailmedia_v2023_07.model.balance202110_paged_list_response import Balance202110PagedListResponse
+from criteo_api_retailmedia_v2023_07.model.balance_campaign202110_list_request import BalanceCampaign202110ListRequest
+from criteo_api_retailmedia_v2023_07.model.balance_campaign202110_paged_list_response import BalanceCampaign202110PagedListResponse
+from criteo_api_retailmedia_v2023_07.model.category202204 import Category202204
+from criteo_api_retailmedia_v2023_07.model.category202204_list_response import Category202204ListResponse
+from criteo_api_retailmedia_v2023_07.model.common_line_item_paged_list_response import CommonLineItemPagedListResponse
+from criteo_api_retailmedia_v2023_07.model.common_line_item_response import CommonLineItemResponse
+from criteo_api_retailmedia_v2023_07.model.creative202110_list_response import Creative202110ListResponse
+from criteo_api_retailmedia_v2023_07.model.creative202210_list_response import Creative202210ListResponse
+from criteo_api_retailmedia_v2023_07.model.creative202210_response import Creative202210Response
+from criteo_api_retailmedia_v2023_07.model.creative_create_model202207 import CreativeCreateModel202207
+from criteo_api_retailmedia_v2023_07.model.creative_update_model202207 import CreativeUpdateModel202207
+from criteo_api_retailmedia_v2023_07.model.external_retailer_pages202110 import ExternalRetailerPages202110
+from criteo_api_retailmedia_v2023_07.model.json_api_page_response_of_account import JsonApiPageResponseOfAccount
+from criteo_api_retailmedia_v2023_07.model.json_api_page_response_of_brand import JsonApiPageResponseOfBrand
+from criteo_api_retailmedia_v2023_07.model.json_api_page_response_of_campaign_v202301 import JsonApiPageResponseOfCampaignV202301
+from criteo_api_retailmedia_v2023_07.model.json_api_page_response_of_retailer import JsonApiPageResponseOfRetailer
+from criteo_api_retailmedia_v2023_07.model.json_api_request_of_catalog_request import JsonApiRequestOfCatalogRequest
+from criteo_api_retailmedia_v2023_07.model.json_api_single_response_of_campaign_v202301 import JsonApiSingleResponseOfCampaignV202301
+from criteo_api_retailmedia_v2023_07.model.json_api_single_response_of_catalog_status import JsonApiSingleResponseOfCatalogStatus
+from criteo_api_retailmedia_v2023_07.model.json_api_single_response_of_line_item_bid_multipliers import JsonApiSingleResponseOfLineItemBidMultipliers
+from criteo_api_retailmedia_v2023_07.model.keyword_target202110_request import KeywordTarget202110Request
+from criteo_api_retailmedia_v2023_07.model.keyword_target202110_response import KeywordTarget202110Response
+from criteo_api_retailmedia_v2023_07.model.line_item_bid_multipliers_request import LineItemBidMultipliersRequest
+from criteo_api_retailmedia_v2023_07.model.line_item_bid_multipliers_response import LineItemBidMultipliersResponse
+from criteo_api_retailmedia_v2023_07.model.post_campaign_v202301 import PostCampaignV202301
+from criteo_api_retailmedia_v2023_07.model.preferred_line_item202110_paged_list_response import PreferredLineItem202110PagedListResponse
+from criteo_api_retailmedia_v2023_07.model.preferred_line_item202110_response import PreferredLineItem202110Response
+from criteo_api_retailmedia_v2023_07.model.preferred_line_item_create_model202110_request import PreferredLineItemCreateModel202110Request
+from criteo_api_retailmedia_v2023_07.model.preferred_line_item_update_model202110_request import PreferredLineItemUpdateModel202110Request
+from criteo_api_retailmedia_v2023_07.model.promoted_product202110_list_request import PromotedProduct202110ListRequest
+from criteo_api_retailmedia_v2023_07.model.promoted_product202110_paged_list_response import PromotedProduct202110PagedListResponse
+from criteo_api_retailmedia_v2023_07.model.put_campaign_v202301 import PutCampaignV202301
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_add_remove_keywords_model_request import RetailMediaExternalv1AddRemoveKeywordsModelRequest
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_keywords_model_response import RetailMediaExternalv1KeywordsModelResponse
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_proposal_status_model_response import RetailMediaExternalv1ProposalStatusModelResponse
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_resource_outcome import RetailMediaExternalv1ResourceOutcome
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_set_bids_model_request import RetailMediaExternalv1SetBidsModelRequest
+from criteo_api_retailmedia_v2023_07.model.store_ids_update_model202110_request import StoreIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2023_07.model.store_target202110_request import StoreTarget202110Request
+from criteo_api_retailmedia_v2023_07.model.store_target202110_response import StoreTarget202110Response
+from criteo_api_retailmedia_v2023_07.model.template_list_response import TemplateListResponse
+from criteo_api_retailmedia_v2023_07.model.template_response import TemplateResponse
 
 
 class CampaignApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -91,15 +91,15 @@
         self.add_remove_keywords_endpoint = _Endpoint(
             settings={
                 'response_type': (RetailMediaExternalv1ResourceOutcome,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/line-items/{id}/keywords/add-remove',
+                'endpoint_path': '/2023-07/retail-media/line-items/{id}/keywords/add-remove',
                 'operation_id': 'add_remove_keywords',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
@@ -151,15 +151,15 @@
         self.create_asset_endpoint = _Endpoint(
             settings={
                 'response_type': (AssetResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/assets',
+                'endpoint_path': '/2023-07/retail-media/assets',
                 'operation_id': 'create_asset',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'asset_file',
@@ -207,15 +207,15 @@
         self.fetch_keywords_endpoint = _Endpoint(
             settings={
                 'response_type': (RetailMediaExternalv1KeywordsModelResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/line-items/{id}/keywords',
+                'endpoint_path': '/2023-07/retail-media/line-items/{id}/keywords',
                 'operation_id': 'fetch_keywords',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
@@ -261,15 +261,15 @@
         self.fetch_proposal_endpoint = _Endpoint(
             settings={
                 'response_type': (RetailMediaExternalv1ProposalStatusModelResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-deal-line-items/{id}/proposal',
+                'endpoint_path': '/2023-07/retail-media/preferred-deal-line-items/{id}/proposal',
                 'operation_id': 'fetch_proposal',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
@@ -315,15 +315,15 @@
         self.get_api202110_external_account_balances_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Balance202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/accounts/{account-id}/balances',
+                'endpoint_path': '/2023-07/retail-media/accounts/{account-id}/balances',
                 'operation_id': 'get_api202110_external_account_balances_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -383,15 +383,15 @@
         self.get_api202110_external_account_creatives_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Creative202110ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/accounts/{account-id}/creatives',
+                'endpoint_path': '/2023-07/retail-media/accounts/{account-id}/creatives',
                 'operation_id': 'get_api202110_external_account_creatives_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -435,15 +435,15 @@
         self.get_api202110_external_auction_line_item_targeting_keywords_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (KeywordTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/auction-line-items/{line-item-id}/targeting/keywords',
+                'endpoint_path': '/2023-07/retail-media/auction-line-items/{line-item-id}/targeting/keywords',
                 'operation_id': 'get_api202110_external_auction_line_item_targeting_keywords_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -487,15 +487,15 @@
         self.get_api202110_external_balance_campaigns_by_balance_id_endpoint = _Endpoint(
             settings={
                 'response_type': (BalanceCampaign202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/balances/{balance-id}/campaigns',
+                'endpoint_path': '/2023-07/retail-media/balances/{balance-id}/campaigns',
                 'operation_id': 'get_api202110_external_balance_campaigns_by_balance_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'balance_id',
@@ -555,15 +555,15 @@
         self.get_api202110_external_campaign_preferred_line_items_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PreferredLineItem202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/campaigns/{campaign-id}/preferred-line-items',
+                'endpoint_path': '/2023-07/retail-media/campaigns/{campaign-id}/preferred-line-items',
                 'operation_id': 'get_api202110_external_campaign_preferred_line_items_by_campaign_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -623,15 +623,15 @@
         self.get_api202110_external_line_item_products_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PromotedProduct202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}/products',
+                'endpoint_path': '/2023-07/retail-media/line-items/{line-item-id}/products',
                 'operation_id': 'get_api202110_external_line_item_products_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -691,15 +691,15 @@
         self.get_api202110_external_preferred_line_item_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PreferredLineItem202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}',
+                'endpoint_path': '/2023-07/retail-media/preferred-line-items/{line-item-id}',
                 'operation_id': 'get_api202110_external_preferred_line_item_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -743,15 +743,15 @@
         self.get_api202110_external_preferred_line_item_targeting_add_to_basket_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AddToBasketTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket',
+                'endpoint_path': '/2023-07/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket',
                 'operation_id': 'get_api202110_external_preferred_line_item_targeting_add_to_basket_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -795,15 +795,15 @@
         self.get_api202110_external_preferred_line_item_targeting_audiences_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/audiences',
+                'endpoint_path': '/2023-07/retail-media/preferred-line-items/{line-item-id}/targeting/audiences',
                 'operation_id': 'get_api202110_external_preferred_line_item_targeting_audiences_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -847,15 +847,15 @@
         self.get_api202110_external_preferred_line_item_targeting_stores_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (StoreTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/stores',
+                'endpoint_path': '/2023-07/retail-media/preferred-line-items/{line-item-id}/targeting/stores',
                 'operation_id': 'get_api202110_external_preferred_line_item_targeting_stores_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -899,15 +899,15 @@
         self.get_api202110_external_retailer_pages_by_retailer_id_endpoint = _Endpoint(
             settings={
                 'response_type': (ExternalRetailerPages202110,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/retailers/{retailerId}/pages',
+                'endpoint_path': '/2023-07/retail-media/retailers/{retailerId}/pages',
                 'operation_id': 'get_api202110_external_retailer_pages_by_retailer_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'retailer_id',
@@ -951,15 +951,15 @@
         self.get_api202204_external_categorie_by_category_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Category202204,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/categories/{categoryId}',
+                'endpoint_path': '/2023-07/retail-media/categories/{categoryId}',
                 'operation_id': 'get_api202204_external_categorie_by_category_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'category_id',
@@ -1003,15 +1003,15 @@
         self.get_api202204_external_categories_endpoint = _Endpoint(
             settings={
                 'response_type': (Category202204ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/categories',
+                'endpoint_path': '/2023-07/retail-media/categories',
                 'operation_id': 'get_api202204_external_categories',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'retailer_id',
@@ -1080,15 +1080,15 @@
         self.get_api202207_external_retailer_by_retailer_id_templatestemplate_id_endpoint = _Endpoint(
             settings={
                 'response_type': (TemplateResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/retailers/{retailer-id}/templates/{template-id}',
+                'endpoint_path': '/2023-07/retail-media/retailers/{retailer-id}/templates/{template-id}',
                 'operation_id': 'get_api202207_external_retailer_by_retailer_id_templatestemplate_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'retailer_id',
@@ -1138,15 +1138,15 @@
         self.get_api202207_external_retailer_templates_by_retailer_id_endpoint = _Endpoint(
             settings={
                 'response_type': (TemplateListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/retailers/{retailer-id}/templates',
+                'endpoint_path': '/2023-07/retail-media/retailers/{retailer-id}/templates',
                 'operation_id': 'get_api202207_external_retailer_templates_by_retailer_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'retailer_id',
@@ -1190,15 +1190,15 @@
         self.get_api202210_external_account_by_account_id_creativescreative_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Creative202210Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/accounts/{account-id}/creatives/{creative-id}',
+                'endpoint_path': '/2023-07/retail-media/accounts/{account-id}/creatives/{creative-id}',
                 'operation_id': 'get_api202210_external_account_by_account_id_creativescreative_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1248,15 +1248,15 @@
         self.get_api202301_external_account_campaigns_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiPageResponseOfCampaignV202301,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/accounts/{accountId}/campaigns',
+                'endpoint_path': '/2023-07/retail-media/accounts/{accountId}/campaigns',
                 'operation_id': 'get_api202301_external_account_campaigns_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1316,15 +1316,15 @@
         self.get_api202301_external_campaign_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfCampaignV202301,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/campaigns/{campaignId}',
+                'endpoint_path': '/2023-07/retail-media/campaigns/{campaignId}',
                 'operation_id': 'get_api202301_external_campaign_by_campaign_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -1368,15 +1368,15 @@
         self.get_api202301_external_line_item_bid_multipliers_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfLineItemBidMultipliers,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}/bid-multipliers',
+                'endpoint_path': '/2023-07/retail-media/line-items/{line-item-id}/bid-multipliers',
                 'operation_id': 'get_api202301_external_line_item_bid_multipliers_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -1422,15 +1422,15 @@
         self.get_api_v1_external_account_brands_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiPageResponseOfBrand,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/accounts/{accountId}/brands',
+                'endpoint_path': '/2023-07/retail-media/accounts/{accountId}/brands',
                 'operation_id': 'get_api_v1_external_account_brands_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1490,15 +1490,15 @@
         self.get_api_v1_external_account_retailers_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiPageResponseOfRetailer,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/accounts/{accountId}/retailers',
+                'endpoint_path': '/2023-07/retail-media/accounts/{accountId}/retailers',
                 'operation_id': 'get_api_v1_external_account_retailers_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1558,15 +1558,15 @@
         self.get_api_v1_external_accounts_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiPageResponseOfAccount,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/accounts',
+                'endpoint_path': '/2023-07/retail-media/accounts',
                 'operation_id': 'get_api_v1_external_accounts',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'limit_to_id',
@@ -1619,15 +1619,15 @@
         self.get_api_v1_external_catalog_output_by_catalog_id_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/catalogs/{catalogId}/output',
+                'endpoint_path': '/2023-07/retail-media/catalogs/{catalogId}/output',
                 'operation_id': 'get_api_v1_external_catalog_output_by_catalog_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'catalog_id',
@@ -1672,15 +1672,15 @@
         self.get_api_v1_external_catalog_status_by_catalog_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfCatalogStatus,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/catalogs/{catalogId}/status',
+                'endpoint_path': '/2023-07/retail-media/catalogs/{catalogId}/status',
                 'operation_id': 'get_api_v1_external_catalog_status_by_catalog_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'catalog_id',
@@ -1724,15 +1724,15 @@
         self.get_api_v2_external_account_line_items_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (CommonLineItemPagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/accounts/{account-id}/line-items',
+                'endpoint_path': '/2023-07/retail-media/accounts/{account-id}/line-items',
                 'operation_id': 'get_api_v2_external_account_line_items_by_account_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -1810,15 +1810,15 @@
         self.get_api_v2_external_auction_line_item_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AuctionLineItemResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/auction-line-items/{line-item-id}',
+                'endpoint_path': '/2023-07/retail-media/auction-line-items/{line-item-id}',
                 'operation_id': 'get_api_v2_external_auction_line_item_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -1862,15 +1862,15 @@
         self.get_api_v2_external_campaign_auction_line_items_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AuctionLineItemPagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/campaigns/{campaign-id}/auction-line-items',
+                'endpoint_path': '/2023-07/retail-media/campaigns/{campaign-id}/auction-line-items',
                 'operation_id': 'get_api_v2_external_campaign_auction_line_items_by_campaign_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -1930,15 +1930,15 @@
         self.get_api_v2_external_line_item_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (CommonLineItemResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}',
+                'endpoint_path': '/2023-07/retail-media/line-items/{line-item-id}',
                 'operation_id': 'get_api_v2_external_line_item_by_line_item_id',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -1982,15 +1982,15 @@
         self.post_api202110_external_auction_line_item_targeting_keywords_append_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (KeywordTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/auction-line-items/{line-item-id}/targeting/keywords/append',
+                'endpoint_path': '/2023-07/retail-media/auction-line-items/{line-item-id}/targeting/keywords/append',
                 'operation_id': 'post_api202110_external_auction_line_item_targeting_keywords_append_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2040,15 +2040,15 @@
         self.post_api202110_external_auction_line_item_targeting_keywords_delete_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (KeywordTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/auction-line-items/{line-item-id}/targeting/keywords/delete',
+                'endpoint_path': '/2023-07/retail-media/auction-line-items/{line-item-id}/targeting/keywords/delete',
                 'operation_id': 'post_api202110_external_auction_line_item_targeting_keywords_delete_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2098,15 +2098,15 @@
         self.post_api202110_external_balance_campaigns_append_by_balance_id_endpoint = _Endpoint(
             settings={
                 'response_type': (BalanceCampaign202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/balances/{balance-id}/campaigns/append',
+                'endpoint_path': '/2023-07/retail-media/balances/{balance-id}/campaigns/append',
                 'operation_id': 'post_api202110_external_balance_campaigns_append_by_balance_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'balance_id',
@@ -2156,15 +2156,15 @@
         self.post_api202110_external_balance_campaigns_delete_by_balance_id_endpoint = _Endpoint(
             settings={
                 'response_type': (BalanceCampaign202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/balances/{balance-id}/campaigns/delete',
+                'endpoint_path': '/2023-07/retail-media/balances/{balance-id}/campaigns/delete',
                 'operation_id': 'post_api202110_external_balance_campaigns_delete_by_balance_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'balance_id',
@@ -2214,15 +2214,15 @@
         self.post_api202110_external_campaign_preferred_line_items_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PreferredLineItem202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/campaigns/{campaign-id}/preferred-line-items',
+                'endpoint_path': '/2023-07/retail-media/campaigns/{campaign-id}/preferred-line-items',
                 'operation_id': 'post_api202110_external_campaign_preferred_line_items_by_campaign_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -2272,15 +2272,15 @@
         self.post_api202110_external_line_item_products_append_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PromotedProduct202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}/products/append',
+                'endpoint_path': '/2023-07/retail-media/line-items/{line-item-id}/products/append',
                 'operation_id': 'post_api202110_external_line_item_products_append_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2330,15 +2330,15 @@
         self.post_api202110_external_line_item_products_delete_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PromotedProduct202110PagedListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}/products/delete',
+                'endpoint_path': '/2023-07/retail-media/line-items/{line-item-id}/products/delete',
                 'operation_id': 'post_api202110_external_line_item_products_delete_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2388,15 +2388,15 @@
         self.post_api202110_external_line_item_products_pause_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}/products/pause',
+                'endpoint_path': '/2023-07/retail-media/line-items/{line-item-id}/products/pause',
                 'operation_id': 'post_api202110_external_line_item_products_pause_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2444,15 +2444,15 @@
         self.post_api202110_external_line_item_products_unpause_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}/products/unpause',
+                'endpoint_path': '/2023-07/retail-media/line-items/{line-item-id}/products/unpause',
                 'operation_id': 'post_api202110_external_line_item_products_unpause_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2500,15 +2500,15 @@
         self.post_api202110_external_preferred_line_item_targeting_add_to_basket_append_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AddToBasketTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket/append',
+                'endpoint_path': '/2023-07/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket/append',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_add_to_basket_append_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2558,15 +2558,15 @@
         self.post_api202110_external_preferred_line_item_targeting_add_to_basket_delete_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AddToBasketTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket/delete',
+                'endpoint_path': '/2023-07/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket/delete',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_add_to_basket_delete_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2616,15 +2616,15 @@
         self.post_api202110_external_preferred_line_item_targeting_audiences_append_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/audiences/append',
+                'endpoint_path': '/2023-07/retail-media/preferred-line-items/{line-item-id}/targeting/audiences/append',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_audiences_append_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2674,15 +2674,15 @@
         self.post_api202110_external_preferred_line_item_targeting_audiences_delete_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/audiences/delete',
+                'endpoint_path': '/2023-07/retail-media/preferred-line-items/{line-item-id}/targeting/audiences/delete',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_audiences_delete_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2732,15 +2732,15 @@
         self.post_api202110_external_preferred_line_item_targeting_stores_append_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (StoreTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/stores/append',
+                'endpoint_path': '/2023-07/retail-media/preferred-line-items/{line-item-id}/targeting/stores/append',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_stores_append_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2790,15 +2790,15 @@
         self.post_api202110_external_preferred_line_item_targeting_stores_delete_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (StoreTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/stores/delete',
+                'endpoint_path': '/2023-07/retail-media/preferred-line-items/{line-item-id}/targeting/stores/delete',
                 'operation_id': 'post_api202110_external_preferred_line_item_targeting_stores_delete_by_line_item_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -2848,15 +2848,15 @@
         self.post_api202210_external_account_creatives_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Creative202210Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/accounts/{account-id}/creatives',
+                'endpoint_path': '/2023-07/retail-media/accounts/{account-id}/creatives',
                 'operation_id': 'post_api202210_external_account_creatives_by_account_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -2906,15 +2906,15 @@
         self.post_api202210_external_account_creatives_search_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Creative202210ListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/accounts/{account-id}/creatives/search',
+                'endpoint_path': '/2023-07/retail-media/accounts/{account-id}/creatives/search',
                 'operation_id': 'post_api202210_external_account_creatives_search_by_account_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -2964,15 +2964,15 @@
         self.post_api202301_external_account_campaigns_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfCampaignV202301,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/accounts/{accountId}/campaigns',
+                'endpoint_path': '/2023-07/retail-media/accounts/{accountId}/campaigns',
                 'operation_id': 'post_api202301_external_account_campaigns_by_account_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -3022,15 +3022,15 @@
         self.post_api_v1_external_account_catalogs_by_account_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfCatalogStatus,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/accounts/{accountId}/catalogs',
+                'endpoint_path': '/2023-07/retail-media/accounts/{accountId}/catalogs',
                 'operation_id': 'post_api_v1_external_account_catalogs_by_account_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -3080,15 +3080,15 @@
         self.post_api_v2_external_campaign_auction_line_items_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AuctionLineItemResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/campaigns/{campaign-id}/auction-line-items',
+                'endpoint_path': '/2023-07/retail-media/campaigns/{campaign-id}/auction-line-items',
                 'operation_id': 'post_api_v2_external_campaign_auction_line_items_by_campaign_id',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -3138,15 +3138,15 @@
         self.put_api202110_external_preferred_line_item_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (PreferredLineItem202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}',
+                'endpoint_path': '/2023-07/retail-media/preferred-line-items/{line-item-id}',
                 'operation_id': 'put_api202110_external_preferred_line_item_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3196,15 +3196,15 @@
         self.put_api202110_external_preferred_line_item_targeting_add_to_basket_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AddToBasketTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket',
+                'endpoint_path': '/2023-07/retail-media/preferred-line-items/{line-item-id}/targeting/add-to-basket',
                 'operation_id': 'put_api202110_external_preferred_line_item_targeting_add_to_basket_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3254,15 +3254,15 @@
         self.put_api202110_external_preferred_line_item_targeting_audiences_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AudienceTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/audiences',
+                'endpoint_path': '/2023-07/retail-media/preferred-line-items/{line-item-id}/targeting/audiences',
                 'operation_id': 'put_api202110_external_preferred_line_item_targeting_audiences_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3312,15 +3312,15 @@
         self.put_api202110_external_preferred_line_item_targeting_stores_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (StoreTarget202110Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-line-items/{line-item-id}/targeting/stores',
+                'endpoint_path': '/2023-07/retail-media/preferred-line-items/{line-item-id}/targeting/stores',
                 'operation_id': 'put_api202110_external_preferred_line_item_targeting_stores_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3370,15 +3370,15 @@
         self.put_api202210_external_account_by_account_id_creativescreative_id_endpoint = _Endpoint(
             settings={
                 'response_type': (Creative202210Response,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/accounts/{account-id}/creatives/{creative-id}',
+                'endpoint_path': '/2023-07/retail-media/accounts/{account-id}/creatives/{creative-id}',
                 'operation_id': 'put_api202210_external_account_by_account_id_creativescreative_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'account_id',
@@ -3434,15 +3434,15 @@
         self.put_api202301_external_campaign_by_campaign_id_endpoint = _Endpoint(
             settings={
                 'response_type': (JsonApiSingleResponseOfCampaignV202301,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/campaigns/{campaignId}',
+                'endpoint_path': '/2023-07/retail-media/campaigns/{campaignId}',
                 'operation_id': 'put_api202301_external_campaign_by_campaign_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -3492,15 +3492,15 @@
         self.put_api202301_external_line_item_bid_multipliers_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (LineItemBidMultipliersResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/line-items/{line-item-id}/bid-multipliers',
+                'endpoint_path': '/2023-07/retail-media/line-items/{line-item-id}/bid-multipliers',
                 'operation_id': 'put_api202301_external_line_item_bid_multipliers_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3552,15 +3552,15 @@
         self.put_api_v2_external_auction_line_item_by_line_item_id_endpoint = _Endpoint(
             settings={
                 'response_type': (AuctionLineItemResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/auction-line-items/{line-item-id}',
+                'endpoint_path': '/2023-07/retail-media/auction-line-items/{line-item-id}',
                 'operation_id': 'put_api_v2_external_auction_line_item_by_line_item_id',
                 'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'line_item_id',
@@ -3610,15 +3610,15 @@
         self.set_keyword_bids_endpoint = _Endpoint(
             settings={
                 'response_type': (RetailMediaExternalv1ResourceOutcome,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/line-items/{id}/keywords/set-bid',
+                'endpoint_path': '/2023-07/retail-media/line-items/{id}/keywords/set-bid',
                 'operation_id': 'set_keyword_bids',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
@@ -3670,15 +3670,15 @@
         self.submit_proposal_endpoint = _Endpoint(
             settings={
                 'response_type': (RetailMediaExternalv1ProposalStatusModelResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/preferred-deal-line-items/{id}/proposal/submit',
+                'endpoint_path': '/2023-07/retail-media/preferred-deal-line-items/{id}/proposal/submit',
                 'operation_id': 'submit_proposal',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'id',
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/api/gateway_api.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/api/gateway_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_retailmedia_v2023_04.model.application_summary_model_response import ApplicationSummaryModelResponse
+from criteo_api_retailmedia_v2023_07.model.application_summary_model_response import ApplicationSummaryModelResponse
 
 
 class GatewayApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -38,15 +38,15 @@
         self.get_current_application_endpoint = _Endpoint(
             settings={
                 'response_type': (ApplicationSummaryModelResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/retail-media/me',
+                'endpoint_path': '/2023-07/retail-media/me',
                 'operation_id': 'get_current_application',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                 ],
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/api_client.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
@@ -16,18 +16,18 @@
 import os
 import re
 import typing
 from urllib.parse import quote
 from urllib3.fields import RequestField
 
 
-from criteo_api_retailmedia_v2023_04 import rest
-from criteo_api_retailmedia_v2023_04.configuration import Configuration
-from criteo_api_retailmedia_v2023_04.exceptions import ApiTypeError, ApiValueError, ApiException
-from criteo_api_retailmedia_v2023_04.model_utils import (
+from criteo_api_retailmedia_v2023_07 import rest
+from criteo_api_retailmedia_v2023_07.configuration import Configuration
+from criteo_api_retailmedia_v2023_07.exceptions import ApiTypeError, ApiValueError, ApiException
+from criteo_api_retailmedia_v2023_07.model_utils import (
     ModelNormal,
     ModelSimple,
     ModelComposed,
     check_allowed_values,
     check_validations,
     date,
     datetime,
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2023.04.0.230726/python'
+        self.user_agent = 'OpenAPI-Generator/2023.07.0.230726/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
@@ -800,18 +800,18 @@
         return params
 
     def __call__(self, *args, **kwargs):
         """ This method is invoked when endpoints are called
         Example:
 
         api_instance = AnalyticsApi()
-        api_instance.get_report_output  # this is an instance of the class Endpoint
-        api_instance.get_report_output()  # this invokes api_instance.get_report_output.__call__()
+        api_instance.generate_campaign_reports  # this is an instance of the class Endpoint
+        api_instance.generate_campaign_reports()  # this invokes api_instance.generate_campaign_reports.__call__()
         which then invokes the callable functions stored in that endpoint at
-        api_instance.get_report_output.callable or self.callable in this class
+        api_instance.generate_campaign_reports.callable or self.callable in this class
 
         """
         return self.callable(self, *args, **kwargs)
 
     def call_with_http_info(self, **kwargs):
 
         try:
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/api_client_builder.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/api_client_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from criteo_api_retailmedia_v2023_04.configuration import Configuration
-from criteo_api_retailmedia_v2023_04.criteo_api_client import CriteoApiClient
-from criteo_api_retailmedia_v2023_04 import flow_constants
+from criteo_api_retailmedia_v2023_07.configuration import Configuration
+from criteo_api_retailmedia_v2023_07.criteo_api_client import CriteoApiClient
+from criteo_api_retailmedia_v2023_07 import flow_constants
 
 class ApiClientBuilder :
 
     @staticmethod
     def WithClientCredentials(clientId, clientSecret, host=None):
         configuration = Configuration(username=clientId, password=clientSecret, host=host)
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/apis/__init__.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/apis/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # flake8: noqa
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
 # In order to avoid this, import only the API that you directly need like:
 #
-#   from criteo_api_retailmedia_v2023_04.api.analytics_api import AnalyticsApi
+#   from criteo_api_retailmedia_v2023_07.api.analytics_api import AnalyticsApi
 #
 # or import this package, but before doing it, use:
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
-from criteo_api_retailmedia_v2023_04.api.analytics_api import AnalyticsApi
-from criteo_api_retailmedia_v2023_04.api.audience_api import AudienceApi
-from criteo_api_retailmedia_v2023_04.api.campaign_api import CampaignApi
-from criteo_api_retailmedia_v2023_04.api.gateway_api import GatewayApi
+from criteo_api_retailmedia_v2023_07.api.analytics_api import AnalyticsApi
+from criteo_api_retailmedia_v2023_07.api.audience_api import AudienceApi
+from criteo_api_retailmedia_v2023_07.api.campaign_api import CampaignApi
+from criteo_api_retailmedia_v2023_07.api.gateway_api import GatewayApi
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/configuration.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
 from http import client as http_client
-from criteo_api_retailmedia_v2023_04.exceptions import ApiValueError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiValueError
 
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems'
 }
@@ -129,15 +129,15 @@
         """Password for HTTP basic authentication
         """
         self.discard_unknown_keys = discard_unknown_keys
         self.disabled_client_side_validations = disabled_client_side_validations
         self.logger = {}
         """Logging Settings
         """
-        self.logger["package_logger"] = logging.getLogger("criteo_api_retailmedia_v2023_04")
+        self.logger["package_logger"] = logging.getLogger("criteo_api_retailmedia_v2023_07")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
@@ -390,16 +390,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2023-04\n"\
-               "SDK Package Version: 2023.04.0.230726".\
+               "Version of the API: 2023-07\n"\
+               "SDK Package Version: 2023.07.0.230726".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/criteo_api_client.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/criteo_api_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from criteo_api_retailmedia_v2023_04.api_client import ApiClient
-from criteo_api_retailmedia_v2023_04.criteo_rest import CriteoRESTClientObject
+from criteo_api_retailmedia_v2023_07.api_client import ApiClient
+from criteo_api_retailmedia_v2023_07.criteo_rest import CriteoRESTClientObject
 
 class CriteoApiClient(ApiClient):
     def __init__(self, configuration=None, header_name=None, header_value=None,
              cookie=None, pool_threads=1, additional_parameters= {}):
         super().__init__(configuration=configuration,header_name=header_name, header_value=header_value, cookie=cookie, pool_threads=pool_threads)
         self.rest_client = CriteoRESTClientObject(self.configuration, additional_parameters)
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/criteo_auth.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/criteo_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from datetime import datetime, timedelta
-from criteo_api_retailmedia_v2023_04.exceptions import ApiException
-from criteo_api_retailmedia_v2023_04.api_client import ApiClient
-from criteo_api_retailmedia_v2023_04 import flow_constants
+from criteo_api_retailmedia_v2023_07.exceptions import ApiException
+from criteo_api_retailmedia_v2023_07.api_client import ApiClient
+from criteo_api_retailmedia_v2023_07 import flow_constants
 
 class Token(object):
 
     def __init__(self, token_string , expiration_date = None):
         self.expiration_date = expiration_date 
         self.token_string = token_string
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/criteo_rest.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/criteo_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from criteo_api_retailmedia_v2023_04.rest import RESTClientObject
-from criteo_api_retailmedia_v2023_04.criteo_auth import *
-from criteo_api_retailmedia_v2023_04 import flow_constants
+from criteo_api_retailmedia_v2023_07.rest import RESTClientObject
+from criteo_api_retailmedia_v2023_07.criteo_auth import *
+from criteo_api_retailmedia_v2023_07 import flow_constants
 
 
 class CriteoRESTClientObject(RESTClientObject):
 
     def __init__(self, configuration, additional_parameters = {}, pools_size=4, maxsize=None):
         super().__init__(configuration, pools_size, maxsize)
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/exceptions.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/add_to_basket_ids_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/add_to_basket_ids_update_model202110_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_add_to_basket_ids_update_model202110 import ValueTypeResourceOfAddToBasketIdsUpdateModel202110
+    from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_add_to_basket_ids_update_model202110 import ValueTypeResourceOfAddToBasketIdsUpdateModel202110
     globals()['ValueTypeResourceOfAddToBasketIdsUpdateModel202110'] = ValueTypeResourceOfAddToBasketIdsUpdateModel202110
 
 
 class AddToBasketIdsUpdateModel202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/add_to_basket_target202110_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
+    from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
     globals()['ValueTypeResourceOfAddToBasketTarget202110'] = ValueTypeResourceOfAddToBasketTarget202110
 
 
 class AddToBasketTarget202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/add_to_basket_target202110_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ValueTypeResourceOfAddToBasketTarget202110'] = ValueTypeResourceOfAddToBasketTarget202110
 
 
 class AddToBasketTarget202110Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/application_summary_model.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/application_summary_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ApplicationSummaryModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/application_summary_model_resource.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/application_summary_model_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.application_summary_model import ApplicationSummaryModel
+    from criteo_api_retailmedia_v2023_07.model.application_summary_model import ApplicationSummaryModel
     globals()['ApplicationSummaryModel'] = ApplicationSummaryModel
 
 
 class ApplicationSummaryModelResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/application_summary_model_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/application_summary_model_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.application_summary_model_resource import ApplicationSummaryModelResource
-    from criteo_api_retailmedia_v2023_04.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2023_07.model.application_summary_model_resource import ApplicationSummaryModelResource
+    from criteo_api_retailmedia_v2023_07.model.common_problem import CommonProblem
     globals()['ApplicationSummaryModelResource'] = ApplicationSummaryModelResource
     globals()['CommonProblem'] = CommonProblem
 
 
 class ApplicationSummaryModelResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/asset.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class Asset(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/asset_resource.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/asset_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.asset import Asset
+    from criteo_api_retailmedia_v2023_07.model.asset import Asset
     globals()['Asset'] = Asset
 
 
 class AssetResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/asset_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/asset_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.asset_resource import AssetResource
-    from criteo_api_retailmedia_v2023_04.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2023_07.model.asset_resource import AssetResource
+    from criteo_api_retailmedia_v2023_07.model.common_problem import CommonProblem
     globals()['AssetResource'] = AssetResource
     globals()['CommonProblem'] = CommonProblem
 
 
 class AssetResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/auction_line_item_create_model_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/auction_line_item_create_model_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.input_resource_of_auction_line_item_create_model import InputResourceOfAuctionLineItemCreateModel
+    from criteo_api_retailmedia_v2023_07.model.input_resource_of_auction_line_item_create_model import InputResourceOfAuctionLineItemCreateModel
     globals()['InputResourceOfAuctionLineItemCreateModel'] = InputResourceOfAuctionLineItemCreateModel
 
 
 class AuctionLineItemCreateModelRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/auction_line_item_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/auction_line_item_paged_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
+    from criteo_api_retailmedia_v2023_07.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfAuctionLineItem'] = ResourceOfAuctionLineItem
 
 
 class AuctionLineItemPagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/auction_line_item_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/auction_line_item_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfAuctionLineItem'] = ResourceOfAuctionLineItem
 
 
 class AuctionLineItemResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/auction_line_item_update_model_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/auction_line_item_update_model_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.resource_of_auction_line_item_update_model import ResourceOfAuctionLineItemUpdateModel
+    from criteo_api_retailmedia_v2023_07.model.resource_of_auction_line_item_update_model import ResourceOfAuctionLineItemUpdateModel
     globals()['ResourceOfAuctionLineItemUpdateModel'] = ResourceOfAuctionLineItemUpdateModel
 
 
 class AuctionLineItemUpdateModelRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/audience_ids_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/audience_ids_update_model202110_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_audience_ids_update_model202110 import ValueTypeResourceOfAudienceIdsUpdateModel202110
+    from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_audience_ids_update_model202110 import ValueTypeResourceOfAudienceIdsUpdateModel202110
     globals()['ValueTypeResourceOfAudienceIdsUpdateModel202110'] = ValueTypeResourceOfAudienceIdsUpdateModel202110
 
 
 class AudienceIdsUpdateModel202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/audience_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/audience_target202110_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
+    from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
     globals()['ValueTypeResourceOfAudienceTarget202110'] = ValueTypeResourceOfAudienceTarget202110
 
 
 class AudienceTarget202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/audience_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/audience_target202110_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ValueTypeResourceOfAudienceTarget202110'] = ValueTypeResourceOfAudienceTarget202110
 
 
 class AudienceTarget202110Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/bad_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_brand.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.error import Error
-    globals()['Error'] = Error
 
-
-class BadRequest(ModelNormal):
+class ExternalBrand(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -58,60 +54,65 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('name',): {
+            'max_length': 120,
+            'min_length': 0,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'errors': ([Error],),  # noqa: E501
+            'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'errors': 'errors',  # noqa: E501
+        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """BadRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
+        """ExternalBrand - a model defined in OpenAPI
+
+        Args:
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +137,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            errors ([Error]): The errors. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -168,14 +168,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -188,16 +189,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """BadRequest - a model defined in OpenAPI
+    def __init__(self, name, *args, **kwargs):  # noqa: E501
+        """ExternalBrand - a model defined in OpenAPI
+
+        Args:
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,15 +226,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            errors ([Error]): The errors. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -252,14 +255,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/balance202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/balance202110_paged_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_balance202110 import ResourceOfBalance202110
+    from criteo_api_retailmedia_v2023_07.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_balance202110 import ResourceOfBalance202110
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfBalance202110'] = ResourceOfBalance202110
 
 
 class Balance202110PagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_list_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/balance_campaign202110_list_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
+    from criteo_api_retailmedia_v2023_07.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
     globals()['ResourceOfBalanceCampaign202110'] = ResourceOfBalanceCampaign202110
 
 
 class BalanceCampaign202110ListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/balance_campaign202110_paged_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
+    from criteo_api_retailmedia_v2023_07.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfBalanceCampaign202110'] = ResourceOfBalanceCampaign202110
 
 
 class BalanceCampaign202110PagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/campaign_attributes_v202301.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/campaign_attributes_v202301.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class CampaignAttributesV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/campaign_v202301.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class CampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/category202204.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/category202204.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class Category202204(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/category202204_list_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/category202204_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_category202204 import ResourceOfCategory202204
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_category202204 import ResourceOfCategory202204
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfCategory202204'] = ResourceOfCategory202204
 
 
 class Category202204ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/choice_option.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/choice_option.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.template_variable import TemplateVariable
+    from criteo_api_retailmedia_v2023_07.model.template_variable import TemplateVariable
     globals()['TemplateVariable'] = TemplateVariable
 
 
 class ChoiceOption(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/choice_variable_specification.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/choice_variable_specification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.choice_option import ChoiceOption
+    from criteo_api_retailmedia_v2023_07.model.choice_option import ChoiceOption
     globals()['ChoiceOption'] = ChoiceOption
 
 
 class ChoiceVariableSpecification(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/choice_variable_value.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/choice_variable_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ChoiceVariableValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/color_variable_value.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/color_variable_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ColorVariableValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/common_error.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/common_warning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
-class CommonError(ModelNormal):
+class CommonWarning(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -121,15 +121,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CommonError - a model defined in OpenAPI
+        """CommonWarning - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -214,15 +214,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CommonError - a model defined in OpenAPI
+        """CommonWarning - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/common_line_item_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/common_line_item_paged_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_common_line_item import ResourceOfCommonLineItem
+    from criteo_api_retailmedia_v2023_07.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_common_line_item import ResourceOfCommonLineItem
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfCommonLineItem'] = ResourceOfCommonLineItem
 
 
 class CommonLineItemPagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/common_line_item_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/common_line_item_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_common_line_item import ResourceOfCommonLineItem
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_common_line_item import ResourceOfCommonLineItem
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfCommonLineItem'] = ResourceOfCommonLineItem
 
 
 class CommonLineItemResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/common_problem.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/common_problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class CommonProblem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/common_status_code_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/common_status_code_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2023_07.model.common_problem import CommonProblem
     globals()['CommonProblem'] = CommonProblem
 
 
 class CommonStatusCodeResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/common_warning.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/common_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
-class CommonWarning(ModelNormal):
+class CommonError(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -121,15 +121,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CommonWarning - a model defined in OpenAPI
+        """CommonError - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -214,15 +214,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CommonWarning - a model defined in OpenAPI
+        """CommonError - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_attributes import CreateRetailMediaAudienceAttributes
+    from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_attributes import CreateRetailMediaAudienceAttributes
     globals()['CreateRetailMediaAudienceAttributes'] = CreateRetailMediaAudienceAttributes
 
 
 class CreateRetailMediaAudience(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_attributes.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class CreateRetailMediaAudienceAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_body.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_attributes import CreateRetailMediaAudienceAttributes
+    from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_attributes import CreateRetailMediaAudienceAttributes
     globals()['CreateRetailMediaAudienceAttributes'] = CreateRetailMediaAudienceAttributes
 
 
 class CreateRetailMediaAudienceBody(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_body import CreateRetailMediaAudienceBody
+    from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_body import CreateRetailMediaAudienceBody
     globals()['CreateRetailMediaAudienceBody'] = CreateRetailMediaAudienceBody
 
 
 class CreateRetailMediaAudienceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience import CreateRetailMediaAudience
+    from criteo_api_retailmedia_v2023_07.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_07.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience import CreateRetailMediaAudience
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['CreateRetailMediaAudience'] = CreateRetailMediaAudience
 
 
 class CreateRetailMediaAudienceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2_attributes import CreateRetailMediaAudienceV2Attributes
+    from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_v2_attributes import CreateRetailMediaAudienceV2Attributes
     globals()['CreateRetailMediaAudienceV2Attributes'] = CreateRetailMediaAudienceV2Attributes
 
 
 class CreateRetailMediaAudienceV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_attributes.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_v2_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.user_behavior_details_v2 import UserBehaviorDetailsV2
+    from criteo_api_retailmedia_v2023_07.model.user_behavior_details_v2 import UserBehaviorDetailsV2
     globals()['UserBehaviorDetailsV2'] = UserBehaviorDetailsV2
 
 
 class CreateRetailMediaAudienceV2Attributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_data.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_v2_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2_attributes import CreateRetailMediaAudienceV2Attributes
+    from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_v2_attributes import CreateRetailMediaAudienceV2Attributes
     globals()['CreateRetailMediaAudienceV2Attributes'] = CreateRetailMediaAudienceV2Attributes
 
 
 class CreateRetailMediaAudienceV2Data(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_retail_media_audience_v2_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2_data import CreateRetailMediaAudienceV2Data
+    from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_v2_data import CreateRetailMediaAudienceV2Data
     globals()['CreateRetailMediaAudienceV2Data'] = CreateRetailMediaAudienceV2Data
 
 
 class CreateRetailMediaAudienceV2Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/create_user_behavior_segment_v2.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/create_user_behavior_segment_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class CreateUserBehaviorSegmentV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/creative202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/creative202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class Creative202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/creative202110_list_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/creative202210_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_creative202110 import ResourceOfCreative202110
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_creative202210 import ResourceOfCreative202210
     globals()['ProblemDetails'] = ProblemDetails
-    globals()['ResourceOfCreative202110'] = ResourceOfCreative202110
+    globals()['ResourceOfCreative202210'] = ResourceOfCreative202210
 
 
-class Creative202110ListResponse(ModelNormal):
+class Creative202210ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([ResourceOfCreative202110],),  # noqa: E501
+            'data': ([ResourceOfCreative202210],),  # noqa: E501
             'warnings': ([ProblemDetails],),  # noqa: E501
             'errors': ([ProblemDetails],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -111,15 +111,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Creative202110ListResponse - a model defined in OpenAPI
+        """Creative202210ListResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,15 +144,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([ResourceOfCreative202110]): [optional]  # noqa: E501
+            data ([ResourceOfCreative202210]): [optional]  # noqa: E501
             warnings ([ProblemDetails]): [optional]  # noqa: E501
             errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -199,15 +199,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Creative202110ListResponse - a model defined in OpenAPI
+        """Creative202210ListResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -232,15 +232,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([ResourceOfCreative202110]): [optional]  # noqa: E501
+            data ([ResourceOfCreative202210]): [optional]  # noqa: E501
             warnings ([ProblemDetails]): [optional]  # noqa: E501
             errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/creative202210.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/creative202210.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.page_type_environment import PageTypeEnvironment
-    from criteo_api_retailmedia_v2023_04.model.template_variable_value import TemplateVariableValue
+    from criteo_api_retailmedia_v2023_07.model.page_type_environment import PageTypeEnvironment
+    from criteo_api_retailmedia_v2023_07.model.template_variable_value import TemplateVariableValue
     globals()['PageTypeEnvironment'] = PageTypeEnvironment
     globals()['TemplateVariableValue'] = TemplateVariableValue
 
 
 class Creative202210(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/creative202210_list_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/creative202110_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_creative202210 import ResourceOfCreative202210
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_creative202110 import ResourceOfCreative202110
     globals()['ProblemDetails'] = ProblemDetails
-    globals()['ResourceOfCreative202210'] = ResourceOfCreative202210
+    globals()['ResourceOfCreative202110'] = ResourceOfCreative202110
 
 
-class Creative202210ListResponse(ModelNormal):
+class Creative202110ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([ResourceOfCreative202210],),  # noqa: E501
+            'data': ([ResourceOfCreative202110],),  # noqa: E501
             'warnings': ([ProblemDetails],),  # noqa: E501
             'errors': ([ProblemDetails],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -111,15 +111,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Creative202210ListResponse - a model defined in OpenAPI
+        """Creative202110ListResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,15 +144,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([ResourceOfCreative202210]): [optional]  # noqa: E501
+            data ([ResourceOfCreative202110]): [optional]  # noqa: E501
             warnings ([ProblemDetails]): [optional]  # noqa: E501
             errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -199,15 +199,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Creative202210ListResponse - a model defined in OpenAPI
+        """Creative202110ListResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -232,15 +232,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([ResourceOfCreative202210]): [optional]  # noqa: E501
+            data ([ResourceOfCreative202110]): [optional]  # noqa: E501
             warnings ([ProblemDetails]): [optional]  # noqa: E501
             errors ([ProblemDetails]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/creative202210_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/creative202210_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_creative202210 import ResourceOfCreative202210
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_creative202210 import ResourceOfCreative202210
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfCreative202210'] = ResourceOfCreative202210
 
 
 class Creative202210Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/creative_create_model202207.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/creative_create_model202207.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.template_variable_value import TemplateVariableValue
+    from criteo_api_retailmedia_v2023_07.model.template_variable_value import TemplateVariableValue
     globals()['TemplateVariableValue'] = TemplateVariableValue
 
 
 class CreativeCreateModel202207(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/creative_update_model202207.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/creative_update_model202207.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.template_variable_value import TemplateVariableValue
+    from criteo_api_retailmedia_v2023_07.model.template_variable_value import TemplateVariableValue
     globals()['TemplateVariableValue'] = TemplateVariableValue
 
 
 class CreativeUpdateModel202207(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/customer_list_details.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/customer_list_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class CustomerListDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/editable_campaign_attributes_v202301.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/editable_campaign_attributes_v202301.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class EditableCampaignAttributesV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/envelope_report_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_retailer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.report_request import ReportRequest
-    globals()['ReportRequest'] = ReportRequest
 
-
-class EnvelopeReportRequest(ModelNormal):
+class ExternalRetailer(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,66 +51,74 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('campaign_eligibilities',): {
+            'UNKNOWN': "unknown",
+            'AUCTION': "auction",
+            'PREFERRED': "preferred",
+        },
     }
 
     validations = {
+        ('name',): {
+            'max_length': 100,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': (ReportRequest,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'campaign_eligibilities': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'campaign_eligibilities': 'campaignEligibilities',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """EnvelopeReportRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
+        """ExternalRetailer - a model defined in OpenAPI
 
         Args:
-            data (ReportRequest):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,14 +143,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            campaign_eligibilities ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -170,15 +175,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -191,19 +196,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """EnvelopeReportRequest - a model defined in OpenAPI
+    def __init__(self, name, *args, **kwargs):  # noqa: E501
+        """ExternalRetailer - a model defined in OpenAPI
 
         Args:
-            data (ReportRequest):
+            name (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,14 +233,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            campaign_eligibilities ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -257,15 +263,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/envelope_report_status.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/hyperlink_variable_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.report_status import ReportStatus
-    globals()['ReportStatus'] = ReportStatus
 
-
-class EnvelopeReportStatus(ModelNormal):
+class HyperlinkVariableValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,55 +62,53 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': (ReportStatus,),  # noqa: E501
+            'url': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'url': 'url',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, data, *args, **kwargs):  # noqa: E501
-        """EnvelopeReportStatus - a model defined in OpenAPI
+    def _from_openapi_data(cls, url, *args, **kwargs):  # noqa: E501
+        """HyperlinkVariableValue - a model defined in OpenAPI
 
         Args:
-            data (ReportStatus):
+            url (str): The url to redirect to
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -170,15 +164,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -191,19 +185,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, data, *args, **kwargs):  # noqa: E501
-        """EnvelopeReportStatus - a model defined in OpenAPI
+    def __init__(self, url, *args, **kwargs):  # noqa: E501
+        """HyperlinkVariableValue - a model defined in OpenAPI
 
         Args:
-            data (ReportStatus):
+            url (str): The url to redirect to
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -257,15 +251,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
+        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/error.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_keyword_data_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.map_string import MapString
-    globals()['MapString'] = MapString
+    from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_input_keywords_model import RetailMediaExternalv1InputKeywordsModel
+    globals()['RetailMediaExternalv1InputKeywordsModel'] = RetailMediaExternalv1InputKeywordsModel
 
 
-class Error(ModelNormal):
+class RetailMediaExternalv1KeywordDataModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,22 +55,26 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('type',): {
-            'ACCESS-CONTROL': "access-control",
-            'AUTHENTICATION': "authentication",
-            'AUTHORIZATION': "authorization",
-            'AVAILABILITY': "availability",
-            'DEPRECATION': "deprecation",
-            'QUOTA': "quota",
-            'VALIDATION': "validation",
+        ('review_state',): {
+            'INREVIEW': "InReview",
+            'RECOMMENDED': "Recommended",
+            'APPROVED': "Approved",
+            'AUTOAPPROVED': "AutoApproved",
+            'REJECTED': "Rejected",
+            'AUTOREJECTED': "AutoRejected",
+        },
+        ('match_type',): {
+            'POSITIVEEXACTMATCH': "PositiveExactMatch",
+            'NEGATIVEEXACTMATCH': "NegativeExactMatch",
+            'NEGATIVEBROADMATCH': "NegativeBroadMatch",
         },
     }
 
     validations = {
     }
 
     @cached_property
@@ -92,55 +96,45 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'code': (str,),  # noqa: E501
-            'instance': (str,),  # noqa: E501
-            'trace_id': (str,),  # noqa: E501
-            'type': (str,),  # noqa: E501
-            'detail': (str,),  # noqa: E501
-            'source': (MapString,),  # noqa: E501
-            'stack_trace': ([str],),  # noqa: E501
-            'title': (str,),  # noqa: E501
+            'review_state': (str,),  # noqa: E501
+            'match_type': (str,),  # noqa: E501
+            'bid': (float,),  # noqa: E501
+            'input_keywords': (RetailMediaExternalv1InputKeywordsModel,),  # noqa: E501
+            'created_at': (datetime,),  # noqa: E501
+            'updated_at': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'code': 'code',  # noqa: E501
-        'instance': 'instance',  # noqa: E501
-        'trace_id': 'traceId',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'detail': 'detail',  # noqa: E501
-        'source': 'source',  # noqa: E501
-        'stack_trace': 'stackTrace',  # noqa: E501
-        'title': 'title',  # noqa: E501
+        'review_state': 'reviewState',  # noqa: E501
+        'match_type': 'matchType',  # noqa: E501
+        'bid': 'bid',  # noqa: E501
+        'input_keywords': 'inputKeywords',  # noqa: E501
+        'created_at': 'createdAt',  # noqa: E501
+        'updated_at': 'updatedAt',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, code, instance, trace_id, type, *args, **kwargs):  # noqa: E501
-        """Error - a model defined in OpenAPI
-
-        Args:
-            code (str): (REQUIRED) A machine-readable unique error code, expressed as a string value. The format used must be kabab-case.
-            instance (str): (REQUIRED) A URI reference that identifies the specific occurrence of the problem.
-            trace_id (str): (REQUIRED) The Correlation ID provided by the Gateway. It is also a unique identifier for this particular occurrence of the problem.
-            type (str): Type should be: \"validation\", \"unavailable, \"violation\", \"permission\", ...
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """RetailMediaExternalv1KeywordDataModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -165,18 +159,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            detail (str): (RECOMMENDED) A human-readable explanation specific to this occurrence of the problem.. [optional]  # noqa: E501
-            source (MapString): [optional]  # noqa: E501
-            stack_trace ([str]): (NEVER IN PRODUCTION) A human-readable stacktrace produced by the implementation technology e.g. .Net, Scala, etc. [optional]  # noqa: E501
-            title (str): (RECOMMENDED) A short, human-readable summary of the problem type.. [optional]  # noqa: E501
+            review_state (str): [optional]  # noqa: E501
+            match_type (str): [optional]  # noqa: E501
+            bid (float): [optional]  # noqa: E501
+            input_keywords (RetailMediaExternalv1InputKeywordsModel): [optional]  # noqa: E501
+            created_at (datetime): [optional]  # noqa: E501
+            updated_at (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -200,18 +196,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.code = code
-        self.instance = instance
-        self.trace_id = trace_id
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -224,22 +216,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, code, instance, trace_id, type, *args, **kwargs):  # noqa: E501
-        """Error - a model defined in OpenAPI
-
-        Args:
-            code (str): (REQUIRED) A machine-readable unique error code, expressed as a string value. The format used must be kabab-case.
-            instance (str): (REQUIRED) A URI reference that identifies the specific occurrence of the problem.
-            trace_id (str): (REQUIRED) The Correlation ID provided by the Gateway. It is also a unique identifier for this particular occurrence of the problem.
-            type (str): Type should be: \"validation\", \"unavailable, \"violation\", \"permission\", ...
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """RetailMediaExternalv1KeywordDataModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -264,18 +250,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            detail (str): (RECOMMENDED) A human-readable explanation specific to this occurrence of the problem.. [optional]  # noqa: E501
-            source (MapString): [optional]  # noqa: E501
-            stack_trace ([str]): (NEVER IN PRODUCTION) A human-readable stacktrace produced by the implementation technology e.g. .Net, Scala, etc. [optional]  # noqa: E501
-            title (str): (RECOMMENDED) A short, human-readable summary of the problem type.. [optional]  # noqa: E501
+            review_state (str): [optional]  # noqa: E501
+            match_type (str): [optional]  # noqa: E501
+            bid (float): [optional]  # noqa: E501
+            input_keywords (RetailMediaExternalv1InputKeywordsModel): [optional]  # noqa: E501
+            created_at (datetime): [optional]  # noqa: E501
+            updated_at (datetime): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -297,18 +285,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.code = code
-        self.instance = instance
-        self.trace_id = trace_id
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_account.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalAccount(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_add_to_basket_ids_update_model202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalAddToBasketIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_target202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_add_to_basket_target202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalAddToBasketTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_auction_line_item.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_auction_line_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalAuctionLineItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_create_model.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_auction_line_item_create_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalAuctionLineItemCreateModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_update_model.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_auction_line_item_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalAuctionLineItemUpdateModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_audience_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_audience_ids_update_model202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalAudienceIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_audience_target202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_audience_target202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalAudienceTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_balance202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_balance202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalBalance202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_brand.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_keyword_target202110.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
-class ExternalBrand(ModelNormal):
+class ExternalKeywordTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,21 +51,22 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('keywords',): {
+            'UNKNOWN': "unknown",
+            'NEGATIVEEXACT': "negativeExact",
+            'NEGATIVEBROAD': "negativeBroad",
+        },
     }
 
     validations = {
-        ('name',): {
-            'max_length': 120,
-            'min_length': 0,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -81,38 +82,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'name': (str,),  # noqa: E501
+            'keywords': ({str: (str,)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
+        'keywords': 'keywords',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """ExternalBrand - a model defined in OpenAPI
+    def _from_openapi_data(cls, keywords, *args, **kwargs):  # noqa: E501
+        """ExternalKeywordTarget202110 - a model defined in OpenAPI
 
         Args:
-            name (str):
+            keywords ({str: (str,)}): Keywords that targeting specifications exist for
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -168,15 +169,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
+        self.keywords = keywords
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,19 +190,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, *args, **kwargs):  # noqa: E501
-        """ExternalBrand - a model defined in OpenAPI
+    def __init__(self, keywords, *args, **kwargs):  # noqa: E501
+        """ExternalKeywordTarget202110 - a model defined in OpenAPI
 
         Args:
-            name (str):
+            keywords ({str: (str,)}): Keywords that targeting specifications exist for
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -255,15 +256,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
+        self.keywords = keywords
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_catalog_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_catalog_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalCatalogRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_catalog_status.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_catalog_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalCatalogStatus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_common_line_item.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_common_line_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalCommonLineItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_keyword_target202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/text_variable_value.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
-class ExternalKeywordTarget202110(ModelNormal):
+class TextVariableValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,19 +51,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('keywords',): {
-            'UNKNOWN': "unknown",
-            'NEGATIVEEXACT': "negativeExact",
-            'NEGATIVEBROAD': "negativeBroad",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -82,38 +77,38 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'keywords': ({str: (str,)},),  # noqa: E501
+            'text': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'keywords': 'keywords',  # noqa: E501
+        'text': 'text',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, keywords, *args, **kwargs):  # noqa: E501
-        """ExternalKeywordTarget202110 - a model defined in OpenAPI
+    def _from_openapi_data(cls, text, *args, **kwargs):  # noqa: E501
+        """TextVariableValue - a model defined in OpenAPI
 
         Args:
-            keywords ({str: (str,)}): Keywords that targeting specifications exist for
+            text (str): The displayed text
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -169,15 +164,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.keywords = keywords
+        self.text = text
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -190,19 +185,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, keywords, *args, **kwargs):  # noqa: E501
-        """ExternalKeywordTarget202110 - a model defined in OpenAPI
+    def __init__(self, text, *args, **kwargs):  # noqa: E501
+        """TextVariableValue - a model defined in OpenAPI
 
         Args:
-            keywords ({str: (str,)}): Keywords that targeting specifications exist for
+            text (str): The displayed text
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -256,15 +251,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.keywords = keywords
+        self.text = text
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_line_item_capping202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_line_item_capping202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalLineItemCapping202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_line_item_page202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_line_item_page202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_line_item_page_category202110 import ExternalLineItemPageCategory202110
+    from criteo_api_retailmedia_v2023_07.model.external_line_item_page_category202110 import ExternalLineItemPageCategory202110
     globals()['ExternalLineItemPageCategory202110'] = ExternalLineItemPageCategory202110
 
 
 class ExternalLineItemPage202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_line_item_page_category202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_line_item_page_category202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalLineItemPageCategory202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_preferred_line_item202110.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_line_item_capping202110 import ExternalLineItemCapping202110
-    from criteo_api_retailmedia_v2023_04.model.external_line_item_page202110 import ExternalLineItemPage202110
+    from criteo_api_retailmedia_v2023_07.model.external_line_item_capping202110 import ExternalLineItemCapping202110
+    from criteo_api_retailmedia_v2023_07.model.external_line_item_page202110 import ExternalLineItemPage202110
     globals()['ExternalLineItemCapping202110'] = ExternalLineItemCapping202110
     globals()['ExternalLineItemPage202110'] = ExternalLineItemPage202110
 
 
 class ExternalPreferredLineItem202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_create_model202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_preferred_line_item_create_model202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_line_item_capping202110 import ExternalLineItemCapping202110
-    from criteo_api_retailmedia_v2023_04.model.external_line_item_page202110 import ExternalLineItemPage202110
+    from criteo_api_retailmedia_v2023_07.model.external_line_item_capping202110 import ExternalLineItemCapping202110
+    from criteo_api_retailmedia_v2023_07.model.external_line_item_page202110 import ExternalLineItemPage202110
     globals()['ExternalLineItemCapping202110'] = ExternalLineItemCapping202110
     globals()['ExternalLineItemPage202110'] = ExternalLineItemPage202110
 
 
 class ExternalPreferredLineItemCreateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_preferred_line_item_update_model202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_line_item_capping202110 import ExternalLineItemCapping202110
-    from criteo_api_retailmedia_v2023_04.model.external_line_item_page202110 import ExternalLineItemPage202110
+    from criteo_api_retailmedia_v2023_07.model.external_line_item_capping202110 import ExternalLineItemCapping202110
+    from criteo_api_retailmedia_v2023_07.model.external_line_item_page202110 import ExternalLineItemPage202110
     globals()['ExternalLineItemCapping202110'] = ExternalLineItemCapping202110
     globals()['ExternalLineItemPage202110'] = ExternalLineItemPage202110
 
 
 class ExternalPreferredLineItemUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_promoted_product202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_promoted_product202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalPromotedProduct202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_retailer.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_retailer_pages202110.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
-class ExternalRetailer(ModelNormal):
+class ExternalRetailerPages202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,25 +51,17 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('campaign_eligibilities',): {
-            'UNKNOWN': "unknown",
-            'AUCTION': "auction",
-            'PREFERRED': "preferred",
-        },
     }
 
     validations = {
-        ('name',): {
-            'max_length': 100,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -85,40 +77,35 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'name': (str,),  # noqa: E501
-            'campaign_eligibilities': ([str],),  # noqa: E501
+            'page_types': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'campaign_eligibilities': 'campaignEligibilities',  # noqa: E501
+        'page_types': 'pageTypes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """ExternalRetailer - a model defined in OpenAPI
-
-        Args:
-            name (str):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """ExternalRetailerPages202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,15 +130,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            campaign_eligibilities ([str]): [optional]  # noqa: E501
+            page_types ([str]): List of valid pages for a retailer. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -175,15 +162,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -196,19 +182,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, name, *args, **kwargs):  # noqa: E501
-        """ExternalRetailer - a model defined in OpenAPI
-
-        Args:
-            name (str):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """ExternalRetailerPages202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -233,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            campaign_eligibilities ([str]): [optional]  # noqa: E501
+            page_types ([str]): List of valid pages for a retailer. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -263,15 +246,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.name = name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_retailer_pages202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_set_bid_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
-class ExternalRetailerPages202110(ModelNormal):
+class RetailMediaExternalv1SetBidModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -54,14 +54,18 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('phrase',): {
+            'max_length': 255,
+            'min_length': 0,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -77,35 +81,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'page_types': ([str],),  # noqa: E501
+            'phrase': (str,),  # noqa: E501
+            'bid': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'page_types': 'pageTypes',  # noqa: E501
+        'phrase': 'phrase',  # noqa: E501
+        'bid': 'bid',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ExternalRetailerPages202110 - a model defined in OpenAPI
+        """RetailMediaExternalv1SetBidModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,15 +136,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            page_types ([str]): List of valid pages for a retailer. [optional]  # noqa: E501
+            phrase (str): [optional]  # noqa: E501
+            bid (float): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +190,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ExternalRetailerPages202110 - a model defined in OpenAPI
+        """RetailMediaExternalv1SetBidModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +223,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            page_types ([str]): List of valid pages for a retailer. [optional]  # noqa: E501
+            phrase (str): [optional]  # noqa: E501
+            bid (float): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_store_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_store_ids_update_model202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalStoreIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/external_store_target202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/external_store_target202110.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ExternalStoreTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/files_variable_value.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/files_variable_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class FilesVariableValue(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/files_variables_specification.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/files_variables_specification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class FilesVariablesSpecification(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/get_page_of_audiences_by_account_id_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_audience_v2_list_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_04.model.retail_media_audience import RetailMediaAudience
-    globals()['CommonError'] = CommonError
-    globals()['CommonWarning'] = CommonWarning
+    from criteo_api_retailmedia_v2023_07.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2023_07.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_07.model.retail_media_audience_v2 import RetailMediaAudienceV2
+    globals()['CommonProblem'] = CommonProblem
     globals()['PageMetadata'] = PageMetadata
-    globals()['RetailMediaAudience'] = RetailMediaAudience
+    globals()['RetailMediaAudienceV2'] = RetailMediaAudienceV2
 
 
-class GetPageOfAudiencesByAccountIdResponse(ModelNormal):
+class RetailMediaAudienceV2ListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -89,18 +87,18 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([RetailMediaAudience],),  # noqa: E501
+            'data': ([RetailMediaAudienceV2],),  # noqa: E501
             'metadata': (PageMetadata,),  # noqa: E501
-            'errors': ([CommonError],),  # noqa: E501
-            'warnings': ([CommonWarning],),  # noqa: E501
+            'errors': ([CommonProblem],),  # noqa: E501
+            'warnings': ([CommonProblem],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -118,18 +116,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, data, metadata, *args, **kwargs):  # noqa: E501
-        """GetPageOfAudiencesByAccountIdResponse - a model defined in OpenAPI
+        """RetailMediaAudienceV2ListResponse - a model defined in OpenAPI
 
         Args:
-            data ([RetailMediaAudience]): data
+            data ([RetailMediaAudienceV2]): data
             metadata (PageMetadata):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -155,16 +153,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            errors ([CommonError]): errors. [optional]  # noqa: E501
-            warnings ([CommonWarning]): warnings. [optional]  # noqa: E501
+            errors ([CommonProblem]): errors. [optional]  # noqa: E501
+            warnings ([CommonProblem]): warnings. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -211,15 +209,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, metadata, *args, **kwargs):  # noqa: E501
-        """GetPageOfAudiencesByAccountIdResponse - a model defined in OpenAPI
+        """RetailMediaAudienceV2ListResponse - a model defined in OpenAPI
 
             metadata (PageMetadata):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -246,16 +244,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            errors ([CommonError]): errors. [optional]  # noqa: E501
-            warnings ([CommonWarning]): warnings. [optional]  # noqa: E501
+            errors ([CommonProblem]): errors. [optional]  # noqa: E501
+            warnings ([CommonProblem]): warnings. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/hyperlink_variable_value.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/line_item_report_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from criteo_api_retailmedia_v2023_07.model.line_item_report import LineItemReport
+    globals()['LineItemReport'] = LineItemReport
 
-class HyperlinkVariableValue(ModelNormal):
+
+class LineItemReportResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,53 +66,54 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'url': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'attributes': (LineItemReport,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'url': 'url',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, url, *args, **kwargs):  # noqa: E501
-        """HyperlinkVariableValue - a model defined in OpenAPI
-
-        Args:
-            url (str): The url to redirect to
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """LineItemReportResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,14 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            type (str): [optional]  # noqa: E501
+            attributes (LineItemReport): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -164,15 +171,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -185,19 +191,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, url, *args, **kwargs):  # noqa: E501
-        """HyperlinkVariableValue - a model defined in OpenAPI
-
-        Args:
-            url (str): The url to redirect to
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """LineItemReportResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,14 +225,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            type (str): [optional]  # noqa: E501
+            attributes (LineItemReport): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -251,15 +256,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.url = url
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/input_resource_of_auction_line_item_create_model.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/input_resource_of_auction_line_item_create_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_auction_line_item_create_model import ExternalAuctionLineItemCreateModel
+    from criteo_api_retailmedia_v2023_07.model.external_auction_line_item_create_model import ExternalAuctionLineItemCreateModel
     globals()['ExternalAuctionLineItemCreateModel'] = ExternalAuctionLineItemCreateModel
 
 
 class InputResourceOfAuctionLineItemCreateModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/input_resource_of_preferred_line_item_create_model202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/input_resource_of_preferred_line_item_create_model202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_preferred_line_item_create_model202110 import ExternalPreferredLineItemCreateModel202110
+    from criteo_api_retailmedia_v2023_07.model.external_preferred_line_item_create_model202110 import ExternalPreferredLineItemCreateModel202110
     globals()['ExternalPreferredLineItemCreateModel202110'] = ExternalPreferredLineItemCreateModel202110
 
 
 class InputResourceOfPreferredLineItemCreateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.editable_campaign_attributes_v202301 import EditableCampaignAttributesV202301
+    from criteo_api_retailmedia_v2023_07.model.editable_campaign_attributes_v202301 import EditableCampaignAttributesV202301
     globals()['EditableCampaignAttributesV202301'] = EditableCampaignAttributesV202301
 
 
 class JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_account_and_account.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_account_and_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_account import ExternalAccount
+    from criteo_api_retailmedia_v2023_07.model.external_account import ExternalAccount
     globals()['ExternalAccount'] = ExternalAccount
 
 
 class JsonApiBodyWithIdOfInt64AndAccountAndAccount(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_brand_and_brand.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_brand_and_brand.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_brand import ExternalBrand
+    from criteo_api_retailmedia_v2023_07.model.external_brand import ExternalBrand
     globals()['ExternalBrand'] = ExternalBrand
 
 
 class JsonApiBodyWithIdOfInt64AndBrandAndBrand(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.campaign_v202301 import CampaignV202301
+    from criteo_api_retailmedia_v2023_07.model.campaign_v202301 import CampaignV202301
     globals()['CampaignV202301'] = CampaignV202301
 
 
 class JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_catalog_status import ExternalCatalogStatus
+    from criteo_api_retailmedia_v2023_07.model.external_catalog_status import ExternalCatalogStatus
     globals()['ExternalCatalogStatus'] = ExternalCatalogStatus
 
 
 class JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.line_item_bid_multipliers import LineItemBidMultipliers
+    from criteo_api_retailmedia_v2023_07.model.line_item_bid_multipliers import LineItemBidMultipliers
     globals()['LineItemBidMultipliers'] = LineItemBidMultipliers
 
 
 class JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_retailer import ExternalRetailer
+    from criteo_api_retailmedia_v2023_07.model.external_retailer import ExternalRetailer
     globals()['ExternalRetailer'] = ExternalRetailer
 
 
 class JsonApiBodyWithIdOfInt64AndRetailerAndRetailer(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.campaign_attributes_v202301 import CampaignAttributesV202301
+    from criteo_api_retailmedia_v2023_07.model.campaign_attributes_v202301 import CampaignAttributesV202301
     globals()['CampaignAttributesV202301'] = CampaignAttributesV202301
 
 
 class JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_catalog_request import ExternalCatalogRequest
+    from criteo_api_retailmedia_v2023_07.model.external_catalog_request import ExternalCatalogRequest
     globals()['ExternalCatalogRequest'] = ExternalCatalogRequest
 
 
 class JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_account.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_page_response_of_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_account_and_account import JsonApiBodyWithIdOfInt64AndAccountAndAccount
-    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_07.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_07.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_07.model.json_api_body_with_id_of_int64_and_account_and_account import JsonApiBodyWithIdOfInt64AndAccountAndAccount
+    from criteo_api_retailmedia_v2023_07.model.page_metadata import PageMetadata
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndAccountAndAccount'] = JsonApiBodyWithIdOfInt64AndAccountAndAccount
     globals()['PageMetadata'] = PageMetadata
 
 
 class JsonApiPageResponseOfAccount(ModelNormal):
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_brand.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_page_response_of_brand.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_brand_and_brand import JsonApiBodyWithIdOfInt64AndBrandAndBrand
-    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_07.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_07.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_07.model.json_api_body_with_id_of_int64_and_brand_and_brand import JsonApiBodyWithIdOfInt64AndBrandAndBrand
+    from criteo_api_retailmedia_v2023_07.model.page_metadata import PageMetadata
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndBrandAndBrand'] = JsonApiBodyWithIdOfInt64AndBrandAndBrand
     globals()['PageMetadata'] = PageMetadata
 
 
 class JsonApiPageResponseOfBrand(ModelNormal):
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_page_response_of_campaign_v202301.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
-    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_07.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_07.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_07.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
+    from criteo_api_retailmedia_v2023_07.model.page_metadata import PageMetadata
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301'] = JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
     globals()['PageMetadata'] = PageMetadata
 
 
 class JsonApiPageResponseOfCampaignV202301(ModelNormal):
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_retailer.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_page_response_of_retailer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_retailer_and_retailer import JsonApiBodyWithIdOfInt64AndRetailerAndRetailer
-    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_07.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_07.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_07.model.json_api_body_with_id_of_int64_and_retailer_and_retailer import JsonApiBodyWithIdOfInt64AndRetailerAndRetailer
+    from criteo_api_retailmedia_v2023_07.model.page_metadata import PageMetadata
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndRetailerAndRetailer'] = JsonApiBodyWithIdOfInt64AndRetailerAndRetailer
     globals()['PageMetadata'] = PageMetadata
 
 
 class JsonApiPageResponseOfRetailer(ModelNormal):
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_request_of_catalog_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_request_of_catalog_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.json_api_body_without_id_of_catalog_request_and_catalog_request import JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest
+    from criteo_api_retailmedia_v2023_07.model.json_api_body_without_id_of_catalog_request_and_catalog_request import JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest
     globals()['JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest'] = JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest
 
 
 class JsonApiRequestOfCatalogRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_single_response_of_campaign_v202301.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
+    from criteo_api_retailmedia_v2023_07.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_07.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_07.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301'] = JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
 
 
 class JsonApiSingleResponseOfCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_catalog_status.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_single_response_of_catalog_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status import JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus
+    from criteo_api_retailmedia_v2023_07.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_07.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_07.model.json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status import JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus'] = JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus
 
 
 class JsonApiSingleResponseOfCatalogStatus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/json_api_single_response_of_line_item_bid_multipliers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
-    from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
-    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers import JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers
+    from criteo_api_retailmedia_v2023_07.model.common_error import CommonError
+    from criteo_api_retailmedia_v2023_07.model.common_warning import CommonWarning
+    from criteo_api_retailmedia_v2023_07.model.json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers import JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers
     globals()['CommonError'] = CommonError
     globals()['CommonWarning'] = CommonWarning
     globals()['JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers'] = JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers
 
 
 class JsonApiSingleResponseOfLineItemBidMultipliers(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/keyword_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/keyword_target202110_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
+    from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
     globals()['ValueTypeResourceOfKeywordTarget202110'] = ValueTypeResourceOfKeywordTarget202110
 
 
 class KeywordTarget202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/keyword_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/keyword_target202110_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ValueTypeResourceOfKeywordTarget202110'] = ValueTypeResourceOfKeywordTarget202110
 
 
 class KeywordTarget202110Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/line_item_bid_multipliers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class LineItemBidMultipliers(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/line_item_bid_multipliers_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
+    from criteo_api_retailmedia_v2023_07.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
     globals()['ResourceOfLineItemBidMultipliers'] = ResourceOfLineItemBidMultipliers
 
 
 class LineItemBidMultipliersRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/line_item_bid_multipliers_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfLineItemBidMultipliers'] = ResourceOfLineItemBidMultipliers
 
 
 class LineItemBidMultipliersResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/map_string.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/line_item_report_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from criteo_api_retailmedia_v2023_07.model.line_item_report_resource import LineItemReportResource
+    globals()['LineItemReportResource'] = LineItemReportResource
 
-class MapString(ModelNormal):
+
+class LineItemReportRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,48 +66,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        return (str,)  # noqa: E501
+        lazy_import()
+        return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
+            'data': (LineItemReportResource,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """MapString - a model defined in OpenAPI
+        """LineItemReportRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -128,14 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            data (LineItemReportResource): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -180,15 +189,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """MapString - a model defined in OpenAPI
+        """LineItemReportRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,14 +222,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            data (LineItemReportResource): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/page_metadata.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/page_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class PageMetadata(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/page_type_environment.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/page_type_environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class PageTypeEnvironment(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/post_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/post_campaign_v202301.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301
+    from criteo_api_retailmedia_v2023_07.model.json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301
     globals()['JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301'] = JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301
 
 
 class PostCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/preferred_line_item202110_paged_list_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
+    from criteo_api_retailmedia_v2023_07.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfPreferredLineItem202110'] = ResourceOfPreferredLineItem202110
 
 
 class PreferredLineItem202110PagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/preferred_line_item202110_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfPreferredLineItem202110'] = ResourceOfPreferredLineItem202110
 
 
 class PreferredLineItem202110Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/preferred_line_item_create_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/preferred_line_item_create_model202110_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.input_resource_of_preferred_line_item_create_model202110 import InputResourceOfPreferredLineItemCreateModel202110
+    from criteo_api_retailmedia_v2023_07.model.input_resource_of_preferred_line_item_create_model202110 import InputResourceOfPreferredLineItemCreateModel202110
     globals()['InputResourceOfPreferredLineItemCreateModel202110'] = InputResourceOfPreferredLineItemCreateModel202110
 
 
 class PreferredLineItemCreateModel202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/preferred_line_item_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/preferred_line_item_update_model202110_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.resource_of_preferred_line_item_update_model202110 import ResourceOfPreferredLineItemUpdateModel202110
+    from criteo_api_retailmedia_v2023_07.model.resource_of_preferred_line_item_update_model202110 import ResourceOfPreferredLineItemUpdateModel202110
     globals()['ResourceOfPreferredLineItemUpdateModel202110'] = ResourceOfPreferredLineItemUpdateModel202110
 
 
 class PreferredLineItemUpdateModel202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/problem_details.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ProblemDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/promoted_product202110_list_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/promoted_product202110_list_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
+    from criteo_api_retailmedia_v2023_07.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
     globals()['ResourceOfPromotedProduct202110'] = ResourceOfPromotedProduct202110
 
 
 class PromotedProduct202110ListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/promoted_product202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/promoted_product202110_paged_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
+    from criteo_api_retailmedia_v2023_07.model.page_metadata import PageMetadata
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
     globals()['PageMetadata'] = PageMetadata
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfPromotedProduct202110'] = ResourceOfPromotedProduct202110
 
 
 class PromotedProduct202110PagedListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/put_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/put_campaign_v202301.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301
+    from criteo_api_retailmedia_v2023_07.model.json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301
     globals()['JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301'] = JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301
 
 
 class PutCampaignV202301(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/report_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_auction_line_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.report_request_attributes import ReportRequestAttributes
-    globals()['ReportRequestAttributes'] = ReportRequestAttributes
+    from criteo_api_retailmedia_v2023_07.model.external_auction_line_item import ExternalAuctionLineItem
+    globals()['ExternalAuctionLineItem'] = ExternalAuctionLineItem
 
 
-class ReportRequest(ModelNormal):
+class ResourceOfAuctionLineItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,41 +83,39 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'attributes': (ReportRequestAttributes,),  # noqa: E501
+            'id': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
+            'attributes': (ExternalAuctionLineItem,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'attributes': 'attributes',  # noqa: E501
+        'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, attributes, type, *args, **kwargs):  # noqa: E501
-        """ReportRequest - a model defined in OpenAPI
-
-        Args:
-            attributes (ReportRequestAttributes):
-            type (str): Always \"RetailMediaReportRequest\"
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """ResourceOfAuctionLineItem - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,14 +140,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            id (str): Id of the entity. [optional]  # noqa: E501
+            type (str): Canonical type name of the entity. [optional]  # noqa: E501
+            attributes (ExternalAuctionLineItem): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -173,16 +174,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.attributes = attributes
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -195,20 +194,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, attributes, type, *args, **kwargs):  # noqa: E501
-        """ReportRequest - a model defined in OpenAPI
-
-        Args:
-            attributes (ReportRequestAttributes):
-            type (str): Always \"RetailMediaReportRequest\"
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """ResourceOfAuctionLineItem - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -233,14 +228,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            id (str): Id of the entity. [optional]  # noqa: E501
+            type (str): Canonical type name of the entity. [optional]  # noqa: E501
+            attributes (ExternalAuctionLineItem): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -262,16 +260,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.attributes = attributes
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/report_request_attributes.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/line_item_report.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
-class ReportRequestAttributes(ModelNormal):
+class LineItemReport(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -53,37 +53,73 @@
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('report_type',): {
             'SUMMARY': "summary",
-            'KEYWORD': "keyword",
             'PAGETYPE': "pageType",
+            'KEYWORD': "keyword",
             'PRODUCTCATEGORY': "productCategory",
             'PRODUCT': "product",
-            'ATTRIBUTEDTRANSACTIONS': "attributedTransactions",
+        },
+        ('metrics',): {
+            'IMPRESSIONS': "impressions",
+            'CLICKS': "clicks",
+            'SPEND': "spend",
+            'ATTRIBUTEDSALES': "attributedSales",
+            'ATTRIBUTEDUNITS': "attributedUnits",
+            'ATTRIBUTEDORDERS': "attributedOrders",
+            'CTR': "ctr",
+            'CPC': "cpc",
+            'CPO': "cpo",
+            'ROAS': "roas",
+            'ASSISTEDUNITS': "assistedUnits",
+            'ASSISTEDSALES': "assistedSales",
+            'UNIQUEVISITORS': "uniqueVisitors",
+            'FREQUENCY': "frequency",
+        },
+        ('dimensions',): {
+            'DATE': "date",
+            'CAMPAIGNID': "campaignId",
+            'CAMPAIGNNAME': "campaignName",
+            'CAMPAIGNTYPENAME': "campaignTypeName",
+            'ADVPRODUCTCATEGORY': "advProductCategory",
+            'ADVPRODUCTID': "advProductId",
+            'ADVPRODUCTNAME': "advProductName",
+            'BRANDID': "brandId",
+            'BRANDNAME': "brandName",
+            'LINEITEMID': "lineItemId",
+            'LINEITEMNAME': "lineItemName",
+            'RETAILERID': "retailerId",
+            'RETAILERNAME': "retailerName",
+            'KEYWORD': "keyword",
+            'PAGETYPENAME': "pageTypeName",
+            'SALESCHANNEL': "salesChannel",
         },
         ('click_attribution_window',): {
             '7D': "7D",
             '14D': "14D",
             '30D': "30D",
-        },
-        ('format',): {
-            'CSV': "csv",
-            'JSON': "json",
-            'JSON-COMPACT': "json-compact",
-            'JSON-NEWLINE': "json-newline",
+            'NONE': "none",
         },
         ('view_attribution_window',): {
-            'NONE': "none",
             '1D': "1D",
             '7D': "7D",
             '14D': "14D",
             '30D': "30D",
+            'NONE': "none",
+        },
+        ('campaign_type',): {
+            'SPONSOREDPRODUCTS': "sponsoredProducts",
+            'ONSITEDISPLAYS': "onSiteDisplays",
+        },
+        ('sales_channel',): {
+            'OFFLINE': "offline",
+            'ONLINE': "online",
         },
     }
 
     validations = {
     }
 
     @cached_property
@@ -103,58 +139,64 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'end_date': (date,),  # noqa: E501
+            'account_id': (str,),  # noqa: E501
+            'start_date': (datetime,),  # noqa: E501
+            'end_date': (datetime,),  # noqa: E501
             'report_type': (str,),  # noqa: E501
-            'start_date': (date,),  # noqa: E501
+            'line_item_ids': ([str],),  # noqa: E501
+            'campaign_ids': ([str],),  # noqa: E501
+            'metrics': ([str],),  # noqa: E501
+            'dimensions': ([str],),  # noqa: E501
+            'timezone': (str,),  # noqa: E501
             'click_attribution_window': (str,),  # noqa: E501
-            'format': (str,),  # noqa: E501
-            'id': (str,),  # noqa: E501
-            'ids': ([str],),  # noqa: E501
-            'revenue_type': (str,),  # noqa: E501
-            'time_zone': (str,),  # noqa: E501
             'view_attribution_window': (str,),  # noqa: E501
+            'campaign_type': (str,),  # noqa: E501
+            'sales_channel': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'account_id': 'accountId',  # noqa: E501
+        'start_date': 'startDate',  # noqa: E501
         'end_date': 'endDate',  # noqa: E501
         'report_type': 'reportType',  # noqa: E501
-        'start_date': 'startDate',  # noqa: E501
+        'line_item_ids': 'lineItemIds',  # noqa: E501
+        'campaign_ids': 'campaignIds',  # noqa: E501
+        'metrics': 'metrics',  # noqa: E501
+        'dimensions': 'dimensions',  # noqa: E501
+        'timezone': 'timezone',  # noqa: E501
         'click_attribution_window': 'clickAttributionWindow',  # noqa: E501
-        'format': 'format',  # noqa: E501
-        'id': 'id',  # noqa: E501
-        'ids': 'ids',  # noqa: E501
-        'revenue_type': 'revenueType',  # noqa: E501
-        'time_zone': 'timeZone',  # noqa: E501
         'view_attribution_window': 'viewAttributionWindow',  # noqa: E501
+        'campaign_type': 'campaignType',  # noqa: E501
+        'sales_channel': 'salesChannel',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, end_date, report_type, start_date, *args, **kwargs):  # noqa: E501
-        """ReportRequestAttributes - a model defined in OpenAPI
+    def _from_openapi_data(cls, account_id, start_date, end_date, *args, **kwargs):  # noqa: E501
+        """LineItemReport - a model defined in OpenAPI
 
         Args:
-            end_date (date): YYYY-MM-DD, must not be before startDate and not more than 100 days later
-            report_type (str): One of \"summary\", \"keyword\", \"pageType\", \"productCategory\", \"product\", or \"attributedTransactions\"
-            start_date (date): YYYY-MM-DD
+            account_id (str):
+            start_date (datetime):
+            end_date (datetime):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -179,21 +221,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            click_attribution_window (str): Defaults to value from campaign or one of \"7D\", \"14D\", or \"30D\". If specified, viewAttributionWindow must also be specified. [optional]  # noqa: E501
-            format (str): One of \"json\" (default),\"json-compact\",\"json-newline\" or \"csv\". [optional] if omitted the server will use the default value of "json"  # noqa: E501
-            id (str): The id of the campaign or line item.  Either 'id' or 'ids' must be specified, but not both. [optional]  # noqa: E501
-            ids ([str]): The ids of the campaigns or line items.  Either 'id' or 'ids' must be specified, but not both. [optional]  # noqa: E501
-            revenue_type (str): [optional]  # noqa: E501
-            time_zone (str): [optional]  # noqa: E501
-            view_attribution_window (str): Defaults to value from campaign or one of \"none\", \"1D\", \"7D\", \"14D\", or \"30D\". If specified, must be less than clickAttributionWindow, which must also be specified.. [optional]  # noqa: E501
+            report_type (str): [optional]  # noqa: E501
+            line_item_ids ([str]): [optional]  # noqa: E501
+            campaign_ids ([str]): [optional]  # noqa: E501
+            metrics ([str]): [optional]  # noqa: E501
+            dimensions ([str]): List of dimensions to report on. [optional]  # noqa: E501
+            timezone (str): [optional]  # noqa: E501
+            click_attribution_window (str): [optional]  # noqa: E501
+            view_attribution_window (str): [optional]  # noqa: E501
+            campaign_type (str): [optional]  # noqa: E501
+            sales_channel (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -217,17 +262,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.end_date = end_date
-        self.report_type = report_type
+        self.account_id = account_id
         self.start_date = start_date
+        self.end_date = end_date
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -240,21 +285,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, end_date, report_type, start_date, *args, **kwargs):  # noqa: E501
-        """ReportRequestAttributes - a model defined in OpenAPI
+    def __init__(self, account_id, start_date, end_date, *args, **kwargs):  # noqa: E501
+        """LineItemReport - a model defined in OpenAPI
 
         Args:
-            end_date (date): YYYY-MM-DD, must not be before startDate and not more than 100 days later
-            report_type (str): One of \"summary\", \"keyword\", \"pageType\", \"productCategory\", \"product\", or \"attributedTransactions\"
-            start_date (date): YYYY-MM-DD
+            account_id (str):
+            start_date (datetime):
+            end_date (datetime):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -279,21 +324,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            click_attribution_window (str): Defaults to value from campaign or one of \"7D\", \"14D\", or \"30D\". If specified, viewAttributionWindow must also be specified. [optional]  # noqa: E501
-            format (str): One of \"json\" (default),\"json-compact\",\"json-newline\" or \"csv\". [optional] if omitted the server will use the default value of "json"  # noqa: E501
-            id (str): The id of the campaign or line item.  Either 'id' or 'ids' must be specified, but not both. [optional]  # noqa: E501
-            ids ([str]): The ids of the campaigns or line items.  Either 'id' or 'ids' must be specified, but not both. [optional]  # noqa: E501
-            revenue_type (str): [optional]  # noqa: E501
-            time_zone (str): [optional]  # noqa: E501
-            view_attribution_window (str): Defaults to value from campaign or one of \"none\", \"1D\", \"7D\", \"14D\", or \"30D\". If specified, must be less than clickAttributionWindow, which must also be specified.. [optional]  # noqa: E501
+            report_type (str): [optional]  # noqa: E501
+            line_item_ids ([str]): [optional]  # noqa: E501
+            campaign_ids ([str]): [optional]  # noqa: E501
+            metrics ([str]): [optional]  # noqa: E501
+            dimensions ([str]): List of dimensions to report on. [optional]  # noqa: E501
+            timezone (str): [optional]  # noqa: E501
+            click_attribution_window (str): [optional]  # noqa: E501
+            view_attribution_window (str): [optional]  # noqa: E501
+            campaign_type (str): [optional]  # noqa: E501
+            sales_channel (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -315,17 +363,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.end_date = end_date
-        self.report_type = report_type
+        self.account_id = account_id
         self.start_date = start_date
+        self.end_date = end_date
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/report_status.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/text_variable_specification.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.report_status_attributes import ReportStatusAttributes
-    globals()['ReportStatusAttributes'] = ReportStatusAttributes
 
-
-class ReportStatus(ModelNormal):
+class TextVariableSpecification(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,61 +62,50 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'attributes': (ReportStatusAttributes,),  # noqa: E501
-            'id': (str,),  # noqa: E501
-            'type': (str,),  # noqa: E501
+            'max_chars': (int, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'attributes': 'attributes',  # noqa: E501
-        'id': 'id',  # noqa: E501
-        'type': 'type',  # noqa: E501
+        'max_chars': 'maxChars',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, attributes, id, type, *args, **kwargs):  # noqa: E501
-        """ReportStatus - a model defined in OpenAPI
-
-        Args:
-            attributes (ReportStatusAttributes):
-            id (str): The reportId
-            type (str): Always \"RetailMediaReportStatus\"
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """TextVariableSpecification - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -145,14 +130,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            max_chars (int, none_type): The maximum amount of characters accepted for the text. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -176,17 +162,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.attributes = attributes
-        self.id = id
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -199,21 +182,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, attributes, id, type, *args, **kwargs):  # noqa: E501
-        """ReportStatus - a model defined in OpenAPI
-
-        Args:
-            attributes (ReportStatusAttributes):
-            id (str): The reportId
-            type (str): Always \"RetailMediaReportStatus\"
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """TextVariableSpecification - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -238,14 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            max_chars (int, none_type): The maximum amount of characters accepted for the text. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -267,17 +246,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.attributes = attributes
-        self.id = id
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/report_status_attributes.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/status_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
-class ReportStatusAttributes(ModelNormal):
+class StatusResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,49 +84,48 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'status': (str,),  # noqa: E501
-            'created_at': (datetime,),  # noqa: E501
-            'expires_at': (datetime,),  # noqa: E501
+            'row_count': (int,),  # noqa: E501
             'file_size_bytes': (int,),  # noqa: E501
-            'md5_checksum': (str,),  # noqa: E501
+            'md5_check_sum': (str,),  # noqa: E501
+            'created_at': (str,),  # noqa: E501
+            'expires_at': (str,),  # noqa: E501
             'message': (str,),  # noqa: E501
-            'row_count': (int,),  # noqa: E501
+            'id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'status': 'status',  # noqa: E501
+        'row_count': 'rowCount',  # noqa: E501
+        'file_size_bytes': 'fileSizeBytes',  # noqa: E501
+        'md5_check_sum': 'md5CheckSum',  # noqa: E501
         'created_at': 'createdAt',  # noqa: E501
         'expires_at': 'expiresAt',  # noqa: E501
-        'file_size_bytes': 'fileSizeBytes',  # noqa: E501
-        'md5_checksum': 'md5Checksum',  # noqa: E501
         'message': 'message',  # noqa: E501
-        'row_count': 'rowCount',  # noqa: E501
+        'id': 'id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, status, *args, **kwargs):  # noqa: E501
-        """ReportStatusAttributes - a model defined in OpenAPI
-
-        Args:
-            status (str): One of \"pending\", \"success\", \"failure\", or \"expired\"
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """StatusResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -151,20 +150,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            created_at (datetime): Timestamp when the report started to execute. [optional]  # noqa: E501
-            expires_at (datetime): Timestamp when the cached report will expire. [optional]  # noqa: E501
-            file_size_bytes (int): Total size of file, only populated on success. [optional]  # noqa: E501
-            md5_checksum (str): The MD5 checksum of the content, only populated on success. [optional]  # noqa: E501
-            message (str): Failure message, only populated on failure. [optional]  # noqa: E501
-            row_count (int): Rows of data in report, only populated on success. [optional]  # noqa: E501
+            status (str): [optional]  # noqa: E501
+            row_count (int): [optional]  # noqa: E501
+            file_size_bytes (int): [optional]  # noqa: E501
+            md5_check_sum (str): [optional]  # noqa: E501
+            created_at (str): [optional]  # noqa: E501
+            expires_at (str): [optional]  # noqa: E501
+            message (str): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +189,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.status = status
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -209,19 +209,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, status, *args, **kwargs):  # noqa: E501
-        """ReportStatusAttributes - a model defined in OpenAPI
-
-        Args:
-            status (str): One of \"pending\", \"success\", \"failure\", or \"expired\"
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """StatusResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -246,20 +243,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            created_at (datetime): Timestamp when the report started to execute. [optional]  # noqa: E501
-            expires_at (datetime): Timestamp when the cached report will expire. [optional]  # noqa: E501
-            file_size_bytes (int): Total size of file, only populated on success. [optional]  # noqa: E501
-            md5_checksum (str): The MD5 checksum of the content, only populated on success. [optional]  # noqa: E501
-            message (str): Failure message, only populated on failure. [optional]  # noqa: E501
-            row_count (int): Rows of data in report, only populated on success. [optional]  # noqa: E501
+            status (str): [optional]  # noqa: E501
+            row_count (int): [optional]  # noqa: E501
+            file_size_bytes (int): [optional]  # noqa: E501
+            md5_check_sum (str): [optional]  # noqa: E501
+            created_at (str): [optional]  # noqa: E501
+            expires_at (str): [optional]  # noqa: E501
+            message (str): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -281,15 +280,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.status = status
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_auction_line_item_update_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_auction_line_item import ExternalAuctionLineItem
-    globals()['ExternalAuctionLineItem'] = ExternalAuctionLineItem
+    from criteo_api_retailmedia_v2023_07.model.external_auction_line_item_update_model import ExternalAuctionLineItemUpdateModel
+    globals()['ExternalAuctionLineItemUpdateModel'] = ExternalAuctionLineItemUpdateModel
 
 
-class ResourceOfAuctionLineItem(ModelNormal):
+class ResourceOfAuctionLineItemUpdateModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
-            'attributes': (ExternalAuctionLineItem,),  # noqa: E501
+            'attributes': (ExternalAuctionLineItemUpdateModel,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -107,15 +107,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ResourceOfAuctionLineItem - a model defined in OpenAPI
+        """ResourceOfAuctionLineItemUpdateModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,15 +142,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalAuctionLineItem): [optional]  # noqa: E501
+            attributes (ExternalAuctionLineItemUpdateModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ResourceOfAuctionLineItem - a model defined in OpenAPI
+        """ResourceOfAuctionLineItemUpdateModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -230,15 +230,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalAuctionLineItem): [optional]  # noqa: E501
+            attributes (ExternalAuctionLineItemUpdateModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item_update_model.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_promoted_product202110.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_auction_line_item_update_model import ExternalAuctionLineItemUpdateModel
-    globals()['ExternalAuctionLineItemUpdateModel'] = ExternalAuctionLineItemUpdateModel
+    from criteo_api_retailmedia_v2023_07.model.external_promoted_product202110 import ExternalPromotedProduct202110
+    globals()['ExternalPromotedProduct202110'] = ExternalPromotedProduct202110
 
 
-class ResourceOfAuctionLineItemUpdateModel(ModelNormal):
+class ResourceOfPromotedProduct202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
-            'attributes': (ExternalAuctionLineItemUpdateModel,),  # noqa: E501
+            'attributes': (ExternalPromotedProduct202110,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -107,15 +107,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ResourceOfAuctionLineItemUpdateModel - a model defined in OpenAPI
+        """ResourceOfPromotedProduct202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,15 +142,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalAuctionLineItemUpdateModel): [optional]  # noqa: E501
+            attributes (ExternalPromotedProduct202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ResourceOfAuctionLineItemUpdateModel - a model defined in OpenAPI
+        """ResourceOfPromotedProduct202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -230,15 +230,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalAuctionLineItemUpdateModel): [optional]  # noqa: E501
+            attributes (ExternalPromotedProduct202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_balance202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_balance202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_balance202110 import ExternalBalance202110
+    from criteo_api_retailmedia_v2023_07.model.external_balance202110 import ExternalBalance202110
     globals()['ExternalBalance202110'] = ExternalBalance202110
 
 
 class ResourceOfBalance202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_balance_campaign202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_balance_campaign202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ResourceOfBalanceCampaign202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_category202204.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_category202204.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.category202204 import Category202204
+    from criteo_api_retailmedia_v2023_07.model.category202204 import Category202204
     globals()['Category202204'] = Category202204
 
 
 class ResourceOfCategory202204(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_common_line_item.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_common_line_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_common_line_item import ExternalCommonLineItem
+    from criteo_api_retailmedia_v2023_07.model.external_common_line_item import ExternalCommonLineItem
     globals()['ExternalCommonLineItem'] = ExternalCommonLineItem
 
 
 class ResourceOfCommonLineItem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_creative202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_creative202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.creative202110 import Creative202110
+    from criteo_api_retailmedia_v2023_07.model.creative202110 import Creative202110
     globals()['Creative202110'] = Creative202110
 
 
 class ResourceOfCreative202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_creative202210.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_creative202210.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.creative202210 import Creative202210
+    from criteo_api_retailmedia_v2023_07.model.creative202210 import Creative202210
     globals()['Creative202210'] = Creative202210
 
 
 class ResourceOfCreative202210(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_line_item_bid_multipliers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.line_item_bid_multipliers import LineItemBidMultipliers
+    from criteo_api_retailmedia_v2023_07.model.line_item_bid_multipliers import LineItemBidMultipliers
     globals()['LineItemBidMultipliers'] = LineItemBidMultipliers
 
 
 class ResourceOfLineItemBidMultipliers(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_preferred_line_item202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_preferred_line_item202110 import ExternalPreferredLineItem202110
+    from criteo_api_retailmedia_v2023_07.model.external_preferred_line_item202110 import ExternalPreferredLineItem202110
     globals()['ExternalPreferredLineItem202110'] = ExternalPreferredLineItem202110
 
 
 class ResourceOfPreferredLineItem202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_preferred_line_item_update_model202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_preferred_line_item_update_model202110 import ExternalPreferredLineItemUpdateModel202110
+    from criteo_api_retailmedia_v2023_07.model.external_preferred_line_item_update_model202110 import ExternalPreferredLineItemUpdateModel202110
     globals()['ExternalPreferredLineItemUpdateModel202110'] = ExternalPreferredLineItemUpdateModel202110
 
 
 class ResourceOfPreferredLineItemUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_promoted_product202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_set_bids_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_promoted_product202110 import ExternalPromotedProduct202110
-    globals()['ExternalPromotedProduct202110'] = ExternalPromotedProduct202110
+    from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_set_bid_model import RetailMediaExternalv1SetBidModel
+    globals()['RetailMediaExternalv1SetBidModel'] = RetailMediaExternalv1SetBidModel
 
 
-class ResourceOfPromotedProduct202110(ModelNormal):
+class RetailMediaExternalv1SetBidsModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -58,14 +58,16 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('keywords',): {
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -83,39 +85,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str,),  # noqa: E501
-            'type': (str,),  # noqa: E501
-            'attributes': (ExternalPromotedProduct202110,),  # noqa: E501
+            'keywords': ([RetailMediaExternalv1SetBidModel],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
+        'keywords': 'keywords',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ResourceOfPromotedProduct202110 - a model defined in OpenAPI
+        """RetailMediaExternalv1SetBidsModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +138,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): Id of the entity. [optional]  # noqa: E501
-            type (str): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalPromotedProduct202110): [optional]  # noqa: E501
+            keywords ([RetailMediaExternalv1SetBidModel]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +191,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ResourceOfPromotedProduct202110 - a model defined in OpenAPI
+        """RetailMediaExternalv1SetBidsModel - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,17 +224,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): Id of the entity. [optional]  # noqa: E501
-            type (str): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (ExternalPromotedProduct202110): [optional]  # noqa: E501
+            keywords ([RetailMediaExternalv1SetBidModel]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/resource_of_template.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/resource_of_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.template import Template
+    from criteo_api_retailmedia_v2023_07.model.template import Template
     globals()['Template'] = Template
 
 
 class ResourceOfTemplate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_audience.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_audience.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.retail_media_audience_attributes import RetailMediaAudienceAttributes
+    from criteo_api_retailmedia_v2023_07.model.retail_media_audience_attributes import RetailMediaAudienceAttributes
     globals()['RetailMediaAudienceAttributes'] = RetailMediaAudienceAttributes
 
 
 class RetailMediaAudience(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_audience_attributes.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_audience_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.customer_list_details import CustomerListDetails
-    from criteo_api_retailmedia_v2023_04.model.user_behavior_details import UserBehaviorDetails
+    from criteo_api_retailmedia_v2023_07.model.customer_list_details import CustomerListDetails
+    from criteo_api_retailmedia_v2023_07.model.user_behavior_details import UserBehaviorDetails
     globals()['CustomerListDetails'] = CustomerListDetails
     globals()['UserBehaviorDetails'] = UserBehaviorDetails
 
 
 class RetailMediaAudienceAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_audience_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2_attributes import RetailMediaAudienceV2Attributes
+    from criteo_api_retailmedia_v2023_07.model.retail_media_audience_v2_attributes import RetailMediaAudienceV2Attributes
     globals()['RetailMediaAudienceV2Attributes'] = RetailMediaAudienceV2Attributes
 
 
 class RetailMediaAudienceV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_attributes.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_audience_v2_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.customer_list_details import CustomerListDetails
-    from criteo_api_retailmedia_v2023_04.model.user_behavior_details_v2 import UserBehaviorDetailsV2
+    from criteo_api_retailmedia_v2023_07.model.customer_list_details import CustomerListDetails
+    from criteo_api_retailmedia_v2023_07.model.user_behavior_details_v2 import UserBehaviorDetailsV2
     globals()['CustomerListDetails'] = CustomerListDetails
     globals()['UserBehaviorDetailsV2'] = UserBehaviorDetailsV2
 
 
 class RetailMediaAudienceV2Attributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_list_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_audience_v2_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.common_problem import CommonProblem
-    from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
-    from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2 import RetailMediaAudienceV2
+    from criteo_api_retailmedia_v2023_07.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_v2 import CreateRetailMediaAudienceV2
     globals()['CommonProblem'] = CommonProblem
-    globals()['PageMetadata'] = PageMetadata
-    globals()['RetailMediaAudienceV2'] = RetailMediaAudienceV2
+    globals()['CreateRetailMediaAudienceV2'] = CreateRetailMediaAudienceV2
 
 
-class RetailMediaAudienceV2ListResponse(ModelNormal):
+class RetailMediaAudienceV2Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -87,48 +85,41 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([RetailMediaAudienceV2],),  # noqa: E501
-            'metadata': (PageMetadata,),  # noqa: E501
+            'data': (CreateRetailMediaAudienceV2,),  # noqa: E501
             'errors': ([CommonProblem],),  # noqa: E501
             'warnings': ([CommonProblem],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'data': 'data',  # noqa: E501
-        'metadata': 'metadata',  # noqa: E501
         'errors': 'errors',  # noqa: E501
         'warnings': 'warnings',  # noqa: E501
     }
 
     read_only_vars = {
-        'data',  # noqa: E501
         'errors',  # noqa: E501
         'warnings',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, data, metadata, *args, **kwargs):  # noqa: E501
-        """RetailMediaAudienceV2ListResponse - a model defined in OpenAPI
-
-        Args:
-            data ([RetailMediaAudienceV2]): data
-            metadata (PageMetadata):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """RetailMediaAudienceV2Response - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -153,14 +144,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            data (CreateRetailMediaAudienceV2): [optional]  # noqa: E501
             errors ([CommonProblem]): errors. [optional]  # noqa: E501
             warnings ([CommonProblem]): warnings. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -186,16 +178,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.data = data
-        self.metadata = metadata
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -208,18 +198,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, metadata, *args, **kwargs):  # noqa: E501
-        """RetailMediaAudienceV2ListResponse - a model defined in OpenAPI
-
-            metadata (PageMetadata):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """RetailMediaAudienceV2Response - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,14 +232,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            data (CreateRetailMediaAudienceV2): [optional]  # noqa: E501
             errors ([CommonProblem]): errors. [optional]  # noqa: E501
             warnings ([CommonProblem]): warnings. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -275,15 +264,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.metadata = metadata
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/async_report_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.common_problem import CommonProblem
-    from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2 import CreateRetailMediaAudienceV2
+    from criteo_api_retailmedia_v2023_07.model.common_problem import CommonProblem
+    from criteo_api_retailmedia_v2023_07.model.status_response_resource import StatusResponseResource
     globals()['CommonProblem'] = CommonProblem
-    globals()['CreateRetailMediaAudienceV2'] = CreateRetailMediaAudienceV2
+    globals()['StatusResponseResource'] = StatusResponseResource
 
 
-class RetailMediaAudienceV2Response(ModelNormal):
+class AsyncReportResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,41 +85,41 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (CreateRetailMediaAudienceV2,),  # noqa: E501
-            'errors': ([CommonProblem],),  # noqa: E501
+            'data': (StatusResponseResource,),  # noqa: E501
             'warnings': ([CommonProblem],),  # noqa: E501
+            'errors': ([CommonProblem],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'data': 'data',  # noqa: E501
-        'errors': 'errors',  # noqa: E501
         'warnings': 'warnings',  # noqa: E501
+        'errors': 'errors',  # noqa: E501
     }
 
     read_only_vars = {
-        'errors',  # noqa: E501
         'warnings',  # noqa: E501
+        'errors',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RetailMediaAudienceV2Response - a model defined in OpenAPI
+        """AsyncReportResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -144,17 +144,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (CreateRetailMediaAudienceV2): [optional]  # noqa: E501
-            errors ([CommonProblem]): errors. [optional]  # noqa: E501
-            warnings ([CommonProblem]): warnings. [optional]  # noqa: E501
+            data (StatusResponseResource): [optional]  # noqa: E501
+            warnings ([CommonProblem]): [optional]  # noqa: E501
+            errors ([CommonProblem]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -199,15 +199,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RetailMediaAudienceV2Response - a model defined in OpenAPI
+        """AsyncReportResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -232,17 +232,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (CreateRetailMediaAudienceV2): [optional]  # noqa: E501
-            errors ([CommonProblem]): errors. [optional]  # noqa: E501
-            warnings ([CommonProblem]): warnings. [optional]  # noqa: E501
+            data (StatusResponseResource): [optional]  # noqa: E501
+            warnings ([CommonProblem]): [optional]  # noqa: E501
+            errors ([CommonProblem]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keyword_model.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_add_remove_keyword_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class RetailMediaExternalv1AddRemoveKeywordModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_add_remove_keywords_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_add_remove_keyword_model import RetailMediaExternalv1AddRemoveKeywordModel
+    from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_add_remove_keyword_model import RetailMediaExternalv1AddRemoveKeywordModel
     globals()['RetailMediaExternalv1AddRemoveKeywordModel'] = RetailMediaExternalv1AddRemoveKeywordModel
 
 
 class RetailMediaExternalv1AddRemoveKeywordsModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_add_remove_keywords_model_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_add_remove_keywords_model_resource import RetailMediaExternalv1AddRemoveKeywordsModelResource
+    from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_add_remove_keywords_model_resource import RetailMediaExternalv1AddRemoveKeywordsModelResource
     globals()['RetailMediaExternalv1AddRemoveKeywordsModelResource'] = RetailMediaExternalv1AddRemoveKeywordsModelResource
 
 
 class RetailMediaExternalv1AddRemoveKeywordsModelRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_resource.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_add_remove_keywords_model_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_add_remove_keywords_model import RetailMediaExternalv1AddRemoveKeywordsModel
+    from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_add_remove_keywords_model import RetailMediaExternalv1AddRemoveKeywordsModel
     globals()['RetailMediaExternalv1AddRemoveKeywordsModel'] = RetailMediaExternalv1AddRemoveKeywordsModel
 
 
 class RetailMediaExternalv1AddRemoveKeywordsModelResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_input_keywords_model.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_input_keywords_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class RetailMediaExternalv1InputKeywordsModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keyword_data_model.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_keywords_model_resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_input_keywords_model import RetailMediaExternalv1InputKeywordsModel
-    globals()['RetailMediaExternalv1InputKeywordsModel'] = RetailMediaExternalv1InputKeywordsModel
+    from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_keywords_model import RetailMediaExternalv1KeywordsModel
+    globals()['RetailMediaExternalv1KeywordsModel'] = RetailMediaExternalv1KeywordsModel
 
 
-class RetailMediaExternalv1KeywordDataModel(ModelNormal):
+class RetailMediaExternalv1KeywordsModelResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,27 +55,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('review_state',): {
-            'INREVIEW': "InReview",
-            'RECOMMENDED': "Recommended",
-            'APPROVED': "Approved",
-            'AUTOAPPROVED': "AutoApproved",
-            'REJECTED': "Rejected",
-            'AUTOREJECTED': "AutoRejected",
-        },
-        ('match_type',): {
-            'POSITIVEEXACTMATCH': "PositiveExactMatch",
-            'NEGATIVEEXACTMATCH': "NegativeExactMatch",
-            'NEGATIVEBROADMATCH': "NegativeBroadMatch",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -96,45 +83,42 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'review_state': (str,),  # noqa: E501
-            'match_type': (str,),  # noqa: E501
-            'bid': (float,),  # noqa: E501
-            'input_keywords': (RetailMediaExternalv1InputKeywordsModel,),  # noqa: E501
-            'created_at': (datetime,),  # noqa: E501
-            'updated_at': (datetime,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'attributes': (RetailMediaExternalv1KeywordsModel,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'review_state': 'reviewState',  # noqa: E501
-        'match_type': 'matchType',  # noqa: E501
-        'bid': 'bid',  # noqa: E501
-        'input_keywords': 'inputKeywords',  # noqa: E501
-        'created_at': 'createdAt',  # noqa: E501
-        'updated_at': 'updatedAt',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RetailMediaExternalv1KeywordDataModel - a model defined in OpenAPI
+    def _from_openapi_data(cls, type, *args, **kwargs):  # noqa: E501
+        """RetailMediaExternalv1KeywordsModelResource - a model defined in OpenAPI
+
+        Args:
+            type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -159,20 +143,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            review_state (str): [optional]  # noqa: E501
-            match_type (str): [optional]  # noqa: E501
-            bid (float): [optional]  # noqa: E501
-            input_keywords (RetailMediaExternalv1InputKeywordsModel): [optional]  # noqa: E501
-            created_at (datetime): [optional]  # noqa: E501
-            updated_at (datetime): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            attributes (RetailMediaExternalv1KeywordsModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -196,14 +176,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -216,16 +197,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """RetailMediaExternalv1KeywordDataModel - a model defined in OpenAPI
+    def __init__(self, type, *args, **kwargs):  # noqa: E501
+        """RetailMediaExternalv1KeywordsModelResource - a model defined in OpenAPI
+
+        Args:
+            type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -250,20 +234,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            review_state (str): [optional]  # noqa: E501
-            match_type (str): [optional]  # noqa: E501
-            bid (float): [optional]  # noqa: E501
-            input_keywords (RetailMediaExternalv1InputKeywordsModel): [optional]  # noqa: E501
-            created_at (datetime): [optional]  # noqa: E501
-            updated_at (datetime): [optional]  # noqa: E501
+            id (str): [optional]  # noqa: E501
+            attributes (RetailMediaExternalv1KeywordsModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -285,14 +265,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_keywords_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_keyword_data_model import RetailMediaExternalv1KeywordDataModel
+    from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_keyword_data_model import RetailMediaExternalv1KeywordDataModel
     globals()['RetailMediaExternalv1KeywordDataModel'] = RetailMediaExternalv1KeywordDataModel
 
 
 class RetailMediaExternalv1KeywordsModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_resource.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_set_bids_model_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_keywords_model import RetailMediaExternalv1KeywordsModel
-    globals()['RetailMediaExternalv1KeywordsModel'] = RetailMediaExternalv1KeywordsModel
+    from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_set_bids_model import RetailMediaExternalv1SetBidsModel
+    globals()['RetailMediaExternalv1SetBidsModel'] = RetailMediaExternalv1SetBidsModel
 
 
-class RetailMediaExternalv1KeywordsModelResource(ModelNormal):
+class RetailMediaExternalv1SetBidsModelResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'type': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'attributes': (RetailMediaExternalv1KeywordsModel,),  # noqa: E501
+            'attributes': (RetailMediaExternalv1SetBidsModel,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -107,15 +107,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, type, *args, **kwargs):  # noqa: E501
-        """RetailMediaExternalv1KeywordsModelResource - a model defined in OpenAPI
+        """RetailMediaExternalv1SetBidsModelResource - a model defined in OpenAPI
 
         Args:
             type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -144,15 +144,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
-            attributes (RetailMediaExternalv1KeywordsModel): [optional]  # noqa: E501
+            attributes (RetailMediaExternalv1SetBidsModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -198,15 +198,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, type, *args, **kwargs):  # noqa: E501
-        """RetailMediaExternalv1KeywordsModelResource - a model defined in OpenAPI
+        """RetailMediaExternalv1SetBidsModelResource - a model defined in OpenAPI
 
         Args:
             type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -235,15 +235,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): [optional]  # noqa: E501
-            attributes (RetailMediaExternalv1KeywordsModel): [optional]  # noqa: E501
+            attributes (RetailMediaExternalv1SetBidsModel): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_keywords_model_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_keywords_model_resource import RetailMediaExternalv1KeywordsModelResource
-    from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_problem_details import RetailMediaExternalv1ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_keywords_model_resource import RetailMediaExternalv1KeywordsModelResource
+    from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_problem_details import RetailMediaExternalv1ProblemDetails
     globals()['RetailMediaExternalv1KeywordsModelResource'] = RetailMediaExternalv1KeywordsModelResource
     globals()['RetailMediaExternalv1ProblemDetails'] = RetailMediaExternalv1ProblemDetails
 
 
 class RetailMediaExternalv1KeywordsModelResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_problem_details.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class RetailMediaExternalv1ProblemDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_proposal_status_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class RetailMediaExternalv1ProposalStatusModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_resource.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_proposal_status_model_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_proposal_status_model import RetailMediaExternalv1ProposalStatusModel
+    from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_proposal_status_model import RetailMediaExternalv1ProposalStatusModel
     globals()['RetailMediaExternalv1ProposalStatusModel'] = RetailMediaExternalv1ProposalStatusModel
 
 
 class RetailMediaExternalv1ProposalStatusModelResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_proposal_status_model_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_problem_details import RetailMediaExternalv1ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_proposal_status_model_resource import RetailMediaExternalv1ProposalStatusModelResource
+    from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_problem_details import RetailMediaExternalv1ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_proposal_status_model_resource import RetailMediaExternalv1ProposalStatusModelResource
     globals()['RetailMediaExternalv1ProblemDetails'] = RetailMediaExternalv1ProblemDetails
     globals()['RetailMediaExternalv1ProposalStatusModelResource'] = RetailMediaExternalv1ProposalStatusModelResource
 
 
 class RetailMediaExternalv1ProposalStatusModelResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_resource_outcome.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_resource_outcome.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_problem_details import RetailMediaExternalv1ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_problem_details import RetailMediaExternalv1ProblemDetails
     globals()['RetailMediaExternalv1ProblemDetails'] = RetailMediaExternalv1ProblemDetails
 
 
 class RetailMediaExternalv1ResourceOutcome(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bid_model.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/campaign_report_resource.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from criteo_api_retailmedia_v2023_07.model.campaign_report import CampaignReport
+    globals()['CampaignReport'] = CampaignReport
 
-class RetailMediaExternalv1SetBidModel(ModelNormal):
+
+class CampaignReportResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -54,64 +58,62 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('phrase',): {
-            'max_length': 255,
-            'min_length': 0,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'phrase': (str,),  # noqa: E501
-            'bid': (float,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'attributes': (CampaignReport,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'phrase': 'phrase',  # noqa: E501
-        'bid': 'bid',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RetailMediaExternalv1SetBidModel - a model defined in OpenAPI
+        """CampaignReportResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,16 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            phrase (str): [optional]  # noqa: E501
-            bid (float): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            attributes (CampaignReport): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -190,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RetailMediaExternalv1SetBidModel - a model defined in OpenAPI
+        """CampaignReportResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -223,16 +225,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            phrase (str): [optional]  # noqa: E501
-            bid (float): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            attributes (CampaignReport): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/retail_media_externalv1_set_bids_model_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_set_bid_model import RetailMediaExternalv1SetBidModel
-    globals()['RetailMediaExternalv1SetBidModel'] = RetailMediaExternalv1SetBidModel
+    from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_set_bids_model_resource import RetailMediaExternalv1SetBidsModelResource
+    globals()['RetailMediaExternalv1SetBidsModelResource'] = RetailMediaExternalv1SetBidsModelResource
 
 
-class RetailMediaExternalv1SetBidsModel(ModelNormal):
+class RetailMediaExternalv1SetBidsModelRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -58,16 +58,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('keywords',): {
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -85,35 +83,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'keywords': ([RetailMediaExternalv1SetBidModel],),  # noqa: E501
+            'data': (RetailMediaExternalv1SetBidsModelResource,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'keywords': 'keywords',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RetailMediaExternalv1SetBidsModel - a model defined in OpenAPI
+        """RetailMediaExternalv1SetBidsModelRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,15 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            keywords ([RetailMediaExternalv1SetBidModel]): [optional]  # noqa: E501
+            data (RetailMediaExternalv1SetBidsModelResource): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,15 +189,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RetailMediaExternalv1SetBidsModel - a model defined in OpenAPI
+        """RetailMediaExternalv1SetBidsModelRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,15 +222,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            keywords ([RetailMediaExternalv1SetBidModel]): [optional]  # noqa: E501
+            data (RetailMediaExternalv1SetBidsModelResource): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/value_type_resource_of_store_target202110.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_set_bids_model_resource import RetailMediaExternalv1SetBidsModelResource
-    globals()['RetailMediaExternalv1SetBidsModelResource'] = RetailMediaExternalv1SetBidsModelResource
+    from criteo_api_retailmedia_v2023_07.model.external_store_target202110 import ExternalStoreTarget202110
+    globals()['ExternalStoreTarget202110'] = ExternalStoreTarget202110
 
 
-class RetailMediaExternalv1SetBidsModelRequest(ModelNormal):
+class ValueTypeResourceOfStoreTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,35 +83,37 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': (RetailMediaExternalv1SetBidsModelResource,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'attributes': (ExternalStoreTarget202110,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """RetailMediaExternalv1SetBidsModelRequest - a model defined in OpenAPI
+        """ValueTypeResourceOfStoreTarget202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (RetailMediaExternalv1SetBidsModelResource): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            attributes (ExternalStoreTarget202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -189,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """RetailMediaExternalv1SetBidsModelRequest - a model defined in OpenAPI
+        """ValueTypeResourceOfStoreTarget202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,15 +225,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (RetailMediaExternalv1SetBidsModelResource): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            attributes (ExternalStoreTarget202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_resource.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/value_type_resource_of_audience_target202110.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_set_bids_model import RetailMediaExternalv1SetBidsModel
-    globals()['RetailMediaExternalv1SetBidsModel'] = RetailMediaExternalv1SetBidsModel
+    from criteo_api_retailmedia_v2023_07.model.external_audience_target202110 import ExternalAudienceTarget202110
+    globals()['ExternalAudienceTarget202110'] = ExternalAudienceTarget202110
 
 
-class RetailMediaExternalv1SetBidsModelResource(ModelNormal):
+class ValueTypeResourceOfAudienceTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,41 +84,36 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'type': (str,),  # noqa: E501
-            'id': (str,),  # noqa: E501
-            'attributes': (RetailMediaExternalv1SetBidsModel,),  # noqa: E501
+            'attributes': (ExternalAudienceTarget202110,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'type': 'type',  # noqa: E501
-        'id': 'id',  # noqa: E501
         'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, type, *args, **kwargs):  # noqa: E501
-        """RetailMediaExternalv1SetBidsModelResource - a model defined in OpenAPI
-
-        Args:
-            type (str):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """ValueTypeResourceOfAudienceTarget202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,16 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            attributes (RetailMediaExternalv1SetBidsModel): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            attributes (ExternalAudienceTarget202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -176,15 +171,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -197,19 +191,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, type, *args, **kwargs):  # noqa: E501
-        """RetailMediaExternalv1SetBidsModelResource - a model defined in OpenAPI
-
-        Args:
-            type (str):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """ValueTypeResourceOfAudienceTarget202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -234,16 +225,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            attributes (RetailMediaExternalv1SetBidsModel): [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            attributes (ExternalAudienceTarget202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -265,15 +256,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/section.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/section.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.template_variable import TemplateVariable
+    from criteo_api_retailmedia_v2023_07.model.template_variable import TemplateVariable
     globals()['TemplateVariable'] = TemplateVariable
 
 
 class Section(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/store_ids_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/store_ids_update_model202110_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_store_ids_update_model202110 import ValueTypeResourceOfStoreIdsUpdateModel202110
+    from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_store_ids_update_model202110 import ValueTypeResourceOfStoreIdsUpdateModel202110
     globals()['ValueTypeResourceOfStoreIdsUpdateModel202110'] = ValueTypeResourceOfStoreIdsUpdateModel202110
 
 
 class StoreIdsUpdateModel202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/store_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/store_target202110_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
+    from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
     globals()['ValueTypeResourceOfStoreTarget202110'] = ValueTypeResourceOfStoreTarget202110
 
 
 class StoreTarget202110Request(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/store_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/store_target202110_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ValueTypeResourceOfStoreTarget202110'] = ValueTypeResourceOfStoreTarget202110
 
 
 class StoreTarget202110Response(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/template.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.section import Section
+    from criteo_api_retailmedia_v2023_07.model.section import Section
     globals()['Section'] = Section
 
 
 class Template(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/template_list_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/template_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_template import ResourceOfTemplate
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_template import ResourceOfTemplate
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfTemplate'] = ResourceOfTemplate
 
 
 class TemplateListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/template_response.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/template_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_retailmedia_v2023_04.model.resource_of_template import ResourceOfTemplate
+    from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_retailmedia_v2023_07.model.resource_of_template import ResourceOfTemplate
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ResourceOfTemplate'] = ResourceOfTemplate
 
 
 class TemplateResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/template_variable.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/template_variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.choice_variable_specification import ChoiceVariableSpecification
-    from criteo_api_retailmedia_v2023_04.model.files_variables_specification import FilesVariablesSpecification
-    from criteo_api_retailmedia_v2023_04.model.text_variable_specification import TextVariableSpecification
+    from criteo_api_retailmedia_v2023_07.model.choice_variable_specification import ChoiceVariableSpecification
+    from criteo_api_retailmedia_v2023_07.model.files_variables_specification import FilesVariablesSpecification
+    from criteo_api_retailmedia_v2023_07.model.text_variable_specification import TextVariableSpecification
     globals()['ChoiceVariableSpecification'] = ChoiceVariableSpecification
     globals()['FilesVariablesSpecification'] = FilesVariablesSpecification
     globals()['TextVariableSpecification'] = TextVariableSpecification
 
 
 class TemplateVariable(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/template_variable_value.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/template_variable_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.choice_variable_value import ChoiceVariableValue
-    from criteo_api_retailmedia_v2023_04.model.color_variable_value import ColorVariableValue
-    from criteo_api_retailmedia_v2023_04.model.files_variable_value import FilesVariableValue
-    from criteo_api_retailmedia_v2023_04.model.hyperlink_variable_value import HyperlinkVariableValue
-    from criteo_api_retailmedia_v2023_04.model.text_variable_value import TextVariableValue
+    from criteo_api_retailmedia_v2023_07.model.choice_variable_value import ChoiceVariableValue
+    from criteo_api_retailmedia_v2023_07.model.color_variable_value import ColorVariableValue
+    from criteo_api_retailmedia_v2023_07.model.files_variable_value import FilesVariableValue
+    from criteo_api_retailmedia_v2023_07.model.hyperlink_variable_value import HyperlinkVariableValue
+    from criteo_api_retailmedia_v2023_07.model.text_variable_value import TextVariableValue
     globals()['ChoiceVariableValue'] = ChoiceVariableValue
     globals()['ColorVariableValue'] = ColorVariableValue
     globals()['FilesVariableValue'] = FilesVariableValue
     globals()['HyperlinkVariableValue'] = HyperlinkVariableValue
     globals()['TextVariableValue'] = TextVariableValue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/text_variable_specification.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/report_data_response_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
-class TextVariableSpecification(ModelNormal):
+class ReportDataResponseResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,35 +77,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'max_chars': (int, none_type,),  # noqa: E501
+            'type': (str,),  # noqa: E501
+            'attributes': ([[{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'max_chars': 'maxChars',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TextVariableSpecification - a model defined in OpenAPI
+        """ReportDataResponseResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,15 +132,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            max_chars (int, none_type): The maximum amount of characters accepted for the text. [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            attributes ([[{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TextVariableSpecification - a model defined in OpenAPI
+        """ReportDataResponseResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +219,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            max_chars (int, none_type): The maximum amount of characters accepted for the text. [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
+            attributes ([[{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/text_variable_value.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/export_report_meta_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from criteo_api_retailmedia_v2023_07.model.export_report_column import ExportReportColumn
+    globals()['ExportReportColumn'] = ExportReportColumn
 
-class TextVariableValue(ModelNormal):
+
+class ExportReportMetaData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,53 +66,54 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'text': (str,),  # noqa: E501
+            'columns': ([ExportReportColumn],),  # noqa: E501
+            'rows': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'text': 'text',  # noqa: E501
+        'columns': 'columns',  # noqa: E501
+        'rows': 'rows',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, text, *args, **kwargs):  # noqa: E501
-        """TextVariableValue - a model defined in OpenAPI
-
-        Args:
-            text (str): The displayed text
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """ExportReportMetaData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,14 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            columns ([ExportReportColumn]): [optional]  # noqa: E501
+            rows (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -164,15 +171,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.text = text
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -185,19 +191,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, text, *args, **kwargs):  # noqa: E501
-        """TextVariableValue - a model defined in OpenAPI
-
-        Args:
-            text (str): The displayed text
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """ExportReportMetaData - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,14 +225,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            columns ([ExportReportColumn]): [optional]  # noqa: E501
+            rows (int): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -251,15 +256,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.text = text
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/user_behavior_details.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/user_behavior_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 
 class UserBehaviorDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/user_behavior_details_v2.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/user_behavior_details_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.create_user_behavior_segment_v2 import CreateUserBehaviorSegmentV2
+    from criteo_api_retailmedia_v2023_07.model.create_user_behavior_segment_v2 import CreateUserBehaviorSegmentV2
     globals()['CreateUserBehaviorSegmentV2'] = CreateUserBehaviorSegmentV2
 
 
 class UserBehaviorDetailsV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/value_type_resource_of_add_to_basket_ids_update_model202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_add_to_basket_ids_update_model202110 import ExternalAddToBasketIdsUpdateModel202110
+    from criteo_api_retailmedia_v2023_07.model.external_add_to_basket_ids_update_model202110 import ExternalAddToBasketIdsUpdateModel202110
     globals()['ExternalAddToBasketIdsUpdateModel202110'] = ExternalAddToBasketIdsUpdateModel202110
 
 
 class ValueTypeResourceOfAddToBasketIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_target202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/value_type_resource_of_add_to_basket_target202110.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_add_to_basket_target202110 import ExternalAddToBasketTarget202110
+    from criteo_api_retailmedia_v2023_07.model.external_add_to_basket_target202110 import ExternalAddToBasketTarget202110
     globals()['ExternalAddToBasketTarget202110'] = ExternalAddToBasketTarget202110
 
 
 class ValueTypeResourceOfAddToBasketTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/value_type_resource_of_audience_ids_update_model202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_audience_ids_update_model202110 import ExternalAudienceIdsUpdateModel202110
+    from criteo_api_retailmedia_v2023_07.model.external_audience_ids_update_model202110 import ExternalAudienceIdsUpdateModel202110
     globals()['ExternalAudienceIdsUpdateModel202110'] = ExternalAudienceIdsUpdateModel202110
 
 
 class ValueTypeResourceOfAudienceIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_target202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/value_type_resource_of_keyword_target202110.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_audience_target202110 import ExternalAudienceTarget202110
-    globals()['ExternalAudienceTarget202110'] = ExternalAudienceTarget202110
+    from criteo_api_retailmedia_v2023_07.model.external_keyword_target202110 import ExternalKeywordTarget202110
+    globals()['ExternalKeywordTarget202110'] = ExternalKeywordTarget202110
 
 
-class ValueTypeResourceOfAudienceTarget202110(ModelNormal):
+class ValueTypeResourceOfKeywordTarget202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -84,15 +84,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'type': (str,),  # noqa: E501
-            'attributes': (ExternalAudienceTarget202110,),  # noqa: E501
+            'attributes': (ExternalKeywordTarget202110,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -105,15 +105,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ValueTypeResourceOfAudienceTarget202110 - a model defined in OpenAPI
+        """ValueTypeResourceOfKeywordTarget202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,15 +139,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             type (str): [optional]  # noqa: E501
-            attributes (ExternalAudienceTarget202110): [optional]  # noqa: E501
+            attributes (ExternalKeywordTarget202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -192,15 +192,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ValueTypeResourceOfAudienceTarget202110 - a model defined in OpenAPI
+        """ValueTypeResourceOfKeywordTarget202110 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -226,15 +226,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             type (str): [optional]  # noqa: E501
-            attributes (ExternalAudienceTarget202110): [optional]  # noqa: E501
+            attributes (ExternalKeywordTarget202110): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_keyword_target202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/report_outcome.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_keyword_target202110 import ExternalKeywordTarget202110
-    globals()['ExternalKeywordTarget202110'] = ExternalKeywordTarget202110
+    from criteo_api_retailmedia_v2023_07.model.common_problem import CommonProblem
+    globals()['CommonProblem'] = CommonProblem
 
 
-class ValueTypeResourceOfKeywordTarget202110(ModelNormal):
+class ReportOutcome(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,37 +83,39 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'type': (str,),  # noqa: E501
-            'attributes': (ExternalKeywordTarget202110,),  # noqa: E501
+            'warnings': ([CommonProblem],),  # noqa: E501
+            'errors': ([CommonProblem],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
+        'warnings': 'warnings',  # noqa: E501
+        'errors': 'errors',  # noqa: E501
     }
 
     read_only_vars = {
+        'warnings',  # noqa: E501
+        'errors',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ValueTypeResourceOfKeywordTarget202110 - a model defined in OpenAPI
+        """ReportOutcome - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,16 +140,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): [optional]  # noqa: E501
-            attributes (ExternalKeywordTarget202110): [optional]  # noqa: E501
+            warnings ([CommonProblem]): [optional]  # noqa: E501
+            errors ([CommonProblem]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -192,15 +194,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ValueTypeResourceOfKeywordTarget202110 - a model defined in OpenAPI
+        """ReportOutcome - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -225,16 +227,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): [optional]  # noqa: E501
-            attributes (ExternalKeywordTarget202110): [optional]  # noqa: E501
+            warnings ([CommonProblem]): [optional]  # noqa: E501
+            errors ([CommonProblem]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/value_type_resource_of_store_ids_update_model202110.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_store_ids_update_model202110 import ExternalStoreIdsUpdateModel202110
+    from criteo_api_retailmedia_v2023_07.model.external_store_ids_update_model202110 import ExternalStoreIdsUpdateModel202110
     globals()['ExternalStoreIdsUpdateModel202110'] = ExternalStoreIdsUpdateModel202110
 
 
 class ValueTypeResourceOfStoreIdsUpdateModel202110(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_target202110.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model/campaign_report_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_retailmedia_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_retailmedia_v2023_07.model_utils import (  # noqa: F401
     ApiTypeError,
     ModelComposed,
     ModelNormal,
     ModelSimple,
     cached_property,
     change_keys_js_to_python,
     convert_js_args_to_python_args,
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
-from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_retailmedia_v2023_04.model.external_store_target202110 import ExternalStoreTarget202110
-    globals()['ExternalStoreTarget202110'] = ExternalStoreTarget202110
+    from criteo_api_retailmedia_v2023_07.model.campaign_report_resource import CampaignReportResource
+    globals()['CampaignReportResource'] = CampaignReportResource
 
 
-class ValueTypeResourceOfStoreTarget202110(ModelNormal):
+class CampaignReportRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,37 +83,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'type': (str,),  # noqa: E501
-            'attributes': (ExternalStoreTarget202110,),  # noqa: E501
+            'data': (CampaignReportResource,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ValueTypeResourceOfStoreTarget202110 - a model defined in OpenAPI
+        """CampaignReportRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,16 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): [optional]  # noqa: E501
-            attributes (ExternalStoreTarget202110): [optional]  # noqa: E501
+            data (CampaignReportResource): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -192,15 +189,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ValueTypeResourceOfStoreTarget202110 - a model defined in OpenAPI
+        """CampaignReportRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -225,16 +222,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            type (str): [optional]  # noqa: E501
-            attributes (ExternalStoreTarget202110): [optional]  # noqa: E501
+            data (CampaignReportResource): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/model_utils.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
@@ -16,15 +16,15 @@
 import pprint
 import re
 import tempfile
 import uuid
 
 from dateutil.parser import parse
 
-from criteo_api_retailmedia_v2023_04.exceptions import (
+from criteo_api_retailmedia_v2023_07.exceptions import (
     ApiKeyError,
     ApiAttributeError,
     ApiTypeError,
     ApiValueError,
 )
 
 none_type = type(None)
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/models/__init__.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/models/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,193 +1,198 @@
 # flake8: noqa
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
-# from criteo_api_retailmedia_v2023_04.model.pet import Pet
+# from criteo_api_retailmedia_v2023_07.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
-from criteo_api_retailmedia_v2023_04.model.add_to_basket_ids_update_model202110_request import AddToBasketIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2023_04.model.add_to_basket_target202110_request import AddToBasketTarget202110Request
-from criteo_api_retailmedia_v2023_04.model.add_to_basket_target202110_response import AddToBasketTarget202110Response
-from criteo_api_retailmedia_v2023_04.model.application_summary_model import ApplicationSummaryModel
-from criteo_api_retailmedia_v2023_04.model.application_summary_model_resource import ApplicationSummaryModelResource
-from criteo_api_retailmedia_v2023_04.model.application_summary_model_response import ApplicationSummaryModelResponse
-from criteo_api_retailmedia_v2023_04.model.asset import Asset
-from criteo_api_retailmedia_v2023_04.model.asset_resource import AssetResource
-from criteo_api_retailmedia_v2023_04.model.asset_response import AssetResponse
-from criteo_api_retailmedia_v2023_04.model.auction_line_item_create_model_request import AuctionLineItemCreateModelRequest
-from criteo_api_retailmedia_v2023_04.model.auction_line_item_paged_list_response import AuctionLineItemPagedListResponse
-from criteo_api_retailmedia_v2023_04.model.auction_line_item_response import AuctionLineItemResponse
-from criteo_api_retailmedia_v2023_04.model.auction_line_item_update_model_request import AuctionLineItemUpdateModelRequest
-from criteo_api_retailmedia_v2023_04.model.audience_ids_update_model202110_request import AudienceIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2023_04.model.audience_target202110_request import AudienceTarget202110Request
-from criteo_api_retailmedia_v2023_04.model.audience_target202110_response import AudienceTarget202110Response
-from criteo_api_retailmedia_v2023_04.model.bad_request import BadRequest
-from criteo_api_retailmedia_v2023_04.model.balance202110_paged_list_response import Balance202110PagedListResponse
-from criteo_api_retailmedia_v2023_04.model.balance_campaign202110_list_request import BalanceCampaign202110ListRequest
-from criteo_api_retailmedia_v2023_04.model.balance_campaign202110_paged_list_response import BalanceCampaign202110PagedListResponse
-from criteo_api_retailmedia_v2023_04.model.campaign_attributes_v202301 import CampaignAttributesV202301
-from criteo_api_retailmedia_v2023_04.model.campaign_v202301 import CampaignV202301
-from criteo_api_retailmedia_v2023_04.model.category202204 import Category202204
-from criteo_api_retailmedia_v2023_04.model.category202204_list_response import Category202204ListResponse
-from criteo_api_retailmedia_v2023_04.model.choice_option import ChoiceOption
-from criteo_api_retailmedia_v2023_04.model.choice_variable_specification import ChoiceVariableSpecification
-from criteo_api_retailmedia_v2023_04.model.choice_variable_value import ChoiceVariableValue
-from criteo_api_retailmedia_v2023_04.model.color_variable_value import ColorVariableValue
-from criteo_api_retailmedia_v2023_04.model.common_error import CommonError
-from criteo_api_retailmedia_v2023_04.model.common_line_item_paged_list_response import CommonLineItemPagedListResponse
-from criteo_api_retailmedia_v2023_04.model.common_line_item_response import CommonLineItemResponse
-from criteo_api_retailmedia_v2023_04.model.common_problem import CommonProblem
-from criteo_api_retailmedia_v2023_04.model.common_status_code_response import CommonStatusCodeResponse
-from criteo_api_retailmedia_v2023_04.model.common_warning import CommonWarning
-from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience import CreateRetailMediaAudience
-from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_attributes import CreateRetailMediaAudienceAttributes
-from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_body import CreateRetailMediaAudienceBody
-from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_request import CreateRetailMediaAudienceRequest
-from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_response import CreateRetailMediaAudienceResponse
-from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2 import CreateRetailMediaAudienceV2
-from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2_attributes import CreateRetailMediaAudienceV2Attributes
-from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2_data import CreateRetailMediaAudienceV2Data
-from criteo_api_retailmedia_v2023_04.model.create_retail_media_audience_v2_request import CreateRetailMediaAudienceV2Request
-from criteo_api_retailmedia_v2023_04.model.create_user_behavior_segment_v2 import CreateUserBehaviorSegmentV2
-from criteo_api_retailmedia_v2023_04.model.creative202110 import Creative202110
-from criteo_api_retailmedia_v2023_04.model.creative202110_list_response import Creative202110ListResponse
-from criteo_api_retailmedia_v2023_04.model.creative202210 import Creative202210
-from criteo_api_retailmedia_v2023_04.model.creative202210_list_response import Creative202210ListResponse
-from criteo_api_retailmedia_v2023_04.model.creative202210_response import Creative202210Response
-from criteo_api_retailmedia_v2023_04.model.creative_create_model202207 import CreativeCreateModel202207
-from criteo_api_retailmedia_v2023_04.model.creative_update_model202207 import CreativeUpdateModel202207
-from criteo_api_retailmedia_v2023_04.model.customer_list_details import CustomerListDetails
-from criteo_api_retailmedia_v2023_04.model.editable_campaign_attributes_v202301 import EditableCampaignAttributesV202301
-from criteo_api_retailmedia_v2023_04.model.envelope_report_request import EnvelopeReportRequest
-from criteo_api_retailmedia_v2023_04.model.envelope_report_status import EnvelopeReportStatus
-from criteo_api_retailmedia_v2023_04.model.error import Error
-from criteo_api_retailmedia_v2023_04.model.external_account import ExternalAccount
-from criteo_api_retailmedia_v2023_04.model.external_add_to_basket_ids_update_model202110 import ExternalAddToBasketIdsUpdateModel202110
-from criteo_api_retailmedia_v2023_04.model.external_add_to_basket_target202110 import ExternalAddToBasketTarget202110
-from criteo_api_retailmedia_v2023_04.model.external_auction_line_item import ExternalAuctionLineItem
-from criteo_api_retailmedia_v2023_04.model.external_auction_line_item_create_model import ExternalAuctionLineItemCreateModel
-from criteo_api_retailmedia_v2023_04.model.external_auction_line_item_update_model import ExternalAuctionLineItemUpdateModel
-from criteo_api_retailmedia_v2023_04.model.external_audience_ids_update_model202110 import ExternalAudienceIdsUpdateModel202110
-from criteo_api_retailmedia_v2023_04.model.external_audience_target202110 import ExternalAudienceTarget202110
-from criteo_api_retailmedia_v2023_04.model.external_balance202110 import ExternalBalance202110
-from criteo_api_retailmedia_v2023_04.model.external_brand import ExternalBrand
-from criteo_api_retailmedia_v2023_04.model.external_catalog_request import ExternalCatalogRequest
-from criteo_api_retailmedia_v2023_04.model.external_catalog_status import ExternalCatalogStatus
-from criteo_api_retailmedia_v2023_04.model.external_common_line_item import ExternalCommonLineItem
-from criteo_api_retailmedia_v2023_04.model.external_keyword_target202110 import ExternalKeywordTarget202110
-from criteo_api_retailmedia_v2023_04.model.external_line_item_capping202110 import ExternalLineItemCapping202110
-from criteo_api_retailmedia_v2023_04.model.external_line_item_page202110 import ExternalLineItemPage202110
-from criteo_api_retailmedia_v2023_04.model.external_line_item_page_category202110 import ExternalLineItemPageCategory202110
-from criteo_api_retailmedia_v2023_04.model.external_preferred_line_item202110 import ExternalPreferredLineItem202110
-from criteo_api_retailmedia_v2023_04.model.external_preferred_line_item_create_model202110 import ExternalPreferredLineItemCreateModel202110
-from criteo_api_retailmedia_v2023_04.model.external_preferred_line_item_update_model202110 import ExternalPreferredLineItemUpdateModel202110
-from criteo_api_retailmedia_v2023_04.model.external_promoted_product202110 import ExternalPromotedProduct202110
-from criteo_api_retailmedia_v2023_04.model.external_retailer import ExternalRetailer
-from criteo_api_retailmedia_v2023_04.model.external_retailer_pages202110 import ExternalRetailerPages202110
-from criteo_api_retailmedia_v2023_04.model.external_store_ids_update_model202110 import ExternalStoreIdsUpdateModel202110
-from criteo_api_retailmedia_v2023_04.model.external_store_target202110 import ExternalStoreTarget202110
-from criteo_api_retailmedia_v2023_04.model.files_variable_value import FilesVariableValue
-from criteo_api_retailmedia_v2023_04.model.files_variables_specification import FilesVariablesSpecification
-from criteo_api_retailmedia_v2023_04.model.get_page_of_audiences_by_account_id_response import GetPageOfAudiencesByAccountIdResponse
-from criteo_api_retailmedia_v2023_04.model.hyperlink_variable_value import HyperlinkVariableValue
-from criteo_api_retailmedia_v2023_04.model.input_resource_of_auction_line_item_create_model import InputResourceOfAuctionLineItemCreateModel
-from criteo_api_retailmedia_v2023_04.model.input_resource_of_preferred_line_item_create_model202110 import InputResourceOfPreferredLineItemCreateModel202110
-from criteo_api_retailmedia_v2023_04.model.json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301
-from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_account_and_account import JsonApiBodyWithIdOfInt64AndAccountAndAccount
-from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_brand_and_brand import JsonApiBodyWithIdOfInt64AndBrandAndBrand
-from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
-from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status import JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus
-from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers import JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers
-from criteo_api_retailmedia_v2023_04.model.json_api_body_with_id_of_int64_and_retailer_and_retailer import JsonApiBodyWithIdOfInt64AndRetailerAndRetailer
-from criteo_api_retailmedia_v2023_04.model.json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301
-from criteo_api_retailmedia_v2023_04.model.json_api_body_without_id_of_catalog_request_and_catalog_request import JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest
-from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_account import JsonApiPageResponseOfAccount
-from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_brand import JsonApiPageResponseOfBrand
-from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_campaign_v202301 import JsonApiPageResponseOfCampaignV202301
-from criteo_api_retailmedia_v2023_04.model.json_api_page_response_of_retailer import JsonApiPageResponseOfRetailer
-from criteo_api_retailmedia_v2023_04.model.json_api_request_of_catalog_request import JsonApiRequestOfCatalogRequest
-from criteo_api_retailmedia_v2023_04.model.json_api_single_response_of_campaign_v202301 import JsonApiSingleResponseOfCampaignV202301
-from criteo_api_retailmedia_v2023_04.model.json_api_single_response_of_catalog_status import JsonApiSingleResponseOfCatalogStatus
-from criteo_api_retailmedia_v2023_04.model.json_api_single_response_of_line_item_bid_multipliers import JsonApiSingleResponseOfLineItemBidMultipliers
-from criteo_api_retailmedia_v2023_04.model.keyword_target202110_request import KeywordTarget202110Request
-from criteo_api_retailmedia_v2023_04.model.keyword_target202110_response import KeywordTarget202110Response
-from criteo_api_retailmedia_v2023_04.model.line_item_bid_multipliers import LineItemBidMultipliers
-from criteo_api_retailmedia_v2023_04.model.line_item_bid_multipliers_request import LineItemBidMultipliersRequest
-from criteo_api_retailmedia_v2023_04.model.line_item_bid_multipliers_response import LineItemBidMultipliersResponse
-from criteo_api_retailmedia_v2023_04.model.map_string import MapString
-from criteo_api_retailmedia_v2023_04.model.page_metadata import PageMetadata
-from criteo_api_retailmedia_v2023_04.model.page_type_environment import PageTypeEnvironment
-from criteo_api_retailmedia_v2023_04.model.post_campaign_v202301 import PostCampaignV202301
-from criteo_api_retailmedia_v2023_04.model.preferred_line_item202110_paged_list_response import PreferredLineItem202110PagedListResponse
-from criteo_api_retailmedia_v2023_04.model.preferred_line_item202110_response import PreferredLineItem202110Response
-from criteo_api_retailmedia_v2023_04.model.preferred_line_item_create_model202110_request import PreferredLineItemCreateModel202110Request
-from criteo_api_retailmedia_v2023_04.model.preferred_line_item_update_model202110_request import PreferredLineItemUpdateModel202110Request
-from criteo_api_retailmedia_v2023_04.model.problem_details import ProblemDetails
-from criteo_api_retailmedia_v2023_04.model.promoted_product202110_list_request import PromotedProduct202110ListRequest
-from criteo_api_retailmedia_v2023_04.model.promoted_product202110_paged_list_response import PromotedProduct202110PagedListResponse
-from criteo_api_retailmedia_v2023_04.model.put_campaign_v202301 import PutCampaignV202301
-from criteo_api_retailmedia_v2023_04.model.report_request import ReportRequest
-from criteo_api_retailmedia_v2023_04.model.report_request_attributes import ReportRequestAttributes
-from criteo_api_retailmedia_v2023_04.model.report_status import ReportStatus
-from criteo_api_retailmedia_v2023_04.model.report_status_attributes import ReportStatusAttributes
-from criteo_api_retailmedia_v2023_04.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
-from criteo_api_retailmedia_v2023_04.model.resource_of_auction_line_item_update_model import ResourceOfAuctionLineItemUpdateModel
-from criteo_api_retailmedia_v2023_04.model.resource_of_balance202110 import ResourceOfBalance202110
-from criteo_api_retailmedia_v2023_04.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
-from criteo_api_retailmedia_v2023_04.model.resource_of_category202204 import ResourceOfCategory202204
-from criteo_api_retailmedia_v2023_04.model.resource_of_common_line_item import ResourceOfCommonLineItem
-from criteo_api_retailmedia_v2023_04.model.resource_of_creative202110 import ResourceOfCreative202110
-from criteo_api_retailmedia_v2023_04.model.resource_of_creative202210 import ResourceOfCreative202210
-from criteo_api_retailmedia_v2023_04.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
-from criteo_api_retailmedia_v2023_04.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
-from criteo_api_retailmedia_v2023_04.model.resource_of_preferred_line_item_update_model202110 import ResourceOfPreferredLineItemUpdateModel202110
-from criteo_api_retailmedia_v2023_04.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
-from criteo_api_retailmedia_v2023_04.model.resource_of_template import ResourceOfTemplate
-from criteo_api_retailmedia_v2023_04.model.retail_media_audience import RetailMediaAudience
-from criteo_api_retailmedia_v2023_04.model.retail_media_audience_attributes import RetailMediaAudienceAttributes
-from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2 import RetailMediaAudienceV2
-from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2_attributes import RetailMediaAudienceV2Attributes
-from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2_list_response import RetailMediaAudienceV2ListResponse
-from criteo_api_retailmedia_v2023_04.model.retail_media_audience_v2_response import RetailMediaAudienceV2Response
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_add_remove_keyword_model import RetailMediaExternalv1AddRemoveKeywordModel
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_add_remove_keywords_model import RetailMediaExternalv1AddRemoveKeywordsModel
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_add_remove_keywords_model_request import RetailMediaExternalv1AddRemoveKeywordsModelRequest
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_add_remove_keywords_model_resource import RetailMediaExternalv1AddRemoveKeywordsModelResource
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_input_keywords_model import RetailMediaExternalv1InputKeywordsModel
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_keyword_data_model import RetailMediaExternalv1KeywordDataModel
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_keywords_model import RetailMediaExternalv1KeywordsModel
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_keywords_model_resource import RetailMediaExternalv1KeywordsModelResource
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_keywords_model_response import RetailMediaExternalv1KeywordsModelResponse
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_problem_details import RetailMediaExternalv1ProblemDetails
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_proposal_status_model import RetailMediaExternalv1ProposalStatusModel
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_proposal_status_model_resource import RetailMediaExternalv1ProposalStatusModelResource
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_proposal_status_model_response import RetailMediaExternalv1ProposalStatusModelResponse
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_resource_outcome import RetailMediaExternalv1ResourceOutcome
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_set_bid_model import RetailMediaExternalv1SetBidModel
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_set_bids_model import RetailMediaExternalv1SetBidsModel
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_set_bids_model_request import RetailMediaExternalv1SetBidsModelRequest
-from criteo_api_retailmedia_v2023_04.model.retail_media_externalv1_set_bids_model_resource import RetailMediaExternalv1SetBidsModelResource
-from criteo_api_retailmedia_v2023_04.model.section import Section
-from criteo_api_retailmedia_v2023_04.model.store_ids_update_model202110_request import StoreIdsUpdateModel202110Request
-from criteo_api_retailmedia_v2023_04.model.store_target202110_request import StoreTarget202110Request
-from criteo_api_retailmedia_v2023_04.model.store_target202110_response import StoreTarget202110Response
-from criteo_api_retailmedia_v2023_04.model.template import Template
-from criteo_api_retailmedia_v2023_04.model.template_list_response import TemplateListResponse
-from criteo_api_retailmedia_v2023_04.model.template_response import TemplateResponse
-from criteo_api_retailmedia_v2023_04.model.template_variable import TemplateVariable
-from criteo_api_retailmedia_v2023_04.model.template_variable_value import TemplateVariableValue
-from criteo_api_retailmedia_v2023_04.model.text_variable_specification import TextVariableSpecification
-from criteo_api_retailmedia_v2023_04.model.text_variable_value import TextVariableValue
-from criteo_api_retailmedia_v2023_04.model.user_behavior_details import UserBehaviorDetails
-from criteo_api_retailmedia_v2023_04.model.user_behavior_details_v2 import UserBehaviorDetailsV2
-from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_add_to_basket_ids_update_model202110 import ValueTypeResourceOfAddToBasketIdsUpdateModel202110
-from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
-from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_audience_ids_update_model202110 import ValueTypeResourceOfAudienceIdsUpdateModel202110
-from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
-from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
-from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_store_ids_update_model202110 import ValueTypeResourceOfStoreIdsUpdateModel202110
-from criteo_api_retailmedia_v2023_04.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
+from criteo_api_retailmedia_v2023_07.model.add_to_basket_ids_update_model202110_request import AddToBasketIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2023_07.model.add_to_basket_target202110_request import AddToBasketTarget202110Request
+from criteo_api_retailmedia_v2023_07.model.add_to_basket_target202110_response import AddToBasketTarget202110Response
+from criteo_api_retailmedia_v2023_07.model.application_summary_model import ApplicationSummaryModel
+from criteo_api_retailmedia_v2023_07.model.application_summary_model_resource import ApplicationSummaryModelResource
+from criteo_api_retailmedia_v2023_07.model.application_summary_model_response import ApplicationSummaryModelResponse
+from criteo_api_retailmedia_v2023_07.model.asset import Asset
+from criteo_api_retailmedia_v2023_07.model.asset_resource import AssetResource
+from criteo_api_retailmedia_v2023_07.model.asset_response import AssetResponse
+from criteo_api_retailmedia_v2023_07.model.async_report_response import AsyncReportResponse
+from criteo_api_retailmedia_v2023_07.model.auction_line_item_create_model_request import AuctionLineItemCreateModelRequest
+from criteo_api_retailmedia_v2023_07.model.auction_line_item_paged_list_response import AuctionLineItemPagedListResponse
+from criteo_api_retailmedia_v2023_07.model.auction_line_item_response import AuctionLineItemResponse
+from criteo_api_retailmedia_v2023_07.model.auction_line_item_update_model_request import AuctionLineItemUpdateModelRequest
+from criteo_api_retailmedia_v2023_07.model.audience_ids_update_model202110_request import AudienceIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2023_07.model.audience_target202110_request import AudienceTarget202110Request
+from criteo_api_retailmedia_v2023_07.model.audience_target202110_response import AudienceTarget202110Response
+from criteo_api_retailmedia_v2023_07.model.balance202110_paged_list_response import Balance202110PagedListResponse
+from criteo_api_retailmedia_v2023_07.model.balance_campaign202110_list_request import BalanceCampaign202110ListRequest
+from criteo_api_retailmedia_v2023_07.model.balance_campaign202110_paged_list_response import BalanceCampaign202110PagedListResponse
+from criteo_api_retailmedia_v2023_07.model.campaign_attributes_v202301 import CampaignAttributesV202301
+from criteo_api_retailmedia_v2023_07.model.campaign_report import CampaignReport
+from criteo_api_retailmedia_v2023_07.model.campaign_report_request import CampaignReportRequest
+from criteo_api_retailmedia_v2023_07.model.campaign_report_resource import CampaignReportResource
+from criteo_api_retailmedia_v2023_07.model.campaign_v202301 import CampaignV202301
+from criteo_api_retailmedia_v2023_07.model.category202204 import Category202204
+from criteo_api_retailmedia_v2023_07.model.category202204_list_response import Category202204ListResponse
+from criteo_api_retailmedia_v2023_07.model.choice_option import ChoiceOption
+from criteo_api_retailmedia_v2023_07.model.choice_variable_specification import ChoiceVariableSpecification
+from criteo_api_retailmedia_v2023_07.model.choice_variable_value import ChoiceVariableValue
+from criteo_api_retailmedia_v2023_07.model.color_variable_value import ColorVariableValue
+from criteo_api_retailmedia_v2023_07.model.common_error import CommonError
+from criteo_api_retailmedia_v2023_07.model.common_line_item_paged_list_response import CommonLineItemPagedListResponse
+from criteo_api_retailmedia_v2023_07.model.common_line_item_response import CommonLineItemResponse
+from criteo_api_retailmedia_v2023_07.model.common_problem import CommonProblem
+from criteo_api_retailmedia_v2023_07.model.common_status_code_response import CommonStatusCodeResponse
+from criteo_api_retailmedia_v2023_07.model.common_warning import CommonWarning
+from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience import CreateRetailMediaAudience
+from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_attributes import CreateRetailMediaAudienceAttributes
+from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_body import CreateRetailMediaAudienceBody
+from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_request import CreateRetailMediaAudienceRequest
+from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_response import CreateRetailMediaAudienceResponse
+from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_v2 import CreateRetailMediaAudienceV2
+from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_v2_attributes import CreateRetailMediaAudienceV2Attributes
+from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_v2_data import CreateRetailMediaAudienceV2Data
+from criteo_api_retailmedia_v2023_07.model.create_retail_media_audience_v2_request import CreateRetailMediaAudienceV2Request
+from criteo_api_retailmedia_v2023_07.model.create_user_behavior_segment_v2 import CreateUserBehaviorSegmentV2
+from criteo_api_retailmedia_v2023_07.model.creative202110 import Creative202110
+from criteo_api_retailmedia_v2023_07.model.creative202110_list_response import Creative202110ListResponse
+from criteo_api_retailmedia_v2023_07.model.creative202210 import Creative202210
+from criteo_api_retailmedia_v2023_07.model.creative202210_list_response import Creative202210ListResponse
+from criteo_api_retailmedia_v2023_07.model.creative202210_response import Creative202210Response
+from criteo_api_retailmedia_v2023_07.model.creative_create_model202207 import CreativeCreateModel202207
+from criteo_api_retailmedia_v2023_07.model.creative_update_model202207 import CreativeUpdateModel202207
+from criteo_api_retailmedia_v2023_07.model.customer_list_details import CustomerListDetails
+from criteo_api_retailmedia_v2023_07.model.editable_campaign_attributes_v202301 import EditableCampaignAttributesV202301
+from criteo_api_retailmedia_v2023_07.model.export_report_column import ExportReportColumn
+from criteo_api_retailmedia_v2023_07.model.export_report_meta_data import ExportReportMetaData
+from criteo_api_retailmedia_v2023_07.model.external_account import ExternalAccount
+from criteo_api_retailmedia_v2023_07.model.external_add_to_basket_ids_update_model202110 import ExternalAddToBasketIdsUpdateModel202110
+from criteo_api_retailmedia_v2023_07.model.external_add_to_basket_target202110 import ExternalAddToBasketTarget202110
+from criteo_api_retailmedia_v2023_07.model.external_auction_line_item import ExternalAuctionLineItem
+from criteo_api_retailmedia_v2023_07.model.external_auction_line_item_create_model import ExternalAuctionLineItemCreateModel
+from criteo_api_retailmedia_v2023_07.model.external_auction_line_item_update_model import ExternalAuctionLineItemUpdateModel
+from criteo_api_retailmedia_v2023_07.model.external_audience_ids_update_model202110 import ExternalAudienceIdsUpdateModel202110
+from criteo_api_retailmedia_v2023_07.model.external_audience_target202110 import ExternalAudienceTarget202110
+from criteo_api_retailmedia_v2023_07.model.external_balance202110 import ExternalBalance202110
+from criteo_api_retailmedia_v2023_07.model.external_brand import ExternalBrand
+from criteo_api_retailmedia_v2023_07.model.external_catalog_request import ExternalCatalogRequest
+from criteo_api_retailmedia_v2023_07.model.external_catalog_status import ExternalCatalogStatus
+from criteo_api_retailmedia_v2023_07.model.external_common_line_item import ExternalCommonLineItem
+from criteo_api_retailmedia_v2023_07.model.external_keyword_target202110 import ExternalKeywordTarget202110
+from criteo_api_retailmedia_v2023_07.model.external_line_item_capping202110 import ExternalLineItemCapping202110
+from criteo_api_retailmedia_v2023_07.model.external_line_item_page202110 import ExternalLineItemPage202110
+from criteo_api_retailmedia_v2023_07.model.external_line_item_page_category202110 import ExternalLineItemPageCategory202110
+from criteo_api_retailmedia_v2023_07.model.external_preferred_line_item202110 import ExternalPreferredLineItem202110
+from criteo_api_retailmedia_v2023_07.model.external_preferred_line_item_create_model202110 import ExternalPreferredLineItemCreateModel202110
+from criteo_api_retailmedia_v2023_07.model.external_preferred_line_item_update_model202110 import ExternalPreferredLineItemUpdateModel202110
+from criteo_api_retailmedia_v2023_07.model.external_promoted_product202110 import ExternalPromotedProduct202110
+from criteo_api_retailmedia_v2023_07.model.external_retailer import ExternalRetailer
+from criteo_api_retailmedia_v2023_07.model.external_retailer_pages202110 import ExternalRetailerPages202110
+from criteo_api_retailmedia_v2023_07.model.external_store_ids_update_model202110 import ExternalStoreIdsUpdateModel202110
+from criteo_api_retailmedia_v2023_07.model.external_store_target202110 import ExternalStoreTarget202110
+from criteo_api_retailmedia_v2023_07.model.files_variable_value import FilesVariableValue
+from criteo_api_retailmedia_v2023_07.model.files_variables_specification import FilesVariablesSpecification
+from criteo_api_retailmedia_v2023_07.model.get_page_of_audiences_by_account_id_response import GetPageOfAudiencesByAccountIdResponse
+from criteo_api_retailmedia_v2023_07.model.hyperlink_variable_value import HyperlinkVariableValue
+from criteo_api_retailmedia_v2023_07.model.input_resource_of_auction_line_item_create_model import InputResourceOfAuctionLineItemCreateModel
+from criteo_api_retailmedia_v2023_07.model.input_resource_of_preferred_line_item_create_model202110 import InputResourceOfPreferredLineItemCreateModel202110
+from criteo_api_retailmedia_v2023_07.model.json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithExternalIdOfEditableCampaignAttributesV202301AndCampaignV202301
+from criteo_api_retailmedia_v2023_07.model.json_api_body_with_id_of_int64_and_account_and_account import JsonApiBodyWithIdOfInt64AndAccountAndAccount
+from criteo_api_retailmedia_v2023_07.model.json_api_body_with_id_of_int64_and_brand_and_brand import JsonApiBodyWithIdOfInt64AndBrandAndBrand
+from criteo_api_retailmedia_v2023_07.model.json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301 import JsonApiBodyWithIdOfInt64AndCampaignV202301AndCampaignV202301
+from criteo_api_retailmedia_v2023_07.model.json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status import JsonApiBodyWithIdOfInt64AndCatalogStatusAndCatalogStatus
+from criteo_api_retailmedia_v2023_07.model.json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers import JsonApiBodyWithIdOfInt64AndLineItemBidMultipliersAndLineItemBidMultipliers
+from criteo_api_retailmedia_v2023_07.model.json_api_body_with_id_of_int64_and_retailer_and_retailer import JsonApiBodyWithIdOfInt64AndRetailerAndRetailer
+from criteo_api_retailmedia_v2023_07.model.json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301 import JsonApiBodyWithoutIdOfCampaignAttributesV202301AndCampaignV202301
+from criteo_api_retailmedia_v2023_07.model.json_api_body_without_id_of_catalog_request_and_catalog_request import JsonApiBodyWithoutIdOfCatalogRequestAndCatalogRequest
+from criteo_api_retailmedia_v2023_07.model.json_api_page_response_of_account import JsonApiPageResponseOfAccount
+from criteo_api_retailmedia_v2023_07.model.json_api_page_response_of_brand import JsonApiPageResponseOfBrand
+from criteo_api_retailmedia_v2023_07.model.json_api_page_response_of_campaign_v202301 import JsonApiPageResponseOfCampaignV202301
+from criteo_api_retailmedia_v2023_07.model.json_api_page_response_of_retailer import JsonApiPageResponseOfRetailer
+from criteo_api_retailmedia_v2023_07.model.json_api_request_of_catalog_request import JsonApiRequestOfCatalogRequest
+from criteo_api_retailmedia_v2023_07.model.json_api_single_response_of_campaign_v202301 import JsonApiSingleResponseOfCampaignV202301
+from criteo_api_retailmedia_v2023_07.model.json_api_single_response_of_catalog_status import JsonApiSingleResponseOfCatalogStatus
+from criteo_api_retailmedia_v2023_07.model.json_api_single_response_of_line_item_bid_multipliers import JsonApiSingleResponseOfLineItemBidMultipliers
+from criteo_api_retailmedia_v2023_07.model.keyword_target202110_request import KeywordTarget202110Request
+from criteo_api_retailmedia_v2023_07.model.keyword_target202110_response import KeywordTarget202110Response
+from criteo_api_retailmedia_v2023_07.model.line_item_bid_multipliers import LineItemBidMultipliers
+from criteo_api_retailmedia_v2023_07.model.line_item_bid_multipliers_request import LineItemBidMultipliersRequest
+from criteo_api_retailmedia_v2023_07.model.line_item_bid_multipliers_response import LineItemBidMultipliersResponse
+from criteo_api_retailmedia_v2023_07.model.line_item_report import LineItemReport
+from criteo_api_retailmedia_v2023_07.model.line_item_report_request import LineItemReportRequest
+from criteo_api_retailmedia_v2023_07.model.line_item_report_resource import LineItemReportResource
+from criteo_api_retailmedia_v2023_07.model.page_metadata import PageMetadata
+from criteo_api_retailmedia_v2023_07.model.page_type_environment import PageTypeEnvironment
+from criteo_api_retailmedia_v2023_07.model.post_campaign_v202301 import PostCampaignV202301
+from criteo_api_retailmedia_v2023_07.model.preferred_line_item202110_paged_list_response import PreferredLineItem202110PagedListResponse
+from criteo_api_retailmedia_v2023_07.model.preferred_line_item202110_response import PreferredLineItem202110Response
+from criteo_api_retailmedia_v2023_07.model.preferred_line_item_create_model202110_request import PreferredLineItemCreateModel202110Request
+from criteo_api_retailmedia_v2023_07.model.preferred_line_item_update_model202110_request import PreferredLineItemUpdateModel202110Request
+from criteo_api_retailmedia_v2023_07.model.problem_details import ProblemDetails
+from criteo_api_retailmedia_v2023_07.model.promoted_product202110_list_request import PromotedProduct202110ListRequest
+from criteo_api_retailmedia_v2023_07.model.promoted_product202110_paged_list_response import PromotedProduct202110PagedListResponse
+from criteo_api_retailmedia_v2023_07.model.put_campaign_v202301 import PutCampaignV202301
+from criteo_api_retailmedia_v2023_07.model.report_data_response_resource import ReportDataResponseResource
+from criteo_api_retailmedia_v2023_07.model.report_outcome import ReportOutcome
+from criteo_api_retailmedia_v2023_07.model.report_response import ReportResponse
+from criteo_api_retailmedia_v2023_07.model.resource_of_auction_line_item import ResourceOfAuctionLineItem
+from criteo_api_retailmedia_v2023_07.model.resource_of_auction_line_item_update_model import ResourceOfAuctionLineItemUpdateModel
+from criteo_api_retailmedia_v2023_07.model.resource_of_balance202110 import ResourceOfBalance202110
+from criteo_api_retailmedia_v2023_07.model.resource_of_balance_campaign202110 import ResourceOfBalanceCampaign202110
+from criteo_api_retailmedia_v2023_07.model.resource_of_category202204 import ResourceOfCategory202204
+from criteo_api_retailmedia_v2023_07.model.resource_of_common_line_item import ResourceOfCommonLineItem
+from criteo_api_retailmedia_v2023_07.model.resource_of_creative202110 import ResourceOfCreative202110
+from criteo_api_retailmedia_v2023_07.model.resource_of_creative202210 import ResourceOfCreative202210
+from criteo_api_retailmedia_v2023_07.model.resource_of_line_item_bid_multipliers import ResourceOfLineItemBidMultipliers
+from criteo_api_retailmedia_v2023_07.model.resource_of_preferred_line_item202110 import ResourceOfPreferredLineItem202110
+from criteo_api_retailmedia_v2023_07.model.resource_of_preferred_line_item_update_model202110 import ResourceOfPreferredLineItemUpdateModel202110
+from criteo_api_retailmedia_v2023_07.model.resource_of_promoted_product202110 import ResourceOfPromotedProduct202110
+from criteo_api_retailmedia_v2023_07.model.resource_of_template import ResourceOfTemplate
+from criteo_api_retailmedia_v2023_07.model.retail_media_audience import RetailMediaAudience
+from criteo_api_retailmedia_v2023_07.model.retail_media_audience_attributes import RetailMediaAudienceAttributes
+from criteo_api_retailmedia_v2023_07.model.retail_media_audience_v2 import RetailMediaAudienceV2
+from criteo_api_retailmedia_v2023_07.model.retail_media_audience_v2_attributes import RetailMediaAudienceV2Attributes
+from criteo_api_retailmedia_v2023_07.model.retail_media_audience_v2_list_response import RetailMediaAudienceV2ListResponse
+from criteo_api_retailmedia_v2023_07.model.retail_media_audience_v2_response import RetailMediaAudienceV2Response
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_add_remove_keyword_model import RetailMediaExternalv1AddRemoveKeywordModel
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_add_remove_keywords_model import RetailMediaExternalv1AddRemoveKeywordsModel
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_add_remove_keywords_model_request import RetailMediaExternalv1AddRemoveKeywordsModelRequest
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_add_remove_keywords_model_resource import RetailMediaExternalv1AddRemoveKeywordsModelResource
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_input_keywords_model import RetailMediaExternalv1InputKeywordsModel
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_keyword_data_model import RetailMediaExternalv1KeywordDataModel
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_keywords_model import RetailMediaExternalv1KeywordsModel
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_keywords_model_resource import RetailMediaExternalv1KeywordsModelResource
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_keywords_model_response import RetailMediaExternalv1KeywordsModelResponse
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_problem_details import RetailMediaExternalv1ProblemDetails
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_proposal_status_model import RetailMediaExternalv1ProposalStatusModel
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_proposal_status_model_resource import RetailMediaExternalv1ProposalStatusModelResource
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_proposal_status_model_response import RetailMediaExternalv1ProposalStatusModelResponse
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_resource_outcome import RetailMediaExternalv1ResourceOutcome
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_set_bid_model import RetailMediaExternalv1SetBidModel
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_set_bids_model import RetailMediaExternalv1SetBidsModel
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_set_bids_model_request import RetailMediaExternalv1SetBidsModelRequest
+from criteo_api_retailmedia_v2023_07.model.retail_media_externalv1_set_bids_model_resource import RetailMediaExternalv1SetBidsModelResource
+from criteo_api_retailmedia_v2023_07.model.section import Section
+from criteo_api_retailmedia_v2023_07.model.status_response import StatusResponse
+from criteo_api_retailmedia_v2023_07.model.status_response_resource import StatusResponseResource
+from criteo_api_retailmedia_v2023_07.model.store_ids_update_model202110_request import StoreIdsUpdateModel202110Request
+from criteo_api_retailmedia_v2023_07.model.store_target202110_request import StoreTarget202110Request
+from criteo_api_retailmedia_v2023_07.model.store_target202110_response import StoreTarget202110Response
+from criteo_api_retailmedia_v2023_07.model.template import Template
+from criteo_api_retailmedia_v2023_07.model.template_list_response import TemplateListResponse
+from criteo_api_retailmedia_v2023_07.model.template_response import TemplateResponse
+from criteo_api_retailmedia_v2023_07.model.template_variable import TemplateVariable
+from criteo_api_retailmedia_v2023_07.model.template_variable_value import TemplateVariableValue
+from criteo_api_retailmedia_v2023_07.model.text_variable_specification import TextVariableSpecification
+from criteo_api_retailmedia_v2023_07.model.text_variable_value import TextVariableValue
+from criteo_api_retailmedia_v2023_07.model.user_behavior_details import UserBehaviorDetails
+from criteo_api_retailmedia_v2023_07.model.user_behavior_details_v2 import UserBehaviorDetailsV2
+from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_add_to_basket_ids_update_model202110 import ValueTypeResourceOfAddToBasketIdsUpdateModel202110
+from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_add_to_basket_target202110 import ValueTypeResourceOfAddToBasketTarget202110
+from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_audience_ids_update_model202110 import ValueTypeResourceOfAudienceIdsUpdateModel202110
+from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_audience_target202110 import ValueTypeResourceOfAudienceTarget202110
+from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_keyword_target202110 import ValueTypeResourceOfKeywordTarget202110
+from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_store_ids_update_model202110 import ValueTypeResourceOfStoreIdsUpdateModel202110
+from criteo_api_retailmedia_v2023_07.model.value_type_resource_of_store_target202110 import ValueTypeResourceOfStoreTarget202110
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/criteo_api_retailmedia_v2023_04/rest.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/criteo_api_retailmedia_v2023_07/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - RetailMedia  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
@@ -15,15 +15,15 @@
 import ssl
 from urllib.parse import urlencode
 from urllib.parse import urlparse
 from urllib.request import proxy_bypass_environment
 import urllib3
 import ipaddress
 
-from criteo_api_retailmedia_v2023_04.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
+from criteo_api_retailmedia_v2023_07.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/setup.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "criteo-api-retailmedia-sdk"
-VERSION = "2023.04.0.230726"
+VERSION = "2023.07.0.230726"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -20,21 +20,21 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-retailmedia-sdk==2023.04.0.230726
+pip install criteo-api-retailmedia-sdk==2023.07.0.230726
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230726`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.07.0.230726`)
 
 Then import the package:
 ```python
-import criteo_api_retailmedia_v2023_04
+import criteo_api_retailmedia_v2023_07
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230726/test/test_gateway_api.py` & `criteo-api-retailmedia-sdk-2023.7.0.230726/test/test_gateway_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import os
 
-from criteo_api_retailmedia_v2023_04.api.gateway_api import GatewayApi
-from criteo_api_retailmedia_v2023_04.api_client_builder import ApiClientBuilder
-from criteo_api_retailmedia_v2023_04.rest import ApiException
+from criteo_api_retailmedia_v2023_07.api.gateway_api import GatewayApi
+from criteo_api_retailmedia_v2023_07.api_client_builder import ApiClientBuilder
+from criteo_api_retailmedia_v2023_07.rest import ApiException
 from example_application_with_client_credentials import ExampleApplication
 
 class TestGatewayApi:
   @pytest.fixture(autouse=True)
   def before_each(self):
     self.client_id = os.environ.get("TEST_CLIENT_ID")
     self.client_secret = os.environ.get("TEST_CLIENT_SECRET")
```

