# Comparing `tmp/criteo-api-marketingsolutions-sdk-2023.4.0.230726.tar.gz` & `tmp/criteo-api-marketingsolutions-sdk-2023.7.0.230726.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criteo-api-marketingsolutions-sdk-2023.4.0.230726.tar", last modified: Wed Jul 26 09:55:39 2023, max compression
+gzip compressed data, was "criteo-api-marketingsolutions-sdk-2023.7.0.230726.tar", last modified: Wed Jul 26 09:55:52 2023, max compression
```

## Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726.tar` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726.tar`

### file list

```diff
@@ -1,142 +1,298 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:39.154967 criteo-api-marketingsolutions-sdk-2023.4.0.230726/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-26 09:55:39.154967 criteo-api-marketingsolutions-sdk-2023.4.0.230726/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:39.114967 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-26 09:55:39.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-07-26 09:55:39.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:55:39.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 09:55:39.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-26 09:55:39.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:39.118967 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:39.122967 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/api/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/api/advertiser_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23686 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/api/analytics_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33709 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/api/audience_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    66388 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/api/campaign_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/api/gateway_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39256 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/api_client_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:39.122967 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/criteo_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/criteo_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/criteo_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/flow_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:39.154967 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_delivery_limitations.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_frequency_capping.py
--rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_geo_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/application_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    13856 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/audience_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/audience_name_description.py
--rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/audience_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/basic_audience_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/campaign_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/campaign_read_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/campaign_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/campaign_search_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/campaign_search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/campaign_spend_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/common_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/criteo_api_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13856 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/criteo_api_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/delete_audience_contact_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/delete_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/entity_of_portfolio_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/error_code_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/get_audiences_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/get_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/modify_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/new_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/new_audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/new_audience_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/new_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11515 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/nillable_date_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/nillable_decimal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_budget.py
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12652 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_spend_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12157 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_write_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_read_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_data_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    16412 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/portfolio_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/problem_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/problems_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_budget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/read_model_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12094 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/read_model_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/replace_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/replace_audience_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/replace_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/request_ad_set_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/requests_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/requests_patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/response_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/response_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/responses_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/responses_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    16559 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/statistics_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_data_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transparency_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transparency_report_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transparency_report_data_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transparency_report_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transparency_report_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/write_model_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/write_model_patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    82579 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:39.154967 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/models/
--rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14256 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 09:55:39.154967 criteo-api-marketingsolutions-sdk-2023.4.0.230726/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:39.154967 criteo-api-marketingsolutions-sdk-2023.4.0.230726/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230726/test/test_gateway_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:52.634917 criteo-api-marketingsolutions-sdk-2023.7.0.230726/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-26 09:55:52.634917 criteo-api-marketingsolutions-sdk-2023.7.0.230726/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18889 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:52.598917 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-26 09:55:52.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20961 2023-07-26 09:55:52.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:55:52.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 09:55:52.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-26 09:55:52.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:52.598917 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:52.602917 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api/advertiser_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23686 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api/analytics_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124239 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api/audience_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83723 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api/campaign_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96298 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api/creative_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api/gateway_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39256 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api_client_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:52.602917 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16743 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/criteo_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/criteo_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/criteo_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/flow_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:52.634917 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11925 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_audience_link_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_audience_link_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12502 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_audience_link_entity_v1_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_audience_link_input_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_category_bid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_category_bid_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_category_bid_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_delivery_limitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_display_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_display_multiplier_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_display_multiplier_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_frequency_capping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_geo_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_targeting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_write_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17524 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/adaptive_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/adaptive_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/adaptive_write_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/algebra_node_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/application_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/application_summary_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/application_summary_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13856 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_bulk_create_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_bulk_delete_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_bulk_update_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_compute_size_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_compute_sizes_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_create_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_create_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_delete_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13456 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_entity_v1_audience_search_metadata_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_estimate_size_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_estimate_size_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_estimate_size_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_id_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_id_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_name_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_search_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11960 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_search_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_search_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11997 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_search_metadata_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_bulk_create_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_bulk_delete_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_bulk_update_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12210 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_compute_size_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_compute_sizes_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14771 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_create_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12031 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_create_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12125 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_delete_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_entity_v1_audience_segment_search_metadata_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_estimate_size_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_id_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_id_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_search_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12031 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_search_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_search_input_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12018 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_search_metadata_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_size_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_size_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_size_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_size_estimation_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_size_estimation_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_size_estimation_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_size_estimation_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_size_estimation_v1_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_update_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_segment_update_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_size_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12468 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_size_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_size_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_size_estimation_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_size_estimation_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12490 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_size_estimation_v1_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_update_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_update_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/basic_audience_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12611 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/behavioral_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_read_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_search_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_spend_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_spend_limit_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_v23_q1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_v23_q1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_v23_q1_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/common_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/contact_list_statistics_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/contact_list_statistics_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/contact_list_statistics_entity_v1_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/contact_list_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/contactlist_amendment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/contactlist_amendment_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/contactlist_amendment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/contactlist_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13642 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/contactlist_operation_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/coupon_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/coupon_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/coupon_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/coupon_supported_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/coupon_supported_sizes_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/coupon_supported_sizes_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15475 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12502 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_ad_set_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_ad_set_budget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_ad_set_geo_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_ad_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_ad_set_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11757 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_ad_set_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_ad_set_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_campaign_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_campaign_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_campaign_spend_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16102 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_coupon_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_coupon_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12151 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/create_image_slide.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/creative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12447 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/creative_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11985 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/creative_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/creative_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/creative_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/creative_write_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/creative_write_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/criteo_api_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13856 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/criteo_api_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/delete_audience_contact_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/delete_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14917 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/dynamic_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15146 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/dynamic_write_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/entity_of_portfolio_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/error_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/get_audiences_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/get_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/html_tag_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/html_tag_write_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/image_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/image_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/image_set_base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/image_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/image_slide.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/image_write_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/in_market_audience_segment_brand_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/in_market_audience_segment_brand_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/in_market_audience_segment_brand_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/in_market_audience_segment_interest_entity_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/in_market_audience_segment_interest_entity_v1_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/in_market_audience_segment_interest_entity_v1_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/in_market_create_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/in_market_size_estimation_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/in_market_update_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/in_market_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/location_create_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/location_size_estimation_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/location_update_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/location_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/lookalike_create_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/lookalike_update_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11882 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/lookalike_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/modify_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/new_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/new_audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/new_audience_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/new_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/nillable_ad_set_targeting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/nillable_ad_set_targeting_rule_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11515 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/nillable_date_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11503 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/nillable_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/nillable_gender_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/nillable_int32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/nillable_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_budget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_category_bid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_category_bid_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_category_bid_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12652 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_category_bid_result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_category_bid_result_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_display_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_display_multiplier_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_display_multiplier_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_display_multiplier_result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_display_multiplier_result_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_campaign_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_campaign_spend_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12157 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_campaign_write_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_result_campaign_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_result_campaign_read_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/placements_report_query_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/placements_report_query_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16412 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/placements_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/point_of_interest_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/portfolio_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/problems_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/prospecting_create_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/prospecting_update_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/prospecting_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/read_ad_set_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13866 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/read_ad_set_budget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/read_ad_set_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/read_model_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12094 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/read_model_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/replace_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/replace_audience_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/replace_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/request_ad_set_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/requests_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/requests_patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/response_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/response_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12478 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/responses_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/responses_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/retargeting_create_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/retargeting_update_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/retargeting_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16559 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/statistics_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transactions_report_query_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transactions_report_query_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transactions_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transparency_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transparency_report_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transparency_report_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transparency_report_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transparency_report_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/update_coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/update_coupon_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/update_coupon_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/video_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/write_model_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/write_model_patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82579 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:52.634917 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    28393 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14256 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 09:55:52.634917 criteo-api-marketingsolutions-sdk-2023.7.0.230726/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:52.634917 criteo-api-marketingsolutions-sdk-2023.7.0.230726/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-26 09:54:50.000000 criteo-api-marketingsolutions-sdk-2023.7.0.230726/test/test_gateway_api.py
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/PKG-INFO` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-marketingsolutions-sdk
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
-pip install criteo-api-marketingsolutions-sdk==2023.04.0.230726
+pip install criteo-api-marketingsolutions-sdk==2023.07.0.230726
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.04.0.230726`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.07.0.230726`)
 
 Then import the package:
 ```python
-import criteo_api_marketingsolutions_v2023_04
+import criteo_api_marketingsolutions_v2023_07
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-marketingsolutions-sdk
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
-pip install criteo-api-marketingsolutions-sdk==2023.04.0.230726
+pip install criteo-api-marketingsolutions-sdk==2023.07.0.230726
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.04.0.230726`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.07.0.230726`)
 
 Then import the package:
 ```python
-import criteo_api_marketingsolutions_v2023_04
+import criteo_api_marketingsolutions_v2023_07
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/__init__.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "2023.04.0.230726"
+__version__ = "2023.07.0.230726"
 
 # import ApiClient
-from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient
-from criteo_api_marketingsolutions_v2023_04.criteo_api_client import CriteoApiClient
-from criteo_api_marketingsolutions_v2023_04.api_client_builder import ApiClientBuilder
-from criteo_api_marketingsolutions_v2023_04 import flow_constants
+from criteo_api_marketingsolutions_v2023_07.api_client import ApiClient
+from criteo_api_marketingsolutions_v2023_07.criteo_api_client import CriteoApiClient
+from criteo_api_marketingsolutions_v2023_07.api_client_builder import ApiClientBuilder
+from criteo_api_marketingsolutions_v2023_07 import flow_constants
 
 # import Configuration
-from criteo_api_marketingsolutions_v2023_04.configuration import Configuration
+from criteo_api_marketingsolutions_v2023_07.configuration import Configuration
 
 # import exceptions
-from criteo_api_marketingsolutions_v2023_04.exceptions import OpenApiException
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiTypeError
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiValueError
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiKeyError
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiException
+from criteo_api_marketingsolutions_v2023_07.exceptions import OpenApiException
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiTypeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiValueError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiKeyError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiException
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/api/advertiser_api.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api/advertiser_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_marketingsolutions_v2023_04.model.get_portfolio_response import GetPortfolioResponse
+from criteo_api_marketingsolutions_v2023_07.model.get_portfolio_response import GetPortfolioResponse
 
 
 class AdvertiserApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -38,15 +38,15 @@
         self.api_portfolio_get_endpoint = _Endpoint(
             settings={
                 'response_type': (GetPortfolioResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/advertisers/me',
+                'endpoint_path': '/2023-07/advertisers/me',
                 'operation_id': 'api_portfolio_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                 ],
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/api/analytics_api.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api/analytics_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_marketingsolutions_v2023_04.model.placements_report_query_data_message import PlacementsReportQueryDataMessage
-from criteo_api_marketingsolutions_v2023_04.model.problems_details import ProblemsDetails
-from criteo_api_marketingsolutions_v2023_04.model.statistics_report_query_message import StatisticsReportQueryMessage
-from criteo_api_marketingsolutions_v2023_04.model.transactions_report_query_data_message import TransactionsReportQueryDataMessage
-from criteo_api_marketingsolutions_v2023_04.model.transparency_query_message import TransparencyQueryMessage
-from criteo_api_marketingsolutions_v2023_04.model.transparency_report_data_message import TransparencyReportDataMessage
+from criteo_api_marketingsolutions_v2023_07.model.placements_report_query_data_message import PlacementsReportQueryDataMessage
+from criteo_api_marketingsolutions_v2023_07.model.problems_details import ProblemsDetails
+from criteo_api_marketingsolutions_v2023_07.model.statistics_report_query_message import StatisticsReportQueryMessage
+from criteo_api_marketingsolutions_v2023_07.model.transactions_report_query_data_message import TransactionsReportQueryDataMessage
+from criteo_api_marketingsolutions_v2023_07.model.transparency_query_message import TransparencyQueryMessage
+from criteo_api_marketingsolutions_v2023_07.model.transparency_report_data_message import TransparencyReportDataMessage
 
 
 class AnalyticsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -43,15 +43,15 @@
         self.get_adset_report_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/statistics/report',
+                'endpoint_path': '/2023-07/statistics/report',
                 'operation_id': 'get_adset_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'statistics_report_query_message',
@@ -102,15 +102,15 @@
         self.get_placements_report_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/placements/report',
+                'endpoint_path': '/2023-07/placements/report',
                 'operation_id': 'get_placements_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'placements_report_query_data_message',
@@ -158,15 +158,15 @@
         self.get_transactions_report_endpoint = _Endpoint(
             settings={
                 'response_type': (str,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/transactions/report',
+                'endpoint_path': '/2023-07/transactions/report',
                 'operation_id': 'get_transactions_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'transactions_report_query_data_message',
@@ -217,15 +217,15 @@
         self.get_transparency_report_endpoint = _Endpoint(
             settings={
                 'response_type': (TransparencyReportDataMessage,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/log-level/advertisers/{advertiser-id}/report',
+                'endpoint_path': '/2023-07/log-level/advertisers/{advertiser-id}/report',
                 'operation_id': 'get_transparency_report',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'advertiser_id',
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/api/campaign_api.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api/campaign_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,190 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_marketingsolutions_v2023_04.model.ad_set_category_bid_list_response import AdSetCategoryBidListResponse
-from criteo_api_marketingsolutions_v2023_04.model.ad_set_display_multiplier_list_response import AdSetDisplayMultiplierListResponse
-from criteo_api_marketingsolutions_v2023_04.model.campaign_list_response import CampaignListResponse
-from criteo_api_marketingsolutions_v2023_04.model.campaign_response import CampaignResponse
-from criteo_api_marketingsolutions_v2023_04.model.campaign_search_request import CampaignSearchRequest
-from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_category_bid_list_request import PatchAdSetCategoryBidListRequest
-from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_category_bid_result_list_response import PatchAdSetCategoryBidResultListResponse
-from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier_list_request import PatchAdSetDisplayMultiplierListRequest
-from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier_result_list_response import PatchAdSetDisplayMultiplierResultListResponse
-from criteo_api_marketingsolutions_v2023_04.model.patch_campaign_list_request import PatchCampaignListRequest
-from criteo_api_marketingsolutions_v2023_04.model.patch_result_campaign_list_response import PatchResultCampaignListResponse
-from criteo_api_marketingsolutions_v2023_04.model.request_ad_set_search import RequestAdSetSearch
-from criteo_api_marketingsolutions_v2023_04.model.requests_ad_set_id import RequestsAdSetId
-from criteo_api_marketingsolutions_v2023_04.model.requests_patch_ad_set import RequestsPatchAdSet
-from criteo_api_marketingsolutions_v2023_04.model.response_ad_set_id import ResponseAdSetId
-from criteo_api_marketingsolutions_v2023_04.model.response_read_ad_set import ResponseReadAdSet
-from criteo_api_marketingsolutions_v2023_04.model.responses_ad_set_id import ResponsesAdSetId
-from criteo_api_marketingsolutions_v2023_04.model.responses_read_ad_set import ResponsesReadAdSet
+from criteo_api_marketingsolutions_v2023_07.model.ad_set_audience_link_entity_v1_response import AdSetAudienceLinkEntityV1Response
+from criteo_api_marketingsolutions_v2023_07.model.ad_set_audience_link_input_entity_v1 import AdSetAudienceLinkInputEntityV1
+from criteo_api_marketingsolutions_v2023_07.model.ad_set_category_bid_list_response import AdSetCategoryBidListResponse
+from criteo_api_marketingsolutions_v2023_07.model.ad_set_display_multiplier_list_response import AdSetDisplayMultiplierListResponse
+from criteo_api_marketingsolutions_v2023_07.model.campaign_list_response import CampaignListResponse
+from criteo_api_marketingsolutions_v2023_07.model.campaign_response import CampaignResponse
+from criteo_api_marketingsolutions_v2023_07.model.campaign_search_request import CampaignSearchRequest
+from criteo_api_marketingsolutions_v2023_07.model.campaign_v23_q1_response import CampaignV23Q1Response
+from criteo_api_marketingsolutions_v2023_07.model.create_ad_set_request import CreateAdSetRequest
+from criteo_api_marketingsolutions_v2023_07.model.create_campaign_request import CreateCampaignRequest
+from criteo_api_marketingsolutions_v2023_07.model.patch_ad_set_category_bid_list_request import PatchAdSetCategoryBidListRequest
+from criteo_api_marketingsolutions_v2023_07.model.patch_ad_set_category_bid_result_list_response import PatchAdSetCategoryBidResultListResponse
+from criteo_api_marketingsolutions_v2023_07.model.patch_ad_set_display_multiplier_list_request import PatchAdSetDisplayMultiplierListRequest
+from criteo_api_marketingsolutions_v2023_07.model.patch_ad_set_display_multiplier_result_list_response import PatchAdSetDisplayMultiplierResultListResponse
+from criteo_api_marketingsolutions_v2023_07.model.patch_campaign_list_request import PatchCampaignListRequest
+from criteo_api_marketingsolutions_v2023_07.model.patch_result_campaign_list_response import PatchResultCampaignListResponse
+from criteo_api_marketingsolutions_v2023_07.model.request_ad_set_search import RequestAdSetSearch
+from criteo_api_marketingsolutions_v2023_07.model.requests_ad_set_id import RequestsAdSetId
+from criteo_api_marketingsolutions_v2023_07.model.requests_patch_ad_set import RequestsPatchAdSet
+from criteo_api_marketingsolutions_v2023_07.model.response_ad_set_id import ResponseAdSetId
+from criteo_api_marketingsolutions_v2023_07.model.response_read_ad_set import ResponseReadAdSet
+from criteo_api_marketingsolutions_v2023_07.model.responses_ad_set_id import ResponsesAdSetId
+from criteo_api_marketingsolutions_v2023_07.model.responses_read_ad_set import ResponsesReadAdSet
 
 
 class CampaignApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
+        self.create_ad_set_endpoint = _Endpoint(
+            settings={
+                'response_type': (ResponseReadAdSet,),
+                'auth': [
+                    'oauth',
+                    'oauth'
+                ],
+                'endpoint_path': '/2023-07/marketing-solutions/ad-sets',
+                'operation_id': 'create_ad_set',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'create_ad_set_request',
+                ],
+                'required': [
+                    'create_ad_set_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'create_ad_set_request':
+                        (CreateAdSetRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'create_ad_set_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'text/plain',
+                    'application/json',
+                    'text/json'
+                ],
+                'content_type': [
+                    'application/json-patch+json',
+                    'application/json',
+                    'text/json',
+                    'application/*+json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.create_campaign_endpoint = _Endpoint(
+            settings={
+                'response_type': (CampaignV23Q1Response,),
+                'auth': [
+                    'oauth',
+                    'oauth'
+                ],
+                'endpoint_path': '/2023-07/marketing-solutions/campaigns',
+                'operation_id': 'create_campaign',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'create_campaign_request',
+                ],
+                'required': [
+                    'create_campaign_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'create_campaign_request':
+                        (CreateCampaignRequest,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'create_campaign_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'text/plain',
+                    'application/json',
+                    'text/json'
+                ],
+                'content_type': [
+                    'application/json-patch+json',
+                    'application/json',
+                    'text/json',
+                    'application/*+json'
+                ]
+            },
+            api_client=api_client
+        )
         self.get_ad_set_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponseReadAdSet,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/{adSetId}',
+                'endpoint_path': '/2023-07/marketing-solutions/ad-sets/{adSetId}',
                 'operation_id': 'get_ad_set',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
@@ -109,15 +230,15 @@
         self.get_campaign_endpoint = _Endpoint(
             settings={
                 'response_type': (CampaignResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/marketing-solutions/campaigns/{campaign-id}',
+                'endpoint_path': '/2023-07/marketing-solutions/campaigns/{campaign-id}',
                 'operation_id': 'get_campaign',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_id',
@@ -163,15 +284,15 @@
         self.get_category_bid_list_endpoint = _Endpoint(
             settings={
                 'response_type': (AdSetCategoryBidListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/{ad-set-id}/category-bids',
+                'endpoint_path': '/2023-07/marketing-solutions/ad-sets/{ad-set-id}/category-bids',
                 'operation_id': 'get_category_bid_list',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
@@ -217,15 +338,15 @@
         self.get_display_multipliers_endpoint = _Endpoint(
             settings={
                 'response_type': (AdSetDisplayMultiplierListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/{ad-set-id}/display-multipliers',
+                'endpoint_path': '/2023-07/marketing-solutions/ad-sets/{ad-set-id}/display-multipliers',
                 'operation_id': 'get_display_multipliers',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
@@ -271,15 +392,15 @@
         self.patch_ad_sets_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponseAdSetId,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/marketing-solutions/ad-sets',
+                'endpoint_path': '/2023-07/marketing-solutions/ad-sets',
                 'operation_id': 'patch_ad_sets',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'requests_patch_ad_set',
@@ -327,15 +448,15 @@
         self.patch_campaigns_endpoint = _Endpoint(
             settings={
                 'response_type': (PatchResultCampaignListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/marketing-solutions/campaigns',
+                'endpoint_path': '/2023-07/marketing-solutions/campaigns',
                 'operation_id': 'patch_campaigns',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'patch_campaign_list_request',
@@ -383,15 +504,15 @@
         self.patch_category_bid_list_endpoint = _Endpoint(
             settings={
                 'response_type': (PatchAdSetCategoryBidResultListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/{ad-set-id}/category-bids',
+                'endpoint_path': '/2023-07/marketing-solutions/ad-sets/{ad-set-id}/category-bids',
                 'operation_id': 'patch_category_bid_list',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
@@ -446,15 +567,15 @@
         self.patch_display_multipliers_endpoint = _Endpoint(
             settings={
                 'response_type': (PatchAdSetDisplayMultiplierResultListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/{ad-set-id}/display-multipliers',
+                'endpoint_path': '/2023-07/marketing-solutions/ad-sets/{ad-set-id}/display-multipliers',
                 'operation_id': 'patch_display_multipliers',
                 'http_method': 'PATCH',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'ad_set_id',
@@ -509,15 +630,15 @@
         self.search_ad_sets_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponsesReadAdSet,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/search',
+                'endpoint_path': '/2023-07/marketing-solutions/ad-sets/search',
                 'operation_id': 'search_ad_sets',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'request_ad_set_search',
@@ -565,15 +686,15 @@
         self.search_campaigns_endpoint = _Endpoint(
             settings={
                 'response_type': (CampaignListResponse,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/marketing-solutions/campaigns/search',
+                'endpoint_path': '/2023-07/marketing-solutions/campaigns/search',
                 'operation_id': 'search_campaigns',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'campaign_search_request',
@@ -621,15 +742,15 @@
         self.start_ad_sets_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponsesAdSetId,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/start',
+                'endpoint_path': '/2023-07/marketing-solutions/ad-sets/start',
                 'operation_id': 'start_ad_sets',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'requests_ad_set_id',
@@ -677,15 +798,15 @@
         self.stop_ad_sets_endpoint = _Endpoint(
             settings={
                 'response_type': (ResponsesAdSetId,),
                 'auth': [
                     'oauth',
                     'oauth'
                 ],
-                'endpoint_path': '/2023-04/marketing-solutions/ad-sets/stop',
+                'endpoint_path': '/2023-07/marketing-solutions/ad-sets/stop',
                 'operation_id': 'stop_ad_sets',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'requests_ad_set_id',
@@ -726,14 +847,244 @@
                     'application/json',
                     'text/json',
                     'application/*+json'
                 ]
             },
             api_client=api_client
         )
+        self.update_ad_set_audience_endpoint = _Endpoint(
+            settings={
+                'response_type': (AdSetAudienceLinkEntityV1Response,),
+                'auth': [
+                    'oauth',
+                    'oauth'
+                ],
+                'endpoint_path': '/2023-07/marketing-solutions/ad-sets/{ad-set-id}/audience',
+                'operation_id': 'update_ad_set_audience',
+                'http_method': 'PUT',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'ad_set_id',
+                    'ad_set_audience_link_input_entity_v1',
+                ],
+                'required': [
+                    'ad_set_id',
+                    'ad_set_audience_link_input_entity_v1',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'ad_set_id':
+                        (str,),
+                    'ad_set_audience_link_input_entity_v1':
+                        (AdSetAudienceLinkInputEntityV1,),
+                },
+                'attribute_map': {
+                    'ad_set_id': 'ad-set-id',
+                },
+                'location_map': {
+                    'ad_set_id': 'path',
+                    'ad_set_audience_link_input_entity_v1': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'text/plain',
+                    'application/json',
+                    'text/json'
+                ],
+                'content_type': [
+                    'application/json-patch+json',
+                    'application/json',
+                    'text/json',
+                    'application/*+json'
+                ]
+            },
+            api_client=api_client
+        )
+
+    def create_ad_set(
+        self,
+        create_ad_set_request,
+        **kwargs
+    ):
+        """create_ad_set  # noqa: E501
+
+        Create the specified ad set  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_ad_set(create_ad_set_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            create_ad_set_request (CreateAdSetRequest): the ad sets to create
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ResponseReadAdSet
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['create_ad_set_request'] = \
+            create_ad_set_request
+        return self.create_ad_set_endpoint.call_with_http_info(**kwargs)
+
+    def create_campaign(
+        self,
+        create_campaign_request,
+        **kwargs
+    ):
+        """create_campaign  # noqa: E501
+
+        Create the specified campaign  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_campaign(create_campaign_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            create_campaign_request (CreateCampaignRequest): the campaigns to create
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            CampaignV23Q1Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['create_campaign_request'] = \
+            create_campaign_request
+        return self.create_campaign_endpoint.call_with_http_info(**kwargs)
 
     def get_ad_set(
         self,
         ad_set_id,
         **kwargs
     ):
         """get_ad_set  # noqa: E501
@@ -1701,7 +2052,94 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.stop_ad_sets_endpoint.call_with_http_info(**kwargs)
 
+    def update_ad_set_audience(
+        self,
+        ad_set_id,
+        ad_set_audience_link_input_entity_v1,
+        **kwargs
+    ):
+        """update_ad_set_audience  # noqa: E501
+
+        Link or unlink an audience with an ad set  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_ad_set_audience(ad_set_id, ad_set_audience_link_input_entity_v1, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            ad_set_id (str): The ad set ID.
+            ad_set_audience_link_input_entity_v1 (AdSetAudienceLinkInputEntityV1): Ad set-Audience update request.
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            AdSetAudienceLinkEntityV1Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['ad_set_id'] = \
+            ad_set_id
+        kwargs['ad_set_audience_link_input_entity_v1'] = \
+            ad_set_audience_link_input_entity_v1
+        return self.update_ad_set_audience_endpoint.call_with_http_info(**kwargs)
+
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/api/gateway_api.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api/gateway_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient, Endpoint as _Endpoint
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.api_client import ApiClient, Endpoint as _Endpoint
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
     check_allowed_values,
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
-from criteo_api_marketingsolutions_v2023_04.model.application_summary_model_response import ApplicationSummaryModelResponse
+from criteo_api_marketingsolutions_v2023_07.model.application_summary_model_response import ApplicationSummaryModelResponse
 
 
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
-                'endpoint_path': '/2023-04/marketing-solutions/me',
+                'endpoint_path': '/2023-07/marketing-solutions/me',
                 'operation_id': 'get_current_application',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                 ],
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/api_client.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
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
 
 
-from criteo_api_marketingsolutions_v2023_04 import rest
-from criteo_api_marketingsolutions_v2023_04.configuration import Configuration
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiTypeError, ApiValueError, ApiException
-from criteo_api_marketingsolutions_v2023_04.model_utils import (
+from criteo_api_marketingsolutions_v2023_07 import rest
+from criteo_api_marketingsolutions_v2023_07.configuration import Configuration
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiTypeError, ApiValueError, ApiException
+from criteo_api_marketingsolutions_v2023_07.model_utils import (
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
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/api_client_builder.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/api_client_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from criteo_api_marketingsolutions_v2023_04.configuration import Configuration
-from criteo_api_marketingsolutions_v2023_04.criteo_api_client import CriteoApiClient
-from criteo_api_marketingsolutions_v2023_04 import flow_constants
+from criteo_api_marketingsolutions_v2023_07.configuration import Configuration
+from criteo_api_marketingsolutions_v2023_07.criteo_api_client import CriteoApiClient
+from criteo_api_marketingsolutions_v2023_07 import flow_constants
 
 class ApiClientBuilder :
 
     @staticmethod
     def WithClientCredentials(clientId, clientSecret, host=None):
         configuration = Configuration(username=clientId, password=clientSecret, host=host)
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/apis/__init__.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/apis/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 # flake8: noqa
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
 # In order to avoid this, import only the API that you directly need like:
 #
-#   from criteo_api_marketingsolutions_v2023_04.api.advertiser_api import AdvertiserApi
+#   from criteo_api_marketingsolutions_v2023_07.api.advertiser_api import AdvertiserApi
 #
 # or import this package, but before doing it, use:
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
-from criteo_api_marketingsolutions_v2023_04.api.advertiser_api import AdvertiserApi
-from criteo_api_marketingsolutions_v2023_04.api.analytics_api import AnalyticsApi
-from criteo_api_marketingsolutions_v2023_04.api.audience_api import AudienceApi
-from criteo_api_marketingsolutions_v2023_04.api.campaign_api import CampaignApi
-from criteo_api_marketingsolutions_v2023_04.api.gateway_api import GatewayApi
+from criteo_api_marketingsolutions_v2023_07.api.advertiser_api import AdvertiserApi
+from criteo_api_marketingsolutions_v2023_07.api.analytics_api import AnalyticsApi
+from criteo_api_marketingsolutions_v2023_07.api.audience_api import AudienceApi
+from criteo_api_marketingsolutions_v2023_07.api.campaign_api import CampaignApi
+from criteo_api_marketingsolutions_v2023_07.api.creative_api import CreativeApi
+from criteo_api_marketingsolutions_v2023_07.api.gateway_api import GatewayApi
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/configuration.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiValueError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiValueError
 
 
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
-        self.logger["package_logger"] = logging.getLogger("criteo_api_marketingsolutions_v2023_04")
+        self.logger["package_logger"] = logging.getLogger("criteo_api_marketingsolutions_v2023_07")
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

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/criteo_api_client.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/criteo_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient
-from criteo_api_marketingsolutions_v2023_04.criteo_rest import CriteoRESTClientObject
+from criteo_api_marketingsolutions_v2023_07.api_client import ApiClient
+from criteo_api_marketingsolutions_v2023_07.criteo_rest import CriteoRESTClientObject
 
 class CriteoApiClient(ApiClient):
     def __init__(self, configuration=None, header_name=None, header_value=None,
              cookie=None, pool_threads=1, additional_parameters= {}):
         super().__init__(configuration=configuration,header_name=header_name, header_value=header_value, cookie=cookie, pool_threads=pool_threads)
         self.rest_client = CriteoRESTClientObject(self.configuration, additional_parameters)
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/criteo_auth.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/criteo_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from datetime import datetime, timedelta
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiException
-from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient
-from criteo_api_marketingsolutions_v2023_04 import flow_constants
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiException
+from criteo_api_marketingsolutions_v2023_07.api_client import ApiClient
+from criteo_api_marketingsolutions_v2023_07 import flow_constants
 
 class Token(object):
 
     def __init__(self, token_string , expiration_date = None):
         self.expiration_date = expiration_date 
         self.token_string = token_string
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/criteo_rest.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/criteo_rest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from criteo_api_marketingsolutions_v2023_04.rest import RESTClientObject
-from criteo_api_marketingsolutions_v2023_04.criteo_auth import *
-from criteo_api_marketingsolutions_v2023_04 import flow_constants
+from criteo_api_marketingsolutions_v2023_07.rest import RESTClientObject
+from criteo_api_marketingsolutions_v2023_07.criteo_auth import *
+from criteo_api_marketingsolutions_v2023_07 import flow_constants
 
 
 class CriteoRESTClientObject(RESTClientObject):
 
     def __init__(self, configuration, additional_parameters = {}, pools_size=4, maxsize=None):
         super().__init__(configuration, pools_size, maxsize)
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/exceptions.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_category_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class AdSetCategoryBid(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_category_bid_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.ad_set_category_bid_resource import AdSetCategoryBidResource
-    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_07.model.ad_set_category_bid_resource import AdSetCategoryBidResource
+    from criteo_api_marketingsolutions_v2023_07.model.problem_details import ProblemDetails
     globals()['AdSetCategoryBidResource'] = AdSetCategoryBidResource
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class AdSetCategoryBidListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_resource.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_category_bid_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.ad_set_category_bid import AdSetCategoryBid
+    from criteo_api_marketingsolutions_v2023_07.model.ad_set_category_bid import AdSetCategoryBid
     globals()['AdSetCategoryBid'] = AdSetCategoryBid
 
 
 class AdSetCategoryBidResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_delivery_limitations.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_delivery_limitations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class AdSetDeliveryLimitations(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_display_multiplier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class AdSetDisplayMultiplier(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_display_multiplier_list_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.ad_set_display_multiplier_resource import AdSetDisplayMultiplierResource
-    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_07.model.ad_set_display_multiplier_resource import AdSetDisplayMultiplierResource
+    from criteo_api_marketingsolutions_v2023_07.model.problem_details import ProblemDetails
     globals()['AdSetDisplayMultiplierResource'] = AdSetDisplayMultiplierResource
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class AdSetDisplayMultiplierListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_resource.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_display_multiplier_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.ad_set_display_multiplier import AdSetDisplayMultiplier
+    from criteo_api_marketingsolutions_v2023_07.model.ad_set_display_multiplier import AdSetDisplayMultiplier
     globals()['AdSetDisplayMultiplier'] = AdSetDisplayMultiplier
 
 
 class AdSetDisplayMultiplierResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_frequency_capping.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_frequency_capping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class AdSetFrequencyCapping(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_geo_location.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_geo_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.nillable_ad_set_targeting_rule import NillableAdSetTargetingRule
+    from criteo_api_marketingsolutions_v2023_07.model.nillable_ad_set_targeting_rule import NillableAdSetTargetingRule
     globals()['NillableAdSetTargetingRule'] = NillableAdSetTargetingRule
 
 
 class AdSetGeoLocation(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_search_filter.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_search_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class AdSetSearchFilter(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_targeting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.ad_set_delivery_limitations import AdSetDeliveryLimitations
-    from criteo_api_marketingsolutions_v2023_04.model.ad_set_frequency_capping import AdSetFrequencyCapping
-    from criteo_api_marketingsolutions_v2023_04.model.ad_set_geo_location import AdSetGeoLocation
+    from criteo_api_marketingsolutions_v2023_07.model.ad_set_delivery_limitations import AdSetDeliveryLimitations
+    from criteo_api_marketingsolutions_v2023_07.model.ad_set_frequency_capping import AdSetFrequencyCapping
+    from criteo_api_marketingsolutions_v2023_07.model.ad_set_geo_location import AdSetGeoLocation
     globals()['AdSetDeliveryLimitations'] = AdSetDeliveryLimitations
     globals()['AdSetFrequencyCapping'] = AdSetFrequencyCapping
     globals()['AdSetGeoLocation'] = AdSetGeoLocation
 
 
 class AdSetTargeting(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting_rule.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/ad_set_targeting_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class AdSetTargetingRule(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/application_summary_model.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/application_summary_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ApplicationSummaryModel(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_resource.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/application_summary_model_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.application_summary_model import ApplicationSummaryModel
+    from criteo_api_marketingsolutions_v2023_07.model.application_summary_model import ApplicationSummaryModel
     globals()['ApplicationSummaryModel'] = ApplicationSummaryModel
 
 
 class ApplicationSummaryModelResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/application_summary_model_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.application_summary_model_resource import ApplicationSummaryModelResource
-    from criteo_api_marketingsolutions_v2023_04.model.common_problem import CommonProblem
+    from criteo_api_marketingsolutions_v2023_07.model.application_summary_model_resource import ApplicationSummaryModelResource
+    from criteo_api_marketingsolutions_v2023_07.model.common_problem import CommonProblem
     globals()['ApplicationSummaryModelResource'] = ApplicationSummaryModelResource
     globals()['CommonProblem'] = CommonProblem
 
 
 class ApplicationSummaryModelResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/audience.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.audience_attributes import AudienceAttributes
+    from criteo_api_marketingsolutions_v2023_07.model.audience_attributes import AudienceAttributes
     globals()['AudienceAttributes'] = AudienceAttributes
 
 
 class Audience(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/audience_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class AudienceAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/audience_error.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class AudienceError(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/audience_name_description.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_name_description.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class AudienceNameDescription(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/audience_warning.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/audience_warning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class AudienceWarning(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/basic_audience_definition.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/basic_audience_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.audience_name_description import AudienceNameDescription
+    from criteo_api_marketingsolutions_v2023_07.model.audience_name_description import AudienceNameDescription
     globals()['AudienceNameDescription'] = AudienceNameDescription
 
 
 class BasicAudienceDefinition(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/campaign.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.campaign_spend_limit import CampaignSpendLimit
+    from criteo_api_marketingsolutions_v2023_07.model.campaign_spend_limit import CampaignSpendLimit
     globals()['CampaignSpendLimit'] = CampaignSpendLimit
 
 
 class Campaign(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/campaign_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.campaign_read_resource import CampaignReadResource
-    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_07.model.campaign_read_resource import CampaignReadResource
+    from criteo_api_marketingsolutions_v2023_07.model.problem_details import ProblemDetails
     globals()['CampaignReadResource'] = CampaignReadResource
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class CampaignListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/campaign_read_resource.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_read_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.campaign import Campaign
+    from criteo_api_marketingsolutions_v2023_07.model.campaign import Campaign
     globals()['Campaign'] = Campaign
 
 
 class CampaignReadResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/campaign_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.campaign_read_resource import CampaignReadResource
-    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_07.model.campaign_read_resource import CampaignReadResource
+    from criteo_api_marketingsolutions_v2023_07.model.problem_details import ProblemDetails
     globals()['CampaignReadResource'] = CampaignReadResource
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class CampaignResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/campaign_search_filters.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_search_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class CampaignSearchFilters(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/campaign_search_request.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_search_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.campaign_search_filters import CampaignSearchFilters
+    from criteo_api_marketingsolutions_v2023_07.model.campaign_search_filters import CampaignSearchFilters
     globals()['CampaignSearchFilters'] = CampaignSearchFilters
 
 
 class CampaignSearchRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/campaign_spend_limit.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/campaign_spend_limit_v23_q1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2023_07.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
-class CampaignSpendLimit(ModelNormal):
+class CampaignSpendLimitV23Q1(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -117,15 +117,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CampaignSpendLimit - a model defined in OpenAPI
+        """CampaignSpendLimitV23Q1 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -205,15 +205,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CampaignSpendLimit - a model defined in OpenAPI
+        """CampaignSpendLimitV23Q1 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/common_problem.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/common_problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class CommonProblem(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/contactlist_amendment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.contactlist_amendment_attributes import ContactlistAmendmentAttributes
+    from criteo_api_marketingsolutions_v2023_07.model.contactlist_amendment_attributes import ContactlistAmendmentAttributes
     globals()['ContactlistAmendmentAttributes'] = ContactlistAmendmentAttributes
 
 
 class ContactlistAmendment(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/contactlist_amendment_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ContactlistAmendmentAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_request.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/contactlist_amendment_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.contactlist_amendment import ContactlistAmendment
+    from criteo_api_marketingsolutions_v2023_07.model.contactlist_amendment import ContactlistAmendment
     globals()['ContactlistAmendment'] = ContactlistAmendment
 
 
 class ContactlistAmendmentRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/contactlist_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.contactlist_operation_attributes import ContactlistOperationAttributes
+    from criteo_api_marketingsolutions_v2023_07.model.contactlist_operation_attributes import ContactlistOperationAttributes
     globals()['ContactlistOperationAttributes'] = ContactlistOperationAttributes
 
 
 class ContactlistOperation(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/contactlist_operation_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ContactlistOperationAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/criteo_api_error.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/criteo_api_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class CriteoApiError(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/criteo_api_warning.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/criteo_api_warning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class CriteoApiWarning(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/delete_audience_contact_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/delete_audience_contact_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2023_04.model.audience_warning import AudienceWarning
-    from criteo_api_marketingsolutions_v2023_04.model.basic_audience_definition import BasicAudienceDefinition
+    from criteo_api_marketingsolutions_v2023_07.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2023_07.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2023_07.model.basic_audience_definition import BasicAudienceDefinition
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
     globals()['BasicAudienceDefinition'] = BasicAudienceDefinition
 
 
 class DeleteAudienceContactListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/delete_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/delete_audience_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2023_04.model.audience_warning import AudienceWarning
-    from criteo_api_marketingsolutions_v2023_04.model.basic_audience_definition import BasicAudienceDefinition
+    from criteo_api_marketingsolutions_v2023_07.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2023_07.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2023_07.model.basic_audience_definition import BasicAudienceDefinition
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
     globals()['BasicAudienceDefinition'] = BasicAudienceDefinition
 
 
 class DeleteAudienceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/entity_of_portfolio_message.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/entity_of_portfolio_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.portfolio_message import PortfolioMessage
+    from criteo_api_marketingsolutions_v2023_07.model.portfolio_message import PortfolioMessage
     globals()['PortfolioMessage'] = PortfolioMessage
 
 
 class EntityOfPortfolioMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/error_code_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/error_code_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2023_04.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2023_07.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2023_07.model.audience_warning import AudienceWarning
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
 
 
 class ErrorCodeResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/get_audiences_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/get_audiences_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.audience import Audience
-    from criteo_api_marketingsolutions_v2023_04.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2023_04.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2023_07.model.audience import Audience
+    from criteo_api_marketingsolutions_v2023_07.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2023_07.model.audience_warning import AudienceWarning
     globals()['Audience'] = Audience
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
 
 
 class GetAudiencesResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/get_portfolio_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/get_portfolio_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.criteo_api_error import CriteoApiError
-    from criteo_api_marketingsolutions_v2023_04.model.criteo_api_warning import CriteoApiWarning
-    from criteo_api_marketingsolutions_v2023_04.model.entity_of_portfolio_message import EntityOfPortfolioMessage
+    from criteo_api_marketingsolutions_v2023_07.model.criteo_api_error import CriteoApiError
+    from criteo_api_marketingsolutions_v2023_07.model.criteo_api_warning import CriteoApiWarning
+    from criteo_api_marketingsolutions_v2023_07.model.entity_of_portfolio_message import EntityOfPortfolioMessage
     globals()['CriteoApiError'] = CriteoApiError
     globals()['CriteoApiWarning'] = CriteoApiWarning
     globals()['EntityOfPortfolioMessage'] = EntityOfPortfolioMessage
 
 
 class GetPortfolioResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/modify_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/modify_audience_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2023_04.model.audience_warning import AudienceWarning
-    from criteo_api_marketingsolutions_v2023_04.model.contactlist_operation import ContactlistOperation
+    from criteo_api_marketingsolutions_v2023_07.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2023_07.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2023_07.model.contactlist_operation import ContactlistOperation
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
     globals()['ContactlistOperation'] = ContactlistOperation
 
 
 class ModifyAudienceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/new_audience.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/new_audience.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.new_audience_attributes import NewAudienceAttributes
+    from criteo_api_marketingsolutions_v2023_07.model.new_audience_attributes import NewAudienceAttributes
     globals()['NewAudienceAttributes'] = NewAudienceAttributes
 
 
 class NewAudience(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/new_audience_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/new_audience_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class NewAudienceAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/new_audience_request.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/new_audience_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.new_audience import NewAudience
+    from criteo_api_marketingsolutions_v2023_07.model.new_audience import NewAudience
     globals()['NewAudience'] = NewAudience
 
 
 class NewAudienceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/new_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/new_audience_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2023_04.model.audience_warning import AudienceWarning
-    from criteo_api_marketingsolutions_v2023_04.model.basic_audience_definition import BasicAudienceDefinition
+    from criteo_api_marketingsolutions_v2023_07.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2023_07.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2023_07.model.basic_audience_definition import BasicAudienceDefinition
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
     globals()['BasicAudienceDefinition'] = BasicAudienceDefinition
 
 
 class NewAudienceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/nillable_ad_set_targeting_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.nillable_ad_set_targeting_rule_value import NillableAdSetTargetingRuleValue
+    from criteo_api_marketingsolutions_v2023_07.model.nillable_ad_set_targeting_rule_value import NillableAdSetTargetingRuleValue
     globals()['NillableAdSetTargetingRuleValue'] = NillableAdSetTargetingRuleValue
 
 
 class NillableAdSetTargetingRule(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule_value.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/nillable_ad_set_targeting_rule_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.ad_set_targeting_rule import AdSetTargetingRule
+    from criteo_api_marketingsolutions_v2023_07.model.ad_set_targeting_rule import AdSetTargetingRule
     globals()['AdSetTargetingRule'] = AdSetTargetingRule
 
 
 class NillableAdSetTargetingRuleValue(ModelComposed):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/nillable_date_time.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/nillable_date_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class NillableDateTime(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/nillable_decimal.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/nillable_decimal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class NillableDecimal(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.ad_set_targeting import AdSetTargeting
-    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_bidding import PatchAdSetBidding
-    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_budget import PatchAdSetBudget
-    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_scheduling import PatchAdSetScheduling
+    from criteo_api_marketingsolutions_v2023_07.model.ad_set_targeting import AdSetTargeting
+    from criteo_api_marketingsolutions_v2023_07.model.patch_ad_set_bidding import PatchAdSetBidding
+    from criteo_api_marketingsolutions_v2023_07.model.patch_ad_set_budget import PatchAdSetBudget
+    from criteo_api_marketingsolutions_v2023_07.model.patch_ad_set_scheduling import PatchAdSetScheduling
     globals()['AdSetTargeting'] = AdSetTargeting
     globals()['PatchAdSetBidding'] = PatchAdSetBidding
     globals()['PatchAdSetBudget'] = PatchAdSetBudget
     globals()['PatchAdSetScheduling'] = PatchAdSetScheduling
 
 
 class PatchAdSet(ModelNormal):
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_bidding.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_bidding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2023_07.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class PatchAdSetBidding(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_budget.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_budget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2023_07.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class PatchAdSetBudget(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_category_bid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class PatchAdSetCategoryBid(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_list_request.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_category_bid_list_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_category_bid_resource import PatchAdSetCategoryBidResource
+    from criteo_api_marketingsolutions_v2023_07.model.patch_ad_set_category_bid_resource import PatchAdSetCategoryBidResource
     globals()['PatchAdSetCategoryBidResource'] = PatchAdSetCategoryBidResource
 
 
 class PatchAdSetCategoryBidListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_resource.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_category_bid_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_category_bid import PatchAdSetCategoryBid
+    from criteo_api_marketingsolutions_v2023_07.model.patch_ad_set_category_bid import PatchAdSetCategoryBid
     globals()['PatchAdSetCategoryBid'] = PatchAdSetCategoryBid
 
 
 class PatchAdSetCategoryBidResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_category_bid_result_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_category_bid_result_resource import PatchAdSetCategoryBidResultResource
-    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_07.model.patch_ad_set_category_bid_result_resource import PatchAdSetCategoryBidResultResource
+    from criteo_api_marketingsolutions_v2023_07.model.problem_details import ProblemDetails
     globals()['PatchAdSetCategoryBidResultResource'] = PatchAdSetCategoryBidResultResource
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class PatchAdSetCategoryBidResultListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_resource.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_category_bid_result_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class PatchAdSetCategoryBidResultResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_display_multiplier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class PatchAdSetDisplayMultiplier(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_list_request.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_display_multiplier_list_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier_resource import PatchAdSetDisplayMultiplierResource
+    from criteo_api_marketingsolutions_v2023_07.model.patch_ad_set_display_multiplier_resource import PatchAdSetDisplayMultiplierResource
     globals()['PatchAdSetDisplayMultiplierResource'] = PatchAdSetDisplayMultiplierResource
 
 
 class PatchAdSetDisplayMultiplierListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_resource.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_display_multiplier_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier import PatchAdSetDisplayMultiplier
+    from criteo_api_marketingsolutions_v2023_07.model.patch_ad_set_display_multiplier import PatchAdSetDisplayMultiplier
     globals()['PatchAdSetDisplayMultiplier'] = PatchAdSetDisplayMultiplier
 
 
 class PatchAdSetDisplayMultiplierResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_display_multiplier_result_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier_result_resource import PatchAdSetDisplayMultiplierResultResource
-    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_07.model.patch_ad_set_display_multiplier_result_resource import PatchAdSetDisplayMultiplierResultResource
+    from criteo_api_marketingsolutions_v2023_07.model.problem_details import ProblemDetails
     globals()['PatchAdSetDisplayMultiplierResultResource'] = PatchAdSetDisplayMultiplierResultResource
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class PatchAdSetDisplayMultiplierResultListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_resource.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_display_multiplier_result_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class PatchAdSetDisplayMultiplierResultResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_scheduling.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_ad_set_scheduling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.nillable_date_time import NillableDateTime
+    from criteo_api_marketingsolutions_v2023_07.model.nillable_date_time import NillableDateTime
     globals()['NillableDateTime'] = NillableDateTime
 
 
 class PatchAdSetScheduling(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_campaign.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_campaign.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.patch_campaign_spend_limit import PatchCampaignSpendLimit
+    from criteo_api_marketingsolutions_v2023_07.model.patch_campaign_spend_limit import PatchCampaignSpendLimit
     globals()['PatchCampaignSpendLimit'] = PatchCampaignSpendLimit
 
 
 class PatchCampaign(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_list_request.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_campaign_list_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.patch_campaign_write_resource import PatchCampaignWriteResource
+    from criteo_api_marketingsolutions_v2023_07.model.patch_campaign_write_resource import PatchCampaignWriteResource
     globals()['PatchCampaignWriteResource'] = PatchCampaignWriteResource
 
 
 class PatchCampaignListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_spend_limit.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_campaign_spend_limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2023_07.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class PatchCampaignSpendLimit(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_write_resource.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_campaign_write_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.patch_campaign import PatchCampaign
+    from criteo_api_marketingsolutions_v2023_07.model.patch_campaign import PatchCampaign
     globals()['PatchCampaign'] = PatchCampaign
 
 
 class PatchCampaignWriteResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_result_campaign_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.patch_result_campaign_read_resource import PatchResultCampaignReadResource
-    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_07.model.patch_result_campaign_read_resource import PatchResultCampaignReadResource
+    from criteo_api_marketingsolutions_v2023_07.model.problem_details import ProblemDetails
     globals()['PatchResultCampaignReadResource'] = PatchResultCampaignReadResource
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class PatchResultCampaignListResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_read_resource.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/patch_result_campaign_read_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class PatchResultCampaignReadResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_data_message.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/placements_report_query_data_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.placements_report_query_entity_message import PlacementsReportQueryEntityMessage
+    from criteo_api_marketingsolutions_v2023_07.model.placements_report_query_entity_message import PlacementsReportQueryEntityMessage
     globals()['PlacementsReportQueryEntityMessage'] = PlacementsReportQueryEntityMessage
 
 
 class PlacementsReportQueryDataMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_entity_message.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/placements_report_query_entity_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.placements_report_query_message import PlacementsReportQueryMessage
+    from criteo_api_marketingsolutions_v2023_07.model.placements_report_query_message import PlacementsReportQueryMessage
     globals()['PlacementsReportQueryMessage'] = PlacementsReportQueryMessage
 
 
 class PlacementsReportQueryEntityMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/placements_report_query_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class PlacementsReportQueryMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/portfolio_message.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/portfolio_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class PortfolioMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/problem_details.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ProblemDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/problems_details.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/problems_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_07.model.problem_details import ProblemDetails
     globals()['ProblemDetails'] = ProblemDetails
 
 
 class ProblemsDetails(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/read_ad_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.ad_set_targeting import AdSetTargeting
-    from criteo_api_marketingsolutions_v2023_04.model.read_ad_set_bidding import ReadAdSetBidding
-    from criteo_api_marketingsolutions_v2023_04.model.read_ad_set_budget import ReadAdSetBudget
-    from criteo_api_marketingsolutions_v2023_04.model.read_ad_set_schedule import ReadAdSetSchedule
+    from criteo_api_marketingsolutions_v2023_07.model.ad_set_targeting import AdSetTargeting
+    from criteo_api_marketingsolutions_v2023_07.model.read_ad_set_bidding import ReadAdSetBidding
+    from criteo_api_marketingsolutions_v2023_07.model.read_ad_set_budget import ReadAdSetBudget
+    from criteo_api_marketingsolutions_v2023_07.model.read_ad_set_schedule import ReadAdSetSchedule
     globals()['AdSetTargeting'] = AdSetTargeting
     globals()['ReadAdSetBidding'] = ReadAdSetBidding
     globals()['ReadAdSetBudget'] = ReadAdSetBudget
     globals()['ReadAdSetSchedule'] = ReadAdSetSchedule
 
 
 class ReadAdSet(ModelNormal):
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_bidding.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/read_ad_set_bidding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2023_07.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class ReadAdSetBidding(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_budget.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/read_ad_set_budget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.nillable_decimal import NillableDecimal
+    from criteo_api_marketingsolutions_v2023_07.model.nillable_decimal import NillableDecimal
     globals()['NillableDecimal'] = NillableDecimal
 
 
 class ReadAdSetBudget(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_schedule.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/read_ad_set_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.nillable_date_time import NillableDateTime
+    from criteo_api_marketingsolutions_v2023_07.model.nillable_date_time import NillableDateTime
     globals()['NillableDateTime'] = NillableDateTime
 
 
 class ReadAdSetSchedule(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/read_model_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/read_model_ad_set_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class ReadModelAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/read_model_read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/read_model_read_ad_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.read_ad_set import ReadAdSet
+    from criteo_api_marketingsolutions_v2023_07.model.read_ad_set import ReadAdSet
     globals()['ReadAdSet'] = ReadAdSet
 
 
 class ReadModelReadAdSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/replace_audience.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/replace_audience.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.audience_name_description import AudienceNameDescription
+    from criteo_api_marketingsolutions_v2023_07.model.audience_name_description import AudienceNameDescription
     globals()['AudienceNameDescription'] = AudienceNameDescription
 
 
 class ReplaceAudience(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/replace_audience_request.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/replace_audience_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.replace_audience import ReplaceAudience
+    from criteo_api_marketingsolutions_v2023_07.model.replace_audience import ReplaceAudience
     globals()['ReplaceAudience'] = ReplaceAudience
 
 
 class ReplaceAudienceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/replace_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/replace_audience_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.audience_error import AudienceError
-    from criteo_api_marketingsolutions_v2023_04.model.audience_warning import AudienceWarning
-    from criteo_api_marketingsolutions_v2023_04.model.basic_audience_definition import BasicAudienceDefinition
+    from criteo_api_marketingsolutions_v2023_07.model.audience_error import AudienceError
+    from criteo_api_marketingsolutions_v2023_07.model.audience_warning import AudienceWarning
+    from criteo_api_marketingsolutions_v2023_07.model.basic_audience_definition import BasicAudienceDefinition
     globals()['AudienceError'] = AudienceError
     globals()['AudienceWarning'] = AudienceWarning
     globals()['BasicAudienceDefinition'] = BasicAudienceDefinition
 
 
 class ReplaceAudienceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/request_ad_set_search.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/request_ad_set_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.ad_set_search_filter import AdSetSearchFilter
+    from criteo_api_marketingsolutions_v2023_07.model.ad_set_search_filter import AdSetSearchFilter
     globals()['AdSetSearchFilter'] = AdSetSearchFilter
 
 
 class RequestAdSetSearch(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/requests_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/requests_ad_set_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.write_model_ad_set_id import WriteModelAdSetId
+    from criteo_api_marketingsolutions_v2023_07.model.write_model_ad_set_id import WriteModelAdSetId
     globals()['WriteModelAdSetId'] = WriteModelAdSetId
 
 
 class RequestsAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/requests_patch_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/requests_patch_ad_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.write_model_patch_ad_set import WriteModelPatchAdSet
+    from criteo_api_marketingsolutions_v2023_07.model.write_model_patch_ad_set import WriteModelPatchAdSet
     globals()['WriteModelPatchAdSet'] = WriteModelPatchAdSet
 
 
 class RequestsPatchAdSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/response_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/response_ad_set_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_marketingsolutions_v2023_04.model.read_model_ad_set_id import ReadModelAdSetId
+    from criteo_api_marketingsolutions_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_07.model.read_model_ad_set_id import ReadModelAdSetId
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ReadModelAdSetId'] = ReadModelAdSetId
 
 
 class ResponseAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/response_read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/response_read_ad_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_marketingsolutions_v2023_04.model.read_model_read_ad_set import ReadModelReadAdSet
+    from criteo_api_marketingsolutions_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_07.model.read_model_read_ad_set import ReadModelReadAdSet
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ReadModelReadAdSet'] = ReadModelReadAdSet
 
 
 class ResponseReadAdSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/responses_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/responses_ad_set_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_marketingsolutions_v2023_04.model.read_model_ad_set_id import ReadModelAdSetId
+    from criteo_api_marketingsolutions_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_07.model.read_model_ad_set_id import ReadModelAdSetId
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ReadModelAdSetId'] = ReadModelAdSetId
 
 
 class ResponsesAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/responses_read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/responses_read_ad_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.problem_details import ProblemDetails
-    from criteo_api_marketingsolutions_v2023_04.model.read_model_read_ad_set import ReadModelReadAdSet
+    from criteo_api_marketingsolutions_v2023_07.model.problem_details import ProblemDetails
+    from criteo_api_marketingsolutions_v2023_07.model.read_model_read_ad_set import ReadModelReadAdSet
     globals()['ProblemDetails'] = ProblemDetails
     globals()['ReadModelReadAdSet'] = ReadModelReadAdSet
 
 
 class ResponsesReadAdSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/statistics_report_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/statistics_report_query_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class StatisticsReportQueryMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_data_message.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transactions_report_query_data_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.transactions_report_query_entity_message import TransactionsReportQueryEntityMessage
+    from criteo_api_marketingsolutions_v2023_07.model.transactions_report_query_entity_message import TransactionsReportQueryEntityMessage
     globals()['TransactionsReportQueryEntityMessage'] = TransactionsReportQueryEntityMessage
 
 
 class TransactionsReportQueryDataMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_entity_message.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transactions_report_query_entity_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.transactions_report_query_message import TransactionsReportQueryMessage
+    from criteo_api_marketingsolutions_v2023_07.model.transactions_report_query_message import TransactionsReportQueryMessage
     globals()['TransactionsReportQueryMessage'] = TransactionsReportQueryMessage
 
 
 class TransactionsReportQueryEntityMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transactions_report_query_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class TransactionsReportQueryMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transparency_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transparency_query_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class TransparencyQueryMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transparency_report_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transparency_report_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.transparency_report_file import TransparencyReportFile
+    from criteo_api_marketingsolutions_v2023_07.model.transparency_report_file import TransparencyReportFile
     globals()['TransparencyReportFile'] = TransparencyReportFile
 
 
 class TransparencyReportAttributes(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transparency_report_data_message.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transparency_report_data_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.transparency_report_entity_message import TransparencyReportEntityMessage
+    from criteo_api_marketingsolutions_v2023_07.model.transparency_report_entity_message import TransparencyReportEntityMessage
     globals()['TransparencyReportEntityMessage'] = TransparencyReportEntityMessage
 
 
 class TransparencyReportDataMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transparency_report_entity_message.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transparency_report_entity_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.transparency_report_attributes import TransparencyReportAttributes
+    from criteo_api_marketingsolutions_v2023_07.model.transparency_report_attributes import TransparencyReportAttributes
     globals()['TransparencyReportAttributes'] = TransparencyReportAttributes
 
 
 class TransparencyReportEntityMessage(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/transparency_report_file.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/transparency_report_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class TransparencyReportFile(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/write_model_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/write_model_ad_set_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 
 class WriteModelAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model/write_model_patch_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model/write_model_patch_ad_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
-    The version of the OpenAPI document: 2023-04
+    The version of the OpenAPI document: 2023-07
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
-from criteo_api_marketingsolutions_v2023_04.model_utils import (  # noqa: F401
+from criteo_api_marketingsolutions_v2023_07.model_utils import (  # noqa: F401
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
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set import PatchAdSet
+    from criteo_api_marketingsolutions_v2023_07.model.patch_ad_set import PatchAdSet
     globals()['PatchAdSet'] = PatchAdSet
 
 
 class WriteModelPatchAdSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/model_utils.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
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
 
-from criteo_api_marketingsolutions_v2023_04.exceptions import (
+from criteo_api_marketingsolutions_v2023_07.exceptions import (
     ApiKeyError,
     ApiAttributeError,
     ApiTypeError,
     ApiValueError,
 )
 
 none_type = type(None)
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/criteo_api_marketingsolutions_v2023_04/rest.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/criteo_api_marketingsolutions_v2023_07/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Criteo API
 
     Criteo API - MarketingSolutions  # noqa: E501
 
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
 
-from criteo_api_marketingsolutions_v2023_04.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
+from criteo_api_marketingsolutions_v2023_07.exceptions import ApiException, UnauthorizedException, ForbiddenException, NotFoundException, ServiceException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTResponse(io.IOBase):
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/setup.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "criteo-api-marketingsolutions-sdk"
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
-pip install criteo-api-marketingsolutions-sdk==2023.04.0.230726
+pip install criteo-api-marketingsolutions-sdk==2023.07.0.230726
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.04.0.230726`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.07.0.230726`)
 
 Then import the package:
 ```python
-import criteo_api_marketingsolutions_v2023_04
+import criteo_api_marketingsolutions_v2023_07
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
 
 ## Disclaimer
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230726/test/test_gateway_api.py` & `criteo-api-marketingsolutions-sdk-2023.7.0.230726/test/test_gateway_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import os
 
-from criteo_api_marketingsolutions_v2023_04.api.gateway_api import GatewayApi
-from criteo_api_marketingsolutions_v2023_04.api_client_builder import ApiClientBuilder
-from criteo_api_marketingsolutions_v2023_04.rest import ApiException
+from criteo_api_marketingsolutions_v2023_07.api.gateway_api import GatewayApi
+from criteo_api_marketingsolutions_v2023_07.api_client_builder import ApiClientBuilder
+from criteo_api_marketingsolutions_v2023_07.rest import ApiException
 from example_application_with_client_credentials import ExampleApplication
 
 class TestGatewayApi:
   @pytest.fixture(autouse=True)
   def before_each(self):
     self.client_id = os.environ.get("TEST_CLIENT_ID")
     self.client_secret = os.environ.get("TEST_CLIENT_SECRET")
```

