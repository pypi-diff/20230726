# Comparing `tmp/rockset-2.0.0.tar.gz` & `tmp/rockset-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockset-2.0.0.tar", max compression
+gzip compressed data, was "rockset-2.0.2.tar", max compression
```

## Comparing `rockset-2.0.0.tar` & `rockset-2.0.2.tar`

### file list

```diff
@@ -1,237 +1,245 @@
--rw-r--r--   0        0        0      357 2022-12-13 01:58:51.206007 rockset-2.0.0/LONG_DESCRIPTION.rst
--rw-r--r--   0        0        0     1615 2023-05-17 23:59:17.562975 rockset-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1338 2022-12-13 01:58:51.321191 rockset-2.0.0/rockset/__init__.py
--rw-r--r--   0        0        0      208 2022-12-13 01:58:42.690343 rockset-2.0.0/rockset/api/__init__.py
--rw-r--r--   0        0        0    34696 2022-12-13 01:58:51.322358 rockset-2.0.0/rockset/api/aliases_api.py
--rw-r--r--   0        0        0    29724 2022-12-13 01:58:51.323252 rockset-2.0.0/rockset/api/api_keys_api.py
--rw-r--r--   0        0        0   130795 2022-12-13 01:58:51.324989 rockset-2.0.0/rockset/api/collections_api.py
--rw-r--r--   0        0        0    28165 2022-12-13 01:58:42.693877 rockset-2.0.0/rockset/api/custom_roles_api.py
--rw-r--r--   0        0        0    21187 2022-12-13 01:58:51.325994 rockset-2.0.0/rockset/api/documents_api.py
--rw-r--r--   0        0        0    73682 2022-12-13 01:58:51.327346 rockset-2.0.0/rockset/api/integrations_api.py
--rw-r--r--   0        0        0     6168 2022-12-13 01:58:42.696525 rockset-2.0.0/rockset/api/organizations_api.py
--rw-r--r--   0        0        0    34734 2023-05-12 17:22:20.907117 rockset-2.0.0/rockset/api/queries_api.py
--rw-r--r--   0        0        0    87549 2022-12-13 01:58:51.329493 rockset-2.0.0/rockset/api/query_lambdas_api.py
--rw-r--r--   0        0        0     7727 2023-05-12 17:22:20.910399 rockset-2.0.0/rockset/api/shared_lambdas_api.py
--rw-r--r--   0        0        0    43268 2023-05-12 17:22:20.918078 rockset-2.0.0/rockset/api/users_api.py
--rw-r--r--   0        0        0    34441 2022-12-13 01:58:51.332337 rockset-2.0.0/rockset/api/views_api.py
--rw-r--r--   0        0        0    76220 2023-05-12 17:22:20.924296 rockset-2.0.0/rockset/api/virtual_instances_api.py
--rw-r--r--   0        0        0    22087 2022-12-13 01:58:51.335148 rockset-2.0.0/rockset/api/workspaces_api.py
--rw-r--r--   0        0        0    36245 2022-12-13 01:58:51.336141 rockset-2.0.0/rockset/api_client.py
--rw-r--r--   0        0        0     1112 2022-12-13 01:58:51.337188 rockset-2.0.0/rockset/apis/__init__.py
--rw-r--r--   0        0        0    15516 2022-12-13 01:58:51.338079 rockset-2.0.0/rockset/configuration.py
--rw-r--r--   0        0        0     3831 2022-12-13 01:58:42.708412 rockset-2.0.0/rockset/document.py
--rw-r--r--   0        0        0     6072 2022-12-13 01:58:51.338930 rockset-2.0.0/rockset/exceptions.py
--rw-r--r--   0        0        0      348 2022-12-13 01:58:42.709463 rockset-2.0.0/rockset/model/__init__.py
--rw-r--r--   0        0        0    11950 2022-12-13 01:58:51.340059 rockset-2.0.0/rockset/model/add_documents_request.py
--rw-r--r--   0        0        0    11922 2022-12-13 01:58:51.341043 rockset-2.0.0/rockset/model/add_documents_response.py
--rw-r--r--   0        0        0    13623 2022-12-13 01:58:51.342438 rockset-2.0.0/rockset/model/alias.py
--rw-r--r--   0        0        0    13945 2022-12-13 01:58:51.343654 rockset-2.0.0/rockset/model/api_key.py
--rw-r--r--   0        0        0    13542 2022-12-13 01:58:51.344826 rockset-2.0.0/rockset/model/async_query_options.py
--rw-r--r--   0        0        0    12229 2022-12-13 01:58:51.346082 rockset-2.0.0/rockset/model/aws_access_key.py
--rw-r--r--   0        0        0    12101 2022-12-13 01:58:51.347099 rockset-2.0.0/rockset/model/aws_role.py
--rw-r--r--   0        0        0    15124 2022-12-13 01:58:51.347977 rockset-2.0.0/rockset/model/azure_blob_storage_collection_creation_request.py
--rw-r--r--   0        0        0    11893 2022-12-13 01:58:51.348793 rockset-2.0.0/rockset/model/azure_blob_storage_integration.py
--rw-r--r--   0        0        0    12616 2022-12-13 01:58:51.349789 rockset-2.0.0/rockset/model/azure_blob_storage_integration_creation_request.py
--rw-r--r--   0        0        0    14449 2022-12-13 01:58:51.350910 rockset-2.0.0/rockset/model/azure_blob_storage_source_wrapper.py
--rw-r--r--   0        0        0    15104 2022-12-13 01:58:51.355455 rockset-2.0.0/rockset/model/azure_event_hubs_collection_creation_request.py
--rw-r--r--   0        0        0    11787 2022-12-13 01:58:51.356462 rockset-2.0.0/rockset/model/azure_event_hubs_integration.py
--rw-r--r--   0        0        0    12586 2022-12-13 01:58:51.357448 rockset-2.0.0/rockset/model/azure_event_hubs_integration_creation_request.py
--rw-r--r--   0        0        0    13452 2022-12-13 01:58:51.358672 rockset-2.0.0/rockset/model/azure_event_hubs_source_wrapper.py
--rw-r--r--   0        0        0    15114 2022-12-13 01:58:51.359647 rockset-2.0.0/rockset/model/azure_service_bus_collection_creation_request.py
--rw-r--r--   0        0        0    11888 2022-12-13 01:58:51.361464 rockset-2.0.0/rockset/model/azure_service_bus_integration.py
--rw-r--r--   0        0        0    13333 2022-12-13 01:58:51.363034 rockset-2.0.0/rockset/model/azure_service_bus_source_wrapper.py
--rw-r--r--   0        0        0    18743 2023-05-12 17:22:20.928164 rockset-2.0.0/rockset/model/bulk_stats.py
--rw-r--r--   0        0        0    11798 2022-12-13 01:58:51.364718 rockset-2.0.0/rockset/model/cancel_query_response.py
--rw-r--r--   0        0        0    13225 2022-12-13 01:58:51.365908 rockset-2.0.0/rockset/model/cluster.py
--rw-r--r--   0        0        0    17684 2022-12-13 01:58:51.367440 rockset-2.0.0/rockset/model/collection.py
--rw-r--r--   0        0        0    14579 2023-05-12 17:22:20.935169 rockset-2.0.0/rockset/model/collection_mount.py
--rw-r--r--   0        0        0    11852 2022-12-13 01:58:51.369480 rockset-2.0.0/rockset/model/collection_mount_response.py
--rw-r--r--   0        0        0    11772 2023-05-12 17:22:20.942953 rockset-2.0.0/rockset/model/collection_mount_stats.py
--rw-r--r--   0        0        0    16965 2022-12-13 01:58:51.370768 rockset-2.0.0/rockset/model/collection_stats.py
--rw-r--r--   0        0        0    12333 2022-12-13 01:58:51.371874 rockset-2.0.0/rockset/model/create_alias_request.py
--rw-r--r--   0        0        0    11769 2022-12-13 01:58:51.373053 rockset-2.0.0/rockset/model/create_alias_response.py
--rw-r--r--   0        0        0    12098 2022-12-13 01:58:51.373927 rockset-2.0.0/rockset/model/create_api_key_request.py
--rw-r--r--   0        0        0    11780 2022-12-13 01:58:51.374901 rockset-2.0.0/rockset/model/create_api_key_response.py
--rw-r--r--   0        0        0    12071 2022-12-13 01:58:51.375498 rockset-2.0.0/rockset/model/create_collection_mount_request.py
--rw-r--r--   0        0        0    11913 2023-05-12 17:22:20.945604 rockset-2.0.0/rockset/model/create_collection_mounts_response.py
--rw-r--r--   0        0        0    14506 2022-12-13 01:58:51.376828 rockset-2.0.0/rockset/model/create_collection_request.py
--rw-r--r--   0        0        0    11819 2022-12-13 01:58:51.377747 rockset-2.0.0/rockset/model/create_collection_response.py
--rw-r--r--   0        0        0    16037 2022-12-13 01:58:51.378736 rockset-2.0.0/rockset/model/create_integration_request.py
--rw-r--r--   0        0        0    11829 2022-12-13 01:58:51.379675 rockset-2.0.0/rockset/model/create_integration_response.py
--rw-r--r--   0        0        0    12571 2022-12-13 01:58:51.381735 rockset-2.0.0/rockset/model/create_query_lambda_request.py
--rw-r--r--   0        0        0    12063 2022-12-13 01:58:51.382700 rockset-2.0.0/rockset/model/create_query_lambda_tag_request.py
--rw-r--r--   0        0        0    12501 2022-12-13 01:58:51.383928 rockset-2.0.0/rockset/model/create_role_request.py
--rw-r--r--   0        0        0    12479 2023-05-12 17:22:20.953879 rockset-2.0.0/rockset/model/create_user_request.py
--rw-r--r--   0        0        0    11759 2022-12-13 01:58:51.387934 rockset-2.0.0/rockset/model/create_user_response.py
--rw-r--r--   0        0        0    12170 2022-12-13 01:58:51.388848 rockset-2.0.0/rockset/model/create_view_request.py
--rw-r--r--   0        0        0    11759 2022-12-13 01:58:51.389749 rockset-2.0.0/rockset/model/create_view_response.py
--rw-r--r--   0        0        0    13224 2022-12-13 01:58:51.390403 rockset-2.0.0/rockset/model/create_virtual_instance_request.py
--rw-r--r--   0        0        0    11870 2022-12-13 01:58:51.391137 rockset-2.0.0/rockset/model/create_virtual_instance_response.py
--rw-r--r--   0        0        0    12038 2022-12-13 01:58:51.391990 rockset-2.0.0/rockset/model/create_workspace_request.py
--rw-r--r--   0        0        0    11809 2022-12-13 01:58:51.392971 rockset-2.0.0/rockset/model/create_workspace_response.py
--rw-r--r--   0        0        0    14179 2022-12-13 01:58:51.394177 rockset-2.0.0/rockset/model/csv_params.py
--rw-r--r--   0        0        0    11769 2022-12-13 01:58:51.395065 rockset-2.0.0/rockset/model/delete_alias_response.py
--rw-r--r--   0        0        0    11780 2022-12-13 01:58:51.395871 rockset-2.0.0/rockset/model/delete_api_key_response.py
--rw-r--r--   0        0        0    11819 2022-12-13 01:58:51.397342 rockset-2.0.0/rockset/model/delete_collection_response.py
--rw-r--r--   0        0        0    12036 2022-12-13 01:58:51.398103 rockset-2.0.0/rockset/model/delete_documents_request.py
--rw-r--r--   0        0        0    11686 2022-12-13 01:58:51.398891 rockset-2.0.0/rockset/model/delete_documents_request_data.py
--rw-r--r--   0        0        0    11927 2022-12-13 01:58:51.399594 rockset-2.0.0/rockset/model/delete_documents_response.py
--rw-r--r--   0        0        0    11829 2022-12-13 01:58:51.400868 rockset-2.0.0/rockset/model/delete_integration_response.py
--rw-r--r--   0        0        0    11830 2022-12-13 01:58:51.401717 rockset-2.0.0/rockset/model/delete_query_lambda_response.py
--rw-r--r--   0        0        0    11759 2022-12-13 01:58:51.405750 rockset-2.0.0/rockset/model/delete_user_response.py
--rw-r--r--   0        0        0    11759 2022-12-13 01:58:51.406881 rockset-2.0.0/rockset/model/delete_view_response.py
--rw-r--r--   0        0        0    11870 2022-12-13 01:58:51.407738 rockset-2.0.0/rockset/model/delete_virtual_instance_response.py
--rw-r--r--   0        0        0    11809 2022-12-13 01:58:51.408605 rockset-2.0.0/rockset/model/delete_workspace_response.py
--rw-r--r--   0        0        0    13023 2022-12-13 01:58:51.409506 rockset-2.0.0/rockset/model/document_status.py
--rw-r--r--   0        0        0    15042 2022-12-13 01:58:51.410273 rockset-2.0.0/rockset/model/dynamodb_collection_creation_request.py
--rw-r--r--   0        0        0    12563 2022-12-13 01:58:51.411173 rockset-2.0.0/rockset/model/dynamodb_integration.py
--rw-r--r--   0        0        0    12484 2022-12-13 01:58:51.411877 rockset-2.0.0/rockset/model/dynamodb_integration_creation_request.py
--rw-r--r--   0        0        0    14440 2022-12-13 01:58:51.412536 rockset-2.0.0/rockset/model/dynamodb_source_wrapper.py
--rw-r--r--   0        0        0    14520 2023-05-12 17:22:20.957148 rockset-2.0.0/rockset/model/error_model.py
--rw-r--r--   0        0        0    12392 2022-12-13 01:58:51.414156 rockset-2.0.0/rockset/model/event_time_info.py
--rw-r--r--   0        0        0    12656 2023-05-12 17:22:20.961849 rockset-2.0.0/rockset/model/execute_public_query_lambda_request.py
--rw-r--r--   0        0        0    14367 2022-12-13 01:58:51.414854 rockset-2.0.0/rockset/model/execute_query_lambda_request.py
--rw-r--r--   0        0        0    11743 2022-12-13 01:58:51.415485 rockset-2.0.0/rockset/model/field_mapping_query.py
--rw-r--r--   0        0        0    13075 2022-12-13 01:58:51.416534 rockset-2.0.0/rockset/model/field_mapping_v2.py
--rw-r--r--   0        0        0    12543 2022-12-13 01:58:51.417789 rockset-2.0.0/rockset/model/field_partition.py
--rw-r--r--   0        0        0    15063 2022-12-13 01:58:51.418937 rockset-2.0.0/rockset/model/file_upload_collection_creation_request.py
--rw-r--r--   0        0        0    13611 2022-12-13 01:58:51.419752 rockset-2.0.0/rockset/model/file_upload_source_wrapper.py
--rw-r--r--   0        0        0    13202 2022-12-13 01:58:51.420839 rockset-2.0.0/rockset/model/format_params.py
--rw-r--r--   0        0        0    12001 2022-12-13 01:58:51.421612 rockset-2.0.0/rockset/model/gcp_service_account.py
--rw-r--r--   0        0        0    14992 2022-12-13 01:58:51.422369 rockset-2.0.0/rockset/model/gcs_collection_creation_request.py
--rw-r--r--   0        0        0    11915 2022-12-13 01:58:51.423092 rockset-2.0.0/rockset/model/gcs_integration.py
--rw-r--r--   0        0        0    12409 2022-12-13 01:58:51.423760 rockset-2.0.0/rockset/model/gcs_integration_creation_request.py
--rw-r--r--   0        0        0    14666 2022-12-13 01:58:51.424461 rockset-2.0.0/rockset/model/gcs_source_wrapper.py
--rw-r--r--   0        0        0    11760 2022-12-13 01:58:51.425075 rockset-2.0.0/rockset/model/get_alias_response.py
--rw-r--r--   0        0        0    11771 2022-12-13 01:58:51.425773 rockset-2.0.0/rockset/model/get_api_key_response.py
--rw-r--r--   0        0        0    11810 2022-12-13 01:58:51.426421 rockset-2.0.0/rockset/model/get_collection_response.py
--rw-r--r--   0        0        0    11820 2022-12-13 01:58:51.427289 rockset-2.0.0/rockset/model/get_integration_response.py
--rw-r--r--   0        0        0    11789 2022-12-13 01:58:51.428017 rockset-2.0.0/rockset/model/get_query_response.py
--rw-r--r--   0        0        0    11750 2022-12-13 01:58:51.428894 rockset-2.0.0/rockset/model/get_view_response.py
--rw-r--r--   0        0        0    11861 2022-12-13 01:58:51.429731 rockset-2.0.0/rockset/model/get_virtual_instance_response.py
--rw-r--r--   0        0        0    11800 2022-12-13 01:58:51.430619 rockset-2.0.0/rockset/model/get_workspace_response.py
--rw-r--r--   0        0        0    12704 2022-12-13 01:58:51.431409 rockset-2.0.0/rockset/model/input_field.py
--rw-r--r--   0        0        0    17362 2022-12-13 01:58:51.432299 rockset-2.0.0/rockset/model/integration.py
--rw-r--r--   0        0        0    15012 2022-12-13 01:58:51.433257 rockset-2.0.0/rockset/model/kafka_collection_creation_request.py
--rw-r--r--   0        0        0    14826 2022-12-13 01:58:51.433924 rockset-2.0.0/rockset/model/kafka_integration.py
--rw-r--r--   0        0        0    12439 2022-12-13 01:58:51.434725 rockset-2.0.0/rockset/model/kafka_integration_creation_request.py
--rw-r--r--   0        0        0    14027 2022-12-13 01:58:51.435418 rockset-2.0.0/rockset/model/kafka_source_wrapper.py
--rw-r--r--   0        0        0    11845 2022-12-13 01:58:51.436134 rockset-2.0.0/rockset/model/kafka_v3_security_config.py
--rw-r--r--   0        0        0    15032 2022-12-13 01:58:51.436744 rockset-2.0.0/rockset/model/kinesis_collection_creation_request.py
--rw-r--r--   0        0        0    12169 2022-12-13 01:58:51.438159 rockset-2.0.0/rockset/model/kinesis_integration.py
--rw-r--r--   0        0        0    12469 2022-12-13 01:58:51.438947 rockset-2.0.0/rockset/model/kinesis_integration_creation_request.py
--rw-r--r--   0        0        0    14265 2022-12-13 01:58:51.439735 rockset-2.0.0/rockset/model/kinesis_source_wrapper.py
--rw-r--r--   0        0        0    11819 2022-12-13 01:58:51.440610 rockset-2.0.0/rockset/model/list_aliases_response.py
--rw-r--r--   0        0        0    11835 2022-12-13 01:58:51.441850 rockset-2.0.0/rockset/model/list_api_keys_response.py
--rw-r--r--   0        0        0    11937 2022-12-13 01:58:51.442402 rockset-2.0.0/rockset/model/list_collection_mounts_response.py
--rw-r--r--   0        0        0    11874 2022-12-13 01:58:51.443359 rockset-2.0.0/rockset/model/list_collections_response.py
--rw-r--r--   0        0        0    11892 2022-12-13 01:58:51.444428 rockset-2.0.0/rockset/model/list_integrations_response.py
--rw-r--r--   0        0        0    11804 2022-12-13 01:58:51.445389 rockset-2.0.0/rockset/model/list_queries_response.py
--rw-r--r--   0        0        0    11964 2022-12-13 01:58:51.446199 rockset-2.0.0/rockset/model/list_query_lambda_tags_response.py
--rw-r--r--   0        0        0    12010 2022-12-13 01:58:51.447037 rockset-2.0.0/rockset/model/list_query_lambda_versions_response.py
--rw-r--r--   0        0        0    11889 2022-12-13 01:58:51.448465 rockset-2.0.0/rockset/model/list_query_lambdas_response.py
--rw-r--r--   0        0        0    11802 2022-12-13 01:58:51.449343 rockset-2.0.0/rockset/model/list_roles_response.py
--rw-r--r--   0        0        0    12003 2022-12-13 01:58:51.450548 rockset-2.0.0/rockset/model/list_unsubscribe_preferences_response.py
--rw-r--r--   0        0        0    11794 2022-12-13 01:58:51.451885 rockset-2.0.0/rockset/model/list_users_response.py
--rw-r--r--   0        0        0    11802 2022-12-13 01:58:51.455878 rockset-2.0.0/rockset/model/list_views_response.py
--rw-r--r--   0        0        0    11937 2022-12-13 01:58:51.456878 rockset-2.0.0/rockset/model/list_virtual_instances_response.py
--rw-r--r--   0        0        0    11854 2022-12-13 01:58:51.457814 rockset-2.0.0/rockset/model/list_workspaces_response.py
--rw-r--r--   0        0        0    11815 2022-12-13 01:58:51.458840 rockset-2.0.0/rockset/model/mongo_db_integration.py
--rw-r--r--   0        0        0    15032 2022-12-13 01:58:51.459596 rockset-2.0.0/rockset/model/mongodb_collection_creation_request.py
--rw-r--r--   0        0        0    12470 2022-12-13 01:58:51.460283 rockset-2.0.0/rockset/model/mongodb_integration_creation_request.py
--rw-r--r--   0        0        0    13434 2022-12-13 01:58:51.460926 rockset-2.0.0/rockset/model/mongodb_source_wrapper.py
--rw-r--r--   0        0        0    13277 2022-12-13 01:58:51.461621 rockset-2.0.0/rockset/model/organization.py
--rw-r--r--   0        0        0    11821 2022-12-13 01:58:51.462439 rockset-2.0.0/rockset/model/organization_response.py
--rw-r--r--   0        0        0    12527 2022-12-13 01:58:51.463085 rockset-2.0.0/rockset/model/output_field.py
--rw-r--r--   0        0        0    11775 2022-12-13 01:58:51.463873 rockset-2.0.0/rockset/model/pagination.py
--rw-r--r--   0        0        0    13055 2022-12-13 01:58:51.464710 rockset-2.0.0/rockset/model/pagination_info.py
--rw-r--r--   0        0        0    12155 2022-12-13 01:58:51.465583 rockset-2.0.0/rockset/model/patch_document.py
--rw-r--r--   0        0        0    11920 2022-12-13 01:58:51.466714 rockset-2.0.0/rockset/model/patch_documents_request.py
--rw-r--r--   0        0        0    11868 2022-12-13 01:58:51.468318 rockset-2.0.0/rockset/model/patch_documents_response.py
--rw-r--r--   0        0        0    13672 2022-12-13 01:58:51.469338 rockset-2.0.0/rockset/model/patch_operation.py
--rw-r--r--   0        0        0    15362 2023-05-12 17:22:20.967106 rockset-2.0.0/rockset/model/privilege.py
--rw-r--r--   0        0        0    12407 2022-12-13 01:58:51.471138 rockset-2.0.0/rockset/model/query_error.py
--rw-r--r--   0        0        0    11907 2022-12-13 01:58:51.472036 rockset-2.0.0/rockset/model/query_field_type.py
--rw-r--r--   0        0        0    14725 2022-12-13 01:58:51.472774 rockset-2.0.0/rockset/model/query_info.py
--rw-r--r--   0        0        0    13688 2022-12-13 01:58:51.473624 rockset-2.0.0/rockset/model/query_lambda.py
--rw-r--r--   0        0        0    12219 2022-12-13 01:58:51.474716 rockset-2.0.0/rockset/model/query_lambda_sql.py
--rw-r--r--   0        0        0    12786 2022-12-13 01:58:51.475873 rockset-2.0.0/rockset/model/query_lambda_stats.py
--rw-r--r--   0        0        0    12124 2022-12-13 01:58:51.477013 rockset-2.0.0/rockset/model/query_lambda_tag.py
--rw-r--r--   0        0        0    11843 2022-12-13 01:58:51.477906 rockset-2.0.0/rockset/model/query_lambda_tag_response.py
--rw-r--r--   0        0        0    14841 2022-12-13 01:58:51.478799 rockset-2.0.0/rockset/model/query_lambda_version.py
--rw-r--r--   0        0        0    11883 2022-12-13 01:58:51.479680 rockset-2.0.0/rockset/model/query_lambda_version_response.py
--rw-r--r--   0        0        0    13051 2023-05-18 17:55:09.709562 rockset-2.0.0/rockset/model/query_pagination_response.py
--rw-r--r--   0        0        0    12164 2022-12-13 01:58:51.481278 rockset-2.0.0/rockset/model/query_parameter.py
--rw-r--r--   0        0        0    12227 2022-12-13 01:58:51.481934 rockset-2.0.0/rockset/model/query_request.py
--rw-r--r--   0        0        0    14009 2023-05-12 17:22:20.984866 rockset-2.0.0/rockset/model/query_request_sql.py
--rw-r--r--   0        0        0    16189 2023-05-17 23:55:16.173168 rockset-2.0.0/rockset/model/query_response.py
--rw-r--r--   0        0        0    12105 2022-12-13 01:58:51.483887 rockset-2.0.0/rockset/model/query_response_stats.py
--rw-r--r--   0        0        0    11870 2022-12-13 01:58:51.484388 rockset-2.0.0/rockset/model/resume_virtual_instance_response.py
--rw-r--r--   0        0        0    13363 2022-12-13 01:58:51.485738 rockset-2.0.0/rockset/model/role.py
--rw-r--r--   0        0        0    11741 2022-12-13 01:58:51.487202 rockset-2.0.0/rockset/model/role_response.py
--rw-r--r--   0        0        0    14982 2022-12-13 01:58:51.488257 rockset-2.0.0/rockset/model/s3_collection_creation_request.py
--rw-r--r--   0        0        0    12154 2022-12-13 01:58:51.489532 rockset-2.0.0/rockset/model/s3_integration.py
--rw-r--r--   0        0        0    12394 2022-12-13 01:58:51.491627 rockset-2.0.0/rockset/model/s3_integration_creation_request.py
--rw-r--r--   0        0        0    15239 2022-12-13 01:58:51.492470 rockset-2.0.0/rockset/model/s3_source_wrapper.py
--rw-r--r--   0        0        0    12201 2022-12-13 01:58:51.493440 rockset-2.0.0/rockset/model/schema_registry_config.py
--rw-r--r--   0        0        0    11696 2022-12-13 01:58:51.494236 rockset-2.0.0/rockset/model/segment_integration.py
--rw-r--r--   0        0        0    12465 2022-12-13 01:58:51.495198 rockset-2.0.0/rockset/model/segment_integration_creation_request.py
--rw-r--r--   0        0        0    15052 2022-12-13 01:58:51.495692 rockset-2.0.0/rockset/model/snowflake_collection_creation_request.py
--rw-r--r--   0        0        0    14450 2022-12-13 01:58:51.496199 rockset-2.0.0/rockset/model/snowflake_integration.py
--rw-r--r--   0        0        0    12499 2022-12-13 01:58:51.496726 rockset-2.0.0/rockset/model/snowflake_integration_creation_request.py
--rw-r--r--   0        0        0    13907 2022-12-13 01:58:51.497226 rockset-2.0.0/rockset/model/snowflake_source_wrapper.py
--rw-r--r--   0        0        0    12501 2022-12-13 01:58:51.498002 rockset-2.0.0/rockset/model/source.py
--rw-r--r--   0        0        0    13169 2022-12-13 01:58:51.498911 rockset-2.0.0/rockset/model/source_azure_blob_storage.py
--rw-r--r--   0        0        0    12664 2022-12-13 01:58:51.499899 rockset-2.0.0/rockset/model/source_azure_event_hubs.py
--rw-r--r--   0        0        0    12552 2022-12-13 01:58:51.500742 rockset-2.0.0/rockset/model/source_azure_service_bus.py
--rw-r--r--   0        0        0    13624 2022-12-13 01:58:51.502104 rockset-2.0.0/rockset/model/source_dynamo_db.py
--rw-r--r--   0        0        0    12391 2022-12-13 01:58:51.506381 rockset-2.0.0/rockset/model/source_file_upload.py
--rw-r--r--   0        0        0    13371 2022-12-13 01:58:51.507531 rockset-2.0.0/rockset/model/source_gcs.py
--rw-r--r--   0        0        0    13209 2022-12-13 01:58:51.509226 rockset-2.0.0/rockset/model/source_kafka.py
--rw-r--r--   0        0        0    13024 2022-12-13 01:58:51.510021 rockset-2.0.0/rockset/model/source_kinesis.py
--rw-r--r--   0        0        0    12652 2022-12-13 01:58:51.510772 rockset-2.0.0/rockset/model/source_mongo_db.py
--rw-r--r--   0        0        0    13923 2022-12-13 01:58:51.511460 rockset-2.0.0/rockset/model/source_s3.py
--rw-r--r--   0        0        0    13110 2022-12-13 01:58:51.511957 rockset-2.0.0/rockset/model/source_snowflake.py
--rw-r--r--   0        0        0    11661 2022-12-13 01:58:51.512868 rockset-2.0.0/rockset/model/sql_expression.py
--rw-r--r--   0        0        0    13116 2022-12-13 01:58:51.513635 rockset-2.0.0/rockset/model/stats.py
--rw-r--r--   0        0        0    13658 2023-05-12 17:22:21.008906 rockset-2.0.0/rockset/model/status.py
--rw-r--r--   0        0        0    13111 2022-12-13 01:58:51.515374 rockset-2.0.0/rockset/model/status_azure_event_hubs.py
--rw-r--r--   0        0        0    12364 2022-12-13 01:58:51.516105 rockset-2.0.0/rockset/model/status_azure_event_hubs_partition.py
--rw-r--r--   0        0        0    12727 2022-12-13 01:58:51.516913 rockset-2.0.0/rockset/model/status_azure_service_bus.py
--rw-r--r--   0        0        0    12210 2022-12-13 01:58:51.517709 rockset-2.0.0/rockset/model/status_azure_service_bus_session.py
--rw-r--r--   0        0        0    13563 2022-12-13 01:58:51.518336 rockset-2.0.0/rockset/model/status_dynamo_db.py
--rw-r--r--   0        0        0    12705 2022-12-13 01:58:51.519331 rockset-2.0.0/rockset/model/status_dynamo_db_v2.py
--rw-r--r--   0        0        0    13123 2022-12-13 01:58:51.520073 rockset-2.0.0/rockset/model/status_kafka.py
--rw-r--r--   0        0        0    12337 2022-12-13 01:58:51.520751 rockset-2.0.0/rockset/model/status_kafka_partition.py
--rw-r--r--   0        0        0    15614 2022-12-13 01:58:51.521466 rockset-2.0.0/rockset/model/status_mongo_db.py
--rw-r--r--   0        0        0    11924 2022-12-13 01:58:51.521971 rockset-2.0.0/rockset/model/status_snowflake.py
--rw-r--r--   0        0        0    11873 2022-12-13 01:58:51.522386 rockset-2.0.0/rockset/model/suspend_virtual_instance_response.py
--rw-r--r--   0        0        0    11894 2022-12-13 01:58:51.523204 rockset-2.0.0/rockset/model/unsubscribe_preference.py
--rw-r--r--   0        0        0    12119 2022-12-13 01:58:51.523819 rockset-2.0.0/rockset/model/update_alias_request.py
--rw-r--r--   0        0        0    11818 2022-12-13 01:58:51.524650 rockset-2.0.0/rockset/model/update_api_key_request.py
--rw-r--r--   0        0        0    11780 2022-12-13 01:58:51.525248 rockset-2.0.0/rockset/model/update_api_key_response.py
--rw-r--r--   0        0        0    11867 2022-12-13 01:58:51.525826 rockset-2.0.0/rockset/model/update_integration_request.py
--rw-r--r--   0        0        0    11829 2022-12-13 01:58:51.526397 rockset-2.0.0/rockset/model/update_integration_response.py
--rw-r--r--   0        0        0    12329 2022-12-13 01:58:51.526916 rockset-2.0.0/rockset/model/update_query_lambda_request.py
--rw-r--r--   0        0        0    12222 2022-12-13 01:58:51.527531 rockset-2.0.0/rockset/model/update_role_request.py
--rw-r--r--   0        0        0    12006 2022-12-13 01:58:51.528227 rockset-2.0.0/rockset/model/update_unsubscribe_preferences_request.py
--rw-r--r--   0        0        0    12009 2022-12-13 01:58:51.528766 rockset-2.0.0/rockset/model/update_unsubscribe_preferences_response.py
--rw-r--r--   0        0        0    12206 2022-12-13 01:58:51.529107 rockset-2.0.0/rockset/model/update_user_request.py
--rw-r--r--   0        0        0    11958 2022-12-13 01:58:51.529732 rockset-2.0.0/rockset/model/update_view_request.py
--rw-r--r--   0        0        0    11759 2022-12-13 01:58:51.530315 rockset-2.0.0/rockset/model/update_view_response.py
--rw-r--r--   0        0        0    13762 2022-12-13 01:58:51.531030 rockset-2.0.0/rockset/model/update_virtual_instance_request.py
--rw-r--r--   0        0        0    11870 2022-12-13 01:58:51.531710 rockset-2.0.0/rockset/model/update_virtual_instance_response.py
--rw-r--r--   0        0        0    12907 2022-12-13 01:58:51.532928 rockset-2.0.0/rockset/model/user.py
--rw-r--r--   0        0        0    12155 2022-12-13 01:58:51.533563 rockset-2.0.0/rockset/model/validate_query_response.py
--rw-r--r--   0        0        0    14473 2022-12-13 01:58:51.534222 rockset-2.0.0/rockset/model/view.py
--rw-r--r--   0        0        0    17180 2022-12-13 01:58:51.535531 rockset-2.0.0/rockset/model/virtual_instance.py
--rw-r--r--   0        0        0    11772 2022-12-13 01:58:51.536198 rockset-2.0.0/rockset/model/virtual_instance_stats.py
--rw-r--r--   0        0        0    12971 2022-12-13 01:58:51.537165 rockset-2.0.0/rockset/model/workspace.py
--rw-r--r--   0        0        0    12998 2022-12-13 01:58:51.537919 rockset-2.0.0/rockset/model/xml_params.py
--rw-r--r--   0        0        0    84037 2022-12-13 01:58:51.539401 rockset-2.0.0/rockset/model_utils.py
--rw-r--r--   0        0        0    14505 2023-05-12 17:22:21.013772 rockset-2.0.0/rockset/models/__init__.py
--rw-r--r--   0        0        0     1819 2022-12-13 01:58:42.845037 rockset-2.0.0/rockset/query_paginator.py
--rw-r--r--   0        0        0    14645 2022-12-13 01:58:51.541699 rockset-2.0.0/rockset/rest.py
--rw-r--r--   0        0        0     8491 2022-12-13 01:58:51.542775 rockset-2.0.0/rockset/rockset_client.py
--rw-r--r--   0        0        0     3644 2022-12-13 01:58:42.847883 rockset-2.0.0/rockset/value.py
--rw-r--r--   0        0        0     2369 1970-01-01 00:00:00.000000 rockset-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      357 2023-07-26 00:43:43.282647 rockset-2.0.2/LONG_DESCRIPTION.rst
+-rw-r--r--   0        0        0     1616 2023-07-26 01:10:25.867240 rockset-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1338 2023-07-26 01:02:17.339333 rockset-2.0.2/rockset/__init__.py
+-rw-r--r--   0        0        0      208 2023-07-26 01:02:17.339333 rockset-2.0.2/rockset/api/__init__.py
+-rw-r--r--   0        0        0    34696 2023-07-26 01:02:17.459334 rockset-2.0.2/rockset/api/aliases_api.py
+-rw-r--r--   0        0        0    29724 2023-07-26 01:02:17.451334 rockset-2.0.2/rockset/api/api_keys_api.py
+-rw-r--r--   0        0        0   110990 2023-07-26 01:02:17.455334 rockset-2.0.2/rockset/api/collections_api.py
+-rw-r--r--   0        0        0    28165 2023-07-26 01:02:17.451334 rockset-2.0.2/rockset/api/custom_roles_api.py
+-rw-r--r--   0        0        0    21187 2023-07-26 01:02:17.451334 rockset-2.0.2/rockset/api/documents_api.py
+-rw-r--r--   0        0        0    73682 2023-07-26 01:02:17.451334 rockset-2.0.2/rockset/api/integrations_api.py
+-rw-r--r--   0        0        0     6168 2023-07-26 01:02:17.451334 rockset-2.0.2/rockset/api/organizations_api.py
+-rw-r--r--   0        0        0    38326 2023-07-26 01:02:17.459334 rockset-2.0.2/rockset/api/queries_api.py
+-rw-r--r--   0        0        0    87833 2023-07-26 01:02:17.455334 rockset-2.0.2/rockset/api/query_lambdas_api.py
+-rw-r--r--   0        0        0     7727 2023-07-26 01:02:17.451334 rockset-2.0.2/rockset/api/shared_lambdas_api.py
+-rw-r--r--   0        0        0   101734 2023-07-26 01:02:17.459334 rockset-2.0.2/rockset/api/sources_api.py
+-rw-r--r--   0        0        0    43268 2023-07-26 01:02:17.451334 rockset-2.0.2/rockset/api/users_api.py
+-rw-r--r--   0        0        0    34441 2023-07-26 01:02:17.451334 rockset-2.0.2/rockset/api/views_api.py
+-rw-r--r--   0        0        0    79266 2023-07-26 01:02:17.455334 rockset-2.0.2/rockset/api/virtual_instances_api.py
+-rw-r--r--   0        0        0    22087 2023-07-26 01:02:17.459334 rockset-2.0.2/rockset/api/workspaces_api.py
+-rw-r--r--   0        0        0    36245 2023-07-26 01:02:17.343333 rockset-2.0.2/rockset/api_client.py
+-rw-r--r--   0        0        0     1156 2023-07-26 01:02:17.359333 rockset-2.0.2/rockset/apis/__init__.py
+-rw-r--r--   0        0        0    15516 2023-07-26 01:02:17.339333 rockset-2.0.2/rockset/configuration.py
+-rw-r--r--   0        0        0     3831 2023-07-26 00:43:43.302647 rockset-2.0.2/rockset/document.py
+-rw-r--r--   0        0        0     6072 2023-07-26 01:02:17.343333 rockset-2.0.2/rockset/exceptions.py
+-rw-r--r--   0        0        0      348 2023-07-26 01:02:17.355333 rockset-2.0.2/rockset/model/__init__.py
+-rw-r--r--   0        0        0    11950 2023-07-26 01:02:14.907314 rockset-2.0.2/rockset/model/add_documents_request.py
+-rw-r--r--   0        0        0    11922 2023-07-26 01:02:14.931314 rockset-2.0.2/rockset/model/add_documents_response.py
+-rw-r--r--   0        0        0    14049 2023-07-26 01:02:14.955314 rockset-2.0.2/rockset/model/alias.py
+-rw-r--r--   0        0        0    14557 2023-07-26 01:02:14.975314 rockset-2.0.2/rockset/model/api_key.py
+-rw-r--r--   0        0        0    14462 2023-07-26 01:02:14.987315 rockset-2.0.2/rockset/model/async_query_options.py
+-rw-r--r--   0        0        0    13732 2023-07-26 01:02:15.007315 rockset-2.0.2/rockset/model/auto_scaling_policy.py
+-rw-r--r--   0        0        0    12229 2023-07-26 01:02:15.023315 rockset-2.0.2/rockset/model/aws_access_key.py
+-rw-r--r--   0        0        0    12101 2023-07-26 01:02:15.095315 rockset-2.0.2/rockset/model/aws_role.py
+-rw-r--r--   0        0        0    15072 2023-07-26 01:02:15.131316 rockset-2.0.2/rockset/model/azure_blob_storage_collection_creation_request.py
+-rw-r--r--   0        0        0    11893 2023-07-26 01:02:15.147316 rockset-2.0.2/rockset/model/azure_blob_storage_integration.py
+-rw-r--r--   0        0        0    12616 2023-07-26 01:02:15.159316 rockset-2.0.2/rockset/model/azure_blob_storage_integration_creation_request.py
+-rw-r--r--   0        0        0    14079 2023-07-26 01:02:15.187316 rockset-2.0.2/rockset/model/azure_blob_storage_source_wrapper.py
+-rw-r--r--   0        0        0    15052 2023-07-26 01:02:15.203316 rockset-2.0.2/rockset/model/azure_event_hubs_collection_creation_request.py
+-rw-r--r--   0        0        0    11787 2023-07-26 01:02:15.223316 rockset-2.0.2/rockset/model/azure_event_hubs_integration.py
+-rw-r--r--   0        0        0    12586 2023-07-26 01:02:15.239317 rockset-2.0.2/rockset/model/azure_event_hubs_integration_creation_request.py
+-rw-r--r--   0        0        0    13452 2023-07-26 01:02:15.251317 rockset-2.0.2/rockset/model/azure_event_hubs_source_wrapper.py
+-rw-r--r--   0        0        0    15062 2023-07-26 00:43:43.302647 rockset-2.0.2/rockset/model/azure_service_bus_collection_creation_request.py
+-rw-r--r--   0        0        0    11888 2023-07-26 01:02:15.267317 rockset-2.0.2/rockset/model/azure_service_bus_integration.py
+-rw-r--r--   0        0        0    13333 2023-07-26 00:43:43.302647 rockset-2.0.2/rockset/model/azure_service_bus_source_wrapper.py
+-rw-r--r--   0        0        0    18743 2023-07-26 01:02:15.291317 rockset-2.0.2/rockset/model/bulk_stats.py
+-rw-r--r--   0        0        0    11798 2023-07-26 01:02:15.303317 rockset-2.0.2/rockset/model/cancel_query_response.py
+-rw-r--r--   0        0        0    13225 2023-07-26 01:02:15.315317 rockset-2.0.2/rockset/model/cluster.py
+-rw-r--r--   0        0        0    18118 2023-07-26 01:02:15.331317 rockset-2.0.2/rockset/model/collection.py
+-rw-r--r--   0        0        0    14847 2023-07-26 01:02:15.339317 rockset-2.0.2/rockset/model/collection_mount.py
+-rw-r--r--   0        0        0    11852 2023-07-26 01:02:15.359317 rockset-2.0.2/rockset/model/collection_mount_response.py
+-rw-r--r--   0        0        0    11772 2023-07-26 01:02:15.395318 rockset-2.0.2/rockset/model/collection_mount_stats.py
+-rw-r--r--   0        0        0    16965 2023-07-26 01:02:15.403318 rockset-2.0.2/rockset/model/collection_stats.py
+-rw-r--r--   0        0        0    12333 2023-07-26 01:02:15.411318 rockset-2.0.2/rockset/model/create_alias_request.py
+-rw-r--r--   0        0        0    11769 2023-07-26 01:02:15.419318 rockset-2.0.2/rockset/model/create_alias_response.py
+-rw-r--r--   0        0        0    12098 2023-07-26 01:02:15.427318 rockset-2.0.2/rockset/model/create_api_key_request.py
+-rw-r--r--   0        0        0    11780 2023-07-26 01:02:15.435318 rockset-2.0.2/rockset/model/create_api_key_response.py
+-rw-r--r--   0        0        0    11765 2023-07-26 01:02:15.439318 rockset-2.0.2/rockset/model/create_collection_mount_request.py
+-rw-r--r--   0        0        0    11913 2023-07-26 01:02:15.447318 rockset-2.0.2/rockset/model/create_collection_mounts_response.py
+-rw-r--r--   0        0        0    14454 2023-07-26 01:02:15.459318 rockset-2.0.2/rockset/model/create_collection_request.py
+-rw-r--r--   0        0        0    11819 2023-07-26 01:02:15.467318 rockset-2.0.2/rockset/model/create_collection_response.py
+-rw-r--r--   0        0        0    16037 2023-07-26 01:02:15.491318 rockset-2.0.2/rockset/model/create_integration_request.py
+-rw-r--r--   0        0        0    11829 2023-07-26 01:02:15.503319 rockset-2.0.2/rockset/model/create_integration_response.py
+-rw-r--r--   0        0        0    12571 2023-07-26 01:02:15.507319 rockset-2.0.2/rockset/model/create_query_lambda_request.py
+-rw-r--r--   0        0        0    12063 2023-07-26 01:02:15.519319 rockset-2.0.2/rockset/model/create_query_lambda_tag_request.py
+-rw-r--r--   0        0        0    12501 2023-07-26 01:02:15.527319 rockset-2.0.2/rockset/model/create_role_request.py
+-rw-r--r--   0        0        0    12479 2023-07-26 01:02:15.531319 rockset-2.0.2/rockset/model/create_user_request.py
+-rw-r--r--   0        0        0    11759 2023-07-26 01:02:15.539319 rockset-2.0.2/rockset/model/create_user_response.py
+-rw-r--r--   0        0        0    12170 2023-07-26 01:02:15.547319 rockset-2.0.2/rockset/model/create_view_request.py
+-rw-r--r--   0        0        0    11759 2023-07-26 01:02:15.555319 rockset-2.0.2/rockset/model/create_view_response.py
+-rw-r--r--   0        0        0    14405 2023-07-26 01:02:15.563319 rockset-2.0.2/rockset/model/create_virtual_instance_request.py
+-rw-r--r--   0        0        0    11870 2023-07-26 01:02:15.579319 rockset-2.0.2/rockset/model/create_virtual_instance_response.py
+-rw-r--r--   0        0        0    12038 2023-07-26 01:02:15.595319 rockset-2.0.2/rockset/model/create_workspace_request.py
+-rw-r--r--   0        0        0    11809 2023-07-26 01:02:15.607319 rockset-2.0.2/rockset/model/create_workspace_response.py
+-rw-r--r--   0        0        0    14179 2023-07-26 01:02:15.623319 rockset-2.0.2/rockset/model/csv_params.py
+-rw-r--r--   0        0        0    11769 2023-07-26 01:02:15.635320 rockset-2.0.2/rockset/model/delete_alias_response.py
+-rw-r--r--   0        0        0    11780 2023-07-26 01:02:15.651320 rockset-2.0.2/rockset/model/delete_api_key_response.py
+-rw-r--r--   0        0        0    11819 2023-07-26 01:02:15.663320 rockset-2.0.2/rockset/model/delete_collection_response.py
+-rw-r--r--   0        0        0    12036 2023-07-26 01:02:15.679320 rockset-2.0.2/rockset/model/delete_documents_request.py
+-rw-r--r--   0        0        0    11686 2023-07-26 01:02:15.695320 rockset-2.0.2/rockset/model/delete_documents_request_data.py
+-rw-r--r--   0        0        0    11927 2023-07-26 01:02:15.711320 rockset-2.0.2/rockset/model/delete_documents_response.py
+-rw-r--r--   0        0        0    11829 2023-07-26 01:02:15.723320 rockset-2.0.2/rockset/model/delete_integration_response.py
+-rw-r--r--   0        0        0    11830 2023-07-26 01:02:15.735320 rockset-2.0.2/rockset/model/delete_query_lambda_response.py
+-rw-r--r--   0        0        0    11779 2023-07-26 01:02:15.763321 rockset-2.0.2/rockset/model/delete_source_response.py
+-rw-r--r--   0        0        0    11759 2023-07-26 01:02:15.775321 rockset-2.0.2/rockset/model/delete_user_response.py
+-rw-r--r--   0        0        0    11759 2023-07-26 01:02:15.791321 rockset-2.0.2/rockset/model/delete_view_response.py
+-rw-r--r--   0        0        0    11870 2023-07-26 01:02:15.807321 rockset-2.0.2/rockset/model/delete_virtual_instance_response.py
+-rw-r--r--   0        0        0    11809 2023-07-26 01:02:15.815321 rockset-2.0.2/rockset/model/delete_workspace_response.py
+-rw-r--r--   0        0        0    13023 2023-07-26 01:02:15.823321 rockset-2.0.2/rockset/model/document_status.py
+-rw-r--r--   0        0        0    14990 2023-07-26 01:02:15.831321 rockset-2.0.2/rockset/model/dynamodb_collection_creation_request.py
+-rw-r--r--   0        0        0    12563 2023-07-26 01:02:15.839321 rockset-2.0.2/rockset/model/dynamodb_integration.py
+-rw-r--r--   0        0        0    12484 2023-07-26 01:02:15.847321 rockset-2.0.2/rockset/model/dynamodb_integration_creation_request.py
+-rw-r--r--   0        0        0    14440 2023-07-26 01:02:15.851321 rockset-2.0.2/rockset/model/dynamodb_source_wrapper.py
+-rw-r--r--   0        0        0    14520 2023-07-26 01:02:15.867321 rockset-2.0.2/rockset/model/error_model.py
+-rw-r--r--   0        0        0    12392 2023-07-26 01:02:15.875321 rockset-2.0.2/rockset/model/event_time_info.py
+-rw-r--r--   0        0        0    12656 2023-07-26 01:02:15.879321 rockset-2.0.2/rockset/model/execute_public_query_lambda_request.py
+-rw-r--r--   0        0        0    18176 2023-07-26 01:02:15.887322 rockset-2.0.2/rockset/model/execute_query_lambda_request.py
+-rw-r--r--   0        0        0    11743 2023-07-26 01:02:15.891322 rockset-2.0.2/rockset/model/field_mapping_query.py
+-rw-r--r--   0        0        0    13075 2023-07-26 01:02:15.899322 rockset-2.0.2/rockset/model/field_mapping_v2.py
+-rw-r--r--   0        0        0    12543 2023-07-26 01:02:15.903322 rockset-2.0.2/rockset/model/field_partition.py
+-rw-r--r--   0        0        0    15063 2023-07-26 00:43:43.306647 rockset-2.0.2/rockset/model/file_upload_collection_creation_request.py
+-rw-r--r--   0        0        0    13611 2023-07-26 00:43:43.306647 rockset-2.0.2/rockset/model/file_upload_source_wrapper.py
+-rw-r--r--   0        0        0    13202 2023-07-26 01:02:15.911322 rockset-2.0.2/rockset/model/format_params.py
+-rw-r--r--   0        0        0    12001 2023-07-26 01:02:15.915322 rockset-2.0.2/rockset/model/gcp_service_account.py
+-rw-r--r--   0        0        0    14940 2023-07-26 01:02:15.923322 rockset-2.0.2/rockset/model/gcs_collection_creation_request.py
+-rw-r--r--   0        0        0    11915 2023-07-26 01:02:15.931322 rockset-2.0.2/rockset/model/gcs_integration.py
+-rw-r--r--   0        0        0    12409 2023-07-26 01:02:15.935322 rockset-2.0.2/rockset/model/gcs_integration_creation_request.py
+-rw-r--r--   0        0        0    14296 2023-07-26 01:02:15.943322 rockset-2.0.2/rockset/model/gcs_source_wrapper.py
+-rw-r--r--   0        0        0    11760 2023-07-26 01:02:15.947322 rockset-2.0.2/rockset/model/get_alias_response.py
+-rw-r--r--   0        0        0    11771 2023-07-26 01:02:15.955322 rockset-2.0.2/rockset/model/get_api_key_response.py
+-rw-r--r--   0        0        0    11810 2023-07-26 01:02:15.959322 rockset-2.0.2/rockset/model/get_collection_response.py
+-rw-r--r--   0        0        0    11820 2023-07-26 01:02:15.967322 rockset-2.0.2/rockset/model/get_integration_response.py
+-rw-r--r--   0        0        0    11789 2023-07-26 01:02:15.971322 rockset-2.0.2/rockset/model/get_query_response.py
+-rw-r--r--   0        0        0    11770 2023-07-26 01:02:15.975322 rockset-2.0.2/rockset/model/get_source_response.py
+-rw-r--r--   0        0        0    11750 2023-07-26 01:02:15.983322 rockset-2.0.2/rockset/model/get_view_response.py
+-rw-r--r--   0        0        0    11861 2023-07-26 01:02:15.987322 rockset-2.0.2/rockset/model/get_virtual_instance_response.py
+-rw-r--r--   0        0        0    11800 2023-07-26 01:02:15.995322 rockset-2.0.2/rockset/model/get_workspace_response.py
+-rw-r--r--   0        0        0    12704 2023-07-26 01:02:15.999323 rockset-2.0.2/rockset/model/input_field.py
+-rw-r--r--   0        0        0    17788 2023-07-26 01:02:16.007322 rockset-2.0.2/rockset/model/integration.py
+-rw-r--r--   0        0        0    14960 2023-07-26 01:02:16.011323 rockset-2.0.2/rockset/model/kafka_collection_creation_request.py
+-rw-r--r--   0        0        0    14826 2023-07-26 01:02:16.019322 rockset-2.0.2/rockset/model/kafka_integration.py
+-rw-r--r--   0        0        0    12439 2023-07-26 01:02:16.027323 rockset-2.0.2/rockset/model/kafka_integration_creation_request.py
+-rw-r--r--   0        0        0    14027 2023-07-26 01:02:16.035323 rockset-2.0.2/rockset/model/kafka_source_wrapper.py
+-rw-r--r--   0        0        0    11845 2023-07-26 01:02:16.039323 rockset-2.0.2/rockset/model/kafka_v3_security_config.py
+-rw-r--r--   0        0        0    14980 2023-07-26 01:02:16.047323 rockset-2.0.2/rockset/model/kinesis_collection_creation_request.py
+-rw-r--r--   0        0        0    12169 2023-07-26 01:02:16.055323 rockset-2.0.2/rockset/model/kinesis_integration.py
+-rw-r--r--   0        0        0    12469 2023-07-26 01:02:16.059323 rockset-2.0.2/rockset/model/kinesis_integration_creation_request.py
+-rw-r--r--   0        0        0    13895 2023-07-26 01:02:16.067323 rockset-2.0.2/rockset/model/kinesis_source_wrapper.py
+-rw-r--r--   0        0        0    11819 2023-07-26 01:02:16.071323 rockset-2.0.2/rockset/model/list_aliases_response.py
+-rw-r--r--   0        0        0    11835 2023-07-26 01:02:16.079323 rockset-2.0.2/rockset/model/list_api_keys_response.py
+-rw-r--r--   0        0        0    11937 2023-07-26 01:02:16.083323 rockset-2.0.2/rockset/model/list_collection_mounts_response.py
+-rw-r--r--   0        0        0    11874 2023-07-26 01:02:16.091323 rockset-2.0.2/rockset/model/list_collections_response.py
+-rw-r--r--   0        0        0    11892 2023-07-26 01:02:16.095323 rockset-2.0.2/rockset/model/list_integrations_response.py
+-rw-r--r--   0        0        0    11804 2023-07-26 01:02:16.103323 rockset-2.0.2/rockset/model/list_queries_response.py
+-rw-r--r--   0        0        0    11964 2023-07-26 01:02:16.107323 rockset-2.0.2/rockset/model/list_query_lambda_tags_response.py
+-rw-r--r--   0        0        0    12010 2023-07-26 01:02:16.111323 rockset-2.0.2/rockset/model/list_query_lambda_versions_response.py
+-rw-r--r--   0        0        0    11889 2023-07-26 01:02:16.119323 rockset-2.0.2/rockset/model/list_query_lambdas_response.py
+-rw-r--r--   0        0        0    11802 2023-07-26 01:02:16.123324 rockset-2.0.2/rockset/model/list_roles_response.py
+-rw-r--r--   0        0        0    11856 2023-07-26 01:02:16.131323 rockset-2.0.2/rockset/model/list_sources_response.py
+-rw-r--r--   0        0        0    12003 2023-07-26 01:02:16.135324 rockset-2.0.2/rockset/model/list_unsubscribe_preferences_response.py
+-rw-r--r--   0        0        0    11794 2023-07-26 01:02:16.139324 rockset-2.0.2/rockset/model/list_users_response.py
+-rw-r--r--   0        0        0    11802 2023-07-26 01:02:16.147324 rockset-2.0.2/rockset/model/list_views_response.py
+-rw-r--r--   0        0        0    11937 2023-07-26 01:02:16.151324 rockset-2.0.2/rockset/model/list_virtual_instances_response.py
+-rw-r--r--   0        0        0    11854 2023-07-26 01:02:16.155324 rockset-2.0.2/rockset/model/list_workspaces_response.py
+-rw-r--r--   0        0        0    11815 2023-07-26 01:02:16.163324 rockset-2.0.2/rockset/model/mongo_db_integration.py
+-rw-r--r--   0        0        0    14980 2023-07-26 01:02:16.167324 rockset-2.0.2/rockset/model/mongodb_collection_creation_request.py
+-rw-r--r--   0        0        0    12470 2023-07-26 01:02:16.175324 rockset-2.0.2/rockset/model/mongodb_integration_creation_request.py
+-rw-r--r--   0        0        0    14123 2023-07-26 01:02:16.179324 rockset-2.0.2/rockset/model/mongodb_source_wrapper.py
+-rw-r--r--   0        0        0    13910 2023-07-26 01:02:16.187324 rockset-2.0.2/rockset/model/organization.py
+-rw-r--r--   0        0        0    11821 2023-07-26 01:02:16.191324 rockset-2.0.2/rockset/model/organization_response.py
+-rw-r--r--   0        0        0    12527 2023-07-26 01:02:16.195324 rockset-2.0.2/rockset/model/output_field.py
+-rw-r--r--   0        0        0    11775 2023-07-26 01:02:16.203324 rockset-2.0.2/rockset/model/pagination.py
+-rw-r--r--   0        0        0    13055 2023-07-26 01:02:16.207324 rockset-2.0.2/rockset/model/pagination_info.py
+-rw-r--r--   0        0        0    12155 2023-07-26 01:02:16.211324 rockset-2.0.2/rockset/model/patch_document.py
+-rw-r--r--   0        0        0    11920 2023-07-26 01:02:16.215324 rockset-2.0.2/rockset/model/patch_documents_request.py
+-rw-r--r--   0        0        0    11868 2023-07-26 01:02:16.223324 rockset-2.0.2/rockset/model/patch_documents_response.py
+-rw-r--r--   0        0        0    13672 2023-07-26 01:02:16.227324 rockset-2.0.2/rockset/model/patch_operation.py
+-rw-r--r--   0        0        0    15452 2023-07-26 01:02:16.235324 rockset-2.0.2/rockset/model/privilege.py
+-rw-r--r--   0        0        0    12407 2023-07-26 01:02:16.239324 rockset-2.0.2/rockset/model/query_error.py
+-rw-r--r--   0        0        0    11907 2023-07-26 01:02:16.247324 rockset-2.0.2/rockset/model/query_field_type.py
+-rw-r--r--   0        0        0    14972 2023-07-26 01:02:16.255324 rockset-2.0.2/rockset/model/query_info.py
+-rw-r--r--   0        0        0    13688 2023-07-26 01:02:16.263325 rockset-2.0.2/rockset/model/query_lambda.py
+-rw-r--r--   0        0        0    12219 2023-07-26 01:02:16.267325 rockset-2.0.2/rockset/model/query_lambda_sql.py
+-rw-r--r--   0        0        0    12786 2023-07-26 01:02:16.275325 rockset-2.0.2/rockset/model/query_lambda_stats.py
+-rw-r--r--   0        0        0    12124 2023-07-26 01:02:16.283325 rockset-2.0.2/rockset/model/query_lambda_tag.py
+-rw-r--r--   0        0        0    11843 2023-07-26 01:02:16.287325 rockset-2.0.2/rockset/model/query_lambda_tag_response.py
+-rw-r--r--   0        0        0    15267 2023-07-26 01:02:16.295325 rockset-2.0.2/rockset/model/query_lambda_version.py
+-rw-r--r--   0        0        0    11883 2023-07-26 01:02:16.303325 rockset-2.0.2/rockset/model/query_lambda_version_response.py
+-rw-r--r--   0        0        0    13051 2023-07-26 00:43:43.310647 rockset-2.0.2/rockset/model/query_pagination_response.py
+-rw-r--r--   0        0        0    12188 2023-07-26 01:02:16.315325 rockset-2.0.2/rockset/model/query_parameter.py
+-rw-r--r--   0        0        0    15940 2023-07-26 01:02:16.323325 rockset-2.0.2/rockset/model/query_request.py
+-rw-r--r--   0        0        0    13722 2023-07-26 01:02:16.327325 rockset-2.0.2/rockset/model/query_request_sql.py
+-rw-r--r--   0        0        0    16189 2023-07-26 00:43:43.310647 rockset-2.0.2/rockset/model/query_response.py
+-rw-r--r--   0        0        0    12105 2023-07-26 01:02:16.339325 rockset-2.0.2/rockset/model/query_response_stats.py
+-rw-r--r--   0        0        0    11870 2023-07-26 01:02:16.347325 rockset-2.0.2/rockset/model/resume_virtual_instance_response.py
+-rw-r--r--   0        0        0    13363 2023-07-26 01:02:16.351325 rockset-2.0.2/rockset/model/role.py
+-rw-r--r--   0        0        0    11741 2023-07-26 01:02:16.359325 rockset-2.0.2/rockset/model/role_response.py
+-rw-r--r--   0        0        0    14930 2023-07-26 01:02:16.363325 rockset-2.0.2/rockset/model/s3_collection_creation_request.py
+-rw-r--r--   0        0        0    12154 2023-07-26 01:02:16.371325 rockset-2.0.2/rockset/model/s3_integration.py
+-rw-r--r--   0        0        0    12394 2023-07-26 01:02:16.375325 rockset-2.0.2/rockset/model/s3_integration_creation_request.py
+-rw-r--r--   0        0        0    14862 2023-07-26 01:02:16.379325 rockset-2.0.2/rockset/model/s3_source_wrapper.py
+-rw-r--r--   0        0        0    12201 2023-07-26 01:02:16.387325 rockset-2.0.2/rockset/model/schema_registry_config.py
+-rw-r--r--   0        0        0    11696 2023-07-26 00:43:43.310647 rockset-2.0.2/rockset/model/segment_integration.py
+-rw-r--r--   0        0        0    12465 2023-07-26 00:43:43.310647 rockset-2.0.2/rockset/model/segment_integration_creation_request.py
+-rw-r--r--   0        0        0    15000 2023-07-26 01:02:16.399326 rockset-2.0.2/rockset/model/snowflake_collection_creation_request.py
+-rw-r--r--   0        0        0    14450 2023-07-26 01:02:16.407326 rockset-2.0.2/rockset/model/snowflake_integration.py
+-rw-r--r--   0        0        0    12499 2023-07-26 01:02:16.415326 rockset-2.0.2/rockset/model/snowflake_integration_creation_request.py
+-rw-r--r--   0        0        0    13907 2023-07-26 01:02:16.419326 rockset-2.0.2/rockset/model/snowflake_source_wrapper.py
+-rw-r--r--   0        0        0    17773 2023-07-26 01:02:16.427326 rockset-2.0.2/rockset/model/source.py
+-rw-r--r--   0        0        0    13169 2023-07-26 01:02:16.435326 rockset-2.0.2/rockset/model/source_azure_blob_storage.py
+-rw-r--r--   0        0        0    12664 2023-07-26 01:02:16.443326 rockset-2.0.2/rockset/model/source_azure_event_hubs.py
+-rw-r--r--   0        0        0    12552 2023-07-26 01:02:16.447326 rockset-2.0.2/rockset/model/source_azure_service_bus.py
+-rw-r--r--   0        0        0    13624 2023-07-26 01:02:16.455326 rockset-2.0.2/rockset/model/source_dynamo_db.py
+-rw-r--r--   0        0        0    12391 2023-07-26 01:02:16.463326 rockset-2.0.2/rockset/model/source_file_upload.py
+-rw-r--r--   0        0        0    13371 2023-07-26 01:02:16.471326 rockset-2.0.2/rockset/model/source_gcs.py
+-rw-r--r--   0        0        0    13209 2023-07-26 01:02:16.483326 rockset-2.0.2/rockset/model/source_kafka.py
+-rw-r--r--   0        0        0    13024 2023-07-26 01:02:16.487326 rockset-2.0.2/rockset/model/source_kinesis.py
+-rw-r--r--   0        0        0    13315 2023-07-26 01:02:16.495326 rockset-2.0.2/rockset/model/source_mongo_db.py
+-rw-r--r--   0        0        0    13916 2023-07-26 01:02:16.507326 rockset-2.0.2/rockset/model/source_s3.py
+-rw-r--r--   0        0        0    12223 2023-07-26 01:02:16.511326 rockset-2.0.2/rockset/model/source_snapshot.py
+-rw-r--r--   0        0        0    13110 2023-07-26 01:02:16.523326 rockset-2.0.2/rockset/model/source_snowflake.py
+-rw-r--r--   0        0        0    11873 2023-07-26 01:02:16.527327 rockset-2.0.2/rockset/model/source_system.py
+-rw-r--r--   0        0        0    11661 2023-07-26 01:02:16.531327 rockset-2.0.2/rockset/model/sql_expression.py
+-rw-r--r--   0        0        0    13116 2023-07-26 01:02:16.539327 rockset-2.0.2/rockset/model/stats.py
+-rw-r--r--   0        0        0    13696 2023-07-26 01:02:16.547327 rockset-2.0.2/rockset/model/status.py
+-rw-r--r--   0        0        0    13111 2023-07-26 01:02:16.551327 rockset-2.0.2/rockset/model/status_azure_event_hubs.py
+-rw-r--r--   0        0        0    12364 2023-07-26 01:02:16.555327 rockset-2.0.2/rockset/model/status_azure_event_hubs_partition.py
+-rw-r--r--   0        0        0    12727 2023-07-26 01:02:16.559327 rockset-2.0.2/rockset/model/status_azure_service_bus.py
+-rw-r--r--   0        0        0    12210 2023-07-26 01:02:16.563327 rockset-2.0.2/rockset/model/status_azure_service_bus_session.py
+-rw-r--r--   0        0        0    13563 2023-07-26 01:02:16.567327 rockset-2.0.2/rockset/model/status_dynamo_db.py
+-rw-r--r--   0        0        0    12705 2023-07-26 01:02:16.575327 rockset-2.0.2/rockset/model/status_dynamo_db_v2.py
+-rw-r--r--   0        0        0    13123 2023-07-26 01:02:16.579327 rockset-2.0.2/rockset/model/status_kafka.py
+-rw-r--r--   0        0        0    12337 2023-07-26 01:02:16.583327 rockset-2.0.2/rockset/model/status_kafka_partition.py
+-rw-r--r--   0        0        0    15614 2023-07-26 01:02:16.587327 rockset-2.0.2/rockset/model/status_mongo_db.py
+-rw-r--r--   0        0        0    11924 2023-07-26 01:02:16.591327 rockset-2.0.2/rockset/model/status_snowflake.py
+-rw-r--r--   0        0        0    11873 2023-07-26 01:02:16.599327 rockset-2.0.2/rockset/model/suspend_virtual_instance_response.py
+-rw-r--r--   0        0        0    11894 2023-07-26 01:02:16.603327 rockset-2.0.2/rockset/model/unsubscribe_preference.py
+-rw-r--r--   0        0        0    12119 2023-07-26 01:02:16.607327 rockset-2.0.2/rockset/model/update_alias_request.py
+-rw-r--r--   0        0        0    11818 2023-07-26 01:02:16.615327 rockset-2.0.2/rockset/model/update_api_key_request.py
+-rw-r--r--   0        0        0    11780 2023-07-26 01:02:16.623327 rockset-2.0.2/rockset/model/update_api_key_response.py
+-rw-r--r--   0        0        0    12247 2023-07-26 01:02:16.627327 rockset-2.0.2/rockset/model/update_collection_request.py
+-rw-r--r--   0        0        0    11867 2023-07-26 00:43:43.310647 rockset-2.0.2/rockset/model/update_integration_request.py
+-rw-r--r--   0        0        0    11829 2023-07-26 00:43:43.310647 rockset-2.0.2/rockset/model/update_integration_response.py
+-rw-r--r--   0        0        0    12329 2023-07-26 01:02:16.635327 rockset-2.0.2/rockset/model/update_query_lambda_request.py
+-rw-r--r--   0        0        0    12222 2023-07-26 01:02:16.647328 rockset-2.0.2/rockset/model/update_role_request.py
+-rw-r--r--   0        0        0    12006 2023-07-26 01:02:16.663328 rockset-2.0.2/rockset/model/update_unsubscribe_preferences_request.py
+-rw-r--r--   0        0        0    12009 2023-07-26 01:02:16.667328 rockset-2.0.2/rockset/model/update_unsubscribe_preferences_response.py
+-rw-r--r--   0        0        0    12206 2023-07-26 01:02:16.675328 rockset-2.0.2/rockset/model/update_user_request.py
+-rw-r--r--   0        0        0    11958 2023-07-26 01:02:16.691328 rockset-2.0.2/rockset/model/update_view_request.py
+-rw-r--r--   0        0        0    11759 2023-07-26 01:02:16.695328 rockset-2.0.2/rockset/model/update_view_response.py
+-rw-r--r--   0        0        0    15174 2023-07-26 01:02:16.699328 rockset-2.0.2/rockset/model/update_virtual_instance_request.py
+-rw-r--r--   0        0        0    11870 2023-07-26 01:02:16.703328 rockset-2.0.2/rockset/model/update_virtual_instance_response.py
+-rw-r--r--   0        0        0    12907 2023-07-26 01:02:16.707328 rockset-2.0.2/rockset/model/user.py
+-rw-r--r--   0        0        0    12155 2023-07-26 01:02:16.711328 rockset-2.0.2/rockset/model/validate_query_response.py
+-rw-r--r--   0        0        0    14899 2023-07-26 01:02:16.715328 rockset-2.0.2/rockset/model/view.py
+-rw-r--r--   0        0        0    18629 2023-07-26 01:02:16.719328 rockset-2.0.2/rockset/model/virtual_instance.py
+-rw-r--r--   0        0        0    11772 2023-07-26 01:02:16.727328 rockset-2.0.2/rockset/model/virtual_instance_stats.py
+-rw-r--r--   0        0        0    12971 2023-07-26 01:02:16.731328 rockset-2.0.2/rockset/model/workspace.py
+-rw-r--r--   0        0        0    12998 2023-07-26 01:02:16.735328 rockset-2.0.2/rockset/model/xml_params.py
+-rw-r--r--   0        0        0    84037 2023-07-26 01:02:17.355333 rockset-2.0.2/rockset/model_utils.py
+-rw-r--r--   0        0        0    14577 2023-07-26 01:02:17.355333 rockset-2.0.2/rockset/models/__init__.py
+-rw-r--r--   0        0        0     1819 2023-07-26 00:43:43.314648 rockset-2.0.2/rockset/query_paginator.py
+-rw-r--r--   0        0        0    14645 2023-07-26 01:02:17.347333 rockset-2.0.2/rockset/rest.py
+-rw-r--r--   0        0        0     9063 2023-07-26 00:43:43.314648 rockset-2.0.2/rockset/rockset_client.py
+-rw-r--r--   0        0        0     3644 2023-07-26 00:43:43.314648 rockset-2.0.2/rockset/value.py
+-rw-r--r--   0        0        0     2169 1970-01-01 00:00:00.000000 rockset-2.0.2/PKG-INFO
```

### Comparing `rockset-2.0.0/pyproject.toml` & `rockset-2.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rockset"
-version = "2.0.0"
+version = "2.0.2"
 description = "The python client for the Rockset API."
 authors = ["Rockset <support@rockset.com>"]
 packages = [
     {include = "rockset"}
 ]
 documentation = "https://github.com/rockset/rockset-python-client"
 repository = "https://github.com/rockset/rockset-python-client"
@@ -42,8 +42,8 @@
 [tool.poetry.dev-dependencies]
 setuptools = "^21.0.0"
 openapi-core = "^0.14.2"
 pytest = "^7.0.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `rockset-2.0.0/rockset/__init__.py` & `rockset-2.0.2/rockset/__init__.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/api/aliases_api.py` & `rockset-2.0.2/rockset/api/aliases_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/api/api_keys_api.py` & `rockset-2.0.2/rockset/api/api_keys_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/api/collections_api.py` & `rockset-2.0.2/rockset/api/collections_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,28 +22,27 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from rockset.model.azure_blob_storage_collection_creation_request import AzureBlobStorageCollectionCreationRequest
 from rockset.model.azure_event_hubs_collection_creation_request import AzureEventHubsCollectionCreationRequest
-from rockset.model.azure_service_bus_collection_creation_request import AzureServiceBusCollectionCreationRequest
 from rockset.model.create_collection_response import CreateCollectionResponse
 from rockset.model.delete_collection_response import DeleteCollectionResponse
 from rockset.model.dynamodb_collection_creation_request import DynamodbCollectionCreationRequest
 from rockset.model.error_model import ErrorModel
-from rockset.model.file_upload_collection_creation_request import FileUploadCollectionCreationRequest
 from rockset.model.gcs_collection_creation_request import GcsCollectionCreationRequest
 from rockset.model.get_collection_response import GetCollectionResponse
 from rockset.model.kafka_collection_creation_request import KafkaCollectionCreationRequest
 from rockset.model.kinesis_collection_creation_request import KinesisCollectionCreationRequest
 from rockset.model.list_collections_response import ListCollectionsResponse
 from rockset.model.mongodb_collection_creation_request import MongodbCollectionCreationRequest
 from rockset.model.s3_collection_creation_request import S3CollectionCreationRequest
 from rockset.model.snowflake_collection_creation_request import SnowflakeCollectionCreationRequest
+from rockset.model.update_collection_request import UpdateCollectionRequest
 from rockset.models import *
 
 
 class Collections(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
@@ -164,71 +163,14 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.create_azure_service_bus_collection_endpoint = _Endpoint(
-            settings={
-                'response_type': (CreateCollectionResponse,),
-                'auth': [
-                    'apikey'
-                ],
-                'endpoint_path': '/v1/orgs/self/ws/{workspace}/collections',
-                'operation_id': 'create_azure_service_bus_collection',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'workspace',
-                    'azure_service_bus_collection_creation_request',
-                ],
-                'required': [
-                    'workspace',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'workspace':
-                        (str,),
-                    'azure_service_bus_collection_creation_request':
-                        (AzureServiceBusCollectionCreationRequest,),
-                },
-                'attribute_map': {
-                    'workspace': 'workspace',
-                },
-                'location_map': {
-                    'workspace': 'path',
-                    'azure_service_bus_collection_creation_request': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
         self.create_dynamodb_collection_endpoint = _Endpoint(
             settings={
                 'response_type': (CreateCollectionResponse,),
                 'auth': [
                     'apikey'
                 ],
                 'endpoint_path': '/v1/orgs/self/ws/{workspace}/collections',
@@ -278,29 +220,29 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.create_file_upload_collection_endpoint = _Endpoint(
+        self.create_gcs_collection_endpoint = _Endpoint(
             settings={
                 'response_type': (CreateCollectionResponse,),
                 'auth': [
                     'apikey'
                 ],
                 'endpoint_path': '/v1/orgs/self/ws/{workspace}/collections',
-                'operation_id': 'create_file_upload_collection',
+                'operation_id': 'create_gcs_collection',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'workspace',
-                    'file_upload_collection_creation_request',
+                    'gcs_collection_creation_request',
                 ],
                 'required': [
                     'workspace',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -312,52 +254,52 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'workspace':
                         (str,),
-                    'file_upload_collection_creation_request':
-                        (FileUploadCollectionCreationRequest,),
+                    'gcs_collection_creation_request':
+                        (GcsCollectionCreationRequest,),
                 },
                 'attribute_map': {
                     'workspace': 'workspace',
                 },
                 'location_map': {
                     'workspace': 'path',
-                    'file_upload_collection_creation_request': 'body',
+                    'gcs_collection_creation_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.create_gcs_collection_endpoint = _Endpoint(
+        self.create_kafka_collection_endpoint = _Endpoint(
             settings={
                 'response_type': (CreateCollectionResponse,),
                 'auth': [
                     'apikey'
                 ],
                 'endpoint_path': '/v1/orgs/self/ws/{workspace}/collections',
-                'operation_id': 'create_gcs_collection',
+                'operation_id': 'create_kafka_collection',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'workspace',
-                    'gcs_collection_creation_request',
+                    'kafka_collection_creation_request',
                 ],
                 'required': [
                     'workspace',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -369,52 +311,52 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'workspace':
                         (str,),
-                    'gcs_collection_creation_request':
-                        (GcsCollectionCreationRequest,),
+                    'kafka_collection_creation_request':
+                        (KafkaCollectionCreationRequest,),
                 },
                 'attribute_map': {
                     'workspace': 'workspace',
                 },
                 'location_map': {
                     'workspace': 'path',
-                    'gcs_collection_creation_request': 'body',
+                    'kafka_collection_creation_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.create_kafka_collection_endpoint = _Endpoint(
+        self.create_kinesis_collection_endpoint = _Endpoint(
             settings={
                 'response_type': (CreateCollectionResponse,),
                 'auth': [
                     'apikey'
                 ],
                 'endpoint_path': '/v1/orgs/self/ws/{workspace}/collections',
-                'operation_id': 'create_kafka_collection',
+                'operation_id': 'create_kinesis_collection',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'workspace',
-                    'kafka_collection_creation_request',
+                    'kinesis_collection_creation_request',
                 ],
                 'required': [
                     'workspace',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -426,52 +368,52 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'workspace':
                         (str,),
-                    'kafka_collection_creation_request':
-                        (KafkaCollectionCreationRequest,),
+                    'kinesis_collection_creation_request':
+                        (KinesisCollectionCreationRequest,),
                 },
                 'attribute_map': {
                     'workspace': 'workspace',
                 },
                 'location_map': {
                     'workspace': 'path',
-                    'kafka_collection_creation_request': 'body',
+                    'kinesis_collection_creation_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.create_kinesis_collection_endpoint = _Endpoint(
+        self.create_mongodb_collection_endpoint = _Endpoint(
             settings={
                 'response_type': (CreateCollectionResponse,),
                 'auth': [
                     'apikey'
                 ],
                 'endpoint_path': '/v1/orgs/self/ws/{workspace}/collections',
-                'operation_id': 'create_kinesis_collection',
+                'operation_id': 'create_mongodb_collection',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'workspace',
-                    'kinesis_collection_creation_request',
+                    'mongodb_collection_creation_request',
                 ],
                 'required': [
                     'workspace',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -483,52 +425,52 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'workspace':
                         (str,),
-                    'kinesis_collection_creation_request':
-                        (KinesisCollectionCreationRequest,),
+                    'mongodb_collection_creation_request':
+                        (MongodbCollectionCreationRequest,),
                 },
                 'attribute_map': {
                     'workspace': 'workspace',
                 },
                 'location_map': {
                     'workspace': 'path',
-                    'kinesis_collection_creation_request': 'body',
+                    'mongodb_collection_creation_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.create_mongodb_collection_endpoint = _Endpoint(
+        self.create_s3_collection_endpoint = _Endpoint(
             settings={
                 'response_type': (CreateCollectionResponse,),
                 'auth': [
                     'apikey'
                 ],
                 'endpoint_path': '/v1/orgs/self/ws/{workspace}/collections',
-                'operation_id': 'create_mongodb_collection',
+                'operation_id': 'create_s3_collection',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'workspace',
-                    'mongodb_collection_creation_request',
+                    's3_collection_creation_request',
                 ],
                 'required': [
                     'workspace',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -540,52 +482,52 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'workspace':
                         (str,),
-                    'mongodb_collection_creation_request':
-                        (MongodbCollectionCreationRequest,),
+                    's3_collection_creation_request':
+                        (S3CollectionCreationRequest,),
                 },
                 'attribute_map': {
                     'workspace': 'workspace',
                 },
                 'location_map': {
                     'workspace': 'path',
-                    'mongodb_collection_creation_request': 'body',
+                    's3_collection_creation_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.create_s3_collection_endpoint = _Endpoint(
+        self.create_snowflake_collection_endpoint = _Endpoint(
             settings={
                 'response_type': (CreateCollectionResponse,),
                 'auth': [
                     'apikey'
                 ],
                 'endpoint_path': '/v1/orgs/self/ws/{workspace}/collections',
-                'operation_id': 'create_s3_collection',
+                'operation_id': 'create_snowflake_collection',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'workspace',
-                    's3_collection_creation_request',
+                    'snowflake_collection_creation_request',
                 ],
                 'required': [
                     'workspace',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -597,55 +539,56 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'workspace':
                         (str,),
-                    's3_collection_creation_request':
-                        (S3CollectionCreationRequest,),
+                    'snowflake_collection_creation_request':
+                        (SnowflakeCollectionCreationRequest,),
                 },
                 'attribute_map': {
                     'workspace': 'workspace',
                 },
                 'location_map': {
                     'workspace': 'path',
-                    's3_collection_creation_request': 'body',
+                    'snowflake_collection_creation_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
-        self.create_snowflake_collection_endpoint = _Endpoint(
+        self.delete_endpoint = _Endpoint(
             settings={
-                'response_type': (CreateCollectionResponse,),
+                'response_type': (DeleteCollectionResponse,),
                 'auth': [
                     'apikey'
                 ],
-                'endpoint_path': '/v1/orgs/self/ws/{workspace}/collections',
-                'operation_id': 'create_snowflake_collection',
-                'http_method': 'POST',
+                'endpoint_path': '/v1/orgs/self/ws/{workspace}/collections/{collection}',
+                'operation_id': 'delete',
+                'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'workspace',
-                    'snowflake_collection_creation_request',
+                    'collection',
                 ],
                 'required': [
                     'workspace',
+                    'collection',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
@@ -654,46 +597,45 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'workspace':
                         (str,),
-                    'snowflake_collection_creation_request':
-                        (SnowflakeCollectionCreationRequest,),
+                    'collection':
+                        (str,),
                 },
                 'attribute_map': {
                     'workspace': 'workspace',
+                    'collection': 'collection',
                 },
                 'location_map': {
                     'workspace': 'path',
-                    'snowflake_collection_creation_request': 'body',
+                    'collection': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [
-                    'application/json'
-                ]
+                'content_type': [],
             },
             api_client=api_client
         )
-        self.delete_endpoint = _Endpoint(
+        self.get_endpoint = _Endpoint(
             settings={
-                'response_type': (DeleteCollectionResponse,),
+                'response_type': (GetCollectionResponse,),
                 'auth': [
                     'apikey'
                 ],
                 'endpoint_path': '/v1/orgs/self/ws/{workspace}/collections/{collection}',
-                'operation_id': 'delete',
-                'http_method': 'DELETE',
+                'operation_id': 'get',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'workspace',
                     'collection',
                 ],
@@ -734,29 +676,30 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
-        self.get_endpoint = _Endpoint(
+        self.get_0_endpoint = _Endpoint(
             settings={
                 'response_type': (GetCollectionResponse,),
                 'auth': [
                     'apikey'
                 ],
                 'endpoint_path': '/v1/orgs/self/ws/{workspace}/collections/{collection}',
-                'operation_id': 'get',
-                'http_method': 'GET',
+                'operation_id': 'get_0',
+                'http_method': 'PUT',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'workspace',
                     'collection',
+                    'update_collection_request',
                 ],
                 'required': [
                     'workspace',
                     'collection',
                 ],
                 'nullable': [
                 ],
@@ -771,31 +714,36 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'workspace':
                         (str,),
                     'collection':
                         (str,),
+                    'update_collection_request':
+                        (UpdateCollectionRequest,),
                 },
                 'attribute_map': {
                     'workspace': 'workspace',
                     'collection': 'collection',
                 },
                 'location_map': {
                     'workspace': 'path',
                     'collection': 'path',
+                    'update_collection_request': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
-                'content_type': [],
+                'content_type': [
+                    'application/json'
+                ]
             },
             api_client=api_client
         )
         self.list_endpoint = _Endpoint(
             settings={
                 'response_type': (ListCollectionsResponse,),
                 'auth': [
@@ -895,17 +843,17 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[AzureBlobStorageSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create azure blob storage collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
@@ -926,34 +874,14 @@
                 field="timestamp",
                 format="seconds_since_epoch",
                 time_zone="UTC",
             ),
             field_mapping_query=FieldMappingQuery(
                 sql="sql",
             ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
             name="global-transactions",
             retention_secs=1000000,
             sources=[
                 AzureBlobStorageSourceWrapper(
                     format_params=FormatParams(
                         csv=CsvParams(
                             column_names=["c1","c2","c3"],
@@ -979,29 +907,30 @@
                     ),
                     integration_name="aws-integration",
                     container="server-logs",
                     pattern="prefix/to/**/keys/*.format",
                     prefix="prefix/to/blobs",
                 ),
             ],
+            storage_compression_type="LZ4",
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([AzureBlobStorageSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1066,17 +995,17 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[AzureEventHubsSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create azure event hubs collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
@@ -1097,34 +1026,14 @@
                 field="timestamp",
                 format="seconds_since_epoch",
                 time_zone="UTC",
             ),
             field_mapping_query=FieldMappingQuery(
                 sql="sql",
             ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
             name="global-transactions",
             retention_secs=1000000,
             sources=[
                 AzureEventHubsSourceWrapper(
                     format_params=FormatParams(
                         csv=CsvParams(
                             column_names=["c1","c2","c3"],
@@ -1149,29 +1058,30 @@
                         ),
                     ),
                     integration_name="aws-integration",
                     hub_id="event-hub-1",
                     offset_reset_policy="EARLIEST",
                 ),
             ],
+            storage_compression_type="LZ4",
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([AzureEventHubsSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1228,195 +1138,25 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['workspace'] = \
             workspace
         kwargs['azure_event_hubs_collection_creation_request'] = \
             kwargs['azure_event_hubs_collection_creation_request']
         return self.create_azure_event_hubs_collection_endpoint.call_with_http_info(**kwargs)
 
-    def create_azure_service_bus_collection(
-        self,
-        *,
-        name: str,
-        clustering_key: typing.Sequence[FieldPartition] = None,
-        description: str = None,
-        event_time_info: EventTimeInfo = None,
-        field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
-        retention_secs: int = None,
-        sources: typing.Sequence[AzureServiceBusSourceWrapper] = None,
-        workspace = "commons",
-        **kwargs
-    ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
-        """Create azure service bus collection  # noqa: E501
-
-        Create new collection in a workspace.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.create_azure_service_bus_collection(
-            clustering_key=[
-                FieldPartition(
-                    field_name="address.city.zipcode",
-                    keys=["value1","value2"],
-                    type="AUTO",
-                ),
-            ],
-            description="transactions from stores worldwide",
-            event_time_info=EventTimeInfo(
-                field="timestamp",
-                format="seconds_since_epoch",
-                time_zone="UTC",
-            ),
-            field_mapping_query=FieldMappingQuery(
-                sql="sql",
-            ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
-            name="global-transactions",
-            retention_secs=1000000,
-            sources=[
-                AzureServiceBusSourceWrapper(
-                    format_params=FormatParams(
-                        csv=CsvParams(
-                            column_names=["c1","c2","c3"],
-                            column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
-                            encoding="UTF-8",
-                            escape_char="\\",
-                            first_line_as_column_names=True,
-                            quote_char="\"",
-                            separator=",",
-                        ),
-                        json=True,
-                        mssql_dms=True,
-                        mysql_dms=True,
-                        oracle_dms=True,
-                        postgres_dms=True,
-                        xml=XmlParams(
-                            attribute_prefix="_attr",
-                            doc_tag="row",
-                            encoding="UTF-8",
-                            root_tag="root",
-                            value_tag="value",
-                        ),
-                    ),
-                    integration_name="aws-integration",
-                    subscription="rockset-subscription",
-                    topic="rockset-topic",
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
-
-        Keyword Args:
-            workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
-            clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
-            description (str): Text describing the collection.. [optional]
-            event_time_info (EventTimeInfo): [optional]
-            field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
-            name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
-            retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
-            sources ([AzureServiceBusSourceWrapper]): List of sources from which to ingest data. [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done on the data received from the server.
-                If False, the client will also not convert nested inner objects
-                into the respective model types (the outermost object
-                is still converted to the model).
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            CreateCollectionResponse
-                If the method is called asynchronously, returns an asyncio.Future which resolves to the response.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['workspace'] = \
-            workspace
-        kwargs['azure_service_bus_collection_creation_request'] = \
-            kwargs['azure_service_bus_collection_creation_request']
-        return self.create_azure_service_bus_collection_endpoint.call_with_http_info(**kwargs)
-
     def create_dynamodb_collection(
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[DynamodbSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create dynamodb collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
@@ -1437,34 +1177,14 @@
                 field="timestamp",
                 format="seconds_since_epoch",
                 time_zone="UTC",
             ),
             field_mapping_query=FieldMappingQuery(
                 sql="sql",
             ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
             name="global-transactions",
             retention_secs=1000000,
             sources=[
                 DynamodbSourceWrapper(
                     format_params=FormatParams(
                         csv=CsvParams(
                             column_names=["c1","c2","c3"],
@@ -1491,29 +1211,30 @@
                     integration_name="aws-integration",
                     aws_region="us-east-2",
                     rcu=1000,
                     table_name="dynamodb_table_name",
                     use_scan_api=True,
                 ),
             ],
+            storage_compression_type="LZ4",
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([DynamodbSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1570,196 +1291,25 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['workspace'] = \
             workspace
         kwargs['dynamodb_collection_creation_request'] = \
             kwargs['dynamodb_collection_creation_request']
         return self.create_dynamodb_collection_endpoint.call_with_http_info(**kwargs)
 
-    def create_file_upload_collection(
-        self,
-        *,
-        name: str,
-        clustering_key: typing.Sequence[FieldPartition] = None,
-        description: str = None,
-        event_time_info: EventTimeInfo = None,
-        field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
-        retention_secs: int = None,
-        sources: typing.Sequence[FileUploadSourceWrapper] = None,
-        workspace = "commons",
-        **kwargs
-    ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
-        """Create file upload collection  # noqa: E501
-
-        Create new collection in a workspace.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        ```python
-        rs = RocksetClient(api_key=APIKEY)
-        future = rs.Collections.create_file_upload_collection(
-            clustering_key=[
-                FieldPartition(
-                    field_name="address.city.zipcode",
-                    keys=["value1","value2"],
-                    type="AUTO",
-                ),
-            ],
-            description="transactions from stores worldwide",
-            event_time_info=EventTimeInfo(
-                field="timestamp",
-                format="seconds_since_epoch",
-                time_zone="UTC",
-            ),
-            field_mapping_query=FieldMappingQuery(
-                sql="sql",
-            ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
-            name="global-transactions",
-            retention_secs=1000000,
-            sources=[
-                FileUploadSourceWrapper(
-                    format_params=FormatParams(
-                        csv=CsvParams(
-                            column_names=["c1","c2","c3"],
-                            column_types=["BOOLEAN","INTEGER","FLOAT","STRING"],
-                            encoding="UTF-8",
-                            escape_char="\\",
-                            first_line_as_column_names=True,
-                            quote_char="\"",
-                            separator=",",
-                        ),
-                        json=True,
-                        mssql_dms=True,
-                        mysql_dms=True,
-                        oracle_dms=True,
-                        postgres_dms=True,
-                        xml=XmlParams(
-                            attribute_prefix="_attr",
-                            doc_tag="row",
-                            encoding="UTF-8",
-                            root_tag="root",
-                            value_tag="value",
-                        ),
-                    ),
-                    integration_name="aws-integration",
-                    file_name="file1.json",
-                    file_size=12345,
-                    file_upload_time="2019-01-15T21:48:23Z",
-                ),
-            ],
-            async_req=True,
-        )
-        result = await future
-        ```
-
-        Keyword Args:
-            workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
-            clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
-            description (str): Text describing the collection.. [optional]
-            event_time_info (EventTimeInfo): [optional]
-            field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
-            name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
-            retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
-            sources ([FileUploadSourceWrapper]): List of sources from which to ingest data. [optional]
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done on the data received from the server.
-                If False, the client will also not convert nested inner objects
-                into the respective model types (the outermost object
-                is still converted to the model).
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            CreateCollectionResponse
-                If the method is called asynchronously, returns an asyncio.Future which resolves to the response.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_spec_property_naming'] = kwargs.get(
-            '_spec_property_naming', False
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['workspace'] = \
-            workspace
-        kwargs['file_upload_collection_creation_request'] = \
-            kwargs['file_upload_collection_creation_request']
-        return self.create_file_upload_collection_endpoint.call_with_http_info(**kwargs)
-
     def create_gcs_collection(
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[GcsSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create gcs collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
@@ -1780,34 +1330,14 @@
                 field="timestamp",
                 format="seconds_since_epoch",
                 time_zone="UTC",
             ),
             field_mapping_query=FieldMappingQuery(
                 sql="sql",
             ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
             name="global-transactions",
             retention_secs=1000000,
             sources=[
                 GcsSourceWrapper(
                     format_params=FormatParams(
                         csv=CsvParams(
                             column_names=["c1","c2","c3"],
@@ -1833,29 +1363,30 @@
                     ),
                     integration_name="aws-integration",
                     bucket="server-logs",
                     pattern="prefix/to/**/keys/*.format",
                     prefix="prefix/to/keys",
                 ),
             ],
+            storage_compression_type="LZ4",
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([GcsSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1920,17 +1451,17 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[KafkaSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create kafka collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
@@ -1951,34 +1482,14 @@
                 field="timestamp",
                 format="seconds_since_epoch",
                 time_zone="UTC",
             ),
             field_mapping_query=FieldMappingQuery(
                 sql="sql",
             ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
             name="global-transactions",
             retention_secs=1000000,
             sources=[
                 KafkaSourceWrapper(
                     format_params=FormatParams(
                         csv=CsvParams(
                             column_names=["c1","c2","c3"],
@@ -2005,29 +1516,30 @@
                     integration_name="aws-integration",
                     consumer_group_id="org-collection",
                     kafka_topic_name="example-topic",
                     offset_reset_policy="EARLIEST",
                     use_v3=True,
                 ),
             ],
+            storage_compression_type="LZ4",
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([KafkaSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2092,17 +1604,17 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[KinesisSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create kinesis collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
@@ -2123,34 +1635,14 @@
                 field="timestamp",
                 format="seconds_since_epoch",
                 time_zone="UTC",
             ),
             field_mapping_query=FieldMappingQuery(
                 sql="sql",
             ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
             name="global-transactions",
             retention_secs=1000000,
             sources=[
                 KinesisSourceWrapper(
                     format_params=FormatParams(
                         csv=CsvParams(
                             column_names=["c1","c2","c3"],
@@ -2179,29 +1671,30 @@
                     dms_primary_key=[
                         "dms_primary_key_example",
                     ],
                     offset_reset_policy="EARLIEST",
                     stream_name="click_stream",
                 ),
             ],
+            storage_compression_type="LZ4",
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([KinesisSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2266,17 +1759,17 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[MongodbSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create mongodb collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
@@ -2297,34 +1790,14 @@
                 field="timestamp",
                 format="seconds_since_epoch",
                 time_zone="UTC",
             ),
             field_mapping_query=FieldMappingQuery(
                 sql="sql",
             ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
             name="global-transactions",
             retention_secs=1000000,
             sources=[
                 MongodbSourceWrapper(
                     format_params=FormatParams(
                         csv=CsvParams(
                             column_names=["c1","c2","c3"],
@@ -2347,31 +1820,33 @@
                             root_tag="root",
                             value_tag="value",
                         ),
                     ),
                     integration_name="aws-integration",
                     collection_name="my_collection",
                     database_name="my_database",
+                    retrieve_full_document=True,
                 ),
             ],
+            storage_compression_type="LZ4",
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([MongodbSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2436,17 +1911,17 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[S3SourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create s3 collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
@@ -2467,34 +1942,14 @@
                 field="timestamp",
                 format="seconds_since_epoch",
                 time_zone="UTC",
             ),
             field_mapping_query=FieldMappingQuery(
                 sql="sql",
             ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
             name="global-transactions",
             retention_secs=1000000,
             sources=[
                 S3SourceWrapper(
                     format_params=FormatParams(
                         csv=CsvParams(
                             column_names=["c1","c2","c3"],
@@ -2521,29 +1976,30 @@
                     integration_name="aws-integration",
                     bucket="s3://customer-account-info",
                     pattern="prefix/to/**/keys/*.format",
                     prefix="prefix/to/keys",
                     region="us-west-2",
                 ),
             ],
+            storage_compression_type="LZ4",
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([S3SourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2608,17 +2064,17 @@
         self,
         *,
         name: str,
         clustering_key: typing.Sequence[FieldPartition] = None,
         description: str = None,
         event_time_info: EventTimeInfo = None,
         field_mapping_query: FieldMappingQuery = None,
-        field_mappings: typing.Sequence[FieldMappingV2] = None,
         retention_secs: int = None,
         sources: typing.Sequence[SnowflakeSourceWrapper] = None,
+        storage_compression_type: str = None,
         workspace = "commons",
         **kwargs
     ) -> typing.Union[CreateCollectionResponse, asyncio.Future]:
         """Create snowflake collection  # noqa: E501
 
         Create new collection in a workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
@@ -2639,34 +2095,14 @@
                 field="timestamp",
                 format="seconds_since_epoch",
                 time_zone="UTC",
             ),
             field_mapping_query=FieldMappingQuery(
                 sql="sql",
             ),
-            field_mappings=[
-                FieldMappingV2(
-                    input_fields=[
-                        InputField(
-                            field_name="address.city.zipcode",
-                            if_missing="SKIP",
-                            is_drop=True,
-                            param="zip",
-                        ),
-                    ],
-                    name="myTestMapping",
-                    output_field=OutputField(
-                        field_name="zip_hash",
-                        on_error="SKIP",
-                        value=SqlExpression(
-                            sql="SHA256()",
-                        ),
-                    ),
-                ),
-            ],
             name="global-transactions",
             retention_secs=1000000,
             sources=[
                 SnowflakeSourceWrapper(
                     format_params=FormatParams(
                         csv=CsvParams(
                             column_names=["c1","c2","c3"],
@@ -2693,29 +2129,30 @@
                     integration_name="aws-integration",
                     database="NASDAQ",
                     schema="PUBLIC",
                     table_name="COMPANIES",
                     warehouse="COMPUTE_XL",
                 ),
             ],
+            storage_compression_type="LZ4",
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]
             description (str): Text describing the collection.. [optional]
             event_time_info (EventTimeInfo): [optional]
             field_mapping_query (FieldMappingQuery): [optional]
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [required]
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]
             sources ([SnowflakeSourceWrapper]): List of sources from which to ingest data. [optional]
+            storage_compression_type (str): RocksDB storage compression type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -2950,14 +2387,113 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['workspace'] = \
             workspace
         kwargs['collection'] = \
             collection
         return self.get_endpoint.call_with_http_info(**kwargs)
 
+    def get_0(
+        self,
+        *,
+        collection: str,
+        description: str = None,
+        field_mapping_query: FieldMappingQuery = None,
+        workspace = "commons",
+        **kwargs
+    ) -> typing.Union[GetCollectionResponse, asyncio.Future]:
+        """Update Collection  # noqa: E501
+
+        Update details about a collection.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        ```python
+        rs = RocksetClient(api_key=APIKEY)
+        future = rs.Collections.get_0(
+            collection="collection_example",
+            description="transactions from stores worldwide",
+            field_mapping_query=FieldMappingQuery(
+                sql="sql",
+            ),
+            async_req=True,
+        )
+        result = await future
+        ```
+
+        Keyword Args:
+            workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
+            collection (str): name of the collection. [required]
+            description (str): Updated text describing the collection.. [optional]
+            field_mapping_query (FieldMappingQuery): [optional]
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
+                should be done on the data received from the server.
+                If False, the client will also not convert nested inner objects
+                into the respective model types (the outermost object
+                is still converted to the model).
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
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            GetCollectionResponse
+                If the method is called asynchronously, returns an asyncio.Future which resolves to the response.
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
+        kwargs['workspace'] = \
+            workspace
+        kwargs['collection'] = \
+            collection
+        kwargs['update_collection_request'] = \
+            kwargs['update_collection_request']
+        return self.get_0_endpoint.call_with_http_info(**kwargs)
+
     def list(
         self,
         **kwargs
     ) -> typing.Union[ListCollectionsResponse, asyncio.Future]:
         """List Collections  # noqa: E501
 
         Retrieve all collections in an organization.  # noqa: E501
@@ -3120,25 +2656,23 @@
 
     body_params_dict = dict()
     return_types_dict = dict()
     body_params_dict['create_azure_blob_storage_collection'] = 'azure_blob_storage_collection_creation_request'
     return_types_dict['create_azure_blob_storage_collection'] = AzureBlobStorageCollectionCreationRequest
     body_params_dict['create_azure_event_hubs_collection'] = 'azure_event_hubs_collection_creation_request'
     return_types_dict['create_azure_event_hubs_collection'] = AzureEventHubsCollectionCreationRequest
-    body_params_dict['create_azure_service_bus_collection'] = 'azure_service_bus_collection_creation_request'
-    return_types_dict['create_azure_service_bus_collection'] = AzureServiceBusCollectionCreationRequest
     body_params_dict['create_dynamodb_collection'] = 'dynamodb_collection_creation_request'
     return_types_dict['create_dynamodb_collection'] = DynamodbCollectionCreationRequest
-    body_params_dict['create_file_upload_collection'] = 'file_upload_collection_creation_request'
-    return_types_dict['create_file_upload_collection'] = FileUploadCollectionCreationRequest
     body_params_dict['create_gcs_collection'] = 'gcs_collection_creation_request'
     return_types_dict['create_gcs_collection'] = GcsCollectionCreationRequest
     body_params_dict['create_kafka_collection'] = 'kafka_collection_creation_request'
     return_types_dict['create_kafka_collection'] = KafkaCollectionCreationRequest
     body_params_dict['create_kinesis_collection'] = 'kinesis_collection_creation_request'
     return_types_dict['create_kinesis_collection'] = KinesisCollectionCreationRequest
     body_params_dict['create_mongodb_collection'] = 'mongodb_collection_creation_request'
     return_types_dict['create_mongodb_collection'] = MongodbCollectionCreationRequest
     body_params_dict['create_s3_collection'] = 's3_collection_creation_request'
     return_types_dict['create_s3_collection'] = S3CollectionCreationRequest
     body_params_dict['create_snowflake_collection'] = 'snowflake_collection_creation_request'
     return_types_dict['create_snowflake_collection'] = SnowflakeCollectionCreationRequest
+    body_params_dict['get_0'] = 'update_collection_request'
+    return_types_dict['get_0'] = UpdateCollectionRequest
```

### Comparing `rockset-2.0.0/rockset/api/custom_roles_api.py` & `rockset-2.0.2/rockset/api/custom_roles_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/api/documents_api.py` & `rockset-2.0.2/rockset/api/documents_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/api/integrations_api.py` & `rockset-2.0.2/rockset/api/integrations_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/api/organizations_api.py` & `rockset-2.0.2/rockset/api/organizations_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/api/queries_api.py` & `rockset-2.0.2/rockset/api/queries_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -710,53 +710,64 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         return self.list_active_queries_endpoint.call_with_http_info(**kwargs)
 
     def query(
         self,
         *,
         sql: QueryRequestSql,
+        _async: bool = None,
         async_options: AsyncQueryOptions = None,
+        debug_threshold_ms: int = None,
+        max_initial_results: int = None,
+        timeout_ms: int = None,
         **kwargs
     ) -> typing.Union[QueryResponse, asyncio.Future]:
         """Execute SQL Query  # noqa: E501
 
         Make a SQL query to Rockset.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         ```python
         rs = RocksetClient(api_key=APIKEY)
         future = rs.Queries.query(
+            _async=True,
             async_options=AsyncQueryOptions(
                 client_timeout_ms=1,
                 max_initial_results=1,
                 timeout_ms=1,
             ),
+            debug_threshold_ms=1,
+            max_initial_results=1,
             sql=QueryRequestSql(
                 default_row_limit=1,
                 generate_warnings=False,
                 initial_paginate_response_doc_count=1,
-                paginate=True,
                 parameters=[
                     QueryParameter(
                         name="_id",
                         type="string",
                         value="85beb391",
                     ),
                 ],
                 query="SELECT * FROM foo where _id = :_id",
             ),
+            timeout_ms=1,
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
+            _async (bool): If true, the query will run asynchronously for up to 30 minutes. The query request will immediately return with a query id that can be used to retrieve the query status and results. If false or not specified, the query will return with results once completed or timeout after 2 minutes. (To return results directly for shorter queries while still allowing a timeout of up to 30 minutes, set `async_options.client_timeout_ms`.) . [optional]
             async_options (AsyncQueryOptions): [optional]
+            debug_threshold_ms (int): If query execution takes longer than this value, debug information will be logged. If the query text includes the DEBUG hint and this parameter is also provided, only this value will be used and the DEBUG hint will be ignored.. [optional]
+            max_initial_results (int): This limits the maximum number of results in the initial response. A pagination cursor is returned if the number of results exceeds `max_initial_results`. If `max_initial_results` is not set, all results will be returned in the initial response up to 4 million. If `max_initial_results` is set, the value must be between 0 and 100,000. If the query is async and `client_timeout_ms` is exceeded, `max_initial_results` does not apply since none of the results will be returned with the initial response.. [optional]
             sql (QueryRequestSql): [required]
+            timeout_ms (int): If a query exceeds the specified timeout, the query will automatically stop and return an error. The query timeout defaults to a maximum of 2 minutes. If `async` is true, the query timeout defaults to a maximum of 30 minutes.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -815,53 +826,64 @@
             kwargs['query_request']
         return self.query_endpoint.call_with_http_info(**kwargs)
 
     def validate(
         self,
         *,
         sql: QueryRequestSql,
+        _async: bool = None,
         async_options: AsyncQueryOptions = None,
+        debug_threshold_ms: int = None,
+        max_initial_results: int = None,
+        timeout_ms: int = None,
         **kwargs
     ) -> typing.Union[ValidateQueryResponse, asyncio.Future]:
         """Validate Query  # noqa: E501
 
         Validate a SQL query with Rockset's parser and planner.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         ```python
         rs = RocksetClient(api_key=APIKEY)
         future = rs.Queries.validate(
+            _async=True,
             async_options=AsyncQueryOptions(
                 client_timeout_ms=1,
                 max_initial_results=1,
                 timeout_ms=1,
             ),
+            debug_threshold_ms=1,
+            max_initial_results=1,
             sql=QueryRequestSql(
                 default_row_limit=1,
                 generate_warnings=False,
                 initial_paginate_response_doc_count=1,
-                paginate=True,
                 parameters=[
                     QueryParameter(
                         name="_id",
                         type="string",
                         value="85beb391",
                     ),
                 ],
                 query="SELECT * FROM foo where _id = :_id",
             ),
+            timeout_ms=1,
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
+            _async (bool): If true, the query will run asynchronously for up to 30 minutes. The query request will immediately return with a query id that can be used to retrieve the query status and results. If false or not specified, the query will return with results once completed or timeout after 2 minutes. (To return results directly for shorter queries while still allowing a timeout of up to 30 minutes, set `async_options.client_timeout_ms`.) . [optional]
             async_options (AsyncQueryOptions): [optional]
+            debug_threshold_ms (int): If query execution takes longer than this value, debug information will be logged. If the query text includes the DEBUG hint and this parameter is also provided, only this value will be used and the DEBUG hint will be ignored.. [optional]
+            max_initial_results (int): This limits the maximum number of results in the initial response. A pagination cursor is returned if the number of results exceeds `max_initial_results`. If `max_initial_results` is not set, all results will be returned in the initial response up to 4 million. If `max_initial_results` is set, the value must be between 0 and 100,000. If the query is async and `client_timeout_ms` is exceeded, `max_initial_results` does not apply since none of the results will be returned with the initial response.. [optional]
             sql (QueryRequestSql): [required]
+            timeout_ms (int): If a query exceeds the specified timeout, the query will automatically stop and return an error. The query timeout defaults to a maximum of 2 minutes. If `async` is true, the query timeout defaults to a maximum of 30 minutes.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `rockset-2.0.0/rockset/api/query_lambdas_api.py` & `rockset-2.0.2/rockset/api/query_lambdas_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1378,20 +1378,24 @@
 
     def execute_query_lambda(
         self,
         *,
         query_lambda: str,
         version: str,
         workspace = "commons",
+        _async: bool = None,
         async_options: AsyncQueryOptions = None,
+        debug_threshold_ms: int = None,
         default_row_limit: int = None,
         generate_warnings: bool = None,
         initial_paginate_response_doc_count: int = None,
+        max_initial_results: int = None,
         paginate: bool = None,
         parameters: typing.Sequence[QueryParameter] = None,
+        timeout_ms: int = None,
         virtual_instance_id: str = None,
         **kwargs
     ) -> typing.Union[QueryResponse, asyncio.Future]:
         """Execute Query Lambda By Version  # noqa: E501
 
         Execute a particular version of a Query Lambda.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
@@ -1480,20 +1484,24 @@
 
     def execute_query_lambda_by_tag(
         self,
         *,
         query_lambda: str,
         tag: str,
         workspace = "commons",
+        _async: bool = None,
         async_options: AsyncQueryOptions = None,
+        debug_threshold_ms: int = None,
         default_row_limit: int = None,
         generate_warnings: bool = None,
         initial_paginate_response_doc_count: int = None,
+        max_initial_results: int = None,
         paginate: bool = None,
         parameters: typing.Sequence[QueryParameter] = None,
+        timeout_ms: int = None,
         virtual_instance_id: str = None,
         **kwargs
     ) -> typing.Union[QueryResponse, asyncio.Future]:
         """Execute Query Lambda By Tag  # noqa: E501
 
         Execute the Query Lambda version associated with a given tag.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
```

### Comparing `rockset-2.0.0/rockset/api/shared_lambdas_api.py` & `rockset-2.0.2/rockset/api/shared_lambdas_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/api/users_api.py` & `rockset-2.0.2/rockset/api/users_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/api/views_api.py` & `rockset-2.0.2/rockset/api/views_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/api/virtual_instances_api.py` & `rockset-2.0.2/rockset/api/virtual_instances_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -744,38 +744,44 @@
 
     def create(
         self,
         *,
         name: str,
         auto_suspend_seconds: int = None,
         description: str = None,
+        enable_remount_on_resume: bool = None,
+        mount_refresh_interval_seconds: int = None,
         type: str = None,
         **kwargs
     ) -> typing.Union[CreateVirtualInstanceResponse, asyncio.Future]:
         """Create Virtual Instance  # noqa: E501
 
         [beta] Create virtual instance  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         ```python
         rs = RocksetClient(api_key=APIKEY)
         future = rs.VirtualInstances.create(
             auto_suspend_seconds=3600,
             description="VI serving prod traffic",
+            enable_remount_on_resume=True,
+            mount_refresh_interval_seconds=3600,
             name="prod_vi",
             type="LARGE",
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
             auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]
             description (str): Description of requested virtual instance.. [optional]
+            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]
+            mount_refresh_interval_seconds (int): Number of seconds between data refreshes for mounts on this Virtual Instance. A value of 0 means continuous refresh and a value of null means never refresh.. [optional]
             name (str): Unique identifier for virtual instance, can contain alphanumeric or dash characters.. [required]
             type (str): Requested virtual instance type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1011,15 +1017,15 @@
         *,
         virtual_instance_id: str,
         collection_path: str,
         **kwargs
     ) -> typing.Union[CollectionMountResponse, asyncio.Future]:
         """Get Collection Mount  # noqa: E501
 
-        [beta] Get a mount on this virtual instance.  # noqa: E501
+        [beta] Retrieve a mount on this virtual instance.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         ```python
         rs = RocksetClient(api_key=APIKEY)
         future = rs.VirtualInstances.get_collection_mount(
             virtual_instance_id="virtualInstanceId_example",
@@ -1346,38 +1352,35 @@
         return self.list_collection_mounts_endpoint.call_with_http_info(**kwargs)
 
     def mount_collection(
         self,
         *,
         virtual_instance_id: str,
         collection_paths: typing.Sequence[str] = None,
-        type: str = None,
         **kwargs
     ) -> typing.Union[CreateCollectionMountsResponse, asyncio.Future]:
-        """Mount Collection  # noqa: E501
+        """Mount Collections  # noqa: E501
 
         [beta] Mount a collection to this virtual instance.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         ```python
         rs = RocksetClient(api_key=APIKEY)
         future = rs.VirtualInstances.mount_collection(
             virtual_instance_id="virtualInstanceId_example",
             collection_paths=["commons.foo","commons.bar"],
-            type="STATIC",
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
             virtual_instance_id (str): Virtual Instance RRN. [required]
             collection_paths ([str]): Collections to mount.. [optional]
-            type (str): Mount type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1439,55 +1442,66 @@
         return self.mount_collection_endpoint.call_with_http_info(**kwargs)
 
     def query_virtual_instance(
         self,
         *,
         virtual_instance_id: str,
         sql: QueryRequestSql,
+        _async: bool = None,
         async_options: AsyncQueryOptions = None,
+        debug_threshold_ms: int = None,
+        max_initial_results: int = None,
+        timeout_ms: int = None,
         **kwargs
     ) -> typing.Union[QueryResponse, asyncio.Future]:
         """Execute SQL Query  # noqa: E501
 
         [beta] Make a SQL query to Rockset.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         ```python
         rs = RocksetClient(api_key=APIKEY)
         future = rs.VirtualInstances.query_virtual_instance(
             virtual_instance_id="virtualInstanceId_example",
+            _async=True,
             async_options=AsyncQueryOptions(
                 client_timeout_ms=1,
                 max_initial_results=1,
                 timeout_ms=1,
             ),
+            debug_threshold_ms=1,
+            max_initial_results=1,
             sql=QueryRequestSql(
                 default_row_limit=1,
                 generate_warnings=False,
                 initial_paginate_response_doc_count=1,
-                paginate=True,
                 parameters=[
                     QueryParameter(
                         name="_id",
                         type="string",
                         value="85beb391",
                     ),
                 ],
                 query="SELECT * FROM foo where _id = :_id",
             ),
+            timeout_ms=1,
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
             virtual_instance_id (str): Virtual Instance RRN. [required]
+            _async (bool): If true, the query will run asynchronously for up to 30 minutes. The query request will immediately return with a query id that can be used to retrieve the query status and results. If false or not specified, the query will return with results once completed or timeout after 2 minutes. (To return results directly for shorter queries while still allowing a timeout of up to 30 minutes, set `async_options.client_timeout_ms`.) . [optional]
             async_options (AsyncQueryOptions): [optional]
+            debug_threshold_ms (int): If query execution takes longer than this value, debug information will be logged. If the query text includes the DEBUG hint and this parameter is also provided, only this value will be used and the DEBUG hint will be ignored.. [optional]
+            max_initial_results (int): This limits the maximum number of results in the initial response. A pagination cursor is returned if the number of results exceeds `max_initial_results`. If `max_initial_results` is not set, all results will be returned in the initial response up to 4 million. If `max_initial_results` is set, the value must be between 0 and 100,000. If the query is async and `client_timeout_ms` is exceeded, `max_initial_results` does not apply since none of the results will be returned with the initial response.. [optional]
             sql (QueryRequestSql): [required]
+            timeout_ms (int): If a query exceeds the specified timeout, the query will automatically stop and return an error. The query timeout defaults to a maximum of 2 minutes. If `async` is true, the query timeout defaults to a maximum of 30 minutes.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -1808,49 +1822,59 @@
             collection_path
         return self.unmount_collection_endpoint.call_with_http_info(**kwargs)
 
     def update(
         self,
         *,
         virtual_instance_id: str,
+        auto_scaling_policy: AutoScalingPolicy = None,
         auto_suspend_enabled: bool = None,
         auto_suspend_seconds: int = None,
         description: str = None,
-        monitoring_enabled: bool = None,
+        enable_remount_on_resume: bool = None,
+        mount_refresh_interval_seconds: int = None,
         name: str = None,
         new_size: str = None,
         **kwargs
     ) -> typing.Union[UpdateVirtualInstanceResponse, asyncio.Future]:
         """Update Virtual Instance  # noqa: E501
 
         Update the properties of a virtual instance.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         ```python
         rs = RocksetClient(api_key=APIKEY)
         future = rs.VirtualInstances.update(
             virtual_instance_id="virtualInstanceId_example",
+            auto_scaling_policy=AutoScalingPolicy(
+                enabled=True,
+                max_size="XLARGE2",
+                min_size="LARGE",
+            ),
             auto_suspend_enabled=True,
             auto_suspend_seconds=3600,
             description="VI for prod traffic",
-            monitoring_enabled=True,
+            enable_remount_on_resume=True,
+            mount_refresh_interval_seconds=3600,
             name="prod_vi",
             new_size="LARGE",
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
             virtual_instance_id (str): Virtual Instance RRN. [required]
+            auto_scaling_policy (AutoScalingPolicy): [optional]
             auto_suspend_enabled (bool): Whether auto-suspend should be enabled for this Virtual Instance.. [optional]
             auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]
             description (str): New virtual instance description.. [optional]
-            monitoring_enabled (bool): [optional]
+            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]
+            mount_refresh_interval_seconds (int): Number of seconds between data refreshes for mounts on this Virtual Instance. A value of 0 means continuous refresh and a value of null means never refresh.. [optional]
             name (str): New virtual instance name.. [optional]
             new_size (str): Requested virtual instance size.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
```

### Comparing `rockset-2.0.0/rockset/api/workspaces_api.py` & `rockset-2.0.2/rockset/api/workspaces_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/api_client.py` & `rockset-2.0.2/rockset/api_client.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/apis/__init__.py` & `rockset-2.0.2/rockset/apis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,11 +20,12 @@
 from rockset.api.custom_roles_api import CustomRoles
 from rockset.api.documents_api import Documents
 from rockset.api.integrations_api import Integrations
 from rockset.api.organizations_api import Organizations
 from rockset.api.queries_api import Queries
 from rockset.api.query_lambdas_api import QueryLambdas
 from rockset.api.shared_lambdas_api import SharedLambdas
+from rockset.api.sources_api import Sources
 from rockset.api.users_api import Users
 from rockset.api.views_api import Views
 from rockset.api.virtual_instances_api import VirtualInstances
 from rockset.api.workspaces_api import Workspaces
```

### Comparing `rockset-2.0.0/rockset/configuration.py` & `rockset-2.0.2/rockset/configuration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/document.py` & `rockset-2.0.2/rockset/document.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/exceptions.py` & `rockset-2.0.2/rockset/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/add_documents_request.py` & `rockset-2.0.2/rockset/model/add_documents_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/add_documents_response.py` & `rockset-2.0.2/rockset/model/add_documents_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/alias.py` & `rockset-2.0.2/rockset/model/alias.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,15 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'collections': ([str], none_type),  # noqa: E501
             'created_at': (str, none_type),  # noqa: E501
+            'created_by_apikey_name': (str, none_type),  # noqa: E501
             'creator_email': (str, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'modified_at': (str, none_type),  # noqa: E501
             'name': (str, none_type),  # noqa: E501
             'state': (str, none_type),  # noqa: E501
             'workspace': (str, none_type),  # noqa: E501
         }
@@ -99,14 +100,15 @@
     def discriminator():
         return None
 
 
     attribute_map = {
         'collections': 'collections',  # noqa: E501
         'created_at': 'created_at',  # noqa: E501
+        'created_by_apikey_name': 'created_by_apikey_name',  # noqa: E501
         'creator_email': 'creator_email',  # noqa: E501
         'description': 'description',  # noqa: E501
         'modified_at': 'modified_at',  # noqa: E501
         'name': 'name',  # noqa: E501
         'state': 'state',  # noqa: E501
         'workspace': 'workspace',  # noqa: E501
     }
@@ -150,14 +152,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             collections ([str]): List of fully qualified collection names referenced by alias.. [optional]  # noqa: E501
             created_at (str): ISO-8601 date.. [optional]  # noqa: E501
+            created_by_apikey_name (str): Name of the API key that was used to create this object if one was used.. [optional]  # noqa: E501
             creator_email (str): Email of the creator.. [optional]  # noqa: E501
             description (str): Alias description.. [optional]  # noqa: E501
             modified_at (str): ISO-8601 date.. [optional]  # noqa: E501
             name (str): Name of the alias.. [optional]  # noqa: E501
             state (str): State of the alias.. [optional]  # noqa: E501
             workspace (str): Name of the workspace.. [optional]  # noqa: E501
         """
@@ -209,14 +212,15 @@
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
         """Alias - a model defined in OpenAPI
 
         Keyword Args:
             collections ([str]): List of fully qualified collection names referenced by alias.. [optional]  # noqa: E501
             created_at (str): ISO-8601 date.. [optional]  # noqa: E501
+            created_by_apikey_name (str): Name of the API key that was used to create this object if one was used.. [optional]  # noqa: E501
             creator_email (str): Email of the creator.. [optional]  # noqa: E501
             description (str): Alias description.. [optional]  # noqa: E501
             modified_at (str): ISO-8601 date.. [optional]  # noqa: E501
             name (str): Name of the alias.. [optional]  # noqa: E501
             state (str): State of the alias.. [optional]  # noqa: E501
             workspace (str): Name of the workspace.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
```

### Comparing `rockset-2.0.0/rockset/model/api_key.py` & `rockset-2.0.2/rockset/model/api_key.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,14 +85,15 @@
                 and the value is attribute type.
         """
         return {
             'key': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'created_at': (str, none_type),  # noqa: E501
             'created_by': (str, none_type),  # noqa: E501
+            'created_by_apikey_name': (str, none_type),  # noqa: E501
             'expiry_time': (str, none_type),  # noqa: E501
             'last_access_time': (str, none_type),  # noqa: E501
             'role': (str, none_type),  # noqa: E501
             'state': (str, none_type),  # noqa: E501
         }
 
     @cached_property
@@ -101,14 +102,15 @@
 
 
     attribute_map = {
         'key': 'key',  # noqa: E501
         'name': 'name',  # noqa: E501
         'created_at': 'created_at',  # noqa: E501
         'created_by': 'created_by',  # noqa: E501
+        'created_by_apikey_name': 'created_by_apikey_name',  # noqa: E501
         'expiry_time': 'expiry_time',  # noqa: E501
         'last_access_time': 'last_access_time',  # noqa: E501
         'role': 'role',  # noqa: E501
         'state': 'state',  # noqa: E501
     }
 
     read_only_vars = {
@@ -118,15 +120,15 @@
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, key, name, *args, **kwargs):  # noqa: E501
         """ApiKey - a model defined in OpenAPI
 
         Args:
-            key (str): API key string of 64 alphanumeric characters.
+            key (str): This field will only be populated with the full key when creating an API key. Otherwise, it will be an API key identifier of 6 characters.
             name (str): Name of the API key.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -154,14 +156,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             created_at (str): Date that API key was created (ISO-8601 format).. [optional]  # noqa: E501
             created_by (str): Email of API key owner.. [optional]  # noqa: E501
+            created_by_apikey_name (str): Name of the API key that was used to create this object if one was used.. [optional]  # noqa: E501
             expiry_time (str): The expiration date of this API key.. [optional]  # noqa: E501
             last_access_time (str): Date that API key was most recently used (ISO-8601 format).. [optional]  # noqa: E501
             role (str): Role specifying access control. If not specified, API key will have access to all of the associated user's roles.. [optional]  # noqa: E501
             state (str): Current state of this key.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
@@ -211,18 +214,19 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, key, name, **kwargs):  # noqa: E501
         """ApiKey - a model defined in OpenAPI
 
         Keyword Args:
-            key (str): API key string of 64 alphanumeric characters.
+            key (str): This field will only be populated with the full key when creating an API key. Otherwise, it will be an API key identifier of 6 characters.
             name (str): Name of the API key.
             created_at (str): Date that API key was created (ISO-8601 format).. [optional]  # noqa: E501
             created_by (str): Email of API key owner.. [optional]  # noqa: E501
+            created_by_apikey_name (str): Name of the API key that was used to create this object if one was used.. [optional]  # noqa: E501
             expiry_time (str): The expiration date of this API key.. [optional]  # noqa: E501
             last_access_time (str): Date that API key was most recently used (ISO-8601 format).. [optional]  # noqa: E501
             role (str): Role specifying access control. If not specified, API key will have access to all of the associated user's roles.. [optional]  # noqa: E501
             state (str): Current state of this key.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
```

### Comparing `rockset-2.0.0/rockset/model/async_query_options.py` & `rockset-2.0.2/rockset/model/async_query_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,17 +134,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            client_timeout_ms (int): The maximum amount of time that the client is willing to wait for the query to complete. If the query is not complete by this timeout, a response will be returned with a `query_id` that can be used to check the status of the query and retrieve results once the query has completed.. [optional]  # noqa: E501
-            max_initial_results (int): The maximum number of results you will receive as a client. If the query exceeds this limit, the remaining results can be requested using a returned pagination cursor. In addition, there is a maximum response size of 100MiB so fewer than `max_results` may be returned.. [optional]  # noqa: E501
-            timeout_ms (int): The maximum amount of time that the system will attempt to complete query execution before aborting the query and returning an error.. [optional]  # noqa: E501
+            client_timeout_ms (int): If the query completes before the client timeout, the results are returned. Otherwise if the client timeout is exceeded, the query id will be returned, and the query will continue to run in the background for up to 30 minutes. (The 30 minute timeout can be configured lower with timeout_ms.) `async_options.client_timeout_ms` only applies when `async` is true. The default value of `client_timeout_ms` is 0, so async query requests will immediately return with a query id by default. . [optional]  # noqa: E501
+            max_initial_results (int): [DEPRECATED] Use the query request `max_initial_results` instead. The maximum number of results you will receive as a client. If the query exceeds this limit, the remaining results can be requested using a returned pagination cursor. In addition, there is a maximum response size of 100MiB so fewer than `max_results` may be returned.. [optional]  # noqa: E501
+            timeout_ms (int): [DEPRECATED] Use the query request `timeout_ms` instead. The maximum amount of time that the system will attempt to complete query execution before aborting the query and returning an error. This must be set to a value that is greater than or equal to the client timeout, and the maximum value of this timeout is 30 minutes.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,17 +188,17 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
         """AsyncQueryOptions - a model defined in OpenAPI
 
         Keyword Args:
-            client_timeout_ms (int): The maximum amount of time that the client is willing to wait for the query to complete. If the query is not complete by this timeout, a response will be returned with a `query_id` that can be used to check the status of the query and retrieve results once the query has completed.. [optional]  # noqa: E501
-            max_initial_results (int): The maximum number of results you will receive as a client. If the query exceeds this limit, the remaining results can be requested using a returned pagination cursor. In addition, there is a maximum response size of 100MiB so fewer than `max_results` may be returned.. [optional]  # noqa: E501
-            timeout_ms (int): The maximum amount of time that the system will attempt to complete query execution before aborting the query and returning an error.. [optional]  # noqa: E501
+            client_timeout_ms (int): If the query completes before the client timeout, the results are returned. Otherwise if the client timeout is exceeded, the query id will be returned, and the query will continue to run in the background for up to 30 minutes. (The 30 minute timeout can be configured lower with timeout_ms.) `async_options.client_timeout_ms` only applies when `async` is true. The default value of `client_timeout_ms` is 0, so async query requests will immediately return with a query id by default. . [optional]  # noqa: E501
+            max_initial_results (int): [DEPRECATED] Use the query request `max_initial_results` instead. The maximum number of results you will receive as a client. If the query exceeds this limit, the remaining results can be requested using a returned pagination cursor. In addition, there is a maximum response size of 100MiB so fewer than `max_results` may be returned.. [optional]  # noqa: E501
+            timeout_ms (int): [DEPRECATED] Use the query request `timeout_ms` instead. The maximum amount of time that the system will attempt to complete query execution before aborting the query and returning an error. This must be set to a value that is greater than or equal to the client timeout, and the maximum value of this timeout is 30 minutes.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/aws_access_key.py` & `rockset-2.0.2/rockset/model/aws_access_key.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/aws_role.py` & `rockset-2.0.2/rockset/model/aws_role.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/azure_blob_storage_collection_creation_request.py` & `rockset-2.0.2/rockset/model/file_upload_collection_creation_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,27 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.azure_blob_storage_source_wrapper import AzureBlobStorageSourceWrapper
     from rockset.model.event_time_info import EventTimeInfo
     from rockset.model.field_mapping_query import FieldMappingQuery
     from rockset.model.field_mapping_v2 import FieldMappingV2
     from rockset.model.field_partition import FieldPartition
-    globals()['AzureBlobStorageSourceWrapper'] = AzureBlobStorageSourceWrapper
+    from rockset.model.file_upload_source_wrapper import FileUploadSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
     globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
+    globals()['FileUploadSourceWrapper'] = FileUploadSourceWrapper
 
 
-class AzureBlobStorageCollectionCreationRequest(ModelNormal):
+class FileUploadCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -101,15 +101,15 @@
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
             'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([AzureBlobStorageSourceWrapper], none_type),  # noqa: E501
+            'sources': ([FileUploadSourceWrapper], none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -128,15 +128,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """AzureBlobStorageCollectionCreationRequest - a model defined in OpenAPI
+        """FileUploadCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -170,15 +170,15 @@
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
             field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([AzureBlobStorageSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([FileUploadSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +220,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """AzureBlobStorageCollectionCreationRequest - a model defined in OpenAPI
+        """FileUploadCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
             field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([AzureBlobStorageSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([FileUploadSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/azure_blob_storage_integration.py` & `rockset-2.0.2/rockset/model/azure_blob_storage_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/azure_blob_storage_integration_creation_request.py` & `rockset-2.0.2/rockset/model/azure_blob_storage_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/azure_blob_storage_source_wrapper.py` & `rockset-2.0.2/rockset/model/azure_blob_storage_source_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,15 @@
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from rockset.model.format_params import FormatParams
-    from rockset.model.status import Status
     globals()['FormatParams'] = FormatParams
-    globals()['Status'] = Status
 
 
 class AzureBlobStorageSourceWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -88,15 +86,14 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'format_params': (FormatParams, none_type),  # noqa: E501
             'integration_name': (str, none_type),  # noqa: E501
-            'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
             'blob_bytes_total': (int, none_type),  # noqa: E501
             'blob_count_downloaded': (int, none_type),  # noqa: E501
             'blob_count_total': (int, none_type),  # noqa: E501
             'container': (str, none_type),  # noqa: E501
             'pattern': (str, none_type),  # noqa: E501
             'prefix': (str, none_type),  # noqa: E501
         }
@@ -105,25 +102,23 @@
     def discriminator():
         return None
 
 
     attribute_map = {
         'format_params': 'format_params',  # noqa: E501
         'integration_name': 'integration_name',  # noqa: E501
-        'status': 'status',  # noqa: E501
         'blob_bytes_total': 'blob_bytes_total',  # noqa: E501
         'blob_count_downloaded': 'blob_count_downloaded',  # noqa: E501
         'blob_count_total': 'blob_count_total',  # noqa: E501
         'container': 'container',  # noqa: E501
         'pattern': 'pattern',  # noqa: E501
         'prefix': 'prefix',  # noqa: E501
     }
 
     read_only_vars = {
-        'status',  # noqa: E501
         'blob_bytes_total',  # noqa: E501
         'blob_count_downloaded',  # noqa: E501
         'blob_count_total',  # noqa: E501
     }
 
     _composed_schemas = {}
 
@@ -161,15 +156,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             format_params (FormatParams): [optional]  # noqa: E501
             integration_name (str): Name of integration to use.. [optional]  # noqa: E501
-            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             blob_bytes_total (int): [optional]  # noqa: E501
             blob_count_downloaded (int): [optional]  # noqa: E501
             blob_count_total (int): [optional]  # noqa: E501
             container (str): Name of Azure blob Storage container you want to ingest from.. [optional]  # noqa: E501
             pattern (str): Glob-style pattern that selects keys to ingest. Only either prefix or pattern can be specified.. [optional]  # noqa: E501
             prefix (str): Prefix that selects blobs to ingest.. [optional]  # noqa: E501
         """
```

### Comparing `rockset-2.0.0/rockset/model/azure_event_hubs_collection_creation_request.py` & `rockset-2.0.2/rockset/model/snowflake_collection_creation_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,27 +26,25 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.azure_event_hubs_source_wrapper import AzureEventHubsSourceWrapper
     from rockset.model.event_time_info import EventTimeInfo
     from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
     from rockset.model.field_partition import FieldPartition
-    globals()['AzureEventHubsSourceWrapper'] = AzureEventHubsSourceWrapper
+    from rockset.model.snowflake_source_wrapper import SnowflakeSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
+    globals()['SnowflakeSourceWrapper'] = SnowflakeSourceWrapper
 
 
-class AzureEventHubsCollectionCreationRequest(ModelNormal):
+class SnowflakeCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([AzureEventHubsSourceWrapper], none_type),  # noqa: E501
+            'sources': ([SnowflakeSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """AzureEventHubsCollectionCreationRequest - a model defined in OpenAPI
+        """SnowflakeCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([AzureEventHubsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([SnowflakeSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """AzureEventHubsCollectionCreationRequest - a model defined in OpenAPI
+        """SnowflakeCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([AzureEventHubsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([SnowflakeSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/azure_event_hubs_integration.py` & `rockset-2.0.2/rockset/model/azure_event_hubs_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/azure_event_hubs_integration_creation_request.py` & `rockset-2.0.2/rockset/model/azure_event_hubs_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/azure_event_hubs_source_wrapper.py` & `rockset-2.0.2/rockset/model/azure_event_hubs_source_wrapper.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -92,30 +92,30 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'format_params': (FormatParams, none_type),  # noqa: E501
             'integration_name': (str, none_type),  # noqa: E501
-            'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
             'hub_id': (str, none_type),  # noqa: E501
             'offset_reset_policy': (str, none_type),  # noqa: E501
+            'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'format_params': 'format_params',  # noqa: E501
         'integration_name': 'integration_name',  # noqa: E501
-        'status': 'status',  # noqa: E501
         'hub_id': 'hub_id',  # noqa: E501
         'offset_reset_policy': 'offset_reset_policy',  # noqa: E501
+        'status': 'status',  # noqa: E501
     }
 
     read_only_vars = {
         'status',  # noqa: E501
     }
 
     _composed_schemas = {}
@@ -154,17 +154,17 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             format_params (FormatParams): [optional]  # noqa: E501
             integration_name (str): Name of integration to use.. [optional]  # noqa: E501
-            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             hub_id (str): Name of the hub which rockset should ingest from.. [optional]  # noqa: E501
             offset_reset_policy (str): The offset reset policy.. [optional]  # noqa: E501
+            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `rockset-2.0.0/rockset/model/azure_service_bus_collection_creation_request.py` & `rockset-2.0.2/rockset/model/azure_blob_storage_collection_creation_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,27 +26,25 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.azure_service_bus_source_wrapper import AzureServiceBusSourceWrapper
+    from rockset.model.azure_blob_storage_source_wrapper import AzureBlobStorageSourceWrapper
     from rockset.model.event_time_info import EventTimeInfo
     from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
     from rockset.model.field_partition import FieldPartition
-    globals()['AzureServiceBusSourceWrapper'] = AzureServiceBusSourceWrapper
+    globals()['AzureBlobStorageSourceWrapper'] = AzureBlobStorageSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
 
 
-class AzureServiceBusCollectionCreationRequest(ModelNormal):
+class AzureBlobStorageCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([AzureServiceBusSourceWrapper], none_type),  # noqa: E501
+            'sources': ([AzureBlobStorageSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """AzureServiceBusCollectionCreationRequest - a model defined in OpenAPI
+        """AzureBlobStorageCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([AzureServiceBusSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([AzureBlobStorageSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """AzureServiceBusCollectionCreationRequest - a model defined in OpenAPI
+        """AzureBlobStorageCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([AzureServiceBusSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([AzureBlobStorageSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/azure_service_bus_integration.py` & `rockset-2.0.2/rockset/model/azure_service_bus_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/azure_service_bus_source_wrapper.py` & `rockset-2.0.2/rockset/model/azure_service_bus_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/bulk_stats.py` & `rockset-2.0.2/rockset/model/bulk_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/cancel_query_response.py` & `rockset-2.0.2/rockset/model/cancel_query_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/cluster.py` & `rockset-2.0.2/rockset/model/cluster.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/collection.py` & `rockset-2.0.2/rockset/model/collection.py`

 * *Files 9% similar despite different names*

```diff
@@ -118,14 +118,15 @@
         lazy_import()
         return {
             'aliases': ([Alias], none_type),  # noqa: E501
             'bulk_stats': ([BulkStats], none_type),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'created_at': (str, none_type),  # noqa: E501
             'created_by': (str, none_type),  # noqa: E501
+            'created_by_apikey_name': (str, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
             'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'insert_only': (bool, none_type),  # noqa: E501
             'name': (str, none_type),  # noqa: E501
             'read_only': (bool, none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
@@ -142,14 +143,15 @@
 
     attribute_map = {
         'aliases': 'aliases',  # noqa: E501
         'bulk_stats': 'bulk_stats',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'created_at': 'created_at',  # noqa: E501
         'created_by': 'created_by',  # noqa: E501
+        'created_by_apikey_name': 'created_by_apikey_name',  # noqa: E501
         'description': 'description',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
         'field_mappings': 'field_mappings',  # noqa: E501
         'insert_only': 'insert_only',  # noqa: E501
         'name': 'name',  # noqa: E501
         'read_only': 'read_only',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
@@ -201,14 +203,15 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             aliases ([Alias]): List of aliases for a collection.. [optional]  # noqa: E501
             bulk_stats ([BulkStats]): [optional]  # noqa: E501
             clustering_key ([FieldPartition]): List of clustering fields for a collection.. [optional]  # noqa: E501
             created_at (str): ISO-8601 date.. [optional]  # noqa: E501
             created_by (str): Email of user who created the collection.. [optional]  # noqa: E501
+            created_by_apikey_name (str): Name of the API key that was used to create this collection if one was used.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
             field_mappings ([FieldMappingV2]): List of mappings applied on all documents in a collection.. [optional]  # noqa: E501
             insert_only (bool): Whether the collection is insert only or not.. [optional]  # noqa: E501
             name (str): Unique identifer for collection, can contain alphanumeric or dash characters.. [optional]  # noqa: E501
             read_only (bool): Whether the collection is read-only or not.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged based on event time.. [optional]  # noqa: E501
@@ -268,14 +271,15 @@
 
         Keyword Args:
             aliases ([Alias]): List of aliases for a collection.. [optional]  # noqa: E501
             bulk_stats ([BulkStats]): [optional]  # noqa: E501
             clustering_key ([FieldPartition]): List of clustering fields for a collection.. [optional]  # noqa: E501
             created_at (str): ISO-8601 date.. [optional]  # noqa: E501
             created_by (str): Email of user who created the collection.. [optional]  # noqa: E501
+            created_by_apikey_name (str): Name of the API key that was used to create this collection if one was used.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
             field_mappings ([FieldMappingV2]): List of mappings applied on all documents in a collection.. [optional]  # noqa: E501
             insert_only (bool): Whether the collection is insert only or not.. [optional]  # noqa: E501
             name (str): Unique identifer for collection, can contain alphanumeric or dash characters.. [optional]  # noqa: E501
             read_only (bool): Whether the collection is read-only or not.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged based on event time.. [optional]  # noqa: E501
```

### Comparing `rockset-2.0.0/rockset/model/collection_mount.py` & `rockset-2.0.2/rockset/model/collection_mount.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,18 +61,17 @@
     allowed_values = {
         ('state',): {
             'CREATING': "CREATING",
             'ACTIVE': "ACTIVE",
             'REFRESHING': "REFRESHING",
             'EXPIRED': "EXPIRED",
             'DELETING': "DELETING",
-        },
-        ('type',): {
-            'STATIC': "STATIC",
-            'LIVE': "LIVE",
+            'SWITCHING_REFRESH_TYPE': "SWITCHING_REFRESH_TYPE",
+            'SUSPENDED': "SUSPENDED",
+            'SUSPENDING': "SUSPENDING",
         },
     }
 
     validations = {
     }
 
     @cached_property
@@ -97,37 +96,37 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'collection_path': (str, none_type),  # noqa: E501
             'created_at': (str, none_type),  # noqa: E501
             'id': (str, none_type),  # noqa: E501
+            'last_refresh_time_millis': (int, none_type),  # noqa: E501
             'rrn': (str, none_type),  # noqa: E501
             'snapshot_expiration_time_millis': (int, none_type),  # noqa: E501
             'state': (str, none_type),  # noqa: E501
             'stats': (CollectionMountStats, none_type),  # noqa: E501
-            'type': (str, none_type),  # noqa: E501
             'virtual_instance_id': (str, none_type),  # noqa: E501
             'virtual_instance_rrn': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'collection_path': 'collection_path',  # noqa: E501
         'created_at': 'created_at',  # noqa: E501
         'id': 'id',  # noqa: E501
+        'last_refresh_time_millis': 'last_refresh_time_millis',  # noqa: E501
         'rrn': 'rrn',  # noqa: E501
         'snapshot_expiration_time_millis': 'snapshot_expiration_time_millis',  # noqa: E501
         'state': 'state',  # noqa: E501
         'stats': 'stats',  # noqa: E501
-        'type': 'type',  # noqa: E501
         'virtual_instance_id': 'virtual_instance_id',  # noqa: E501
         'virtual_instance_rrn': 'virtual_instance_rrn',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
@@ -168,19 +167,19 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             collection_path (str): Collection path.. [optional]  # noqa: E501
             created_at (str): ISO-8601 date.. [optional]  # noqa: E501
             id (str): Mount ID.. [optional]  # noqa: E501
+            last_refresh_time_millis (int): Unix timestamp of most recent refresh. Not applicable for live mounts.. [optional]  # noqa: E501
             rrn (str): Mount RRN.. [optional]  # noqa: E501
             snapshot_expiration_time_millis (int): Time in millis at which the snapshot expires.. [optional]  # noqa: E501
             state (str): Mount type.. [optional]  # noqa: E501
             stats (CollectionMountStats): [optional]  # noqa: E501
-            type (str): Mount type.. [optional]  # noqa: E501
             virtual_instance_id (str): Virtual instance ID.. [optional]  # noqa: E501
             virtual_instance_rrn (str): Virtual Instance RRN.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -229,19 +228,19 @@
     def __init__(self, **kwargs):  # noqa: E501
         """CollectionMount - a model defined in OpenAPI
 
         Keyword Args:
             collection_path (str): Collection path.. [optional]  # noqa: E501
             created_at (str): ISO-8601 date.. [optional]  # noqa: E501
             id (str): Mount ID.. [optional]  # noqa: E501
+            last_refresh_time_millis (int): Unix timestamp of most recent refresh. Not applicable for live mounts.. [optional]  # noqa: E501
             rrn (str): Mount RRN.. [optional]  # noqa: E501
             snapshot_expiration_time_millis (int): Time in millis at which the snapshot expires.. [optional]  # noqa: E501
             state (str): Mount type.. [optional]  # noqa: E501
             stats (CollectionMountStats): [optional]  # noqa: E501
-            type (str): Mount type.. [optional]  # noqa: E501
             virtual_instance_id (str): Virtual instance ID.. [optional]  # noqa: E501
             virtual_instance_rrn (str): Virtual Instance RRN.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `rockset-2.0.0/rockset/model/collection_mount_response.py` & `rockset-2.0.2/rockset/model/collection_mount_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/collection_mount_stats.py` & `rockset-2.0.2/rockset/model/collection_mount_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/collection_stats.py` & `rockset-2.0.2/rockset/model/collection_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_alias_request.py` & `rockset-2.0.2/rockset/model/create_alias_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_alias_response.py` & `rockset-2.0.2/rockset/model/create_alias_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_api_key_request.py` & `rockset-2.0.2/rockset/model/create_api_key_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_api_key_response.py` & `rockset-2.0.2/rockset/model/create_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_collection_mount_request.py` & `rockset-2.0.2/rockset/model/create_collection_mount_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,18 +51,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
-        ('type',): {
-            'STATIC': "STATIC",
-            'LIVE': "LIVE",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -82,25 +78,23 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'collection_paths': ([str], none_type),  # noqa: E501
-            'type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'collection_paths': 'collection_paths',  # noqa: E501
-        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -137,15 +131,14 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             collection_paths ([str]): Collections to mount.. [optional]  # noqa: E501
-            type (str): Mount type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -190,15 +183,14 @@
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
         """CreateCollectionMountRequest - a model defined in OpenAPI
 
         Keyword Args:
             collection_paths ([str]): Collections to mount.. [optional]  # noqa: E501
-            type (str): Mount type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/create_collection_mounts_response.py` & `rockset-2.0.2/rockset/model/create_collection_mounts_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_collection_request.py` & `rockset-2.0.2/rockset/model/create_collection_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,19 +28,17 @@
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from rockset.model.event_time_info import EventTimeInfo
     from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
     from rockset.model.field_partition import FieldPartition
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
 
 
 class CreateCollectionRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -61,14 +59,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -96,32 +98,32 @@
         """
         lazy_import()
         return {
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'name': (str, none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'name': 'name',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -161,17 +163,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -219,17 +221,17 @@
         """CreateCollectionRequest - a model defined in OpenAPI
 
         Keyword Args:
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/create_collection_response.py` & `rockset-2.0.2/rockset/model/create_collection_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_integration_request.py` & `rockset-2.0.2/rockset/model/create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_integration_response.py` & `rockset-2.0.2/rockset/model/create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_query_lambda_request.py` & `rockset-2.0.2/rockset/model/create_query_lambda_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_query_lambda_tag_request.py` & `rockset-2.0.2/rockset/model/create_query_lambda_tag_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_role_request.py` & `rockset-2.0.2/rockset/model/create_role_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_user_request.py` & `rockset-2.0.2/rockset/model/create_user_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_user_response.py` & `rockset-2.0.2/rockset/model/create_user_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_view_request.py` & `rockset-2.0.2/rockset/model/create_view_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_view_response.py` & `rockset-2.0.2/rockset/model/create_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_virtual_instance_request.py` & `rockset-2.0.2/rockset/model/update_user_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 
-class CreateVirtualInstanceRequest(ModelNormal):
+class UpdateUserRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,28 +51,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
-        ('type',): {
-            'FREE': "FREE",
-            'NANO': "NANO",
-            'SHARED': "SHARED",
-            'MILLI': "MILLI",
-            'SMALL': "SMALL",
-            'MEDIUM': "MEDIUM",
-            'LARGE': "LARGE",
-            'XLARGE': "XLARGE",
-            'XLARGE2': "XLARGE2",
-            'XLARGE4': "XLARGE4",
-            'XLARGE8': "XLARGE8",
-            'XLARGE16': "XLARGE16",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -91,44 +77,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'name': (str,),  # noqa: E501
-            'auto_suspend_seconds': (int, none_type),  # noqa: E501
-            'description': (str, none_type),  # noqa: E501
-            'type': (str, none_type),  # noqa: E501
+            'first_name': (str, none_type),  # noqa: E501
+            'last_name': (str, none_type),  # noqa: E501
+            'roles': ([str], none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'name': 'name',  # noqa: E501
-        'auto_suspend_seconds': 'auto_suspend_seconds',  # noqa: E501
-        'description': 'description',  # noqa: E501
-        'type': 'type',  # noqa: E501
+        'first_name': 'first_name',  # noqa: E501
+        'last_name': 'last_name',  # noqa: E501
+        'roles': 'roles',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """CreateVirtualInstanceRequest - a model defined in OpenAPI
-
-        Args:
-            name (str): Unique identifier for virtual instance, can contain alphanumeric or dash characters.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """UpdateUserRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -153,17 +134,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
-            description (str): Description of requested virtual instance.. [optional]  # noqa: E501
-            type (str): Requested virtual instance type.. [optional]  # noqa: E501
+            first_name (str): User first name.. [optional]  # noqa: E501
+            last_name (str): User last name.. [optional]  # noqa: E501
+            roles ([str]): New list of roles for a given user.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +164,14 @@
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
@@ -204,22 +184,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *, name, **kwargs):  # noqa: E501
-        """CreateVirtualInstanceRequest - a model defined in OpenAPI
+    def __init__(self, **kwargs):  # noqa: E501
+        """UpdateUserRequest - a model defined in OpenAPI
 
         Keyword Args:
-            name (str): Unique identifier for virtual instance, can contain alphanumeric or dash characters.
-            auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
-            description (str): Description of requested virtual instance.. [optional]  # noqa: E501
-            type (str): Requested virtual instance type.. [optional]  # noqa: E501
+            first_name (str): User first name.. [optional]  # noqa: E501
+            last_name (str): User last name.. [optional]  # noqa: E501
+            roles ([str]): New list of roles for a given user.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -268,15 +247,14 @@
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

### Comparing `rockset-2.0.0/rockset/model/create_virtual_instance_response.py` & `rockset-2.0.2/rockset/model/create_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_workspace_request.py` & `rockset-2.0.2/rockset/model/create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/create_workspace_response.py` & `rockset-2.0.2/rockset/model/create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/csv_params.py` & `rockset-2.0.2/rockset/model/csv_params.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/delete_alias_response.py` & `rockset-2.0.2/rockset/model/delete_alias_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/delete_api_key_response.py` & `rockset-2.0.2/rockset/model/delete_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/delete_collection_response.py` & `rockset-2.0.2/rockset/model/delete_collection_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/delete_documents_request.py` & `rockset-2.0.2/rockset/model/delete_documents_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/delete_documents_request_data.py` & `rockset-2.0.2/rockset/model/delete_documents_request_data.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/delete_documents_response.py` & `rockset-2.0.2/rockset/model/delete_documents_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/delete_integration_response.py` & `rockset-2.0.2/rockset/model/delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/delete_query_lambda_response.py` & `rockset-2.0.2/rockset/model/delete_query_lambda_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/delete_user_response.py` & `rockset-2.0.2/rockset/model/delete_user_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/delete_view_response.py` & `rockset-2.0.2/rockset/model/delete_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/delete_virtual_instance_response.py` & `rockset-2.0.2/rockset/model/delete_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/delete_workspace_response.py` & `rockset-2.0.2/rockset/model/delete_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/document_status.py` & `rockset-2.0.2/rockset/model/document_status.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/dynamodb_collection_creation_request.py` & `rockset-2.0.2/rockset/model/dynamodb_collection_creation_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,20 +29,18 @@
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from rockset.model.dynamodb_source_wrapper import DynamodbSourceWrapper
     from rockset.model.event_time_info import EventTimeInfo
     from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
     from rockset.model.field_partition import FieldPartition
     globals()['DynamodbSourceWrapper'] = DynamodbSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
 
 
 class DynamodbCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,33 +101,33 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
             'sources': ([DynamodbSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
             sources ([DynamodbSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -228,17 +230,17 @@
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
             sources ([DynamodbSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/dynamodb_integration.py` & `rockset-2.0.2/rockset/model/dynamodb_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/dynamodb_integration_creation_request.py` & `rockset-2.0.2/rockset/model/dynamodb_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/dynamodb_source_wrapper.py` & `rockset-2.0.2/rockset/model/dynamodb_source_wrapper.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -91,40 +91,40 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'table_name': (str,),  # noqa: E501
             'format_params': (FormatParams, none_type),  # noqa: E501
             'integration_name': (str, none_type),  # noqa: E501
-            'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
             'aws_region': (str, none_type),  # noqa: E501
             'current_status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
             'rcu': (int, none_type),  # noqa: E501
+            'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
             'use_scan_api': (bool, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'table_name': 'table_name',  # noqa: E501
         'format_params': 'format_params',  # noqa: E501
         'integration_name': 'integration_name',  # noqa: E501
-        'status': 'status',  # noqa: E501
         'aws_region': 'aws_region',  # noqa: E501
         'current_status': 'current_status',  # noqa: E501
         'rcu': 'rcu',  # noqa: E501
+        'status': 'status',  # noqa: E501
         'use_scan_api': 'use_scan_api',  # noqa: E501
     }
 
     read_only_vars = {
-        'status',  # noqa: E501
         'current_status',  # noqa: E501
+        'status',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, table_name, *args, **kwargs):  # noqa: E501
@@ -162,18 +162,18 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             format_params (FormatParams): [optional]  # noqa: E501
             integration_name (str): Name of integration to use.. [optional]  # noqa: E501
-            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             aws_region (str): AWS region name of DynamoDB table, by default us-west-2 is used.. [optional]  # noqa: E501
             current_status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             rcu (int): Max RCU usage for scan.. [optional]  # noqa: E501
+            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             use_scan_api (bool): Whether to use DynamoDB Scan API for the initial scan.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `rockset-2.0.0/rockset/model/error_model.py` & `rockset-2.0.2/rockset/model/error_model.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/event_time_info.py` & `rockset-2.0.2/rockset/model/event_time_info.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/execute_public_query_lambda_request.py` & `rockset-2.0.2/rockset/model/execute_public_query_lambda_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/execute_query_lambda_request.py` & `rockset-2.0.2/rockset/model/query_request_sql.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,21 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.async_query_options import AsyncQueryOptions
     from rockset.model.query_parameter import QueryParameter
-    globals()['AsyncQueryOptions'] = AsyncQueryOptions
     globals()['QueryParameter'] = QueryParameter
 
 
-class ExecuteQueryLambdaRequest(ModelNormal):
+class QueryRequestSql(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,47 +83,46 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'async_options': (AsyncQueryOptions, none_type),  # noqa: E501
+            'query': (str,),  # noqa: E501
             'default_row_limit': (int, none_type),  # noqa: E501
             'generate_warnings': (bool, none_type),  # noqa: E501
             'initial_paginate_response_doc_count': (int, none_type),  # noqa: E501
-            'paginate': (bool, none_type),  # noqa: E501
             'parameters': ([QueryParameter], none_type),  # noqa: E501
-            'virtual_instance_id': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'async_options': 'async_options',  # noqa: E501
+        'query': 'query',  # noqa: E501
         'default_row_limit': 'default_row_limit',  # noqa: E501
         'generate_warnings': 'generate_warnings',  # noqa: E501
         'initial_paginate_response_doc_count': 'initial_paginate_response_doc_count',  # noqa: E501
-        'paginate': 'paginate',  # noqa: E501
         'parameters': 'parameters',  # noqa: E501
-        'virtual_instance_id': 'virtual_instance_id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ExecuteQueryLambdaRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, query, *args, **kwargs):  # noqa: E501
+        """QueryRequestSql - a model defined in OpenAPI
+
+        Args:
+            query (str): SQL query string.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -150,21 +147,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            async_options (AsyncQueryOptions): [optional]  # noqa: E501
-            default_row_limit (int): Row limit to use if no limit specified in the SQL query text.. [optional]  # noqa: E501
-            generate_warnings (bool): Whether to generate warnings.. [optional]  # noqa: E501
-            initial_paginate_response_doc_count (int): Number of documents to return in addition to paginating for this query call. Only relevant if `paginate` flag is also set.. [optional]  # noqa: E501
-            paginate (bool): Flag to paginate and store the results of this query for later / sequential retrieval.. [optional]  # noqa: E501
+            default_row_limit (int): Row limit to use. Limits specified in the query text will override this default.. [optional]  # noqa: E501
+            generate_warnings (bool): Flag to enable warnings. Warnings can help debug query issues but negatively affect performance.. [optional]  # noqa: E501
+            initial_paginate_response_doc_count (int): [DEPRECATED] Use `max_initial_results` instead. Number of documents to return in addition to paginating for this query call. Only relevant if `paginate` flag is also set.. [optional]  # noqa: E501
             parameters ([QueryParameter]): List of named parameters.. [optional]  # noqa: E501
-            virtual_instance_id (str): Virtual instance on which to run the query.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -184,14 +178,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.query = query
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -204,25 +199,23 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, **kwargs):  # noqa: E501
-        """ExecuteQueryLambdaRequest - a model defined in OpenAPI
+    def __init__(self, *, query, **kwargs):  # noqa: E501
+        """QueryRequestSql - a model defined in OpenAPI
 
         Keyword Args:
-            async_options (AsyncQueryOptions): [optional]  # noqa: E501
-            default_row_limit (int): Row limit to use if no limit specified in the SQL query text.. [optional]  # noqa: E501
-            generate_warnings (bool): Whether to generate warnings.. [optional]  # noqa: E501
-            initial_paginate_response_doc_count (int): Number of documents to return in addition to paginating for this query call. Only relevant if `paginate` flag is also set.. [optional]  # noqa: E501
-            paginate (bool): Flag to paginate and store the results of this query for later / sequential retrieval.. [optional]  # noqa: E501
+            query (str): SQL query string.
+            default_row_limit (int): Row limit to use. Limits specified in the query text will override this default.. [optional]  # noqa: E501
+            generate_warnings (bool): Flag to enable warnings. Warnings can help debug query issues but negatively affect performance.. [optional]  # noqa: E501
+            initial_paginate_response_doc_count (int): [DEPRECATED] Use `max_initial_results` instead. Number of documents to return in addition to paginating for this query call. Only relevant if `paginate` flag is also set.. [optional]  # noqa: E501
             parameters ([QueryParameter]): List of named parameters.. [optional]  # noqa: E501
-            virtual_instance_id (str): Virtual instance on which to run the query.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -271,14 +264,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.query = query
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset-2.0.0/rockset/model/field_mapping_query.py` & `rockset-2.0.2/rockset/model/field_mapping_query.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/field_mapping_v2.py` & `rockset-2.0.2/rockset/model/field_mapping_v2.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/field_partition.py` & `rockset-2.0.2/rockset/model/field_partition.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/file_upload_collection_creation_request.py` & `rockset-2.0.2/rockset/model/kafka_collection_creation_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,25 +28,23 @@
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from rockset.model.event_time_info import EventTimeInfo
     from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
     from rockset.model.field_partition import FieldPartition
-    from rockset.model.file_upload_source_wrapper import FileUploadSourceWrapper
+    from rockset.model.kafka_source_wrapper import KafkaSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
-    globals()['FileUploadSourceWrapper'] = FileUploadSourceWrapper
+    globals()['KafkaSourceWrapper'] = KafkaSourceWrapper
 
 
-class FileUploadCollectionCreationRequest(ModelNormal):
+class KafkaCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([FileUploadSourceWrapper], none_type),  # noqa: E501
+            'sources': ([KafkaSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """FileUploadCollectionCreationRequest - a model defined in OpenAPI
+        """KafkaCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([FileUploadSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([KafkaSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """FileUploadCollectionCreationRequest - a model defined in OpenAPI
+        """KafkaCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([FileUploadSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([KafkaSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/file_upload_source_wrapper.py` & `rockset-2.0.2/rockset/model/file_upload_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/format_params.py` & `rockset-2.0.2/rockset/model/format_params.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/gcp_service_account.py` & `rockset-2.0.2/rockset/model/gcp_service_account.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/gcs_collection_creation_request.py` & `rockset-2.0.2/rockset/model/mongodb_collection_creation_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,25 +28,23 @@
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from rockset.model.event_time_info import EventTimeInfo
     from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
     from rockset.model.field_partition import FieldPartition
-    from rockset.model.gcs_source_wrapper import GcsSourceWrapper
+    from rockset.model.mongodb_source_wrapper import MongodbSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
-    globals()['GcsSourceWrapper'] = GcsSourceWrapper
+    globals()['MongodbSourceWrapper'] = MongodbSourceWrapper
 
 
-class GcsCollectionCreationRequest(ModelNormal):
+class MongodbCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([GcsSourceWrapper], none_type),  # noqa: E501
+            'sources': ([MongodbSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """GcsCollectionCreationRequest - a model defined in OpenAPI
+        """MongodbCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([GcsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([MongodbSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """GcsCollectionCreationRequest - a model defined in OpenAPI
+        """MongodbCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([GcsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([MongodbSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/gcs_integration.py` & `rockset-2.0.2/rockset/model/gcs_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/gcs_integration_creation_request.py` & `rockset-2.0.2/rockset/model/gcs_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/gcs_source_wrapper.py` & `rockset-2.0.2/rockset/model/gcs_source_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,15 @@
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from rockset.model.format_params import FormatParams
-    from rockset.model.status import Status
     globals()['FormatParams'] = FormatParams
-    globals()['Status'] = Status
 
 
 class GcsSourceWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -88,15 +86,14 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'format_params': (FormatParams, none_type),  # noqa: E501
             'integration_name': (str, none_type),  # noqa: E501
-            'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
             'bucket': (str, none_type),  # noqa: E501
             'object_bytes_downloaded': (int, none_type),  # noqa: E501
             'object_bytes_total': (int, none_type),  # noqa: E501
             'object_count_downloaded': (int, none_type),  # noqa: E501
             'object_count_total': (int, none_type),  # noqa: E501
             'pattern': (str, none_type),  # noqa: E501
             'prefix': (str, none_type),  # noqa: E501
@@ -106,26 +103,24 @@
     def discriminator():
         return None
 
 
     attribute_map = {
         'format_params': 'format_params',  # noqa: E501
         'integration_name': 'integration_name',  # noqa: E501
-        'status': 'status',  # noqa: E501
         'bucket': 'bucket',  # noqa: E501
         'object_bytes_downloaded': 'object_bytes_downloaded',  # noqa: E501
         'object_bytes_total': 'object_bytes_total',  # noqa: E501
         'object_count_downloaded': 'object_count_downloaded',  # noqa: E501
         'object_count_total': 'object_count_total',  # noqa: E501
         'pattern': 'pattern',  # noqa: E501
         'prefix': 'prefix',  # noqa: E501
     }
 
     read_only_vars = {
-        'status',  # noqa: E501
         'object_bytes_downloaded',  # noqa: E501
         'object_bytes_total',  # noqa: E501
         'object_count_downloaded',  # noqa: E501
         'object_count_total',  # noqa: E501
     }
 
     _composed_schemas = {}
@@ -164,15 +159,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             format_params (FormatParams): [optional]  # noqa: E501
             integration_name (str): Name of integration to use.. [optional]  # noqa: E501
-            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             bucket (str): Name of GCS bucket you want to ingest from.. [optional]  # noqa: E501
             object_bytes_downloaded (int): [optional]  # noqa: E501
             object_bytes_total (int): [optional]  # noqa: E501
             object_count_downloaded (int): [optional]  # noqa: E501
             object_count_total (int): [optional]  # noqa: E501
             pattern (str): Glob-style pattern that selects keys to ingest. Only either prefix or pattern can be specified.. [optional]  # noqa: E501
             prefix (str): Prefix that selects keys to ingest.. [optional]  # noqa: E501
```

### Comparing `rockset-2.0.0/rockset/model/get_alias_response.py` & `rockset-2.0.2/rockset/model/get_alias_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/get_api_key_response.py` & `rockset-2.0.2/rockset/model/get_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/get_collection_response.py` & `rockset-2.0.2/rockset/model/get_collection_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/get_integration_response.py` & `rockset-2.0.2/rockset/model/get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/get_query_response.py` & `rockset-2.0.2/rockset/model/get_query_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/get_view_response.py` & `rockset-2.0.2/rockset/model/get_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/get_virtual_instance_response.py` & `rockset-2.0.2/rockset/model/get_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/get_workspace_response.py` & `rockset-2.0.2/rockset/model/get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/input_field.py` & `rockset-2.0.2/rockset/model/input_field.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/integration.py` & `rockset-2.0.2/rockset/model/integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
             'created_by': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'azure_blob_storage': (AzureBlobStorageIntegration, none_type),  # noqa: E501
             'azure_event_hubs': (AzureEventHubsIntegration, none_type),  # noqa: E501
             'azure_service_bus': (AzureServiceBusIntegration, none_type),  # noqa: E501
             'collections': ([Collection], none_type),  # noqa: E501
             'created_at': (str, none_type),  # noqa: E501
+            'created_by_apikey_name': (str, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'dynamodb': (DynamodbIntegration, none_type),  # noqa: E501
             'gcs': (GcsIntegration, none_type),  # noqa: E501
             'kafka': (KafkaIntegration, none_type),  # noqa: E501
             'kinesis': (KinesisIntegration, none_type),  # noqa: E501
             'mongodb': (MongoDbIntegration, none_type),  # noqa: E501
             'owner_email': (str, none_type),  # noqa: E501
@@ -134,14 +135,15 @@
         'created_by': 'created_by',  # noqa: E501
         'name': 'name',  # noqa: E501
         'azure_blob_storage': 'azure_blob_storage',  # noqa: E501
         'azure_event_hubs': 'azure_event_hubs',  # noqa: E501
         'azure_service_bus': 'azure_service_bus',  # noqa: E501
         'collections': 'collections',  # noqa: E501
         'created_at': 'created_at',  # noqa: E501
+        'created_by_apikey_name': 'created_by_apikey_name',  # noqa: E501
         'description': 'description',  # noqa: E501
         'dynamodb': 'dynamodb',  # noqa: E501
         'gcs': 'gcs',  # noqa: E501
         'kafka': 'kafka',  # noqa: E501
         'kinesis': 'kinesis',  # noqa: E501
         'mongodb': 'mongodb',  # noqa: E501
         'owner_email': 'owner_email',  # noqa: E501
@@ -195,14 +197,15 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             azure_blob_storage (AzureBlobStorageIntegration): [optional]  # noqa: E501
             azure_event_hubs (AzureEventHubsIntegration): [optional]  # noqa: E501
             azure_service_bus (AzureServiceBusIntegration): [optional]  # noqa: E501
             collections ([Collection]): List of collections that use the integration.. [optional]  # noqa: E501
             created_at (str): ISO-8601 date.. [optional]  # noqa: E501
+            created_by_apikey_name (str): Name of the API key that was used to create this object if one was used.. [optional]  # noqa: E501
             description (str): Longer explanation for the integration.. [optional]  # noqa: E501
             dynamodb (DynamodbIntegration): [optional]  # noqa: E501
             gcs (GcsIntegration): [optional]  # noqa: E501
             kafka (KafkaIntegration): [optional]  # noqa: E501
             kinesis (KinesisIntegration): [optional]  # noqa: E501
             mongodb (MongoDbIntegration): [optional]  # noqa: E501
             owner_email (str): User that owns this integration.. [optional]  # noqa: E501
@@ -264,14 +267,15 @@
             created_by (str): Email of user who created the integration.
             name (str): Descriptive label and unique identifier.
             azure_blob_storage (AzureBlobStorageIntegration): [optional]  # noqa: E501
             azure_event_hubs (AzureEventHubsIntegration): [optional]  # noqa: E501
             azure_service_bus (AzureServiceBusIntegration): [optional]  # noqa: E501
             collections ([Collection]): List of collections that use the integration.. [optional]  # noqa: E501
             created_at (str): ISO-8601 date.. [optional]  # noqa: E501
+            created_by_apikey_name (str): Name of the API key that was used to create this object if one was used.. [optional]  # noqa: E501
             description (str): Longer explanation for the integration.. [optional]  # noqa: E501
             dynamodb (DynamodbIntegration): [optional]  # noqa: E501
             gcs (GcsIntegration): [optional]  # noqa: E501
             kafka (KafkaIntegration): [optional]  # noqa: E501
             kinesis (KinesisIntegration): [optional]  # noqa: E501
             mongodb (MongoDbIntegration): [optional]  # noqa: E501
             owner_email (str): User that owns this integration.. [optional]  # noqa: E501
```

### Comparing `rockset-2.0.0/rockset/model/kafka_collection_creation_request.py` & `rockset-2.0.2/rockset/model/azure_event_hubs_collection_creation_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,27 +26,25 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from rockset.model.azure_event_hubs_source_wrapper import AzureEventHubsSourceWrapper
     from rockset.model.event_time_info import EventTimeInfo
     from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
     from rockset.model.field_partition import FieldPartition
-    from rockset.model.kafka_source_wrapper import KafkaSourceWrapper
+    globals()['AzureEventHubsSourceWrapper'] = AzureEventHubsSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
-    globals()['KafkaSourceWrapper'] = KafkaSourceWrapper
 
 
-class KafkaCollectionCreationRequest(ModelNormal):
+class AzureEventHubsCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([KafkaSourceWrapper], none_type),  # noqa: E501
+            'sources': ([AzureEventHubsSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """KafkaCollectionCreationRequest - a model defined in OpenAPI
+        """AzureEventHubsCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([KafkaSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([AzureEventHubsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """KafkaCollectionCreationRequest - a model defined in OpenAPI
+        """AzureEventHubsCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([KafkaSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([AzureEventHubsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/kafka_integration.py` & `rockset-2.0.2/rockset/model/kafka_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/kafka_integration_creation_request.py` & `rockset-2.0.2/rockset/model/kafka_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/kafka_source_wrapper.py` & `rockset-2.0.2/rockset/model/kafka_source_wrapper.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -92,33 +92,33 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'format_params': (FormatParams, none_type),  # noqa: E501
             'integration_name': (str, none_type),  # noqa: E501
-            'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
             'consumer_group_id': (str, none_type),  # noqa: E501
             'kafka_topic_name': (str, none_type),  # noqa: E501
             'offset_reset_policy': (str, none_type),  # noqa: E501
+            'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
             'use_v3': (bool, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'format_params': 'format_params',  # noqa: E501
         'integration_name': 'integration_name',  # noqa: E501
-        'status': 'status',  # noqa: E501
         'consumer_group_id': 'consumer_group_id',  # noqa: E501
         'kafka_topic_name': 'kafka_topic_name',  # noqa: E501
         'offset_reset_policy': 'offset_reset_policy',  # noqa: E501
+        'status': 'status',  # noqa: E501
         'use_v3': 'use_v3',  # noqa: E501
     }
 
     read_only_vars = {
         'status',  # noqa: E501
     }
 
@@ -158,18 +158,18 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             format_params (FormatParams): [optional]  # noqa: E501
             integration_name (str): Name of integration to use.. [optional]  # noqa: E501
-            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             consumer_group_id (str): The Kafka consumer group Id being used.. [optional]  # noqa: E501
             kafka_topic_name (str): The Kafka topic to be tailed.. [optional]  # noqa: E501
             offset_reset_policy (str): The offset reset policy.. [optional]  # noqa: E501
+            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             use_v3 (bool): Whether to use v3 integration.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `rockset-2.0.0/rockset/model/kafka_v3_security_config.py` & `rockset-2.0.2/rockset/model/kafka_v3_security_config.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/kinesis_collection_creation_request.py` & `rockset-2.0.2/rockset/model/s3_collection_creation_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,25 +28,23 @@
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from rockset.model.event_time_info import EventTimeInfo
     from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
     from rockset.model.field_partition import FieldPartition
-    from rockset.model.kinesis_source_wrapper import KinesisSourceWrapper
+    from rockset.model.s3_source_wrapper import S3SourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
-    globals()['KinesisSourceWrapper'] = KinesisSourceWrapper
+    globals()['S3SourceWrapper'] = S3SourceWrapper
 
 
-class KinesisCollectionCreationRequest(ModelNormal):
+class S3CollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([KinesisSourceWrapper], none_type),  # noqa: E501
+            'sources': ([S3SourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """KinesisCollectionCreationRequest - a model defined in OpenAPI
+        """S3CollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([KinesisSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([S3SourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """KinesisCollectionCreationRequest - a model defined in OpenAPI
+        """S3CollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([KinesisSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([S3SourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/kinesis_integration.py` & `rockset-2.0.2/rockset/model/kinesis_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/kinesis_integration_creation_request.py` & `rockset-2.0.2/rockset/model/kinesis_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/kinesis_source_wrapper.py` & `rockset-2.0.2/rockset/model/kinesis_source_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,15 @@
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from rockset.model.format_params import FormatParams
-    from rockset.model.status import Status
     globals()['FormatParams'] = FormatParams
-    globals()['Status'] = Status
 
 
 class KinesisSourceWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -93,37 +91,34 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'stream_name': (str,),  # noqa: E501
             'format_params': (FormatParams, none_type),  # noqa: E501
             'integration_name': (str, none_type),  # noqa: E501
-            'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
             'aws_region': (str, none_type),  # noqa: E501
             'dms_primary_key': ([str], none_type),  # noqa: E501
             'offset_reset_policy': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'stream_name': 'stream_name',  # noqa: E501
         'format_params': 'format_params',  # noqa: E501
         'integration_name': 'integration_name',  # noqa: E501
-        'status': 'status',  # noqa: E501
         'aws_region': 'aws_region',  # noqa: E501
         'dms_primary_key': 'dms_primary_key',  # noqa: E501
         'offset_reset_policy': 'offset_reset_policy',  # noqa: E501
     }
 
     read_only_vars = {
-        'status',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, stream_name, *args, **kwargs):  # noqa: E501
@@ -161,15 +156,14 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             format_params (FormatParams): [optional]  # noqa: E501
             integration_name (str): Name of integration to use.. [optional]  # noqa: E501
-            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             aws_region (str): AWS region name of Kinesis stream, by default us-west-2 is used.. [optional]  # noqa: E501
             dms_primary_key ([str]): Set of fields that correspond to a DMS primary key.. [optional]  # noqa: E501
             offset_reset_policy (str): For non-DMS streams, Rockset can tail from the earliest end or latest end of kinesis source.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `rockset-2.0.0/rockset/model/list_aliases_response.py` & `rockset-2.0.2/rockset/model/list_aliases_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/list_api_keys_response.py` & `rockset-2.0.2/rockset/model/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/list_collection_mounts_response.py` & `rockset-2.0.2/rockset/model/list_collection_mounts_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/list_collections_response.py` & `rockset-2.0.2/rockset/model/list_collections_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/list_integrations_response.py` & `rockset-2.0.2/rockset/model/list_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/list_queries_response.py` & `rockset-2.0.2/rockset/model/list_queries_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/list_query_lambda_tags_response.py` & `rockset-2.0.2/rockset/model/list_query_lambda_tags_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/list_query_lambda_versions_response.py` & `rockset-2.0.2/rockset/model/list_query_lambda_versions_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/list_query_lambdas_response.py` & `rockset-2.0.2/rockset/model/list_query_lambdas_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/list_roles_response.py` & `rockset-2.0.2/rockset/model/list_roles_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/list_unsubscribe_preferences_response.py` & `rockset-2.0.2/rockset/model/list_unsubscribe_preferences_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/list_users_response.py` & `rockset-2.0.2/rockset/model/list_users_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/list_views_response.py` & `rockset-2.0.2/rockset/model/list_views_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/list_virtual_instances_response.py` & `rockset-2.0.2/rockset/model/list_virtual_instances_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/list_workspaces_response.py` & `rockset-2.0.2/rockset/model/list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/mongo_db_integration.py` & `rockset-2.0.2/rockset/model/mongo_db_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/mongodb_collection_creation_request.py` & `rockset-2.0.2/rockset/model/gcs_collection_creation_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,25 +28,23 @@
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from rockset.model.event_time_info import EventTimeInfo
     from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
     from rockset.model.field_partition import FieldPartition
-    from rockset.model.mongodb_source_wrapper import MongodbSourceWrapper
+    from rockset.model.gcs_source_wrapper import GcsSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
-    globals()['MongodbSourceWrapper'] = MongodbSourceWrapper
+    globals()['GcsSourceWrapper'] = GcsSourceWrapper
 
 
-class MongodbCollectionCreationRequest(ModelNormal):
+class GcsCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([MongodbSourceWrapper], none_type),  # noqa: E501
+            'sources': ([GcsSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """MongodbCollectionCreationRequest - a model defined in OpenAPI
+        """GcsCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([MongodbSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([GcsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """MongodbCollectionCreationRequest - a model defined in OpenAPI
+        """GcsCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([MongodbSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([GcsSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/mongodb_integration_creation_request.py` & `rockset-2.0.2/rockset/model/mongodb_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/mongodb_source_wrapper.py` & `rockset-2.0.2/rockset/model/mongodb_source_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     inner_field = "mongodb"
-    inner_properties = ["collection_name", "database_name", "status"]
+    inner_properties = ["collection_name", "database_name", "retrieve_full_document", "status"]
     allowed_values = {
     }
 
     validations = {
     }
 
     @cached_property
@@ -90,27 +90,29 @@
         """
         lazy_import()
         return {
             'collection_name': (str,),  # noqa: E501
             'database_name': (str,),  # noqa: E501
             'format_params': (FormatParams, none_type),  # noqa: E501
             'integration_name': (str, none_type),  # noqa: E501
+            'retrieve_full_document': (bool, none_type),  # noqa: E501
             'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'collection_name': 'collection_name',  # noqa: E501
         'database_name': 'database_name',  # noqa: E501
         'format_params': 'format_params',  # noqa: E501
         'integration_name': 'integration_name',  # noqa: E501
+        'retrieve_full_document': 'retrieve_full_document',  # noqa: E501
         'status': 'status',  # noqa: E501
     }
 
     read_only_vars = {
         'status',  # noqa: E501
     }
 
@@ -154,14 +156,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             format_params (FormatParams): [optional]  # noqa: E501
             integration_name (str): Name of integration to use.. [optional]  # noqa: E501
+            retrieve_full_document (bool): Whether to get the full document from the MongoDB change stream to enable multi-field expression transformations. Selecting this option will increase load on your upstream MongoDB database.. [optional]  # noqa: E501
             status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -212,14 +215,15 @@
         """MongodbSourceWrapper - a model defined in OpenAPI
 
         Keyword Args:
             collection_name (str): MongoDB collection name.
             database_name (str): MongoDB database name containing this collection.
             format_params (FormatParams): [optional]  # noqa: E501
             integration_name (str): Name of integration to use.. [optional]  # noqa: E501
+            retrieve_full_document (bool): Whether to get the full document from the MongoDB change stream to enable multi-field expression transformations. Selecting this option will increase load on your upstream MongoDB database.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/organization.py` & `rockset-2.0.2/rockset/model/organization.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,28 +89,32 @@
         return {
             'clusters': ([Cluster], none_type),  # noqa: E501
             'created_at': (str, none_type),  # noqa: E501
             'display_name': (str, none_type),  # noqa: E501
             'external_id': (str, none_type),  # noqa: E501
             'id': (str, none_type),  # noqa: E501
             'rockset_user': (str, none_type),  # noqa: E501
+            'sso_connection': (str, none_type),  # noqa: E501
+            'sso_only': (bool, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'clusters': 'clusters',  # noqa: E501
         'created_at': 'created_at',  # noqa: E501
         'display_name': 'display_name',  # noqa: E501
         'external_id': 'external_id',  # noqa: E501
         'id': 'id',  # noqa: E501
         'rockset_user': 'rockset_user',  # noqa: E501
+        'sso_connection': 'sso_connection',  # noqa: E501
+        'sso_only': 'sso_only',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -152,14 +156,16 @@
                                 _visited_composed_classes = (Animal,)
             clusters ([Cluster]): List of clusters associated with this org.. [optional]  # noqa: E501
             created_at (str): ISO-8601 date.. [optional]  # noqa: E501
             display_name (str): Name of the organization.. [optional]  # noqa: E501
             external_id (str): Organization's unique external ID within Rockset.. [optional]  # noqa: E501
             id (str): Unique identifier for the organization.. [optional]  # noqa: E501
             rockset_user (str): Rockset's global AWS user.. [optional]  # noqa: E501
+            sso_connection (str): Connection name of SSO connection.. [optional]  # noqa: E501
+            sso_only (bool): Whether or not SSO is the only permitted form of auth.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -209,14 +215,16 @@
         Keyword Args:
             clusters ([Cluster]): List of clusters associated with this org.. [optional]  # noqa: E501
             created_at (str): ISO-8601 date.. [optional]  # noqa: E501
             display_name (str): Name of the organization.. [optional]  # noqa: E501
             external_id (str): Organization's unique external ID within Rockset.. [optional]  # noqa: E501
             id (str): Unique identifier for the organization.. [optional]  # noqa: E501
             rockset_user (str): Rockset's global AWS user.. [optional]  # noqa: E501
+            sso_connection (str): Connection name of SSO connection.. [optional]  # noqa: E501
+            sso_only (bool): Whether or not SSO is the only permitted form of auth.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/organization_response.py` & `rockset-2.0.2/rockset/model/organization_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/output_field.py` & `rockset-2.0.2/rockset/model/output_field.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/pagination.py` & `rockset-2.0.2/rockset/model/pagination.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/pagination_info.py` & `rockset-2.0.2/rockset/model/pagination_info.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/patch_document.py` & `rockset-2.0.2/rockset/model/patch_document.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/patch_documents_request.py` & `rockset-2.0.2/rockset/model/patch_documents_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/patch_documents_response.py` & `rockset-2.0.2/rockset/model/patch_documents_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/patch_operation.py` & `rockset-2.0.2/rockset/model/patch_operation.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/privilege.py` & `rockset-2.0.2/rockset/model/privilege.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
             'UPDATE_RESOURCE_OWNER_GLOBAL': "UPDATE_RESOURCE_OWNER_GLOBAL",
             'CREATE_API_KEY_GLOBAL': "CREATE_API_KEY_GLOBAL",
             'CREATE_ROLE_GLOBAL': "CREATE_ROLE_GLOBAL",
             'UPDATE_ROLE_GLOBAL': "UPDATE_ROLE_GLOBAL",
             'DELETE_ROLE_GLOBAL': "DELETE_ROLE_GLOBAL",
             'LIST_ROLES_GLOBAL': "LIST_ROLES_GLOBAL",
             'GRANT_REVOKE_ROLE_GLOBAL': "GRANT_REVOKE_ROLE_GLOBAL",
+            'CREATE_QUERY_LOGS_COLLECTION_GLOBAL': "CREATE_QUERY_LOGS_COLLECTION_GLOBAL",
             'ALL_INTEGRATION_ACTIONS': "ALL_INTEGRATION_ACTIONS",
             'CREATE_COLLECTION_INTEGRATION': "CREATE_COLLECTION_INTEGRATION",
             'ALL_WORKSPACE_ACTIONS': "ALL_WORKSPACE_ACTIONS",
             'DELETE_WS': "DELETE_WS",
             'QUERY_DATA_WS': "QUERY_DATA_WS",
             'WRITE_DATA_WS': "WRITE_DATA_WS",
             'CREATE_COLLECTION_WS': "CREATE_COLLECTION_WS",
```

### Comparing `rockset-2.0.0/rockset/model/query_error.py` & `rockset-2.0.2/rockset/model/query_error.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/query_field_type.py` & `rockset-2.0.2/rockset/model/query_field_type.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/query_info.py` & `rockset-2.0.2/rockset/model/query_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         return {
             'executed_by': (str, none_type),  # noqa: E501
             'expires_at': (str, none_type),  # noqa: E501
             'last_offset': (str, none_type),  # noqa: E501
             'pagination': (Pagination, none_type),  # noqa: E501
             'query_errors': ([QueryError], none_type),  # noqa: E501
             'query_id': (str, none_type),  # noqa: E501
+            'sql': (str, none_type),  # noqa: E501
             'stats': (Stats, none_type),  # noqa: E501
             'status': (str, none_type),  # noqa: E501
             'submitted_at': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -117,14 +118,15 @@
     attribute_map = {
         'executed_by': 'executed_by',  # noqa: E501
         'expires_at': 'expires_at',  # noqa: E501
         'last_offset': 'last_offset',  # noqa: E501
         'pagination': 'pagination',  # noqa: E501
         'query_errors': 'query_errors',  # noqa: E501
         'query_id': 'query_id',  # noqa: E501
+        'sql': 'sql',  # noqa: E501
         'stats': 'stats',  # noqa: E501
         'status': 'status',  # noqa: E501
         'submitted_at': 'submitted_at',  # noqa: E501
     }
 
     read_only_vars = {
     }
@@ -169,14 +171,15 @@
                                 _visited_composed_classes = (Animal,)
             executed_by (str): User ID who executed the query.. [optional]  # noqa: E501
             expires_at (str): Time (UTC) that query results expire. Only populated if `status` is `COMPLETE`.. [optional]  # noqa: E501
             last_offset (str): The log offset that query results were written to in the destination collection. Only populated for INSERT INTO queries.. [optional]  # noqa: E501
             pagination (Pagination): [optional]  # noqa: E501
             query_errors ([QueryError]): Errors encountered while executing the query.. [optional]  # noqa: E501
             query_id (str): Unique Query ID.. [optional]  # noqa: E501
+            sql (str): The SQL query for this request. [optional]  # noqa: E501
             stats (Stats): [optional]  # noqa: E501
             status (str): Status of the query.. [optional]  # noqa: E501
             submitted_at (str): Time (UTC) the query request was first received and queued for execution.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -229,14 +232,15 @@
         Keyword Args:
             executed_by (str): User ID who executed the query.. [optional]  # noqa: E501
             expires_at (str): Time (UTC) that query results expire. Only populated if `status` is `COMPLETE`.. [optional]  # noqa: E501
             last_offset (str): The log offset that query results were written to in the destination collection. Only populated for INSERT INTO queries.. [optional]  # noqa: E501
             pagination (Pagination): [optional]  # noqa: E501
             query_errors ([QueryError]): Errors encountered while executing the query.. [optional]  # noqa: E501
             query_id (str): Unique Query ID.. [optional]  # noqa: E501
+            sql (str): The SQL query for this request. [optional]  # noqa: E501
             stats (Stats): [optional]  # noqa: E501
             status (str): Status of the query.. [optional]  # noqa: E501
             submitted_at (str): Time (UTC) the query request was first received and queued for execution.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `rockset-2.0.0/rockset/model/query_lambda.py` & `rockset-2.0.2/rockset/model/query_lambda.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/query_lambda_sql.py` & `rockset-2.0.2/rockset/model/query_lambda_sql.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/query_lambda_stats.py` & `rockset-2.0.2/rockset/model/query_lambda_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/query_lambda_tag.py` & `rockset-2.0.2/rockset/model/query_lambda_tag.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/query_lambda_tag_response.py` & `rockset-2.0.2/rockset/model/query_lambda_tag_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/query_lambda_version.py` & `rockset-2.0.2/rockset/model/query_lambda_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'collections': ([str], none_type),  # noqa: E501
             'created_at': (str, none_type),  # noqa: E501
             'created_by': (str, none_type),  # noqa: E501
+            'created_by_apikey_name': (str, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'name': (str, none_type),  # noqa: E501
             'public_access_id': (str, none_type),  # noqa: E501
             'sql': (QueryLambdaSql, none_type),  # noqa: E501
             'state': (str, none_type),  # noqa: E501
             'stats': (QueryLambdaStats, none_type),  # noqa: E501
             'version': (str, none_type),  # noqa: E501
@@ -111,14 +112,15 @@
         return None
 
 
     attribute_map = {
         'collections': 'collections',  # noqa: E501
         'created_at': 'created_at',  # noqa: E501
         'created_by': 'created_by',  # noqa: E501
+        'created_by_apikey_name': 'created_by_apikey_name',  # noqa: E501
         'description': 'description',  # noqa: E501
         'name': 'name',  # noqa: E501
         'public_access_id': 'public_access_id',  # noqa: E501
         'sql': 'sql',  # noqa: E501
         'state': 'state',  # noqa: E501
         'stats': 'stats',  # noqa: E501
         'version': 'version',  # noqa: E501
@@ -165,14 +167,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             collections ([str]): Collections queried by underlying SQL query.. [optional]  # noqa: E501
             created_at (str): ISO-8601 date of when Query Lambda was created.. [optional]  # noqa: E501
             created_by (str): User that created this Query Lambda.. [optional]  # noqa: E501
+            created_by_apikey_name (str): Name of the API key that was used to create this object if one was used.. [optional]  # noqa: E501
             description (str): Optional description.. [optional]  # noqa: E501
             name (str): Query Lambda name.. [optional]  # noqa: E501
             public_access_id (str): Public access ID associated with this QL version. [optional]  # noqa: E501
             sql (QueryLambdaSql): [optional]  # noqa: E501
             state (str): Status of this Query Lambda.. [optional]  # noqa: E501
             stats (QueryLambdaStats): [optional]  # noqa: E501
             version (str): Query Lambda version.. [optional]  # noqa: E501
@@ -227,14 +230,15 @@
     def __init__(self, **kwargs):  # noqa: E501
         """QueryLambdaVersion - a model defined in OpenAPI
 
         Keyword Args:
             collections ([str]): Collections queried by underlying SQL query.. [optional]  # noqa: E501
             created_at (str): ISO-8601 date of when Query Lambda was created.. [optional]  # noqa: E501
             created_by (str): User that created this Query Lambda.. [optional]  # noqa: E501
+            created_by_apikey_name (str): Name of the API key that was used to create this object if one was used.. [optional]  # noqa: E501
             description (str): Optional description.. [optional]  # noqa: E501
             name (str): Query Lambda name.. [optional]  # noqa: E501
             public_access_id (str): Public access ID associated with this QL version. [optional]  # noqa: E501
             sql (QueryLambdaSql): [optional]  # noqa: E501
             state (str): Status of this Query Lambda.. [optional]  # noqa: E501
             stats (QueryLambdaStats): [optional]  # noqa: E501
             version (str): Query Lambda version.. [optional]  # noqa: E501
```

### Comparing `rockset-2.0.0/rockset/model/query_lambda_version_response.py` & `rockset-2.0.2/rockset/model/query_lambda_version_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/query_pagination_response.py` & `rockset-2.0.2/rockset/model/query_pagination_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/query_parameter.py` & `rockset-2.0.2/rockset/model/query_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, type, value, *args, **kwargs):  # noqa: E501
         """QueryParameter - a model defined in OpenAPI
 
         Args:
             name (str): Name of the field.
-            type (str): Data type of the field.
+            type (str): Deprecated. Data type of the field.
             value (str): Literal value of the field.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -194,15 +194,15 @@
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, type, value, **kwargs):  # noqa: E501
         """QueryParameter - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Name of the field.
-            type (str): Data type of the field.
+            type (str): Deprecated. Data type of the field.
             value (str): Literal value of the field.
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
```

### Comparing `rockset-2.0.0/rockset/model/query_request.py` & `rockset-2.0.2/rockset/model/update_api_key_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,22 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rockset.model.async_query_options import AsyncQueryOptions
-    from rockset.model.query_request_sql import QueryRequestSql
-    globals()['AsyncQueryOptions'] = AsyncQueryOptions
-    globals()['QueryRequestSql'] = QueryRequestSql
 
-
-class QueryRequest(ModelNormal):
+class UpdateApiKeyRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -57,68 +51,65 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('state',): {
+            'ACTIVE': "ACTIVE",
+            'SUSPENDED': "SUSPENDED",
+        },
     }
 
     validations = {
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
-            'sql': (QueryRequestSql,),  # noqa: E501
-            'async_options': (AsyncQueryOptions, none_type),  # noqa: E501
+            'state': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'sql': 'sql',  # noqa: E501
-        'async_options': 'async_options',  # noqa: E501
+        'state': 'state',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, sql, *args, **kwargs):  # noqa: E501
-        """QueryRequest - a model defined in OpenAPI
-
-        Args:
-            sql (QueryRequestSql):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """UpdateApiKeyRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,15 +134,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            async_options (AsyncQueryOptions): [optional]  # noqa: E501
+            state (str): State that the api key should be set to.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -171,15 +162,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.sql = sql
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -192,20 +182,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *, sql, **kwargs):  # noqa: E501
-        """QueryRequest - a model defined in OpenAPI
+    def __init__(self, **kwargs):  # noqa: E501
+        """UpdateApiKeyRequest - a model defined in OpenAPI
 
         Keyword Args:
-            sql (QueryRequestSql):
-            async_options (AsyncQueryOptions): [optional]  # noqa: E501
+            state (str): State that the api key should be set to.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -254,15 +243,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.sql = sql
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset-2.0.0/rockset/model/query_request_sql.py` & `rockset-2.0.2/rockset/model/source_kafka.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_parameter import QueryParameter
-    globals()['QueryParameter'] = QueryParameter
+    from rockset.model.status_kafka import StatusKafka
+    globals()['StatusKafka'] = StatusKafka
 
 
-class QueryRequestSql(ModelNormal):
+class SourceKafka(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,14 +55,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('offset_reset_policy',): {
+            'LATEST': "LATEST",
+            'EARLIEST': "EARLIEST",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -83,48 +87,44 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'query': (str,),  # noqa: E501
-            'default_row_limit': (int, none_type),  # noqa: E501
-            'generate_warnings': (bool, none_type),  # noqa: E501
-            'initial_paginate_response_doc_count': (int, none_type),  # noqa: E501
-            'paginate': (bool, none_type),  # noqa: E501
-            'parameters': ([QueryParameter], none_type),  # noqa: E501
+            'consumer_group_id': (str, none_type),  # noqa: E501
+            'kafka_topic_name': (str, none_type),  # noqa: E501
+            'offset_reset_policy': (str, none_type),  # noqa: E501
+            'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
+            'use_v3': (bool, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'query': 'query',  # noqa: E501
-        'default_row_limit': 'default_row_limit',  # noqa: E501
-        'generate_warnings': 'generate_warnings',  # noqa: E501
-        'initial_paginate_response_doc_count': 'initial_paginate_response_doc_count',  # noqa: E501
-        'paginate': 'paginate',  # noqa: E501
-        'parameters': 'parameters',  # noqa: E501
+        'consumer_group_id': 'consumer_group_id',  # noqa: E501
+        'kafka_topic_name': 'kafka_topic_name',  # noqa: E501
+        'offset_reset_policy': 'offset_reset_policy',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'use_v3': 'use_v3',  # noqa: E501
     }
 
     read_only_vars = {
+        'status',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, query, *args, **kwargs):  # noqa: E501
-        """QueryRequestSql - a model defined in OpenAPI
-
-        Args:
-            query (str): SQL query string.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """SourceKafka - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -149,19 +149,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            default_row_limit (int): Row limit to use. Limits specified in the query text will override this default.. [optional]  # noqa: E501
-            generate_warnings (bool): Flag to enable warnings. Warnings can help debug query issues but negatively affect performance.. [optional]  # noqa: E501
-            initial_paginate_response_doc_count (int): Number of documents to return in addition to paginating for this query call. Only relevant if `paginate` flag is also set.. [optional]  # noqa: E501
-            paginate (bool): Flag to paginate and store the results of this query for later sequential retrieval.. [optional]  # noqa: E501
-            parameters ([QueryParameter]): List of named parameters.. [optional]  # noqa: E501
+            consumer_group_id (str): The Kafka consumer group Id being used.. [optional]  # noqa: E501
+            kafka_topic_name (str): The Kafka topic to be tailed.. [optional]  # noqa: E501
+            offset_reset_policy (str): The offset reset policy.. [optional]  # noqa: E501
+            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            use_v3 (bool): Whether to use v3 integration.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -181,15 +181,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.query = query
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -202,24 +201,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *, query, **kwargs):  # noqa: E501
-        """QueryRequestSql - a model defined in OpenAPI
+    def __init__(self, **kwargs):  # noqa: E501
+        """SourceKafka - a model defined in OpenAPI
 
         Keyword Args:
-            query (str): SQL query string.
-            default_row_limit (int): Row limit to use. Limits specified in the query text will override this default.. [optional]  # noqa: E501
-            generate_warnings (bool): Flag to enable warnings. Warnings can help debug query issues but negatively affect performance.. [optional]  # noqa: E501
-            initial_paginate_response_doc_count (int): Number of documents to return in addition to paginating for this query call. Only relevant if `paginate` flag is also set.. [optional]  # noqa: E501
-            paginate (bool): Flag to paginate and store the results of this query for later sequential retrieval.. [optional]  # noqa: E501
-            parameters ([QueryParameter]): List of named parameters.. [optional]  # noqa: E501
+            consumer_group_id (str): The Kafka consumer group Id being used.. [optional]  # noqa: E501
+            kafka_topic_name (str): The Kafka topic to be tailed.. [optional]  # noqa: E501
+            offset_reset_policy (str): The offset reset policy.. [optional]  # noqa: E501
+            use_v3 (bool): Whether to use v3 integration.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -268,15 +265,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.query = query
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset-2.0.0/rockset/model/query_response.py` & `rockset-2.0.2/rockset/model/query_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/query_response_stats.py` & `rockset-2.0.2/rockset/model/query_response_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/resume_virtual_instance_response.py` & `rockset-2.0.2/rockset/model/resume_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/role.py` & `rockset-2.0.2/rockset/model/role.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/role_response.py` & `rockset-2.0.2/rockset/model/role_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/s3_collection_creation_request.py` & `rockset-2.0.2/rockset/model/kinesis_collection_creation_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,25 +28,23 @@
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from rockset.model.event_time_info import EventTimeInfo
     from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
     from rockset.model.field_partition import FieldPartition
-    from rockset.model.s3_source_wrapper import S3SourceWrapper
+    from rockset.model.kinesis_source_wrapper import KinesisSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
-    globals()['S3SourceWrapper'] = S3SourceWrapper
+    globals()['KinesisSourceWrapper'] = KinesisSourceWrapper
 
 
-class S3CollectionCreationRequest(ModelNormal):
+class KinesisCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([S3SourceWrapper], none_type),  # noqa: E501
+            'sources': ([KinesisSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """S3CollectionCreationRequest - a model defined in OpenAPI
+        """KinesisCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([S3SourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([KinesisSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """S3CollectionCreationRequest - a model defined in OpenAPI
+        """KinesisCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([S3SourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([KinesisSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/s3_integration.py` & `rockset-2.0.2/rockset/model/s3_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/s3_integration_creation_request.py` & `rockset-2.0.2/rockset/model/s3_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/s3_source_wrapper.py` & `rockset-2.0.2/rockset/model/s3_source_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,15 @@
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from rockset.model.format_params import FormatParams
-    from rockset.model.status import Status
     globals()['FormatParams'] = FormatParams
-    globals()['Status'] = Status
 
 
 class S3SourceWrapper(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -87,66 +85,62 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'bucket': (str,),  # noqa: E501
-            'prefixes': ([str],),  # noqa: E501
             'format_params': (FormatParams, none_type),  # noqa: E501
             'integration_name': (str, none_type),  # noqa: E501
-            'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
             'object_bytes_downloaded': (int, none_type),  # noqa: E501
             'object_bytes_total': (int, none_type),  # noqa: E501
             'object_count_downloaded': (int, none_type),  # noqa: E501
             'object_count_total': (int, none_type),  # noqa: E501
             'pattern': (str, none_type),  # noqa: E501
             'prefix': (str, none_type),  # noqa: E501
+            'prefixes': ([str], none_type),  # noqa: E501
             'region': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'bucket': 'bucket',  # noqa: E501
-        'prefixes': 'prefixes',  # noqa: E501
         'format_params': 'format_params',  # noqa: E501
         'integration_name': 'integration_name',  # noqa: E501
-        'status': 'status',  # noqa: E501
         'object_bytes_downloaded': 'object_bytes_downloaded',  # noqa: E501
         'object_bytes_total': 'object_bytes_total',  # noqa: E501
         'object_count_downloaded': 'object_count_downloaded',  # noqa: E501
         'object_count_total': 'object_count_total',  # noqa: E501
         'pattern': 'pattern',  # noqa: E501
         'prefix': 'prefix',  # noqa: E501
+        'prefixes': 'prefixes',  # noqa: E501
         'region': 'region',  # noqa: E501
     }
 
     read_only_vars = {
-        'prefixes',  # noqa: E501
-        'status',  # noqa: E501
         'object_bytes_downloaded',  # noqa: E501
         'object_bytes_total',  # noqa: E501
         'object_count_downloaded',  # noqa: E501
         'object_count_total',  # noqa: E501
+        'prefixes',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, bucket, prefixes, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, bucket, *args, **kwargs):  # noqa: E501
         """S3SourceWrapper - a model defined in OpenAPI
 
         Args:
             bucket (str): Address of S3 bucket containing data.
-            prefixes ([str]): List of prefixes to paths from which data should be ingested.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -173,21 +167,21 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             format_params (FormatParams): [optional]  # noqa: E501
             integration_name (str): Name of integration to use.. [optional]  # noqa: E501
-            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             object_bytes_downloaded (int): [optional]  # noqa: E501
             object_bytes_total (int): [optional]  # noqa: E501
             object_count_downloaded (int): [optional]  # noqa: E501
             object_count_total (int): [optional]  # noqa: E501
             pattern (str): Glob-style pattern that selects keys to ingest. Only either prefix or pattern can be specified.. [optional]  # noqa: E501
             prefix (str): Prefix that selects keys to ingest.. [optional]  # noqa: E501
+            prefixes ([str]): List of prefixes to paths from which data should be ingested.. [optional]  # noqa: E501
             region (str): AWS region containing source bucket.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -209,15 +203,14 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.bucket = bucket
-        self.prefixes = prefixes
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset-2.0.0/rockset/model/schema_registry_config.py` & `rockset-2.0.2/rockset/model/schema_registry_config.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/segment_integration.py` & `rockset-2.0.2/rockset/model/segment_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/segment_integration_creation_request.py` & `rockset-2.0.2/rockset/model/segment_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/snowflake_collection_creation_request.py` & `rockset-2.0.2/rockset/model/azure_service_bus_collection_creation_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,27 +26,25 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from rockset.model.azure_service_bus_source_wrapper import AzureServiceBusSourceWrapper
     from rockset.model.event_time_info import EventTimeInfo
     from rockset.model.field_mapping_query import FieldMappingQuery
-    from rockset.model.field_mapping_v2 import FieldMappingV2
     from rockset.model.field_partition import FieldPartition
-    from rockset.model.snowflake_source_wrapper import SnowflakeSourceWrapper
+    globals()['AzureServiceBusSourceWrapper'] = AzureServiceBusSourceWrapper
     globals()['EventTimeInfo'] = EventTimeInfo
     globals()['FieldMappingQuery'] = FieldMappingQuery
-    globals()['FieldMappingV2'] = FieldMappingV2
     globals()['FieldPartition'] = FieldPartition
-    globals()['SnowflakeSourceWrapper'] = SnowflakeSourceWrapper
 
 
-class SnowflakeCollectionCreationRequest(ModelNormal):
+class AzureServiceBusCollectionCreationRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -63,14 +61,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('storage_compression_type',): {
+            'LZ4': "LZ4",
+            'ZSTD': "ZSTD",
+        },
     }
 
     validations = {
         ('retention_secs',): {
             'inclusive_minimum': 1,
         },
     }
@@ -99,44 +101,44 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'clustering_key': ([FieldPartition], none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'event_time_info': (EventTimeInfo, none_type),  # noqa: E501
             'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
-            'field_mappings': ([FieldMappingV2], none_type),  # noqa: E501
             'retention_secs': (int, none_type),  # noqa: E501
-            'sources': ([SnowflakeSourceWrapper], none_type),  # noqa: E501
+            'sources': ([AzureServiceBusSourceWrapper], none_type),  # noqa: E501
+            'storage_compression_type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'clustering_key': 'clustering_key',  # noqa: E501
         'description': 'description',  # noqa: E501
         'event_time_info': 'event_time_info',  # noqa: E501
         'field_mapping_query': 'field_mapping_query',  # noqa: E501
-        'field_mappings': 'field_mappings',  # noqa: E501
         'retention_secs': 'retention_secs',  # noqa: E501
         'sources': 'sources',  # noqa: E501
+        'storage_compression_type': 'storage_compression_type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
-        """SnowflakeCollectionCreationRequest - a model defined in OpenAPI
+        """AzureServiceBusCollectionCreationRequest - a model defined in OpenAPI
 
         Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -168,17 +170,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([SnowflakeSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([AzureServiceBusSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,25 +222,25 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
-        """SnowflakeCollectionCreationRequest - a model defined in OpenAPI
+        """AzureServiceBusCollectionCreationRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for collection, can contain alphanumeric or dash characters.
             clustering_key ([FieldPartition]): Deprecated. List of clustering fields. Use CLUSTER BY clause in `field_mapping_query` instead.. [optional]  # noqa: E501
             description (str): Text describing the collection.. [optional]  # noqa: E501
             event_time_info (EventTimeInfo): [optional]  # noqa: E501
             field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
-            field_mappings ([FieldMappingV2]): Deprecated. List of mappings. Use field_mapping_query instead.. [optional]  # noqa: E501
             retention_secs (int): Number of seconds after which data is purged, based on event time.. [optional]  # noqa: E501
-            sources ([SnowflakeSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            sources ([AzureServiceBusSourceWrapper]): List of sources from which to ingest data. [optional]  # noqa: E501
+            storage_compression_type (str): RocksDB storage compression type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/snowflake_integration.py` & `rockset-2.0.2/rockset/model/snowflake_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/snowflake_integration_creation_request.py` & `rockset-2.0.2/rockset/model/snowflake_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/snowflake_source_wrapper.py` & `rockset-2.0.2/rockset/model/snowflake_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/source.py` & `rockset-2.0.2/rockset/model/source_azure_service_bus.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,21 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.format_params import FormatParams
-    from rockset.model.status import Status
-    globals()['FormatParams'] = FormatParams
-    globals()['Status'] = Status
+    from rockset.model.status_azure_service_bus import StatusAzureServiceBus
+    globals()['StatusAzureServiceBus'] = StatusAzureServiceBus
 
 
-class Source(ModelNormal):
+class SourceAzureServiceBus(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,40 +83,40 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'format_params': (FormatParams, none_type),  # noqa: E501
-            'integration_name': (str, none_type),  # noqa: E501
             'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
+            'subscription': (str, none_type),  # noqa: E501
+            'topic': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'format_params': 'format_params',  # noqa: E501
-        'integration_name': 'integration_name',  # noqa: E501
         'status': 'status',  # noqa: E501
+        'subscription': 'subscription',  # noqa: E501
+        'topic': 'topic',  # noqa: E501
     }
 
     read_only_vars = {
         'status',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Source - a model defined in OpenAPI
+        """SourceAzureServiceBus - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,17 +141,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            format_params (FormatParams): [optional]  # noqa: E501
-            integration_name (str): Name of integration to use.. [optional]  # noqa: E501
             status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            subscription (str): The subscription to read from the topic.. [optional]  # noqa: E501
+            topic (str): Name of the topic which rockset should ingest from.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -194,19 +192,19 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """Source - a model defined in OpenAPI
+        """SourceAzureServiceBus - a model defined in OpenAPI
 
         Keyword Args:
-            format_params (FormatParams): [optional]  # noqa: E501
-            integration_name (str): Name of integration to use.. [optional]  # noqa: E501
+            subscription (str): The subscription to read from the topic.. [optional]  # noqa: E501
+            topic (str): Name of the topic which rockset should ingest from.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/source_azure_blob_storage.py` & `rockset-2.0.2/rockset/model/source_azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/source_azure_event_hubs.py` & `rockset-2.0.2/rockset/model/source_azure_event_hubs.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/source_azure_service_bus.py` & `rockset-2.0.2/rockset/model/source_kinesis.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rockset.model.status_azure_service_bus import StatusAzureServiceBus
-    globals()['StatusAzureServiceBus'] = StatusAzureServiceBus
 
-
-class SourceAzureServiceBus(ModelNormal):
+class SourceKinesis(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,68 +51,74 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('offset_reset_policy',): {
+            'LATEST': "LATEST",
+            'EARLIEST': "EARLIEST",
+        },
     }
 
     validations = {
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
-            'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
-            'subscription': (str, none_type),  # noqa: E501
-            'topic': (str, none_type),  # noqa: E501
+            'stream_name': (str,),  # noqa: E501
+            'aws_region': (str, none_type),  # noqa: E501
+            'dms_primary_key': ([str], none_type),  # noqa: E501
+            'offset_reset_policy': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'status': 'status',  # noqa: E501
-        'subscription': 'subscription',  # noqa: E501
-        'topic': 'topic',  # noqa: E501
+        'stream_name': 'stream_name',  # noqa: E501
+        'aws_region': 'aws_region',  # noqa: E501
+        'dms_primary_key': 'dms_primary_key',  # noqa: E501
+        'offset_reset_policy': 'offset_reset_policy',  # noqa: E501
     }
 
     read_only_vars = {
-        'status',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SourceAzureServiceBus - a model defined in OpenAPI
+    def _from_openapi_data(cls, stream_name, *args, **kwargs):  # noqa: E501
+        """SourceKinesis - a model defined in OpenAPI
+
+        Args:
+            stream_name (str): Name of kinesis stream.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,17 +143,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            subscription (str): The subscription to read from the topic.. [optional]  # noqa: E501
-            topic (str): Name of the topic which rockset should ingest from.. [optional]  # noqa: E501
+            aws_region (str): AWS region name of Kinesis stream, by default us-west-2 is used.. [optional]  # noqa: E501
+            dms_primary_key ([str]): Set of fields that correspond to a DMS primary key.. [optional]  # noqa: E501
+            offset_reset_policy (str): For non-DMS streams, Rockset can tail from the earliest end or latest end of kinesis source.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -171,14 +173,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.stream_name = stream_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -191,20 +194,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, **kwargs):  # noqa: E501
-        """SourceAzureServiceBus - a model defined in OpenAPI
+    def __init__(self, *, stream_name, **kwargs):  # noqa: E501
+        """SourceKinesis - a model defined in OpenAPI
 
         Keyword Args:
-            subscription (str): The subscription to read from the topic.. [optional]  # noqa: E501
-            topic (str): Name of the topic which rockset should ingest from.. [optional]  # noqa: E501
+            stream_name (str): Name of kinesis stream.
+            aws_region (str): AWS region name of Kinesis stream, by default us-west-2 is used.. [optional]  # noqa: E501
+            dms_primary_key ([str]): Set of fields that correspond to a DMS primary key.. [optional]  # noqa: E501
+            offset_reset_policy (str): For non-DMS streams, Rockset can tail from the earliest end or latest end of kinesis source.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -253,14 +258,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.stream_name = stream_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset-2.0.0/rockset/model/source_dynamo_db.py` & `rockset-2.0.2/rockset/model/source_dynamo_db.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/source_file_upload.py` & `rockset-2.0.2/rockset/model/source_file_upload.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/source_gcs.py` & `rockset-2.0.2/rockset/model/source_gcs.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/source_kafka.py` & `rockset-2.0.2/rockset/model/status_azure_event_hubs.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.status_kafka import StatusKafka
-    globals()['StatusKafka'] = StatusKafka
+    from rockset.model.status_azure_event_hubs_partition import StatusAzureEventHubsPartition
+    globals()['StatusAzureEventHubsPartition'] = StatusAzureEventHubsPartition
 
 
-class SourceKafka(ModelNormal):
+class StatusAzureEventHubs(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -55,17 +55,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
-        ('offset_reset_policy',): {
-            'LATEST': "LATEST",
-            'EARLIEST': "EARLIEST",
+        ('state',): {
+            'NO_DOCS_YET': "NO_DOCS_YET",
+            'ACTIVE': "ACTIVE",
+            'DORMANT': "DORMANT",
         },
     }
 
     validations = {
     }
 
     @cached_property
@@ -87,44 +88,41 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'consumer_group_id': (str, none_type),  # noqa: E501
-            'kafka_topic_name': (str, none_type),  # noqa: E501
-            'offset_reset_policy': (str, none_type),  # noqa: E501
-            'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
-            'use_v3': (bool, none_type),  # noqa: E501
+            'last_consumed_time': (str, none_type),  # noqa: E501
+            'num_documents_processed': (int, none_type),  # noqa: E501
+            'partitions': ([StatusAzureEventHubsPartition], none_type),  # noqa: E501
+            'state': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'consumer_group_id': 'consumer_group_id',  # noqa: E501
-        'kafka_topic_name': 'kafka_topic_name',  # noqa: E501
-        'offset_reset_policy': 'offset_reset_policy',  # noqa: E501
-        'status': 'status',  # noqa: E501
-        'use_v3': 'use_v3',  # noqa: E501
+        'last_consumed_time': 'last_consumed_time',  # noqa: E501
+        'num_documents_processed': 'num_documents_processed',  # noqa: E501
+        'partitions': 'partitions',  # noqa: E501
+        'state': 'state',  # noqa: E501
     }
 
     read_only_vars = {
-        'status',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SourceKafka - a model defined in OpenAPI
+        """StatusAzureEventHubs - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -149,19 +147,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            consumer_group_id (str): The Kafka consumer group Id being used.. [optional]  # noqa: E501
-            kafka_topic_name (str): The Kafka topic to be tailed.. [optional]  # noqa: E501
-            offset_reset_policy (str): The offset reset policy.. [optional]  # noqa: E501
-            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            use_v3 (bool): Whether to use v3 integration.. [optional]  # noqa: E501
+            last_consumed_time (str): Time at which the last document was consumed.. [optional]  # noqa: E501
+            num_documents_processed (int): Number of documents consumed.. [optional]  # noqa: E501
+            partitions ([StatusAzureEventHubsPartition]): Status info per partition.. [optional]  # noqa: E501
+            state (str): State of the source.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -202,21 +199,21 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """SourceKafka - a model defined in OpenAPI
+        """StatusAzureEventHubs - a model defined in OpenAPI
 
         Keyword Args:
-            consumer_group_id (str): The Kafka consumer group Id being used.. [optional]  # noqa: E501
-            kafka_topic_name (str): The Kafka topic to be tailed.. [optional]  # noqa: E501
-            offset_reset_policy (str): The offset reset policy.. [optional]  # noqa: E501
-            use_v3 (bool): Whether to use v3 integration.. [optional]  # noqa: E501
+            last_consumed_time (str): Time at which the last document was consumed.. [optional]  # noqa: E501
+            num_documents_processed (int): Number of documents consumed.. [optional]  # noqa: E501
+            partitions ([StatusAzureEventHubsPartition]): Status info per partition.. [optional]  # noqa: E501
+            state (str): State of the source.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/source_kinesis.py` & `rockset-2.0.2/rockset/model/user.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 
-class SourceKinesis(ModelNormal):
+class User(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,18 +51,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
-        ('offset_reset_policy',): {
-            'LATEST': "LATEST",
-            'EARLIEST': "EARLIEST",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -81,44 +77,48 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'stream_name': (str,),  # noqa: E501
-            'aws_region': (str, none_type),  # noqa: E501
-            'dms_primary_key': ([str], none_type),  # noqa: E501
-            'offset_reset_policy': (str, none_type),  # noqa: E501
+            'email': (str,),  # noqa: E501
+            'created_at': (str, none_type),  # noqa: E501
+            'first_name': (str, none_type),  # noqa: E501
+            'last_name': (str, none_type),  # noqa: E501
+            'roles': ([str], none_type),  # noqa: E501
+            'state': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'stream_name': 'stream_name',  # noqa: E501
-        'aws_region': 'aws_region',  # noqa: E501
-        'dms_primary_key': 'dms_primary_key',  # noqa: E501
-        'offset_reset_policy': 'offset_reset_policy',  # noqa: E501
+        'email': 'email',  # noqa: E501
+        'created_at': 'created_at',  # noqa: E501
+        'first_name': 'first_name',  # noqa: E501
+        'last_name': 'last_name',  # noqa: E501
+        'roles': 'roles',  # noqa: E501
+        'state': 'state',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, stream_name, *args, **kwargs):  # noqa: E501
-        """SourceKinesis - a model defined in OpenAPI
+    def _from_openapi_data(cls, email, *args, **kwargs):  # noqa: E501
+        """User - a model defined in OpenAPI
 
         Args:
-            stream_name (str): Name of kinesis stream.
+            email (str): User email.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,17 +143,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            aws_region (str): AWS region name of Kinesis stream, by default us-west-2 is used.. [optional]  # noqa: E501
-            dms_primary_key ([str]): Set of fields that correspond to a DMS primary key.. [optional]  # noqa: E501
-            offset_reset_policy (str): For non-DMS streams, Rockset can tail from the earliest end or latest end of kinesis source.. [optional]  # noqa: E501
+            created_at (str): ISO-8601 date.. [optional]  # noqa: E501
+            first_name (str): User first name.. [optional]  # noqa: E501
+            last_name (str): User last name.. [optional]  # noqa: E501
+            roles ([str]): List of roles for a given user.. [optional]  # noqa: E501
+            state (str): State of user - NEW / ACTIVE.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -173,15 +175,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.stream_name = stream_name
+        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -194,22 +196,24 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *, stream_name, **kwargs):  # noqa: E501
-        """SourceKinesis - a model defined in OpenAPI
+    def __init__(self, *, email, **kwargs):  # noqa: E501
+        """User - a model defined in OpenAPI
 
         Keyword Args:
-            stream_name (str): Name of kinesis stream.
-            aws_region (str): AWS region name of Kinesis stream, by default us-west-2 is used.. [optional]  # noqa: E501
-            dms_primary_key ([str]): Set of fields that correspond to a DMS primary key.. [optional]  # noqa: E501
-            offset_reset_policy (str): For non-DMS streams, Rockset can tail from the earliest end or latest end of kinesis source.. [optional]  # noqa: E501
+            email (str): User email.
+            created_at (str): ISO-8601 date.. [optional]  # noqa: E501
+            first_name (str): User first name.. [optional]  # noqa: E501
+            last_name (str): User last name.. [optional]  # noqa: E501
+            roles ([str]): List of roles for a given user.. [optional]  # noqa: E501
+            state (str): State of user - NEW / ACTIVE.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -258,15 +262,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.stream_name = stream_name
+        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset-2.0.0/rockset/model/source_mongo_db.py` & `rockset-2.0.2/rockset/model/source_mongo_db.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,25 +85,27 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'collection_name': (str,),  # noqa: E501
             'database_name': (str,),  # noqa: E501
+            'retrieve_full_document': (bool, none_type),  # noqa: E501
             'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'collection_name': 'collection_name',  # noqa: E501
         'database_name': 'database_name',  # noqa: E501
+        'retrieve_full_document': 'retrieve_full_document',  # noqa: E501
         'status': 'status',  # noqa: E501
     }
 
     read_only_vars = {
         'status',  # noqa: E501
     }
 
@@ -145,14 +147,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            retrieve_full_document (bool): Whether to get the full document from the MongoDB change stream to enable multi-field expression transformations. Selecting this option will increase load on your upstream MongoDB database.. [optional]  # noqa: E501
             status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -201,14 +204,15 @@
     @convert_js_args_to_python_args
     def __init__(self, *, collection_name, database_name, **kwargs):  # noqa: E501
         """SourceMongoDb - a model defined in OpenAPI
 
         Keyword Args:
             collection_name (str): MongoDB collection name.
             database_name (str): MongoDB database name containing this collection.
+            retrieve_full_document (bool): Whether to get the full document from the MongoDB change stream to enable multi-field expression transformations. Selecting this option will increase load on your upstream MongoDB database.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/source_s3.py` & `rockset-2.0.2/rockset/model/source_s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,59 +78,58 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'bucket': (str,),  # noqa: E501
-            'prefixes': ([str],),  # noqa: E501
             'object_bytes_downloaded': (int, none_type),  # noqa: E501
             'object_bytes_total': (int, none_type),  # noqa: E501
             'object_count_downloaded': (int, none_type),  # noqa: E501
             'object_count_total': (int, none_type),  # noqa: E501
             'pattern': (str, none_type),  # noqa: E501
             'prefix': (str, none_type),  # noqa: E501
+            'prefixes': ([str], none_type),  # noqa: E501
             'region': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'bucket': 'bucket',  # noqa: E501
-        'prefixes': 'prefixes',  # noqa: E501
         'object_bytes_downloaded': 'object_bytes_downloaded',  # noqa: E501
         'object_bytes_total': 'object_bytes_total',  # noqa: E501
         'object_count_downloaded': 'object_count_downloaded',  # noqa: E501
         'object_count_total': 'object_count_total',  # noqa: E501
         'pattern': 'pattern',  # noqa: E501
         'prefix': 'prefix',  # noqa: E501
+        'prefixes': 'prefixes',  # noqa: E501
         'region': 'region',  # noqa: E501
     }
 
     read_only_vars = {
-        'prefixes',  # noqa: E501
         'object_bytes_downloaded',  # noqa: E501
         'object_bytes_total',  # noqa: E501
         'object_count_downloaded',  # noqa: E501
         'object_count_total',  # noqa: E501
+        'prefixes',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, bucket, prefixes, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, bucket, *args, **kwargs):  # noqa: E501
         """SourceS3 - a model defined in OpenAPI
 
         Args:
             bucket (str): Address of S3 bucket containing data.
-            prefixes ([str]): List of prefixes to paths from which data should be ingested.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -161,14 +160,15 @@
                                 _visited_composed_classes = (Animal,)
             object_bytes_downloaded (int): [optional]  # noqa: E501
             object_bytes_total (int): [optional]  # noqa: E501
             object_count_downloaded (int): [optional]  # noqa: E501
             object_count_total (int): [optional]  # noqa: E501
             pattern (str): Glob-style pattern that selects keys to ingest. Only either prefix or pattern can be specified.. [optional]  # noqa: E501
             prefix (str): Prefix that selects keys to ingest.. [optional]  # noqa: E501
+            prefixes ([str]): List of prefixes to paths from which data should be ingested.. [optional]  # noqa: E501
             region (str): AWS region containing source bucket.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -190,15 +190,14 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.bucket = bucket
-        self.prefixes = prefixes
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset-2.0.0/rockset/model/source_snowflake.py` & `rockset-2.0.2/rockset/model/source_snowflake.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/sql_expression.py` & `rockset-2.0.2/rockset/model/sql_expression.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/stats.py` & `rockset-2.0.2/rockset/model/stats.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/status.py` & `rockset-2.0.2/rockset/model/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     allowed_values = {
         ('state',): {
             'INITIALIZING': "INITIALIZING",
             'WATCHING': "WATCHING",
             'PROCESSING': "PROCESSING",
             'COMPLETED': "COMPLETED",
             'ERROR': "ERROR",
+            'SUSPENDED': "SUSPENDED",
         },
     }
 
     validations = {
     }
 
     @cached_property
```

### Comparing `rockset-2.0.0/rockset/model/status_azure_event_hubs.py` & `rockset-2.0.2/rockset/model/status_dynamo_db_v2.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rockset.model.status_azure_event_hubs_partition import StatusAzureEventHubsPartition
-    globals()['StatusAzureEventHubsPartition'] = StatusAzureEventHubsPartition
 
-
-class StatusAzureEventHubs(ModelNormal):
+class StatusDynamoDbV2(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -56,73 +52,71 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
         ('state',): {
-            'NO_DOCS_YET': "NO_DOCS_YET",
-            'ACTIVE': "ACTIVE",
-            'DORMANT': "DORMANT",
+            'INITIALIZING': "INITIALIZING",
+            'SCANNING': "SCANNING",
+            'EXPORTING_TO_S3': "EXPORTING_TO_S3",
+            'DOWNLOADING_FROM_S3': "DOWNLOADING_FROM_S3",
+            'PROCESSING_STREAM': "PROCESSING_STREAM",
         },
     }
 
     validations = {
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
-            'last_consumed_time': (str, none_type),  # noqa: E501
-            'num_documents_processed': (int, none_type),  # noqa: E501
-            'partitions': ([StatusAzureEventHubsPartition], none_type),  # noqa: E501
+            'initial_dump_completion_percentage': (float, none_type),  # noqa: E501
             'state': (str, none_type),  # noqa: E501
+            'stream_last_processed_at': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'last_consumed_time': 'last_consumed_time',  # noqa: E501
-        'num_documents_processed': 'num_documents_processed',  # noqa: E501
-        'partitions': 'partitions',  # noqa: E501
+        'initial_dump_completion_percentage': 'initial_dump_completion_percentage',  # noqa: E501
         'state': 'state',  # noqa: E501
+        'stream_last_processed_at': 'stream_last_processed_at',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """StatusAzureEventHubs - a model defined in OpenAPI
+        """StatusDynamoDbV2 - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -147,18 +141,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            last_consumed_time (str): Time at which the last document was consumed.. [optional]  # noqa: E501
-            num_documents_processed (int): Number of documents consumed.. [optional]  # noqa: E501
-            partitions ([StatusAzureEventHubsPartition]): Status info per partition.. [optional]  # noqa: E501
-            state (str): State of the source.. [optional]  # noqa: E501
+            initial_dump_completion_percentage (float): [optional]  # noqa: E501
+            state (str): State of current ingest for this table.. [optional]  # noqa: E501
+            stream_last_processed_at (str): ISO-8601 date when source was last processed.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -199,21 +192,20 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """StatusAzureEventHubs - a model defined in OpenAPI
+        """StatusDynamoDbV2 - a model defined in OpenAPI
 
         Keyword Args:
-            last_consumed_time (str): Time at which the last document was consumed.. [optional]  # noqa: E501
-            num_documents_processed (int): Number of documents consumed.. [optional]  # noqa: E501
-            partitions ([StatusAzureEventHubsPartition]): Status info per partition.. [optional]  # noqa: E501
-            state (str): State of the source.. [optional]  # noqa: E501
+            initial_dump_completion_percentage (float): [optional]  # noqa: E501
+            state (str): State of current ingest for this table.. [optional]  # noqa: E501
+            stream_last_processed_at (str): ISO-8601 date when source was last processed.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/status_azure_event_hubs_partition.py` & `rockset-2.0.2/rockset/model/status_azure_event_hubs_partition.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/status_azure_service_bus.py` & `rockset-2.0.2/rockset/model/status_azure_service_bus.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/status_azure_service_bus_session.py` & `rockset-2.0.2/rockset/model/status_azure_service_bus_session.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/status_dynamo_db.py` & `rockset-2.0.2/rockset/model/status_dynamo_db.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/status_dynamo_db_v2.py` & `rockset-2.0.2/rockset/model/update_query_lambda_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rockset.model.query_lambda_sql import QueryLambdaSql
+    globals()['QueryLambdaSql'] = QueryLambdaSql
 
-class StatusDynamoDbV2(ModelNormal):
+
+class UpdateQueryLambdaRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,72 +55,67 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
-        ('state',): {
-            'INITIALIZING': "INITIALIZING",
-            'SCANNING': "SCANNING",
-            'EXPORTING_TO_S3': "EXPORTING_TO_S3",
-            'DOWNLOADING_FROM_S3': "DOWNLOADING_FROM_S3",
-            'PROCESSING_STREAM': "PROCESSING_STREAM",
-        },
     }
 
     validations = {
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
-            'initial_dump_completion_percentage': (float, none_type),  # noqa: E501
-            'state': (str, none_type),  # noqa: E501
-            'stream_last_processed_at': (str, none_type),  # noqa: E501
+            'description': (str, none_type),  # noqa: E501
+            'is_public': (bool, none_type),  # noqa: E501
+            'sql': (QueryLambdaSql, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'initial_dump_completion_percentage': 'initial_dump_completion_percentage',  # noqa: E501
-        'state': 'state',  # noqa: E501
-        'stream_last_processed_at': 'stream_last_processed_at',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'is_public': 'is_public',  # noqa: E501
+        'sql': 'sql',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """StatusDynamoDbV2 - a model defined in OpenAPI
+        """UpdateQueryLambdaRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -141,17 +140,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            initial_dump_completion_percentage (float): [optional]  # noqa: E501
-            state (str): State of current ingest for this table.. [optional]  # noqa: E501
-            stream_last_processed_at (str): ISO-8601 date when source was last processed.. [optional]  # noqa: E501
+            description (str): Optional description.. [optional]  # noqa: E501
+            is_public (bool): [optional]  # noqa: E501
+            sql (QueryLambdaSql): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -192,20 +191,20 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """StatusDynamoDbV2 - a model defined in OpenAPI
+        """UpdateQueryLambdaRequest - a model defined in OpenAPI
 
         Keyword Args:
-            initial_dump_completion_percentage (float): [optional]  # noqa: E501
-            state (str): State of current ingest for this table.. [optional]  # noqa: E501
-            stream_last_processed_at (str): ISO-8601 date when source was last processed.. [optional]  # noqa: E501
+            description (str): Optional description.. [optional]  # noqa: E501
+            is_public (bool): [optional]  # noqa: E501
+            sql (QueryLambdaSql): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/status_kafka.py` & `rockset-2.0.2/rockset/model/status_kafka.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/status_kafka_partition.py` & `rockset-2.0.2/rockset/model/status_kafka_partition.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/status_mongo_db.py` & `rockset-2.0.2/rockset/model/status_mongo_db.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/status_snowflake.py` & `rockset-2.0.2/rockset/model/status_snowflake.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/suspend_virtual_instance_response.py` & `rockset-2.0.2/rockset/model/suspend_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/unsubscribe_preference.py` & `rockset-2.0.2/rockset/model/unsubscribe_preference.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/update_alias_request.py` & `rockset-2.0.2/rockset/model/update_alias_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/update_api_key_request.py` & `rockset-2.0.2/rockset/model/get_source_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rockset.model.source import Source
+    globals()['Source'] = Source
 
-class UpdateApiKeyRequest(ModelNormal):
+
+class GetSourceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,65 +55,63 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
-        ('state',): {
-            'ACTIVE': "ACTIVE",
-            'SUSPENDED': "SUSPENDED",
-        },
     }
 
     validations = {
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
-            'state': (str, none_type),  # noqa: E501
+            'data': (Source, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'state': 'state',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateApiKeyRequest - a model defined in OpenAPI
+        """GetSourceResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,15 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            state (str): State that the api key should be set to.. [optional]  # noqa: E501
+            data (Source): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,18 +185,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """UpdateApiKeyRequest - a model defined in OpenAPI
+        """GetSourceResponse - a model defined in OpenAPI
 
         Keyword Args:
-            state (str): State that the api key should be set to.. [optional]  # noqa: E501
+            data (Source): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/update_api_key_response.py` & `rockset-2.0.2/rockset/model/update_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/update_integration_request.py` & `rockset-2.0.2/rockset/model/update_integration_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/update_integration_response.py` & `rockset-2.0.2/rockset/model/update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/update_query_lambda_request.py` & `rockset-2.0.2/rockset/model/list_sources_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from rockset.model.query_lambda_sql import QueryLambdaSql
-    globals()['QueryLambdaSql'] = QueryLambdaSql
+    from rockset.model.source import Source
+    globals()['Source'] = Source
 
 
-class UpdateQueryLambdaRequest(ModelNormal):
+class ListSourcesResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,39 +83,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'description': (str, none_type),  # noqa: E501
-            'is_public': (bool, none_type),  # noqa: E501
-            'sql': (QueryLambdaSql, none_type),  # noqa: E501
+            'data': ([Source], none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'description': 'description',  # noqa: E501
-        'is_public': 'is_public',  # noqa: E501
-        'sql': 'sql',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateQueryLambdaRequest - a model defined in OpenAPI
+        """ListSourcesResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            description (str): Optional description.. [optional]  # noqa: E501
-            is_public (bool): [optional]  # noqa: E501
-            sql (QueryLambdaSql): [optional]  # noqa: E501
+            data ([Source]): List of all sources in a collection. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,20 +185,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """UpdateQueryLambdaRequest - a model defined in OpenAPI
+        """ListSourcesResponse - a model defined in OpenAPI
 
         Keyword Args:
-            description (str): Optional description.. [optional]  # noqa: E501
-            is_public (bool): [optional]  # noqa: E501
-            sql (QueryLambdaSql): [optional]  # noqa: E501
+            data ([Source]): List of all sources in a collection. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/update_role_request.py` & `rockset-2.0.2/rockset/model/update_role_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/update_unsubscribe_preferences_request.py` & `rockset-2.0.2/rockset/model/update_unsubscribe_preferences_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/update_unsubscribe_preferences_response.py` & `rockset-2.0.2/rockset/model/update_unsubscribe_preferences_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/update_user_request.py` & `rockset-2.0.2/rockset/model/update_virtual_instance_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rockset.model.virtual_instance import VirtualInstance
+    globals()['VirtualInstance'] = VirtualInstance
 
-class UpdateUserRequest(ModelNormal):
+
+class UpdateVirtualInstanceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,54 +66,52 @@
 
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
-            'first_name': (str, none_type),  # noqa: E501
-            'last_name': (str, none_type),  # noqa: E501
-            'roles': ([str], none_type),  # noqa: E501
+            'data': (VirtualInstance, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'first_name': 'first_name',  # noqa: E501
-        'last_name': 'last_name',  # noqa: E501
-        'roles': 'roles',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateUserRequest - a model defined in OpenAPI
+        """UpdateVirtualInstanceResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,17 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            first_name (str): User first name.. [optional]  # noqa: E501
-            last_name (str): User last name.. [optional]  # noqa: E501
-            roles ([str]): New list of roles for a given user.. [optional]  # noqa: E501
+            data (VirtualInstance): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -185,20 +185,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """UpdateUserRequest - a model defined in OpenAPI
+        """UpdateVirtualInstanceResponse - a model defined in OpenAPI
 
         Keyword Args:
-            first_name (str): User first name.. [optional]  # noqa: E501
-            last_name (str): User last name.. [optional]  # noqa: E501
-            roles ([str]): New list of roles for a given user.. [optional]  # noqa: E501
+            data (VirtualInstance): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/update_view_request.py` & `rockset-2.0.2/rockset/model/update_view_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/update_view_response.py` & `rockset-2.0.2/rockset/model/update_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/update_virtual_instance_request.py` & `rockset-2.0.2/rockset/model/xml_params.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 
-class UpdateVirtualInstanceRequest(ModelNormal):
+class XmlParams(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,28 +51,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
-        ('new_size',): {
-            'FREE': "FREE",
-            'NANO': "NANO",
-            'SHARED': "SHARED",
-            'MILLI': "MILLI",
-            'SMALL': "SMALL",
-            'MEDIUM': "MEDIUM",
-            'LARGE': "LARGE",
-            'XLARGE': "XLARGE",
-            'XLARGE2': "XLARGE2",
-            'XLARGE4': "XLARGE4",
-            'XLARGE8': "XLARGE8",
-            'XLARGE16': "XLARGE16",
-        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -91,45 +77,43 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'auto_suspend_enabled': (bool, none_type),  # noqa: E501
-            'auto_suspend_seconds': (int, none_type),  # noqa: E501
-            'description': (str, none_type),  # noqa: E501
-            'monitoring_enabled': (bool, none_type),  # noqa: E501
-            'name': (str, none_type),  # noqa: E501
-            'new_size': (str, none_type),  # noqa: E501
+            'attribute_prefix': (str, none_type),  # noqa: E501
+            'doc_tag': (str, none_type),  # noqa: E501
+            'encoding': (str, none_type),  # noqa: E501
+            'root_tag': (str, none_type),  # noqa: E501
+            'value_tag': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'auto_suspend_enabled': 'auto_suspend_enabled',  # noqa: E501
-        'auto_suspend_seconds': 'auto_suspend_seconds',  # noqa: E501
-        'description': 'description',  # noqa: E501
-        'monitoring_enabled': 'monitoring_enabled',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'new_size': 'new_size',  # noqa: E501
+        'attribute_prefix': 'attribute_prefix',  # noqa: E501
+        'doc_tag': 'doc_tag',  # noqa: E501
+        'encoding': 'encoding',  # noqa: E501
+        'root_tag': 'root_tag',  # noqa: E501
+        'value_tag': 'value_tag',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateVirtualInstanceRequest - a model defined in OpenAPI
+        """XmlParams - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -154,20 +138,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            auto_suspend_enabled (bool): Whether auto-suspend should be enabled for this Virtual Instance.. [optional]  # noqa: E501
-            auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
-            description (str): New virtual instance description.. [optional]  # noqa: E501
-            monitoring_enabled (bool): [optional]  # noqa: E501
-            name (str): New virtual instance name.. [optional]  # noqa: E501
-            new_size (str): Requested virtual instance size.. [optional]  # noqa: E501
+            attribute_prefix (str): Tag to differentiate between attributes and elements.. [optional]  # noqa: E501
+            doc_tag (str): Tags with which documents are identified.. [optional]  # noqa: E501
+            encoding (str): Encoding in which data source is encoded.. [optional]  # noqa: E501
+            root_tag (str): Tag until which xml is ignored.. [optional]  # noqa: E501
+            value_tag (str): tag used for the value when there are attributes in the element having no child. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -208,23 +191,22 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """UpdateVirtualInstanceRequest - a model defined in OpenAPI
+        """XmlParams - a model defined in OpenAPI
 
         Keyword Args:
-            auto_suspend_enabled (bool): Whether auto-suspend should be enabled for this Virtual Instance.. [optional]  # noqa: E501
-            auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
-            description (str): New virtual instance description.. [optional]  # noqa: E501
-            monitoring_enabled (bool): [optional]  # noqa: E501
-            name (str): New virtual instance name.. [optional]  # noqa: E501
-            new_size (str): Requested virtual instance size.. [optional]  # noqa: E501
+            attribute_prefix (str): Tag to differentiate between attributes and elements.. [optional]  # noqa: E501
+            doc_tag (str): Tags with which documents are identified.. [optional]  # noqa: E501
+            encoding (str): Encoding in which data source is encoded.. [optional]  # noqa: E501
+            root_tag (str): Tag until which xml is ignored.. [optional]  # noqa: E501
+            value_tag (str): tag used for the value when there are attributes in the element having no child. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/update_virtual_instance_response.py` & `rockset-2.0.2/rockset/model/virtual_instance_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from rockset.model.virtual_instance import VirtualInstance
-    globals()['VirtualInstance'] = VirtualInstance
 
-
-class UpdateVirtualInstanceResponse(ModelNormal):
+class VirtualInstanceStats(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,52 +62,50 @@
 
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
-            'data': (VirtualInstance, none_type),  # noqa: E501
+            'last_queried_ms': (int, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'last_queried_ms': 'last_queried_ms',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateVirtualInstanceResponse - a model defined in OpenAPI
+        """VirtualInstanceStats - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +130,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data (VirtualInstance): [optional]  # noqa: E501
+            last_queried_ms (int): Milliseconds since Unix epoch Jan 1, 1970.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -185,18 +179,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """UpdateVirtualInstanceResponse - a model defined in OpenAPI
+        """VirtualInstanceStats - a model defined in OpenAPI
 
         Keyword Args:
-            data (VirtualInstance): [optional]  # noqa: E501
+            last_queried_ms (int): Milliseconds since Unix epoch Jan 1, 1970.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/user.py` & `rockset-2.0.2/rockset/model/workspace.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 
-class User(ModelNormal):
+class Workspace(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,48 +77,43 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'email': (str,),  # noqa: E501
+            'collection_count': (int, none_type),  # noqa: E501
             'created_at': (str, none_type),  # noqa: E501
-            'first_name': (str, none_type),  # noqa: E501
-            'last_name': (str, none_type),  # noqa: E501
-            'roles': ([str], none_type),  # noqa: E501
-            'state': (str, none_type),  # noqa: E501
+            'created_by': (str, none_type),  # noqa: E501
+            'description': (str, none_type),  # noqa: E501
+            'name': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'email': 'email',  # noqa: E501
+        'collection_count': 'collection_count',  # noqa: E501
         'created_at': 'created_at',  # noqa: E501
-        'first_name': 'first_name',  # noqa: E501
-        'last_name': 'last_name',  # noqa: E501
-        'roles': 'roles',  # noqa: E501
-        'state': 'state',  # noqa: E501
+        'created_by': 'created_by',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, email, *args, **kwargs):  # noqa: E501
-        """User - a model defined in OpenAPI
-
-        Args:
-            email (str): User email.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Workspace - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,19 +138,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            created_at (str): ISO-8601 date.. [optional]  # noqa: E501
-            first_name (str): User first name.. [optional]  # noqa: E501
-            last_name (str): User last name.. [optional]  # noqa: E501
-            roles ([str]): List of roles for a given user.. [optional]  # noqa: E501
-            state (str): State of user - NEW / ACTIVE.. [optional]  # noqa: E501
+            collection_count (int): Number of collections that are immediate children of workspace.. [optional]  # noqa: E501
+            created_at (str): ISO-8601 date of when workspace was created.. [optional]  # noqa: E501
+            created_by (str): Email of user who created the workspace.. [optional]  # noqa: E501
+            description (str): Longer explanation for the workspace.. [optional]  # noqa: E501
+            name (str): Descriptive label and unique identifier.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -175,15 +170,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -196,24 +190,23 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *, email, **kwargs):  # noqa: E501
-        """User - a model defined in OpenAPI
+    def __init__(self, **kwargs):  # noqa: E501
+        """Workspace - a model defined in OpenAPI
 
         Keyword Args:
-            email (str): User email.
-            created_at (str): ISO-8601 date.. [optional]  # noqa: E501
-            first_name (str): User first name.. [optional]  # noqa: E501
-            last_name (str): User last name.. [optional]  # noqa: E501
-            roles ([str]): List of roles for a given user.. [optional]  # noqa: E501
-            state (str): State of user - NEW / ACTIVE.. [optional]  # noqa: E501
+            collection_count (int): Number of collections that are immediate children of workspace.. [optional]  # noqa: E501
+            created_at (str): ISO-8601 date of when workspace was created.. [optional]  # noqa: E501
+            created_by (str): Email of user who created the workspace.. [optional]  # noqa: E501
+            description (str): Longer explanation for the workspace.. [optional]  # noqa: E501
+            name (str): Descriptive label and unique identifier.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -262,15 +255,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.email = email
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset-2.0.0/rockset/model/validate_query_response.py` & `rockset-2.0.2/rockset/model/validate_query_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/model/view.py` & `rockset-2.0.2/rockset/model/view.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'created_at': (str, none_type),  # noqa: E501
+            'created_by_apikey_name': (str, none_type),  # noqa: E501
             'creator_email': (str, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'entities': ([str], none_type),  # noqa: E501
             'modified_at': (str, none_type),  # noqa: E501
             'name': (str, none_type),  # noqa: E501
             'owner_email': (str, none_type),  # noqa: E501
             'path': (str, none_type),  # noqa: E501
@@ -102,14 +103,15 @@
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'created_at': 'created_at',  # noqa: E501
+        'created_by_apikey_name': 'created_by_apikey_name',  # noqa: E501
         'creator_email': 'creator_email',  # noqa: E501
         'description': 'description',  # noqa: E501
         'entities': 'entities',  # noqa: E501
         'modified_at': 'modified_at',  # noqa: E501
         'name': 'name',  # noqa: E501
         'owner_email': 'owner_email',  # noqa: E501
         'path': 'path',  # noqa: E501
@@ -156,14 +158,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             created_at (str): ISO-8601 date.. [optional]  # noqa: E501
+            created_by_apikey_name (str): Name of the API key that was used to create this object if one was used.. [optional]  # noqa: E501
             creator_email (str): Email of the creator.. [optional]  # noqa: E501
             description (str): View description.. [optional]  # noqa: E501
             entities ([str]): List of entities referenced by view. An entity can be a view, alias or collection.. [optional]  # noqa: E501
             modified_at (str): ISO-8601 date.. [optional]  # noqa: E501
             name (str): Name of the view.. [optional]  # noqa: E501
             owner_email (str): Email of the owner, note: deprecated and will always be null.. [optional]  # noqa: E501
             path (str): [optional]  # noqa: E501
@@ -218,14 +221,15 @@
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
         """View - a model defined in OpenAPI
 
         Keyword Args:
             created_at (str): ISO-8601 date.. [optional]  # noqa: E501
+            created_by_apikey_name (str): Name of the API key that was used to create this object if one was used.. [optional]  # noqa: E501
             creator_email (str): Email of the creator.. [optional]  # noqa: E501
             description (str): View description.. [optional]  # noqa: E501
             entities ([str]): List of entities referenced by view. An entity can be a view, alias or collection.. [optional]  # noqa: E501
             modified_at (str): ISO-8601 date.. [optional]  # noqa: E501
             name (str): Name of the view.. [optional]  # noqa: E501
             owner_email (str): Email of the owner, note: deprecated and will always be null.. [optional]  # noqa: E501
             path (str): [optional]  # noqa: E501
```

### Comparing `rockset-2.0.0/rockset/model/virtual_instance.py` & `rockset-2.0.2/rockset/model/virtual_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,17 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from rockset.model.auto_scaling_policy import AutoScalingPolicy
     from rockset.model.virtual_instance_stats import VirtualInstanceStats
+    globals()['AutoScalingPolicy'] = AutoScalingPolicy
     globals()['VirtualInstanceStats'] = VirtualInstanceStats
 
 
 class VirtualInstance(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -122,48 +124,54 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
+            'auto_scaling_policy': (AutoScalingPolicy, none_type),  # noqa: E501
             'auto_suspend_seconds': (int, none_type),  # noqa: E501
             'created_at': (str, none_type),  # noqa: E501
             'created_by': (str, none_type),  # noqa: E501
             'current_size': (str, none_type),  # noqa: E501
             'default_pod_count': (int, none_type),  # noqa: E501
             'default_vi': (bool, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'desired_size': (str, none_type),  # noqa: E501
+            'enable_remount_on_resume': (bool, none_type),  # noqa: E501
             'id': (str, none_type),  # noqa: E501
             'monitoring_enabled': (bool, none_type),  # noqa: E501
+            'mount_refresh_interval_seconds': (int, none_type),  # noqa: E501
             'resumed_at': (str, none_type),  # noqa: E501
             'rrn': (str, none_type),  # noqa: E501
             'scaled_pod_count': (int, none_type),  # noqa: E501
             'state': (str, none_type),  # noqa: E501
             'stats': (VirtualInstanceStats, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
+        'auto_scaling_policy': 'auto_scaling_policy',  # noqa: E501
         'auto_suspend_seconds': 'auto_suspend_seconds',  # noqa: E501
         'created_at': 'created_at',  # noqa: E501
         'created_by': 'created_by',  # noqa: E501
         'current_size': 'current_size',  # noqa: E501
         'default_pod_count': 'default_pod_count',  # noqa: E501
         'default_vi': 'default_vi',  # noqa: E501
         'description': 'description',  # noqa: E501
         'desired_size': 'desired_size',  # noqa: E501
+        'enable_remount_on_resume': 'enable_remount_on_resume',  # noqa: E501
         'id': 'id',  # noqa: E501
         'monitoring_enabled': 'monitoring_enabled',  # noqa: E501
+        'mount_refresh_interval_seconds': 'mount_refresh_interval_seconds',  # noqa: E501
         'resumed_at': 'resumed_at',  # noqa: E501
         'rrn': 'rrn',  # noqa: E501
         'scaled_pod_count': 'scaled_pod_count',  # noqa: E501
         'state': 'state',  # noqa: E501
         'stats': 'stats',  # noqa: E501
     }
 
@@ -209,24 +217,27 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            auto_scaling_policy (AutoScalingPolicy): [optional]  # noqa: E501
             auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
             created_at (str): ISO-8601 date of when virtual instance was created.. [optional]  # noqa: E501
             created_by (str): Creator of requested virtual instance.. [optional]  # noqa: E501
             current_size (str): Virtual instance current size.. [optional]  # noqa: E501
             default_pod_count (int): [optional]  # noqa: E501
             default_vi (bool): [optional]  # noqa: E501
             description (str): Virtual instance description.. [optional]  # noqa: E501
             desired_size (str): Virtual instance desired size.. [optional]  # noqa: E501
+            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]  # noqa: E501
             id (str): Unique identifier for virtual instance.. [optional]  # noqa: E501
             monitoring_enabled (bool): [optional]  # noqa: E501
+            mount_refresh_interval_seconds (int): Number of seconds between data refreshes for mounts on this Virtual Instance. [optional]  # noqa: E501
             resumed_at (str): ISO-8601 date of when virtual instance was created.. [optional]  # noqa: E501
             rrn (str): Virtual Instance RRN.. [optional]  # noqa: E501
             scaled_pod_count (int): [optional]  # noqa: E501
             state (str): Virtual instance state.. [optional]  # noqa: E501
             stats (VirtualInstanceStats): [optional]  # noqa: E501
         """
 
@@ -277,22 +288,25 @@
 
     @convert_js_args_to_python_args
     def __init__(self, *, name, **kwargs):  # noqa: E501
         """VirtualInstance - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Virtual instance name.
+            auto_scaling_policy (AutoScalingPolicy): [optional]  # noqa: E501
             auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
             created_at (str): ISO-8601 date of when virtual instance was created.. [optional]  # noqa: E501
             created_by (str): Creator of requested virtual instance.. [optional]  # noqa: E501
             default_pod_count (int): [optional]  # noqa: E501
             default_vi (bool): [optional]  # noqa: E501
             description (str): Virtual instance description.. [optional]  # noqa: E501
+            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]  # noqa: E501
             id (str): Unique identifier for virtual instance.. [optional]  # noqa: E501
             monitoring_enabled (bool): [optional]  # noqa: E501
+            mount_refresh_interval_seconds (int): Number of seconds between data refreshes for mounts on this Virtual Instance. [optional]  # noqa: E501
             resumed_at (str): ISO-8601 date of when virtual instance was created.. [optional]  # noqa: E501
             rrn (str): Virtual Instance RRN.. [optional]  # noqa: E501
             scaled_pod_count (int): [optional]  # noqa: E501
             state (str): Virtual instance state.. [optional]  # noqa: E501
             stats (VirtualInstanceStats): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
```

### Comparing `rockset-2.0.0/rockset/model/virtual_instance_stats.py` & `rockset-2.0.2/rockset/model/delete_source_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rockset.model.source import Source
+    globals()['Source'] = Source
 
-class VirtualInstanceStats(ModelNormal):
+
+class DeleteSourceResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,50 +66,52 @@
 
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
-            'last_queried_ms': (int, none_type),  # noqa: E501
+            'data': (Source, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'last_queried_ms': 'last_queried_ms',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """VirtualInstanceStats - a model defined in OpenAPI
+        """DeleteSourceResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,15 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            last_queried_ms (int): Milliseconds since Unix epoch Jan 1, 1970.. [optional]  # noqa: E501
+            data (Source): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -179,18 +185,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """VirtualInstanceStats - a model defined in OpenAPI
+        """DeleteSourceResponse - a model defined in OpenAPI
 
         Keyword Args:
-            last_queried_ms (int): Milliseconds since Unix epoch Jan 1, 1970.. [optional]  # noqa: E501
+            data (Source): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/workspace.py` & `rockset-2.0.2/rockset/model/update_collection_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from rockset.model.field_mapping_query import FieldMappingQuery
+    globals()['FieldMappingQuery'] = FieldMappingQuery
 
-class Workspace(ModelNormal):
+
+class UpdateCollectionRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,58 +66,54 @@
 
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
-            'collection_count': (int, none_type),  # noqa: E501
-            'created_at': (str, none_type),  # noqa: E501
-            'created_by': (str, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
-            'name': (str, none_type),  # noqa: E501
+            'field_mapping_query': (FieldMappingQuery, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'collection_count': 'collection_count',  # noqa: E501
-        'created_at': 'created_at',  # noqa: E501
-        'created_by': 'created_by',  # noqa: E501
         'description': 'description',  # noqa: E501
-        'name': 'name',  # noqa: E501
+        'field_mapping_query': 'field_mapping_query',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Workspace - a model defined in OpenAPI
+        """UpdateCollectionRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,19 +138,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            collection_count (int): Number of collections that are immediate children of workspace.. [optional]  # noqa: E501
-            created_at (str): ISO-8601 date of when workspace was created.. [optional]  # noqa: E501
-            created_by (str): Email of user who created the workspace.. [optional]  # noqa: E501
-            description (str): Longer explanation for the workspace.. [optional]  # noqa: E501
-            name (str): Descriptive label and unique identifier.. [optional]  # noqa: E501
+            description (str): Updated text describing the collection.. [optional]  # noqa: E501
+            field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,22 +188,19 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
-        """Workspace - a model defined in OpenAPI
+        """UpdateCollectionRequest - a model defined in OpenAPI
 
         Keyword Args:
-            collection_count (int): Number of collections that are immediate children of workspace.. [optional]  # noqa: E501
-            created_at (str): ISO-8601 date of when workspace was created.. [optional]  # noqa: E501
-            created_by (str): Email of user who created the workspace.. [optional]  # noqa: E501
-            description (str): Longer explanation for the workspace.. [optional]  # noqa: E501
-            name (str): Descriptive label and unique identifier.. [optional]  # noqa: E501
+            description (str): Updated text describing the collection.. [optional]  # noqa: E501
+            field_mapping_query (FieldMappingQuery): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.0.0/rockset/model/xml_params.py` & `rockset-2.0.2/rockset/model/create_virtual_instance_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 
-class XmlParams(ModelNormal):
+class CreateVirtualInstanceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -51,14 +51,28 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('type',): {
+            'FREE': "FREE",
+            'NANO': "NANO",
+            'SHARED': "SHARED",
+            'MILLI': "MILLI",
+            'SMALL': "SMALL",
+            'MEDIUM': "MEDIUM",
+            'LARGE': "LARGE",
+            'XLARGE': "XLARGE",
+            'XLARGE2': "XLARGE2",
+            'XLARGE4': "XLARGE4",
+            'XLARGE8': "XLARGE8",
+            'XLARGE16': "XLARGE16",
+        },
     }
 
     validations = {
     }
 
     @cached_property
     def additional_properties_type():
@@ -77,43 +91,48 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'attribute_prefix': (str, none_type),  # noqa: E501
-            'doc_tag': (str, none_type),  # noqa: E501
-            'encoding': (str, none_type),  # noqa: E501
-            'root_tag': (str, none_type),  # noqa: E501
-            'value_tag': (str, none_type),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'auto_suspend_seconds': (int, none_type),  # noqa: E501
+            'description': (str, none_type),  # noqa: E501
+            'enable_remount_on_resume': (bool, none_type),  # noqa: E501
+            'mount_refresh_interval_seconds': (int, none_type),  # noqa: E501
+            'type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'attribute_prefix': 'attribute_prefix',  # noqa: E501
-        'doc_tag': 'doc_tag',  # noqa: E501
-        'encoding': 'encoding',  # noqa: E501
-        'root_tag': 'root_tag',  # noqa: E501
-        'value_tag': 'value_tag',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'auto_suspend_seconds': 'auto_suspend_seconds',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'enable_remount_on_resume': 'enable_remount_on_resume',  # noqa: E501
+        'mount_refresh_interval_seconds': 'mount_refresh_interval_seconds',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """XmlParams - a model defined in OpenAPI
+    def _from_openapi_data(cls, name, *args, **kwargs):  # noqa: E501
+        """CreateVirtualInstanceRequest - a model defined in OpenAPI
+
+        Args:
+            name (str): Unique identifier for virtual instance, can contain alphanumeric or dash characters.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,19 +157,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            attribute_prefix (str): Tag to differentiate between attributes and elements.. [optional]  # noqa: E501
-            doc_tag (str): Tags with which documents are identified.. [optional]  # noqa: E501
-            encoding (str): Encoding in which data source is encoded.. [optional]  # noqa: E501
-            root_tag (str): Tag until which xml is ignored.. [optional]  # noqa: E501
-            value_tag (str): tag used for the value when there are attributes in the element having no child. [optional]  # noqa: E501
+            auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
+            description (str): Description of requested virtual instance.. [optional]  # noqa: E501
+            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]  # noqa: E501
+            mount_refresh_interval_seconds (int): Number of seconds between data refreshes for mounts on this Virtual Instance. A value of 0 means continuous refresh and a value of null means never refresh.. [optional]  # noqa: E501
+            type (str): Requested virtual instance type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -170,14 +189,15 @@
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
@@ -190,23 +210,24 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, **kwargs):  # noqa: E501
-        """XmlParams - a model defined in OpenAPI
+    def __init__(self, *, name, **kwargs):  # noqa: E501
+        """CreateVirtualInstanceRequest - a model defined in OpenAPI
 
         Keyword Args:
-            attribute_prefix (str): Tag to differentiate between attributes and elements.. [optional]  # noqa: E501
-            doc_tag (str): Tags with which documents are identified.. [optional]  # noqa: E501
-            encoding (str): Encoding in which data source is encoded.. [optional]  # noqa: E501
-            root_tag (str): Tag until which xml is ignored.. [optional]  # noqa: E501
-            value_tag (str): tag used for the value when there are attributes in the element having no child. [optional]  # noqa: E501
+            name (str): Unique identifier for virtual instance, can contain alphanumeric or dash characters.
+            auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
+            description (str): Description of requested virtual instance.. [optional]  # noqa: E501
+            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]  # noqa: E501
+            mount_refresh_interval_seconds (int): Number of seconds between data refreshes for mounts on this Virtual Instance. A value of 0 means continuous refresh and a value of null means never refresh.. [optional]  # noqa: E501
+            type (str): Requested virtual instance type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -255,14 +276,15 @@
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

### Comparing `rockset-2.0.0/rockset/model_utils.py` & `rockset-2.0.2/rockset/model_utils.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/models/__init__.py` & `rockset-2.0.2/rockset/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,26 @@
 # sys.setrecursionlimit(n)
 
 from rockset.model.add_documents_request import AddDocumentsRequest
 from rockset.model.add_documents_response import AddDocumentsResponse
 from rockset.model.alias import Alias
 from rockset.model.api_key import ApiKey
 from rockset.model.async_query_options import AsyncQueryOptions
+from rockset.model.auto_scaling_policy import AutoScalingPolicy
 from rockset.model.aws_access_key import AwsAccessKey
 from rockset.model.aws_role import AwsRole
 from rockset.model.azure_blob_storage_collection_creation_request import AzureBlobStorageCollectionCreationRequest
 from rockset.model.azure_blob_storage_integration import AzureBlobStorageIntegration
 from rockset.model.azure_blob_storage_integration_creation_request import AzureBlobStorageIntegrationCreationRequest
 from rockset.model.azure_blob_storage_source_wrapper import AzureBlobStorageSourceWrapper
 from rockset.model.azure_event_hubs_collection_creation_request import AzureEventHubsCollectionCreationRequest
 from rockset.model.azure_event_hubs_integration import AzureEventHubsIntegration
 from rockset.model.azure_event_hubs_integration_creation_request import AzureEventHubsIntegrationCreationRequest
 from rockset.model.azure_event_hubs_source_wrapper import AzureEventHubsSourceWrapper
-from rockset.model.azure_service_bus_collection_creation_request import AzureServiceBusCollectionCreationRequest
 from rockset.model.azure_service_bus_integration import AzureServiceBusIntegration
-from rockset.model.azure_service_bus_source_wrapper import AzureServiceBusSourceWrapper
 from rockset.model.bulk_stats import BulkStats
 from rockset.model.cancel_query_response import CancelQueryResponse
 from rockset.model.cluster import Cluster
 from rockset.model.collection import Collection
 from rockset.model.collection_mount import CollectionMount
 from rockset.model.collection_mount_response import CollectionMountResponse
 from rockset.model.collection_mount_stats import CollectionMountStats
@@ -61,14 +60,15 @@
 from rockset.model.delete_api_key_response import DeleteApiKeyResponse
 from rockset.model.delete_collection_response import DeleteCollectionResponse
 from rockset.model.delete_documents_request import DeleteDocumentsRequest
 from rockset.model.delete_documents_request_data import DeleteDocumentsRequestData
 from rockset.model.delete_documents_response import DeleteDocumentsResponse
 from rockset.model.delete_integration_response import DeleteIntegrationResponse
 from rockset.model.delete_query_lambda_response import DeleteQueryLambdaResponse
+from rockset.model.delete_source_response import DeleteSourceResponse
 from rockset.model.delete_user_response import DeleteUserResponse
 from rockset.model.delete_view_response import DeleteViewResponse
 from rockset.model.delete_virtual_instance_response import DeleteVirtualInstanceResponse
 from rockset.model.delete_workspace_response import DeleteWorkspaceResponse
 from rockset.model.document_status import DocumentStatus
 from rockset.model.dynamodb_collection_creation_request import DynamodbCollectionCreationRequest
 from rockset.model.dynamodb_integration import DynamodbIntegration
@@ -77,27 +77,26 @@
 from rockset.model.error_model import ErrorModel
 from rockset.model.event_time_info import EventTimeInfo
 from rockset.model.execute_public_query_lambda_request import ExecutePublicQueryLambdaRequest
 from rockset.model.execute_query_lambda_request import ExecuteQueryLambdaRequest
 from rockset.model.field_mapping_query import FieldMappingQuery
 from rockset.model.field_mapping_v2 import FieldMappingV2
 from rockset.model.field_partition import FieldPartition
-from rockset.model.file_upload_collection_creation_request import FileUploadCollectionCreationRequest
-from rockset.model.file_upload_source_wrapper import FileUploadSourceWrapper
 from rockset.model.format_params import FormatParams
 from rockset.model.gcp_service_account import GcpServiceAccount
 from rockset.model.gcs_collection_creation_request import GcsCollectionCreationRequest
 from rockset.model.gcs_integration import GcsIntegration
 from rockset.model.gcs_integration_creation_request import GcsIntegrationCreationRequest
 from rockset.model.gcs_source_wrapper import GcsSourceWrapper
 from rockset.model.get_alias_response import GetAliasResponse
 from rockset.model.get_api_key_response import GetApiKeyResponse
 from rockset.model.get_collection_response import GetCollectionResponse
 from rockset.model.get_integration_response import GetIntegrationResponse
 from rockset.model.get_query_response import GetQueryResponse
+from rockset.model.get_source_response import GetSourceResponse
 from rockset.model.get_view_response import GetViewResponse
 from rockset.model.get_virtual_instance_response import GetVirtualInstanceResponse
 from rockset.model.get_workspace_response import GetWorkspaceResponse
 from rockset.model.input_field import InputField
 from rockset.model.integration import Integration
 from rockset.model.kafka_collection_creation_request import KafkaCollectionCreationRequest
 from rockset.model.kafka_integration import KafkaIntegration
@@ -114,14 +113,15 @@
 from rockset.model.list_collections_response import ListCollectionsResponse
 from rockset.model.list_integrations_response import ListIntegrationsResponse
 from rockset.model.list_queries_response import ListQueriesResponse
 from rockset.model.list_query_lambda_tags_response import ListQueryLambdaTagsResponse
 from rockset.model.list_query_lambda_versions_response import ListQueryLambdaVersionsResponse
 from rockset.model.list_query_lambdas_response import ListQueryLambdasResponse
 from rockset.model.list_roles_response import ListRolesResponse
+from rockset.model.list_sources_response import ListSourcesResponse
 from rockset.model.list_unsubscribe_preferences_response import ListUnsubscribePreferencesResponse
 from rockset.model.list_users_response import ListUsersResponse
 from rockset.model.list_views_response import ListViewsResponse
 from rockset.model.list_virtual_instances_response import ListVirtualInstancesResponse
 from rockset.model.list_workspaces_response import ListWorkspacesResponse
 from rockset.model.mongo_db_integration import MongoDbIntegration
 from rockset.model.mongodb_collection_creation_request import MongodbCollectionCreationRequest
@@ -172,15 +172,17 @@
 from rockset.model.source_dynamo_db import SourceDynamoDb
 from rockset.model.source_file_upload import SourceFileUpload
 from rockset.model.source_gcs import SourceGcs
 from rockset.model.source_kafka import SourceKafka
 from rockset.model.source_kinesis import SourceKinesis
 from rockset.model.source_mongo_db import SourceMongoDb
 from rockset.model.source_s3 import SourceS3
+from rockset.model.source_snapshot import SourceSnapshot
 from rockset.model.source_snowflake import SourceSnowflake
+from rockset.model.source_system import SourceSystem
 from rockset.model.sql_expression import SqlExpression
 from rockset.model.stats import Stats
 from rockset.model.status import Status
 from rockset.model.status_azure_event_hubs import StatusAzureEventHubs
 from rockset.model.status_azure_event_hubs_partition import StatusAzureEventHubsPartition
 from rockset.model.status_azure_service_bus import StatusAzureServiceBus
 from rockset.model.status_azure_service_bus_session import StatusAzureServiceBusSession
@@ -191,14 +193,15 @@
 from rockset.model.status_mongo_db import StatusMongoDb
 from rockset.model.status_snowflake import StatusSnowflake
 from rockset.model.suspend_virtual_instance_response import SuspendVirtualInstanceResponse
 from rockset.model.unsubscribe_preference import UnsubscribePreference
 from rockset.model.update_alias_request import UpdateAliasRequest
 from rockset.model.update_api_key_request import UpdateApiKeyRequest
 from rockset.model.update_api_key_response import UpdateApiKeyResponse
+from rockset.model.update_collection_request import UpdateCollectionRequest
 from rockset.model.update_query_lambda_request import UpdateQueryLambdaRequest
 from rockset.model.update_role_request import UpdateRoleRequest
 from rockset.model.update_unsubscribe_preferences_request import UpdateUnsubscribePreferencesRequest
 from rockset.model.update_unsubscribe_preferences_response import UpdateUnsubscribePreferencesResponse
 from rockset.model.update_user_request import UpdateUserRequest
 from rockset.model.update_view_request import UpdateViewRequest
 from rockset.model.update_view_response import UpdateViewResponse
```

### Comparing `rockset-2.0.0/rockset/query_paginator.py` & `rockset-2.0.2/rockset/query_paginator.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/rest.py` & `rockset-2.0.2/rockset/rest.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/rockset/rockset_client.py` & `rockset-2.0.2/rockset/rockset_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,24 +14,24 @@
     CustomRoles,
     Documents,
     Integrations,
     Organizations,
     Queries,
     QueryLambdas,
     SharedLambdas,
+    Sources,
     Users,
     Views,
     VirtualInstances,
     Workspaces,
 )
 from rockset.configuration import Configuration
 from rockset.exceptions import ApiTypeError, ApiValueError, InitializationException
 from rockset.models import QueryParameter, QueryRequestSql, QueryResponse
 
-
 APISERVER_PATTERN = re.compile(r"^https:\/\/(\w|-|\.)+\.rockset\.com$")
 
 
 class Regions(str, Enum):
     rs2 = "https://api.rs2.usw2.rockset.com"
     use1a1 = "https://api.use1a1.rockset.com"
     euc1a1 = "https://api.euc1a1.rockset.com"
@@ -72,14 +72,21 @@
             except TypeError as e:
                 raise ApiValueError(
                     f"Body for the request ({req_type}) could not be created because of a missing argument: {e}"
                 ) from e
 
             other_args[body_param_name] = body
 
+        # A way to pass in arguments that will make it to the body.
+        # This is not officially supported, arguments sent in this way have no compatability gaurentees.
+        if "add_raw_args_to_body" in other_args:
+            for raw_key, raw_value in other_args["add_raw_args_to_body"].items():
+                other_args[body_param_name][raw_key] = raw_value
+            del other_args["add_raw_args_to_body"]
+
         return method(*args, **other_args)
 
     return wrapped
 
 
 class ApiMetaclass(type):
     def __new__(cls, className, bases, classDict):
@@ -150,14 +157,18 @@
     pass
 
 
 class SharedLambdasApiWrapper(SharedLambdas, metaclass=ApiMetaclass):
     pass
 
 
+class SourcesApiWrapper(Sources, metaclass=ApiMetaclass):
+    pass
+
+
 class UsersApiWrapper(Users, metaclass=ApiMetaclass):
     pass
 
 
 class ViewsApiWrapper(Views, metaclass=ApiMetaclass):
     pass
 
@@ -251,22 +262,23 @@
         self.CustomRoles = CustomRolesApiWrapper(self.api_client)
         self.Documents = DocumentsApiWrapper(self.api_client)
         self.Integrations = IntegrationsApiWrapper(self.api_client)
         self.Organizations = OrganizationsApiWrapper(self.api_client)
         self.Queries = QueriesApiWrapper(self.api_client)
         self.QueryLambdas = QueryLambdasApiWrapper(self.api_client)
         self.SharedLambdas = SharedLambdasApiWrapper(self.api_client)
+        self.Sources = SourcesApiWrapper(self.api_client)
         self.Users = UsersApiWrapper(self.api_client)
         self.Views = ViewsApiWrapper(self.api_client)
         self.VirtualInstances = VirtualInstancesApiWrapper(self.api_client)
         self.Workspaces = WorkspacesApiWrapper(self.api_client)
 
     def sql(self, query: str, params: Dict[str, Any] = None) -> QueryResponse:
         """Convenience method for making queries."""
-        if params:
+        if params is not None:
             params = [
                 QueryParameter(
                     name=param, value=str(val), type=convert_to_rockset_type(val)
                 )
                 for param, val in params.items()
             ]
```

### Comparing `rockset-2.0.0/rockset/value.py` & `rockset-2.0.2/rockset/value.py`

 * *Files identical despite different names*

### Comparing `rockset-2.0.0/PKG-INFO` & `rockset-2.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockset
-Version: 2.0.0
+Version: 2.0.2
 Summary: The python client for the Rockset API.
 Home-page: https://github.com/rockset/rockset-python-client
 License: Apache-2.0
 Author: Rockset
 Author-email: support@rockset.com
 Requires-Python: >=3.6,<4.0
 Classifier: Environment :: Console
@@ -17,18 +17,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
```

