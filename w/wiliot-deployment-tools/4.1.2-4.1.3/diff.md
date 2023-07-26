# Comparing `tmp/wiliot-deployment-tools-4.1.2.tar.gz` & `tmp/wiliot-deployment-tools-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-deployment-tools-4.1.2.tar", last modified: Mon Jul 24 13:17:37 2023, max compression
+gzip compressed data, was "wiliot-deployment-tools-4.1.3.tar", last modified: Wed Jul 26 07:53:48 2023, max compression
```

## Comparing `wiliot-deployment-tools-4.1.2.tar` & `wiliot-deployment-tools-4.1.3.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.554506 wiliot-deployment-tools-4.1.2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.534506 wiliot-deployment-tools-4.1.2/.deploy/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.534506 wiliot-deployment-tools-4.1.2/.deploy/aws/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.538506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/common.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.538506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/account.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.538506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.538506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.538506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.534506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.542506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/
--rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh
--rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/terragrunt.hcl
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/dbc.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.542506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.534506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.542506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/
--rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/install_packages.sh
--rw-rw-rw-   0 root         (0) root         (0)     4550 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/terragrunt.hcl
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/region.hcl
--rw-rw-rw-   0 root         (0) root         (0)     1290 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/terragrunt.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.542506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/test/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/test/account.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.542506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/test/us-east-2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.542506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/test/us-east-2/dbc/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.542506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.534506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.542506 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/
--rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh
--rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/terragrunt.hcl
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/test/us-east-2/dbc/dbc.hcl
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/test/us-east-2/region.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.534506 wiliot-deployment-tools-4.1.2/.devcontainer/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.542506 wiliot-deployment-tools-4.1.2/.devcontainer/private/
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.devcontainer/private/devcontainer.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.542506 wiliot-deployment-tools-4.1.2/.devcontainer/public/
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.devcontainer/public/devcontainer.json
--rw-rw-rw-   0 root         (0) root         (0)      455 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.gitignore
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.542506 wiliot-deployment-tools-4.1.2/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      687 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/Makefile
--rw-rw-rw-   0 root         (0) root         (0)    11566 2023-07-24 13:17:37.554506 wiliot-deployment-tools-4.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11048 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)    11458 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.542506 wiliot-deployment-tools-4.1.2/ci/
--rwxrwxrwx   0 root         (0) root         (0)     1696 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/ci/upload_to_s3.sh
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/ci.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/dep-tools-public.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      519 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/dep-tools.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)    14810 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/gw_certificate.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-24 13:17:37.554506 wiliot-deployment-tools-4.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3635 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.542506 wiliot-deployment-tools-4.1.2/unittests/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/unittests/test_debug_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/unittests/test_extended_api_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/unittests/test_extended_api_platform.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/unittests/test_power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2710 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/unittests/test_slack_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/unittests/test_test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     2252 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/unittests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.542506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.546506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/ag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/ag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12545 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/ag/ut_defines.py
--rw-rw-rw-   0 root         (0) root         (0)     3834 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/ag/wlt_types.py
--rw-rw-rw-   0 root         (0) root         (0)    78971 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/ag/wlt_types_ag.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/ag/wlt_types_data.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/ag/wlt_types_imports.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.546506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    50260 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/api/extended_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1187 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/api/gw_ssid.py
--rw-rw-rw-   0 root         (0) root         (0)     1139 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/api/s3_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.546506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/automatic_configuration_tool/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15430 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     3178 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.546506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/calibration_mgmt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/calibration_mgmt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13553 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.546506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    68659 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/common/analysis_data_bricks.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/common/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     6004 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/common/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3135 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/common/utils_defines.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.546506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/connectivity_analyzer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/connectivity_analyzer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14407 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer.py
--rw-rw-rw-   0 root         (0) root         (0)     3084 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.550506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/firmware_update/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/firmware_update/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22977 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/firmware_update/firmware_update.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.550506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2132 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/gw_certificate.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/gw_certificate_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.550506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/interface/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/interface/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6770 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/interface/ble_simulator.py
--rw-rw-rw-   0 root         (0) root         (0)     1554 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/interface/brg_array.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/interface/if_defines.py
--rw-rw-rw-   0 root         (0) root         (0)     7803 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/interface/mqtt.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/interface/packet_error.py
--rw-rw-rw-   0 root         (0) root         (0)     3381 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/interface/pkt_generator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.550506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/tests/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14788 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/tests/coupling.py
--rw-rw-rw-   0 root         (0) root         (0)     3665 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/tests/generated_packet_table.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/tests/generic.py
--rw-rw-rw-   0 root         (0) root         (0)   190851 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/tests/packet_table.csv
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.550506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/interface/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/interface/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/interface/uart_ports.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.550506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/log_viewer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/log_viewer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2541 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.550506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/power_mgmt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/power_mgmt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4653 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
--rw-rw-rw-   0 root         (0) root         (0)    26335 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/power_mgmt/power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     4801 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.550506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2023-07-24 13:17:17.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-24 13:17:37.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-24 13:17:37.546506 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    11566 2023-07-24 13:17:37.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4727 2023-07-24 13:17:37.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-24 13:17:37.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      725 2023-07-24 13:17:37.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-24 13:17:37.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-24 13:17:37.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-24 13:17:37.000000 wiliot-deployment-tools-4.1.2/wiliot_deployment_tools.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.557204 wiliot-deployment-tools-4.1.3/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.533204 wiliot-deployment-tools-4.1.3/.deploy/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.533204 wiliot-deployment-tools-4.1.3/.deploy/aws/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/common.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/account.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.537204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/
+-rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/terragrunt.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/dbc.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.537204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/
+-rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/install_packages.sh
+-rw-rw-rw-   0 root         (0) root         (0)     4550 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/terragrunt.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/region.hcl
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/terragrunt.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/account.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.537204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.545204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/
+-rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/terragrunt.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/dbc.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/region.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.537204 wiliot-deployment-tools-4.1.3/.devcontainer/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.545204 wiliot-deployment-tools-4.1.3/.devcontainer/private/
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.devcontainer/private/devcontainer.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.545204 wiliot-deployment-tools-4.1.3/.devcontainer/public/
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.devcontainer/public/devcontainer.json
+-rw-rw-rw-   0 root         (0) root         (0)      455 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.gitignore
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.545204 wiliot-deployment-tools-4.1.3/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)    11683 2023-07-26 07:53:48.557204 wiliot-deployment-tools-4.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11165 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    11458 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.545204 wiliot-deployment-tools-4.1.3/ci/
+-rwxrwxrwx   0 root         (0) root         (0)     1696 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/ci/upload_to_s3.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/dep-tools-public.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      519 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/dep-tools.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    14810 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/gw_certificate.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-26 07:53:48.557204 wiliot-deployment-tools-4.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.545204 wiliot-deployment-tools-4.1.3/unittests/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests/test_debug_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests/test_extended_api_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests/test_extended_api_platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests/test_power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests/test_slack_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests/test_test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2252 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.545204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.549204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12545 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/ut_defines.py
+-rw-rw-rw-   0 root         (0) root         (0)     3834 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/wlt_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    78971 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/wlt_types_ag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/wlt_types_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/wlt_types_imports.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.549204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    50260 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/extended_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/gw_ssid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/s3_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.549204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/automatic_configuration_tool/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15430 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.549204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/calibration_mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/calibration_mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13553 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.549204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    68659 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/analysis_data_bricks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     6004 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/utils_defines.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.553204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/connectivity_analyzer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/connectivity_analyzer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14407 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3084 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.553204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/firmware_update/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/firmware_update/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22977 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/firmware_update/firmware_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.553204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2131 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/gw_certificate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/gw_certificate_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.553204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6770 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/ble_simulator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/brg_array.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/if_defines.py
+-rw-rw-rw-   0 root         (0) root         (0)     7896 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/mqtt.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/packet_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     3381 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/pkt_generator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.553204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15386 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/coupling.py
+-rw-rw-rw-   0 root         (0) root         (0)     3665 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/generated_packet_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/generic.py
+-rw-rw-rw-   0 root         (0) root         (0)   190851 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/packet_table.csv
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.557204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/interface/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/interface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/interface/uart_ports.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.557204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/log_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/log_viewer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.557204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
+-rw-rw-rw-   0 root         (0) root         (0)    26335 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     4801 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.557204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6057 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.549204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    11683 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4727 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      725 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/top_level.txt
```

### Comparing `wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/common.hcl` & `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/common.hcl`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh` & `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/terragrunt.hcl` & `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/terragrunt.hcl`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/install_packages.sh` & `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/install_packages.sh`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/terragrunt.hcl` & `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/terragrunt.hcl`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/terragrunt.hcl` & `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/terragrunt.hcl`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh` & `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/terragrunt.hcl` & `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/terragrunt.hcl`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/.devcontainer/private/devcontainer.json` & `wiliot-deployment-tools-4.1.3/.devcontainer/private/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/.devcontainer/public/devcontainer.json` & `wiliot-deployment-tools-4.1.3/.devcontainer/public/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/LICENSE` & `wiliot-deployment-tools-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/Makefile` & `wiliot-deployment-tools-4.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/PKG-INFO` & `wiliot-deployment-tools-4.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.1.2
+Version: 4.1.3
 Summary: A library for interacting with Wiliot's Deployment Tools
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -201,14 +201,19 @@
 - Init Stage - Send 4 packet pairs (Data+SI) from 1 BRG, testing maximum/minimum RSSI and NFPKT Values encoded in SI packet
 - One Bridge Stage - Send packet pairs at increasing duplication (1->10) and increasing time delay between packets (15->255 ms) from 1 bridge, including simulated packet error.
 - Three Bridge Init Stage - send same data packet from 3 different bridges, each with different SI.
 - Three Bridge Stage - send same data packet from 3 different bridges, at increasing duplication (1->10) and increasing time delay between packets for each bridge (30->255).
 The test logs all sent packets, and all received packets from the tested GW in log files and outputs a summary of all sent packets in a CSV file (filepath specified at runtime).
 
 #### GW Certificate Release Notes:
+Version 4.1.3:
+* Bugfixes
+* Support for Android
+* Support for python 3.11
+
 Version 4.1.0:
 * Coupling Test
 * Add CSV Output
 * Calculate test run
 
 Version 4.0.13:
 * Initial Release (Alpha)
@@ -227,14 +232,17 @@
 required arguments:
   -owner OWNER  Owner ID
   -gw GW        Gateway ID
   ```
 
 
 ## Release Notes:
+Version 4.1.3:
+* GW Certificate Bugfixes
+
 Version 4.1.1:
 * Bridge-Gw connectivity log print
 
 Version 4.1.0:
 * Custom message support
 * GW Certificate - coupling test
 * Fixes for calibration management
```

### Comparing `wiliot-deployment-tools-4.1.2/README.md` & `wiliot-deployment-tools-4.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,19 @@
 - Init Stage - Send 4 packet pairs (Data+SI) from 1 BRG, testing maximum/minimum RSSI and NFPKT Values encoded in SI packet
 - One Bridge Stage - Send packet pairs at increasing duplication (1->10) and increasing time delay between packets (15->255 ms) from 1 bridge, including simulated packet error.
 - Three Bridge Init Stage - send same data packet from 3 different bridges, each with different SI.
 - Three Bridge Stage - send same data packet from 3 different bridges, at increasing duplication (1->10) and increasing time delay between packets for each bridge (30->255).
 The test logs all sent packets, and all received packets from the tested GW in log files and outputs a summary of all sent packets in a CSV file (filepath specified at runtime).
 
 #### GW Certificate Release Notes:
+Version 4.1.3:
+* Bugfixes
+* Support for Android
+* Support for python 3.11
+
 Version 4.1.0:
 * Coupling Test
 * Add CSV Output
 * Calculate test run
 
 Version 4.0.13:
 * Initial Release (Alpha)
@@ -210,14 +215,17 @@
 required arguments:
   -owner OWNER  Owner ID
   -gw GW        Gateway ID
   ```
 
 
 ## Release Notes:
+Version 4.1.3:
+* GW Certificate Bugfixes
+
 Version 4.1.1:
 * Bridge-Gw connectivity log print
 
 Version 4.1.0:
 * Custom message support
 * GW Certificate - coupling test
 * Fixes for calibration management
```

### Comparing `wiliot-deployment-tools-4.1.2/bitbucket-pipelines.yml` & `wiliot-deployment-tools-4.1.3/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/ci/upload_to_s3.sh` & `wiliot-deployment-tools-4.1.3/ci/upload_to_s3.sh`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/ci.py` & `wiliot-deployment-tools-4.1.3/ci.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/dep-tools.dockerfile` & `wiliot-deployment-tools-4.1.3/dep-tools.dockerfile`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/gw_certificate.ipynb` & `wiliot-deployment-tools-4.1.3/gw_certificate.ipynb`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/setup.py` & `wiliot-deployment-tools-4.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                      'wiliot-core>=4.0.9',
                      'wiliot-api>=4.3.2',
                      'bitstruct==8.17.0',
                      'bokeh==2.4.1',
                      'boto3==1.26.77',
                      'colorama==0.4.6',
                      'jsonpickle==3.0.1',
-                     'numpy==1.22.4',
+                     'numpy>=1.22.4',
                      'pandas==1.5.3',
                      'plotly==5.13.0',
                      'pytz==2022.7.1',
                      'requests>=2.28.1',
                      'setuptools>=65.6.3',
                      'tabulate==0.8.10',
                      'backports.zoneinfo==0.2.1; python_version < "3.9.0"',
```

### Comparing `wiliot-deployment-tools-4.1.2/unittests/test_extended_api_edge.py` & `wiliot-deployment-tools-4.1.3/unittests/test_extended_api_edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/unittests/test_extended_api_platform.py` & `wiliot-deployment-tools-4.1.3/unittests/test_extended_api_platform.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/unittests/test_power_mgmt.py` & `wiliot-deployment-tools-4.1.3/unittests/test_power_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/unittests/test_slack_alerts.py` & `wiliot-deployment-tools-4.1.3/unittests/test_slack_alerts.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/unittests/test_test_tool.py` & `wiliot-deployment-tools-4.1.3/unittests/test_test_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/unittests/test_utils.py` & `wiliot-deployment-tools-4.1.3/unittests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/ag/ut_defines.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/ut_defines.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/ag/wlt_types.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/wlt_types.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/ag/wlt_types_ag.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/wlt_types_ag.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/ag/wlt_types_data.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/wlt_types_data.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/api/extended_api.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/extended_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/api/gw_ssid.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/gw_ssid.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/api/s3_client.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/s3_client.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/common/analysis_data_bricks.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/analysis_data_bricks.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/common/debug.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/debug.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/common/utils.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/common/utils_defines.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/utils_defines.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer_cli.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/firmware_update/firmware_update.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/firmware_update/firmware_update.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/firmware_update/firmware_update_cli.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/firmware_update/firmware_update_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/gw_certificate.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/gw_certificate.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -39,8 +39,8 @@
         self.tests = [CouplingTest(**self.__dict__)]
     
     def run_tests(self):
         for test in self.tests:
             test.run()
 
 # TODO - send HB and CFG 
-# TODO - UnCoupled Mode
+# TODO - UnCoupled Mode
```

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/gw_certificate_cli.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/gw_certificate_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/interface/ble_simulator.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/ble_simulator.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/interface/brg_array.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/brg_array.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/interface/mqtt.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/mqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,18 @@
             
     def __repr__(self) -> str:
         return f'Data {self.data} \n Status {self.status} \n Update {self.update}'
             
 class MqttClient:
 
     def __init__(self, gw_id, owner_id, logger_filepath):
+        # Set variables
+        self.gw_id = gw_id
+        self.owner_id = owner_id
+        
         # Configure logger
         logger = logging.getLogger('mqtt')
         logger.setLevel(logging.DEBUG)
         # create file handler which logs even debug messages
         fh = logging.FileHandler(logger_filepath)
         fh.setLevel(logging.DEBUG)
         logger.addHandler(fh)
```

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/interface/packet_error.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/packet_error.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/interface/pkt_generator.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/pkt_generator.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/tests/coupling.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/coupling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import time
 import pandas as pd
 import tabulate
 from wiliot_deployment_tools.ag.ut_defines import BRIDGE_ID, NFPKT, PAYLOAD, RSSI, TIMESTAMP
-from wiliot_deployment_tools.api.extended_api import ExtendedEdgeClient
+from wiliot_deployment_tools.api.extended_api import ExtendedEdgeClient, GatewayType
 from wiliot_deployment_tools.common.debug import debug_print
 from wiliot_deployment_tools.gw_certificate.interface import packet_error
 from wiliot_deployment_tools.gw_certificate.interface import mqtt
 from wiliot_deployment_tools.gw_certificate.interface.ble_simulator import BLESimulator
 from wiliot_deployment_tools.gw_certificate.interface.brg_array import BrgArray
 from wiliot_deployment_tools.gw_certificate.interface.if_defines import BRIDGES, DEFAULT_DELAY, DEFAULT_OUTPUT_POWER, DUPLICATIONS, MAX_NFPKT, MAX_RSSI, SEP, TIME_DELAYS
 from wiliot_deployment_tools.gw_certificate.interface.mqtt import MqttClient
@@ -48,15 +48,25 @@
     
     def prepare_stage(self):
         debug_print(f'### Starting Stage: {self.stage_name}')
         self.mqttc.flash_pkts()
         self.ble_sim.set_sim_mode(True)
         
     def fetch_mqtt_from_stage(self):
-        self.mqtt_pkts = self.mqttc.get_coupled_tags_pkts()
+        def process_payload(packet:dict):
+            payload = packet[PAYLOAD]
+            payload = payload.upper()
+            # big2little endian
+            if payload[:4] == 'FCC6':
+                payload = 'C6FC' + payload[4:]
+            packet[PAYLOAD] = payload
+            return packet
+        mqtt_pkts = self.mqttc.get_coupled_tags_pkts()
+        self.mqtt_pkts = list(map(lambda p: process_payload(p), mqtt_pkts))
+        
         
     def compare_local_mqtt(self):
         self.fetch_mqtt_from_stage()
         local_pkts_df = pd.DataFrame(self.local_pkts)
         mqtt_pkts_df = pd.DataFrame(self.mqtt_pkts)
         if not set(SHARED_COLUMNS) <= set(mqtt_pkts_df.columns):
             missing_columns = list(set(SHARED_COLUMNS) - set(mqtt_pkts_df.columns))
@@ -264,15 +274,19 @@
     def __init__(self, **kwargs):        
         self.__dict__.update(kwargs)
         self.randomize = True
         super().__init__(**self.__dict__)
         self.stages = [stage(**self.__dict__) for stage in STAGES]
 
     def enter_dev_mode(self):
-        self.edge.enter_dev_mode(self.gw_id, legacy=self.legacy)
+        gw_type = self.edge.get_gateway_type(self.gw_id)
+        if gw_type == GatewayType.MOBILE:
+            debug_print('Android DevMode needs to be enabled manually! Choose HIVE env')
+        else:
+            self.edge.enter_dev_mode(self.gw_id, legacy=self.legacy)
         gw_info = self.mqttc.get_gw_info()
         timeout = datetime.datetime.now() + datetime.timedelta(minutes=3)
         while datetime.datetime.now() < timeout:
             debug_print('Waiting to see GW in DevMode...')
             gw_seen = self.mqttc.userdata['gw_seen']
             if gw_seen is True or gw_info is not False:
                 debug_print(f'GW {self.gw_id} In DevMode')
```

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/tests/generated_packet_table.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/generated_packet_table.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/tests/generic.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/generic.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/gw_certificate/tests/packet_table.csv` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/packet_table.csv`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/interface/uart_ports.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/interface/uart_ports.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/log_viewer/log_viewer_cli.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/log_viewer/log_viewer_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/power_mgmt/power_mgmt.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/power_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools/utils/get_version.py` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools.egg-info/PKG-INFO` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.1.2
+Version: 4.1.3
 Summary: A library for interacting with Wiliot's Deployment Tools
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -201,14 +201,19 @@
 - Init Stage - Send 4 packet pairs (Data+SI) from 1 BRG, testing maximum/minimum RSSI and NFPKT Values encoded in SI packet
 - One Bridge Stage - Send packet pairs at increasing duplication (1->10) and increasing time delay between packets (15->255 ms) from 1 bridge, including simulated packet error.
 - Three Bridge Init Stage - send same data packet from 3 different bridges, each with different SI.
 - Three Bridge Stage - send same data packet from 3 different bridges, at increasing duplication (1->10) and increasing time delay between packets for each bridge (30->255).
 The test logs all sent packets, and all received packets from the tested GW in log files and outputs a summary of all sent packets in a CSV file (filepath specified at runtime).
 
 #### GW Certificate Release Notes:
+Version 4.1.3:
+* Bugfixes
+* Support for Android
+* Support for python 3.11
+
 Version 4.1.0:
 * Coupling Test
 * Add CSV Output
 * Calculate test run
 
 Version 4.0.13:
 * Initial Release (Alpha)
@@ -227,14 +232,17 @@
 required arguments:
   -owner OWNER  Owner ID
   -gw GW        Gateway ID
   ```
 
 
 ## Release Notes:
+Version 4.1.3:
+* GW Certificate Bugfixes
+
 Version 4.1.1:
 * Bridge-Gw connectivity log print
 
 Version 4.1.0:
 * Custom message support
 * GW Certificate - coupling test
 * Fixes for calibration management
```

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools.egg-info/SOURCES.txt` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.2/wiliot_deployment_tools.egg-info/entry_points.txt` & `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/entry_points.txt`

 * *Files identical despite different names*

