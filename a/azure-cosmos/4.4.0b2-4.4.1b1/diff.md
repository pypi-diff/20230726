# Comparing `tmp/azure-cosmos-4.4.0b2.zip` & `tmp/azure-cosmos-4.4.1b1.zip`

## zipinfo {}

```diff
@@ -1,177 +1,177 @@
-Zip file size: 452043 bytes, number of entries: 175
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure_cosmos.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/test/
--rw-rw-r--  2.0 unx     1073 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/LICENSE
--rw-rw-r--  2.0 unx      147 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/Contributing.md
--rw-rw-r--  2.0 unx     2416 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/setup.py
--rw-rw-r--  2.0 unx    19741 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/CHANGELOG.md
--rw-rw-r--  2.0 unx    34526 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/README.md
--rw-rw-r--  2.0 unx       38 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/setup.cfg
--rw-rw-r--  2.0 unx    55251 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/PKG-INFO
--rw-rw-r--  2.0 unx       99 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/pyproject.toml
--rw-rw-r--  2.0 unx      149 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/MANIFEST.in
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/samples/MultiMasterOperations/
--rw-rw-r--  2.0 unx     8376 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/examples_async.py
--rw-rw-r--  2.0 unx     6419 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/database_management_async.py
--rw-rw-r--  2.0 unx     5234 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/access_cosmos_with_aad_async.py
--rw-rw-r--  2.0 unx    13997 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/container_management_async.py
--rw-rw-r--  2.0 unx     2538 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/client_user_configs.py
--rw-rw-r--  2.0 unx     2640 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/tracing_open_telemetry.py
--rw-rw-r--  2.0 unx    30428 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/index_management_async.py
--rw-rw-r--  2.0 unx    11297 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/container_management.py
--rw-rw-r--  2.0 unx    30131 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/index_management.py
--rw-rw-r--  2.0 unx     6438 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/examples.py
--rw-rw-r--  2.0 unx     3581 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/README.md
--rw-rw-r--  2.0 unx     9407 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/access_cosmos_with_resource_token.py
--rw-rw-r--  2.0 unx    11590 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/document_management.py
--rw-rw-r--  2.0 unx     4258 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/change_feed_management_async.py
--rw-rw-r--  2.0 unx     4292 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/database_management.py
--rw-rw-r--  2.0 unx      820 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/config.py
--rw-rw-r--  2.0 unx    10642 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/access_cosmos_with_resource_token_async.py
--rw-rw-r--  2.0 unx     2571 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/client_user_configs_async.py
--rw-rw-r--  2.0 unx     4484 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/access_cosmos_with_aad.py
--rw-rw-r--  2.0 unx    13013 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/document_management_async.py
--rw-rw-r--  2.0 unx     3794 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/change_feed_management.py
--rw-rw-r--  2.0 unx     4083 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/MultiMasterOperations/MultiMasterScenario.py
--rw-rw-r--  2.0 unx     2843 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/MultiMasterOperations/Worker.py
--rw-rw-r--  2.0 unx      318 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/MultiMasterOperations/Program.py
--rw-rw-r--  2.0 unx      402 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/MultiMasterOperations/Configurations.py
--rw-rw-r--  2.0 unx    35093 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/samples/MultiMasterOperations/ConflictWorker.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure/cosmos/
--rw-rw-r--  2.0 unx       81 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure/cosmos/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure/cosmos/_routing/
--rw-rw-r--  2.0 unx     2603 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/offer.py
--rw-rw-r--  2.0 unx    19609 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/scripts.py
--rw-rw-r--  2.0 unx    10529 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_retry_utility.py
--rw-rw-r--  2.0 unx     1848 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/permission.py
--rw-rw-r--  2.0 unx     2720 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/diagnostics.py
--rw-rw-r--  2.0 unx    29424 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_base.py
--rw-rw-r--  2.0 unx     6575 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_vector_session_token.py
--rw-rw-r--  2.0 unx     3695 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_timeout_failover_retry_policy.py
--rw-rw-r--  2.0 unx    12763 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/user.py
--rw-rw-r--  2.0 unx     2430 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_retry_options.py
--rw-rw-r--  2.0 unx     2593 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_partition.py
--rw-rw-r--  2.0 unx     3274 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_default_retry_policy.py
--rw-rw-r--  2.0 unx    44598 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/container.py
--rw-rw-r--  2.0 unx     2861 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/partition_key.py
--rw-rw-r--  2.0 unx    15269 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/documents.py
--rw-rw-r--  2.0 unx     2302 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_gone_retry_policy.py
--rw-rw-r--  2.0 unx    39514 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/database.py
--rw-rw-r--  2.0 unx     3427 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/exceptions.py
--rw-rw-r--  2.0 unx     4798 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_range_partition_resolver.py
--rw-rw-r--  2.0 unx    14934 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_location_cache.py
--rw-rw-r--  2.0 unx    14926 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/http_constants.py
--rw-rw-r--  2.0 unx     2992 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_resource_throttle_retry_policy.py
--rw-rw-r--  2.0 unx     6007 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/auth.py
--rw-rw-r--  2.0 unx     5771 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_session_retry_policy.py
--rw-rw-r--  2.0 unx    24316 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/cosmos_client.py
--rw-rw-r--  2.0 unx     2200 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/__init__.py
--rw-rw-r--  2.0 unx     1142 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_version.py
--rw-rw-r--  2.0 unx     1696 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_runtime_constants.py
--rw-rw-r--  2.0 unx     1990 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_utils.py
--rw-rw-r--  2.0 unx     7909 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_synchronized_request.py
--rw-rw-r--  2.0 unx        0 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/py.typed
--rw-rw-r--  2.0 unx     3478 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_cosmos_http_logging_policy.py
--rw-rw-r--  2.0 unx     2258 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_request_object.py
--rw-rw-r--  2.0 unx     1509 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/errors.py
--rw-rw-r--  2.0 unx     7801 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_global_endpoint_manager.py
--rw-rw-r--  2.0 unx     1753 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_constants.py
--rw-rw-r--  2.0 unx     2806 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_range.py
--rw-rw-r--  2.0 unx     9656 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_session.py
--rw-rw-r--  2.0 unx     4685 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_endpoint_discovery_retry_policy.py
--rw-rw-r--  2.0 unx    97299 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_cosmos_client_connection.py
--rw-rw-r--  2.0 unx     7198 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_auth_policy.py
--rw-rw-r--  2.0 unx     3996 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_query_iterable.py
--rw-rw-r--  2.0 unx    95918 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_cosmos_client_connection_async.py
--rw-rw-r--  2.0 unx     7230 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_asynchronous_request.py
--rw-rw-r--  2.0 unx    20800 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_cosmos_client.py
--rw-rw-r--  2.0 unx    14320 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_user.py
--rw-rw-r--  2.0 unx    22102 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_scripts.py
--rw-rw-r--  2.0 unx     8185 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_auth_policy_async.py
--rw-rw-r--  2.0 unx     9962 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_retry_utility_async.py
--rw-rw-r--  2.0 unx     7761 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_global_endpoint_manager_async.py
--rw-rw-r--  2.0 unx     1417 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/__init__.py
--rw-rw-r--  2.0 unx    43363 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_container.py
--rw-rw-r--  2.0 unx     4215 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_query_iterable_async.py
--rw-rw-r--  2.0 unx    39434 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/aio/_database.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/
--rw-rw-r--  2.0 unx     4697 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/query_execution_info.py
--rw-rw-r--  2.0 unx     7627 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/endpoint_component.py
--rw-rw-r--  2.0 unx     8091 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/multi_execution_aggregator.py
--rw-rw-r--  2.0 unx     3295 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aggregators.py
--rw-rw-r--  2.0 unx     9096 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/execution_dispatcher.py
--rw-rw-r--  2.0 unx     1121 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/__init__.py
--rw-rw-r--  2.0 unx     6113 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/base_execution_context.py
--rw-rw-r--  2.0 unx     9259 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/document_producer.py
--rw-rw-r--  2.0 unx     7472 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/endpoint_component.py
--rw-rw-r--  2.0 unx     8507 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py
--rw-rw-r--  2.0 unx     8955 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/execution_dispatcher.py
--rw-rw-r--  2.0 unx     1121 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/__init__.py
--rw-rw-r--  2.0 unx     6197 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/base_execution_context.py
--rw-rw-r--  2.0 unx     3220 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/_queue_async_helper.py
--rw-rw-r--  2.0 unx     9210 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/document_producer.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/
--rw-rw-r--  2.0 unx     7964 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_routing/routing_map_provider.py
--rw-rw-r--  2.0 unx     4520 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_routing/routing_range.py
--rw-rw-r--  2.0 unx     1121 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_routing/__init__.py
--rw-rw-r--  2.0 unx     7528 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_routing/collection_routing_map.py
--rw-rw-r--  2.0 unx     8085 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/routing_map_provider.py
--rw-rw-r--  2.0 unx     1121 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/__init__.py
--rw-rw-r--  2.0 unx        1 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/azure_cosmos.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/azure_cosmos.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx     5263 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/azure_cosmos.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx    55251 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/azure_cosmos.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx       26 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/azure_cosmos.egg-info/requires.txt
--rw-rw-r--  2.0 unx        6 b- defN 23-May-22 15:33 azure-cosmos-4.4.0b2/azure_cosmos.egg-info/top_level.txt
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-22 15:33 azure-cosmos-4.4.0b2/test/routing/
--rw-rw-r--  2.0 unx     3985 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_session_token_unit.py
--rw-rw-r--  2.0 unx   123357 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_crud.py
--rw-rw-r--  2.0 unx    24366 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_location_cache.py
--rw-rw-r--  2.0 unx    12416 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_multi_orderby.py
--rw-rw-r--  2.0 unx    14793 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_ttl.py
--rw-rw-r--  2.0 unx     2382 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_media.py
--rw-rw-r--  2.0 unx     4317 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_partition_key.py
--rw-rw-r--  2.0 unx     7167 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_auto_scale.py
--rw-rw-r--  2.0 unx   128585 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_crud_async.py
--rw-rw-r--  2.0 unx     8455 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_config.py
--rw-rw-r--  2.0 unx     4003 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_routing_map.py
--rw-rw-r--  2.0 unx     1338 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/cleanup.py
--rw-rw-r--  2.0 unx     6967 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_user_configs.py
--rw-rw-r--  2.0 unx     9864 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_aggregate.py
--rw-rw-r--  2.0 unx     9482 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_globaldb_mock.py
--rw-rw-r--  2.0 unx     7579 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_auto_scale_async.py
--rw-rw-r--  2.0 unx    13679 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_analytical_ttl.py
--rw-rw-r--  2.0 unx     2960 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_encoding.py
--rw-rw-r--  2.0 unx    15048 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_retry_policy.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_cosmos_http_logging_policy.py
--rw-rw-r--  2.0 unx     4541 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_backwards_compatibility.py
--rw-rw-r--  2.0 unx    26150 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_globaldb.py
--rw-rw-r--  2.0 unx     3879 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_headers.py
--rw-rw-r--  2.0 unx     9224 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_query_execution_context.py
--rw-rw-r--  2.0 unx     3861 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_session_container.py
--rw-rw-r--  2.0 unx     5354 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_session.py
--rw-rw-r--  2.0 unx     5014 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_multimaster.py
--rw-rw-r--  2.0 unx     4384 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_env.py
--rw-rw-r--  2.0 unx     1357 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_diagnostics.py
--rw-rw-r--  2.0 unx     4204 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_proxy.py
--rw-rw-r--  2.0 unx     4762 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_integrated_cache.py
--rw-rw-r--  2.0 unx    22619 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_orderby.py
--rw-rw-r--  2.0 unx     2673 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_correlated_activity_id.py
--rw-rw-r--  2.0 unx      465 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_base_unit.py
--rw-rw-r--  2.0 unx     2120 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_utils.py
--rw-rw-r--  2.0 unx    13949 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_analytical_ttl_async.py
--rw-rw-r--  2.0 unx     8567 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_streaming_failover.py
--rw-rw-r--  2.0 unx     1508 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/conftest.py
--rw-rw-r--  2.0 unx    41041 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_query.py
--rw-rw-r--  2.0 unx     2335 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_client_user_agent.py
--rw-rw-r--  2.0 unx     4757 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_partition_split_query.py
--rw-rw-r--  2.0 unx     7087 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/test_aad.py
--rw-rw-r--  2.0 unx    10369 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/routing/test_collection_routing_map.py
--rw-rw-r--  2.0 unx     1103 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/routing/__init__.py
--rw-rw-r--  2.0 unx    10381 b- defN 23-May-22 15:32 azure-cosmos-4.4.0b2/test/routing/test_routing_map_provider.py
-175 files, 1847877 bytes uncompressed, 420669 bytes compressed:  77.2%
+Zip file size: 453812 bytes, number of entries: 175
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 21:23 azure-cosmos-4.4.1b1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 21:23 azure-cosmos-4.4.1b1/test/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 21:23 azure-cosmos-4.4.1b1/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 21:23 azure-cosmos-4.4.1b1/azure_cosmos.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 21:23 azure-cosmos-4.4.1b1/azure/
+-rw-rw-r--  2.0 unx    20376 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/CHANGELOG.md
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jul-25 21:23 azure-cosmos-4.4.1b1/setup.cfg
+-rw-rw-r--  2.0 unx    55886 b- defN 23-Jul-25 21:23 azure-cosmos-4.4.1b1/PKG-INFO
+-rw-rw-r--  2.0 unx     2416 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/setup.py
+-rw-rw-r--  2.0 unx    34526 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/README.md
+-rw-rw-r--  2.0 unx      147 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/Contributing.md
+-rw-rw-r--  2.0 unx      149 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/MANIFEST.in
+-rw-rw-r--  2.0 unx      113 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/pyproject.toml
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/LICENSE
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 21:23 azure-cosmos-4.4.1b1/test/routing/
+-rw-rw-r--  2.0 unx     3985 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_session_token_unit.py
+-rw-rw-r--  2.0 unx     2673 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_correlated_activity_id.py
+-rw-rw-r--  2.0 unx     1357 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_diagnostics.py
+-rw-rw-r--  2.0 unx     4541 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_backwards_compatibility.py
+-rw-rw-r--  2.0 unx     7167 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_auto_scale.py
+-rw-rw-r--  2.0 unx     4317 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_partition_key.py
+-rw-rw-r--  2.0 unx      465 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_base_unit.py
+-rw-rw-r--  2.0 unx     9224 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_query_execution_context.py
+-rw-rw-r--  2.0 unx     5354 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_session.py
+-rw-rw-r--  2.0 unx     3861 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_session_container.py
+-rw-rw-r--  2.0 unx     4384 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_env.py
+-rw-rw-r--  2.0 unx    15048 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_retry_policy.py
+-rw-rw-r--  2.0 unx     5014 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_multimaster.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_cosmos_http_logging_policy.py
+-rw-rw-r--  2.0 unx     4003 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_routing_map.py
+-rw-rw-r--  2.0 unx    14793 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_ttl.py
+-rw-rw-r--  2.0 unx     1338 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/cleanup.py
+-rw-rw-r--  2.0 unx     6967 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_user_configs.py
+-rw-rw-r--  2.0 unx     2960 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_encoding.py
+-rw-rw-r--  2.0 unx     4762 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_integrated_cache.py
+-rw-rw-r--  2.0 unx     3879 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_headers.py
+-rw-rw-r--  2.0 unx     9864 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_aggregate.py
+-rw-rw-r--  2.0 unx     7087 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_aad.py
+-rw-rw-r--  2.0 unx     4757 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_partition_split_query.py
+-rw-rw-r--  2.0 unx     2382 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_media.py
+-rw-rw-r--  2.0 unx    12416 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_multi_orderby.py
+-rw-rw-r--  2.0 unx     7579 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_auto_scale_async.py
+-rw-rw-r--  2.0 unx    13679 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_analytical_ttl.py
+-rw-rw-r--  2.0 unx    26150 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_globaldb.py
+-rw-rw-r--  2.0 unx     1508 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/conftest.py
+-rw-rw-r--  2.0 unx     2120 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_utils.py
+-rw-rw-r--  2.0 unx   128585 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_crud_async.py
+-rw-rw-r--  2.0 unx    13949 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_analytical_ttl_async.py
+-rw-rw-r--  2.0 unx     4204 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_proxy.py
+-rw-rw-r--  2.0 unx    42060 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_query.py
+-rw-rw-r--  2.0 unx    22619 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_orderby.py
+-rw-rw-r--  2.0 unx     2335 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_client_user_agent.py
+-rw-rw-r--  2.0 unx     8455 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_config.py
+-rw-rw-r--  2.0 unx   123357 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_crud.py
+-rw-rw-r--  2.0 unx     8567 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_streaming_failover.py
+-rw-rw-r--  2.0 unx    24366 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_location_cache.py
+-rw-rw-r--  2.0 unx     9482 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/test_globaldb_mock.py
+-rw-rw-r--  2.0 unx    10369 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/routing/test_collection_routing_map.py
+-rw-rw-r--  2.0 unx     1103 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/routing/__init__.py
+-rw-rw-r--  2.0 unx    10381 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/test/routing/test_routing_map_provider.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 21:23 azure-cosmos-4.4.1b1/samples/MultiMasterOperations/
+-rw-rw-r--  2.0 unx     2538 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/client_user_configs.py
+-rw-rw-r--  2.0 unx     2571 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/client_user_configs_async.py
+-rw-rw-r--  2.0 unx    11297 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/container_management.py
+-rw-rw-r--  2.0 unx     4292 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/database_management.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/config.py
+-rw-rw-r--  2.0 unx     3794 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/change_feed_management.py
+-rw-rw-r--  2.0 unx     3581 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/README.md
+-rw-rw-r--  2.0 unx     6419 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/database_management_async.py
+-rw-rw-r--  2.0 unx     8376 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/examples_async.py
+-rw-rw-r--  2.0 unx    30428 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/index_management_async.py
+-rw-rw-r--  2.0 unx     5234 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/access_cosmos_with_aad_async.py
+-rw-rw-r--  2.0 unx    12267 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/document_management.py
+-rw-rw-r--  2.0 unx    30131 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/index_management.py
+-rw-rw-r--  2.0 unx     4484 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/access_cosmos_with_aad.py
+-rw-rw-r--  2.0 unx     4258 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/change_feed_management_async.py
+-rw-rw-r--  2.0 unx    13706 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/document_management_async.py
+-rw-rw-r--  2.0 unx    13997 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/container_management_async.py
+-rw-rw-r--  2.0 unx    10642 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/access_cosmos_with_resource_token_async.py
+-rw-rw-r--  2.0 unx     6438 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/examples.py
+-rw-rw-r--  2.0 unx     9407 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/access_cosmos_with_resource_token.py
+-rw-rw-r--  2.0 unx     2640 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/tracing_open_telemetry.py
+-rw-rw-r--  2.0 unx    35093 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/MultiMasterOperations/ConflictWorker.py
+-rw-rw-r--  2.0 unx      402 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/MultiMasterOperations/Configurations.py
+-rw-rw-r--  2.0 unx      318 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/MultiMasterOperations/Program.py
+-rw-rw-r--  2.0 unx     2843 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/MultiMasterOperations/Worker.py
+-rw-rw-r--  2.0 unx     4083 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/samples/MultiMasterOperations/MultiMasterScenario.py
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jul-25 21:23 azure-cosmos-4.4.1b1/azure_cosmos.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx    55886 b- defN 23-Jul-25 21:23 azure-cosmos-4.4.1b1/azure_cosmos.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx     5263 b- defN 23-Jul-25 21:23 azure-cosmos-4.4.1b1/azure_cosmos.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-25 21:23 azure-cosmos-4.4.1b1/azure_cosmos.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-25 21:23 azure-cosmos-4.4.1b1/azure_cosmos.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-25 21:23 azure-cosmos-4.4.1b1/azure_cosmos.egg-info/requires.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 21:23 azure-cosmos-4.4.1b1/azure/cosmos/
+-rw-rw-r--  2.0 unx       81 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 21:23 azure-cosmos-4.4.1b1/azure/cosmos/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 21:23 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 21:23 azure-cosmos-4.4.1b1/azure/cosmos/_routing/
+-rw-rw-r--  2.0 unx     6007 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/auth.py
+-rw-rw-r--  2.0 unx     1753 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_constants.py
+-rw-rw-r--  2.0 unx     7198 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_auth_policy.py
+-rw-rw-r--  2.0 unx     2806 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_range.py
+-rw-rw-r--  2.0 unx     2603 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/offer.py
+-rw-rw-r--  2.0 unx     5771 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_session_retry_policy.py
+-rw-rw-r--  2.0 unx    45978 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/container.py
+-rw-rw-r--  2.0 unx    15043 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/http_constants.py
+-rw-rw-r--  2.0 unx     3996 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_query_iterable.py
+-rw-rw-r--  2.0 unx     2200 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/__init__.py
+-rw-rw-r--  2.0 unx    10529 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_retry_utility.py
+-rw-rw-r--  2.0 unx     4798 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_range_partition_resolver.py
+-rw-rw-r--  2.0 unx     3478 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_cosmos_http_logging_policy.py
+-rw-rw-r--  2.0 unx    14934 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_location_cache.py
+-rw-rw-r--  2.0 unx     1848 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/permission.py
+-rw-rw-r--  2.0 unx     2861 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/partition_key.py
+-rw-rw-r--  2.0 unx    97299 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_cosmos_client_connection.py
+-rw-rw-r--  2.0 unx     4685 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_endpoint_discovery_retry_policy.py
+-rw-rw-r--  2.0 unx     3427 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/exceptions.py
+-rw-rw-r--  2.0 unx     2720 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/diagnostics.py
+-rw-rw-r--  2.0 unx     1696 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_runtime_constants.py
+-rw-rw-r--  2.0 unx    29642 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_base.py
+-rw-rw-r--  2.0 unx     7909 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_synchronized_request.py
+-rw-rw-r--  2.0 unx     3695 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_timeout_failover_retry_policy.py
+-rw-rw-r--  2.0 unx    19609 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/scripts.py
+-rw-rw-r--  2.0 unx     1509 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/errors.py
+-rw-rw-r--  2.0 unx     2302 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_gone_retry_policy.py
+-rw-rw-r--  2.0 unx     2992 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_resource_throttle_retry_policy.py
+-rw-rw-r--  2.0 unx     2593 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_partition.py
+-rw-rw-r--  2.0 unx     2430 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_retry_options.py
+-rw-rw-r--  2.0 unx     1990 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_utils.py
+-rw-rw-r--  2.0 unx    12763 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/user.py
+-rw-rw-r--  2.0 unx    39514 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/database.py
+-rw-rw-r--  2.0 unx     6575 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_vector_session_token.py
+-rw-rw-r--  2.0 unx     3274 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_default_retry_policy.py
+-rw-rw-r--  2.0 unx     9656 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_session.py
+-rw-rw-r--  2.0 unx     2258 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_request_object.py
+-rw-rw-r--  2.0 unx    24650 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/cosmos_client.py
+-rw-rw-r--  2.0 unx    15269 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/documents.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/py.typed
+-rw-rw-r--  2.0 unx     7801 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_global_endpoint_manager.py
+-rw-rw-r--  2.0 unx     1142 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_version.py
+-rw-rw-r--  2.0 unx    21134 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/aio/_cosmos_client.py
+-rw-rw-r--  2.0 unx    39434 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/aio/_database.py
+-rw-rw-r--  2.0 unx     1417 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/aio/__init__.py
+-rw-rw-r--  2.0 unx     7230 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/aio/_asynchronous_request.py
+-rw-rw-r--  2.0 unx    95918 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/aio/_cosmos_client_connection_async.py
+-rw-rw-r--  2.0 unx     4215 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/aio/_query_iterable_async.py
+-rw-rw-r--  2.0 unx     8185 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/aio/_auth_policy_async.py
+-rw-rw-r--  2.0 unx    14320 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/aio/_user.py
+-rw-rw-r--  2.0 unx     9962 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/aio/_retry_utility_async.py
+-rw-rw-r--  2.0 unx    44742 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/aio/_container.py
+-rw-rw-r--  2.0 unx    22102 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/aio/_scripts.py
+-rw-rw-r--  2.0 unx     7761 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/aio/_global_endpoint_manager_async.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 21:23 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/
+-rw-rw-r--  2.0 unx     7627 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/endpoint_component.py
+-rw-rw-r--  2.0 unx     6113 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/base_execution_context.py
+-rw-rw-r--  2.0 unx     1121 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/__init__.py
+-rw-rw-r--  2.0 unx     9259 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/document_producer.py
+-rw-rw-r--  2.0 unx     9096 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/execution_dispatcher.py
+-rw-rw-r--  2.0 unx     4697 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/query_execution_info.py
+-rw-rw-r--  2.0 unx     3295 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aggregators.py
+-rw-rw-r--  2.0 unx     8091 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/multi_execution_aggregator.py
+-rw-rw-r--  2.0 unx     7472 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/endpoint_component.py
+-rw-rw-r--  2.0 unx     6197 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/base_execution_context.py
+-rw-rw-r--  2.0 unx     3220 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/_queue_async_helper.py
+-rw-rw-r--  2.0 unx     1121 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/__init__.py
+-rw-rw-r--  2.0 unx     9210 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/document_producer.py
+-rw-rw-r--  2.0 unx     8955 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/execution_dispatcher.py
+-rw-rw-r--  2.0 unx     8507 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-25 21:23 azure-cosmos-4.4.1b1/azure/cosmos/_routing/aio/
+-rw-rw-r--  2.0 unx     7964 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_routing/routing_map_provider.py
+-rw-rw-r--  2.0 unx     7528 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_routing/collection_routing_map.py
+-rw-rw-r--  2.0 unx     1121 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_routing/__init__.py
+-rw-rw-r--  2.0 unx     4520 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_routing/routing_range.py
+-rw-rw-r--  2.0 unx     8085 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_routing/aio/routing_map_provider.py
+-rw-rw-r--  2.0 unx     1121 b- defN 23-Jul-25 21:22 azure-cosmos-4.4.1b1/azure/cosmos/_routing/aio/__init__.py
+175 files, 1855947 bytes uncompressed, 422438 bytes compressed:  77.2%
```

## zipnote {}

```diff
@@ -1,526 +1,526 @@
-Filename: azure-cosmos-4.4.0b2/
+Filename: azure-cosmos-4.4.1b1/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/
+Filename: azure-cosmos-4.4.1b1/test/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/
+Filename: azure-cosmos-4.4.1b1/samples/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure_cosmos.egg-info/
+Filename: azure-cosmos-4.4.1b1/azure_cosmos.egg-info/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/
+Filename: azure-cosmos-4.4.1b1/azure/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/LICENSE
+Filename: azure-cosmos-4.4.1b1/CHANGELOG.md
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/Contributing.md
+Filename: azure-cosmos-4.4.1b1/setup.cfg
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/setup.py
+Filename: azure-cosmos-4.4.1b1/PKG-INFO
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/CHANGELOG.md
+Filename: azure-cosmos-4.4.1b1/setup.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/README.md
+Filename: azure-cosmos-4.4.1b1/README.md
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/setup.cfg
+Filename: azure-cosmos-4.4.1b1/Contributing.md
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/PKG-INFO
+Filename: azure-cosmos-4.4.1b1/MANIFEST.in
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/pyproject.toml
+Filename: azure-cosmos-4.4.1b1/pyproject.toml
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/MANIFEST.in
+Filename: azure-cosmos-4.4.1b1/LICENSE
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/MultiMasterOperations/
+Filename: azure-cosmos-4.4.1b1/test/routing/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/examples_async.py
+Filename: azure-cosmos-4.4.1b1/test/test_session_token_unit.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/database_management_async.py
+Filename: azure-cosmos-4.4.1b1/test/test_correlated_activity_id.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/access_cosmos_with_aad_async.py
+Filename: azure-cosmos-4.4.1b1/test/test_diagnostics.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/container_management_async.py
+Filename: azure-cosmos-4.4.1b1/test/test_backwards_compatibility.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/client_user_configs.py
+Filename: azure-cosmos-4.4.1b1/test/test_auto_scale.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/tracing_open_telemetry.py
+Filename: azure-cosmos-4.4.1b1/test/test_partition_key.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/index_management_async.py
+Filename: azure-cosmos-4.4.1b1/test/test_base_unit.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/container_management.py
+Filename: azure-cosmos-4.4.1b1/test/test_query_execution_context.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/index_management.py
+Filename: azure-cosmos-4.4.1b1/test/test_session.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/examples.py
+Filename: azure-cosmos-4.4.1b1/test/test_session_container.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/README.md
+Filename: azure-cosmos-4.4.1b1/test/test_env.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/access_cosmos_with_resource_token.py
+Filename: azure-cosmos-4.4.1b1/test/test_retry_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/document_management.py
+Filename: azure-cosmos-4.4.1b1/test/test_multimaster.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/change_feed_management_async.py
+Filename: azure-cosmos-4.4.1b1/test/test_cosmos_http_logging_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/database_management.py
+Filename: azure-cosmos-4.4.1b1/test/test_routing_map.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/config.py
+Filename: azure-cosmos-4.4.1b1/test/test_ttl.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/access_cosmos_with_resource_token_async.py
+Filename: azure-cosmos-4.4.1b1/test/cleanup.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/client_user_configs_async.py
+Filename: azure-cosmos-4.4.1b1/test/test_user_configs.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/access_cosmos_with_aad.py
+Filename: azure-cosmos-4.4.1b1/test/test_encoding.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/document_management_async.py
+Filename: azure-cosmos-4.4.1b1/test/test_integrated_cache.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/change_feed_management.py
+Filename: azure-cosmos-4.4.1b1/test/test_headers.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/MultiMasterOperations/MultiMasterScenario.py
+Filename: azure-cosmos-4.4.1b1/test/test_aggregate.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/MultiMasterOperations/Worker.py
+Filename: azure-cosmos-4.4.1b1/test/test_aad.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/MultiMasterOperations/Program.py
+Filename: azure-cosmos-4.4.1b1/test/test_partition_split_query.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/MultiMasterOperations/Configurations.py
+Filename: azure-cosmos-4.4.1b1/test/test_media.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/samples/MultiMasterOperations/ConflictWorker.py
+Filename: azure-cosmos-4.4.1b1/test/test_multi_orderby.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/
+Filename: azure-cosmos-4.4.1b1/test/test_auto_scale_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/__init__.py
+Filename: azure-cosmos-4.4.1b1/test/test_analytical_ttl.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/
+Filename: azure-cosmos-4.4.1b1/test/test_globaldb.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/
+Filename: azure-cosmos-4.4.1b1/test/conftest.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/
+Filename: azure-cosmos-4.4.1b1/test/test_utils.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/offer.py
+Filename: azure-cosmos-4.4.1b1/test/test_crud_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/scripts.py
+Filename: azure-cosmos-4.4.1b1/test/test_analytical_ttl_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_retry_utility.py
+Filename: azure-cosmos-4.4.1b1/test/test_proxy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/permission.py
+Filename: azure-cosmos-4.4.1b1/test/test_query.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/diagnostics.py
+Filename: azure-cosmos-4.4.1b1/test/test_orderby.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_base.py
+Filename: azure-cosmos-4.4.1b1/test/test_client_user_agent.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_vector_session_token.py
+Filename: azure-cosmos-4.4.1b1/test/test_config.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_timeout_failover_retry_policy.py
+Filename: azure-cosmos-4.4.1b1/test/test_crud.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/user.py
+Filename: azure-cosmos-4.4.1b1/test/test_streaming_failover.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_retry_options.py
+Filename: azure-cosmos-4.4.1b1/test/test_location_cache.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_partition.py
+Filename: azure-cosmos-4.4.1b1/test/test_globaldb_mock.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_default_retry_policy.py
+Filename: azure-cosmos-4.4.1b1/test/routing/test_collection_routing_map.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/container.py
+Filename: azure-cosmos-4.4.1b1/test/routing/__init__.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/partition_key.py
+Filename: azure-cosmos-4.4.1b1/test/routing/test_routing_map_provider.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/documents.py
+Filename: azure-cosmos-4.4.1b1/samples/MultiMasterOperations/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_gone_retry_policy.py
+Filename: azure-cosmos-4.4.1b1/samples/client_user_configs.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/database.py
+Filename: azure-cosmos-4.4.1b1/samples/client_user_configs_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/exceptions.py
+Filename: azure-cosmos-4.4.1b1/samples/container_management.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_range_partition_resolver.py
+Filename: azure-cosmos-4.4.1b1/samples/database_management.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_location_cache.py
+Filename: azure-cosmos-4.4.1b1/samples/config.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/http_constants.py
+Filename: azure-cosmos-4.4.1b1/samples/change_feed_management.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_resource_throttle_retry_policy.py
+Filename: azure-cosmos-4.4.1b1/samples/README.md
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/auth.py
+Filename: azure-cosmos-4.4.1b1/samples/database_management_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_session_retry_policy.py
+Filename: azure-cosmos-4.4.1b1/samples/examples_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/cosmos_client.py
+Filename: azure-cosmos-4.4.1b1/samples/index_management_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/__init__.py
+Filename: azure-cosmos-4.4.1b1/samples/access_cosmos_with_aad_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_version.py
+Filename: azure-cosmos-4.4.1b1/samples/document_management.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_runtime_constants.py
+Filename: azure-cosmos-4.4.1b1/samples/index_management.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_utils.py
+Filename: azure-cosmos-4.4.1b1/samples/access_cosmos_with_aad.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_synchronized_request.py
+Filename: azure-cosmos-4.4.1b1/samples/change_feed_management_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/py.typed
+Filename: azure-cosmos-4.4.1b1/samples/document_management_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_cosmos_http_logging_policy.py
+Filename: azure-cosmos-4.4.1b1/samples/container_management_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_request_object.py
+Filename: azure-cosmos-4.4.1b1/samples/access_cosmos_with_resource_token_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/errors.py
+Filename: azure-cosmos-4.4.1b1/samples/examples.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_global_endpoint_manager.py
+Filename: azure-cosmos-4.4.1b1/samples/access_cosmos_with_resource_token.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_constants.py
+Filename: azure-cosmos-4.4.1b1/samples/tracing_open_telemetry.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_range.py
+Filename: azure-cosmos-4.4.1b1/samples/MultiMasterOperations/ConflictWorker.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_session.py
+Filename: azure-cosmos-4.4.1b1/samples/MultiMasterOperations/Configurations.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_endpoint_discovery_retry_policy.py
+Filename: azure-cosmos-4.4.1b1/samples/MultiMasterOperations/Program.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_cosmos_client_connection.py
+Filename: azure-cosmos-4.4.1b1/samples/MultiMasterOperations/Worker.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_auth_policy.py
+Filename: azure-cosmos-4.4.1b1/samples/MultiMasterOperations/MultiMasterScenario.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_query_iterable.py
+Filename: azure-cosmos-4.4.1b1/azure_cosmos.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_cosmos_client_connection_async.py
+Filename: azure-cosmos-4.4.1b1/azure_cosmos.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_asynchronous_request.py
+Filename: azure-cosmos-4.4.1b1/azure_cosmos.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_cosmos_client.py
+Filename: azure-cosmos-4.4.1b1/azure_cosmos.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_user.py
+Filename: azure-cosmos-4.4.1b1/azure_cosmos.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_scripts.py
+Filename: azure-cosmos-4.4.1b1/azure_cosmos.egg-info/requires.txt
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_auth_policy_async.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_retry_utility_async.py
+Filename: azure-cosmos-4.4.1b1/azure/__init__.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_global_endpoint_manager_async.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/aio/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/__init__.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_container.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_routing/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_query_iterable_async.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/auth.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/aio/_database.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_constants.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_auth_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/query_execution_info.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_range.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/endpoint_component.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/offer.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/multi_execution_aggregator.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_session_retry_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aggregators.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/container.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/execution_dispatcher.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/http_constants.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/__init__.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_query_iterable.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/base_execution_context.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/__init__.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/document_producer.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_retry_utility.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/endpoint_component.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_range_partition_resolver.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_cosmos_http_logging_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/execution_dispatcher.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_location_cache.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/__init__.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/permission.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/base_execution_context.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/partition_key.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/_queue_async_helper.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_cosmos_client_connection.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/document_producer.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_endpoint_discovery_retry_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/exceptions.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/routing_map_provider.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/diagnostics.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/routing_range.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_runtime_constants.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/__init__.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_base.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/collection_routing_map.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_synchronized_request.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/routing_map_provider.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_timeout_failover_retry_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/__init__.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/scripts.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure_cosmos.egg-info/dependency_links.txt
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/errors.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure_cosmos.egg-info/not-zip-safe
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_gone_retry_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure_cosmos.egg-info/SOURCES.txt
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_resource_throttle_retry_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure_cosmos.egg-info/PKG-INFO
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_partition.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure_cosmos.egg-info/requires.txt
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_retry_options.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/azure_cosmos.egg-info/top_level.txt
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_utils.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/routing/
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/user.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_session_token_unit.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/database.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_crud.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_vector_session_token.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_location_cache.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_default_retry_policy.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_multi_orderby.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_session.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_ttl.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_request_object.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_media.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/cosmos_client.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_partition_key.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/documents.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_auto_scale.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/py.typed
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_crud_async.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_global_endpoint_manager.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_config.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_version.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_routing_map.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/aio/_cosmos_client.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/cleanup.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/aio/_database.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_user_configs.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/aio/__init__.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_aggregate.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/aio/_asynchronous_request.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_globaldb_mock.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/aio/_cosmos_client_connection_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_auto_scale_async.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/aio/_query_iterable_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_analytical_ttl.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/aio/_auth_policy_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_encoding.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/aio/_user.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_retry_policy.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/aio/_retry_utility_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_cosmos_http_logging_policy.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/aio/_container.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_backwards_compatibility.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/aio/_scripts.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_globaldb.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/aio/_global_endpoint_manager_async.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_headers.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_query_execution_context.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/endpoint_component.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_session_container.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/base_execution_context.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_session.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/__init__.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_multimaster.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/document_producer.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_env.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/execution_dispatcher.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_diagnostics.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/query_execution_info.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_proxy.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aggregators.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_integrated_cache.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/multi_execution_aggregator.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_orderby.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/endpoint_component.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_correlated_activity_id.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/base_execution_context.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_base_unit.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/_queue_async_helper.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_utils.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/__init__.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_analytical_ttl_async.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/document_producer.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_streaming_failover.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/execution_dispatcher.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/conftest.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_query.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_routing/aio/
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_client_user_agent.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_routing/routing_map_provider.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_partition_split_query.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_routing/collection_routing_map.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/test_aad.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_routing/__init__.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/routing/test_collection_routing_map.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_routing/routing_range.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/routing/__init__.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_routing/aio/routing_map_provider.py
 Comment: 
 
-Filename: azure-cosmos-4.4.0b2/test/routing/test_routing_map_provider.py
+Filename: azure-cosmos-4.4.1b1/azure/cosmos/_routing/aio/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-cosmos-4.4.0b2/LICENSE` & `azure-cosmos-4.4.1b1/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/setup.py` & `azure-cosmos-4.4.1b1/setup.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/CHANGELOG.md` & `azure-cosmos-4.4.1b1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 ## Release History
 
+### 4.4.1b1 (2023-07-25)
+
+#### Features Added
+* Added ability to limit continuation token size when querying for items. See [PR 30731](https://github.com/Azure/azure-sdk-for-python/pull/30731)
+
+#### Bugs Fixed
+* Fixed bug with async patch_item method. See [PR 30804](https://github.com/Azure/azure-sdk-for-python/pull/30804).
+
+### 4.4.0 (2023-06-09)
+
+#### Features Added
+- GA release of Patch API and Delete All Items By Partition Key
+
 ### 4.4.0b2 (2023-05-22)
 
 #### Features Added
 * Added conditional patching for Patch operations. See [PR 30455](https://github.com/Azure/azure-sdk-for-python/pull/30455).
 
 #### Bugs Fixed
 * Fixed bug with non english locales causing an error with the RFC 1123 Date Format. See [PR 30125](https://github.com/Azure/azure-sdk-for-python/pull/30125).
 
 #### Other Changes
 * Refactoring of our client `connection_timeout` and `request_timeout` configurations. See [PR 30171](https://github.com/Azure/azure-sdk-for-python/pull/30171).
 
 ### 4.4.0b1 (2023-04-11)
 
 #### Features Added
- - Added **preview** delete all items by partition key functionality. See [PR 29186](https://github.com/Azure/azure-sdk-for-python/pull/29186).
+ - Added **preview** delete all items by partition key functionality. See [PR 29186](https://github.com/Azure/azure-sdk-for-python/pull/29186). For more information on Partition Key Delete, please see [Azure Cosmos DB Partition Key Delete](https://learn.microsoft.com/azure/cosmos-db/nosql/how-to-delete-by-partition-key?tabs=python-example).
  - Added **preview** partial document update (Patch API) functionality and container methods for patching items with operations. See [PR 29497](https://github.com/Azure/azure-sdk-for-python/pull/29497). For more information on Patch, please see [Azure Cosmos DB Partial Document Update](https://learn.microsoft.com/azure/cosmos-db/partial-document-update).
 
 #### Bugs Fixed
 * Fixed bug in method `create_container_if_not_exists()` of async database client for unexpected kwargs being passed into `read()` method used internally. See [PR 29136](https://github.com/Azure/azure-sdk-for-python/pull/29136).
 * Fixed bug with method `query_items()` of our async container class, where partition key and cross partition headers would both be set when using partition keys. See [PR 29366](https://github.com/Azure/azure-sdk-for-python/pull/29366/).
 * Fixed bug with client not properly surfacing errors for invalid credentials and identities with insufficient permissions. Users running into 'NoneType has no attribute ConsistencyPolicy' errors when initializing their clients will now see proper authentication exceptions. See [PR 29256](https://github.com/Azure/azure-sdk-for-python/pull/29256).
```

## Comparing `azure-cosmos-4.4.0b2/README.md` & `azure-cosmos-4.4.1b1/README.md`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/PKG-INFO` & `azure-cosmos-4.4.1b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-cosmos
-Version: 4.4.0b2
+Version: 4.4.1b1
 Summary: Microsoft Azure Cosmos Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: askdocdb@microsoft.com
 Maintainer: Microsoft
 Maintainer-email: askdocdb@microsoft.com
 License: MIT License
@@ -756,29 +756,42 @@
 This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
 For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
 contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
 
 ## Release History
 
+### 4.4.1b1 (2023-07-25)
+
+#### Features Added
+* Added ability to limit continuation token size when querying for items. See [PR 30731](https://github.com/Azure/azure-sdk-for-python/pull/30731)
+
+#### Bugs Fixed
+* Fixed bug with async patch_item method. See [PR 30804](https://github.com/Azure/azure-sdk-for-python/pull/30804).
+
+### 4.4.0 (2023-06-09)
+
+#### Features Added
+- GA release of Patch API and Delete All Items By Partition Key
+
 ### 4.4.0b2 (2023-05-22)
 
 #### Features Added
 * Added conditional patching for Patch operations. See [PR 30455](https://github.com/Azure/azure-sdk-for-python/pull/30455).
 
 #### Bugs Fixed
 * Fixed bug with non english locales causing an error with the RFC 1123 Date Format. See [PR 30125](https://github.com/Azure/azure-sdk-for-python/pull/30125).
 
 #### Other Changes
 * Refactoring of our client `connection_timeout` and `request_timeout` configurations. See [PR 30171](https://github.com/Azure/azure-sdk-for-python/pull/30171).
 
 ### 4.4.0b1 (2023-04-11)
 
 #### Features Added
- - Added **preview** delete all items by partition key functionality. See [PR 29186](https://github.com/Azure/azure-sdk-for-python/pull/29186).
+ - Added **preview** delete all items by partition key functionality. See [PR 29186](https://github.com/Azure/azure-sdk-for-python/pull/29186). For more information on Partition Key Delete, please see [Azure Cosmos DB Partition Key Delete](https://learn.microsoft.com/azure/cosmos-db/nosql/how-to-delete-by-partition-key?tabs=python-example).
  - Added **preview** partial document update (Patch API) functionality and container methods for patching items with operations. See [PR 29497](https://github.com/Azure/azure-sdk-for-python/pull/29497). For more information on Patch, please see [Azure Cosmos DB Partial Document Update](https://learn.microsoft.com/azure/cosmos-db/partial-document-update).
 
 #### Bugs Fixed
 * Fixed bug in method `create_container_if_not_exists()` of async database client for unexpected kwargs being passed into `read()` method used internally. See [PR 29136](https://github.com/Azure/azure-sdk-for-python/pull/29136).
 * Fixed bug with method `query_items()` of our async container class, where partition key and cross partition headers would both be set when using partition keys. See [PR 29366](https://github.com/Azure/azure-sdk-for-python/pull/29366/).
 * Fixed bug with client not properly surfacing errors for invalid credentials and identities with insufficient permissions. Users running into 'NoneType has no attribute ConsistencyPolicy' errors when initializing their clients will now see proper authentication exceptions. See [PR 29256](https://github.com/Azure/azure-sdk-for-python/pull/29256).
```

## Comparing `azure-cosmos-4.4.0b2/samples/examples_async.py` & `azure-cosmos-4.4.1b1/samples/examples_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/database_management_async.py` & `azure-cosmos-4.4.1b1/samples/database_management_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/access_cosmos_with_aad_async.py` & `azure-cosmos-4.4.1b1/samples/access_cosmos_with_aad_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/container_management_async.py` & `azure-cosmos-4.4.1b1/samples/container_management_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/client_user_configs.py` & `azure-cosmos-4.4.1b1/samples/client_user_configs.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/tracing_open_telemetry.py` & `azure-cosmos-4.4.1b1/samples/tracing_open_telemetry.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/index_management_async.py` & `azure-cosmos-4.4.1b1/samples/index_management_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/container_management.py` & `azure-cosmos-4.4.1b1/samples/container_management.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/index_management.py` & `azure-cosmos-4.4.1b1/samples/index_management.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/examples.py` & `azure-cosmos-4.4.1b1/samples/examples.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/README.md` & `azure-cosmos-4.4.1b1/samples/README.md`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/access_cosmos_with_resource_token.py` & `azure-cosmos-4.4.1b1/samples/access_cosmos_with_resource_token.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/document_management.py` & `azure-cosmos-4.4.1b1/samples/document_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,14 +187,31 @@
     item_list = list(container.read_all_items())
 
     print('Found {0} items'.format(item_list.__len__()))
 
     for doc in item_list:
         print('Item Id: {0}; Partition Key: {1}'.format(doc.get('id'), doc.get("company")))
 
+
+def query_items_with_continuation_token_size_limit(container, doc_id):
+    print('\n1.11 Query Items With Continuation Token Size Limit.\n')
+
+    size_limit_in_kb = 8
+    sales_order = get_sales_order(doc_id)
+    container.create_item(body=sales_order)
+
+    # set response_continuation_token_limit_in_kb to 8 to limit size to 8KB
+    items = list(container.query_items(
+        query="SELECT * FROM r",
+        partition_key=doc_id,
+        response_continuation_token_limit_in_kb=size_limit_in_kb
+    ))
+
+    print('Continuation Token size has been limited to {}KB.'.format(size_limit_in_kb))
+
 def get_sales_order(item_id):
     order1 = {'id' : item_id,
             'account_number' : 'Account1',
             'purchase_order_number' : 'PO18009186470',
             'order_date' : datetime.date(2005,1,10).strftime('%c'),
             'subtotal' : 419.4589,
             'tax_amount' : 12.5838,
@@ -255,14 +272,15 @@
         query_items(container, 'SalesOrder1')
         replace_item(container, 'SalesOrder1')
         upsert_item(container, 'SalesOrder1')
         conditional_patch_item(container, 'SalesOrder1')
         patch_item(container, 'SalesOrder1')
         delete_item(container, 'SalesOrder1')
         delete_all_items_by_partition_key(db, "CompanyA")
+        query_items_with_continuation_token_size_limit(container, 'SalesOrder1')
 
         # cleanup database after sample
         try:
             client.delete_database(db)
 
         except exceptions.CosmosResourceNotFoundError:
             pass
```

## Comparing `azure-cosmos-4.4.0b2/samples/change_feed_management_async.py` & `azure-cosmos-4.4.1b1/samples/change_feed_management_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/database_management.py` & `azure-cosmos-4.4.1b1/samples/database_management.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/config.py` & `azure-cosmos-4.4.1b1/samples/config.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/access_cosmos_with_resource_token_async.py` & `azure-cosmos-4.4.1b1/samples/access_cosmos_with_resource_token_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/client_user_configs_async.py` & `azure-cosmos-4.4.1b1/samples/client_user_configs_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/access_cosmos_with_aad.py` & `azure-cosmos-4.4.1b1/samples/access_cosmos_with_aad.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/document_management_async.py` & `azure-cosmos-4.4.1b1/samples/document_management_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -204,14 +204,31 @@
     item_list = [item async for item in container.read_all_items()]
 
     print('Found {0} items'.format(item_list.__len__()))
 
     for doc in item_list:
         print('Item Id: {0}; Partition Key: {1}'.format(doc.get('id'), doc.get("company")))
 
+
+async def query_items_with_continuation_token_size_limit(container, doc_id):
+    print('\n1.11 Query Items With Continuation Token Size Limit.\n')
+
+    size_limit_in_kb = 8
+    sales_order = get_sales_order(doc_id)
+    await container.create_item(body=sales_order)
+
+    # set response_continuation_token_limit_in_kb to 8 to limit size to 8KB
+    items = container.query_items(
+        query="SELECT * FROM r",
+        partition_key=doc_id,
+        response_continuation_token_limit_in_kb=size_limit_in_kb
+    )
+
+    print('Continuation Token size has been limited to {}KB.'.format(size_limit_in_kb))
+
 def get_sales_order(item_id):
     order1 = {'id' : item_id,
             'account_number' : 'Account1',
             'purchase_order_number' : 'PO18009186470',
             'order_date' : datetime.date(2005,1,10).strftime('%c'),
             'subtotal' : 419.4589,
             'tax_amount' : 12.5838,
@@ -274,14 +291,15 @@
             await query_items(container, 'SalesOrder1')
             await replace_item(container, 'SalesOrder1')
             await upsert_item(container, 'SalesOrder1')
             await conditional_patch_item(container, 'SalesOrder1')
             await patch_item(container, 'SalesOrder1')
             await delete_item(container, 'SalesOrder1')
             await delete_all_items_by_partition_key(db, "CompanyA")
+            await query_items_with_continuation_token_size_limit(container, 'SalesOrder1')
 
             # cleanup database after sample
             try:
                 await client.delete_database(db)
 
             except exceptions.CosmosResourceNotFoundError:
                 pass
```

## Comparing `azure-cosmos-4.4.0b2/samples/change_feed_management.py` & `azure-cosmos-4.4.1b1/samples/change_feed_management.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/MultiMasterOperations/MultiMasterScenario.py` & `azure-cosmos-4.4.1b1/samples/MultiMasterOperations/MultiMasterScenario.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/MultiMasterOperations/Worker.py` & `azure-cosmos-4.4.1b1/samples/MultiMasterOperations/Worker.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/samples/MultiMasterOperations/ConflictWorker.py` & `azure-cosmos-4.4.1b1/samples/MultiMasterOperations/ConflictWorker.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/offer.py` & `azure-cosmos-4.4.1b1/azure/cosmos/offer.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/scripts.py` & `azure-cosmos-4.4.1b1/azure/cosmos/scripts.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_retry_utility.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_retry_utility.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/permission.py` & `azure-cosmos-4.4.1b1/azure/cosmos/permission.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/diagnostics.py` & `azure-cosmos-4.4.1b1/azure/cosmos/diagnostics.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_base.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,14 +219,17 @@
 
     if options.get("enableCrossPartitionQuery"):
         headers[http_constants.HttpHeaders.EnableCrossPartitionQuery] = options["enableCrossPartitionQuery"]
 
     if options.get("populateQueryMetrics"):
         headers[http_constants.HttpHeaders.PopulateQueryMetrics] = options["populateQueryMetrics"]
 
+    if options.get("responseContinuationTokenLimitInKb"):
+        headers[http_constants.HttpHeaders.ResponseContinuationTokenLimitInKb] = options["responseContinuationTokenLimitInKb"] # pylint: disable=line-too-long
+
     if cosmos_client_connection.master_key:
         #formatedate guarantees RFC 1123 date format regardless of current locale
         headers[http_constants.HttpHeaders.XDate] = formatdate(timeval=None, localtime=False, usegmt=True)
 
     if cosmos_client_connection.master_key or cosmos_client_connection.resource_tokens:
         resource_type = _internal_resourcetype(resource_type)
         authorization = auth._get_authorization_header(
```

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_vector_session_token.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_vector_session_token.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_timeout_failover_retry_policy.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_timeout_failover_retry_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/user.py` & `azure-cosmos-4.4.1b1/azure/cosmos/user.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_retry_options.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_retry_options.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_partition.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_partition.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_default_retry_policy.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_default_retry_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/container.py` & `azure-cosmos-4.4.1b1/azure/cosmos/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,14 +350,17 @@
         :param max_item_count: Max number of items to be returned in the enumeration operation.
         :param enable_scan_in_query: Allow scan on the queries which couldn't be served as
             indexing was opted out on the requested paths.
         :param populate_query_metrics: Enable returning query metrics in response headers.
         :keyword str session_token: Token for use with Session consistency.
         :keyword dict[str,str] initial_headers: Initial headers to be sent as part of the request.
         :keyword Callable response_hook: A callable invoked with the response metadata.
+        :keyword int response_continuation_token_limit_in_kb: **provisional keyword** The size limit in kb of the
+        response continuation token in the query response. Valid values are positive integers.
+        A value of 0 is the same as not passing a value (default no limit).
         :keyword int max_integrated_cache_staleness_in_ms: The max cache staleness for the integrated cache in
             milliseconds. For accounts configured to use the integrated cache, using Session or Eventual consistency,
             responses are guaranteed to be no staler than this value.
         :returns: An Iterable of items (dicts).
         :rtype: ItemPaged[Dict[str, Any]]
 
         .. admonition:: Example:
@@ -392,14 +395,17 @@
             feed_options["enableScanInQuery"] = enable_scan_in_query
         max_integrated_cache_staleness_in_ms = kwargs.pop('max_integrated_cache_staleness_in_ms', None)
         if max_integrated_cache_staleness_in_ms:
             validate_cache_staleness_value(max_integrated_cache_staleness_in_ms)
             feed_options["maxIntegratedCacheStaleness"] = max_integrated_cache_staleness_in_ms
         correlated_activity_id = GenerateGuidId()
         feed_options["correlatedActivityId"] = correlated_activity_id
+        response_continuation_token_limit_in_kb = kwargs.pop("response_continuation_token_limit_in_kb", None)
+        if response_continuation_token_limit_in_kb is not None:
+            feed_options["responseContinuationTokenLimitInKb"] = response_continuation_token_limit_in_kb
         if hasattr(response_hook, "clear"):
             response_hook.clear()
 
         items = self.client_connection.QueryItems(
             database_or_container_link=self.container_link,
             query=query if parameters is None else dict(query=query, parameters=parameters),
             options=feed_options,
@@ -589,15 +595,14 @@
         :type partition_key: Union[str, int, float, bool]
         :param patch_operations: The list of patch operations to apply to the item.
         :type patch_operations: List[Dict[str, Any]]
         :keyword str filter_predicate: conditional filter to apply to Patch operations.
         :keyword str pre_trigger_include: trigger id to be used as pre operation trigger.
         :keyword str post_trigger_include: trigger id to be used as post operation trigger.
         :keyword str session_token: Token for use with Session consistency.
-        :keyword dict[str,str] initial_headers: Initial headers to be sent as part of the request.
         :keyword str etag: An ETag value, or the wildcard character (*). Used to check if the resource
             has changed, and act according to the condition specified by the `match_condition` parameter.
         :keyword ~azure.core.MatchConditions match_condition: The match condition to use upon the etag.
         :keyword Callable response_hook: A callable invoked with the response metadata.
         :returns: A dict representing the item after the patch operations went through.
         :raises ~azure.cosmos.exceptions.CosmosHttpResponseError: The patch operations failed or the item with
             given id does not exist.
@@ -866,19 +871,29 @@
 
     @distributed_trace
     def delete_all_items_by_partition_key(
         self,
         partition_key: Union[str, int, float, bool],
         **kwargs: Any
     ) -> None:
-        """Exposes an API to delete all items with a single partition key without the user having
-         to explicitly call delete on each record in the partition key.
+        """The delete by partition key feature is an asynchronous, background operation that allows you to delete all
+        documents with the same logical partition key value, using the Cosmos SDK. The delete by partition key
+        operation is constrained to consume at most 10% of the total
+        available RU/s on the container each second. This helps in limiting the resources used by
+        this background task.
 
         :param partition_key: Partition key for the items to be deleted.
         :type partition_key: Any
+        :keyword str pre_trigger_include: trigger id to be used as pre operation trigger.
+        :keyword str post_trigger_include: trigger id to be used as post operation trigger.
+        :keyword str session_token: Token for use with Session consistency.
+        :keyword str etag: An ETag value, or the wildcard character (*). Used to check if the resource
+            has changed, and act according to the condition specified by the `match_condition` parameter.
+        :keyword ~azure.core.MatchConditions match_condition: The match condition to use upon the etag.
+        :keyword Callable response_hook: A callable invoked with the response metadata.
         :rtype: None
         """
         request_options = build_options(kwargs)
         response_hook = kwargs.pop('response_hook', None)
         # regardless if partition key is valid we set it as invalid partition keys are set to a default empty value
         request_options["partitionKey"] = self._set_partition_key(partition_key)
```

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/partition_key.py` & `azure-cosmos-4.4.1b1/azure/cosmos/partition_key.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/documents.py` & `azure-cosmos-4.4.1b1/azure/cosmos/documents.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_gone_retry_policy.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_gone_retry_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/database.py` & `azure-cosmos-4.4.1b1/azure/cosmos/database.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/exceptions.py` & `azure-cosmos-4.4.1b1/azure/cosmos/exceptions.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_range_partition_resolver.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_range_partition_resolver.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_location_cache.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_location_cache.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/http_constants.py` & `azure-cosmos-4.4.1b1/azure/cosmos/http_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
     QueryVersion = "x-ms-cosmos-query-version"
     QueryMetrics = "x-ms-documentdb-query-metrics"
     QueryExecutionInfo = "x-ms-cosmos-query-execution-info"
 
     # Our custom DocDB headers
     Continuation = "x-ms-continuation"
     PageSize = "x-ms-max-item-count"
+    ResponseContinuationTokenLimitInKb = "x-ms-documentdb-responsecontinuationtokenlimitinkb"  # cspell:disable-line
 
     # Request sender generated. Simply echoed by backend.
     ActivityId = "x-ms-activity-id"
     CorrelatedActivityId = "x-ms-cosmos-correlated-activityid"  # cspell:disable-line
     PreTriggerInclude = "x-ms-documentdb-pre-trigger-include"
     PreTriggerExclude = "x-ms-documentdb-pre-trigger-exclude"
     PostTriggerInclude = "x-ms-documentdb-post-trigger-include"
```

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_resource_throttle_retry_policy.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_resource_throttle_retry_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/auth.py` & `azure-cosmos-4.4.1b1/azure/cosmos/auth.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_session_retry_policy.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_session_retry_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/cosmos_client.py` & `azure-cosmos-4.4.1b1/azure/cosmos/cosmos_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,20 @@
 
 
 class CosmosClient(object):  # pylint: disable=client-accepts-api-version-keyword
     """A client-side logical representation of an Azure Cosmos DB account.
 
     Use this client to configure and execute requests to the Azure Cosmos DB service.
 
+    Its recommended to maintain a single instance of CosmosClient per lifetime of the application which enables
+        efficient connection management and performance.
+
+    CosmosClient initialization is a heavy operation - don't use initialization CosmosClient instances as
+        credentials or network connectivity validations.
+
     :param str url: The URL of the Cosmos DB account.
     :param credential: Can be the account key, or a dictionary of resource tokens.
     :type credential: Union[str, Dict[str, str], ~azure.core.credentials.TokenCredential]
     :param str consistency_level: Consistency level to use for the session. The default value is None (Account level).
         More on consistency levels and possible values: https://aka.ms/cosmos-consistency-levels
     :keyword int timeout: An absolute timeout in seconds, for the combined HTTP request and response processing.
     :keyword int connection_timeout: The HTTP request timeout in seconds.
```

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/__init__.py` & `azure-cosmos-4.4.1b1/azure/cosmos/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_version.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-VERSION = "4.4.0b2"
+VERSION = "4.4.1b1"
```

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_runtime_constants.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_runtime_constants.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_utils.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_utils.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_synchronized_request.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_synchronized_request.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_cosmos_http_logging_policy.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_cosmos_http_logging_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_request_object.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_request_object.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/errors.py` & `azure-cosmos-4.4.1b1/azure/cosmos/errors.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_global_endpoint_manager.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_global_endpoint_manager.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_constants.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_constants.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_range.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_range.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_session.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_session.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_endpoint_discovery_retry_policy.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_endpoint_discovery_retry_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_cosmos_client_connection.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_cosmos_client_connection.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_auth_policy.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_auth_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_query_iterable.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_query_iterable.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/aio/_cosmos_client_connection_async.py` & `azure-cosmos-4.4.1b1/azure/cosmos/aio/_cosmos_client_connection_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/aio/_asynchronous_request.py` & `azure-cosmos-4.4.1b1/azure/cosmos/aio/_asynchronous_request.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/aio/_cosmos_client.py` & `azure-cosmos-4.4.1b1/azure/cosmos/aio/_cosmos_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,20 @@
 
 
 class CosmosClient(object):  # pylint: disable=client-accepts-api-version-keyword
     """A client-side logical representation of an Azure Cosmos DB account.
 
     Use this client to configure and execute requests to the Azure Cosmos DB service.
 
+    Its recommended to maintain a single instance of CosmosClient per lifetime of the application which enables
+        efficient connection management and performance.
+
+    CosmosClient initialization is a heavy operation - don't use initialization CosmosClient instances as
+        credentials or network connectivity validations.
+
     :param str url: The URL of the Cosmos DB account.
     :param credential: Can be the account key, or a dictionary of resource tokens.
     :type credential: Union[str, Dict[str, str], ~azure.core.credentials_async.AsyncTokenCredential]
     :keyword str consistency_level: Consistency level to use for the session. Default value is None (account-level).
         More on consistency levels and possible values: https://aka.ms/cosmos-consistency-levels
     :keyword int timeout: An absolute timeout in seconds, for the combined HTTP request and response processing.
     :keyword int connection_timeout: The HTTP request timeout in seconds.
```

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/aio/_user.py` & `azure-cosmos-4.4.1b1/azure/cosmos/aio/_user.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/aio/_scripts.py` & `azure-cosmos-4.4.1b1/azure/cosmos/aio/_scripts.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/aio/_auth_policy_async.py` & `azure-cosmos-4.4.1b1/azure/cosmos/aio/_auth_policy_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/aio/_retry_utility_async.py` & `azure-cosmos-4.4.1b1/azure/cosmos/aio/_retry_utility_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/aio/_global_endpoint_manager_async.py` & `azure-cosmos-4.4.1b1/azure/cosmos/aio/_global_endpoint_manager_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/aio/__init__.py` & `azure-cosmos-4.4.1b1/azure/cosmos/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/aio/_container.py` & `azure-cosmos-4.4.1b1/azure/cosmos/aio/_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,14 +316,17 @@
         :keyword bool enable_scan_in_query: Allow scan on the queries which couldn't be served as
             indexing was opted out on the requested paths.
         :keyword bool populate_query_metrics: Enable returning query metrics in response headers.
         :keyword str session_token: Token for use with Session consistency.
         :keyword dict[str, str] initial_headers: Initial headers to be sent as part of the request.
         :keyword response_hook: A callable invoked with the response metadata.
         :paramtype response_hook: Callable[[Dict[str, str], AsyncItemPaged[Dict[str, Any]]], None]
+        :keyword int response_continuation_token_limit_in_kb: **provisional keyword** The size limit in kb of the
+        response continuation token in the query response. Valid values are positive integers.
+        A value of 0 is the same as not passing a value (default no limit).
         :keyword int max_integrated_cache_staleness_in_ms: The max cache staleness for the integrated cache in
             milliseconds. For accounts configured to use the integrated cache, using Session or Eventual consistency,
             responses are guaranteed to be no staler than this value.
         :returns: An AsyncItemPaged of items (dicts).
         :rtype: AsyncItemPaged[Dict[str, Any]]
 
         .. admonition:: Example:
@@ -362,17 +365,21 @@
             feed_options["enableCrossPartitionQuery"] = True
         max_integrated_cache_staleness_in_ms = kwargs.pop('max_integrated_cache_staleness_in_ms', None)
         if max_integrated_cache_staleness_in_ms:
             validate_cache_staleness_value(max_integrated_cache_staleness_in_ms)
             feed_options["maxIntegratedCacheStaleness"] = max_integrated_cache_staleness_in_ms
         correlated_activity_id = GenerateGuidId()
         feed_options["correlatedActivityId"] = correlated_activity_id
+        response_continuation_token_limit_in_kb = kwargs.pop("response_continuation_token_limit_in_kb", None)
+        if response_continuation_token_limit_in_kb is not None:
+            feed_options["responseContinuationTokenLimitInKb"] = response_continuation_token_limit_in_kb
         if hasattr(response_hook, "clear"):
             response_hook.clear()
 
+
         parameters = kwargs.pop('parameters', None)
         items = self.client_connection.QueryItems(
             database_or_container_link=self.container_link,
             query=query if parameters is None else dict(query=query, parameters=parameters),
             options=feed_options,
             partition_key=partition_key,
             response_hook=response_hook,
@@ -541,29 +548,28 @@
         :type partition_key: Union[str, int, float, bool]
         :param patch_operations: The list of patch operations to apply to the item.
         :type patch_operations: List[Dict[str, Any]]
         :keyword str filter_predicate: conditional filter to apply to Patch operations.
         :keyword str pre_trigger_include: trigger id to be used as pre operation trigger.
         :keyword str post_trigger_include: trigger id to be used as post operation trigger.
         :keyword str session_token: Token for use with Session consistency.
-        :keyword dict[str,str] initial_headers: Initial headers to be sent as part of the request.
         :keyword str etag: An ETag value, or the wildcard character (*). Used to check if the resource
             has changed, and act according to the condition specified by the `match_condition` parameter.
         :keyword ~azure.core.MatchConditions match_condition: The match condition to use upon the etag.
         :keyword Callable response_hook: A callable invoked with the response metadata.
         :returns: A dict representing the item after the patch operations went through.
         :raises ~azure.cosmos.exceptions.CosmosHttpResponseError: The patch operations failed or the item with
             given id does not exist.
         :rtype: dict[str, Any]
         """
         request_options = _build_options(kwargs)
         response_hook = kwargs.pop('response_hook', None)
         request_options["disableAutomaticIdGeneration"] = True
         request_options["partitionKey"] = partition_key
-        filter_predicate = kwargs.pop("filter_predicate")
+        filter_predicate = kwargs.pop("filter_predicate", None)
         if filter_predicate is not None:
             request_options["filterPredicate"] = filter_predicate
 
         item_link = self._get_document_link(item)
         result = await self.client_connection.PatchItem(
             document_link=item_link, operations=patch_operations, options=request_options, **kwargs)
         if response_hook:
@@ -811,19 +817,29 @@
 
     @distributed_trace_async
     async def delete_all_items_by_partition_key(
         self,
         partition_key: Union[str, int, float, bool],
         **kwargs: Any
     ) -> None:
-        """Exposes an API to delete all items with a single partition key without the user having
-                 to explicitly call delete on each record in the partition key.
+        """The delete by partition key feature is an asynchronous, background operation that allows you to delete all
+        documents with the same logical partition key value, using the Cosmos SDK. The delete by partition key
+        operation is constrained to consume at most 10% of the total
+        available RU/s on the container each second. This helps in limiting the resources used by
+        this background task.
 
         :param partition_key: Partition key for the items to be deleted.
         :type partition_key: Any
+        :keyword str pre_trigger_include: trigger id to be used as pre operation trigger.
+        :keyword str post_trigger_include: trigger id to be used as post operation trigger.
+        :keyword str session_token: Token for use with Session consistency.
+        :keyword str etag: An ETag value, or the wildcard character (*). Used to check if the resource
+            has changed, and act according to the condition specified by the `match_condition` parameter.
+        :keyword ~azure.core.MatchConditions match_condition: The match condition to use upon the etag.
+        :keyword Callable response_hook: A callable invoked with the response metadata.
         :rtype: None
         """
         request_options = _build_options(kwargs)
         response_hook = kwargs.pop('response_hook', None)
         # regardless if partition key is valid we set it as invalid partition keys are set to a default empty value
         request_options["partitionKey"] = self._set_partition_key(partition_key)
```

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/aio/_query_iterable_async.py` & `azure-cosmos-4.4.1b1/azure/cosmos/aio/_query_iterable_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/aio/_database.py` & `azure-cosmos-4.4.1b1/azure/cosmos/aio/_database.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/query_execution_info.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/query_execution_info.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/endpoint_component.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/endpoint_component.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/multi_execution_aggregator.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/multi_execution_aggregator.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aggregators.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aggregators.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/execution_dispatcher.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/execution_dispatcher.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/__init__.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/base_execution_context.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/base_execution_context.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/document_producer.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/document_producer.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/endpoint_component.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/endpoint_component.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/execution_dispatcher.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/execution_dispatcher.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/__init__.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/base_execution_context.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/base_execution_context.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/_queue_async_helper.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/_queue_async_helper.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_execution_context/aio/document_producer.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_execution_context/aio/document_producer.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_routing/routing_map_provider.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_routing/routing_map_provider.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_routing/routing_range.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_routing/routing_range.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_routing/__init__.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_routing/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_routing/collection_routing_map.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_routing/collection_routing_map.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/routing_map_provider.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_routing/aio/routing_map_provider.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure/cosmos/_routing/aio/__init__.py` & `azure-cosmos-4.4.1b1/azure/cosmos/_routing/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure_cosmos.egg-info/SOURCES.txt` & `azure-cosmos-4.4.1b1/azure_cosmos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/azure_cosmos.egg-info/PKG-INFO` & `azure-cosmos-4.4.1b1/azure_cosmos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-cosmos
-Version: 4.4.0b2
+Version: 4.4.1b1
 Summary: Microsoft Azure Cosmos Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: askdocdb@microsoft.com
 Maintainer: Microsoft
 Maintainer-email: askdocdb@microsoft.com
 License: MIT License
@@ -756,29 +756,42 @@
 This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
 For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
 contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
 
 ## Release History
 
+### 4.4.1b1 (2023-07-25)
+
+#### Features Added
+* Added ability to limit continuation token size when querying for items. See [PR 30731](https://github.com/Azure/azure-sdk-for-python/pull/30731)
+
+#### Bugs Fixed
+* Fixed bug with async patch_item method. See [PR 30804](https://github.com/Azure/azure-sdk-for-python/pull/30804).
+
+### 4.4.0 (2023-06-09)
+
+#### Features Added
+- GA release of Patch API and Delete All Items By Partition Key
+
 ### 4.4.0b2 (2023-05-22)
 
 #### Features Added
 * Added conditional patching for Patch operations. See [PR 30455](https://github.com/Azure/azure-sdk-for-python/pull/30455).
 
 #### Bugs Fixed
 * Fixed bug with non english locales causing an error with the RFC 1123 Date Format. See [PR 30125](https://github.com/Azure/azure-sdk-for-python/pull/30125).
 
 #### Other Changes
 * Refactoring of our client `connection_timeout` and `request_timeout` configurations. See [PR 30171](https://github.com/Azure/azure-sdk-for-python/pull/30171).
 
 ### 4.4.0b1 (2023-04-11)
 
 #### Features Added
- - Added **preview** delete all items by partition key functionality. See [PR 29186](https://github.com/Azure/azure-sdk-for-python/pull/29186).
+ - Added **preview** delete all items by partition key functionality. See [PR 29186](https://github.com/Azure/azure-sdk-for-python/pull/29186). For more information on Partition Key Delete, please see [Azure Cosmos DB Partition Key Delete](https://learn.microsoft.com/azure/cosmos-db/nosql/how-to-delete-by-partition-key?tabs=python-example).
  - Added **preview** partial document update (Patch API) functionality and container methods for patching items with operations. See [PR 29497](https://github.com/Azure/azure-sdk-for-python/pull/29497). For more information on Patch, please see [Azure Cosmos DB Partial Document Update](https://learn.microsoft.com/azure/cosmos-db/partial-document-update).
 
 #### Bugs Fixed
 * Fixed bug in method `create_container_if_not_exists()` of async database client for unexpected kwargs being passed into `read()` method used internally. See [PR 29136](https://github.com/Azure/azure-sdk-for-python/pull/29136).
 * Fixed bug with method `query_items()` of our async container class, where partition key and cross partition headers would both be set when using partition keys. See [PR 29366](https://github.com/Azure/azure-sdk-for-python/pull/29366/).
 * Fixed bug with client not properly surfacing errors for invalid credentials and identities with insufficient permissions. Users running into 'NoneType has no attribute ConsistencyPolicy' errors when initializing their clients will now see proper authentication exceptions. See [PR 29256](https://github.com/Azure/azure-sdk-for-python/pull/29256).
```

## Comparing `azure-cosmos-4.4.0b2/test/test_session_token_unit.py` & `azure-cosmos-4.4.1b1/test/test_session_token_unit.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_crud.py` & `azure-cosmos-4.4.1b1/test/test_crud.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_location_cache.py` & `azure-cosmos-4.4.1b1/test/test_location_cache.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_multi_orderby.py` & `azure-cosmos-4.4.1b1/test/test_multi_orderby.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_ttl.py` & `azure-cosmos-4.4.1b1/test/test_ttl.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_media.py` & `azure-cosmos-4.4.1b1/test/test_media.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_partition_key.py` & `azure-cosmos-4.4.1b1/test/test_partition_key.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_auto_scale.py` & `azure-cosmos-4.4.1b1/test/test_auto_scale.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_crud_async.py` & `azure-cosmos-4.4.1b1/test/test_crud_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_config.py` & `azure-cosmos-4.4.1b1/test/test_config.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_routing_map.py` & `azure-cosmos-4.4.1b1/test/test_routing_map.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/cleanup.py` & `azure-cosmos-4.4.1b1/test/cleanup.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_user_configs.py` & `azure-cosmos-4.4.1b1/test/test_user_configs.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_aggregate.py` & `azure-cosmos-4.4.1b1/test/test_aggregate.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_globaldb_mock.py` & `azure-cosmos-4.4.1b1/test/test_globaldb_mock.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_auto_scale_async.py` & `azure-cosmos-4.4.1b1/test/test_auto_scale_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_analytical_ttl.py` & `azure-cosmos-4.4.1b1/test/test_analytical_ttl.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_encoding.py` & `azure-cosmos-4.4.1b1/test/test_encoding.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_retry_policy.py` & `azure-cosmos-4.4.1b1/test/test_retry_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_cosmos_http_logging_policy.py` & `azure-cosmos-4.4.1b1/test/test_cosmos_http_logging_policy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_backwards_compatibility.py` & `azure-cosmos-4.4.1b1/test/test_backwards_compatibility.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_globaldb.py` & `azure-cosmos-4.4.1b1/test/test_globaldb.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_headers.py` & `azure-cosmos-4.4.1b1/test/test_headers.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_query_execution_context.py` & `azure-cosmos-4.4.1b1/test/test_query_execution_context.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_session_container.py` & `azure-cosmos-4.4.1b1/test/test_session_container.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_session.py` & `azure-cosmos-4.4.1b1/test/test_session.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_multimaster.py` & `azure-cosmos-4.4.1b1/test/test_multimaster.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_env.py` & `azure-cosmos-4.4.1b1/test/test_env.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_diagnostics.py` & `azure-cosmos-4.4.1b1/test/test_diagnostics.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_proxy.py` & `azure-cosmos-4.4.1b1/test/test_proxy.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_integrated_cache.py` & `azure-cosmos-4.4.1b1/test/test_integrated_cache.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_orderby.py` & `azure-cosmos-4.4.1b1/test/test_orderby.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_correlated_activity_id.py` & `azure-cosmos-4.4.1b1/test/test_correlated_activity_id.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_utils.py` & `azure-cosmos-4.4.1b1/test/test_utils.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_analytical_ttl_async.py` & `azure-cosmos-4.4.1b1/test/test_analytical_ttl_async.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_streaming_failover.py` & `azure-cosmos-4.4.1b1/test/test_streaming_failover.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/conftest.py` & `azure-cosmos-4.4.1b1/test/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_query.py` & `azure-cosmos-4.4.1b1/test/test_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -824,14 +824,34 @@
         query = "Select value max(c.version) FROM c where c.isComplete = true and c.lookupVersion = @lookupVersion"
         query_results = container.query_items(query, parameters=[
             {"name": "@lookupVersion", "value": "console_csat"}  # cspell:disable-line
         ], enable_cross_partition_query=True)
 
         self.assertListEqual(list(query_results), [None])
 
+    def test_continuation_token_size_limit_query(self):
+        container = self.created_db.create_container_if_not_exists(
+            self.config.TEST_COLLECTION_MULTI_PARTITION_WITH_CUSTOM_PK_ID, PartitionKey(path="/pk"))
+        for i in range(1, 1000):
+            container.create_item(body=dict(pk='123', id=str(i), some_value=str(i % 3)))
+        query = "Select * from c where c.some_value='2'"
+        response_query = container.query_items(query, partition_key='123', max_item_count=100,
+                                               response_continuation_token_limit_in_kb=1)
+        pager = response_query.by_page()
+        pager.next()
+        token = pager.continuation_token
+        # Continuation token size should be below 1kb
+        self.assertLessEqual(len(token.encode('utf-8')), 1024)
+        pager.next()
+        token = pager.continuation_token
+
+        # verify a second time
+        self.assertLessEqual(len(token.encode('utf-8')), 1024)
+        self.created_db.delete_container(container)
+
     def _MockNextFunction(self):
         if self.count < len(self.payloads):
             item, result = self.get_mock_result(self.payloads, self.count)
             self.count += 1
             if item is not None:
                 return {'orderByItems': [{'item': item}], '_rid': 'fake_rid', 'payload': result}
             else:
```

## Comparing `azure-cosmos-4.4.0b2/test/test_client_user_agent.py` & `azure-cosmos-4.4.1b1/test/test_client_user_agent.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_partition_split_query.py` & `azure-cosmos-4.4.1b1/test/test_partition_split_query.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/test_aad.py` & `azure-cosmos-4.4.1b1/test/test_aad.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/routing/test_collection_routing_map.py` & `azure-cosmos-4.4.1b1/test/routing/test_collection_routing_map.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/routing/__init__.py` & `azure-cosmos-4.4.1b1/test/routing/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-cosmos-4.4.0b2/test/routing/test_routing_map_provider.py` & `azure-cosmos-4.4.1b1/test/routing/test_routing_map_provider.py`

 * *Files identical despite different names*

