# Comparing `tmp/rime_sdk-2.2.0rc3.tar.gz` & `tmp/rime_sdk-2.2.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rime_sdk-2.2.0rc3.tar", last modified: Thu Jul 20 04:41:45 2023, max compression
+gzip compressed data, was "rime_sdk-2.2.0rc4.tar", last modified: Wed Jul 26 20:33:38 2023, max compression
```

## Comparing `rime_sdk-2.2.0rc3.tar` & `rime_sdk-2.2.0rc4.tar`

### file list

```diff
@@ -1,497 +1,512 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.720434 rime_sdk-2.2.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-20 04:41:45.720434 rime_sdk-2.2.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.676434 rime_sdk-2.2.0rc3/rime_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63997 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.676434 rime_sdk-2.2.0rc3/rime_sdk/data_format_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/data_format_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/data_format_check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/data_format_check/data_format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/data_format_check/nlp_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/data_format_check/tabular_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    26099 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.676434 rime_sdk-2.2.0rc3/rime_sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15159 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/rest_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/security_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/swagger_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/swagger_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/throttle_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    73004 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    27443 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.676434 rime_sdk-2.2.0rc3/rime_sdk/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.676434 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)    47967 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.680434 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35443 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/config_validator_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/data_collector_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/detection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/file_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/image_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26888 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/integration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26961 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/job_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21630 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/model_testing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29459 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    55813 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/project_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57319 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/registry_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    72408 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/results_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/rime_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40185 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25498 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/validation_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46002 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.720434 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    45826 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/model_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_object_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    10410 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_config_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_float_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_int_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_language.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_named_double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_str_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_token_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/role_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16800 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    16128 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_private_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_user_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-07-20 04:41:41.000000 rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/rime_sdk/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 04:41:45.676434 rime_sdk-2.2.0rc3/rime_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-20 04:41:45.000000 rime_sdk-2.2.0rc3/rime_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33057 2023-07-20 04:41:45.000000 rime_sdk-2.2.0rc3/rime_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 04:41:45.000000 rime_sdk-2.2.0rc3/rime_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-20 04:41:45.000000 rime_sdk-2.2.0rc3/rime_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-20 04:41:45.000000 rime_sdk-2.2.0rc3/rime_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 04:41:45.000000 rime_sdk-2.2.0rc3/rime_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 04:41:45.720434 rime_sdk-2.2.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-20 04:41:05.000000 rime_sdk-2.2.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:33:38.606129 rime_sdk-2.2.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-26 20:33:38.606129 rime_sdk-2.2.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:33:38.522128 rime_sdk-2.2.0rc4/rime_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63997 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:33:38.522128 rime_sdk-2.2.0rc4/rime_sdk/data_format_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/data_format_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/data_format_check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/data_format_check/data_format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/data_format_check/nlp_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/data_format_check/tabular_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26020 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/generative_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:33:38.522128 rime_sdk-2.2.0rc4/rime_sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15590 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/internal/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/internal/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/internal/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/internal/rest_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/internal/security_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/internal/swagger_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/internal/swagger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/internal/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/internal/throttle_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73004 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27443 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:33:38.522128 rime_sdk-2.2.0rc4/rime_sdk/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:33:38.526128 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    49578 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:33:38.526128 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35619 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/config_validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25305 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/data_collector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/detection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18198 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/file_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/firewall_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/firewall_configuration_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22570 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28418 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/image_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27020 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/integration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27071 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/job_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21740 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19359 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/model_testing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29591 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19832 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56077 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/project_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57583 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/registry_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72694 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/results_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/rime_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40405 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25630 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/validation_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46222 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:33:38.606129 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    47264 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15539 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/detection_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/detection_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_configure_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_get_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_validation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/generativefirewall_validation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/model_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notification_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notification_object_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10410 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_float_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_int_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_named_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_str_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_table_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_token_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/role_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16800 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16128 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/user_private_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/user_user_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/validate_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/validate_request_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-07-26 20:33:34.000000 rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/rime_sdk/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:33:38.522128 rime_sdk-2.2.0rc4/rime_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-26 20:33:38.000000 rime_sdk-2.2.0rc4/rime_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34139 2023-07-26 20:33:38.000000 rime_sdk-2.2.0rc4/rime_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:33:38.000000 rime_sdk-2.2.0rc4/rime_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-26 20:33:38.000000 rime_sdk-2.2.0rc4/rime_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-26 20:33:38.000000 rime_sdk-2.2.0rc4/rime_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 20:33:38.000000 rime_sdk-2.2.0rc4/rime_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 20:33:38.606129 rime_sdk-2.2.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-26 20:32:48.000000 rime_sdk-2.2.0rc4/setup.py
```

### Comparing `rime_sdk-2.2.0rc3/LICENSE` & `rime_sdk-2.2.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/PKG-INFO` & `rime_sdk-2.2.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime_sdk
-Version: 2.2.0rc3
+Version: 2.2.0rc4
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.2.0rc3/README.md` & `rime_sdk-2.2.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/__init__.py` & `rime_sdk-2.2.0rc4/rime_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/client.py` & `rime_sdk-2.2.0rc4/rime_sdk/client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/data_collector.py` & `rime_sdk-2.2.0rc4/rime_sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/data_format_check/cli.py` & `rime_sdk-2.2.0rc4/rime_sdk/data_format_check/cli.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/data_format_check/data_format_checker.py` & `rime_sdk-2.2.0rc4/rime_sdk/data_format_check/data_format_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/data_format_check/nlp_checker.py` & `rime_sdk-2.2.0rc4/rime_sdk/data_format_check/nlp_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/data_format_check/tabular_checker.py` & `rime_sdk-2.2.0rc4/rime_sdk/data_format_check/tabular_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/detection_event.py` & `rime_sdk-2.2.0rc4/rime_sdk/detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/firewall.py` & `rime_sdk-2.2.0rc4/rime_sdk/firewall.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,15 +379,14 @@
     ) -> pd.DataFrame:
         """Get a dataframe of Detected Events for the given Firewall.
 
         Monitors detect Events when degradations occur.
         For example, a Monitor for the metric "Accuracy" will detect an Event
         when the value of the model performance metric drops below a threshold.
         """
-        # TODO(RAT-1943): allow user to specify a time interval to query over.
         detection_api = DetectionApi(self._api_client)
         next_page_token = ""
         has_more = True
         all_events = []
         while has_more:
             kwargs: Dict[str, Any] = {}
             if len(next_page_token) > 0:
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/image_builder.py` & `rime_sdk-2.2.0rc4/rime_sdk/image_builder.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/internal/config_parser.py` & `rime_sdk-2.2.0rc4/rime_sdk/internal/config_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Parse json config to swagger."""
 import functools
 import inspect
 import json
 from copy import deepcopy
 from typing import Any, Callable, Optional, Set, Tuple, Union, cast
 
+from rime_sdk.swagger.swagger_client import RegistryGenerativeLanguageModelInfo
 from rime_sdk.swagger.swagger_client.models import (
     DataParamsFeatureIntersection,
     DataParamsRankingInfo,
     RegistryConnectionInfo,
     RegistryDatabricksInfo,
     RegistryDataCollectorInfo,
     RegistryDataFileInfo,
@@ -361,14 +362,21 @@
                     f" Expected `dict` or json `str`. Got: {type(config_d)}"
                 )
             model_info_swagger = RegistryModelInfo(
                 hugging_face=RegistryHuggingFaceModelInfo(
                     model_uri=model_uri, kwargs=config_str
                 )
             )
+        elif model_type == "generative_language_model":
+            model_info_swagger = RegistryModelInfo(
+                generative_language_model=RegistryGenerativeLanguageModelInfo(
+                    model_path=model_info.pop("model_path"),
+                    system_prompt=model_info.pop("system_prompt", ""),
+                )
+            )
         else:
             raise ValueError(
                 f"model_info type in config should be one of {valid_model_infos}. "
                 f"Got {model_type}."
             )
     except KeyError as e:
         raise ValueError(f"Invalid config: {model_config}") from e
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/internal/constants.py` & `rime_sdk-2.2.0rc4/rime_sdk/internal/constants.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/internal/decorators.py` & `rime_sdk-2.2.0rc4/rime_sdk/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/internal/file_upload.py` & `rime_sdk-2.2.0rc4/rime_sdk/internal/file_upload.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from typing import Iterator, List, Optional
 
 import requests
 from requests.adapters import HTTPAdapter
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 
-from rime_sdk.swagger.swagger_client import ApiClient, FileUploadApi
+from rime_sdk.swagger.swagger_client import (
+    ApiClient,
+    FileUploadApi,
+    FirewallConfigurationApi,
+)
 
 
 def _now_str() -> str:
     """Generate a date string for the current time."""
     return datetime.now(timezone.utc).strftime("%Y-%m-%dT%H:%M:%S%z")
 
 
@@ -25,15 +29,79 @@
 def _get_files_to_upload(dir_path: Path, upload_hidden: bool) -> Iterator[Path]:
     paths: Iterator[Path] = dir_path.rglob("*")
     if not upload_hidden:
         paths = (path for path in paths if not _is_hidden(path, dir_path))
     return paths
 
 
-class FileUploadModule:
+class FileUploadMixin:
+    """Mixin class with basic file upload utilities."""
+
+    def _upload_object(self, file_path: Path, upload_url: str) -> None:
+        """Upload the `file_path` to the location at `upload_url` via a PUT request."""
+        file_size = file_path.stat().st_size
+        with open(file_path, "rb") as f, self._get_requests_session() as session:
+            with tqdm(
+                total=file_size,
+                unit="B",
+                unit_scale=True,
+                unit_divisor=1024,
+                desc=f"Uploading {file_path}",
+            ) as t:
+                if file_size == 0:
+                    # If the file is 0 bytes, using the TQDM io wrapper does not
+                    # work, so we simply write an empty file directly.
+                    http_response = session.put(url=upload_url, data="")
+                    t.close()
+                else:
+                    wrapped_file = CallbackIOWrapper(t.update, f, "read")
+                    http_response = session.put(url=upload_url, data=wrapped_file)
+                if http_response.status_code != requests.codes.ok:
+                    raise ValueError(
+                        f"upload of '{file_path}' failed with "
+                        + f"{http_response.status_code}: {http_response.reason}"
+                    )
+
+    @staticmethod
+    def _get_requests_session() -> requests.Session:
+        """Create request session for submitting HTTPS requests with retries."""
+        session = requests.Session()
+        adapter = HTTPAdapter(max_retries=5)
+        session.mount("https://", adapter)
+        return session
+
+    @staticmethod
+    def _impose_size_constraint(size: int, upload_limit: int) -> None:
+        if (upload_limit != 0) and (size > upload_limit):
+            raise ValueError(
+                "Input is too large to be uploaded. Maximum size permitted "
+                + f"is {upload_limit / (10 ** 6)}MB. "
+                + f"Input size given is {size / (10 ** 6)}MB"
+            )
+
+    def _upload_string(self, file_contents: str, upload_url: str) -> None:
+        """Upload `file_contents` to the location at `upload_url` via a PUT request."""
+        with self._get_requests_session() as session:
+            http_response = session.put(url=upload_url, data=file_contents)
+            if http_response.status_code != requests.codes.ok:
+                raise ValueError(
+                    "upload of raw string file failed with "
+                    + f"{http_response.status_code}: {http_response.reason}"
+                )
+
+    @staticmethod
+    def _validate_file_path(file_path: Path) -> None:
+        """Validate that the local file path is valid."""
+        if not file_path.exists():
+            raise FileNotFoundError(f"path '{file_path}' does not exist")
+        if not file_path.is_file():
+            raise OSError(f"path '{file_path}' is not a file")
+
+
+class FileUploadModule(FileUploadMixin):
     """A module that implements file uploading using a FileUploadStub."""
 
     def __init__(self, api_client: ApiClient):
         """Create a FileUploadModule for the `file_upload_client`."""
         self._api_client = api_client
         self._file_upload_client = FileUploadApi(self._api_client)
 
@@ -63,22 +131,19 @@
                 When the path ``file_path`` does not exist.
             OSError
                 When ``file_path`` is not a file.
             ValueError
                 When there was an error in obtaining a blobstore location from the
                 RIME backend or in uploading ``file_path`` to RIME's blob store.
         """
-        if not file_path.exists():
-            raise FileNotFoundError(f"path '{file_path}' does not exist")
-        if not file_path.is_file():
-            raise OSError(f"path '{file_path}' is not a file")
+        self._validate_file_path(file_path)
 
         file_size = file_path.stat().st_size
-
         file_name = file_path.name
+
         if upload_path is not None:
             resp = self._file_upload_client.file_upload_get_dataset_file_upload_url(
                 file_name=file_name, upload_path=upload_path
             )
         else:
             resp = self._file_upload_client.file_upload_get_dataset_file_upload_url(
                 file_name=file_name,
@@ -165,56 +230,64 @@
 
         Args:
             upload_url: str
                 Url to the file to be deleted in the RIME blob store.
         """
         self._file_upload_client.file_upload_delete_uploaded_file_url(upload_url)
 
-    def _upload_object(self, file_path: Path, upload_url: str) -> None:
-        """Upload the `file_path` to the location at `upload_url` via a PUT request."""
-        file_size = file_path.stat().st_size
-        with open(file_path, "rb") as f, self._get_requests_session() as session:
-            with tqdm(
-                total=file_size,
-                unit="B",
-                unit_scale=True,
-                unit_divisor=1024,
-                desc=f"Uploading {file_path}",
-            ) as t:
-                if file_size == 0:
-                    # If the file is 0 bytes, using the TQDM io wrapper does not
-                    # work, so we simply write an empty file directly.
-                    http_response = session.put(url=upload_url, data="")
-                    t.close()
-                else:
-                    wrapped_file = CallbackIOWrapper(t.update, f, "read")
-                    http_response = session.put(url=upload_url, data=wrapped_file)
-                if http_response.status_code != requests.codes.ok:
-                    raise ValueError(
-                        f"upload of '{file_path}' failed with "
-                        + f"{http_response.status_code}: {http_response.reason}"
-                    )
 
-    def _get_requests_session(self) -> requests.Session:
-        """Create request session for submitting HTTPS requests with retries."""
-        session = requests.Session()
-        adapter = HTTPAdapter(max_retries=5)
-        session.mount("https://", adapter)
-        return session
+_FIREWALL_UPLOAD_SIZE_LIMIT = int(1e7)  # 10 MB
 
-    def _impose_size_constraint(self, size: int, upload_limit: int) -> None:
-        if (upload_limit != 0) and (size > upload_limit):
-            raise ValueError(
-                "Input is too large to be uploaded. Maximum size permitted "
-                + f"is {upload_limit / (10 ** 6)}MB. "
-                + f"Input size given is {size / (10 ** 6)}MB"
-            )
 
-    def _upload_string(self, file_contents: str, upload_url: str) -> None:
-        """Upload `file_contents` to the location at `upload_url` via a PUT request."""
-        with self._get_requests_session() as session:
-            http_response = session.put(url=upload_url, data=file_contents)
-            if http_response.status_code != requests.codes.ok:
-                raise ValueError(
-                    "upload of raw string file failed with "
-                    + f"{http_response.status_code}: {http_response.reason}"
-                )
+class GenerativeFirewallFileUploader(FileUploadMixin):
+    """A module that implements file uploading using the FirewallConfigurationApi."""
+
+    def __init__(self, api_client: ApiClient):
+        """Instantiate a FirewallConfigurationApi client with the `api_client`."""
+        self._configuration_client = FirewallConfigurationApi(api_client)
+
+    def upload_file(self, file_path: Path) -> str:
+        """Upload a file to make it accessible to the RIME cluster.
+
+        The uploaded file is stored in the RIME cluster in a blob store
+        using its file name.
+
+        Args:
+            file_path: Path
+                Path to the file to be uploaded to RIME's blob store.
+
+        Returns:
+            str:
+                A reference to the uploaded file's location in the blob store. This
+                reference can be used to refer to that object when writing RIME configs.
+
+        Raises:
+            FileNotFoundError
+                When the path ``file_path`` does not exist.
+            IOError
+                When ``file_path`` is not a file.
+            ValueError
+                When there was an error in obtaining a blobstore location from the
+                RIME backend or in uploading ``file_path`` to RIME's blob store.
+                When the file upload fails, the incomplete file is
+                NOT automatically deleted.
+
+        Example:
+             .. code-block:: python
+
+                uploaded_file_path = file_uploader.upload_file(file_path)
+        """
+        self._validate_file_path(file_path)
+
+        file_size = file_path.stat().st_size
+        self._impose_size_constraint(
+            file_size, upload_limit=_FIREWALL_UPLOAD_SIZE_LIMIT
+        )
+
+        file_name = file_path.name
+        response = (
+            self._configuration_client.firewall_configuration_get_file_upload_url(
+                file_name=file_name,
+            )
+        )
+        self._upload_object(file_path, response.upload_url)
+        return response.destination_url
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/internal/rest_error_handler.py` & `rime_sdk-2.2.0rc4/rime_sdk/internal/rest_error_handler.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/internal/security_config_parser.py` & `rime_sdk-2.2.0rc4/rime_sdk/internal/security_config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/internal/swagger_parser.py` & `rime_sdk-2.2.0rc4/rime_sdk/internal/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/internal/swagger_utils.py` & `rime_sdk-2.2.0rc4/rime_sdk/internal/swagger_utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/internal/test_helpers.py` & `rime_sdk-2.2.0rc4/rime_sdk/internal/test_helpers.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/internal/throttle_queue.py` & `rime_sdk-2.2.0rc4/rime_sdk/internal/throttle_queue.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/internal/utils.py` & `rime_sdk-2.2.0rc4/rime_sdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/job.py` & `rime_sdk-2.2.0rc4/rime_sdk/job.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/monitor.py` & `rime_sdk-2.2.0rc4/rime_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/project.py` & `rime_sdk-2.2.0rc4/rime_sdk/project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/registry.py` & `rime_sdk-2.2.0rc4/rime_sdk/registry.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/__init__.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from rime_sdk.swagger.swagger_client.api.config_validator_api import ConfigValidatorApi
 from rime_sdk.swagger.swagger_client.api.customer_managed_key_service_api import CustomerManagedKeyServiceApi
 from rime_sdk.swagger.swagger_client.api.data_collector_api import DataCollectorApi
 from rime_sdk.swagger.swagger_client.api.detection_api import DetectionApi
 from rime_sdk.swagger.swagger_client.api.feature_flag_api import FeatureFlagApi
 from rime_sdk.swagger.swagger_client.api.file_scanning_api import FileScanningApi
 from rime_sdk.swagger.swagger_client.api.file_upload_api import FileUploadApi
+from rime_sdk.swagger.swagger_client.api.firewall_api import FirewallApi
+from rime_sdk.swagger.swagger_client.api.firewall_configuration_api import FirewallConfigurationApi
 from rime_sdk.swagger.swagger_client.api.firewall_service_api import FirewallServiceApi
 from rime_sdk.swagger.swagger_client.api.image_registry_api import ImageRegistryApi
 from rime_sdk.swagger.swagger_client.api.integration_service_api import IntegrationServiceApi
 from rime_sdk.swagger.swagger_client.api.job_reader_api import JobReaderApi
 from rime_sdk.swagger.swagger_client.api.model_card_service_api import ModelCardServiceApi
 from rime_sdk.swagger.swagger_client.api.model_testing_api import ModelTestingApi
 from rime_sdk.swagger.swagger_client.api.monitor_service_api import MonitorServiceApi
@@ -87,14 +89,23 @@
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report import FilescanningSecurityReport
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report_import_result import FilescanningSecurityReportImportResult
 from rime_sdk.swagger.swagger_client.models.firewall_firewall import FirewallFirewall
 from rime_sdk.swagger.swagger_client.models.firewall_firewall_firewall_id_uuid_body import FirewallFirewallFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.firewall_latest_run_info import FirewallLatestRunInfo
 from rime_sdk.swagger.swagger_client.models.firewall_scheduled_ct_info import FirewallScheduledCTInfo
 from rime_sdk.swagger.swagger_client.models.firewall_test_category_severity import FirewallTestCategorySeverity
+from rime_sdk.swagger.swagger_client.models.generativefirewall_configure_firewall_response import GenerativefirewallConfigureFirewallResponse
+from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_action import GenerativefirewallFirewallAction
+from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_config import GenerativefirewallFirewallConfig
+from rime_sdk.swagger.swagger_client.models.generativefirewall_get_file_upload_url_response import GenerativefirewallGetFileUploadURLResponse
+from rime_sdk.swagger.swagger_client.models.generativefirewall_rule_output import GenerativefirewallRuleOutput
+from rime_sdk.swagger.swagger_client.models.generativefirewall_validate_request import GenerativefirewallValidateRequest
+from rime_sdk.swagger.swagger_client.models.generativefirewall_validate_response import GenerativefirewallValidateResponse
+from rime_sdk.swagger.swagger_client.models.generativefirewall_validation_result import GenerativefirewallValidationResult
+from rime_sdk.swagger.swagger_client.models.generativefirewall_validation_type import GenerativefirewallValidationType
 from rime_sdk.swagger.swagger_client.models.generativestresstests_project_id_uuid_body import GenerativestresstestsProjectIdUuidBody
 from rime_sdk.swagger.swagger_client.models.googlerpc_status import GooglerpcStatus
 from rime_sdk.swagger.swagger_client.models.heartbeat_agent_id_uuid_body import HeartbeatAgentIdUuidBody
 from rime_sdk.swagger.swagger_client.models.image_reference_reference_type import ImageReferenceReferenceType
 from rime_sdk.swagger.swagger_client.models.integration_integration_level import IntegrationIntegrationLevel
 from rime_sdk.swagger.swagger_client.models.integration_integration_schema import IntegrationIntegrationSchema
 from rime_sdk.swagger.swagger_client.models.integration_integration_type import IntegrationIntegrationType
@@ -172,14 +183,15 @@
 from rime_sdk.swagger.swagger_client.models.registry_data_collector_info import RegistryDataCollectorInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_file_info import RegistryDataFileInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_info import RegistryDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_loading_info import RegistryDataLoadingInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_params import RegistryDataParams
 from rime_sdk.swagger.swagger_client.models.registry_data_type import RegistryDataType
 from rime_sdk.swagger.swagger_client.models.registry_databricks_info import RegistryDatabricksInfo
+from rime_sdk.swagger.swagger_client.models.registry_generative_language_model_info import RegistryGenerativeLanguageModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_data_info import RegistryHuggingFaceDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_model_info import RegistryHuggingFaceModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_metadata import RegistryMetadata
 from rime_sdk.swagger.swagger_client.models.registry_model_info import RegistryModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_model_path_info import RegistryModelPathInfo
 from rime_sdk.swagger.swagger_client.models.registry_pred_info import RegistryPredInfo
 from rime_sdk.swagger.swagger_client.models.registry_prediction_params import RegistryPredictionParams
@@ -451,12 +463,14 @@
 from rime_sdk.swagger.swagger_client.models.v1betamodelcardsmodel_card_model_card_id_uuid_model_card import V1betamodelcardsmodelCardModelCardIdUuidModelCard
 from rime_sdk.swagger.swagger_client.models.v1betamonitorsmonitor_id_uuid_monitor import V1betamonitorsmonitorIdUuidMonitor
 from rime_sdk.swagger.swagger_client.models.v1firewallfirewall_firewall_id_uuid_firewall import V1firewallfirewallFirewallIdUuidFirewall
 from rime_sdk.swagger.swagger_client.models.v1notifsettingsnotification_id_uuid_notification import V1notifsettingsnotificationIdUuidNotification
 from rime_sdk.swagger.swagger_client.models.v1projectsproject_id_uuidroleusersuser_user_id_uuid_user import V1projectsprojectIdUuidroleusersuserUserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1usersuser_id_uuid_user import V1usersuserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1workspaceworkspace_workspace_id_uuid_workspace import V1workspaceworkspaceWorkspaceIdUuidWorkspace
+from rime_sdk.swagger.swagger_client.models.validate_request_input import ValidateRequestInput
+from rime_sdk.swagger.swagger_client.models.validate_request_output import ValidateRequestOutput
 from rime_sdk.swagger.swagger_client.models.validation_validate_dataset_response import ValidationValidateDatasetResponse
 from rime_sdk.swagger.swagger_client.models.validation_validate_model_response import ValidationValidateModelResponse
 from rime_sdk.swagger.swagger_client.models.validation_validate_predictions_response import ValidationValidatePredictionsResponse
 from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_users_body import WorkspaceIdUuidUsersBody
 from rime_sdk.swagger.swagger_client.models.workspace_workspace_workspace_id_uuid_body import WorkspaceWorkspaceWorkspaceIdUuidBody
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/__init__.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from rime_sdk.swagger.swagger_client.api.config_validator_api import ConfigValidatorApi
 from rime_sdk.swagger.swagger_client.api.customer_managed_key_service_api import CustomerManagedKeyServiceApi
 from rime_sdk.swagger.swagger_client.api.data_collector_api import DataCollectorApi
 from rime_sdk.swagger.swagger_client.api.detection_api import DetectionApi
 from rime_sdk.swagger.swagger_client.api.feature_flag_api import FeatureFlagApi
 from rime_sdk.swagger.swagger_client.api.file_scanning_api import FileScanningApi
 from rime_sdk.swagger.swagger_client.api.file_upload_api import FileUploadApi
+from rime_sdk.swagger.swagger_client.api.firewall_api import FirewallApi
+from rime_sdk.swagger.swagger_client.api.firewall_configuration_api import FirewallConfigurationApi
 from rime_sdk.swagger.swagger_client.api.firewall_service_api import FirewallServiceApi
 from rime_sdk.swagger.swagger_client.api.image_registry_api import ImageRegistryApi
 from rime_sdk.swagger.swagger_client.api.integration_service_api import IntegrationServiceApi
 from rime_sdk.swagger.swagger_client.api.job_reader_api import JobReaderApi
 from rime_sdk.swagger.swagger_client.api.model_card_service_api import ModelCardServiceApi
 from rime_sdk.swagger.swagger_client.api.model_testing_api import ModelTestingApi
 from rime_sdk.swagger.swagger_client.api.monitor_service_api import MonitorServiceApi
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/agent_manager_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/agent_manager_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/agents', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -204,15 +204,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/agents/deactivate/{agentId.uuid}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -299,15 +299,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/agents/{agentId.uuid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -394,15 +394,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/agents/{agentId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -499,15 +499,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/internal/agents/heartbeat/{agentId.uuid}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -604,15 +604,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/agents', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -701,15 +701,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/internal/agents/external', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -786,15 +786,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/internal/agents/register', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/config_validator_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/config_validator_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/internal/config-validator/{configType}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/customer-managed-key', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -208,15 +208,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/customer-managed-key', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -307,15 +307,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/customer-managed-key', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -394,15 +394,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/customer-managed-key/status', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/data_collector_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/data_collector_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/data-collector/datapoints/{dataStreamId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -224,15 +224,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/data-collector/predictions/{modelId.uuid}/{dataStreamId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -331,15 +331,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/data-collector/datastream/{projectId.uuid}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -438,15 +438,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/data-collector/data/{dataStreamId.uuid}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -545,15 +545,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/data-collector/predictions/{modelId.uuid}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/detection_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/detection_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/detection-events/{projectId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/feature_flag_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/feature_flag_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/internal/feature-flags/{customerName}/features/{feature}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -208,15 +208,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/internal/feature-flags/{customerName}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -311,15 +311,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/feature-flags/{customerName}/limits/{limit}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -406,15 +406,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/feature-flags/{customerName}/features', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -513,15 +513,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/internal/feature-flags/{customerName}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/file_scanning_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/file_scanning_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/file-scans', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -204,15 +204,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/file-scans', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/file_upload_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/file_upload_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/datasets/upload-url', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -204,15 +204,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/datasets/upload-url', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -312,15 +312,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/models/upload-url', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -399,15 +399,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/uploaded-file-urls', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/firewall_service_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/firewall_service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/firewall', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -204,15 +204,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/firewall/{firewallId.uuid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -299,15 +299,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/firewall/{firewallId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -394,15 +394,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/firewall/{firewallId.uuid}/url', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -501,15 +501,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/firewall/{firewall.firewallId.uuid}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/image_registry_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/image_registry_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/images', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -204,15 +204,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/images/{name}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -299,15 +299,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/images/{name}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -394,15 +394,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/images', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -493,15 +493,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/images/list', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -590,15 +590,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/internal/images/update-info', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/integration_service_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/integration_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/integrations/{integrationId.uuid}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -216,15 +216,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/integrations', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -311,15 +311,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/integrations/{integrationId.uuid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -406,15 +406,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/integrations/{integrationId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -501,15 +501,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/integrations/workspace/{workspaceId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -608,15 +608,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/integrations/{integration.id.uuid}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/job_reader_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/job_reader_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/jobs/cancel/{jobId}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -204,15 +204,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/jobs/{jobId}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -299,15 +299,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/jobs/{jobId}/project-id', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -394,15 +394,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/jobs/{jobId}/test-run-id', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -511,15 +511,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/jobs/project/{projectId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/model_card_service_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/model_card_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/modelcards', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -204,15 +204,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/modelcards/{modelCardId.uuid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -299,15 +299,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/modelcards/{modelCardId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -394,15 +394,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/modelcards/projects/{projectId}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -501,15 +501,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/modelcards/{modelCard.modelCardId.uuid}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/model_testing_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/model_testing_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/internal/logs/{jobId}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -212,15 +212,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/continuous-tests/{firewallId.uuid}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -319,15 +319,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/internal/generative-stress-tests/{projectId.uuid}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -426,15 +426,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/stress-tests/{projectId.uuid}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/monitor_service_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/monitor_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/custom-monitors/{name}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -212,15 +212,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/custom-monitors/{monitorId.uuid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -315,15 +315,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/monitors/result/{monitorId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -410,15 +410,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/custom-monitors/metrics/{firewallId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -527,15 +527,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/monitors/{firewallId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -634,15 +634,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/monitors/{monitor.id.uuid}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/notification_setting_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/notification_setting_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/notif-settings', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -204,15 +204,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/notif-settings/{id.uuid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -309,15 +309,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/notif-settings', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -416,15 +416,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/notif-settings/{notification.id.uuid}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/project_service_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/project_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/projects/{projectId.uuid}/role/users', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -216,15 +216,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/projects', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -311,15 +311,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/projects/{projectId.uuid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -406,15 +406,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/projects/{projectId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -501,15 +501,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/projects/{projectId.uuid}/url', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -596,15 +596,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/projects/{projectId.uuid}/role/workspace', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -695,15 +695,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/projects', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -798,15 +798,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/projects/{projectId.uuid}/role/users', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -901,15 +901,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/projects/{projectId.uuid}/role/users/{userId.uuid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1008,15 +1008,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/projects/{projectId.uuid}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1123,15 +1123,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/projects/{projectId.uuid}/role/users/{user.userId.uuid}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1230,15 +1230,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/projects/{projectId.uuid}/role/workspace', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/registry_service_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/registry_service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/registry/dataset/{datasetId}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -200,15 +200,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/registry/model/{modelId.uuid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -303,15 +303,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/registry/prediction/{modelId.uuid}/{datasetId}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -398,15 +398,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/registry/dataset', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -493,15 +493,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/registry/model', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -596,15 +596,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/registry/prediction/{modelId.uuid}/{datasetId}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -707,15 +707,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/registry/{projectId.uuid}/dataset', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -810,15 +810,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/registry/{projectId.uuid}/model', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -921,15 +921,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/registry/{projectId.uuid}/prediction', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1028,15 +1028,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/registry/{projectId.uuid}/dataset', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1135,15 +1135,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/registry/{projectId.uuid}/model', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1258,15 +1258,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/registry/{projectId.uuid}/model/{modelId.uuid}/dataset/{datasetId}/prediction', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/results_reader_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/results_reader_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/test-runs/{testRunId}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -212,15 +212,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/test-runs/{testRunId}/batch-result/{testType}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -319,15 +319,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/test-runs/{testRunId}/feature-result/{urlSafeFeatureId}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -422,15 +422,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/test-runs/{testRunId}/test-config/{configName}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -517,15 +517,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/test-runs/{testRunId}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -620,15 +620,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/batch-results', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -723,15 +723,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/feature-results', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -810,15 +810,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/test-runs/test-category/monitor', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -909,15 +909,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/summary-tests', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1022,15 +1022,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/test-cases', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1129,15 +1129,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/test-runs', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1216,15 +1216,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1-beta/test-runs/test-category/validation', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1323,15 +1323,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/test-runs/rename/{testRunId}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/rime_info_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/rime_info_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/rime-info', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/user_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/user_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/users/api-tokens', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -208,15 +208,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/users', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -303,15 +303,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/users/api-tokens/{id.uuid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -398,15 +398,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/users/{userId.uuid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -497,15 +497,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/users/{userId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -596,15 +596,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/users/api-tokens', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -683,15 +683,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/users/roles', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -778,15 +778,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/users', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -885,15 +885,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/users/reset-password/{userId.uuid}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -992,15 +992,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/users/{user.id.uuid}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/validation_service_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/validation_service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/validation/dataset/{jobId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -196,15 +196,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/validation/model/{jobId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -289,15 +289,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/validation/predictions/{jobId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -386,15 +386,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/validation/dataset', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -483,15 +483,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/validation/model', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -580,15 +580,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/validation/predictions', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api/workspace_service_api.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api/workspace_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/workspace/{workspaceId.uuid}/users', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -216,15 +216,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/workspace', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -311,15 +311,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/workspace/{workspaceId.uuid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -406,15 +406,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/workspace/{workspaceId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -501,15 +501,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/workspace/{workspaceId.uuid}/tags/project', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -604,15 +604,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/workspace/{workspaceId.uuid}/users', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -699,15 +699,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/workspace', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -802,15 +802,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/workspace/{workspaceId.uuid}/users/{userId.uuid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -917,15 +917,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/workspace/{workspaceId.uuid}/users/{user.userId.uuid}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -1024,15 +1024,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
+        auth_settings = ['X-Firewall-Api-Key', 'rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
             '/v1/workspace/{workspace.workspaceId.uuid}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/api_client.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/configuration.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,14 +225,21 @@
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         return {
+            'X-Firewall-Api-Key':
+                {
+                    'type': 'api_key',
+                    'in': 'header',
+                    'key': 'X-Firewall-Api-Key',
+                    'value': self.get_api_key_with_prefix('X-Firewall-Api-Key')
+                },
             'rime-api-key':
                 {
                     'type': 'api_key',
                     'in': 'header',
                     'key': 'rime-api-key',
                     'value': self.get_api_key_with_prefix('rime-api-key')
                 },
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/__init__.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,23 @@
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report import FilescanningSecurityReport
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report_import_result import FilescanningSecurityReportImportResult
 from rime_sdk.swagger.swagger_client.models.firewall_firewall import FirewallFirewall
 from rime_sdk.swagger.swagger_client.models.firewall_firewall_firewall_id_uuid_body import FirewallFirewallFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.firewall_latest_run_info import FirewallLatestRunInfo
 from rime_sdk.swagger.swagger_client.models.firewall_scheduled_ct_info import FirewallScheduledCTInfo
 from rime_sdk.swagger.swagger_client.models.firewall_test_category_severity import FirewallTestCategorySeverity
+from rime_sdk.swagger.swagger_client.models.generativefirewall_configure_firewall_response import GenerativefirewallConfigureFirewallResponse
+from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_action import GenerativefirewallFirewallAction
+from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_config import GenerativefirewallFirewallConfig
+from rime_sdk.swagger.swagger_client.models.generativefirewall_get_file_upload_url_response import GenerativefirewallGetFileUploadURLResponse
+from rime_sdk.swagger.swagger_client.models.generativefirewall_rule_output import GenerativefirewallRuleOutput
+from rime_sdk.swagger.swagger_client.models.generativefirewall_validate_request import GenerativefirewallValidateRequest
+from rime_sdk.swagger.swagger_client.models.generativefirewall_validate_response import GenerativefirewallValidateResponse
+from rime_sdk.swagger.swagger_client.models.generativefirewall_validation_result import GenerativefirewallValidationResult
+from rime_sdk.swagger.swagger_client.models.generativefirewall_validation_type import GenerativefirewallValidationType
 from rime_sdk.swagger.swagger_client.models.generativestresstests_project_id_uuid_body import GenerativestresstestsProjectIdUuidBody
 from rime_sdk.swagger.swagger_client.models.googlerpc_status import GooglerpcStatus
 from rime_sdk.swagger.swagger_client.models.heartbeat_agent_id_uuid_body import HeartbeatAgentIdUuidBody
 from rime_sdk.swagger.swagger_client.models.image_reference_reference_type import ImageReferenceReferenceType
 from rime_sdk.swagger.swagger_client.models.integration_integration_level import IntegrationIntegrationLevel
 from rime_sdk.swagger.swagger_client.models.integration_integration_schema import IntegrationIntegrationSchema
 from rime_sdk.swagger.swagger_client.models.integration_integration_type import IntegrationIntegrationType
@@ -144,14 +153,15 @@
 from rime_sdk.swagger.swagger_client.models.registry_data_collector_info import RegistryDataCollectorInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_file_info import RegistryDataFileInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_info import RegistryDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_loading_info import RegistryDataLoadingInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_params import RegistryDataParams
 from rime_sdk.swagger.swagger_client.models.registry_data_type import RegistryDataType
 from rime_sdk.swagger.swagger_client.models.registry_databricks_info import RegistryDatabricksInfo
+from rime_sdk.swagger.swagger_client.models.registry_generative_language_model_info import RegistryGenerativeLanguageModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_data_info import RegistryHuggingFaceDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_model_info import RegistryHuggingFaceModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_metadata import RegistryMetadata
 from rime_sdk.swagger.swagger_client.models.registry_model_info import RegistryModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_model_path_info import RegistryModelPathInfo
 from rime_sdk.swagger.swagger_client.models.registry_pred_info import RegistryPredInfo
 from rime_sdk.swagger.swagger_client.models.registry_prediction_params import RegistryPredictionParams
@@ -423,12 +433,14 @@
 from rime_sdk.swagger.swagger_client.models.v1betamodelcardsmodel_card_model_card_id_uuid_model_card import V1betamodelcardsmodelCardModelCardIdUuidModelCard
 from rime_sdk.swagger.swagger_client.models.v1betamonitorsmonitor_id_uuid_monitor import V1betamonitorsmonitorIdUuidMonitor
 from rime_sdk.swagger.swagger_client.models.v1firewallfirewall_firewall_id_uuid_firewall import V1firewallfirewallFirewallIdUuidFirewall
 from rime_sdk.swagger.swagger_client.models.v1notifsettingsnotification_id_uuid_notification import V1notifsettingsnotificationIdUuidNotification
 from rime_sdk.swagger.swagger_client.models.v1projectsproject_id_uuidroleusersuser_user_id_uuid_user import V1projectsprojectIdUuidroleusersuserUserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1usersuser_id_uuid_user import V1usersuserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1workspaceworkspace_workspace_id_uuid_workspace import V1workspaceworkspaceWorkspaceIdUuidWorkspace
+from rime_sdk.swagger.swagger_client.models.validate_request_input import ValidateRequestInput
+from rime_sdk.swagger.swagger_client.models.validate_request_output import ValidateRequestOutput
 from rime_sdk.swagger.swagger_client.models.validation_validate_dataset_response import ValidationValidateDatasetResponse
 from rime_sdk.swagger.swagger_client.models.validation_validate_model_response import ValidationValidateModelResponse
 from rime_sdk.swagger.swagger_client.models.validation_validate_predictions_response import ValidationValidatePredictionsResponse
 from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_users_body import WorkspaceIdUuidUsersBody
 from rime_sdk.swagger.swagger_client.models.workspace_workspace_workspace_id_uuid_body import WorkspaceWorkspaceWorkspaceIdUuidBody
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_dataset.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/dataset_dataset.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_detection_event.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/detection_detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_detail.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/detection_event_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/detection_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_resolution.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/detection_resolution.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/firewall_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/googlerpc_status.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_level.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/integration_integration_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/model_model.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/model_model.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_threshold.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitor_transform.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitor_transform.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_digest_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notification_digest_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notification_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notification_notification_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_object_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notification_object_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_create_project_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_create_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_get_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_owner_details.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_project.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_project_with_details.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_project_with_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_update_project_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_update_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_any.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_connection_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_connection_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,33 +26,38 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'path': 'str',
         'load_func_name': 'str',
-        'loader_kwargs_json': 'str'
+        'loader_kwargs_json': 'str',
+        'data_endpoint_integration_id': 'RimeUUID'
     }
 
     attribute_map = {
         'path': 'path',
         'load_func_name': 'loadFuncName',
-        'loader_kwargs_json': 'loaderKwargsJson'
+        'loader_kwargs_json': 'loaderKwargsJson',
+        'data_endpoint_integration_id': 'dataEndpointIntegrationId'
     }
 
-    def __init__(self, path=None, load_func_name=None, loader_kwargs_json=None):  # noqa: E501
+    def __init__(self, path=None, load_func_name=None, loader_kwargs_json=None, data_endpoint_integration_id=None):  # noqa: E501
         """RegistryDataLoadingInfo - a model defined in Swagger"""  # noqa: E501
         self._path = None
         self._load_func_name = None
         self._loader_kwargs_json = None
+        self._data_endpoint_integration_id = None
         self.discriminator = None
         self.path = path
         self.load_func_name = load_func_name
         if loader_kwargs_json is not None:
             self.loader_kwargs_json = loader_kwargs_json
+        if data_endpoint_integration_id is not None:
+            self.data_endpoint_integration_id = data_endpoint_integration_id
 
     @property
     def path(self):
         """Gets the path of this RegistryDataLoadingInfo.  # noqa: E501
 
         The path to the python file containing the data loading function.  # noqa: E501
 
@@ -119,14 +124,35 @@
 
         :param loader_kwargs_json: The loader_kwargs_json of this RegistryDataLoadingInfo.  # noqa: E501
         :type: str
         """
 
         self._loader_kwargs_json = loader_kwargs_json
 
+    @property
+    def data_endpoint_integration_id(self):
+        """Gets the data_endpoint_integration_id of this RegistryDataLoadingInfo.  # noqa: E501
+
+
+        :return: The data_endpoint_integration_id of this RegistryDataLoadingInfo.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._data_endpoint_integration_id
+
+    @data_endpoint_integration_id.setter
+    def data_endpoint_integration_id(self, data_endpoint_integration_id):
+        """Sets the data_endpoint_integration_id of this RegistryDataLoadingInfo.
+
+
+        :param data_endpoint_integration_id: The data_endpoint_integration_id of this RegistryDataLoadingInfo.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._data_endpoint_integration_id = data_endpoint_integration_id
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_params.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_data_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_metadata.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,87 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RegistryModelInfo(object):
+class RimeListImagesResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'model_path': 'RegistryModelPathInfo',
-        'hugging_face': 'RegistryHuggingFaceModelInfo'
+        'images': 'list[RimeManagedImage]',
+        'next_page_token': 'str'
     }
 
     attribute_map = {
-        'model_path': 'modelPath',
-        'hugging_face': 'huggingFace'
+        'images': 'images',
+        'next_page_token': 'nextPageToken'
     }
 
-    def __init__(self, model_path=None, hugging_face=None):  # noqa: E501
-        """RegistryModelInfo - a model defined in Swagger"""  # noqa: E501
-        self._model_path = None
-        self._hugging_face = None
+    def __init__(self, images=None, next_page_token=None):  # noqa: E501
+        """RimeListImagesResponse - a model defined in Swagger"""  # noqa: E501
+        self._images = None
+        self._next_page_token = None
         self.discriminator = None
-        if model_path is not None:
-            self.model_path = model_path
-        if hugging_face is not None:
-            self.hugging_face = hugging_face
+        if images is not None:
+            self.images = images
+        if next_page_token is not None:
+            self.next_page_token = next_page_token
 
     @property
-    def model_path(self):
-        """Gets the model_path of this RegistryModelInfo.  # noqa: E501
+    def images(self):
+        """Gets the images of this RimeListImagesResponse.  # noqa: E501
 
 
-        :return: The model_path of this RegistryModelInfo.  # noqa: E501
-        :rtype: RegistryModelPathInfo
+        :return: The images of this RimeListImagesResponse.  # noqa: E501
+        :rtype: list[RimeManagedImage]
         """
-        return self._model_path
+        return self._images
 
-    @model_path.setter
-    def model_path(self, model_path):
-        """Sets the model_path of this RegistryModelInfo.
+    @images.setter
+    def images(self, images):
+        """Sets the images of this RimeListImagesResponse.
 
 
-        :param model_path: The model_path of this RegistryModelInfo.  # noqa: E501
-        :type: RegistryModelPathInfo
+        :param images: The images of this RimeListImagesResponse.  # noqa: E501
+        :type: list[RimeManagedImage]
         """
 
-        self._model_path = model_path
+        self._images = images
 
     @property
-    def hugging_face(self):
-        """Gets the hugging_face of this RegistryModelInfo.  # noqa: E501
+    def next_page_token(self):
+        """Gets the next_page_token of this RimeListImagesResponse.  # noqa: E501
 
 
-        :return: The hugging_face of this RegistryModelInfo.  # noqa: E501
-        :rtype: RegistryHuggingFaceModelInfo
+        :return: The next_page_token of this RimeListImagesResponse.  # noqa: E501
+        :rtype: str
         """
-        return self._hugging_face
+        return self._next_page_token
 
-    @hugging_face.setter
-    def hugging_face(self, hugging_face):
-        """Sets the hugging_face of this RegistryModelInfo.
+    @next_page_token.setter
+    def next_page_token(self, next_page_token):
+        """Sets the next_page_token of this RimeListImagesResponse.
 
 
-        :param hugging_face: The hugging_face of this RegistryModelInfo.  # noqa: E501
-        :type: RegistryHuggingFaceModelInfo
+        :param next_page_token: The next_page_token of this RimeListImagesResponse.  # noqa: E501
+        :type: str
         """
 
-        self._hugging_face = hugging_face
+        self._next_page_token = next_page_token
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RegistryModelInfo, dict):
+        if issubclass(RimeListImagesResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RegistryModelInfo):
+        if not isinstance(other, RimeListImagesResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_pred_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_pred_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registry_validity_status.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registry_validity_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_actor_role.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_actor_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_agent.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent_status.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_agent_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_metric.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_category_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_config_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_config_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_row.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_failing_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_feature_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_float_list.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_float_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_image_reference.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_image_reference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_int_list.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_int_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_integration_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_integration_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_data.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_data.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_view.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_job_view.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_language.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_language.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_feature.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_license_feature.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_limit.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_license_limit.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_limit_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,87 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListImagesResponse(object):
+class RuntimeinfoCustomImage(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'images': 'list[RimeManagedImage]',
-        'next_page_token': 'str'
+        'name': 'str',
+        'pull_secret': 'CustomImagePullSecret'
     }
 
     attribute_map = {
-        'images': 'images',
-        'next_page_token': 'nextPageToken'
+        'name': 'name',
+        'pull_secret': 'pullSecret'
     }
 
-    def __init__(self, images=None, next_page_token=None):  # noqa: E501
-        """RimeListImagesResponse - a model defined in Swagger"""  # noqa: E501
-        self._images = None
-        self._next_page_token = None
+    def __init__(self, name=None, pull_secret=None):  # noqa: E501
+        """RuntimeinfoCustomImage - a model defined in Swagger"""  # noqa: E501
+        self._name = None
+        self._pull_secret = None
         self.discriminator = None
-        if images is not None:
-            self.images = images
-        if next_page_token is not None:
-            self.next_page_token = next_page_token
+        if name is not None:
+            self.name = name
+        if pull_secret is not None:
+            self.pull_secret = pull_secret
 
     @property
-    def images(self):
-        """Gets the images of this RimeListImagesResponse.  # noqa: E501
+    def name(self):
+        """Gets the name of this RuntimeinfoCustomImage.  # noqa: E501
 
+        Name of the custom image (e.g. a docker image name).  # noqa: E501
 
-        :return: The images of this RimeListImagesResponse.  # noqa: E501
-        :rtype: list[RimeManagedImage]
+        :return: The name of this RuntimeinfoCustomImage.  # noqa: E501
+        :rtype: str
         """
-        return self._images
+        return self._name
 
-    @images.setter
-    def images(self, images):
-        """Sets the images of this RimeListImagesResponse.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this RuntimeinfoCustomImage.
 
+        Name of the custom image (e.g. a docker image name).  # noqa: E501
 
-        :param images: The images of this RimeListImagesResponse.  # noqa: E501
-        :type: list[RimeManagedImage]
+        :param name: The name of this RuntimeinfoCustomImage.  # noqa: E501
+        :type: str
         """
 
-        self._images = images
+        self._name = name
 
     @property
-    def next_page_token(self):
-        """Gets the next_page_token of this RimeListImagesResponse.  # noqa: E501
+    def pull_secret(self):
+        """Gets the pull_secret of this RuntimeinfoCustomImage.  # noqa: E501
 
 
-        :return: The next_page_token of this RimeListImagesResponse.  # noqa: E501
-        :rtype: str
+        :return: The pull_secret of this RuntimeinfoCustomImage.  # noqa: E501
+        :rtype: CustomImagePullSecret
         """
-        return self._next_page_token
+        return self._pull_secret
 
-    @next_page_token.setter
-    def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this RimeListImagesResponse.
+    @pull_secret.setter
+    def pull_secret(self, pull_secret):
+        """Sets the pull_secret of this RuntimeinfoCustomImage.
 
 
-        :param next_page_token: The next_page_token of this RimeListImagesResponse.  # noqa: E501
-        :type: str
+        :param pull_secret: The pull_secret of this RuntimeinfoCustomImage.  # noqa: E501
+        :type: CustomImagePullSecret
         """
 
-        self._next_page_token = next_page_token
+        self._pull_secret = pull_secret
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListImagesResponse, dict):
+        if issubclass(RuntimeinfoCustomImage, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListImagesResponse):
+        if not isinstance(other, RuntimeinfoCustomImage):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_managed_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_card.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_task.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_task.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_named_double.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_named_double.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_order.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_order.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_safe_url.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_safe_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_str_list.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_str_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_subject_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_subject_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_suggestion.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_suggestion.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_table_column.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_test_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_time_interval.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_time_interval.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_token_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_token_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_role.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_uuid.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_uuid.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/role_users_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/role_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/role_workspace_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/role_workspace_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,89 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RuntimeinfoCustomImage(object):
+class RuntimeinfoCustomImageType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'name': 'str',
-        'pull_secret': 'CustomImagePullSecret'
+        'custom_image': 'RuntimeinfoCustomImage',
+        'managed_image_name': 'str'
     }
 
     attribute_map = {
-        'name': 'name',
-        'pull_secret': 'pullSecret'
+        'custom_image': 'customImage',
+        'managed_image_name': 'managedImageName'
     }
 
-    def __init__(self, name=None, pull_secret=None):  # noqa: E501
-        """RuntimeinfoCustomImage - a model defined in Swagger"""  # noqa: E501
-        self._name = None
-        self._pull_secret = None
+    def __init__(self, custom_image=None, managed_image_name=None):  # noqa: E501
+        """RuntimeinfoCustomImageType - a model defined in Swagger"""  # noqa: E501
+        self._custom_image = None
+        self._managed_image_name = None
         self.discriminator = None
-        if name is not None:
-            self.name = name
-        if pull_secret is not None:
-            self.pull_secret = pull_secret
+        if custom_image is not None:
+            self.custom_image = custom_image
+        if managed_image_name is not None:
+            self.managed_image_name = managed_image_name
 
     @property
-    def name(self):
-        """Gets the name of this RuntimeinfoCustomImage.  # noqa: E501
+    def custom_image(self):
+        """Gets the custom_image of this RuntimeinfoCustomImageType.  # noqa: E501
 
-        Name of the custom image (e.g. a docker image name).  # noqa: E501
 
-        :return: The name of this RuntimeinfoCustomImage.  # noqa: E501
-        :rtype: str
+        :return: The custom_image of this RuntimeinfoCustomImageType.  # noqa: E501
+        :rtype: RuntimeinfoCustomImage
         """
-        return self._name
+        return self._custom_image
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this RuntimeinfoCustomImage.
+    @custom_image.setter
+    def custom_image(self, custom_image):
+        """Sets the custom_image of this RuntimeinfoCustomImageType.
 
-        Name of the custom image (e.g. a docker image name).  # noqa: E501
 
-        :param name: The name of this RuntimeinfoCustomImage.  # noqa: E501
-        :type: str
+        :param custom_image: The custom_image of this RuntimeinfoCustomImageType.  # noqa: E501
+        :type: RuntimeinfoCustomImage
         """
 
-        self._name = name
+        self._custom_image = custom_image
 
     @property
-    def pull_secret(self):
-        """Gets the pull_secret of this RuntimeinfoCustomImage.  # noqa: E501
+    def managed_image_name(self):
+        """Gets the managed_image_name of this RuntimeinfoCustomImageType.  # noqa: E501
 
+        Name of the RI managed image.  # noqa: E501
 
-        :return: The pull_secret of this RuntimeinfoCustomImage.  # noqa: E501
-        :rtype: CustomImagePullSecret
+        :return: The managed_image_name of this RuntimeinfoCustomImageType.  # noqa: E501
+        :rtype: str
         """
-        return self._pull_secret
+        return self._managed_image_name
 
-    @pull_secret.setter
-    def pull_secret(self, pull_secret):
-        """Sets the pull_secret of this RuntimeinfoCustomImage.
+    @managed_image_name.setter
+    def managed_image_name(self, managed_image_name):
+        """Sets the managed_image_name of this RuntimeinfoCustomImageType.
 
+        Name of the RI managed image.  # noqa: E501
 
-        :param pull_secret: The pull_secret of this RuntimeinfoCustomImage.  # noqa: E501
-        :type: CustomImagePullSecret
+        :param managed_image_name: The managed_image_name of this RuntimeinfoCustomImageType.  # noqa: E501
+        :type: str
         """
 
-        self._pull_secret = pull_secret
+        self._managed_image_name = managed_image_name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -108,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RuntimeinfoCustomImage, dict):
+        if issubclass(RuntimeinfoCustomImageType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RuntimeinfoCustomImage):
+        if not isinstance(other, RuntimeinfoCustomImageType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/schemanotification_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/schemanotification_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/statedb_job_status.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/statedb_job_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_private_info.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/user_private_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_role.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/user_user_detail.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/user_user_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/swagger/swagger_client/rest.py` & `rime_sdk-2.2.0rc4/rime_sdk/swagger/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/test_batch.py` & `rime_sdk-2.2.0rc4/rime_sdk/test_batch.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk/test_run.py` & `rime_sdk-2.2.0rc4/rime_sdk/test_run.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.2.0rc3/rime_sdk.egg-info/PKG-INFO` & `rime_sdk-2.2.0rc4/rime_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime-sdk
-Version: 2.2.0rc3
+Version: 2.2.0rc4
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.2.0rc3/rime_sdk.egg-info/SOURCES.txt` & `rime_sdk-2.2.0rc4/rime_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 rime_sdk/__init__.py
 rime_sdk/client.py
 rime_sdk/data_collector.py
 rime_sdk/detection_event.py
 rime_sdk/firewall.py
+rime_sdk/generative_firewall.py
 rime_sdk/image_builder.py
 rime_sdk/job.py
 rime_sdk/monitor.py
 rime_sdk/project.py
 rime_sdk/registry.py
 rime_sdk/test_batch.py
 rime_sdk/test_run.py
@@ -46,14 +47,16 @@
 rime_sdk/swagger/swagger_client/api/config_validator_api.py
 rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
 rime_sdk/swagger/swagger_client/api/data_collector_api.py
 rime_sdk/swagger/swagger_client/api/detection_api.py
 rime_sdk/swagger/swagger_client/api/feature_flag_api.py
 rime_sdk/swagger/swagger_client/api/file_scanning_api.py
 rime_sdk/swagger/swagger_client/api/file_upload_api.py
+rime_sdk/swagger/swagger_client/api/firewall_api.py
+rime_sdk/swagger/swagger_client/api/firewall_configuration_api.py
 rime_sdk/swagger/swagger_client/api/firewall_service_api.py
 rime_sdk/swagger/swagger_client/api/image_registry_api.py
 rime_sdk/swagger/swagger_client/api/integration_service_api.py
 rime_sdk/swagger/swagger_client/api/job_reader_api.py
 rime_sdk/swagger/swagger_client/api/model_card_service_api.py
 rime_sdk/swagger/swagger_client/api/model_testing_api.py
 rime_sdk/swagger/swagger_client/api/monitor_service_api.py
@@ -111,14 +114,23 @@
 rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
 rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
 rime_sdk/swagger/swagger_client/models/firewall_firewall.py
 rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
 rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
 rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+rime_sdk/swagger/swagger_client/models/generativefirewall_configure_firewall_response.py
+rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py
+rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_config.py
+rime_sdk/swagger/swagger_client/models/generativefirewall_get_file_upload_url_response.py
+rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py
+rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py
+rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py
+rime_sdk/swagger/swagger_client/models/generativefirewall_validation_result.py
+rime_sdk/swagger/swagger_client/models/generativefirewall_validation_type.py
 rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/googlerpc_status.py
 rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
 rime_sdk/swagger/swagger_client/models/integration_integration_level.py
 rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
 rime_sdk/swagger/swagger_client/models/integration_integration_type.py
@@ -196,14 +208,15 @@
 rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_params.py
 rime_sdk/swagger/swagger_client/models/registry_data_type.py
 rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
+rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py
 rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
 rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
 rime_sdk/swagger/swagger_client/models/registry_metadata.py
 rime_sdk/swagger/swagger_client/models/registry_model_info.py
 rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
 rime_sdk/swagger/swagger_client/models/registry_pred_info.py
 rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
@@ -475,12 +488,14 @@
 rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
 rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
 rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
 rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
 rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
 rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
 rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+rime_sdk/swagger/swagger_client/models/validate_request_input.py
+rime_sdk/swagger/swagger_client/models/validate_request_output.py
 rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
 rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
 rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
 rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
 rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
```

### Comparing `rime_sdk-2.2.0rc3/setup.py` & `rime_sdk-2.2.0rc4/setup.py`

 * *Files identical despite different names*

