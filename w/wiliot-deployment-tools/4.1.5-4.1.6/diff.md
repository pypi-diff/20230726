# Comparing `tmp/wiliot-deployment-tools-4.1.5.tar.gz` & `tmp/wiliot-deployment-tools-4.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-deployment-tools-4.1.5.tar", last modified: Wed Jul 26 15:56:01 2023, max compression
+gzip compressed data, was "wiliot-deployment-tools-4.1.6.tar", last modified: Wed Jul 26 17:31:53 2023, max compression
```

## Comparing `wiliot-deployment-tools-4.1.5.tar` & `wiliot-deployment-tools-4.1.6.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.272229 wiliot-deployment-tools-4.1.5/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.232228 wiliot-deployment-tools-4.1.5/.deploy/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.232228 wiliot-deployment-tools-4.1.5/.deploy/aws/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.244228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/common.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.244228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/account.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.244228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.244228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.244228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.232228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.244228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/
--rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh
--rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/terragrunt.hcl
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/dbc.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.244228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.232228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.244228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/
--rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/install_packages.sh
--rw-rw-rw-   0 root         (0) root         (0)     4550 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/terragrunt.hcl
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/region.hcl
--rw-rw-rw-   0 root         (0) root         (0)     1290 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/terragrunt.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.244228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/test/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/test/account.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.244228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/test/us-east-2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.244228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/test/us-east-2/dbc/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.244228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.236228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.244228 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/
--rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh
--rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/terragrunt.hcl
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/test/us-east-2/dbc/dbc.hcl
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/test/us-east-2/region.hcl
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.236228 wiliot-deployment-tools-4.1.5/.devcontainer/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.248228 wiliot-deployment-tools-4.1.5/.devcontainer/private/
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.devcontainer/private/devcontainer.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.248228 wiliot-deployment-tools-4.1.5/.devcontainer/public/
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.devcontainer/public/devcontainer.json
--rw-rw-rw-   0 root         (0) root         (0)      455 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.gitignore
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.248228 wiliot-deployment-tools-4.1.5/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      687 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/Makefile
--rw-rw-rw-   0 root         (0) root         (0)    11677 2023-07-26 15:56:01.272229 wiliot-deployment-tools-4.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11159 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)    13775 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.248228 wiliot-deployment-tools-4.1.5/ci/
--rwxrwxrwx   0 root         (0) root         (0)     1696 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/ci/upload_to_s3.sh
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/ci.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/dep-tools-public.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      519 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/dep-tools.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)    14810 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/gw_certificate.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-26 15:56:01.272229 wiliot-deployment-tools-4.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3635 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.248228 wiliot-deployment-tools-4.1.5/unittests/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/unittests/test_debug_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/unittests/test_extended_api_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/unittests/test_extended_api_platform.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/unittests/test_power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2710 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/unittests/test_slack_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/unittests/test_test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     2252 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/unittests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.248228 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.256228 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/ag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/ag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13204 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/ag/ut_defines.py
--rw-rw-rw-   0 root         (0) root         (0)     4492 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/ag/wlt_types.py
--rw-rw-rw-   0 root         (0) root         (0)    92198 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/ag/wlt_types_ag.py
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/ag/wlt_types_data.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/ag/wlt_types_imports.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.256228 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    50280 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/api/extended_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1187 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/api/gw_ssid.py
--rw-rw-rw-   0 root         (0) root         (0)     1139 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/api/s3_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.256228 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/automatic_configuration_tool/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15430 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     3178 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.256228 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/calibration_mgmt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/calibration_mgmt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13553 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.260228 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    68659 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/common/analysis_data_bricks.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/common/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     6004 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/common/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3135 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/common/utils_defines.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.260228 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/connectivity_analyzer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/connectivity_analyzer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14407 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer.py
--rw-rw-rw-   0 root         (0) root         (0)     3084 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.264229 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/firmware_update/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/firmware_update/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22977 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/firmware_update/firmware_update.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.264229 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2177 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/gw_certificate.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/gw_certificate_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.264229 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/interface/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/interface/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6770 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/interface/ble_simulator.py
--rw-rw-rw-   0 root         (0) root         (0)     1554 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/interface/brg_array.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/interface/if_defines.py
--rw-rw-rw-   0 root         (0) root         (0)     7896 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/interface/mqtt.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/interface/packet_error.py
--rw-rw-rw-   0 root         (0) root         (0)     3381 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/interface/pkt_generator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.268229 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/tests/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15356 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/tests/coupling.py
--rw-rw-rw-   0 root         (0) root         (0)     3665 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/tests/generated_packet_table.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/tests/generic.py
--rw-rw-rw-   0 root         (0) root         (0)   190851 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/tests/packet_table.csv
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.268229 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/interface/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/interface/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/interface/uart_ports.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.268229 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/log_viewer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/log_viewer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2541 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.272229 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/power_mgmt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/power_mgmt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4653 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
--rw-rw-rw-   0 root         (0) root         (0)    26335 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/power_mgmt/power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     4801 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.272229 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2023-07-26 15:55:44.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-26 15:56:00.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 15:56:01.252228 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    11677 2023-07-26 15:56:01.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4727 2023-07-26 15:56:01.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 15:56:01.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      725 2023-07-26 15:56:01.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 15:56:01.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-26 15:56:01.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-26 15:56:01.000000 wiliot-deployment-tools-4.1.5/wiliot_deployment_tools.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.910108 wiliot-deployment-tools-4.1.6/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.894108 wiliot-deployment-tools-4.1.6/.deploy/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.894108 wiliot-deployment-tools-4.1.6/.deploy/aws/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.898108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/common.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.898108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/account.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.898108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.898108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.898108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.894108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.898108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/
+-rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/terragrunt.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/dbc.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.898108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.894108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.898108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/
+-rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/install_packages.sh
+-rw-rw-rw-   0 root         (0) root         (0)     4550 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/terragrunt.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/region.hcl
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/terragrunt.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.898108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/test/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/test/account.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.902108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/test/us-east-2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.902108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/test/us-east-2/dbc/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.902108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.894108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.902108 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/
+-rwxrwxrwx   0 root         (0) root         (0)      927 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/terragrunt.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/test/us-east-2/dbc/dbc.hcl
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/test/us-east-2/region.hcl
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.894108 wiliot-deployment-tools-4.1.6/.devcontainer/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.902108 wiliot-deployment-tools-4.1.6/.devcontainer/private/
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.devcontainer/private/devcontainer.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.902108 wiliot-deployment-tools-4.1.6/.devcontainer/public/
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.devcontainer/public/devcontainer.json
+-rw-rw-rw-   0 root         (0) root         (0)      455 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.gitignore
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.902108 wiliot-deployment-tools-4.1.6/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)    11677 2023-07-26 17:31:53.910108 wiliot-deployment-tools-4.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11159 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    13775 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.902108 wiliot-deployment-tools-4.1.6/ci/
+-rwxrwxrwx   0 root         (0) root         (0)     1696 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/ci/upload_to_s3.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/dep-tools-public.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      519 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/dep-tools.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    14810 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/gw_certificate.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-26 17:31:53.910108 wiliot-deployment-tools-4.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.902108 wiliot-deployment-tools-4.1.6/unittests/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/unittests/test_debug_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/unittests/test_extended_api_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/unittests/test_extended_api_platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/unittests/test_power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/unittests/test_slack_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/unittests/test_test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2252 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/unittests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.902108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.906108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/ag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/ag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13204 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/ag/ut_defines.py
+-rw-rw-rw-   0 root         (0) root         (0)     4492 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/ag/wlt_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    92198 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/ag/wlt_types_ag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/ag/wlt_types_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/ag/wlt_types_imports.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.906108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    50280 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/api/extended_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/api/gw_ssid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/api/s3_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.906108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/automatic_configuration_tool/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15430 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.906108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/calibration_mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/calibration_mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13553 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.906108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    68659 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/common/analysis_data_bricks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/common/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     6004 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/common/utils_defines.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.906108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/connectivity_analyzer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/connectivity_analyzer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14407 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3084 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.906108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/firmware_update/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/firmware_update/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22977 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/firmware_update/firmware_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.906108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2177 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/gw_certificate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/gw_certificate_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.910108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/interface/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/interface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6770 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/interface/ble_simulator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/interface/brg_array.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/interface/if_defines.py
+-rw-rw-rw-   0 root         (0) root         (0)     7896 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/interface/mqtt.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/interface/packet_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     3381 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/interface/pkt_generator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.910108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15476 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/tests/coupling.py
+-rw-rw-rw-   0 root         (0) root         (0)     3665 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/tests/generated_packet_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/tests/generic.py
+-rw-rw-rw-   0 root         (0) root         (0)   190851 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/tests/packet_table.csv
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.910108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/interface/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/interface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/interface/uart_ports.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.910108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/log_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/log_viewer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.910108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/power_mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/power_mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
+-rw-rw-rw-   0 root         (0) root         (0)    26335 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/power_mgmt/power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     4801 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.910108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6057 2023-07-26 17:31:35.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-26 17:31:53.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 17:31:53.902108 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    11677 2023-07-26 17:31:53.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4727 2023-07-26 17:31:53.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 17:31:53.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      725 2023-07-26 17:31:53.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-26 17:31:53.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-26 17:31:53.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-26 17:31:53.000000 wiliot-deployment-tools-4.1.6/wiliot_deployment_tools.egg-info/top_level.txt
```

### Comparing `wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/common.hcl` & `wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/common.hcl`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh` & `wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/terragrunt.hcl` & `wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/clusters/terragrunt.hcl`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/install_packages.sh` & `wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/init-scripts/system-network/install_packages.sh`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/terragrunt.hcl` & `wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/prod/us-east-2/dbc/job-clusters/terragrunt.hcl`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/terragrunt.hcl` & `wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/terragrunt.hcl`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh` & `wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/init-scripts/system-network/install_packages.sh`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/terragrunt.hcl` & `wiliot-deployment-tools-4.1.6/.deploy/aws/infrastructure/test/us-east-2/dbc/clusters/terragrunt.hcl`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/.devcontainer/private/devcontainer.json` & `wiliot-deployment-tools-4.1.6/.devcontainer/private/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/.devcontainer/public/devcontainer.json` & `wiliot-deployment-tools-4.1.6/.devcontainer/public/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/LICENSE` & `wiliot-deployment-tools-4.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/Makefile` & `wiliot-deployment-tools-4.1.6/Makefile`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/PKG-INFO` & `wiliot-deployment-tools-4.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.1.5
+Version: 4.1.6
 Summary: A library for interacting with Wiliot's Deployment Tools
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
```

### Comparing `wiliot-deployment-tools-4.1.5/README.md` & `wiliot-deployment-tools-4.1.6/README.md`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/bitbucket-pipelines.yml` & `wiliot-deployment-tools-4.1.6/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/ci/upload_to_s3.sh` & `wiliot-deployment-tools-4.1.6/ci/upload_to_s3.sh`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/ci.py` & `wiliot-deployment-tools-4.1.6/ci.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/dep-tools.dockerfile` & `wiliot-deployment-tools-4.1.6/dep-tools.dockerfile`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/gw_certificate.ipynb` & `wiliot-deployment-tools-4.1.6/gw_certificate.ipynb`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/setup.py` & `wiliot-deployment-tools-4.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/unittests/test_extended_api_edge.py` & `wiliot-deployment-tools-4.1.6/unittests/test_extended_api_edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/unittests/test_extended_api_platform.py` & `wiliot-deployment-tools-4.1.6/unittests/test_extended_api_platform.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/unittests/test_power_mgmt.py` & `wiliot-deployment-tools-4.1.6/unittests/test_power_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/unittests/test_slack_alerts.py` & `wiliot-deployment-tools-4.1.6/unittests/test_slack_alerts.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/unittests/test_test_tool.py` & `wiliot-deployment-tools-4.1.6/unittests/test_test_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/unittests/test_utils.py` & `wiliot-deployment-tools-4.1.6/unittests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/ag/ut_defines.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/ag/ut_defines.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/ag/wlt_types.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/ag/wlt_types.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/ag/wlt_types_ag.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/ag/wlt_types_ag.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/ag/wlt_types_data.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/ag/wlt_types_data.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/api/extended_api.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/api/extended_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/api/gw_ssid.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/api/gw_ssid.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/api/s3_client.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/api/s3_client.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/common/analysis_data_bricks.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/common/analysis_data_bricks.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/common/debug.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/common/debug.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/common/utils.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/common/utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/common/utils_defines.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/common/utils_defines.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer_cli.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/connectivity_analyzer/connectivity_analyzer_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/firmware_update/firmware_update.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/firmware_update/firmware_update.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/firmware_update/firmware_update_cli.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/firmware_update/firmware_update_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/gw_certificate.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/gw_certificate.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/gw_certificate_cli.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/gw_certificate_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/interface/ble_simulator.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/interface/ble_simulator.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/interface/brg_array.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/interface/brg_array.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/interface/mqtt.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/interface/mqtt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/interface/packet_error.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/interface/packet_error.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/interface/pkt_generator.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/interface/pkt_generator.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/tests/coupling.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/tests/coupling.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,17 @@
         self.mqttc.flash_pkts()
         self.ble_sim.set_sim_mode(True)
         
     def fetch_mqtt_from_stage(self):
         def process_payload(packet:dict):
             payload = packet[PAYLOAD]
             payload = payload.upper()
+            if len(payload) == 62:
+                if payload[:4] == '1E16':
+                    payload = payload [4:]
             # big2little endian
             if payload[:4] == 'FCC6':
                 payload = 'C6FC' + payload[4:]
             packet[PAYLOAD] = payload
             return packet
         mqtt_pkts = self.mqttc.get_coupled_tags_pkts()
         self.mqtt_pkts = list(map(lambda p: process_payload(p), mqtt_pkts))
```

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/tests/generated_packet_table.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/tests/generated_packet_table.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/tests/generic.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/tests/generic.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/gw_certificate/tests/packet_table.csv` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/gw_certificate/tests/packet_table.csv`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/interface/uart_ports.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/interface/uart_ports.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/log_viewer/log_viewer_cli.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/log_viewer/log_viewer_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/power_mgmt/power_mgmt.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/power_mgmt/power_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools/utils/get_version.py` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools.egg-info/PKG-INFO` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.1.5
+Version: 4.1.6
 Summary: A library for interacting with Wiliot's Deployment Tools
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
```

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools.egg-info/SOURCES.txt` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.1.5/wiliot_deployment_tools.egg-info/entry_points.txt` & `wiliot-deployment-tools-4.1.6/wiliot_deployment_tools.egg-info/entry_points.txt`

 * *Files identical despite different names*

