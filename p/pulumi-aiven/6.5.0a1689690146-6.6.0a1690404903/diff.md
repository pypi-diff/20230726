# Comparing `tmp/pulumi_aiven-6.5.0a1689690146.tar.gz` & `tmp/pulumi_aiven-6.6.0a1690404903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_aiven-6.5.0a1689690146.tar", last modified: Tue Jul 18 14:27:57 2023, max compression
+gzip compressed data, was "pulumi_aiven-6.6.0a1690404903.tar", last modified: Wed Jul 26 20:59:26 2023, max compression
```

## Comparing `pulumi_aiven-6.5.0a1689690146.tar` & `pulumi_aiven-6.6.0a1690404903.tar`

### file list

```diff
@@ -1,148 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:27:57.919870 pulumi_aiven-6.5.0a1689690146/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-18 14:27:57.919870 pulumi_aiven-6.5.0a1689690146/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:27:57.919870 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/
--rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   618269 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    18710 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/azure_privatelink_connection_approval.py
--rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    34308 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    75264 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    74927 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_grant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:27:57.919870 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    74949 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink.py
--rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    22264 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink_application_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    31939 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_billing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    22288 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_cassanda.py
--rw-r--r--   0 runner    (1001) docker     (123)    21956 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_cassandra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_clickhouse_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    21712 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_flink.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_flink_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    21816 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    21893 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22711 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    22188 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    22457 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22135 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21648 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    21724 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22025 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_organization_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_organizational_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    21537 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_pg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21691 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_service_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    18127 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15549 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_transit_gateway_vpc_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)    74979 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/influx_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    80341 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    77911 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    78467 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19053 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    77311 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)    76197 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/m3_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    76820 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/my_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    75940 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/open_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    14643 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/organization_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/organizational_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)   929584 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    73358 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/pg.py
--rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/pg_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/pg_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    42472 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/project_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    76316 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    30212 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/redis_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/service_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    52318 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/static_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    23726 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven/transit_gateway_vpc_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:27:57.919870 pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:27:57.919870 pulumi_aiven-6.5.0a1689690146/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-18 14:27:57.000000 pulumi_aiven-6.5.0a1689690146/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:26.973699 pulumi_aiven-6.6.0a1690404903/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-26 20:59:26.973699 pulumi_aiven-6.6.0a1690404903/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:26.973699 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/
+-rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   620227 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18710 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36913 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17027 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/azure_privatelink_connection_approval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34308 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75264 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74927 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/clickhouse_grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/clickhouse_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/clickhouse_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:26.973699 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26197 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74949 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17471 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22264 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/flink_application_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31939 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13489 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/gcp_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/gcp_privatelink_connection_approval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_account_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22288 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_cassanda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21956 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_clickhouse_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21712 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_flink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_gcp_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21816 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21893 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22711 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22188 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22457 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22135 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21648 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21724 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22025 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_organization_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_organizational_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21537 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21691 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_service_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18127 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15549 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_transit_gateway_vpc_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74979 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19380 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80341 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77911 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24756 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78467 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22353 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19053 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24119 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18906 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77311 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76197 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16718 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37020 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76820 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17313 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75940 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/open_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14643 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/organization_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10927 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/organizational_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   931914 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73358 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21818 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42472 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13742 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/project_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    76316 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30212 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53125 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52318 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14185 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/static_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23726 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven/transit_gateway_vpc_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:26.973699 pulumi_aiven-6.6.0a1690404903/pulumi_aiven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/pulumi_aiven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 20:59:26.973699 pulumi_aiven-6.6.0a1690404903/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-26 20:59:26.000000 pulumi_aiven-6.6.0a1690404903/setup.py
```

### Comparing `pulumi_aiven-6.5.0a1689690146/PKG-INFO` & `pulumi_aiven-6.6.0a1690404903/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_aiven
-Version: 6.5.0a1689690146
+Version: 6.6.0a1690404903
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_aiven-6.5.0a1689690146/README.md` & `pulumi_aiven-6.6.0a1690404903/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/__init__.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 from .clickhouse_role import *
 from .clickhouse_user import *
 from .connection_pool import *
 from .flink import *
 from .flink_application import *
 from .flink_application_deployment import *
 from .flink_application_version import *
+from .gcp_privatelink import *
+from .gcp_privatelink_connection_approval import *
 from .gcp_vpc_peering_connection import *
 from .get_account import *
 from .get_account_authentication import *
 from .get_account_team import *
 from .get_account_team_member import *
 from .get_account_team_project import *
 from .get_aws_privatelink import *
@@ -45,14 +47,15 @@
 from .get_clickhouse import *
 from .get_clickhouse_database import *
 from .get_clickhouse_user import *
 from .get_connection_pool import *
 from .get_flink import *
 from .get_flink_application import *
 from .get_flink_application_version import *
+from .get_gcp_privatelink import *
 from .get_gcp_vpc_peering_connection import *
 from .get_grafana import *
 from .get_influx_db import *
 from .get_influxdb_database import *
 from .get_influxdb_user import *
 from .get_kafka import *
 from .get_kafka_acl import *
@@ -326,14 +329,30 @@
   "fqn": "pulumi_aiven",
   "classes": {
    "aiven:index/flinkApplicationVersion:FlinkApplicationVersion": "FlinkApplicationVersion"
   }
  },
  {
   "pkg": "aiven",
+  "mod": "index/gcpPrivatelink",
+  "fqn": "pulumi_aiven",
+  "classes": {
+   "aiven:index/gcpPrivatelink:GcpPrivatelink": "GcpPrivatelink"
+  }
+ },
+ {
+  "pkg": "aiven",
+  "mod": "index/gcpPrivatelinkConnectionApproval",
+  "fqn": "pulumi_aiven",
+  "classes": {
+   "aiven:index/gcpPrivatelinkConnectionApproval:GcpPrivatelinkConnectionApproval": "GcpPrivatelinkConnectionApproval"
+  }
+ },
+ {
+  "pkg": "aiven",
   "mod": "index/gcpVpcPeeringConnection",
   "fqn": "pulumi_aiven",
   "classes": {
    "aiven:index/gcpVpcPeeringConnection:GcpVpcPeeringConnection": "GcpVpcPeeringConnection"
   }
  },
  {
```

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/_inputs.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -13132,15 +13132,15 @@
         :param pulumi.Input[Sequence[pulumi.Input['ServiceIntegrationDatadogUserConfigDatadogTagArgs']]] datadog_tags: Custom tags provided by user.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] exclude_consumer_groups: List of custom metrics.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] exclude_topics: List of topics to exclude.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] include_consumer_groups: List of custom metrics.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] include_topics: List of topics to include.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] kafka_custom_metrics: List of custom metrics.
         :param pulumi.Input[int] max_jmx_metrics: Maximum number of JMX metrics to send.
-        :param pulumi.Input['ServiceIntegrationDatadogUserConfigOpensearchArgs'] opensearch: Datadog OpenSearch Options.
+        :param pulumi.Input['ServiceIntegrationDatadogUserConfigOpensearchArgs'] opensearch: Datadog Opensearch Options.
         :param pulumi.Input['ServiceIntegrationDatadogUserConfigRedisArgs'] redis: Datadog Redis Options.
         """
         if datadog_dbm_enabled is not None:
             pulumi.set(__self__, "datadog_dbm_enabled", datadog_dbm_enabled)
         if datadog_tags is not None:
             pulumi.set(__self__, "datadog_tags", datadog_tags)
         if exclude_consumer_groups is not None:
@@ -13256,15 +13256,15 @@
     def max_jmx_metrics(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_jmx_metrics", value)
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional[pulumi.Input['ServiceIntegrationDatadogUserConfigOpensearchArgs']]:
         """
-        Datadog OpenSearch Options.
+        Datadog Opensearch Options.
         """
         return pulumi.get(self, "opensearch")
 
     @opensearch.setter
     def opensearch(self, value: Optional[pulumi.Input['ServiceIntegrationDatadogUserConfigOpensearchArgs']]):
         pulumi.set(self, "opensearch", value)
 
@@ -14481,32 +14481,48 @@
     def status_storage_topic(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status_storage_topic", value)
 
 
 @pulumi.input_type
 class ServiceIntegrationKafkaLogsUserConfigArgs:
     def __init__(__self__, *,
-                 kafka_topic: pulumi.Input[str]):
+                 kafka_topic: pulumi.Input[str],
+                 selected_log_fields: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] kafka_topic: Topic name.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] selected_log_fields: The list of logging fields that will be sent to the integration logging service. The MESSAGE and timestamp fields are always sent.
         """
         pulumi.set(__self__, "kafka_topic", kafka_topic)
+        if selected_log_fields is not None:
+            pulumi.set(__self__, "selected_log_fields", selected_log_fields)
 
     @property
     @pulumi.getter(name="kafkaTopic")
     def kafka_topic(self) -> pulumi.Input[str]:
         """
         Topic name.
         """
         return pulumi.get(self, "kafka_topic")
 
     @kafka_topic.setter
     def kafka_topic(self, value: pulumi.Input[str]):
         pulumi.set(self, "kafka_topic", value)
 
+    @property
+    @pulumi.getter(name="selectedLogFields")
+    def selected_log_fields(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        The list of logging fields that will be sent to the integration logging service. The MESSAGE and timestamp fields are always sent.
+        """
+        return pulumi.get(self, "selected_log_fields")
+
+    @selected_log_fields.setter
+    def selected_log_fields(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "selected_log_fields", value)
+
 
 @pulumi.input_type
 class ServiceIntegrationKafkaMirrormakerUserConfigArgs:
     def __init__(__self__, *,
                  cluster_alias: Optional[pulumi.Input[str]] = None,
                  kafka_mirrormaker: Optional[pulumi.Input['ServiceIntegrationKafkaMirrormakerUserConfigKafkaMirrormakerArgs']] = None):
         """
@@ -14620,23 +14636,27 @@
         pulumi.set(self, "producer_max_request_size", value)
 
 
 @pulumi.input_type
 class ServiceIntegrationLogsUserConfigArgs:
     def __init__(__self__, *,
                  elasticsearch_index_days_max: Optional[pulumi.Input[int]] = None,
-                 elasticsearch_index_prefix: Optional[pulumi.Input[str]] = None):
+                 elasticsearch_index_prefix: Optional[pulumi.Input[str]] = None,
+                 selected_log_fields: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[int] elasticsearch_index_days_max: Elasticsearch index retention limit. The default value is `3`.
         :param pulumi.Input[str] elasticsearch_index_prefix: Elasticsearch index prefix. The default value is `logs`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] selected_log_fields: The list of logging fields that will be sent to the integration logging service. The MESSAGE and timestamp fields are always sent.
         """
         if elasticsearch_index_days_max is not None:
             pulumi.set(__self__, "elasticsearch_index_days_max", elasticsearch_index_days_max)
         if elasticsearch_index_prefix is not None:
             pulumi.set(__self__, "elasticsearch_index_prefix", elasticsearch_index_prefix)
+        if selected_log_fields is not None:
+            pulumi.set(__self__, "selected_log_fields", selected_log_fields)
 
     @property
     @pulumi.getter(name="elasticsearchIndexDaysMax")
     def elasticsearch_index_days_max(self) -> Optional[pulumi.Input[int]]:
         """
         Elasticsearch index retention limit. The default value is `3`.
         """
@@ -14654,14 +14674,26 @@
         """
         return pulumi.get(self, "elasticsearch_index_prefix")
 
     @elasticsearch_index_prefix.setter
     def elasticsearch_index_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "elasticsearch_index_prefix", value)
 
+    @property
+    @pulumi.getter(name="selectedLogFields")
+    def selected_log_fields(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        The list of logging fields that will be sent to the integration logging service. The MESSAGE and timestamp fields are always sent.
+        """
+        return pulumi.get(self, "selected_log_fields")
+
+    @selected_log_fields.setter
+    def selected_log_fields(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "selected_log_fields", value)
+
 
 @pulumi.input_type
 class ServiceIntegrationMetricsUserConfigArgs:
     def __init__(__self__, *,
                  database: Optional[pulumi.Input[str]] = None,
                  retention_days: Optional[pulumi.Input[int]] = None,
                  ro_username: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/_utilities.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_authentication.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_team.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_team_member.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/account_team_project.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/aws_privatelink.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/aws_vpc_peering_connection.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/azure_privatelink.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/azure_privatelink_connection_approval.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/azure_privatelink_connection_approval.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/azure_vpc_peering_connection.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/billing_group.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/cassandra.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/cassandra.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/cassandra_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/clickhouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_database.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_grant.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/clickhouse_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_role.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/clickhouse_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/clickhouse_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/clickhouse_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/config/vars.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/connection_pool.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/flink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink_application.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink_application_deployment.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/flink_application_deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/flink_application_version.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/gcp_vpc_peering_connection.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_authentication.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_team.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_team_member.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_account_team_project.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_aws_privatelink.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_aws_vpc_peering_connection.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_azure_privatelink.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_azure_vpc_peering_connection.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_billing_group.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_cassanda.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_cassanda.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_cassandra.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_cassandra.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_cassandra_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_clickhouse.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_clickhouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_clickhouse_database.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_clickhouse_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_clickhouse_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_connection_pool.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_flink.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_flink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_flink_application.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_flink_application_version.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_gcp_vpc_peering_connection.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_grafana.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_grafana.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_influx_db.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_influx_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_influxdb_database.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_influxdb_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_acl.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_connect.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_connector.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_mirror_maker.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_mirror_maker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_schema.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_schema_configuration.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_schema_registry_acl.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_topic.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_kafka_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_m3_aggregator.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_m3_aggregator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_m3_db.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_m3_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_m3db_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_mirror_maker_replication_flow.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_my_sql.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_my_sql.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_mysql_database.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_mysql_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_open_search.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_open_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         """
         return pulumi.get(self, "maintenance_window_time")
 
     @property
     @pulumi.getter(name="opensearchUserConfigs")
     def opensearch_user_configs(self) -> Sequence['outputs.GetOpenSearchOpensearchUserConfigResult']:
         """
-        OpenSearch user configurable settings
+        Opensearch user configurable settings
         """
         return pulumi.get(self, "opensearch_user_configs")
 
     @property
     @pulumi.getter
     def opensearches(self) -> Sequence['outputs.GetOpenSearchOpensearchResult']:
         """
```

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_open_search_acl_config.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_open_search_acl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_open_search_acl_rule.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_open_search_acl_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_opensearch_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_opensearch_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_organization.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_organization_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_organization_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_organizational_unit.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_organizational_unit.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_pg.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_pg.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_pg_database.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_pg_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_project.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_project_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_project_vpc.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_redis.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_redis.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_redis_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_service_component.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_service_component.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_service_integration.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_service_integration_endpoint.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_service_integration_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         """
         return pulumi.get(self, "external_kafka_user_configs")
 
     @property
     @pulumi.getter(name="externalOpensearchLogsUserConfigs")
     def external_opensearch_logs_user_configs(self) -> Sequence['outputs.GetServiceIntegrationEndpointExternalOpensearchLogsUserConfigResult']:
         """
-        ExternalOpenSearchLogs user configurable settings
+        ExternalOpensearchLogs user configurable settings
         """
         return pulumi.get(self, "external_opensearch_logs_user_configs")
 
     @property
     @pulumi.getter(name="externalSchemaRegistryUserConfigs")
     def external_schema_registry_user_configs(self) -> Sequence['outputs.GetServiceIntegrationEndpointExternalSchemaRegistryUserConfigResult']:
         """
```

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/get_transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/get_transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/grafana.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/grafana.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/influx_db.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/influx_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/influxdb_database.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/influxdb_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_acl.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_connect.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_connector.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_mirror_maker.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_mirror_maker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_schema.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_schema_configuration.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_schema_registry_acl.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_topic.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/kafka_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/m3_aggregator.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/m3_aggregator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/m3_db.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/m3_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/m3db_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/mirror_maker_replication_flow.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/my_sql.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/my_sql.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/mysql_database.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/mysql_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/open_search.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/open_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
         :param pulumi.Input[str] additional_disk_space: Additional disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] cloud_name: Defines where the cloud provider and region where the service is hosted in. This can be changed freely after service is created. Changing the value will trigger a potentially lengthy migration process for the service. Format is cloud provider name (`aws`, `azure`, `do` `google`, `upcloud`, etc.), dash, and the cloud provider specific region name. These are documented on each Cloud provider's own support articles, like [here for Google](https://cloud.google.com/compute/docs/regions-zones/) and [here for AWS](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.RegionsAndAvailabilityZones.html).
         :param pulumi.Input[str] disk_space: Service disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] maintenance_window_dow: Day of week when maintenance operations should be performed. One monday, tuesday, wednesday, etc.
         :param pulumi.Input[str] maintenance_window_time: Time of day when maintenance operations should be performed. UTC time in HH:mm:ss format.
-        :param pulumi.Input['OpenSearchOpensearchUserConfigArgs'] opensearch_user_config: OpenSearch user configurable settings
+        :param pulumi.Input['OpenSearchOpensearchUserConfigArgs'] opensearch_user_config: Opensearch user configurable settings
         :param pulumi.Input[str] plan: Defines what kind of computing resources are allocated for the service. It can be changed after creation, though there are some restrictions when going to a smaller plan such as the new plan must have sufficient amount of disk space to store all current data and switching to a plan with fewer nodes might not be supported. The basic plan names are `hobbyist`, `startup-x`, `business-x` and `premium-x` where `x` is (roughly) the amount of memory on each node (also other attributes like number of CPUs and amount of disk space varies but naming is based on memory). The available options can be seem from the [Aiven pricing page](https://aiven.io/pricing).
         :param pulumi.Input[str] project_vpc_id: Specifies the VPC the service should run in. If the value is not set the service is not run inside a VPC. When set, the value should be given as a reference to set up dependencies correctly and the VPC must be in the same cloud and region as the service itself. Project can be freely moved to and from VPC after creation but doing so triggers migration to new servers so the operation can take significant amount of time to complete if the service has a lot of data.
         :param pulumi.Input[Sequence[pulumi.Input['OpenSearchServiceIntegrationArgs']]] service_integrations: Service integrations to specify when creating a service. Not applied after initial service creation
         :param pulumi.Input[Sequence[pulumi.Input[str]]] static_ips: Static IPs that are going to be associated with this service. Please assign a value using the 'toset' function. Once a static ip resource is in the 'assigned' state it cannot be unbound from the node again
         :param pulumi.Input[Sequence[pulumi.Input['OpenSearchTagArgs']]] tags: Tags are key-value pairs that allow you to categorize services.
         :param pulumi.Input[bool] termination_protection: Prevents the service from being deleted. It is recommended to set this to `true` for all production services to prevent unintentional service deletion. This does not shield against deleting databases or topics but for services with backups much of the content can at least be restored from backup in case accidental deletion is done.
         """
@@ -164,15 +164,15 @@
     def maintenance_window_time(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "maintenance_window_time", value)
 
     @property
     @pulumi.getter(name="opensearchUserConfig")
     def opensearch_user_config(self) -> Optional[pulumi.Input['OpenSearchOpensearchUserConfigArgs']]:
         """
-        OpenSearch user configurable settings
+        Opensearch user configurable settings
         """
         return pulumi.get(self, "opensearch_user_config")
 
     @opensearch_user_config.setter
     def opensearch_user_config(self, value: Optional[pulumi.Input['OpenSearchOpensearchUserConfigArgs']]):
         pulumi.set(self, "opensearch_user_config", value)
 
@@ -287,15 +287,15 @@
         :param pulumi.Input[str] disk_space: Service disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] disk_space_cap: The maximum disk space of the service, possible values depend on the service type, the cloud provider and the project.
         :param pulumi.Input[str] disk_space_default: The default disk space of the service, possible values depend on the service type, the cloud provider and the project. Its also the minimum value for `disk_space`
         :param pulumi.Input[str] disk_space_step: The default disk space step of the service, possible values depend on the service type, the cloud provider and the project. `disk_space` needs to increment from `disk_space_default` by increments of this size.
         :param pulumi.Input[str] disk_space_used: Disk space that service is currently using
         :param pulumi.Input[str] maintenance_window_dow: Day of week when maintenance operations should be performed. One monday, tuesday, wednesday, etc.
         :param pulumi.Input[str] maintenance_window_time: Time of day when maintenance operations should be performed. UTC time in HH:mm:ss format.
-        :param pulumi.Input['OpenSearchOpensearchUserConfigArgs'] opensearch_user_config: OpenSearch user configurable settings
+        :param pulumi.Input['OpenSearchOpensearchUserConfigArgs'] opensearch_user_config: Opensearch user configurable settings
         :param pulumi.Input[Sequence[pulumi.Input['OpenSearchOpensearchArgs']]] opensearches: OpenSearch server provided values
         :param pulumi.Input[str] plan: Defines what kind of computing resources are allocated for the service. It can be changed after creation, though there are some restrictions when going to a smaller plan such as the new plan must have sufficient amount of disk space to store all current data and switching to a plan with fewer nodes might not be supported. The basic plan names are `hobbyist`, `startup-x`, `business-x` and `premium-x` where `x` is (roughly) the amount of memory on each node (also other attributes like number of CPUs and amount of disk space varies but naming is based on memory). The available options can be seem from the [Aiven pricing page](https://aiven.io/pricing).
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] project_vpc_id: Specifies the VPC the service should run in. If the value is not set the service is not run inside a VPC. When set, the value should be given as a reference to set up dependencies correctly and the VPC must be in the same cloud and region as the service itself. Project can be freely moved to and from VPC after creation but doing so triggers migration to new servers so the operation can take significant amount of time to complete if the service has a lot of data.
         :param pulumi.Input[str] service_host: The hostname of the service.
         :param pulumi.Input[Sequence[pulumi.Input['OpenSearchServiceIntegrationArgs']]] service_integrations: Service integrations to specify when creating a service. Not applied after initial service creation
         :param pulumi.Input[str] service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
@@ -490,15 +490,15 @@
     def maintenance_window_time(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "maintenance_window_time", value)
 
     @property
     @pulumi.getter(name="opensearchUserConfig")
     def opensearch_user_config(self) -> Optional[pulumi.Input['OpenSearchOpensearchUserConfigArgs']]:
         """
-        OpenSearch user configurable settings
+        Opensearch user configurable settings
         """
         return pulumi.get(self, "opensearch_user_config")
 
     @opensearch_user_config.setter
     def opensearch_user_config(self, value: Optional[pulumi.Input['OpenSearchOpensearchUserConfigArgs']]):
         pulumi.set(self, "opensearch_user_config", value)
 
@@ -753,15 +753,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] additional_disk_space: Additional disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] cloud_name: Defines where the cloud provider and region where the service is hosted in. This can be changed freely after service is created. Changing the value will trigger a potentially lengthy migration process for the service. Format is cloud provider name (`aws`, `azure`, `do` `google`, `upcloud`, etc.), dash, and the cloud provider specific region name. These are documented on each Cloud provider's own support articles, like [here for Google](https://cloud.google.com/compute/docs/regions-zones/) and [here for AWS](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.RegionsAndAvailabilityZones.html).
         :param pulumi.Input[str] disk_space: Service disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] maintenance_window_dow: Day of week when maintenance operations should be performed. One monday, tuesday, wednesday, etc.
         :param pulumi.Input[str] maintenance_window_time: Time of day when maintenance operations should be performed. UTC time in HH:mm:ss format.
-        :param pulumi.Input[pulumi.InputType['OpenSearchOpensearchUserConfigArgs']] opensearch_user_config: OpenSearch user configurable settings
+        :param pulumi.Input[pulumi.InputType['OpenSearchOpensearchUserConfigArgs']] opensearch_user_config: Opensearch user configurable settings
         :param pulumi.Input[str] plan: Defines what kind of computing resources are allocated for the service. It can be changed after creation, though there are some restrictions when going to a smaller plan such as the new plan must have sufficient amount of disk space to store all current data and switching to a plan with fewer nodes might not be supported. The basic plan names are `hobbyist`, `startup-x`, `business-x` and `premium-x` where `x` is (roughly) the amount of memory on each node (also other attributes like number of CPUs and amount of disk space varies but naming is based on memory). The available options can be seem from the [Aiven pricing page](https://aiven.io/pricing).
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] project_vpc_id: Specifies the VPC the service should run in. If the value is not set the service is not run inside a VPC. When set, the value should be given as a reference to set up dependencies correctly and the VPC must be in the same cloud and region as the service itself. Project can be freely moved to and from VPC after creation but doing so triggers migration to new servers so the operation can take significant amount of time to complete if the service has a lot of data.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OpenSearchServiceIntegrationArgs']]]] service_integrations: Service integrations to specify when creating a service. Not applied after initial service creation
         :param pulumi.Input[str] service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] static_ips: Static IPs that are going to be associated with this service. Please assign a value using the 'toset' function. Once a static ip resource is in the 'assigned' state it cannot be unbound from the node again
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OpenSearchTagArgs']]]] tags: Tags are key-value pairs that allow you to categorize services.
@@ -932,15 +932,15 @@
         :param pulumi.Input[str] disk_space: Service disk space. Possible values depend on the service type, the cloud provider and the project. Therefore, reducing will result in the service rebalancing.
         :param pulumi.Input[str] disk_space_cap: The maximum disk space of the service, possible values depend on the service type, the cloud provider and the project.
         :param pulumi.Input[str] disk_space_default: The default disk space of the service, possible values depend on the service type, the cloud provider and the project. Its also the minimum value for `disk_space`
         :param pulumi.Input[str] disk_space_step: The default disk space step of the service, possible values depend on the service type, the cloud provider and the project. `disk_space` needs to increment from `disk_space_default` by increments of this size.
         :param pulumi.Input[str] disk_space_used: Disk space that service is currently using
         :param pulumi.Input[str] maintenance_window_dow: Day of week when maintenance operations should be performed. One monday, tuesday, wednesday, etc.
         :param pulumi.Input[str] maintenance_window_time: Time of day when maintenance operations should be performed. UTC time in HH:mm:ss format.
-        :param pulumi.Input[pulumi.InputType['OpenSearchOpensearchUserConfigArgs']] opensearch_user_config: OpenSearch user configurable settings
+        :param pulumi.Input[pulumi.InputType['OpenSearchOpensearchUserConfigArgs']] opensearch_user_config: Opensearch user configurable settings
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OpenSearchOpensearchArgs']]]] opensearches: OpenSearch server provided values
         :param pulumi.Input[str] plan: Defines what kind of computing resources are allocated for the service. It can be changed after creation, though there are some restrictions when going to a smaller plan such as the new plan must have sufficient amount of disk space to store all current data and switching to a plan with fewer nodes might not be supported. The basic plan names are `hobbyist`, `startup-x`, `business-x` and `premium-x` where `x` is (roughly) the amount of memory on each node (also other attributes like number of CPUs and amount of disk space varies but naming is based on memory). The available options can be seem from the [Aiven pricing page](https://aiven.io/pricing).
         :param pulumi.Input[str] project: Identifies the project this resource belongs to. To set up proper dependencies please refer to this variable as a reference. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] project_vpc_id: Specifies the VPC the service should run in. If the value is not set the service is not run inside a VPC. When set, the value should be given as a reference to set up dependencies correctly and the VPC must be in the same cloud and region as the service itself. Project can be freely moved to and from VPC after creation but doing so triggers migration to new servers so the operation can take significant amount of time to complete if the service has a lot of data.
         :param pulumi.Input[str] service_host: The hostname of the service.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['OpenSearchServiceIntegrationArgs']]]] service_integrations: Service integrations to specify when creating a service. Not applied after initial service creation
         :param pulumi.Input[str] service_name: Specifies the actual name of the service. The name cannot be changed later without destroying and re-creating the service so name should be picked based on intended service usage rather than current attributes.
@@ -1070,15 +1070,15 @@
         """
         return pulumi.get(self, "maintenance_window_time")
 
     @property
     @pulumi.getter(name="opensearchUserConfig")
     def opensearch_user_config(self) -> pulumi.Output[Optional['outputs.OpenSearchOpensearchUserConfig']]:
         """
-        OpenSearch user configurable settings
+        Opensearch user configurable settings
         """
         return pulumi.get(self, "opensearch_user_config")
 
     @property
     @pulumi.getter
     def opensearches(self) -> pulumi.Output[Sequence['outputs.OpenSearchOpensearch']]:
         """
```

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/open_search_acl_config.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/open_search_acl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/open_search_acl_rule.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/open_search_acl_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/opensearch_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/opensearch_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/organization.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/organization_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/organization_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/organizational_unit.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/organizational_unit.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/outputs.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -12360,15 +12360,15 @@
         :param Sequence['ServiceIntegrationDatadogUserConfigDatadogTagArgs'] datadog_tags: Custom tags provided by user.
         :param Sequence[str] exclude_consumer_groups: List of custom metrics.
         :param Sequence[str] exclude_topics: List of topics to exclude.
         :param Sequence[str] include_consumer_groups: List of custom metrics.
         :param Sequence[str] include_topics: List of topics to include.
         :param Sequence[str] kafka_custom_metrics: List of custom metrics.
         :param int max_jmx_metrics: Maximum number of JMX metrics to send.
-        :param 'ServiceIntegrationDatadogUserConfigOpensearchArgs' opensearch: Datadog OpenSearch Options.
+        :param 'ServiceIntegrationDatadogUserConfigOpensearchArgs' opensearch: Datadog Opensearch Options.
         :param 'ServiceIntegrationDatadogUserConfigRedisArgs' redis: Datadog Redis Options.
         """
         if datadog_dbm_enabled is not None:
             pulumi.set(__self__, "datadog_dbm_enabled", datadog_dbm_enabled)
         if datadog_tags is not None:
             pulumi.set(__self__, "datadog_tags", datadog_tags)
         if exclude_consumer_groups is not None:
@@ -12452,15 +12452,15 @@
         """
         return pulumi.get(self, "max_jmx_metrics")
 
     @property
     @pulumi.getter
     def opensearch(self) -> Optional['outputs.ServiceIntegrationDatadogUserConfigOpensearch']:
         """
-        Datadog OpenSearch Options.
+        Datadog Opensearch Options.
         """
         return pulumi.get(self, "opensearch")
 
     @property
     @pulumi.getter
     def redis(self) -> Optional['outputs.ServiceIntegrationDatadogUserConfigRedis']:
         """
@@ -13694,41 +13694,55 @@
 @pulumi.output_type
 class ServiceIntegrationKafkaLogsUserConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "kafkaTopic":
             suggest = "kafka_topic"
+        elif key == "selectedLogFields":
+            suggest = "selected_log_fields"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ServiceIntegrationKafkaLogsUserConfig. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         ServiceIntegrationKafkaLogsUserConfig.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         ServiceIntegrationKafkaLogsUserConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 kafka_topic: str):
+                 kafka_topic: str,
+                 selected_log_fields: Optional[Sequence[str]] = None):
         """
         :param str kafka_topic: Topic name.
+        :param Sequence[str] selected_log_fields: The list of logging fields that will be sent to the integration logging service. The MESSAGE and timestamp fields are always sent.
         """
         pulumi.set(__self__, "kafka_topic", kafka_topic)
+        if selected_log_fields is not None:
+            pulumi.set(__self__, "selected_log_fields", selected_log_fields)
 
     @property
     @pulumi.getter(name="kafkaTopic")
     def kafka_topic(self) -> str:
         """
         Topic name.
         """
         return pulumi.get(self, "kafka_topic")
 
+    @property
+    @pulumi.getter(name="selectedLogFields")
+    def selected_log_fields(self) -> Optional[Sequence[str]]:
+        """
+        The list of logging fields that will be sent to the integration logging service. The MESSAGE and timestamp fields are always sent.
+        """
+        return pulumi.get(self, "selected_log_fields")
+
 
 @pulumi.output_type
 class ServiceIntegrationKafkaMirrormakerUserConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "clusterAlias":
@@ -13861,37 +13875,43 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "elasticsearchIndexDaysMax":
             suggest = "elasticsearch_index_days_max"
         elif key == "elasticsearchIndexPrefix":
             suggest = "elasticsearch_index_prefix"
+        elif key == "selectedLogFields":
+            suggest = "selected_log_fields"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ServiceIntegrationLogsUserConfig. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         ServiceIntegrationLogsUserConfig.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         ServiceIntegrationLogsUserConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  elasticsearch_index_days_max: Optional[int] = None,
-                 elasticsearch_index_prefix: Optional[str] = None):
+                 elasticsearch_index_prefix: Optional[str] = None,
+                 selected_log_fields: Optional[Sequence[str]] = None):
         """
         :param int elasticsearch_index_days_max: Elasticsearch index retention limit. The default value is `3`.
         :param str elasticsearch_index_prefix: Elasticsearch index prefix. The default value is `logs`.
+        :param Sequence[str] selected_log_fields: The list of logging fields that will be sent to the integration logging service. The MESSAGE and timestamp fields are always sent.
         """
         if elasticsearch_index_days_max is not None:
             pulumi.set(__self__, "elasticsearch_index_days_max", elasticsearch_index_days_max)
         if elasticsearch_index_prefix is not None:
             pulumi.set(__self__, "elasticsearch_index_prefix", elasticsearch_index_prefix)
+        if selected_log_fields is not None:
+            pulumi.set(__self__, "selected_log_fields", selected_log_fields)
 
     @property
     @pulumi.getter(name="elasticsearchIndexDaysMax")
     def elasticsearch_index_days_max(self) -> Optional[int]:
         """
         Elasticsearch index retention limit. The default value is `3`.
         """
@@ -13901,14 +13921,22 @@
     @pulumi.getter(name="elasticsearchIndexPrefix")
     def elasticsearch_index_prefix(self) -> Optional[str]:
         """
         Elasticsearch index prefix. The default value is `logs`.
         """
         return pulumi.get(self, "elasticsearch_index_prefix")
 
+    @property
+    @pulumi.getter(name="selectedLogFields")
+    def selected_log_fields(self) -> Optional[Sequence[str]]:
+        """
+        The list of logging fields that will be sent to the integration logging service. The MESSAGE and timestamp fields are always sent.
+        """
+        return pulumi.get(self, "selected_log_fields")
+
 
 @pulumi.output_type
 class ServiceIntegrationMetricsUserConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "retentionDays":
@@ -23520,22 +23548,30 @@
     def status_storage_topic(self) -> Optional[str]:
         return pulumi.get(self, "status_storage_topic")
 
 
 @pulumi.output_type
 class GetServiceIntegrationKafkaLogsUserConfigResult(dict):
     def __init__(__self__, *,
-                 kafka_topic: str):
+                 kafka_topic: str,
+                 selected_log_fields: Optional[Sequence[str]] = None):
         pulumi.set(__self__, "kafka_topic", kafka_topic)
+        if selected_log_fields is not None:
+            pulumi.set(__self__, "selected_log_fields", selected_log_fields)
 
     @property
     @pulumi.getter(name="kafkaTopic")
     def kafka_topic(self) -> str:
         return pulumi.get(self, "kafka_topic")
 
+    @property
+    @pulumi.getter(name="selectedLogFields")
+    def selected_log_fields(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "selected_log_fields")
+
 
 @pulumi.output_type
 class GetServiceIntegrationKafkaMirrormakerUserConfigResult(dict):
     def __init__(__self__, *,
                  cluster_alias: Optional[str] = None,
                  kafka_mirrormaker: Optional['outputs.GetServiceIntegrationKafkaMirrormakerUserConfigKafkaMirrormakerResult'] = None):
         if cluster_alias is not None:
@@ -23607,30 +23643,38 @@
         return pulumi.get(self, "producer_max_request_size")
 
 
 @pulumi.output_type
 class GetServiceIntegrationLogsUserConfigResult(dict):
     def __init__(__self__, *,
                  elasticsearch_index_days_max: Optional[int] = None,
-                 elasticsearch_index_prefix: Optional[str] = None):
+                 elasticsearch_index_prefix: Optional[str] = None,
+                 selected_log_fields: Optional[Sequence[str]] = None):
         if elasticsearch_index_days_max is not None:
             pulumi.set(__self__, "elasticsearch_index_days_max", elasticsearch_index_days_max)
         if elasticsearch_index_prefix is not None:
             pulumi.set(__self__, "elasticsearch_index_prefix", elasticsearch_index_prefix)
+        if selected_log_fields is not None:
+            pulumi.set(__self__, "selected_log_fields", selected_log_fields)
 
     @property
     @pulumi.getter(name="elasticsearchIndexDaysMax")
     def elasticsearch_index_days_max(self) -> Optional[int]:
         return pulumi.get(self, "elasticsearch_index_days_max")
 
     @property
     @pulumi.getter(name="elasticsearchIndexPrefix")
     def elasticsearch_index_prefix(self) -> Optional[str]:
         return pulumi.get(self, "elasticsearch_index_prefix")
 
+    @property
+    @pulumi.getter(name="selectedLogFields")
+    def selected_log_fields(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "selected_log_fields")
+
 
 @pulumi.output_type
 class GetServiceIntegrationMetricsUserConfigResult(dict):
     def __init__(__self__, *,
                  database: Optional[str] = None,
                  retention_days: Optional[int] = None,
                  ro_username: Optional[str] = None,
```

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/pg.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/pg.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/pg_database.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/pg_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/project.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/project_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/project_vpc.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/provider.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/redis.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/redis.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/redis_user.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/service_integration.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/service_integration_endpoint.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/service_integration_endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         :param pulumi.Input[str] project: Project the service integration endpoint belongs to
         :param pulumi.Input['ServiceIntegrationEndpointDatadogUserConfigArgs'] datadog_user_config: Datadog user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfigArgs'] external_aws_cloudwatch_logs_user_config: ExternalAwsCloudwatchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfigArgs'] external_aws_cloudwatch_metrics_user_config: ExternalAwsCloudwatchMetrics user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalElasticsearchLogsUserConfigArgs'] external_elasticsearch_logs_user_config: ExternalElasticsearchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs'] external_google_cloud_logging_user_config: ExternalGoogleCloudLogging user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalKafkaUserConfigArgs'] external_kafka_user_config: ExternalKafka user configurable settings
-        :param pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs'] external_opensearch_logs_user_config: ExternalOpenSearchLogs user configurable settings
+        :param pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs'] external_opensearch_logs_user_config: ExternalOpensearchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs'] external_schema_registry_user_config: ExternalSchemaRegistry user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointJolokiaUserConfigArgs'] jolokia_user_config: Jolokia user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointPrometheusUserConfigArgs'] prometheus_user_config: Prometheus user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointRsyslogUserConfigArgs'] rsyslog_user_config: Rsyslog user configurable settings
         """
         pulumi.set(__self__, "endpoint_name", endpoint_name)
         pulumi.set(__self__, "endpoint_type", endpoint_type)
@@ -181,15 +181,15 @@
     def external_kafka_user_config(self, value: Optional[pulumi.Input['ServiceIntegrationEndpointExternalKafkaUserConfigArgs']]):
         pulumi.set(self, "external_kafka_user_config", value)
 
     @property
     @pulumi.getter(name="externalOpensearchLogsUserConfig")
     def external_opensearch_logs_user_config(self) -> Optional[pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']]:
         """
-        ExternalOpenSearchLogs user configurable settings
+        ExternalOpensearchLogs user configurable settings
         """
         return pulumi.get(self, "external_opensearch_logs_user_config")
 
     @external_opensearch_logs_user_config.setter
     def external_opensearch_logs_user_config(self, value: Optional[pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']]):
         pulumi.set(self, "external_opensearch_logs_user_config", value)
 
@@ -267,15 +267,15 @@
         :param pulumi.Input[str] endpoint_name: Name of the service integration endpoint
         :param pulumi.Input[str] endpoint_type: Type of the service integration endpoint. Possible values: `datadog`, `prometheus`, `rsyslog`, `external_elasticsearch_logs`, `external_opensearch_logs`, `external_aws_cloudwatch_logs`, `external_google_cloud_logging`, `external_kafka`, `jolokia`, `external_schema_registry`, `external_aws_cloudwatch_metrics`
         :param pulumi.Input['ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfigArgs'] external_aws_cloudwatch_logs_user_config: ExternalAwsCloudwatchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfigArgs'] external_aws_cloudwatch_metrics_user_config: ExternalAwsCloudwatchMetrics user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalElasticsearchLogsUserConfigArgs'] external_elasticsearch_logs_user_config: ExternalElasticsearchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs'] external_google_cloud_logging_user_config: ExternalGoogleCloudLogging user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalKafkaUserConfigArgs'] external_kafka_user_config: ExternalKafka user configurable settings
-        :param pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs'] external_opensearch_logs_user_config: ExternalOpenSearchLogs user configurable settings
+        :param pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs'] external_opensearch_logs_user_config: ExternalOpensearchLogs user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs'] external_schema_registry_user_config: ExternalSchemaRegistry user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointJolokiaUserConfigArgs'] jolokia_user_config: Jolokia user configurable settings
         :param pulumi.Input[str] project: Project the service integration endpoint belongs to
         :param pulumi.Input['ServiceIntegrationEndpointPrometheusUserConfigArgs'] prometheus_user_config: Prometheus user configurable settings
         :param pulumi.Input['ServiceIntegrationEndpointRsyslogUserConfigArgs'] rsyslog_user_config: Rsyslog user configurable settings
         """
         if datadog_user_config is not None:
@@ -417,15 +417,15 @@
     def external_kafka_user_config(self, value: Optional[pulumi.Input['ServiceIntegrationEndpointExternalKafkaUserConfigArgs']]):
         pulumi.set(self, "external_kafka_user_config", value)
 
     @property
     @pulumi.getter(name="externalOpensearchLogsUserConfig")
     def external_opensearch_logs_user_config(self) -> Optional[pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']]:
         """
-        ExternalOpenSearchLogs user configurable settings
+        ExternalOpensearchLogs user configurable settings
         """
         return pulumi.get(self, "external_opensearch_logs_user_config")
 
     @external_opensearch_logs_user_config.setter
     def external_opensearch_logs_user_config(self, value: Optional[pulumi.Input['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']]):
         pulumi.set(self, "external_opensearch_logs_user_config", value)
 
@@ -519,15 +519,15 @@
         :param pulumi.Input[str] endpoint_name: Name of the service integration endpoint
         :param pulumi.Input[str] endpoint_type: Type of the service integration endpoint. Possible values: `datadog`, `prometheus`, `rsyslog`, `external_elasticsearch_logs`, `external_opensearch_logs`, `external_aws_cloudwatch_logs`, `external_google_cloud_logging`, `external_kafka`, `jolokia`, `external_schema_registry`, `external_aws_cloudwatch_metrics`
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfigArgs']] external_aws_cloudwatch_logs_user_config: ExternalAwsCloudwatchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfigArgs']] external_aws_cloudwatch_metrics_user_config: ExternalAwsCloudwatchMetrics user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalElasticsearchLogsUserConfigArgs']] external_elasticsearch_logs_user_config: ExternalElasticsearchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs']] external_google_cloud_logging_user_config: ExternalGoogleCloudLogging user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalKafkaUserConfigArgs']] external_kafka_user_config: ExternalKafka user configurable settings
-        :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']] external_opensearch_logs_user_config: ExternalOpenSearchLogs user configurable settings
+        :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']] external_opensearch_logs_user_config: ExternalOpensearchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs']] external_schema_registry_user_config: ExternalSchemaRegistry user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointJolokiaUserConfigArgs']] jolokia_user_config: Jolokia user configurable settings
         :param pulumi.Input[str] project: Project the service integration endpoint belongs to
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointPrometheusUserConfigArgs']] prometheus_user_config: Prometheus user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointRsyslogUserConfigArgs']] rsyslog_user_config: Rsyslog user configurable settings
         """
         ...
@@ -635,15 +635,15 @@
         :param pulumi.Input[str] endpoint_name: Name of the service integration endpoint
         :param pulumi.Input[str] endpoint_type: Type of the service integration endpoint. Possible values: `datadog`, `prometheus`, `rsyslog`, `external_elasticsearch_logs`, `external_opensearch_logs`, `external_aws_cloudwatch_logs`, `external_google_cloud_logging`, `external_kafka`, `jolokia`, `external_schema_registry`, `external_aws_cloudwatch_metrics`
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalAwsCloudwatchLogsUserConfigArgs']] external_aws_cloudwatch_logs_user_config: ExternalAwsCloudwatchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalAwsCloudwatchMetricsUserConfigArgs']] external_aws_cloudwatch_metrics_user_config: ExternalAwsCloudwatchMetrics user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalElasticsearchLogsUserConfigArgs']] external_elasticsearch_logs_user_config: ExternalElasticsearchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalGoogleCloudLoggingUserConfigArgs']] external_google_cloud_logging_user_config: ExternalGoogleCloudLogging user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalKafkaUserConfigArgs']] external_kafka_user_config: ExternalKafka user configurable settings
-        :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']] external_opensearch_logs_user_config: ExternalOpenSearchLogs user configurable settings
+        :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalOpensearchLogsUserConfigArgs']] external_opensearch_logs_user_config: ExternalOpensearchLogs user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointExternalSchemaRegistryUserConfigArgs']] external_schema_registry_user_config: ExternalSchemaRegistry user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointJolokiaUserConfigArgs']] jolokia_user_config: Jolokia user configurable settings
         :param pulumi.Input[str] project: Project the service integration endpoint belongs to
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointPrometheusUserConfigArgs']] prometheus_user_config: Prometheus user configurable settings
         :param pulumi.Input[pulumi.InputType['ServiceIntegrationEndpointRsyslogUserConfigArgs']] rsyslog_user_config: Rsyslog user configurable settings
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -739,15 +739,15 @@
         """
         return pulumi.get(self, "external_kafka_user_config")
 
     @property
     @pulumi.getter(name="externalOpensearchLogsUserConfig")
     def external_opensearch_logs_user_config(self) -> pulumi.Output[Optional['outputs.ServiceIntegrationEndpointExternalOpensearchLogsUserConfig']]:
         """
-        ExternalOpenSearchLogs user configurable settings
+        ExternalOpensearchLogs user configurable settings
         """
         return pulumi.get(self, "external_opensearch_logs_user_config")
 
     @property
     @pulumi.getter(name="externalSchemaRegistryUserConfig")
     def external_schema_registry_user_config(self) -> pulumi.Output[Optional['outputs.ServiceIntegrationEndpointExternalSchemaRegistryUserConfig']]:
         """
```

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/static_ip.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/static_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven/transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven/transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/PKG-INFO` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-aiven
-Version: 6.5.0a1689690146
+Version: 6.6.0a1690404903
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi aiven
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_aiven-6.5.0a1689690146/pulumi_aiven.egg-info/SOURCES.txt` & `pulumi_aiven-6.6.0a1690404903/pulumi_aiven.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 pulumi_aiven/clickhouse_role.py
 pulumi_aiven/clickhouse_user.py
 pulumi_aiven/connection_pool.py
 pulumi_aiven/flink.py
 pulumi_aiven/flink_application.py
 pulumi_aiven/flink_application_deployment.py
 pulumi_aiven/flink_application_version.py
+pulumi_aiven/gcp_privatelink.py
+pulumi_aiven/gcp_privatelink_connection_approval.py
 pulumi_aiven/gcp_vpc_peering_connection.py
 pulumi_aiven/get_account.py
 pulumi_aiven/get_account_authentication.py
 pulumi_aiven/get_account_team.py
 pulumi_aiven/get_account_team_member.py
 pulumi_aiven/get_account_team_project.py
 pulumi_aiven/get_aws_privatelink.py
@@ -43,14 +45,15 @@
 pulumi_aiven/get_clickhouse.py
 pulumi_aiven/get_clickhouse_database.py
 pulumi_aiven/get_clickhouse_user.py
 pulumi_aiven/get_connection_pool.py
 pulumi_aiven/get_flink.py
 pulumi_aiven/get_flink_application.py
 pulumi_aiven/get_flink_application_version.py
+pulumi_aiven/get_gcp_privatelink.py
 pulumi_aiven/get_gcp_vpc_peering_connection.py
 pulumi_aiven/get_grafana.py
 pulumi_aiven/get_influx_db.py
 pulumi_aiven/get_influxdb_database.py
 pulumi_aiven/get_influxdb_user.py
 pulumi_aiven/get_kafka.py
 pulumi_aiven/get_kafka_acl.py
```

### Comparing `pulumi_aiven-6.5.0a1689690146/setup.py` & `pulumi_aiven-6.6.0a1690404903/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.5.0a1689690146"
-PLUGIN_VERSION = "6.5.0-alpha.1689690146+f57acb18"
+VERSION = "6.6.0a1690404903"
+PLUGIN_VERSION = "6.6.0-alpha.1690404903+2f63fd13"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'aiven', PLUGIN_VERSION])
         except OSError as error:
```

