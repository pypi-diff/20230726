# Comparing `tmp/wiliot-deployment-tools-4.1.3.tar.gz` & `tmp/wiliot-deployment-tools-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-deployment-tools-4.1.3.tar", last modified: Wed Jul 26 07:53:48 2023, max compression
+gzip compressed data, was "wiliot-deployment-tools-4.1.4.tar", last modified: Wed Jul 26 15:20:38 2023, max compression
```

## Comparing `wiliot-deployment-tools-4.1.3.tar` & `wiliot-deployment-tools-4.1.4.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.557204 wiliot-deployment-tools-4.1.3/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.533204 wiliot-deployment-tools-4.1.3/.deploy/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.533204 wiliot-deployment-tools-4.1.3/.deploy/aws/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/common.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/account.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.537204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/
--rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh
--rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/terragrunt.hcl
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/dbc.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.537204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/
--rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/install_packages.sh
--rw-rw-rw-   0 root         (0) root         (0)     4550 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/terragrunt.hcl
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/region.hcl
--rw-rw-rw-   0 root         (0) root         (0)     1290 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/terragrunt.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/account.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.541204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.537204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.545204 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/
--rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh
--rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/terragrunt.hcl
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/dbc.hcl
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/region.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.537204 wiliot-deployment-tools-4.1.3/.devcontainer/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.545204 wiliot-deployment-tools-4.1.3/.devcontainer/private/
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.devcontainer/private/devcontainer.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.545204 wiliot-deployment-tools-4.1.3/.devcontainer/public/
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.devcontainer/public/devcontainer.json
--rw-rw-rw-   0 root         (0) root         (0)      455 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.gitignore
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.545204 wiliot-deployment-tools-4.1.3/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      687 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/Makefile
--rw-rw-rw-   0 root         (0) root         (0)    11683 2023-07-26 07:53:48.557204 wiliot-deployment-tools-4.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11165 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)    11458 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.545204 wiliot-deployment-tools-4.1.3/ci/
--rwxrwxrwx   0 root         (0) root         (0)     1696 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/ci/upload_to_s3.sh
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/ci.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/dep-tools-public.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      519 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/dep-tools.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)    14810 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/gw_certificate.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-26 07:53:48.557204 wiliot-deployment-tools-4.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3635 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.545204 wiliot-deployment-tools-4.1.3/unittests/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests/test_debug_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests/test_extended_api_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests/test_extended_api_platform.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests/test_power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2710 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests/test_slack_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests/test_test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     2252 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.545204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.549204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12545 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/ut_defines.py
--rw-rw-rw-   0 root         (0) root         (0)     3834 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/wlt_types.py
--rw-rw-rw-   0 root         (0) root         (0)    78971 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/wlt_types_ag.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/wlt_types_data.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/wlt_types_imports.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.549204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    50260 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/extended_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1187 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/gw_ssid.py
--rw-rw-rw-   0 root         (0) root         (0)     1139 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/s3_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.549204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/automatic_configuration_tool/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15430 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     3178 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.549204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/calibration_mgmt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/calibration_mgmt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13553 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.549204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    68659 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/analysis_data_bricks.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     6004 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3135 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/utils_defines.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.553204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/connectivity_analyzer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/connectivity_analyzer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14407 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer.py
--rw-rw-rw-   0 root         (0) root         (0)     3084 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.553204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/firmware_update/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/firmware_update/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22977 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/firmware_update/firmware_update.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.553204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2131 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/gw_certificate.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/gw_certificate_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.553204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6770 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/ble_simulator.py
--rw-rw-rw-   0 root         (0) root         (0)     1554 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/brg_array.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/if_defines.py
--rw-rw-rw-   0 root         (0) root         (0)     7896 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/mqtt.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/packet_error.py
--rw-rw-rw-   0 root         (0) root         (0)     3381 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/pkt_generator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.553204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15386 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/coupling.py
--rw-rw-rw-   0 root         (0) root         (0)     3665 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/generated_packet_table.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/generic.py
--rw-rw-rw-   0 root         (0) root         (0)   190851 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/packet_table.csv
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.557204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/interface/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/interface/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/interface/uart_ports.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.557204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/log_viewer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/log_viewer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2541 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.557204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4653 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
--rw-rw-rw-   0 root         (0) root         (0)    26335 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     4801 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.557204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2023-07-26 07:53:18.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 07:53:48.549204 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    11683 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4727 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      725 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-26 07:53:48.000000 wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.089813 wiliot-deployment-tools-4.1.4/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.073813 wiliot-deployment-tools-4.1.4/.deploy/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.073813 wiliot-deployment-tools-4.1.4/.deploy/aws/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.077813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/common.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.077813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/account.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.077813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.073813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/
+-rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/terragrunt.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/dbc.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.073813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/
+-rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/install_packages.sh
+-rw-rw-rw-   0 root         (0) root         (0)     4550 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/terragrunt.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/region.hcl
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/terragrunt.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/test/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/test/account.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/test/us-east-2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/test/us-east-2/dbc/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.077813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/
+-rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/terragrunt.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/test/us-east-2/dbc/dbc.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/test/us-east-2/region.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.077813 wiliot-deployment-tools-4.1.4/.devcontainer/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/.devcontainer/private/
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.devcontainer/private/devcontainer.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/.devcontainer/public/
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.devcontainer/public/devcontainer.json
+-rw-rw-rw-   0 root         (0) root         (0)      455 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.gitignore
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)    11677 2023-07-26 15:20:38.089813 wiliot-deployment-tools-4.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11159 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    13775 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/ci/
+-rwxrwxrwx   0 root         (0) root         (0)     1696 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/ci/upload_to_s3.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/dep-tools-public.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      519 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/dep-tools.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    14810 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/gw_certificate.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-26 15:20:38.089813 wiliot-deployment-tools-4.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/unittests/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/unittests/test_debug_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/unittests/test_extended_api_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/unittests/test_extended_api_platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/unittests/test_power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/unittests/test_slack_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/unittests/test_test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2252 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/unittests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.085813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/ag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/ag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13204 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/ag/ut_defines.py
+-rw-rw-rw-   0 root         (0) root         (0)     4492 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/ag/wlt_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    92198 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/ag/wlt_types_ag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/ag/wlt_types_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/ag/wlt_types_imports.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.085813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    50260 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/api/extended_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/api/gw_ssid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/api/s3_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.085813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/automatic_configuration_tool/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15430 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.085813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/calibration_mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/calibration_mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13553 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.085813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    68659 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/common/analysis_data_bricks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/common/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     6004 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/common/utils_defines.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.085813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/connectivity_analyzer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/connectivity_analyzer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14407 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3084 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.085813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/firmware_update/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/firmware_update/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22977 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/firmware_update/firmware_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.085813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2177 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/gw_certificate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/gw_certificate_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.089813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/interface/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/interface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6770 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/interface/ble_simulator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/interface/brg_array.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/interface/if_defines.py
+-rw-rw-rw-   0 root         (0) root         (0)     7896 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/interface/mqtt.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/interface/packet_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     3381 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/interface/pkt_generator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.089813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15356 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/tests/coupling.py
+-rw-rw-rw-   0 root         (0) root         (0)     3665 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/tests/generated_packet_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/tests/generic.py
+-rw-rw-rw-   0 root         (0) root         (0)   190851 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/tests/packet_table.csv
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.089813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/interface/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/interface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/interface/uart_ports.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.089813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/log_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/log_viewer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.089813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/power_mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/power_mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
+-rw-rw-rw-   0 root         (0) root         (0)    26335 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/power_mgmt/power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     4801 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.089813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6057 2023-07-26 15:20:19.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-26 15:20:37.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:20:38.081813 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    11677 2023-07-26 15:20:37.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4727 2023-07-26 15:20:38.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 15:20:37.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      725 2023-07-26 15:20:37.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 15:20:37.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-26 15:20:37.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-26 15:20:37.000000 wiliot-deployment-tools-4.1.4/wiliot_deployment_tools.egg-info/top_level.txt
```

### Comparing `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/common.hcl` & `wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/common.hcl`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh` & `wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/terragrunt.hcl` & `wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/terragrunt.hcl`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/install_packages.sh` & `wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/install_packages.sh`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/terragrunt.hcl` & `wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/terragrunt.hcl`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/terragrunt.hcl` & `wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/terragrunt.hcl`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh` & `wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/terragrunt.hcl` & `wiliot-deployment-tools-4.1.4/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/terragrunt.hcl`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/.devcontainer/private/devcontainer.json` & `wiliot-deployment-tools-4.1.4/.devcontainer/private/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/.devcontainer/public/devcontainer.json` & `wiliot-deployment-tools-4.1.4/.devcontainer/public/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/LICENSE` & `wiliot-deployment-tools-4.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/Makefile` & `wiliot-deployment-tools-4.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/PKG-INFO` & `wiliot-deployment-tools-4.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.1.3
+Version: 4.1.4
 Summary: A library for interacting with Wiliot's Deployment Tools
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -201,14 +201,17 @@
 - Init Stage - Send 4 packet pairs (Data+SI) from 1 BRG, testing maximum/minimum RSSI and NFPKT Values encoded in SI packet
 - One Bridge Stage - Send packet pairs at increasing duplication (1->10) and increasing time delay between packets (15->255 ms) from 1 bridge, including simulated packet error.
 - Three Bridge Init Stage - send same data packet from 3 different bridges, each with different SI.
 - Three Bridge Stage - send same data packet from 3 different bridges, at increasing duplication (1->10) and increasing time delay between packets for each bridge (30->255).
 The test logs all sent packets, and all received packets from the tested GW in log files and outputs a summary of all sent packets in a CSV file (filepath specified at runtime).
 
 #### GW Certificate Release Notes:
+Version 4.1.4: 
+* Randomize bugfix
+
 Version 4.1.3:
 * Bugfixes
 * Support for Android
 * Support for python 3.11
 
 Version 4.1.0:
 * Coupling Test
@@ -232,17 +235,14 @@
 required arguments:
   -owner OWNER  Owner ID
   -gw GW        Gateway ID
   ```
 
 
 ## Release Notes:
-Version 4.1.3:
-* GW Certificate Bugfixes
-
 Version 4.1.1:
 * Bridge-Gw connectivity log print
 
 Version 4.1.0:
 * Custom message support
 * GW Certificate - coupling test
 * Fixes for calibration management
```

### Comparing `wiliot-deployment-tools-4.1.3/README.md` & `wiliot-deployment-tools-4.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -184,14 +184,17 @@
 - Init Stage - Send 4 packet pairs (Data+SI) from 1 BRG, testing maximum/minimum RSSI and NFPKT Values encoded in SI packet
 - One Bridge Stage - Send packet pairs at increasing duplication (1->10) and increasing time delay between packets (15->255 ms) from 1 bridge, including simulated packet error.
 - Three Bridge Init Stage - send same data packet from 3 different bridges, each with different SI.
 - Three Bridge Stage - send same data packet from 3 different bridges, at increasing duplication (1->10) and increasing time delay between packets for each bridge (30->255).
 The test logs all sent packets, and all received packets from the tested GW in log files and outputs a summary of all sent packets in a CSV file (filepath specified at runtime).
 
 #### GW Certificate Release Notes:
+Version 4.1.4: 
+* Randomize bugfix
+
 Version 4.1.3:
 * Bugfixes
 * Support for Android
 * Support for python 3.11
 
 Version 4.1.0:
 * Coupling Test
@@ -215,17 +218,14 @@
 required arguments:
   -owner OWNER  Owner ID
   -gw GW        Gateway ID
   ```
 
 
 ## Release Notes:
-Version 4.1.3:
-* GW Certificate Bugfixes
-
 Version 4.1.1:
 * Bridge-Gw connectivity log print
 
 Version 4.1.0:
 * Custom message support
 * GW Certificate - coupling test
 * Fixes for calibration management
```

### Comparing `wiliot-deployment-tools-4.1.3/bitbucket-pipelines.yml` & `wiliot-deployment-tools-4.1.4/bitbucket-pipelines.yml`

 * *Files 13% similar despite different names*

```diff
@@ -157,14 +157,53 @@
             - tree && find ./ -name "extended" && find ./ -name "extended" -type d -prune -exec rm -rf {} \; && tree
             - tree && find ./ -name "internal" && find ./ -name "internal" -type d -prune -exec rm -rf {} \; && tree
             - python3 setup.py sdist bdist_wheel
             - ls -al dist/ && ls -al build/
             # push into test-pypi
             - python3 -m twine upload --repository testpypi dist/*
 
+    update-patch-version-number-and-publish-slim-version-to-pypi:
+      - step:
+          name: update patch version number
+          <<: *wiliot-ci-image
+          script:
+            - pip3 install setuptools_scm
+            - pip3 install gitpython
+            - apk add tree
+            #print current version:
+            - python3 wiliot_deployment_tools/utils/get_version.py
+            #Update patch version by git tag:
+            - version="`python3 wiliot_deployment_tools/utils/get_version.py next_patch`" && echo $version && git tag -a -m "[skip ci] build number $BITBUCKET_BUILD_NUMBER set the library patch version to $version." $version  && git push origin $version
+            #print new version
+            - python3 wiliot_deployment_tools/utils/get_version.py
+      - step:
+          name: Build and publish slim version into pypi
+          <<: *wiliot-ci-image
+          script:
+            - pip3 install setuptools_scm build wheel twine
+            - pip3 install gitpython
+            - apk add tree
+            #Get current version (was already updated by prev steps) before cleaning internal files:
+            - version="`python3 wiliot_deployment_tools/utils/get_version.py`"
+            #update version.py with new patch version and build number:
+            - echo "__version__ = '$version'" > wiliot_deployment_tools/version.py
+            - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_deployment_tools/version.py
+            # configure testpypi and pypi access
+            - echo "[pypi]" > ~/.pypirc && echo "username = __token__" >> ~/.pypirc && echo "password = $PYPI_KEY" >> ~/.pypirc && echo "[testpypi]" >> ~/.pypirc && echo "username = __token__" >> ~/.pypirc && echo "password = $TEST_PYPI_KEY" >> ~/.pypirc
+            # cleanup all the "internal" folders
+            - tree && find ./ -name "extended" && find ./ -name "extended" -type d -prune -exec rm -rf {} \; && tree
+            - tree && find ./ -name "internal" && find ./ -name "internal" -type d -prune -exec rm -rf {} \; && tree
+            - python3 setup.py sdist bdist_wheel
+            #Logging(?):
+            - ls -al dist/ && ls -al build/
+            # push into pypi
+            - python3 -m twine upload --repository pypi dist/* #python3 -m twine upload --repository testpypi dist/*
+
+
+    
     run-unit-tests:
       - step:
           name: Run unit tests
           <<: *wiliot-ci-image
           script:
             - apk add tree
             - pip3 install pytest
```

### Comparing `wiliot-deployment-tools-4.1.3/ci/upload_to_s3.sh` & `wiliot-deployment-tools-4.1.4/ci/upload_to_s3.sh`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/ci.py` & `wiliot-deployment-tools-4.1.4/ci.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/dep-tools.dockerfile` & `wiliot-deployment-tools-4.1.4/dep-tools.dockerfile`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/gw_certificate.ipynb` & `wiliot-deployment-tools-4.1.4/gw_certificate.ipynb`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/setup.py` & `wiliot-deployment-tools-4.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/unittests/test_extended_api_edge.py` & `wiliot-deployment-tools-4.1.4/unittests/test_extended_api_edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/unittests/test_extended_api_platform.py` & `wiliot-deployment-tools-4.1.4/unittests/test_extended_api_platform.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/unittests/test_power_mgmt.py` & `wiliot-deployment-tools-4.1.4/unittests/test_power_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/unittests/test_slack_alerts.py` & `wiliot-deployment-tools-4.1.4/unittests/test_slack_alerts.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/unittests/test_test_tool.py` & `wiliot-deployment-tools-4.1.4/unittests/test_test_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/unittests/test_utils.py` & `wiliot-deployment-tools-4.1.4/unittests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/ut_defines.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/ag/ut_defines.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 UT_MQTT_LOG_FILE = "ut_mqtt_log.json"
 
 # GW defines
 GW_ID =                         "gatewayId"
 ADDITIONAL =                    "additional"
 REPORTED_CONF =                 "reportedConf"
 GW_CONF =                       "gatewayConf"
+GW_NAME =                       "gatewayName"
 GW_API_VERSION =                "apiVersion"
+LAT =                           "lat"
+LNG =                           "lng"
+
 
 GW_DATA_MODE =                  "gwDataMode"
 TAGS_AND_BRGS =                 "Tags & Bridges"
 TAGS_ONLY =                     "Tags only"
 BRGS_ONLY_38 =                  "Bridges only (ch38)"
 BRGS_ONLY_39 =                  "Bridges only (ch39)"
 HIBERNATE =                     "Hibernate"
@@ -23,14 +27,15 @@
 WIFI_VERSION =                  "interfaceChipSwVersion"
 BLE_VERSION =                   "bleChipSwVersion"
 DATA_COUPLING =                 "dataCoupling"
 GW_MGMT_MODE =                  "gwMgmtMode"
 GW_MODE =                       "gwMode"
 ACTIVE =                        "active"
 TRANSPARENT =                   "transparent"
+PROD =                          "prod"
 
 GET_INFO_ACTION =               "getGwInfo"
 REBOOT_GW_ACTION =              "rebootGw"
 LOG_PERIOD_ACTION =             "LogPeriodSet"
 GET_LOGS =                      "getLogs"
 GW_INFO =                       "gatewayInfo"
 GW_LOGS =                       "gatewayLogs"
@@ -85,37 +90,39 @@
 PACKETS =                       "packets"
 TIMESTAMP =                     "timestamp"
 ID =                            "id"
 CONFIG =                        "config"
 ACTION =                        "action"
 PAYLOAD =                       "payload"
 
+WLT_SERVER =                    "wiliotServer"
 PACER_INTERVAL =                "pacerInterval"
 PKT_TYPES_MASK =                "packetTypesMask"
 RX_TX_PERIOD =                  "rxTxPeriodMs"
 TX_PERIOD =                     "txPeriodMs"
 ENERGY_PATTERN =                "energyPattern"
 OUTPUT_POWER_2_4 =              "2.4GhzOutputPower"
 NFPKT =                         "nfpkt"
 RSSI =                          "rssi"
+USE_STAT_LOC =                  "useStaticLocation"
 
 # Speedtest
 SPEEDTEST_LATENCY =             "SpeedTestLatency"
 SPEEDTEST_STRESS =              "SpeedTestStress"
 LATENCY_STR =                   "SpeedTestLatency MQTT! Recived"
 STRESS_STR =                    "SpeedTestStress MQTT! finished sending"
 SPEEDTESTS =                    {SPEEDTEST_LATENCY:LATENCY_STR, SPEEDTEST_STRESS:STRESS_STR}
 SPEEDTEST_TIME_LIMIT =          GW_LOG_PERIOD + 20
 
 # External Sensors
 IS_SENSOR =                      "isSensor"
 IS_EMBEDDED =                    "isEmbedded"
 IS_SCRAMBLED =                   "isScrambled"
-SENSOR_UUID =                    "sensorServiceID"
-SENSOR_ID =                      "sensorID"
+SENSOR_UUID =                    "sensorServiceId"
+SENSOR_ID =                      "sensorId"
 
 ACTION_LONG_TIMEOUT =            120
 ACTION_SHORT_TIMEOUT =           5
 
 # Versions
 VERSIONS = {
     "1.5.0" : {WIFI_VERSION: "3.5.32", BLE_VERSION: "3.7.25"},
@@ -138,14 +145,15 @@
 GW_STAT_SCAN_TIMEOUT =              65
 BRG_STAT_SCAN_TIMEOUT =             65
 BRG_OTA_UPDATE_TIMEOUT =            210
 BRG_GLOBAL_PACING_SCAN_TIME =       180
 GW_VERSION_UPDATE_DATA_SCAN_TIME =  180
 GW_LATITUDE_DEFAULT =               33.0222
 GW_LONGITUDE_DEFAULT =              -117.0839
+GW_API_VER_DEFAULT =                "200"
 
 # Internal python ut defines - used only in ut
 PACER_INTERVAL_THRESHOLD =                          0.90
 GLOBAL_PACING_GROUP_THRESHOLD =                     0.70
 TX_REPETITION_THRESHOLD =                           0.50
 NO_RESPONSE =                                       "NO_RESPONSE"
 DONE =                                              "DONE"
@@ -157,16 +165,23 @@
 ACTION_BRG_TEST =                                   "action_brg_test"
 MGMT_PKT =                                          "mgmt_pkt"
 SIDE_INFO_PKT =                                     "side_info_pkt"
 DECODED_DATA =                                      "decoded_data"
 PACKETS_ECHO_OFF =                                  0x10
 
 # Non Default defines
-BRG_NON_DEFAULT_RXTX_PERIOD = 25
-BRG_NON_DEFAULT_TX_PERIOD = 8
+BRG_NON_DEFAULT_RXTX_PERIOD =                       25
+BRG_NON_DEFAULT_TX_PERIOD =                         8
+BRG_NON_DEFAULT_OUTPUT_POWER_SUB1G =                26
+BRG_NON_DEFAULT_PWR_MGMT_KEEP_ALIVE_SCAN =          0
+BRG_NON_DEFAULT_TX_REPETITION = 2
+
+LIS2DW12_ACCEL_NON_DEFAULT_STATE_THRESHOLD =        95
+LIS2DW12_ACCEL_NON_DEFAULT_WAKE_UP_DURATION =       121
+LIS2DW12_ACCEL_NON_DEFAULT_SLEEP_DURATION =         36
 
 # ---------------------------------------------------RTSA defines---------------------------------------------------
 # common defines
 TRACE_LOG_FILE_NAME =                   "TRACELOG"
 TRACE_LOG_FILE_PATH =                   "C:/SignalVu-PC Files/" + TRACE_LOG_FILE_NAME + ".TOV"
 
 # freq defines
```

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/wlt_types.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/ag/wlt_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from wiliot_deployment_tools.ag.ut_defines import *
 from wiliot_deployment_tools.ag.wlt_types_ag import *
 class WltPkt():
+    supported_pkt_types = WLT_PKT_TYPES
+
     def __init__(self, hdr=Hdr(), generic=None, pkt=None):
         self.hdr = hdr
         self.generic = generic
         self.pkt = pkt
 
     def __eq__(self, other):
         if isinstance(other, WltPkt):
@@ -33,17 +35,29 @@
             # MEL modules
             if self.generic.module_type == MODULE_IF and self.generic.msg_type == BRG_MGMT_MSG_TYPE_CFG_INFO:
                 self.pkt = ModuleIfV7()
                 self.pkt.set(string[14:62])
             elif self.generic.module_type == MODULE_ENERGY_2400:
                 self.pkt = ModuleEnergy2400V7()
                 self.pkt.set(string[14:62])
+            elif self.generic.module_type == MODULE_ENERGY_SUB1G:
+                self.pkt = ModuleEnergySub1GV7()
+                self.pkt.set(string[14:62])
             elif self.generic.module_type == MODULE_PWR_MGMT:
                 self.pkt = ModulePwrMgmtV7()
                 self.pkt.set(string[14:62])
+            elif self.generic.module_type == MODULE_PERIPH:
+                self.pkt = ModulePeriphV7()
+                self.pkt.set(string[14:62])
+            elif self.generic.module_type == MODULE_CALIBRATION:
+                self.pkt = ModuleCalibrationV7()
+                self.pkt.set(string[14:62])
+            elif self.generic.module_type == MODULE_DATAPATH:
+                self.pkt = ModuleDatapathV7()
+                self.pkt.set(string[14:62])
             # OLD global config
             elif self.generic.module_type == MODULE_GLOBAL:
                 if self.hdr.group_id == GROUP_ID_GW2BRG:
                     # GROUP_ID_GW2BRG
                     if self.generic.msg_type == BRG_MGMT_MSG_TYPE_CFG_SET:
                         self.pkt = Gw2BrgCfgV7()
                         self.pkt.set(string[14:62])
```

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/wlt_types_ag.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/ag/wlt_types_ag.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 SENSOR_ACTION_IGNORE = 0
 SENSOR_ACTION_ADD = 1
 SENSOR_ACTION_REMOVE = 2
 
 ACTION_EMPTY = 0
 ACTION_REBOOT = 1
 ACTION_BLINK = 2
+ACTION_GET_MODULE = 3
 ACTION_RESTORE_DEFAULTS = 4
 ACTION_SEND_HB = 5
 ACTION_EXT_SENSOR = 6
-ACTION_SPARSE_37 = 7
+ACTION_SPARSE_37_DEPRECATED = 7
 ACTION_GW_HB = 8
 
 API_VERSION_V0 = 0
 API_VERSION_V1 = 1
 API_VERSION_V2 = 2
 API_VERSION_V5 = 5 # Because of backward compatabilty issue we jumped from V2 to V5
 API_VERSION_V6 = 6
@@ -30,20 +31,21 @@
 API_VERSION_LATEST = 7
 
 API_VERSION_SENSOR_V0 = 0
 
 MODULE_EMPTY = 0
 MODULE_GLOBAL = 0
 MODULE_IF = 1
-MODULE_DATA_PATH = 2
+MODULE_DATAPATH = 2
 MODULE_ENERGY_2400 = 3
 MODULE_ENERGY_SUB1G = 4
 MODULE_CALIBRATION = 5
 MODULE_PWR_MGMT = 6
-MODULE_SENSOR = 7
+MODULE_SENSORS = 7
+MODULE_PERIPH = 8
 
 ENERGY_PATTERN_IDX_17 = 17
 ENERGY_PATTERN_IDX_18 = 18
 ENERGY_PATTERN_IDX_20 = 20
 ENERGY_PATTERN_IDX_24 = 24
 ENERGY_PATTERN_IDX_25 = 25
 ENERGY_PATTERN_IDX_26 = 26
@@ -58,14 +60,21 @@
 ENERGY_PATTERN_IDX_55 = 55
 ENERGY_PATTERN_IDX_56 = 56
 ENERGY_PATTERN_IDX_57 = 57
 ENERGY_PATTERN_IDX_61 = 61
 ENERGY_PATTERN_IDX_62 = 62
 ENERGY_PATTERN_IDX_63 = 63
 ENERGY_PATTERN_IDX_64 = 64
+ENERGY_PATTERN_IDX_65 = 65
+ENERGY_PATTERN_IDX_66 = 66
+ENERGY_PATTERN_IDX_67 = 67
+ENERGY_PATTERN_IDX_68 = 68
+ENERGY_PATTERN_IDX_71 = 71
+ENERGY_PATTERN_IDX_72 = 72
+ENERGY_PATTERN_IDX_73 = 73
 ENERGY_PATTERN_IDX_99 = 99
 ENERGY_PATTERN_IDX_LAST = ENERGY_PATTERN_IDX_99
 
 CHANNEL_FREQ_37 = 2402
 CHANNEL_FREQ_38 = 2426
 CHANNEL_FREQ_39 = 2480
 
@@ -74,14 +83,15 @@
 CHANNEL_39 = 39
 
 FREQUENCY_BAND_EDGE_2480 = 2480
 FREQUENCY_BAND_EDGE_2475 = 2475
 
 RADIO_TX_POWER_POS_2_DBM = 2
 RADIO_TX_POWER_POS_3_DBM = 3
+RADIO_TX_POWER_POS_6_DBM = 6
 
 SUB1G_FREQ_865700 = 865700
 SUB1G_FREQ_915000 = 915000
 SUB1G_FREQ_916300 = 916300
 SUB1G_FREQ_917500 = 917500
 SUB1G_FREQ_918000 = 918000
 SUB1G_FREQ_919100 = 919100
@@ -115,29 +125,35 @@
 HDR_DEFAULT_BRG_UUID_MSB = 0xC6
 HDR_DEFAULT_BRG_UUID_LSB = 0xFC
 HDR_DEFAULT_TAG_UUID_MSB = 0xAF
 HDR_DEFAULT_TAG_UUID_LSB = 0xFD
 
 BRG_DEFAULT_GLOBAL_PACING_GROUP = 0
 BRG_DEFAULT_SCAN_CH = CHANNEL_37
+BRG_DEFAULT_BRG_ENERGOUS_V1_OUTPUT_POWER_SUB_1_GHZ = SUB1G_OUTPUT_POWER_29
 BRG_DEFAULT_OUTPUT_POWER_SUB_1_GHZ = SUB1G_OUTPUT_POWER_32
+BRG_DEFAULT_BRG_ENERGOUS_V1_OUTPUT_POWER_SUB_1_GHZ_PROFILE = SUB1G_OUTPUT_POWER_PROFILE_29
 BRG_DEFAULT_OUTPUT_POWER_SUB_1_GHZ_PROFILE = SUB1G_OUTPUT_POWER_PROFILE_32
+BRG_DEFAULT_BRG_ENERGOUS_V1_RXTX_PERIOD = 100
 BRG_DEFAULT_RXTX_PERIOD = 15
+BRG_DEFAULT_BRG_ENERGOUS_V1_TX_PERIOD = 40
 BRG_DEFAULT_TX_PERIOD = 5
+BRG_DEFAULT_BRG_ENERGOUS_V1_ENERGY_PATTERN_IDX = ENERGY_PATTERN_IDX_71
 BRG_DEFAULT_ENERGY_PATTERN_IDX = ENERGY_PATTERN_IDX_50
 BRG_DEFAULT_SB_ENERGY_PATTERN_IDX = ENERGY_PATTERN_IDX_18
 BRG_DEFAULT_ENERGIZE_FREQUENCY_2_4 = FREQUENCY_BAND_EDGE_2480
 BRG_DEFAULT_BRG_ENERGOUS_V0_OUTPUT_POWER_2_4 = RADIO_TX_POWER_POS_3_DBM
+BRG_DEFAULT_BRG_ENERGOUS_V1_OUTPUT_POWER_2_4 = RADIO_TX_POWER_POS_6_DBM
+BRG_DEFAULT_BRG_ENERGOUS_V2_OUTPUT_POWER_2_4 = RADIO_TX_POWER_POS_3_DBM
 BRG_DEFAULT_OUTPUT_POWER_2_4 = RADIO_TX_POWER_POS_2_DBM
 BRG_DEFAULT_PACER_INTERVAL = 15
 BRG_DEFAULT_PKT_TYPES_MASK = 0
 BRG_DEFAULT_TX_PROB = 50
 BRG_DEFAULT_TX_REPETITION = 0
 BRG_DEFAULT_TRANSMIT_TIME_SUB_1_GHZ = 0
-BRG_DEFAULT_BRG_ENERGOUS_V0_SUB1G_FREQ = SUB1G_FREQ_918000
 BRG_DEFAULT_SUB1G_FREQ = SUB1G_FREQ_915000
 BRG_DEFAULT_SUB1G_FREQ_PROFILE = SUB1G_FREQ_PROFILE_915000
 
 BRG_MGMT_MSG_TYPE_CFG_INFO = 1
 BRG_MGMT_MSG_TYPE_OTA_UPDATE = 1
 BRG_MGMT_MSG_TYPE_HB = 2
 BRG_MGMT_MSG_TYPE_REBOOT = 3
@@ -148,14 +164,27 @@
 
 PWR_MGMT_DEFAULTS_LEDS_ON = 1
 PWR_MGMT_DEFAULTS_KEEP_ALIVE_PERIOD = 20
 PWR_MGMT_DEFAULTS_KEEP_ALIVE_SCAN = 300
 PWR_MGMT_DEFAULTS_ON_DURATION = 0
 PWR_MGMT_DEFAULTS_SLEEP_DURATION = 0
 
+PERIPH_ID_EMPTY = 0x00
+PERIPH_ID_LIS2DW12_ACCELEROMETER = 0x01
+PERIPH_ID_MAX_NUM = 0x02
+
+LIS2DW12_ACCEL_CFG_VERSION_V0 = 0
+LIS2DW12_ACCEL_CFG_VERSION_LATEST = 0
+
+LIS2DW12_ACCEL_DEFAULTS_CFG_PACKET_LENGTH = 3
+LIS2DW12_ACCEL_DEFAULTS_CFG_PACKET_VERSION = LIS2DW12_ACCEL_CFG_VERSION_LATEST
+LIS2DW12_ACCEL_DEFAULTS_STATE_THRESHOLD = 65
+LIS2DW12_ACCEL_DEFAULTS_WAKE_UP_DURATION = 91
+LIS2DW12_ACCEL_DEFAULTS_SLEEP_DURATION = 26
+
 class Hdr():
     def __init__(self, pkt_size=HDR_DEFAULT_PKT_SIZE, ad_type=HDR_DEFAULT_AD_TYPE, uuid_msb=HDR_DEFAULT_BRG_UUID_MSB, uuid_lsb=HDR_DEFAULT_BRG_UUID_LSB, group_id=0):
         self.pkt_size = pkt_size
         self.ad_type = ad_type
         self.uuid_msb = uuid_msb
         self.uuid_lsb = uuid_lsb
         self.group_id = group_id
@@ -279,15 +308,15 @@
         self.action_params = d[5]
 
 GW2BRG_CFG_V7_OUTPUT_POWER_SUB_1_GHZ_ENC = {SUB1G_OUTPUT_POWER_14:SUB1G_OUTPUT_POWER_PROFILE_14, SUB1G_OUTPUT_POWER_17:SUB1G_OUTPUT_POWER_PROFILE_17, SUB1G_OUTPUT_POWER_20:SUB1G_OUTPUT_POWER_PROFILE_20, SUB1G_OUTPUT_POWER_23:SUB1G_OUTPUT_POWER_PROFILE_23, SUB1G_OUTPUT_POWER_26:SUB1G_OUTPUT_POWER_PROFILE_26, SUB1G_OUTPUT_POWER_29:SUB1G_OUTPUT_POWER_PROFILE_29, SUB1G_OUTPUT_POWER_32:SUB1G_OUTPUT_POWER_PROFILE_32}
 GW2BRG_CFG_V7_OUTPUT_POWER_SUB_1_GHZ_DEC = {SUB1G_OUTPUT_POWER_PROFILE_14:SUB1G_OUTPUT_POWER_14, SUB1G_OUTPUT_POWER_PROFILE_17:SUB1G_OUTPUT_POWER_17, SUB1G_OUTPUT_POWER_PROFILE_20:SUB1G_OUTPUT_POWER_20, SUB1G_OUTPUT_POWER_PROFILE_23:SUB1G_OUTPUT_POWER_23, SUB1G_OUTPUT_POWER_PROFILE_26:SUB1G_OUTPUT_POWER_26, SUB1G_OUTPUT_POWER_PROFILE_29:SUB1G_OUTPUT_POWER_29, SUB1G_OUTPUT_POWER_PROFILE_32:SUB1G_OUTPUT_POWER_32}
 GW2BRG_CFG_V7_SUB1G_FREQ_PROFILE_ENC = {SUB1G_FREQ_915000:SUB1G_FREQ_PROFILE_915000, SUB1G_FREQ_865700:SUB1G_FREQ_PROFILE_865700, SUB1G_FREQ_916300:SUB1G_FREQ_PROFILE_916300, SUB1G_FREQ_917500:SUB1G_FREQ_PROFILE_917500, SUB1G_FREQ_918000:SUB1G_FREQ_PROFILE_918000, SUB1G_FREQ_919100:SUB1G_FREQ_PROFILE_919100}
 GW2BRG_CFG_V7_SUB1G_FREQ_PROFILE_DEC = {SUB1G_FREQ_PROFILE_915000:SUB1G_FREQ_915000, SUB1G_FREQ_PROFILE_865700:SUB1G_FREQ_865700, SUB1G_FREQ_PROFILE_916300:SUB1G_FREQ_916300, SUB1G_FREQ_PROFILE_917500:SUB1G_FREQ_917500, SUB1G_FREQ_PROFILE_918000:SUB1G_FREQ_918000, SUB1G_FREQ_PROFILE_919100:SUB1G_FREQ_919100}
 class Gw2BrgCfgV7():
-    def __init__(self, msg_type=0, global_pacing_group=BRG_DEFAULT_GLOBAL_PACING_GROUP, output_power_sub_1_ghz=BRG_DEFAULT_OUTPUT_POWER_SUB_1_GHZ, seq_id=0, brg_mac=0, unused0=0, pkt_types_mask=0, unused1=0, rxtx_period=BRG_DEFAULT_RXTX_PERIOD, tx_period=BRG_DEFAULT_TX_PERIOD, energy_pattern_idx=BRG_DEFAULT_ENERGY_PATTERN_IDX, output_power_2_4=BRG_DEFAULT_OUTPUT_POWER_2_4, pacer_interval=BRG_DEFAULT_PACER_INTERVAL, unused2=0, tx_prob=BRG_DEFAULT_TX_PROB, tx_repetition=BRG_DEFAULT_TX_REPETITION, transmit_time_sub_1_ghz=BRG_DEFAULT_TRANSMIT_TIME_SUB_1_GHZ, sub1g_freq_profile=BRG_DEFAULT_SUB1G_FREQ):
+    def __init__(self, msg_type=0, global_pacing_group=BRG_DEFAULT_GLOBAL_PACING_GROUP, output_power_sub_1_ghz=BRG_DEFAULT_OUTPUT_POWER_SUB_1_GHZ, seq_id=0, brg_mac=0, unused0=0, pkt_types_mask=BRG_DEFAULT_PKT_TYPES_MASK, unused1=0, rxtx_period=BRG_DEFAULT_RXTX_PERIOD, tx_period=BRG_DEFAULT_TX_PERIOD, energy_pattern_idx=BRG_DEFAULT_ENERGY_PATTERN_IDX, output_power_2_4=BRG_DEFAULT_OUTPUT_POWER_2_4, pacer_interval=BRG_DEFAULT_PACER_INTERVAL, unused2=0, tx_prob=BRG_DEFAULT_TX_PROB, tx_repetition=BRG_DEFAULT_TX_REPETITION, transmit_time_sub_1_ghz=BRG_DEFAULT_TRANSMIT_TIME_SUB_1_GHZ, sub1g_freq_profile=BRG_DEFAULT_SUB1G_FREQ):
         self.msg_type = msg_type
         self.global_pacing_group = global_pacing_group
         self.output_power_sub_1_ghz = output_power_sub_1_ghz
         self.seq_id = seq_id
         self.brg_mac = brg_mac
         self.unused0 = unused0
         self.pkt_types_mask = pkt_types_mask
@@ -319,19 +348,19 @@
                 self.tx_prob == other.tx_prob and
                 self.tx_repetition == other.tx_repetition and
                 self.sub1g_freq_profile == other.sub1g_freq_profile
             )
         return False
 
     def dump(self):
-        string = bitstruct.pack("u8u4u4u8u48u3u5u48u8u8u8u8u16u1u3u4u4u4", self.msg_type, self.global_pacing_group, GW2BRG_CFG_V7_OUTPUT_POWER_SUB_1_GHZ_ENC[self.output_power_sub_1_ghz], self.seq_id, self.brg_mac, self.unused0, self.pkt_types_mask, self.unused1, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval, self.unused2, ((self.tx_prob-30)//10), self.tx_repetition, self.transmit_time_sub_1_ghz, GW2BRG_CFG_V7_SUB1G_FREQ_PROFILE_ENC[self.sub1g_freq_profile])
+        string = bitstruct.pack("u8u4u4u8u48u3u5u48u8u8u8s8u16u1u3u4u4u4", self.msg_type, self.global_pacing_group, GW2BRG_CFG_V7_OUTPUT_POWER_SUB_1_GHZ_ENC[self.output_power_sub_1_ghz], self.seq_id, self.brg_mac, self.unused0, self.pkt_types_mask, self.unused1, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval, self.unused2, ((self.tx_prob-30)//10), self.tx_repetition, self.transmit_time_sub_1_ghz, GW2BRG_CFG_V7_SUB1G_FREQ_PROFILE_ENC[self.sub1g_freq_profile])
         return string.hex().upper()
 
     def set(self, string):
-        d = bitstruct.unpack("u8u4u4u8u48u3u5u48u8u8u8u8u16u1u3u4u4u4", binascii.unhexlify(string))
+        d = bitstruct.unpack("u8u4u4u8u48u3u5u48u8u8u8s8u16u1u3u4u4u4", binascii.unhexlify(string))
         self.msg_type = d[0]
         self.global_pacing_group = d[1]
         self.output_power_sub_1_ghz = GW2BRG_CFG_V7_OUTPUT_POWER_SUB_1_GHZ_DEC[d[2]]
         self.seq_id = d[3]
         self.brg_mac = d[4]
         self.unused0 = d[5]
         self.pkt_types_mask = d[6]
@@ -382,19 +411,19 @@
                 self.tx_prob == other.tx_prob and
                 self.tx_repetition == other.tx_repetition and
                 self.sub1g_freq_profile == other.sub1g_freq_profile
             )
         return False
 
     def dump(self):
-        string = bitstruct.pack("u8u4u4u8u48u8u48u8u8u8u8u16u1u3u4u4u4", self.msg_type, self.global_pacing_group, self.output_power_sub_1_ghz, self.seq_id, self.brg_mac, self.unused0, self.unused1, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval, self.unused2, self.tx_prob, self.tx_repetition, self.transmit_time_sub_1_ghz, self.sub1g_freq_profile)
+        string = bitstruct.pack("u8u4u4u8u48u8u48u8u8u8s8u16u1u3u4u4u4", self.msg_type, self.global_pacing_group, self.output_power_sub_1_ghz, self.seq_id, self.brg_mac, self.unused0, self.unused1, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval, self.unused2, self.tx_prob, self.tx_repetition, self.transmit_time_sub_1_ghz, self.sub1g_freq_profile)
         return string.hex().upper()
 
     def set(self, string):
-        d = bitstruct.unpack("u8u4u4u8u48u8u48u8u8u8u8u16u1u3u4u4u4", binascii.unhexlify(string))
+        d = bitstruct.unpack("u8u4u4u8u48u8u48u8u8u8s8u16u1u3u4u4u4", binascii.unhexlify(string))
         self.msg_type = d[0]
         self.global_pacing_group = d[1]
         self.output_power_sub_1_ghz = d[2]
         self.seq_id = d[3]
         self.brg_mac = d[4]
         self.unused0 = d[5]
         self.unused1 = d[6]
@@ -443,19 +472,19 @@
                 self.tx_prob == other.tx_prob and
                 self.stat_freq == other.stat_freq and
                 self.sub1g_freq_profile == other.sub1g_freq_profile
             )
         return False
 
     def dump(self):
-        string = bitstruct.pack("u8u4u4u8u48u56u8u8u8u8u16u1u3u4u4u4", self.msg_type, self.unused0, self.output_power_sub_1_ghz, self.seq_id, self.brg_mac, self.unused1, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval, self.global_pacing, self.tx_prob, self.stat_freq, self.transmit_time_sub_1_ghz, self.sub1g_freq_profile)
+        string = bitstruct.pack("u8u4u4u8u48u56u8u8u8s8u16u1u3u4u4u4", self.msg_type, self.unused0, self.output_power_sub_1_ghz, self.seq_id, self.brg_mac, self.unused1, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval, self.global_pacing, self.tx_prob, self.stat_freq, self.transmit_time_sub_1_ghz, self.sub1g_freq_profile)
         return string.hex().upper()
 
     def set(self, string):
-        d = bitstruct.unpack("u8u4u4u8u48u56u8u8u8u8u16u1u3u4u4u4", binascii.unhexlify(string))
+        d = bitstruct.unpack("u8u4u4u8u48u56u8u8u8s8u16u1u3u4u4u4", binascii.unhexlify(string))
         self.msg_type = d[0]
         self.unused0 = d[1]
         self.output_power_sub_1_ghz = d[2]
         self.seq_id = d[3]
         self.brg_mac = d[4]
         self.unused1 = d[5]
         self.rxtx_period = d[6]
@@ -506,19 +535,19 @@
                 self.tx_prob == other.tx_prob and
                 self.stat_freq == other.stat_freq and
                 self.sub1g_freq_profile == other.sub1g_freq_profile
             )
         return False
 
     def dump(self):
-        string = bitstruct.pack("u8u4u4u8u48u48u8u8u8u8u8u16u1u3u4u4u4", self.msg_type, self.unused, self.output_power_sub_1_ghz, self.seq_id, self.brg_mac, self.gw_mac, self.rx_rssi, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval, self.global_pacing, self.tx_prob, self.stat_freq, self.transmit_time_sub_1_ghz, self.sub1g_freq_profile)
+        string = bitstruct.pack("u8u4u4u8u48u48u8u8u8u8s8u16u1u3u4u4u4", self.msg_type, self.unused, self.output_power_sub_1_ghz, self.seq_id, self.brg_mac, self.gw_mac, self.rx_rssi, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval, self.global_pacing, self.tx_prob, self.stat_freq, self.transmit_time_sub_1_ghz, self.sub1g_freq_profile)
         return string.hex().upper()
 
     def set(self, string):
-        d = bitstruct.unpack("u8u4u4u8u48u48u8u8u8u8u8u16u1u3u4u4u4", binascii.unhexlify(string))
+        d = bitstruct.unpack("u8u4u4u8u48u48u8u8u8u8s8u16u1u3u4u4u4", binascii.unhexlify(string))
         self.msg_type = d[0]
         self.unused = d[1]
         self.output_power_sub_1_ghz = d[2]
         self.seq_id = d[3]
         self.brg_mac = d[4]
         self.gw_mac = d[5]
         self.rx_rssi = d[6]
@@ -562,19 +591,19 @@
                 self.output_power == other.output_power and
                 self.pacer_interval == other.pacer_interval and
                 self.tx_prob == other.tx_prob
             )
         return False
 
     def dump(self):
-        string = bitstruct.pack("u8u8u8u48u48u8u8u8u8u8u16u8u8", self.msg_type, self.unused0, self.seq_id, self.brg_mac, self.gw_mac, self.rx_rssi, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power, self.pacer_interval, self.tx_prob, self.unused1)
+        string = bitstruct.pack("u8u8u8u48u48u8u8u8u8s8u16u8u8", self.msg_type, self.unused0, self.seq_id, self.brg_mac, self.gw_mac, self.rx_rssi, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power, self.pacer_interval, self.tx_prob, self.unused1)
         return string.hex().upper()
 
     def set(self, string):
-        d = bitstruct.unpack("u8u8u8u48u48u8u8u8u8u8u16u8u8", binascii.unhexlify(string))
+        d = bitstruct.unpack("u8u8u8u48u48u8u8u8u8s8u16u8u8", binascii.unhexlify(string))
         self.msg_type = d[0]
         self.unused0 = d[1]
         self.seq_id = d[2]
         self.brg_mac = d[3]
         self.gw_mac = d[4]
         self.rx_rssi = d[5]
         self.rxtx_period = d[6]
@@ -586,15 +615,15 @@
         self.unused1 = d[12]
 
 BRG2GW_CFG_V7_OUTPUT_POWER_SUB_1_GHZ_ENC = {SUB1G_OUTPUT_POWER_14:SUB1G_OUTPUT_POWER_PROFILE_14, SUB1G_OUTPUT_POWER_17:SUB1G_OUTPUT_POWER_PROFILE_17, SUB1G_OUTPUT_POWER_20:SUB1G_OUTPUT_POWER_PROFILE_20, SUB1G_OUTPUT_POWER_23:SUB1G_OUTPUT_POWER_PROFILE_23, SUB1G_OUTPUT_POWER_26:SUB1G_OUTPUT_POWER_PROFILE_26, SUB1G_OUTPUT_POWER_29:SUB1G_OUTPUT_POWER_PROFILE_29, SUB1G_OUTPUT_POWER_32:SUB1G_OUTPUT_POWER_PROFILE_32}
 BRG2GW_CFG_V7_OUTPUT_POWER_SUB_1_GHZ_DEC = {SUB1G_OUTPUT_POWER_PROFILE_14:SUB1G_OUTPUT_POWER_14, SUB1G_OUTPUT_POWER_PROFILE_17:SUB1G_OUTPUT_POWER_17, SUB1G_OUTPUT_POWER_PROFILE_20:SUB1G_OUTPUT_POWER_20, SUB1G_OUTPUT_POWER_PROFILE_23:SUB1G_OUTPUT_POWER_23, SUB1G_OUTPUT_POWER_PROFILE_26:SUB1G_OUTPUT_POWER_26, SUB1G_OUTPUT_POWER_PROFILE_29:SUB1G_OUTPUT_POWER_29, SUB1G_OUTPUT_POWER_PROFILE_32:SUB1G_OUTPUT_POWER_32}
 BRG2GW_CFG_V7_SUB1G_FREQ_PROFILE_ENC = {SUB1G_FREQ_915000:SUB1G_FREQ_PROFILE_915000, SUB1G_FREQ_865700:SUB1G_FREQ_PROFILE_865700, SUB1G_FREQ_916300:SUB1G_FREQ_PROFILE_916300, SUB1G_FREQ_917500:SUB1G_FREQ_PROFILE_917500, SUB1G_FREQ_918000:SUB1G_FREQ_PROFILE_918000, SUB1G_FREQ_919100:SUB1G_FREQ_PROFILE_919100}
 BRG2GW_CFG_V7_SUB1G_FREQ_PROFILE_DEC = {SUB1G_FREQ_PROFILE_915000:SUB1G_FREQ_915000, SUB1G_FREQ_PROFILE_865700:SUB1G_FREQ_865700, SUB1G_FREQ_PROFILE_916300:SUB1G_FREQ_916300, SUB1G_FREQ_PROFILE_917500:SUB1G_FREQ_917500, SUB1G_FREQ_PROFILE_918000:SUB1G_FREQ_918000, SUB1G_FREQ_PROFILE_919100:SUB1G_FREQ_919100}
 class Brg2GwCfgV7():
-    def __init__(self, msg_type=0, api_version=7, seq_id=0, unused0=0, tx_prob=BRG_DEFAULT_TX_PROB, tx_repetition=BRG_DEFAULT_TX_REPETITION, global_pacing_group=BRG_DEFAULT_GLOBAL_PACING_GROUP, output_power_sub_1_ghz=BRG_DEFAULT_OUTPUT_POWER_SUB_1_GHZ, transmit_time_sub_1_ghz=BRG_DEFAULT_TRANSMIT_TIME_SUB_1_GHZ, sub1g_freq_profile=BRG_DEFAULT_SUB1G_FREQ, bl_version=0, board_type=0, unused1=0, pkt_types_mask=0, brg_mac=0, major_ver=0, minor_ver=0, build_ver=0, rxtx_period=BRG_DEFAULT_RXTX_PERIOD, tx_period=BRG_DEFAULT_TX_PERIOD, energy_pattern_idx=BRG_DEFAULT_ENERGY_PATTERN_IDX, output_power_2_4=BRG_DEFAULT_OUTPUT_POWER_2_4, pacer_interval=BRG_DEFAULT_PACER_INTERVAL):
+    def __init__(self, msg_type=0, api_version=7, seq_id=0, unused0=0, tx_prob=BRG_DEFAULT_TX_PROB, tx_repetition=BRG_DEFAULT_TX_REPETITION, global_pacing_group=BRG_DEFAULT_GLOBAL_PACING_GROUP, output_power_sub_1_ghz=BRG_DEFAULT_OUTPUT_POWER_SUB_1_GHZ, transmit_time_sub_1_ghz=BRG_DEFAULT_TRANSMIT_TIME_SUB_1_GHZ, sub1g_freq_profile=BRG_DEFAULT_SUB1G_FREQ, bl_version=0, board_type=0, unused1=0, pkt_types_mask=BRG_DEFAULT_PKT_TYPES_MASK, brg_mac=0, major_ver=0, minor_ver=0, build_ver=0, rxtx_period=BRG_DEFAULT_RXTX_PERIOD, tx_period=BRG_DEFAULT_TX_PERIOD, energy_pattern_idx=BRG_DEFAULT_ENERGY_PATTERN_IDX, output_power_2_4=BRG_DEFAULT_OUTPUT_POWER_2_4, pacer_interval=BRG_DEFAULT_PACER_INTERVAL):
         self.msg_type = msg_type
         self.api_version = api_version
         self.seq_id = seq_id
         self.unused0 = unused0
         self.tx_prob = tx_prob
         self.tx_repetition = tx_repetition
         self.global_pacing_group = global_pacing_group
@@ -653,19 +682,19 @@
                 self.energy_pattern_idx == other.energy_pattern_idx and
                 self.output_power_2_4 == other.output_power_2_4 and
                 self.pacer_interval == other.pacer_interval
             )
         return False
 
     def dump(self):
-        string = bitstruct.pack("u8u8u8u1u3u4u4u4u4u4u8u8u3u5u48u8u8u8u8u8u8u8u16", self.msg_type, self.api_version, self.seq_id, self.unused0, ((self.tx_prob-30)//10), self.tx_repetition, self.global_pacing_group, BRG2GW_CFG_V7_OUTPUT_POWER_SUB_1_GHZ_ENC[self.output_power_sub_1_ghz], self.transmit_time_sub_1_ghz, BRG2GW_CFG_V7_SUB1G_FREQ_PROFILE_ENC[self.sub1g_freq_profile], self.bl_version, self.board_type, self.unused1, self.pkt_types_mask, self.brg_mac, self.major_ver, self.minor_ver, self.build_ver, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval)
+        string = bitstruct.pack("u8u8u8u1u3u4u4u4u4u4u8u8u3u5u48u8u8u8u8u8u8s8u16", self.msg_type, self.api_version, self.seq_id, self.unused0, ((self.tx_prob-30)//10), self.tx_repetition, self.global_pacing_group, BRG2GW_CFG_V7_OUTPUT_POWER_SUB_1_GHZ_ENC[self.output_power_sub_1_ghz], self.transmit_time_sub_1_ghz, BRG2GW_CFG_V7_SUB1G_FREQ_PROFILE_ENC[self.sub1g_freq_profile], self.bl_version, self.board_type, self.unused1, self.pkt_types_mask, self.brg_mac, self.major_ver, self.minor_ver, self.build_ver, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval)
         return string.hex().upper()
 
     def set(self, string):
-        d = bitstruct.unpack("u8u8u8u1u3u4u4u4u4u4u8u8u3u5u48u8u8u8u8u8u8u8u16", binascii.unhexlify(string))
+        d = bitstruct.unpack("u8u8u8u1u3u4u4u4u4u4u8u8u3u5u48u8u8u8u8u8u8s8u16", binascii.unhexlify(string))
         self.msg_type = d[0]
         self.api_version = d[1]
         self.seq_id = d[2]
         self.unused0 = d[3]
         self.tx_prob = ((d[4]*10)+30)
         self.tx_repetition = d[5]
         self.global_pacing_group = d[6]
@@ -747,19 +776,19 @@
                 self.energy_pattern_idx == other.energy_pattern_idx and
                 self.output_power_2_4 == other.output_power_2_4 and
                 self.pacer_interval == other.pacer_interval
             )
         return False
 
     def dump(self):
-        string = bitstruct.pack("u8u8u8u1u3u4u4u4u4u4u8u8u8u48u8u8u8u8u8u8u8u16", self.msg_type, self.api_version, self.seq_id, self.unused0, self.tx_prob, self.tx_repetition, self.global_pacing_group, self.output_power_sub_1_ghz, self.transmit_time_sub_1_ghz, self.sub1g_freq_profile, self.bl_version, self.board_type, self.unused1, self.brg_mac, self.major_ver, self.minor_ver, self.build_ver, self.cycle_time, self.transmit_time_2_4, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval)
+        string = bitstruct.pack("u8u8u8u1u3u4u4u4u4u4u8u8u8u48u8u8u8u8u8u8s8u16", self.msg_type, self.api_version, self.seq_id, self.unused0, self.tx_prob, self.tx_repetition, self.global_pacing_group, self.output_power_sub_1_ghz, self.transmit_time_sub_1_ghz, self.sub1g_freq_profile, self.bl_version, self.board_type, self.unused1, self.brg_mac, self.major_ver, self.minor_ver, self.build_ver, self.cycle_time, self.transmit_time_2_4, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval)
         return string.hex().upper()
 
     def set(self, string):
-        d = bitstruct.unpack("u8u8u8u1u3u4u4u4u4u4u8u8u8u48u8u8u8u8u8u8u8u16", binascii.unhexlify(string))
+        d = bitstruct.unpack("u8u8u8u1u3u4u4u4u4u4u8u8u8u48u8u8u8u8u8u8s8u16", binascii.unhexlify(string))
         self.msg_type = d[0]
         self.api_version = d[1]
         self.seq_id = d[2]
         self.unused0 = d[3]
         self.tx_prob = d[4]
         self.tx_repetition = d[5]
         self.global_pacing_group = d[6]
@@ -840,19 +869,19 @@
                 self.energy_pattern_idx == other.energy_pattern_idx and
                 self.output_power_2_4 == other.output_power_2_4 and
                 self.pacer_interval == other.pacer_interval
             )
         return False
 
     def dump(self):
-        string = bitstruct.pack("u8u8u8u1u3u4u4u4u4u4u8u8u8u48u8u8u8u8u8u8u8u16", self.msg_type, self.api_version, self.seq_id, self.global_pacing, self.tx_prob, self.stat_freq, self.unused0, self.output_power_sub_1_ghz, self.transmit_time_sub_1_ghz, self.sub1g_freq_profile, self.bl_version, self.board_type, self.unused1, self.brg_mac, self.major_ver, self.minor_ver, self.build_ver, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval)
+        string = bitstruct.pack("u8u8u8u1u3u4u4u4u4u4u8u8u8u48u8u8u8u8u8u8s8u16", self.msg_type, self.api_version, self.seq_id, self.global_pacing, self.tx_prob, self.stat_freq, self.unused0, self.output_power_sub_1_ghz, self.transmit_time_sub_1_ghz, self.sub1g_freq_profile, self.bl_version, self.board_type, self.unused1, self.brg_mac, self.major_ver, self.minor_ver, self.build_ver, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval)
         return string.hex().upper()
 
     def set(self, string):
-        d = bitstruct.unpack("u8u8u8u1u3u4u4u4u4u4u8u8u8u48u8u8u8u8u8u8u8u16", binascii.unhexlify(string))
+        d = bitstruct.unpack("u8u8u8u1u3u4u4u4u4u4u8u8u8u48u8u8u8u8u8u8s8u16", binascii.unhexlify(string))
         self.msg_type = d[0]
         self.api_version = d[1]
         self.seq_id = d[2]
         self.global_pacing = d[3]
         self.tx_prob = d[4]
         self.stat_freq = d[5]
         self.unused0 = d[6]
@@ -931,19 +960,19 @@
                 self.energy_pattern_idx == other.energy_pattern_idx and
                 self.output_power_2_4 == other.output_power_2_4 and
                 self.pacer_interval == other.pacer_interval
             )
         return False
 
     def dump(self):
-        string = bitstruct.pack("u8u8u8u1u3u4u4u4u4u4u8u16u48u8u8u8u8u8u8u8u16", self.msg_type, self.board_type, self.seq_id, self.global_pacing, self.tx_prob, self.stat_freq, self.unused0, self.output_power_sub_1_ghz, self.transmit_time_sub_1_ghz, self.sub1g_freq_profile, self.bl_version, self.unused1, self.brg_mac, self.major_ver, self.minor_ver, self.build_ver, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval)
+        string = bitstruct.pack("u8u8u8u1u3u4u4u4u4u4u8u16u48u8u8u8u8u8u8s8u16", self.msg_type, self.board_type, self.seq_id, self.global_pacing, self.tx_prob, self.stat_freq, self.unused0, self.output_power_sub_1_ghz, self.transmit_time_sub_1_ghz, self.sub1g_freq_profile, self.bl_version, self.unused1, self.brg_mac, self.major_ver, self.minor_ver, self.build_ver, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power_2_4, self.pacer_interval)
         return string.hex().upper()
 
     def set(self, string):
-        d = bitstruct.unpack("u8u8u8u1u3u4u4u4u4u4u8u16u48u8u8u8u8u8u8u8u16", binascii.unhexlify(string))
+        d = bitstruct.unpack("u8u8u8u1u3u4u4u4u4u4u8u16u48u8u8u8u8u8u8s8u16", binascii.unhexlify(string))
         self.msg_type = d[0]
         self.board_type = d[1]
         self.seq_id = d[2]
         self.global_pacing = d[3]
         self.tx_prob = d[4]
         self.stat_freq = d[5]
         self.unused0 = d[6]
@@ -1010,19 +1039,19 @@
                 self.energy_pattern_idx == other.energy_pattern_idx and
                 self.output_power == other.output_power and
                 self.pacer_interval == other.pacer_interval
             )
         return False
 
     def dump(self):
-        string = bitstruct.pack("u8u8u8u48u48u4u4u4u4u7u1u8u8u8u8u16", self.msg_type, self.unused0, self.seq_id, self.gw_mac, self.brg_mac, self.major_ver, self.minor_ver, self.build_ver, self.unused1, self.tx_prob, self.is_dual_band, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power, self.pacer_interval)
+        string = bitstruct.pack("u8u8u8u48u48u4u4u4u4u7u1u8u8u8s8u16", self.msg_type, self.unused0, self.seq_id, self.gw_mac, self.brg_mac, self.major_ver, self.minor_ver, self.build_ver, self.unused1, self.tx_prob, self.is_dual_band, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power, self.pacer_interval)
         return string.hex().upper()
 
     def set(self, string):
-        d = bitstruct.unpack("u8u8u8u48u48u4u4u4u4u7u1u8u8u8u8u16", binascii.unhexlify(string))
+        d = bitstruct.unpack("u8u8u8u48u48u4u4u4u4u7u1u8u8u8s8u16", binascii.unhexlify(string))
         self.msg_type = d[0]
         self.unused0 = d[1]
         self.seq_id = d[2]
         self.gw_mac = d[3]
         self.brg_mac = d[4]
         self.major_ver = d[5]
         self.minor_ver = d[6]
@@ -1079,19 +1108,19 @@
                 self.energy_pattern_idx == other.energy_pattern_idx and
                 self.output_power == other.output_power and
                 self.pacer_interval == other.pacer_interval
             )
         return False
 
     def dump(self):
-        string = bitstruct.pack("u8u8u8u48u48u8u8u8u8u8u8u8u16", self.msg_type, self.bridge_id, self.seq_id, self.gw_mac, self.brg_mac, self.major_ver, self.minor_ver, self.build_ver, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power, self.pacer_interval)
+        string = bitstruct.pack("u8u8u8u48u48u8u8u8u8u8u8s8u16", self.msg_type, self.bridge_id, self.seq_id, self.gw_mac, self.brg_mac, self.major_ver, self.minor_ver, self.build_ver, self.rxtx_period, self.tx_period, self.energy_pattern_idx, self.output_power, self.pacer_interval)
         return string.hex().upper()
 
     def set(self, string):
-        d = bitstruct.unpack("u8u8u8u48u48u8u8u8u8u8u8u8u16", binascii.unhexlify(string))
+        d = bitstruct.unpack("u8u8u8u48u48u8u8u8u8u8u8s8u16", binascii.unhexlify(string))
         self.msg_type = d[0]
         self.bridge_id = d[1]
         self.seq_id = d[2]
         self.gw_mac = d[3]
         self.brg_mac = d[4]
         self.major_ver = d[5]
         self.minor_ver = d[6]
@@ -1469,18 +1498,18 @@
         self.p2_pacing = d[3]
         self.p1_pacing = d[4]
         self.p0_pacing = d[5]
 
 class PwrMgmt():
     def __init__(self, leds_on=PWR_MGMT_DEFAULTS_LEDS_ON, keep_alive_scan=PWR_MGMT_DEFAULTS_KEEP_ALIVE_SCAN, keep_alive_period=PWR_MGMT_DEFAULTS_KEEP_ALIVE_PERIOD, on_duration=PWR_MGMT_DEFAULTS_ON_DURATION, sleep_duration=PWR_MGMT_DEFAULTS_SLEEP_DURATION, unused=0):
         self.leds_on = leds_on
-        self.keep_alive_scan = keep_alive_scan # 10msec resolution
-        self.keep_alive_period = keep_alive_period # 5sec resolution
-        self.on_duration = on_duration # 30sec resolution
-        self.sleep_duration = sleep_duration # 60sec resolution
+        self.keep_alive_scan = keep_alive_scan # 10 [msec] resolution
+        self.keep_alive_period = keep_alive_period # 5 [sec] resolution
+        self.on_duration = on_duration # 30 [sec] resolution
+        self.sleep_duration = sleep_duration # 60 [sec] resolution
         self.unused = unused
 
     def __eq__(self, other):
         if isinstance(other, PwrMgmt):
             return (
                 self.leds_on == other.leds_on and
                 self.keep_alive_scan == other.keep_alive_scan and
@@ -1499,35 +1528,107 @@
         self.leds_on = d[0]
         self.keep_alive_scan = d[1]
         self.keep_alive_period = d[2]
         self.on_duration = d[3]
         self.sleep_duration = d[4]
         self.unused = d[5]
 
+class Lis2Dw12AccelCfg():
+    def __init__(self, api_version=LIS2DW12_ACCEL_DEFAULTS_CFG_PACKET_VERSION, state_threshold=LIS2DW12_ACCEL_DEFAULTS_STATE_THRESHOLD, wake_up_duration=LIS2DW12_ACCEL_DEFAULTS_WAKE_UP_DURATION, sleep_duration=LIS2DW12_ACCEL_DEFAULTS_SLEEP_DURATION, unused=0):
+        self.api_version = api_version
+        self.state_threshold = state_threshold # 31.25 [mg] resolution
+        self.wake_up_duration = wake_up_duration # 3 [sec] resolution
+        self.sleep_duration = sleep_duration # 5 [sec] resolution
+        self.unused = unused
+
+    def __eq__(self, other):
+        if isinstance(other, Lis2Dw12AccelCfg):
+            return (
+                self.api_version == other.api_version and
+                self.state_threshold == other.state_threshold and
+                self.wake_up_duration == other.wake_up_duration and
+                self.sleep_duration == other.sleep_duration
+            )
+        return False
+
+    def dump(self):
+        string = bitstruct.pack("u8u6u6u4u8", self.api_version, ((self.state_threshold-0)//31.25), ((self.wake_up_duration-0.03)//3), ((self.sleep_duration-0.16)//5.12), self.unused)
+        return string.hex().upper()
+
+    def set(self, string):
+        d = bitstruct.unpack("u8u6u6u4u8", binascii.unhexlify(string))
+        self.api_version = d[0]
+        self.state_threshold = ((d[1]*31.25)+0)
+        self.wake_up_duration = ((d[2]*3)+0.03)
+        self.sleep_duration = ((d[3]*5.12)+0.16)
+        self.unused = d[4]
+
+class GetModuleParams():
+    def __init__(self, interface=0, datapath=0, energy2400=0, energy_sub1g=0, calibration=0, pwr_mgmt=0, sensors=0, periph=0, unused0=0):
+        self.interface = interface
+        self.datapath = datapath
+        self.energy2400 = energy2400
+        self.energy_sub1g = energy_sub1g
+        self.calibration = calibration
+        self.pwr_mgmt = pwr_mgmt
+        self.sensors = sensors
+        self.periph = periph
+        self.unused0 = unused0
+
+    def __eq__(self, other):
+        if isinstance(other, GetModuleParams):
+            return (
+                self.interface == other.interface and
+                self.datapath == other.datapath and
+                self.energy2400 == other.energy2400 and
+                self.energy_sub1g == other.energy_sub1g and
+                self.calibration == other.calibration and
+                self.pwr_mgmt == other.pwr_mgmt and
+                self.sensors == other.sensors and
+                self.periph == other.periph
+            )
+        return False
+
+    def dump(self):
+        string = bitstruct.pack("u1u1u1u1u1u1u1u1u104", self.interface, self.datapath, self.energy2400, self.energy_sub1g, self.calibration, self.pwr_mgmt, self.sensors, self.periph, self.unused0)
+        return string.hex().upper()
+
+    def set(self, string):
+        d = bitstruct.unpack("u1u1u1u1u1u1u1u1u104", binascii.unhexlify(string))
+        self.interface = d[0]
+        self.datapath = d[1]
+        self.energy2400 = d[2]
+        self.energy_sub1g = d[3]
+        self.calibration = d[4]
+        self.pwr_mgmt = d[5]
+        self.sensors = d[6]
+        self.periph = d[7]
+        self.unused0 = d[8]
+
 class ModuleIfV7():
-    def __init__(self, module_type=MODULE_IF, msg_type=0, api_version=7, seq_id=0, brg_mac=0, board_type=0, bl_version=0, major_ver=0, minor_ver=0, patch_ver=0, sup_cap_glob=0, sup_cap_datapath=0, sup_cap_energy_2_4=0, sup_cap_sub1g_energy=0, sup_cap_calibration=0, sup_cap_power_mgmt=0, sup_cap_sensors=0, unused0=0, unused1=0):
+    def __init__(self, module_type=MODULE_IF, msg_type=0, api_version=API_VERSION_V7, seq_id=0, brg_mac=0, board_type=0, bl_version=0, major_ver=0, minor_ver=0, patch_ver=0, sup_cap_glob=0, sup_cap_datapath=0, sup_cap_energy2400=0, sup_cap_energy_sub1g=0, sup_cap_calibration=0, sup_cap_pwr_mgmt=0, sup_cap_sensors=0, sup_cap_periph=0, unused0=0):
         self.module_type = module_type
         self.msg_type = msg_type
         self.api_version = api_version
         self.seq_id = seq_id
         self.brg_mac = brg_mac
         self.board_type = board_type
         self.bl_version = bl_version
         self.major_ver = major_ver
         self.minor_ver = minor_ver
         self.patch_ver = patch_ver
         self.sup_cap_glob = sup_cap_glob
         self.sup_cap_datapath = sup_cap_datapath
-        self.sup_cap_energy_2_4 = sup_cap_energy_2_4
-        self.sup_cap_sub1g_energy = sup_cap_sub1g_energy
+        self.sup_cap_energy2400 = sup_cap_energy2400
+        self.sup_cap_energy_sub1g = sup_cap_energy_sub1g
         self.sup_cap_calibration = sup_cap_calibration
-        self.sup_cap_power_mgmt = sup_cap_power_mgmt
+        self.sup_cap_pwr_mgmt = sup_cap_pwr_mgmt
         self.sup_cap_sensors = sup_cap_sensors
+        self.sup_cap_periph = sup_cap_periph
         self.unused0 = unused0
-        self.unused1 = unused1
 
     def __eq__(self, other):
         if isinstance(other, ModuleIfV7):
             return (
                 self.module_type == other.module_type and
                 self.msg_type == other.msg_type and
                 self.api_version == other.api_version and
@@ -1535,24 +1636,25 @@
                 self.board_type == other.board_type and
                 self.bl_version == other.bl_version and
                 self.major_ver == other.major_ver and
                 self.minor_ver == other.minor_ver and
                 self.patch_ver == other.patch_ver and
                 self.sup_cap_glob == other.sup_cap_glob and
                 self.sup_cap_datapath == other.sup_cap_datapath and
-                self.sup_cap_energy_2_4 == other.sup_cap_energy_2_4 and
-                self.sup_cap_sub1g_energy == other.sup_cap_sub1g_energy and
+                self.sup_cap_energy2400 == other.sup_cap_energy2400 and
+                self.sup_cap_energy_sub1g == other.sup_cap_energy_sub1g and
                 self.sup_cap_calibration == other.sup_cap_calibration and
-                self.sup_cap_power_mgmt == other.sup_cap_power_mgmt and
-                self.sup_cap_sensors == other.sup_cap_sensors
+                self.sup_cap_pwr_mgmt == other.sup_cap_pwr_mgmt and
+                self.sup_cap_sensors == other.sup_cap_sensors and
+                self.sup_cap_periph == other.sup_cap_periph
             )
         return False
 
     def dump(self):
-        string = bitstruct.pack("u4u4u8u8u48u8u8u8u8u8u1u1u1u1u1u1u1u1u72", self.module_type, self.msg_type, self.api_version, self.seq_id, self.brg_mac, self.board_type, self.bl_version, self.major_ver, self.minor_ver, self.patch_ver, self.sup_cap_glob, self.sup_cap_datapath, self.sup_cap_energy_2_4, self.sup_cap_sub1g_energy, self.sup_cap_calibration, self.sup_cap_power_mgmt, self.sup_cap_sensors, self.unused0, self.unused1)
+        string = bitstruct.pack("u4u4u8u8u48u8u8u8u8u8u1u1u1u1u1u1u1u1u72", self.module_type, self.msg_type, self.api_version, self.seq_id, self.brg_mac, self.board_type, self.bl_version, self.major_ver, self.minor_ver, self.patch_ver, self.sup_cap_glob, self.sup_cap_datapath, self.sup_cap_energy2400, self.sup_cap_energy_sub1g, self.sup_cap_calibration, self.sup_cap_pwr_mgmt, self.sup_cap_sensors, self.sup_cap_periph, self.unused0)
         return string.hex().upper()
 
     def set(self, string):
         d = bitstruct.unpack("u4u4u8u8u48u8u8u8u8u8u1u1u1u1u1u1u1u1u72", binascii.unhexlify(string))
         self.module_type = d[0]
         self.msg_type = d[1]
         self.api_version = d[2]
@@ -1561,68 +1663,113 @@
         self.board_type = d[5]
         self.bl_version = d[6]
         self.major_ver = d[7]
         self.minor_ver = d[8]
         self.patch_ver = d[9]
         self.sup_cap_glob = d[10]
         self.sup_cap_datapath = d[11]
-        self.sup_cap_energy_2_4 = d[12]
-        self.sup_cap_sub1g_energy = d[13]
+        self.sup_cap_energy2400 = d[12]
+        self.sup_cap_energy_sub1g = d[13]
         self.sup_cap_calibration = d[14]
-        self.sup_cap_power_mgmt = d[15]
+        self.sup_cap_pwr_mgmt = d[15]
         self.sup_cap_sensors = d[16]
-        self.unused0 = d[17]
-        self.unused1 = d[18]
+        self.sup_cap_periph = d[17]
+        self.unused0 = d[18]
 
 class ModuleEnergy2400V7():
-    def __init__(self, module_type=MODULE_ENERGY_2400, msg_type=0, api_version=7, seq_id=0, brg_mac=0, rxtx_period=0, tx_period=0, energy_pattern=0, output_power=0, unused0=0):
+    def __init__(self, module_type=MODULE_ENERGY_2400, msg_type=0, api_version=API_VERSION_V7, seq_id=0, brg_mac=0, rxtx_period=0, tx_period=0, energy_pattern=0, output_power=0, tx_probability=BRG_DEFAULT_TX_PROB, unused0=0, unused1=0):
         self.module_type = module_type
         self.msg_type = msg_type
         self.api_version = api_version
         self.seq_id = seq_id
         self.brg_mac = brg_mac
         self.rxtx_period = rxtx_period
         self.tx_period = tx_period
         self.energy_pattern = energy_pattern
         self.output_power = output_power
+        self.tx_probability = tx_probability
         self.unused0 = unused0
+        self.unused1 = unused1
 
     def __eq__(self, other):
         if isinstance(other, ModuleEnergy2400V7):
             return (
                 self.module_type == other.module_type and
                 self.msg_type == other.msg_type and
                 self.api_version == other.api_version and
                 self.brg_mac == other.brg_mac and
                 self.rxtx_period == other.rxtx_period and
                 self.tx_period == other.tx_period and
                 self.energy_pattern == other.energy_pattern and
-                self.output_power == other.output_power
+                self.output_power == other.output_power and
+                self.tx_probability == other.tx_probability
             )
         return False
 
     def dump(self):
-        string = bitstruct.pack("u4u4u8u8u48u8u8u8u8u88", self.module_type, self.msg_type, self.api_version, self.seq_id, self.brg_mac, self.rxtx_period, self.tx_period, self.energy_pattern, self.output_power, self.unused0)
+        string = bitstruct.pack("u4u4u8u8u48u8u8u8s8u3u5u80", self.module_type, self.msg_type, self.api_version, self.seq_id, self.brg_mac, self.rxtx_period, self.tx_period, self.energy_pattern, self.output_power, ((self.tx_probability-30)//10), self.unused0, self.unused1)
         return string.hex().upper()
 
     def set(self, string):
-        d = bitstruct.unpack("u4u4u8u8u48u8u8u8u8u88", binascii.unhexlify(string))
+        d = bitstruct.unpack("u4u4u8u8u48u8u8u8s8u3u5u80", binascii.unhexlify(string))
         self.module_type = d[0]
         self.msg_type = d[1]
         self.api_version = d[2]
         self.seq_id = d[3]
         self.brg_mac = d[4]
         self.rxtx_period = d[5]
         self.tx_period = d[6]
         self.energy_pattern = d[7]
         self.output_power = d[8]
-        self.unused0 = d[9]
+        self.tx_probability = ((d[9]*10)+30)
+        self.unused0 = d[10]
+        self.unused1 = d[11]
+
+MODULE_ENERGY_SUB1G_V7_OUTPUT_POWER_ENC = {SUB1G_OUTPUT_POWER_14:SUB1G_OUTPUT_POWER_PROFILE_14, SUB1G_OUTPUT_POWER_17:SUB1G_OUTPUT_POWER_PROFILE_17, SUB1G_OUTPUT_POWER_20:SUB1G_OUTPUT_POWER_PROFILE_20, SUB1G_OUTPUT_POWER_23:SUB1G_OUTPUT_POWER_PROFILE_23, SUB1G_OUTPUT_POWER_26:SUB1G_OUTPUT_POWER_PROFILE_26, SUB1G_OUTPUT_POWER_29:SUB1G_OUTPUT_POWER_PROFILE_29, SUB1G_OUTPUT_POWER_32:SUB1G_OUTPUT_POWER_PROFILE_32}
+MODULE_ENERGY_SUB1G_V7_OUTPUT_POWER_DEC = {SUB1G_OUTPUT_POWER_PROFILE_14:SUB1G_OUTPUT_POWER_14, SUB1G_OUTPUT_POWER_PROFILE_17:SUB1G_OUTPUT_POWER_17, SUB1G_OUTPUT_POWER_PROFILE_20:SUB1G_OUTPUT_POWER_20, SUB1G_OUTPUT_POWER_PROFILE_23:SUB1G_OUTPUT_POWER_23, SUB1G_OUTPUT_POWER_PROFILE_26:SUB1G_OUTPUT_POWER_26, SUB1G_OUTPUT_POWER_PROFILE_29:SUB1G_OUTPUT_POWER_29, SUB1G_OUTPUT_POWER_PROFILE_32:SUB1G_OUTPUT_POWER_32}
+class ModuleEnergySub1GV7():
+    def __init__(self, module_type=0, msg_type=0, api_version=API_VERSION_V7, seq_id=0, brg_mac=0, output_power=BRG_DEFAULT_OUTPUT_POWER_SUB_1_GHZ, freq_profile=SUB1G_FREQ_PROFILE_915000, unused0=0):
+        self.module_type = module_type
+        self.msg_type = msg_type
+        self.api_version = api_version
+        self.seq_id = seq_id
+        self.brg_mac = brg_mac
+        self.output_power = output_power
+        self.freq_profile = freq_profile
+        self.unused0 = unused0
+
+    def __eq__(self, other):
+        if isinstance(other, ModuleEnergySub1GV7):
+            return (
+                self.module_type == other.module_type and
+                self.msg_type == other.msg_type and
+                self.api_version == other.api_version and
+                self.brg_mac == other.brg_mac and
+                self.output_power == other.output_power and
+                self.freq_profile == other.freq_profile
+            )
+        return False
+
+    def dump(self):
+        string = bitstruct.pack("u4u4u8u8u48u8u8u104", self.module_type, self.msg_type, self.api_version, self.seq_id, self.brg_mac, MODULE_ENERGY_SUB1G_V7_OUTPUT_POWER_ENC[self.output_power], self.freq_profile, self.unused0)
+        return string.hex().upper()
+
+    def set(self, string):
+        d = bitstruct.unpack("u4u4u8u8u48u8u8u104", binascii.unhexlify(string))
+        self.module_type = d[0]
+        self.msg_type = d[1]
+        self.api_version = d[2]
+        self.seq_id = d[3]
+        self.brg_mac = d[4]
+        self.output_power = MODULE_ENERGY_SUB1G_V7_OUTPUT_POWER_DEC[d[5]]
+        self.freq_profile = d[6]
+        self.unused0 = d[7]
 
 class ModulePwrMgmtV7():
-    def __init__(self, module_type=MODULE_PWR_MGMT, msg_type=0, api_version=0, seq_id=0, brg_mac=0, static_leds_on=PWR_MGMT_DEFAULTS_LEDS_ON, static_keep_alive_period=PWR_MGMT_DEFAULTS_KEEP_ALIVE_PERIOD, static_keep_alive_scan=PWR_MGMT_DEFAULTS_KEEP_ALIVE_SCAN, static_on_duration=PWR_MGMT_DEFAULTS_ON_DURATION, static_sleep_duration=PWR_MGMT_DEFAULTS_SLEEP_DURATION, dynamic_leds_on=PWR_MGMT_DEFAULTS_LEDS_ON, dynamic_keep_alive_period=PWR_MGMT_DEFAULTS_KEEP_ALIVE_PERIOD, dynamic_keep_alive_scan=PWR_MGMT_DEFAULTS_KEEP_ALIVE_SCAN, dynamic_on_duration=PWR_MGMT_DEFAULTS_ON_DURATION, dynamic_sleep_duration=PWR_MGMT_DEFAULTS_SLEEP_DURATION, unused0=0):
+    def __init__(self, module_type=MODULE_PWR_MGMT, msg_type=0, api_version=API_VERSION_V7, seq_id=0, brg_mac=0, static_leds_on=PWR_MGMT_DEFAULTS_LEDS_ON, static_keep_alive_period=PWR_MGMT_DEFAULTS_KEEP_ALIVE_PERIOD, static_keep_alive_scan=PWR_MGMT_DEFAULTS_KEEP_ALIVE_SCAN, static_on_duration=PWR_MGMT_DEFAULTS_ON_DURATION, static_sleep_duration=PWR_MGMT_DEFAULTS_SLEEP_DURATION, dynamic_leds_on=PWR_MGMT_DEFAULTS_LEDS_ON, dynamic_keep_alive_period=PWR_MGMT_DEFAULTS_KEEP_ALIVE_PERIOD, dynamic_keep_alive_scan=PWR_MGMT_DEFAULTS_KEEP_ALIVE_SCAN, dynamic_on_duration=PWR_MGMT_DEFAULTS_ON_DURATION, dynamic_sleep_duration=PWR_MGMT_DEFAULTS_SLEEP_DURATION, unused0=0):
         self.module_type = module_type
         self.msg_type = msg_type
         self.api_version = api_version
         self.seq_id = seq_id
         self.brg_mac = brg_mac
         self.static_leds_on = static_leds_on
         self.static_keep_alive_period = static_keep_alive_period # 5sec resolution
@@ -1675,7 +1822,147 @@
         self.dynamic_leds_on = d[10]
         self.dynamic_keep_alive_period = ((d[11]*5)+0)
         self.dynamic_keep_alive_scan = ((d[12]*10)+0)
         self.dynamic_on_duration = ((d[13]*30)+0)
         self.dynamic_sleep_duration = ((d[14]*60)+0)
         self.unused0 = d[15]
 
+class ModuleCalibrationV7():
+    def __init__(self, module_type=MODULE_CALIBRATION, msg_type=0, api_version=0, seq_id=0, brg_mac=0, unused0=0):
+        self.module_type = module_type
+        self.msg_type = msg_type
+        self.api_version = api_version
+        self.seq_id = seq_id
+        self.brg_mac = brg_mac
+        self.unused0 = unused0
+
+    def __eq__(self, other):
+        if isinstance(other, ModuleCalibrationV7):
+            return (
+                self.module_type == other.module_type and
+                self.msg_type == other.msg_type and
+                self.api_version == other.api_version and
+                self.brg_mac == other.brg_mac
+            )
+        return False
+
+    def dump(self):
+        string = bitstruct.pack("u4u4u8u8u48u120", self.module_type, self.msg_type, self.api_version, self.seq_id, self.brg_mac, self.unused0)
+        return string.hex().upper()
+
+    def set(self, string):
+        d = bitstruct.unpack("u4u4u8u8u48u120", binascii.unhexlify(string))
+        self.module_type = d[0]
+        self.msg_type = d[1]
+        self.api_version = d[2]
+        self.seq_id = d[3]
+        self.brg_mac = d[4]
+        self.unused0 = d[5]
+
+class ModuleDatapathV7():
+    def __init__(self, module_type=MODULE_DATAPATH, msg_type=0, api_version=0, seq_id=0, brg_mac=0, global_pacing_group=BRG_DEFAULT_GLOBAL_PACING_GROUP, unused0=0, pacer_interval=BRG_DEFAULT_PACER_INTERVAL, pkt_types_mask=BRG_DEFAULT_PKT_TYPES_MASK, tx_repetition=BRG_DEFAULT_TX_REPETITION, unused1=0):
+        self.module_type = module_type
+        self.msg_type = msg_type
+        self.api_version = api_version
+        self.seq_id = seq_id
+        self.brg_mac = brg_mac
+        self.global_pacing_group = global_pacing_group
+        self.unused0 = unused0
+        self.pacer_interval = pacer_interval
+        self.pkt_types_mask = pkt_types_mask
+        self.tx_repetition = tx_repetition
+        self.unused1 = unused1
+
+    def __eq__(self, other):
+        if isinstance(other, ModuleDatapathV7):
+            return (
+                self.module_type == other.module_type and
+                self.msg_type == other.msg_type and
+                self.api_version == other.api_version and
+                self.brg_mac == other.brg_mac and
+                self.global_pacing_group == other.global_pacing_group and
+                self.pacer_interval == other.pacer_interval and
+                self.pkt_types_mask == other.pkt_types_mask and
+                self.tx_repetition == other.tx_repetition
+            )
+        return False
+
+    def dump(self):
+        string = bitstruct.pack("u4u4u8u8u48u4u4u16u5u3u88", self.module_type, self.msg_type, self.api_version, self.seq_id, self.brg_mac, self.global_pacing_group, self.unused0, self.pacer_interval, self.pkt_types_mask, self.tx_repetition, self.unused1)
+        return string.hex().upper()
+
+    def set(self, string):
+        d = bitstruct.unpack("u4u4u8u8u48u4u4u16u5u3u88", binascii.unhexlify(string))
+        self.module_type = d[0]
+        self.msg_type = d[1]
+        self.api_version = d[2]
+        self.seq_id = d[3]
+        self.brg_mac = d[4]
+        self.global_pacing_group = d[5]
+        self.unused0 = d[6]
+        self.pacer_interval = d[7]
+        self.pkt_types_mask = d[8]
+        self.tx_repetition = d[9]
+        self.unused1 = d[10]
+
+class ModulePeriphV7():
+    def __init__(self, module_type=MODULE_PERIPH, msg_type=0, api_version=API_VERSION_V7, seq_id=0, brg_mac=0, peripherals_tlv_params=0):
+        self.module_type = module_type
+        self.msg_type = msg_type
+        self.api_version = api_version
+        self.seq_id = seq_id
+        self.brg_mac = brg_mac
+        self.peripherals_tlv_params = peripherals_tlv_params
+
+    def __eq__(self, other):
+        if isinstance(other, ModulePeriphV7):
+            return (
+                self.module_type == other.module_type and
+                self.msg_type == other.msg_type and
+                self.api_version == other.api_version and
+                self.brg_mac == other.brg_mac and
+                self.peripherals_tlv_params == other.peripherals_tlv_params
+            )
+        return False
+
+    def dump(self):
+        string = bitstruct.pack("u4u4u8u8u48u120", self.module_type, self.msg_type, self.api_version, self.seq_id, self.brg_mac, self.peripherals_tlv_params)
+        return string.hex().upper()
+
+    def set(self, string):
+        d = bitstruct.unpack("u4u4u8u8u48u120", binascii.unhexlify(string))
+        self.module_type = d[0]
+        self.msg_type = d[1]
+        self.api_version = d[2]
+        self.seq_id = d[3]
+        self.brg_mac = d[4]
+        self.peripherals_tlv_params = d[5]
+
+class Lis2Dw12AccelData():
+    def __init__(self, api_version=0, state=0, temperature=0, unused0=0):
+        self.api_version = api_version
+        self.state = state
+        self.temperature = temperature
+        self.unused0 = unused0
+
+    def __eq__(self, other):
+        if isinstance(other, Lis2Dw12AccelData):
+            return (
+                self.api_version == other.api_version and
+                self.state == other.state and
+                self.temperature == other.temperature
+            )
+        return False
+
+    def dump(self):
+        string = bitstruct.pack("u8u8u16u184", self.api_version, self.state, self.temperature, self.unused0)
+        return string.hex().upper()
+
+    def set(self, string):
+        d = bitstruct.unpack("u8u8u16u184", binascii.unhexlify(string))
+        self.api_version = d[0]
+        self.state = d[1]
+        self.temperature = d[2]
+        self.unused0 = d[3]
+
+MODULES_LIST = [ModuleIfV7, ModuleEnergy2400V7, ModuleEnergySub1GV7, ModulePwrMgmtV7, ModuleCalibrationV7, ModuleDatapathV7, ModulePeriphV7]
+WLT_PKT_TYPES = [ActionV7, Gw2BrgCfgV7, Brg2GwCfgV7, Brg2GwCfgV6, Brg2GwCfgV5, Brg2GwCfgV2, Brg2GwHbV7, Brg2GwHbV6, Brg2GwHbV1, SideInfo, SideInfoSensor, ModuleIfV7, ModuleEnergy2400V7, ModuleEnergySub1GV7, ModulePwrMgmtV7, ModuleCalibrationV7, ModuleDatapathV7, ModulePeriphV7]
```

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/ag/wlt_types_data.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/ag/wlt_types_data.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/extended_api.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/api/extended_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/gw_ssid.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/api/gw_ssid.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/api/s3_client.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/api/s3_client.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/analysis_data_bricks.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/common/analysis_data_bricks.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/debug.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/common/debug.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/utils.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/common/utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/common/utils_defines.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/common/utils_defines.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer_cli.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/firmware_update/firmware_update.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/firmware_update/firmware_update.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/firmware_update/firmware_update_cli.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/firmware_update/firmware_update_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/gw_certificate.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/gw_certificate.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,8 +39,13 @@
         self.tests = [CouplingTest(**self.__dict__)]
     
     def run_tests(self):
         for test in self.tests:
             test.run()
 
 # TODO - send HB and CFG 
-# TODO - UnCoupled Mode
+# TODO - UnCoupled Mode
+
+
+# Downlink test
+# Sensor Packets
+# OTA Test
```

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/gw_certificate_cli.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/gw_certificate_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/ble_simulator.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/interface/ble_simulator.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/brg_array.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/interface/brg_array.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/mqtt.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/interface/mqtt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/packet_error.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/interface/packet_error.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/interface/pkt_generator.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/interface/pkt_generator.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/coupling.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/tests/coupling.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,15 +269,14 @@
 
 STAGES = [InitStage, OneBrgStage, ThreeBrgInitStage, ThreeBrgStage]
 # STAGES = [InitStage]
 
 class CouplingTest(GenericTest):
     def __init__(self, **kwargs):        
         self.__dict__.update(kwargs)
-        self.randomize = True
         super().__init__(**self.__dict__)
         self.stages = [stage(**self.__dict__) for stage in STAGES]
 
     def enter_dev_mode(self):
         gw_type = self.edge.get_gateway_type(self.gw_id)
         if gw_type == GatewayType.MOBILE:
             debug_print('Android DevMode needs to be enabled manually! Choose HIVE env')
```

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/generated_packet_table.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/tests/generated_packet_table.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/generic.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/tests/generic.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/gw_certificate/tests/packet_table.csv` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/gw_certificate/tests/packet_table.csv`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/interface/uart_ports.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/interface/uart_ports.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/log_viewer/log_viewer_cli.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/log_viewer/log_viewer_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/power_mgmt.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/power_mgmt/power_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools/utils/get_version.py` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/PKG-INFO` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.1.3
+Version: 4.1.4
 Summary: A library for interacting with Wiliot's Deployment Tools
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -201,14 +201,17 @@
 - Init Stage - Send 4 packet pairs (Data+SI) from 1 BRG, testing maximum/minimum RSSI and NFPKT Values encoded in SI packet
 - One Bridge Stage - Send packet pairs at increasing duplication (1->10) and increasing time delay between packets (15->255 ms) from 1 bridge, including simulated packet error.
 - Three Bridge Init Stage - send same data packet from 3 different bridges, each with different SI.
 - Three Bridge Stage - send same data packet from 3 different bridges, at increasing duplication (1->10) and increasing time delay between packets for each bridge (30->255).
 The test logs all sent packets, and all received packets from the tested GW in log files and outputs a summary of all sent packets in a CSV file (filepath specified at runtime).
 
 #### GW Certificate Release Notes:
+Version 4.1.4: 
+* Randomize bugfix
+
 Version 4.1.3:
 * Bugfixes
 * Support for Android
 * Support for python 3.11
 
 Version 4.1.0:
 * Coupling Test
@@ -232,17 +235,14 @@
 required arguments:
   -owner OWNER  Owner ID
   -gw GW        Gateway ID
   ```
 
 
 ## Release Notes:
-Version 4.1.3:
-* GW Certificate Bugfixes
-
 Version 4.1.1:
 * Bridge-Gw connectivity log print
 
 Version 4.1.0:
 * Custom message support
 * GW Certificate - coupling test
 * Fixes for calibration management
```

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/SOURCES.txt` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.3/wiliot_deployment_tools.egg-info/entry_points.txt` & `wiliot-deployment-tools-4.1.4/wiliot_deployment_tools.egg-info/entry_points.txt`

 * *Files identical despite different names*

