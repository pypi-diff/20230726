# Comparing `tmp/cloudshell-cp-aws-3.4.0.zip` & `tmp/cloudshell-cp-aws-3.5.0.zip`

## zipinfo {}

```diff
@@ -1,199 +1,208 @@
-Zip file size: 160698 bytes, number of entries: 197
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell_cp_aws.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/
--rw-r--r--  2.0 unx      633 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/PKG-INFO
--rw-r--r--  2.0 unx     1019 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tox.ini
--rw-r--r--  2.0 unx     1478 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/setup.py
--rw-r--r--  2.0 unx       98 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/dev_requirements.txt
--rw-r--r--  2.0 unx       38 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/setup.cfg
--rw-r--r--  2.0 unx      579 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/README.md
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/version.txt
--rw-r--r--  2.0 unx       46 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/MANIFEST.in
--rw-r--r--  2.0 unx      232 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/requirements.txt
--rw-r--r--  2.0 unx       43 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/test_requirements.txt
--rw-r--r--  2.0 unx      232 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell_cp_aws.egg-info/requires.txt
--rw-r--r--  2.0 unx      633 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell_cp_aws.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell_cp_aws.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell_cp_aws.egg-info/top_level.txt
--rw-r--r--  2.0 unx     7960 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell_cp_aws.egg-info/SOURCES.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/__init__.py
--rw-r--r--  2.0 unx    31568 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/aws_shell.py
--rw-r--r--  2.0 unx     4101 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/deploy_aws_ec2_ami_instance_resource_model.py
--rw-r--r--  2.0 unx      639 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/port_data.py
--rw-r--r--  2.0 unx      135 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/ami_credentials.py
--rw-r--r--  2.0 unx     1220 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/traffic_mirror_fulfillment.py
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/__init__.py
--rw-r--r--  2.0 unx      159 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/vm_details.py
--rw-r--r--  2.0 unx     1193 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/aws_api.py
--rw-r--r--  2.0 unx      857 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/network_actions_models.py
--rw-r--r--  2.0 unx      707 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/ami_deployment_model.py
--rw-r--r--  2.0 unx     4143 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/aws_ec2_cloud_provider_resource_model.py
--rw-r--r--  2.0 unx      550 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/app_security_groups_model.py
--rw-r--r--  2.0 unx      401 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/reservation_model.py
--rw-r--r--  2.0 unx       43 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/exceptions.py
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/__init__.py
--rw-r--r--  2.0 unx      353 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/retry_helper.py
--rw-r--r--  2.0 unx      458 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/cached_property.py
--rw-r--r--  2.0 unx      940 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/converters.py
--rw-r--r--  2.0 unx     1920 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/deploy_data_holder.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/context/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/operations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/__init__.py
--rw-r--r--  2.0 unx      683 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/context/aws_resource_model.py
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/context/__init__.py
--rw-r--r--  2.0 unx     1308 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/context/aws_api.py
--rw-r--r--  2.0 unx     2770 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/context/aws_shell.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/__init__.py
--rw-r--r--  2.0 unx     3380 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/delete_operation.py
--rw-r--r--  2.0 unx     2308 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/refresh_ip_operation.py
--rw-r--r--  2.0 unx    37924 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/deploy_operation.py
--rw-r--r--  2.0 unx     6840 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/snapshot_operation.py
--rw-r--r--  2.0 unx     1287 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/power_operation.py
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/__init__.py
--rw-r--r--  2.0 unx      825 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/access_key_operation.py
--rw-r--r--  2.0 unx     1007 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/cancellation_service.py
--rw-r--r--  2.0 unx      100 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/list_helper.py
--rw-r--r--  2.0 unx      303 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/exceptions.py
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/__init__.py
--rw-r--r--  2.0 unx      681 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/aws_session_manager.py
--rw-r--r--  2.0 unx      891 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/CheckCancellationThread.py
--rw-r--r--  2.0 unx     5032 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/vm_details_provider.py
--rw-r--r--  2.0 unx     3784 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/operations/autoload_operation.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/operations/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/session_providers/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/s3/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/cloudshell/
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/__init__.py
--rw-r--r--  2.0 unx    15604 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/prepare_cloud_infra.py
--rw-r--r--  2.0 unx    15454 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/prepare_subnets.py
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/__init__.py
--rw-r--r--  2.0 unx     2800 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/device_index.py
--rw-r--r--  2.0 unx    11556 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/cleanup.py
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/session_providers/__init__.py
--rw-r--r--  2.0 unx     5341 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/session_providers/aws_session_provider.py
--rw-r--r--  2.0 unx     1000 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/security_group_parser.py
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/__init__.py
--rw-r--r--  2.0 unx     7225 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/aws_model_parser.py
--rw-r--r--  2.0 unx      577 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/command_results_parser.py
--rw-r--r--  2.0 unx     2569 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/port_group_attribute_parser.py
--rw-r--r--  2.0 unx      692 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/custom_param_extractor.py
--rw-r--r--  2.0 unx     2207 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/s3/bucket.py
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/s3/__init__.py
--rw-r--r--  2.0 unx     5841 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/instance.py
--rw-r--r--  2.0 unx     1121 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/vpc.py
--rw-r--r--  2.0 unx     1622 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/password.py
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/__init__.py
--rw-r--r--  2.0 unx     1361 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/subnet.py
--rw-r--r--  2.0 unx     1358 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/ami.py
--rw-r--r--  2.0 unx     3395 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/network_interface.py
--rw-r--r--  2.0 unx     5441 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/elastic_ip.py
--rw-r--r--  2.0 unx     4829 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/instance.py
--rw-r--r--  2.0 unx     1868 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/instance_credentials.py
--rw-r--r--  2.0 unx    12126 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/vpc.py
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/__init__.py
--rw-r--r--  2.0 unx      434 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/transit_gateway.py
--rw-r--r--  2.0 unx    11020 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/mirroring.py
--rw-r--r--  2.0 unx     1851 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/subnet.py
--rw-r--r--  2.0 unx      818 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/ebs.py
--rw-r--r--  2.0 unx    14324 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/security_group.py
--rw-r--r--  2.0 unx     2635 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/keypair.py
--rw-r--r--  2.0 unx     3990 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/cloudshell/traffic_mirror_pool_services.py
--rw-r--r--  2.0 unx     2515 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/cloudshell/cs_subnet_service.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/__init__.py
--rw-r--r--  2.0 unx    11536 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/traffic_mirror_cleaner.py
--rw-r--r--  2.0 unx    20540 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/traffic_mirroring_operation.py
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/__init__.py
--rw-r--r--  2.0 unx     1591 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/cleanup.py
--rw-r--r--  2.0 unx     7951 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/prepare.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/operations/
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/__init__.py
--rw-r--r--  2.0 unx      553 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/operations/vm_details_operation.py
--rw-r--r--  2.0 unx     4965 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/operations/set_app_security_groups.py
--rw-r--r--  2.0 unx     7348 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/operations/app_ports_operation.py
--rw-r--r--  2.0 unx       97 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/operations/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/__init__.py
--rw-r--r--  2.0 unx     8753 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/route_table_handler.py
--rw-r--r--  2.0 unx     3783 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/cidr_block_handler.py
--rw-r--r--  2.0 unx     4324 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/tags_handler.py
--rw-r--r--  2.0 unx     1225 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/route_handler.py
--rw-r--r--  2.0 unx      432 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/__init__.py
--rw-r--r--  2.0 unx     6426 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/vpc_peering_handler.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_connectivity/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_ami_management/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_deployed_app/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_common/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/handlers/
--rw-r--r--  2.0 unx      732 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/conftest.py
--rw-r--r--  2.0 unx    12996 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_aws_shell.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/__init__.py
--rw-r--r--  2.0 unx     1033 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/base.py
--rw-r--r--  2.0 unx     8746 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_connectivity/test_prepare_connectivity.py
--rw-r--r--  2.0 unx     2734 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_connectivity/test_cleanup_connectivity.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_connectivity/__init__.py
--rw-r--r--  2.0 unx     6299 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_connectivity/test_create_traffic_mirroring.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_ami_management/__init__.py
--rw-r--r--  2.0 unx     2443 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/test_power_operation.py
--rw-r--r--  2.0 unx    31795 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/test_deploy_operation.py
--rw-r--r--  2.0 unx     3225 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/test_delete_operation.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/__init__.py
--rw-r--r--  2.0 unx     3235 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/test_refresh_ip_operation.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_deployed_app/test_operations/
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_deployed_app/__init__.py
--rw-r--r--  2.0 unx     1206 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_deployed_app/test_operations/test_access_key_operation.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_deployed_app/test_operations/__init__.py
--rw-r--r--  2.0 unx     3423 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_deployed_app/test_operations/test_set_app_security_groups_operation.py
--rw-r--r--  2.0 unx     4591 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_deployed_app/test_operations/test_app_ports_operation.py
--rw-r--r--  2.0 unx     2960 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_key_pair.py
--rw-r--r--  2.0 unx     7632 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_vpc.py
--rw-r--r--  2.0 unx     9626 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_elastic_ip.py
--rw-r--r--  2.0 unx      727 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_vm_custom_params_extractor.py
--rw-r--r--  2.0 unx      997 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_port_group_attribute_parser.py
--rw-r--r--  2.0 unx     3090 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_network_interface_service.py
--rw-r--r--  2.0 unx     1182 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_session_provider.py
--rw-r--r--  2.0 unx     2897 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_subnet.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/__init__.py
--rw-r--r--  2.0 unx      770 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_ami_waiter.py
--rw-r--r--  2.0 unx    15674 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_model_parser.py
--rw-r--r--  2.0 unx     7070 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_security_groups.py
--rw-r--r--  2.0 unx     6697 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_instance_waiter.py
--rw-r--r--  2.0 unx     3385 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_ami_creds_service.py
--rw-r--r--  2.0 unx     4162 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_device_index_strategy.py
--rw-r--r--  2.0 unx      767 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_vpc_waiter.py
--rw-r--r--  2.0 unx     4571 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_instance_service.py
--rw-r--r--  2.0 unx      794 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_subnet_waiter.py
--rw-r--r--  2.0 unx     2844 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_bucket.py
--rw-r--r--  2.0 unx     1134 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_password_waiter.py
--rw-r--r--  2.0 unx     1197 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_common/test_cancellation_service.py
--rw-r--r--  2.0 unx     2935 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_common/test_get_vm_details.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_common/__init__.py
--rw-r--r--  2.0 unx     1220 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_common/test_converters.py
--rw-r--r--  2.0 unx     5050 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_common/test_vm_details_provider.py
--rw-r--r--  2.0 unx      482 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/test_common/test_retry_helper.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/handlers/__init__.py
--rw-r--r--  2.0 unx     1958 b- defN 23-Apr-06 09:33 cloudshell-cp-aws-3.4.0/tests/handlers/test_route_table_handler.py
-197 files, 526779 bytes uncompressed, 118334 bytes compressed:  77.5%
+Zip file size: 172223 bytes, number of entries: 206
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell_cp_aws.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/
+-rw-r--r--  2.0 unx      232 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/requirements.txt
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/setup.cfg
+-rw-r--r--  2.0 unx       98 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/dev_requirements.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/version.txt
+-rw-r--r--  2.0 unx      633 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/PKG-INFO
+-rw-r--r--  2.0 unx       43 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/test_requirements.txt
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/MANIFEST.in
+-rw-r--r--  2.0 unx      579 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/README.md
+-rw-r--r--  2.0 unx     1478 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/setup.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tox.ini
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_connectivity/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_deployed_app/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/handlers/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_ami_management/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_common/
+-rw-r--r--  2.0 unx      732 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/conftest.py
+-rw-r--r--  2.0 unx    12996 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_aws_shell.py
+-rw-r--r--  2.0 unx     1033 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/base.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/__init__.py
+-rw-r--r--  2.0 unx     6299 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_connectivity/test_create_traffic_mirroring.py
+-rw-r--r--  2.0 unx     2734 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_connectivity/test_cleanup_connectivity.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_connectivity/__init__.py
+-rw-r--r--  2.0 unx     8746 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_connectivity/test_prepare_connectivity.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_deployed_app/test_operations/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_deployed_app/__init__.py
+-rw-r--r--  2.0 unx     3423 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_deployed_app/test_operations/test_set_app_security_groups_operation.py
+-rw-r--r--  2.0 unx     4591 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_deployed_app/test_operations/test_app_ports_operation.py
+-rw-r--r--  2.0 unx     1206 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_deployed_app/test_operations/test_access_key_operation.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_deployed_app/test_operations/__init__.py
+-rw-r--r--  2.0 unx     1958 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/handlers/test_route_table_handler.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/handlers/__init__.py
+-rw-r--r--  2.0 unx     7070 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_security_groups.py
+-rw-r--r--  2.0 unx      997 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_port_group_attribute_parser.py
+-rw-r--r--  2.0 unx    15849 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_model_parser.py
+-rw-r--r--  2.0 unx     1182 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_session_provider.py
+-rw-r--r--  2.0 unx     2897 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_subnet.py
+-rw-r--r--  2.0 unx     7632 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_vpc.py
+-rw-r--r--  2.0 unx     3090 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_network_interface_service.py
+-rw-r--r--  2.0 unx      794 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_subnet_waiter.py
+-rw-r--r--  2.0 unx     9626 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_elastic_ip.py
+-rw-r--r--  2.0 unx     4162 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_device_index_strategy.py
+-rw-r--r--  2.0 unx     1134 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_password_waiter.py
+-rw-r--r--  2.0 unx      727 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_vm_custom_params_extractor.py
+-rw-r--r--  2.0 unx     6697 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_instance_waiter.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/__init__.py
+-rw-r--r--  2.0 unx      767 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_vpc_waiter.py
+-rw-r--r--  2.0 unx     2844 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_bucket.py
+-rw-r--r--  2.0 unx      770 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_ami_waiter.py
+-rw-r--r--  2.0 unx     2960 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_key_pair.py
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_instance_service.py
+-rw-r--r--  2.0 unx     3385 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_ami_creds_service.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_ami_management/__init__.py
+-rw-r--r--  2.0 unx     2443 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/test_power_operation.py
+-rw-r--r--  2.0 unx    31831 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/test_deploy_operation.py
+-rw-r--r--  2.0 unx     3235 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/test_refresh_ip_operation.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/__init__.py
+-rw-r--r--  2.0 unx     3225 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/test_delete_operation.py
+-rw-r--r--  2.0 unx     1220 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_common/test_converters.py
+-rw-r--r--  2.0 unx     5050 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_common/test_vm_details_provider.py
+-rw-r--r--  2.0 unx     1197 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_common/test_cancellation_service.py
+-rw-r--r--  2.0 unx      482 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_common/test_retry_helper.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_common/__init__.py
+-rw-r--r--  2.0 unx     2935 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/tests/test_common/test_get_vm_details.py
+-rw-r--r--  2.0 unx      633 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell_cp_aws.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       17 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell_cp_aws.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     8426 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell_cp_aws.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      232 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell_cp_aws.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell_cp_aws.egg-info/dependency_links.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/
+-rw-r--r--  2.0 unx    31604 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/aws_shell.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/__init__.py
+-rw-r--r--  2.0 unx      353 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/retry_helper.py
+-rw-r--r--  2.0 unx      940 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/converters.py
+-rw-r--r--  2.0 unx      376 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/subnet_service.py
+-rw-r--r--  2.0 unx     1920 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/deploy_data_holder.py
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/__init__.py
+-rw-r--r--  2.0 unx      458 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/cached_property.py
+-rw-r--r--  2.0 unx       43 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/exceptions.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/operations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/s3/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/session_providers/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/cloudshell/
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/__init__.py
+-rw-r--r--  2.0 unx     7225 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/aws_model_parser.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/security_group_parser.py
+-rw-r--r--  2.0 unx      577 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/command_results_parser.py
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/__init__.py
+-rw-r--r--  2.0 unx      692 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/custom_param_extractor.py
+-rw-r--r--  2.0 unx     2569 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/port_group_attribute_parser.py
+-rw-r--r--  2.0 unx     1361 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/subnet.py
+-rw-r--r--  2.0 unx     1358 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/ami.py
+-rw-r--r--  2.0 unx     5841 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/instance.py
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/vpc_peering.py
+-rw-r--r--  2.0 unx     1696 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/password.py
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/__init__.py
+-rw-r--r--  2.0 unx     1121 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/vpc.py
+-rw-r--r--  2.0 unx     1868 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/instance_credentials.py
+-rw-r--r--  2.0 unx     1851 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/subnet.py
+-rw-r--r--  2.0 unx     4309 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/tags.py
+-rw-r--r--  2.0 unx      818 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/ebs.py
+-rw-r--r--  2.0 unx     5441 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/elastic_ip.py
+-rw-r--r--  2.0 unx     4829 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/instance.py
+-rw-r--r--  2.0 unx    11020 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/mirroring.py
+-rw-r--r--  2.0 unx     3395 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/network_interface.py
+-rw-r--r--  2.0 unx      434 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/transit_gateway.py
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/__init__.py
+-rw-r--r--  2.0 unx    14324 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/security_group.py
+-rw-r--r--  2.0 unx     2635 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/keypair.py
+-rw-r--r--  2.0 unx    12126 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/vpc.py
+-rw-r--r--  2.0 unx     6308 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/route_table.py
+-rw-r--r--  2.0 unx     2800 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/device_index.py
+-rw-r--r--  2.0 unx    16544 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/prepare_subnets.py
+-rw-r--r--  2.0 unx    12438 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/cleanup.py
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/__init__.py
+-rw-r--r--  2.0 unx    16277 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/prepare_cloud_infra.py
+-rw-r--r--  2.0 unx     2207 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/s3/bucket.py
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/s3/__init__.py
+-rw-r--r--  2.0 unx     5610 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/session_providers/aws_session_provider.py
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/session_providers/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/cloudshell/__init__.py
+-rw-r--r--  2.0 unx     3990 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/cloudshell/traffic_mirror_pool_services.py
+-rw-r--r--  2.0 unx     2515 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/cloudshell/cs_subnet_service.py
+-rw-r--r--  2.0 unx     1007 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/cancellation_service.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/list_helper.py
+-rw-r--r--  2.0 unx      891 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/CheckCancellationThread.py
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/__init__.py
+-rw-r--r--  2.0 unx      303 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/exceptions.py
+-rw-r--r--  2.0 unx      681 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/aws_session_manager.py
+-rw-r--r--  2.0 unx     5032 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/vm_details_provider.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/operations/__init__.py
+-rw-r--r--  2.0 unx     3784 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/operations/autoload_operation.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/__init__.py
+-rw-r--r--  2.0 unx     3783 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/cidr_block_handler.py
+-rw-r--r--  2.0 unx     1225 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/route_handler.py
+-rw-r--r--  2.0 unx     4324 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/tags_handler.py
+-rw-r--r--  2.0 unx     6426 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/vpc_peering_handler.py
+-rw-r--r--  2.0 unx     8753 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/route_table_handler.py
+-rw-r--r--  2.0 unx      432 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/__init__.py
+-rw-r--r--  2.0 unx    39026 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/deploy_operation.py
+-rw-r--r--  2.0 unx     2308 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/refresh_ip_operation.py
+-rw-r--r--  2.0 unx      825 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/access_key_operation.py
+-rw-r--r--  2.0 unx     1287 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/power_operation.py
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/__init__.py
+-rw-r--r--  2.0 unx     3380 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/delete_operation.py
+-rw-r--r--  2.0 unx     6840 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/snapshot_operation.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/__init__.py
+-rw-r--r--  2.0 unx    13519 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/prepare_subnet_executor.py
+-rw-r--r--  2.0 unx    20540 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/traffic_mirroring_operation.py
+-rw-r--r--  2.0 unx     8550 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/prepare.py
+-rw-r--r--  2.0 unx     1591 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/cleanup.py
+-rw-r--r--  2.0 unx    11536 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/traffic_mirror_cleaner.py
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/operations/
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/__init__.py
+-rw-r--r--  2.0 unx      553 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/operations/vm_details_operation.py
+-rw-r--r--  2.0 unx     7348 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/operations/app_ports_operation.py
+-rw-r--r--  2.0 unx     4965 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/operations/set_app_security_groups.py
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/operations/__init__.py
+-rw-r--r--  2.0 unx     2770 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/aws_shell.py
+-rw-r--r--  2.0 unx      683 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/aws_resource_model.py
+-rw-r--r--  2.0 unx     1308 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/ec2_session.py
+-rw-r--r--  2.0 unx     1331 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/ec2_client.py
+-rw-r--r--  2.0 unx     1308 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/aws_api.py
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/__init__.py
+-rw-r--r--  2.0 unx     1304 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/s3_session.py
+-rw-r--r--  2.0 unx      415 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/client_error.py
+-rw-r--r--  2.0 unx      135 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/ami_credentials.py
+-rw-r--r--  2.0 unx     1220 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/traffic_mirror_fulfillment.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/vm_details.py
+-rw-r--r--  2.0 unx      707 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/ami_deployment_model.py
+-rw-r--r--  2.0 unx     4184 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/aws_ec2_cloud_provider_resource_model.py
+-rw-r--r--  2.0 unx     1193 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/aws_api.py
+-rw-r--r--  2.0 unx      550 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/app_security_groups_model.py
+-rw-r--r--  2.0 unx       97 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/__init__.py
+-rw-r--r--  2.0 unx      857 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/network_actions_models.py
+-rw-r--r--  2.0 unx     4184 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/deploy_aws_ec2_ami_instance_resource_model.py
+-rw-r--r--  2.0 unx      639 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/port_data.py
+-rw-r--r--  2.0 unx      401 b- defN 23-Jul-26 13:12 cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/reservation_model.py
+206 files, 563889 bytes uncompressed, 127829 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -1,592 +1,619 @@
-Filename: cloudshell-cp-aws-3.4.0/
+Filename: cloudshell-cp-aws-3.5.0/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell_cp_aws.egg-info/
+Filename: cloudshell-cp-aws-3.5.0/tests/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell_cp_aws.egg-info/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/PKG-INFO
+Filename: cloudshell-cp-aws-3.5.0/requirements.txt
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tox.ini
+Filename: cloudshell-cp-aws-3.5.0/setup.cfg
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/setup.py
+Filename: cloudshell-cp-aws-3.5.0/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/dev_requirements.txt
+Filename: cloudshell-cp-aws-3.5.0/version.txt
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/setup.cfg
+Filename: cloudshell-cp-aws-3.5.0/PKG-INFO
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/README.md
+Filename: cloudshell-cp-aws-3.5.0/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/version.txt
+Filename: cloudshell-cp-aws-3.5.0/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/MANIFEST.in
+Filename: cloudshell-cp-aws-3.5.0/README.md
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/requirements.txt
+Filename: cloudshell-cp-aws-3.5.0/setup.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/test_requirements.txt
+Filename: cloudshell-cp-aws-3.5.0/tox.ini
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell_cp_aws.egg-info/requires.txt
+Filename: cloudshell-cp-aws-3.5.0/tests/test_connectivity/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell_cp_aws.egg-info/PKG-INFO
+Filename: cloudshell-cp-aws-3.5.0/tests/test_deployed_app/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell_cp_aws.egg-info/dependency_links.txt
+Filename: cloudshell-cp-aws-3.5.0/tests/handlers/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell_cp_aws.egg-info/top_level.txt
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell_cp_aws.egg-info/SOURCES.txt
+Filename: cloudshell-cp-aws-3.5.0/tests/test_ami_management/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/
+Filename: cloudshell-cp-aws-3.5.0/tests/test_common/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/tests/conftest.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/
+Filename: cloudshell-cp-aws-3.5.0/tests/test_aws_shell.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/tests/base.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/
+Filename: cloudshell-cp-aws-3.5.0/tests/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/
+Filename: cloudshell-cp-aws-3.5.0/tests/test_connectivity/test_create_traffic_mirroring.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/
+Filename: cloudshell-cp-aws-3.5.0/tests/test_connectivity/test_cleanup_connectivity.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_connectivity/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/aws_shell.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_connectivity/test_prepare_connectivity.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/deploy_aws_ec2_ami_instance_resource_model.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_deployed_app/test_operations/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/port_data.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_deployed_app/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/ami_credentials.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_deployed_app/test_operations/test_set_app_security_groups_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/traffic_mirror_fulfillment.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_deployed_app/test_operations/test_app_ports_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_deployed_app/test_operations/test_access_key_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/vm_details.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_deployed_app/test_operations/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/aws_api.py
+Filename: cloudshell-cp-aws-3.5.0/tests/handlers/test_route_table_handler.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/network_actions_models.py
+Filename: cloudshell-cp-aws-3.5.0/tests/handlers/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/ami_deployment_model.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_security_groups.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/aws_ec2_cloud_provider_resource_model.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_port_group_attribute_parser.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/app_security_groups_model.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_model_parser.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/reservation_model.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_session_provider.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/exceptions.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_subnet.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_vpc.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/retry_helper.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_network_interface_service.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/cached_property.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_subnet_waiter.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/converters.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_elastic_ip.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/deploy_data_holder.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_device_index_strategy.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/context/
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_password_waiter.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_vm_custom_params_extractor.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_instance_waiter.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/operations/
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_vpc_waiter.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_bucket.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_ami_waiter.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_key_pair.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_instance_service.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/context/aws_resource_model.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_ami_creds_service.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/context/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/context/aws_api.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_ami_management/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/context/aws_shell.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/test_power_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/
+Filename: cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/test_deploy_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/test_refresh_ip_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/delete_operation.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/refresh_ip_operation.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/test_delete_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/deploy_operation.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_common/test_converters.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/snapshot_operation.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_common/test_vm_details_provider.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/power_operation.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_common/test_cancellation_service.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_common/test_retry_helper.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/access_key_operation.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_common/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/cancellation_service.py
+Filename: cloudshell-cp-aws-3.5.0/tests/test_common/test_get_vm_details.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/list_helper.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell_cp_aws.egg-info/PKG-INFO
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/exceptions.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell_cp_aws.egg-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell_cp_aws.egg-info/SOURCES.txt
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/aws_session_manager.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell_cp_aws.egg-info/requires.txt
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/CheckCancellationThread.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell_cp_aws.egg-info/dependency_links.txt
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/vm_details_provider.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/operations/autoload_operation.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/operations/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/session_providers/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/s3/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/aws_shell.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/cloudshell/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/retry_helper.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/converters.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/prepare_cloud_infra.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/subnet_service.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/prepare_subnets.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/deploy_data_holder.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/device_index.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/cached_property.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/cleanup.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/exceptions.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/session_providers/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/session_providers/aws_session_provider.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/security_group_parser.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/operations/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/aws_model_parser.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/command_results_parser.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/port_group_attribute_parser.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/custom_param_extractor.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/s3/bucket.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/s3/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/instance.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/vpc.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/password.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/s3/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/subnet.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/session_providers/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/ami.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/cloudshell/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/network_interface.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/elastic_ip.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/aws_model_parser.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/instance.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/security_group_parser.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/instance_credentials.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/command_results_parser.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/vpc.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/custom_param_extractor.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/transit_gateway.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/port_group_attribute_parser.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/mirroring.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/subnet.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/subnet.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/ami.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/ebs.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/instance.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/security_group.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/vpc_peering.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/keypair.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/password.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/cloudshell/traffic_mirror_pool_services.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/cloudshell/cs_subnet_service.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/vpc.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/cloudshell/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/instance_credentials.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/subnet.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/tags.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/traffic_mirror_cleaner.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/ebs.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/traffic_mirroring_operation.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/elastic_ip.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/instance.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/cleanup.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/mirroring.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/prepare.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/network_interface.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/operations/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/transit_gateway.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/operations/vm_details_operation.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/security_group.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/operations/set_app_security_groups.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/keypair.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/operations/app_ports_operation.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/vpc.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/operations/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/route_table.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/device_index.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/prepare_subnets.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/route_table_handler.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/cleanup.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/cidr_block_handler.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/tags_handler.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/prepare_cloud_infra.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/route_handler.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/s3/bucket.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/s3/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/vpc_peering_handler.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/session_providers/aws_session_provider.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_connectivity/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/session_providers/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_ami_management/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_deployed_app/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/cloudshell/traffic_mirror_pool_services.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/cloudshell/cs_subnet_service.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_common/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/cancellation_service.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/handlers/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/list_helper.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/conftest.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/CheckCancellationThread.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_aws_shell.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/exceptions.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/base.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/aws_session_manager.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_connectivity/test_prepare_connectivity.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/vm_details_provider.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_connectivity/test_cleanup_connectivity.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/operations/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_connectivity/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/operations/autoload_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_connectivity/test_create_traffic_mirroring.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_ami_management/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/cidr_block_handler.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/test_power_operation.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/route_handler.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/test_deploy_operation.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/tags_handler.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/test_delete_operation.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/vpc_peering_handler.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/route_table_handler.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/test_refresh_ip_operation.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_deployed_app/test_operations/
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_deployed_app/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_deployed_app/test_operations/test_access_key_operation.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/deploy_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_deployed_app/test_operations/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/refresh_ip_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_deployed_app/test_operations/test_set_app_security_groups_operation.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/access_key_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_deployed_app/test_operations/test_app_ports_operation.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/power_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_key_pair.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_vpc.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/delete_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_elastic_ip.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/snapshot_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_vm_custom_params_extractor.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_port_group_attribute_parser.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_network_interface_service.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/prepare_subnet_executor.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_session_provider.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/traffic_mirroring_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_subnet.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/prepare.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/cleanup.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_ami_waiter.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/traffic_mirror_cleaner.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_model_parser.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_security_groups.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/operations/
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_instance_waiter.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_ami_creds_service.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/operations/vm_details_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_device_index_strategy.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/operations/app_ports_operation.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_vpc_waiter.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/operations/set_app_security_groups.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_instance_service.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/operations/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_subnet_waiter.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/aws_shell.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_bucket.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/aws_resource_model.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_password_waiter.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/ec2_session.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_common/test_cancellation_service.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/ec2_client.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_common/test_get_vm_details.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/aws_api.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_common/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/__init__.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_common/test_converters.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/s3_session.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_common/test_vm_details_provider.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/client_error.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/test_common/test_retry_helper.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/ami_credentials.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/handlers/__init__.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/traffic_mirror_fulfillment.py
 Comment: 
 
-Filename: cloudshell-cp-aws-3.4.0/tests/handlers/test_route_table_handler.py
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/vm_details.py
+Comment: 
+
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/ami_deployment_model.py
+Comment: 
+
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/aws_ec2_cloud_provider_resource_model.py
+Comment: 
+
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/aws_api.py
+Comment: 
+
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/app_security_groups_model.py
+Comment: 
+
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/__init__.py
+Comment: 
+
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/network_actions_models.py
+Comment: 
+
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/deploy_aws_ec2_ami_instance_resource_model.py
+Comment: 
+
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/port_data.py
+Comment: 
+
+Filename: cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/reservation_model.py
 Comment: 
 
 Zip file comment:
```

## Comparing `cloudshell-cp-aws-3.4.0/PKG-INFO` & `cloudshell-cp-aws-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudshell-cp-aws
-Version: 3.4.0
+Version: 3.5.0
 Summary: A repository for projects providing out of the box capabilities within CloudShell to define AWS instances in CloudShell and leverage Amazon Cloud Computing capabilities to deploy and connect apps in CloudShell sandboxes.
 Home-page: http://www.qualisystems.com/
 Author: QualiSystems
 Author-email: info@qualisystems.com
 Requires-Python: ~=3.7
 
 A repository for projects providing out of the box capabilities within CloudShell to define AWS instances in CloudShell and leverage Amazon Cloud Computing capabilities to deploy and connect apps in CloudShell sandboxes.
```

## Comparing `cloudshell-cp-aws-3.4.0/tox.ini` & `cloudshell-cp-aws-3.5.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 profile=black
 forced_separate = cloudshell.cp.aws,tests
 
 [flake8]
 max-line-length = 88
 ;we don't need have docstrings in every func, class and package
 ;and W503 is not PEP 8 compliant
-ignore = D100,D101,D102,D103,D104,D105,D106,D107,D401,W503,E203
+ignore = D100,D101,D102,D103,D104,D105,D106,D107,D401,W503,E203,I900
```

## Comparing `cloudshell-cp-aws-3.4.0/setup.py` & `cloudshell-cp-aws-3.5.0/setup.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/README.md` & `cloudshell-cp-aws-3.5.0/README.md`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell_cp_aws.egg-info/PKG-INFO` & `cloudshell-cp-aws-3.5.0/cloudshell_cp_aws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudshell-cp-aws
-Version: 3.4.0
+Version: 3.5.0
 Summary: A repository for projects providing out of the box capabilities within CloudShell to define AWS instances in CloudShell and leverage Amazon Cloud Computing capabilities to deploy and connect apps in CloudShell sandboxes.
 Home-page: http://www.qualisystems.com/
 Author: QualiSystems
 Author-email: info@qualisystems.com
 Requires-Python: ~=3.7
 
 A repository for projects providing out of the box capabilities within CloudShell to define AWS instances in CloudShell and leverage Amazon Cloud Computing capabilities to deploy and connect apps in CloudShell sandboxes.
```

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell_cp_aws.egg-info/SOURCES.txt` & `cloudshell-cp-aws-3.5.0/cloudshell_cp_aws.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 cloudshell/cp/aws/aws_shell.py
 cloudshell/cp/aws/common/__init__.py
 cloudshell/cp/aws/common/cached_property.py
 cloudshell/cp/aws/common/converters.py
 cloudshell/cp/aws/common/deploy_data_holder.py
 cloudshell/cp/aws/common/exceptions.py
 cloudshell/cp/aws/common/retry_helper.py
+cloudshell/cp/aws/common/subnet_service.py
 cloudshell/cp/aws/domain/__init__.py
 cloudshell/cp/aws/domain/ami_management/__init__.py
 cloudshell/cp/aws/domain/ami_management/operations/__init__.py
 cloudshell/cp/aws/domain/ami_management/operations/access_key_operation.py
 cloudshell/cp/aws/domain/ami_management/operations/delete_operation.py
 cloudshell/cp/aws/domain/ami_management/operations/deploy_operation.py
 cloudshell/cp/aws/domain/ami_management/operations/power_operation.py
@@ -32,20 +33,25 @@
 cloudshell/cp/aws/domain/common/exceptions.py
 cloudshell/cp/aws/domain/common/list_helper.py
 cloudshell/cp/aws/domain/common/vm_details_provider.py
 cloudshell/cp/aws/domain/conncetivity/__init__.py
 cloudshell/cp/aws/domain/conncetivity/operations/__init__.py
 cloudshell/cp/aws/domain/conncetivity/operations/cleanup.py
 cloudshell/cp/aws/domain/conncetivity/operations/prepare.py
+cloudshell/cp/aws/domain/conncetivity/operations/prepare_subnet_executor.py
 cloudshell/cp/aws/domain/conncetivity/operations/traffic_mirror_cleaner.py
 cloudshell/cp/aws/domain/conncetivity/operations/traffic_mirroring_operation.py
 cloudshell/cp/aws/domain/context/__init__.py
 cloudshell/cp/aws/domain/context/aws_api.py
 cloudshell/cp/aws/domain/context/aws_resource_model.py
 cloudshell/cp/aws/domain/context/aws_shell.py
+cloudshell/cp/aws/domain/context/client_error.py
+cloudshell/cp/aws/domain/context/ec2_client.py
+cloudshell/cp/aws/domain/context/ec2_session.py
+cloudshell/cp/aws/domain/context/s3_session.py
 cloudshell/cp/aws/domain/deployed_app/__init__.py
 cloudshell/cp/aws/domain/deployed_app/operations/__init__.py
 cloudshell/cp/aws/domain/deployed_app/operations/app_ports_operation.py
 cloudshell/cp/aws/domain/deployed_app/operations/set_app_security_groups.py
 cloudshell/cp/aws/domain/deployed_app/operations/vm_details_operation.py
 cloudshell/cp/aws/domain/handlers/__init__.py
 cloudshell/cp/aws/domain/handlers/ec2/__init__.py
@@ -64,16 +70,18 @@
 cloudshell/cp/aws/domain/services/ec2/ebs.py
 cloudshell/cp/aws/domain/services/ec2/elastic_ip.py
 cloudshell/cp/aws/domain/services/ec2/instance.py
 cloudshell/cp/aws/domain/services/ec2/instance_credentials.py
 cloudshell/cp/aws/domain/services/ec2/keypair.py
 cloudshell/cp/aws/domain/services/ec2/mirroring.py
 cloudshell/cp/aws/domain/services/ec2/network_interface.py
+cloudshell/cp/aws/domain/services/ec2/route_table.py
 cloudshell/cp/aws/domain/services/ec2/security_group.py
 cloudshell/cp/aws/domain/services/ec2/subnet.py
+cloudshell/cp/aws/domain/services/ec2/tags.py
 cloudshell/cp/aws/domain/services/ec2/transit_gateway.py
 cloudshell/cp/aws/domain/services/ec2/vpc.py
 cloudshell/cp/aws/domain/services/parsers/__init__.py
 cloudshell/cp/aws/domain/services/parsers/aws_model_parser.py
 cloudshell/cp/aws/domain/services/parsers/command_results_parser.py
 cloudshell/cp/aws/domain/services/parsers/custom_param_extractor.py
 cloudshell/cp/aws/domain/services/parsers/port_group_attribute_parser.py
@@ -89,14 +97,15 @@
 cloudshell/cp/aws/domain/services/strategy/prepare_subnets.py
 cloudshell/cp/aws/domain/services/waiters/__init__.py
 cloudshell/cp/aws/domain/services/waiters/ami.py
 cloudshell/cp/aws/domain/services/waiters/instance.py
 cloudshell/cp/aws/domain/services/waiters/password.py
 cloudshell/cp/aws/domain/services/waiters/subnet.py
 cloudshell/cp/aws/domain/services/waiters/vpc.py
+cloudshell/cp/aws/domain/services/waiters/vpc_peering.py
 cloudshell/cp/aws/models/__init__.py
 cloudshell/cp/aws/models/ami_credentials.py
 cloudshell/cp/aws/models/ami_deployment_model.py
 cloudshell/cp/aws/models/app_security_groups_model.py
 cloudshell/cp/aws/models/aws_api.py
 cloudshell/cp/aws/models/aws_ec2_cloud_provider_resource_model.py
 cloudshell/cp/aws/models/deploy_aws_ec2_ami_instance_resource_model.py
```

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/aws_shell.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/aws_shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 
 import jsonpickle
 from botocore.exceptions import ClientError, NoCredentialsError
 
 from cloudshell.cp.core.drive_request_parser import DriverRequestParser
 from cloudshell.cp.core.models import ConnectSubnet, DeployApp, VmDetailsData
```

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/deploy_aws_ec2_ami_instance_resource_model.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/deploy_aws_ec2_ami_instance_resource_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,19 +72,20 @@
         private_ip_att_value = get_attr("Private IP")
         self.private_ip_address = self._get_primary_private_ip_address(
             private_ip_att_value
         )
         self.private_ip_addresses_dict = self._get_private_ip_addresses_dict(
             private_ip_att_value
         )
+        self.static_sg_id = get_attr("Static Security Group Id")
 
     def _get_private_ip_addresses_dict(self, private_ip_address):
         try:
             # if dict of private ip address then we take the first as the primary
-            return json.loads(private_ip_address)
+            return json.loads(private_ip_address.replace("'", '"'))
         except Exception:
             return None
 
     def _get_primary_private_ip_address(self, private_ip_address):
         try:
             # if dict of private ip address then we take the first as the primary
             return json.loads(private_ip_address).values()[0]
```

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/port_data.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/port_data.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/traffic_mirror_fulfillment.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/traffic_mirror_fulfillment.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/aws_api.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/aws_api.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/network_actions_models.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/network_actions_models.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/ami_deployment_model.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/ami_deployment_model.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/aws_ec2_cloud_provider_resource_model.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/aws_ec2_cloud_provider_resource_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 
 class VpcMode(Enum):
     DYNAMIC = "Dynamic"
     STATIC = "Static"
     SHARED = "Shared"
     SINGLE = "Single"
+    PREDEFINED = "Predefined networking"
 
 
 @dataclass
 class AWSEc2CloudProviderResourceModel:
     region: str
     aws_mgmt_sg_id: str
     aws_mgmt_vpc_id: str
```

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/models/app_security_groups_model.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/models/app_security_groups_model.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/converters.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/converters.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/common/deploy_data_holder.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/common/deploy_data_holder.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/context/aws_resource_model.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/aws_resource_model.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/context/aws_api.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/aws_api.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/context/aws_shell.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/context/aws_shell.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/delete_operation.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/delete_operation.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/refresh_ip_operation.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/refresh_ip_operation.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/deploy_operation.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/deploy_operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 import traceback
 import uuid
 from multiprocessing import TimeoutError
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING
 
 from cloudshell.cp.core.models import (
     ConnectSubnet,
     ConnectToSubnetActionResult,
     ConnectToSubnetParams,
     DeployAppResult,
 )
@@ -53,20 +55,20 @@
     MAX_IO1_IOPS = 20000
 
     def __init__(
         self,
         instance_service,
         ami_credential_service,
         security_group_service,
-        vpc_service: "VPCService",
+        vpc_service: VPCService,
         key_pair_service,
         subnet_service,
         elastic_ip_service,
-        network_interface_service: "NetworkInterfaceService",
-        device_index_strategy: "AbstractDeviceIndexStrategy",
+        network_interface_service: NetworkInterfaceService,
+        device_index_strategy: AbstractDeviceIndexStrategy,
         vm_details_provider,
     ):
         """# noqa
         :param cloudshell.cp.aws.domain.services.ec2.instance.InstanceService instance_service: Instance Service
         :param InstanceCredentialsService ami_credential_service: AMI Credential Service
         :param SecurityGroupService security_group_service: Security Group Service
         :param KeyPairService key_pair_service: Key Pair Service
@@ -113,19 +115,23 @@
         :param network_actions: The network actions.
         :type network_actions: list[cloudshell.cp.core.models.ConnectSubnet]
         :param logging.Logger logger:
         :param CancellationContext cancellation_context:
         :return: Deploy Result
         :rtype: list[RequestActionBase]
         """
-        ami_deployment_model: "DeployAWSEc2AMIInstanceResourceModel" = (  # noqa
+        ami_deployment_model: DeployAWSEc2AMIInstanceResourceModel = (  # noqa
             ami_deploy_action.actionParams.deployment.customModel
         )
         vpc = self._get_vpc(
-            ec2_session, aws_ec2_cp_resource_model, reservation.reservation_id, logger
+            ec2_session,
+            aws_ec2_cp_resource_model,
+            reservation.reservation_id,
+            logger,
+            network_actions,
         )
         key_name = self.key_pair_service.get_reservation_key_name(
             reservation_id=reservation.reservation_id
         )
         logger.info(f"Found shared sandbox key pair '{key_name}'")
 
         check_if_cancelled(cancellation_context)
@@ -252,28 +258,41 @@
         )
         deploy_app_result.actionId = ami_deploy_action.actionId
         network_actions_results_dtos.append(deploy_app_result)
         return network_actions_results_dtos
 
     def _get_vpc(
         self,
-        ec2_session: "EC2ServiceResource",
-        aws_model: "AWSEc2CloudProviderResourceModel",
+        ec2_session: EC2ServiceResource,
+        aws_model: AWSEc2CloudProviderResourceModel,
         reservation_id: str,
-        logger: "Logger",
-    ) -> "Vpc":
+        logger: Logger,
+        network_actions: list[ConnectSubnet],
+    ) -> Vpc:
         if aws_model.vpc_mode in (VpcMode.DYNAMIC, VpcMode.STATIC):
             logger.info(f"Getting the VPC for the reservation {reservation_id}")
             vpc = self.vpc_service.get_vpc_for_reservation(ec2_session, reservation_id)
         elif aws_model.vpc_mode is VpcMode.SHARED:
             logger.info(f"Getting the VPC by the id {aws_model.shared_vpc_id}")
             vpc = self.vpc_service.get_vpc_by_id(ec2_session, aws_model.shared_vpc_id)
         elif aws_model.vpc_mode is VpcMode.SINGLE:
             logger.info(f"Getting the VPC by the id {aws_model.aws_mgmt_vpc_id}")
             vpc = self.vpc_service.get_vpc_by_id(ec2_session, aws_model.aws_mgmt_vpc_id)
+        elif aws_model.vpc_mode is VpcMode.PREDEFINED:
+            subnet_ids = {a.actionParams.subnetId for a in network_actions}
+            subnet_ids = list(subnet_ids)
+            # # todo check that we receive all requested subnets
+            subnets = list(ec2_session.subnets.filter(SubnetIds=subnet_ids))
+            set_vpc = {s.vpc for s in subnets}
+            if len(set_vpc) > 1:
+                raise Exception(
+                    f"When using {VpcMode.PREDEFINED.value} VPC mode, VM can be "
+                    f"connected to subnets only from the same VPC."
+                )
+            vpc = next(iter(set_vpc))
         else:
             raise ValueError(f"VpcMode is wrong {aws_model.vpc_mode}")
 
         return vpc
 
     def _validate_public_subnet_exist_if_requested_public_or_elastic_ips(
         self, ami_deployment_model, network_actions, logger
@@ -334,16 +353,16 @@
             }
         )
         return ConnectToSubnetActionResult(
             actionId=network_config_result.action_id, interface=interface_data_json_str
         )
 
     def _prepare_network_result_models(
-        self, network_actions: List[ConnectSubnet]
-    ) -> List[DeployNetworkingResultModel]:
+        self, network_actions: list[ConnectSubnet]
+    ) -> list[DeployNetworkingResultModel]:
         network_config_results = []
         if not network_actions:
             network_config_results.append(
                 DeployNetworkingResultModel("")
             )  # init a result object with empty action id
         else:
             for net_config in network_actions:
@@ -447,15 +466,15 @@
 
     @staticmethod
     def _get_name_from_tags(result):
         return [tag["Value"] for tag in result.tags if tag["Key"] == "Name"][0]
 
     def _create_security_group_for_instance(
         self,
-        ami_deployment_model: "DeployAWSEc2AMIInstanceResourceModel",
+        ami_deployment_model: DeployAWSEc2AMIInstanceResourceModel,
         ec2_session,
         reservation,
         vpc,
         logger,
     ):
         if (
             not ami_deployment_model.inbound_ports
@@ -575,20 +594,28 @@
         aws_model.block_device_mappings = self._get_block_device_mappings(
             image=image,
             ami_deployment_model=ami_deployment_model,
             aws_ec2_resource_model=aws_ec2_resource_model,
         )
         aws_model.aws_key = key_pair
 
-        security_group_ids = self._get_security_group_param(
-            reservation,
-            security_group,
-            vpc,
-            ami_deployment_model.allow_all_sandbox_traffic,
-        )
+        if aws_ec2_resource_model.vpc_mode is VpcMode.PREDEFINED:
+            security_group_ids = []
+            if security_group:
+                security_group_ids.append(security_group.group_id)
+        else:
+            security_group_ids = self._get_security_group_param(
+                reservation,
+                security_group,
+                vpc,
+                ami_deployment_model.allow_all_sandbox_traffic,
+            )
+        if ami_deployment_model.static_sg_id:
+            security_group_ids.append(ami_deployment_model.static_sg_id)
+
         aws_model.security_group_ids = security_group_ids
 
         aws_model.network_interfaces = self._prepare_network_interfaces(
             vpc=vpc,
             ami_deployment_model=ami_deployment_model,
             network_actions=network_actions,
             security_group_ids=security_group_ids,
@@ -607,23 +634,23 @@
             return {}
         if role.startswith("arn:"):
             return {"Arn": role}
         return {"Name": role}
 
     def _prepare_network_interfaces(
         self,
-        vpc: "Vpc",
-        ami_deployment_model: "DeployAWSEc2AMIInstanceResourceModel",
-        network_actions: List["ConnectSubnet"],
-        security_group_ids: List[str],
-        network_config_results: List[DeployNetworkingResultModel],
-        reservation: "ReservationModel",
-        aws_model: "AWSEc2CloudProviderResourceModel",
-        ec2_session: "EC2ServiceResource",
-        logger: "Logger",
+        vpc: Vpc,
+        ami_deployment_model: DeployAWSEc2AMIInstanceResourceModel,
+        network_actions: list[ConnectSubnet],
+        security_group_ids: list[str],
+        network_config_results: list[DeployNetworkingResultModel],
+        reservation: ReservationModel,
+        aws_model: AWSEc2CloudProviderResourceModel,
+        ec2_session: EC2ServiceResource,
+        logger: Logger,
     ):
         if not network_actions:
             logger.info("Single subnet mode detected")
             network_config_results[0].device_index = 0
             return [
                 self.network_interface_service.get_network_interface_for_single_subnet_mode(  # noqa: E501
                     add_public_ip=ami_deployment_model.add_public_ip,
```

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/snapshot_operation.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/snapshot_operation.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/power_operation.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/power_operation.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/ami_management/operations/access_key_operation.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/ami_management/operations/access_key_operation.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/cancellation_service.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/cancellation_service.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/aws_session_manager.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/aws_session_manager.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/CheckCancellationThread.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/CheckCancellationThread.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/common/vm_details_provider.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/common/vm_details_provider.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/operations/autoload_operation.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/operations/autoload_operation.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/prepare_cloud_infra.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/prepare_cloud_infra.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 from abc import ABCMeta, abstractmethod
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING
 
 import attr
 
 from cloudshell.cp.core.models import PrepareCloudInfraResult
 
 from cloudshell.cp.aws.common.cached_property import cached_property
 from cloudshell.cp.aws.domain.common.cancellation_service import check_if_cancelled
@@ -44,24 +46,24 @@
         AWSEc2CloudProviderResourceModel,
     )
     from cloudshell.cp.aws.models.reservation_model import ReservationModel
 
 
 @attr.s(auto_attribs=True)
 class PrepareCloudInfraAbsStrategy(metaclass=ABCMeta):
-    _vpc_service: "VPCService"
-    _security_group_service: "SecurityGroupService"
-    _aws_clients: "AwsApiClients"
-    _aws_model: "AWSEc2CloudProviderResourceModel"
-    _reservation: "ReservationModel"
-    _network_action: "PrepareCloudInfra"
-    _cancellation_context: "CancellationContext"
-    _logger: "Logger"
+    _vpc_service: VPCService
+    _security_group_service: SecurityGroupService
+    _aws_clients: AwsApiClients
+    _aws_model: AWSEc2CloudProviderResourceModel
+    _reservation: ReservationModel
+    _network_action: PrepareCloudInfra
+    _cancellation_context: CancellationContext
+    _logger: Logger
 
-    def prepare(self) -> "PrepareCloudInfraResult":
+    def prepare(self) -> PrepareCloudInfraResult:
         check_if_cancelled(self._cancellation_context)
         vpc = self.vpc
         self.enable_dns_hostnames(vpc)
 
         check_if_cancelled(self._cancellation_context)
         igw = self.get_or_create_igw()
 
@@ -77,64 +79,64 @@
         isolated_sg = self.create_isolated_sg()
         default_sg = self.create_default_sg()
         self.set_sg_rules(isolated_sg, default_sg)
 
         return self.prepare_result([isolated_sg, default_sg])
 
     @cached_property
-    def vpc(self) -> "Vpc":
+    def vpc(self) -> Vpc:
         """Get or create a VPC based on the VPC mode."""
         return self._get_or_create_vpc()
 
     @abstractmethod
-    def _get_or_create_vpc(self) -> "Vpc":
+    def _get_or_create_vpc(self) -> Vpc:
         raise NotImplementedError
 
     @cached_property
     def vpc_name(self) -> str:
         return self._vpc_service.get_name(self.vpc)
 
-    def enable_dns_hostnames(self, vpc: "Vpc"):
+    def enable_dns_hostnames(self, vpc: Vpc):
         self._logger.info(f"Enable dns for the VPC '{self.vpc_name}'")
         self._vpc_service.modify_vpc_attribute(
             self._aws_clients.ec2_client, self.vpc.vpc_id, enable_dns_hostnames=True
         )
 
     @abstractmethod
-    def get_or_create_igw(self) -> Optional["InternetGateway"]:
+    def get_or_create_igw(self) -> InternetGateway | None:
         raise NotImplementedError
 
     @abstractmethod
-    def get_or_create_public_rt(self) -> "RouteTableHandler":
+    def get_or_create_public_rt(self) -> RouteTableHandler:
         raise NotImplementedError
 
-    def get_or_create_private_rt(self) -> "RouteTableHandler":
+    def get_or_create_private_rt(self) -> RouteTableHandler:
         return RouteTableHandler.get_or_create_private_rt(
             self.vpc, self._reservation, self._logger
         )
 
     def add_route_to_igw(
-        self, public_rt: "RouteTableHandler", igw: Optional["InternetGateway"]
+        self, public_rt: RouteTableHandler, igw: InternetGateway | None
     ):
         if not igw:
             return
 
         self._logger.info(
             f"Adding default route to IGW {igw.id} from public route table "
             f"'{public_rt.name}'"
         )
         public_rt.add_default_route_to_gw(igw.id)
 
     @abstractmethod
     def connect_vpc_to_mgmt_vpc(
-        self, public_rt: "RouteTableHandler", private_rt: "RouteTableHandler"
+        self, public_rt: RouteTableHandler, private_rt: RouteTableHandler
     ):
         raise NotImplementedError
 
-    def create_isolated_sg(self) -> "SecurityGroup":
+    def create_isolated_sg(self) -> SecurityGroup:
         sg_name = self._security_group_service.sandbox_isolated_sg_name(
             self._reservation.reservation_id
         )
         self._logger.info(
             f"Searching for an isolated SG '{sg_name}' in the VPC '{self.vpc_name}'"
         )
         sg = self._security_group_service.get_security_group_by_name(self.vpc, sg_name)
@@ -151,15 +153,15 @@
                 self._reservation,
                 IsolationTagValue.SHARED,
                 TypeTagValue.ISOLATED,
             )
             tags.add_tags_to_obj(sg)
         return sg
 
-    def create_default_sg(self) -> "SecurityGroup":
+    def create_default_sg(self) -> SecurityGroup:
         sg_name = self._security_group_service.sandbox_default_sg_name(
             self._reservation.reservation_id
         )
         self._logger.info(
             f"Searching for a default SG '{sg_name}' in the VPC '{self.vpc_name}'"
         )
         sg = self._security_group_service.get_security_group_by_name(self.vpc, sg_name)
@@ -177,54 +179,55 @@
                 IsolationTagValue.SHARED,
                 TypeTagValue.DEFAULT,
             )
             tags.add_tags_to_obj(sg)
         return sg
 
     @abstractmethod
-    def set_sg_rules(self, isolated_sg: "SecurityGroup", default_sg: "SecurityGroup"):
+    def set_sg_rules(self, isolated_sg: SecurityGroup, default_sg: SecurityGroup):
         raise NotImplementedError
 
     def prepare_result(
         self,
-        security_groups: List["SecurityGroup"],
-    ) -> "PrepareCloudInfraResult":
+        security_groups: list[SecurityGroup],
+    ) -> PrepareCloudInfraResult:
         result = PrepareCloudInfraResult(
             actionId=self._network_action.actionId,
             success=True,
             infoMessage="PrepareCloudInfra finished successfully",
         )
-        result.vpcId = self.vpc.id
+        if self.vpc:
+            result.vpcId = self.vpc.id
         result.securityGroupId = [sg.id for sg in security_groups]
         return result
 
 
 class PrepareCloudInfraDynamicStrategy(PrepareCloudInfraAbsStrategy):
     def _get_vpc_cidr(self) -> str:
         return self._network_action.actionParams.cidr
 
-    def _get_or_create_vpc(self) -> "Vpc":
+    def _get_or_create_vpc(self) -> Vpc:
         return self._vpc_service.get_or_create_vpc_for_reservation(
             self._reservation,
             self._aws_clients.ec2_session,
             self._get_vpc_cidr(),
             self._logger,
         )
 
-    def get_or_create_igw(self) -> "InternetGateway":
+    def get_or_create_igw(self) -> InternetGateway:
         return self._vpc_service.get_or_create_igw(
             self._aws_clients.ec2_session, self.vpc, self._reservation, self._logger
         )
 
-    def get_or_create_public_rt(self) -> "RouteTableHandler":
+    def get_or_create_public_rt(self) -> RouteTableHandler:
         self._logger.info(f"Getting a main route table for the VPC '{self.vpc_name}'")
         return RouteTableHandler.get_main_rt(self.vpc, self._reservation)
 
     def connect_vpc_to_mgmt_vpc(
-        self, public_rt: "RouteTableHandler", private_rt: "RouteTableHandler"
+        self, public_rt: RouteTableHandler, private_rt: RouteTableHandler
     ):
         try:
             peering = VpcPeeringHandler.get_active_by_reservation_id(
                 self._aws_clients.ec2_session, self._reservation.reservation_id
             )
         except VpcPeeringConnectionNotFoundForReservation:
             peering = VpcPeeringHandler.create(
@@ -242,15 +245,15 @@
         for rt in RouteTableHandler.get_all_rts(mgmt_vpc):
             rt.add_route_to_peering(peering.id, self.vpc.cidr_block)
 
         # create routes to peering from sandbox VPC
         for rt in (public_rt, private_rt):
             rt.add_route_to_peering(peering.id, mgmt_vpc.cidr_block)
 
-    def set_sg_rules(self, isolated_sg: "SecurityGroup", default_sg: "SecurityGroup"):
+    def set_sg_rules(self, isolated_sg: SecurityGroup, default_sg: SecurityGroup):
         self._security_group_service.set_isolated_security_group_rules(
             isolated_sg, self._aws_model.aws_mgmt_sg_id, need_management_access=True
         )
         self._security_group_service.set_shared_reservation_security_group_rules(
             security_group=default_sg,
             management_sg_id=self._aws_model.aws_mgmt_sg_id,
             isolated_sg=isolated_sg,
@@ -258,78 +261,78 @@
         )
 
 
 class PrepareCloudInfraStaticStrategy(PrepareCloudInfraAbsStrategy):
     def _get_vpc_cidr(self) -> str:
         return self._aws_model.static_vpc_cidr
 
-    def _get_or_create_vpc(self) -> "Vpc":
+    def _get_or_create_vpc(self) -> Vpc:
         return self._vpc_service.get_or_create_vpc_for_reservation(
             self._reservation,
             self._aws_clients.ec2_session,
             self._get_vpc_cidr(),
             self._logger,
         )
 
-    def get_or_create_igw(self) -> "InternetGateway":
+    def get_or_create_igw(self) -> InternetGateway:
         return self._vpc_service.get_or_create_igw(
             self._aws_clients.ec2_session, self.vpc, self._reservation, self._logger
         )
 
-    def get_or_create_public_rt(self) -> "RouteTableHandler":
+    def get_or_create_public_rt(self) -> RouteTableHandler:
         self._logger.info(f"Getting a main route table for the VPC '{self.vpc_name}'")
         return RouteTableHandler.get_main_rt(self.vpc, self._reservation)
 
     def connect_vpc_to_mgmt_vpc(
-        self, public_rt: "RouteTableHandler", private_rt: "RouteTableHandler"
+        self, public_rt: RouteTableHandler, private_rt: RouteTableHandler
     ):
         self._logger.info("In Static VPC mode we do not create peering to MGMT VPC")
 
-    def set_sg_rules(self, isolated_sg: "SecurityGroup", default_sg: "SecurityGroup"):
+    def set_sg_rules(self, isolated_sg: SecurityGroup, default_sg: SecurityGroup):
         self._security_group_service.set_isolated_security_group_rules(
             isolated_sg, self._aws_model.aws_mgmt_sg_id, need_management_access=False
         )
         self._security_group_service.set_shared_reservation_security_group_rules(
             security_group=default_sg,
             management_sg_id=self._aws_model.aws_mgmt_sg_id,
             isolated_sg=isolated_sg,
             need_management_sg=False,
         )
 
 
 class PrepareCloudInfraSharedStrategy(PrepareCloudInfraAbsStrategy):
-    def _get_or_create_vpc(self) -> "Vpc":
+    def _get_or_create_vpc(self) -> Vpc:
         return self._vpc_service.get_vpc_by_id(
             self._aws_clients.ec2_session, self._aws_model.shared_vpc_id
         )
 
-    def get_or_create_igw(self) -> Optional["InternetGateway"]:
+    def get_or_create_igw(self) -> InternetGateway | None:
         return self._vpc_service.get_first_igw(self.vpc)
 
-    def get_or_create_public_rt(self) -> "RouteTableHandler":
+    def get_or_create_public_rt(self) -> RouteTableHandler:
         return RouteTableHandler.get_or_create_public_rt(
             self.vpc, self._reservation, self._logger
         )
 
     def connect_vpc_to_mgmt_vpc(
-        self, public_rt: "RouteTableHandler", private_rt: "RouteTableHandler"
+        self, public_rt: RouteTableHandler, private_rt: RouteTableHandler
     ):
         mgmt_vpc = self._vpc_service.get_vpc_by_id(
             self._aws_clients.default_ec2_session, self._aws_model.aws_mgmt_vpc_id
         )
         cidr_blocks = get_transit_gateway_cidr_blocks(
             self._aws_clients.ec2_client, self._aws_model.tgw_id
         )
         cidr_blocks.append(mgmt_vpc.cidr_block)
         cidr_blocks.extend(self._aws_model.additional_mgmt_networks)
 
         for route_table in (public_rt, private_rt):
             route_table.add_routes_to_tgw(self._aws_model.tgw_id, cidr_blocks)
 
-    def set_sg_rules(self, isolated_sg: "SecurityGroup", default_sg: "SecurityGroup"):
+    def set_sg_rules(self, isolated_sg: SecurityGroup, default_sg: SecurityGroup):
         self._security_group_service.set_isolated_security_group_rules(
             isolated_sg, self._aws_model.aws_mgmt_sg_id, need_management_access=False
         )
         self._security_group_service.set_shared_reservation_security_group_rules(
             security_group=default_sg,
             management_sg_id=self._aws_model.aws_mgmt_sg_id,
             isolated_sg=isolated_sg,
@@ -343,33 +346,33 @@
         for sg in (isolated_sg, default_sg):
             self._security_group_service.set_security_group_rules(
                 sg, inbound_ports, logger=self._logger
             )
 
 
 class PrepareCloudInfraSingleStrategy(PrepareCloudInfraAbsStrategy):
-    def _get_or_create_vpc(self) -> "Vpc":
+    def _get_or_create_vpc(self) -> Vpc:
         return self._vpc_service.get_vpc_by_id(
             self._aws_clients.ec2_session, self._aws_model.aws_mgmt_vpc_id
         )
 
-    def get_or_create_igw(self) -> Optional["InternetGateway"]:
+    def get_or_create_igw(self) -> InternetGateway | None:
         return self._vpc_service.get_first_igw(self.vpc)
 
-    def get_or_create_public_rt(self) -> "RouteTableHandler":
+    def get_or_create_public_rt(self) -> RouteTableHandler:
         return RouteTableHandler.get_or_create_public_rt(
             self.vpc, self._reservation, self._logger
         )
 
     def connect_vpc_to_mgmt_vpc(
-        self, public_rt: "RouteTableHandler", private_rt: "RouteTableHandler"
+        self, public_rt: RouteTableHandler, private_rt: RouteTableHandler
     ):
         pass
 
-    def set_sg_rules(self, isolated_sg: "SecurityGroup", default_sg: "SecurityGroup"):
+    def set_sg_rules(self, isolated_sg: SecurityGroup, default_sg: SecurityGroup):
         self._security_group_service.set_isolated_security_group_rules(
             isolated_sg, self._aws_model.aws_mgmt_sg_id, need_management_access=False
         )
         self._security_group_service.set_shared_reservation_security_group_rules(
             security_group=default_sg,
             management_sg_id=self._aws_model.aws_mgmt_sg_id,
             isolated_sg=isolated_sg,
@@ -382,34 +385,60 @@
         ]
         for sg in (isolated_sg, default_sg):
             self._security_group_service.set_security_group_rules(
                 sg, inbound_ports, logger=self._logger
             )
 
 
+class PrepareCloudInfraPredefinedNetworkingStrategy(PrepareCloudInfraAbsStrategy):
+    def prepare(self) -> PrepareCloudInfraResult:
+        # we do not create IGW, RTs, SGs and peering
+        return self.prepare_result([])
+
+    def _get_or_create_vpc(self) -> Vpc:
+        pass
+
+    def get_or_create_igw(self) -> InternetGateway | None:
+        pass
+
+    def get_or_create_public_rt(self) -> RouteTableHandler:
+        pass
+
+    def connect_vpc_to_mgmt_vpc(
+        self, public_rt: RouteTableHandler, private_rt: RouteTableHandler
+    ):
+        pass
+
+    def set_sg_rules(self, isolated_sg: SecurityGroup, default_sg: SecurityGroup):
+        pass
+
+
 STRATEGIES = {
     VpcMode.DYNAMIC: PrepareCloudInfraDynamicStrategy,
     VpcMode.STATIC: PrepareCloudInfraStaticStrategy,
     VpcMode.SHARED: PrepareCloudInfraSharedStrategy,
     VpcMode.SINGLE: PrepareCloudInfraSingleStrategy,
+    VpcMode.PREDEFINED: PrepareCloudInfraPredefinedNetworkingStrategy,
 }
 
 
 def get_prepare_infra_strategy(
-    vpc_service: "VPCService",
-    security_group_service: "SecurityGroupService",
-    aws_clients: "AwsApiClients",
-    aws_model: "AWSEc2CloudProviderResourceModel",
-    reservation: "ReservationModel",
-    network_action: "PrepareCloudInfra",
-    cancellation_context: "CancellationContext",
-    logger: "Logger",
+    vpc_service: VPCService,
+    security_group_service: SecurityGroupService,
+    aws_clients: AwsApiClients,
+    aws_model: AWSEc2CloudProviderResourceModel,
+    reservation: ReservationModel,
+    network_action: PrepareCloudInfra,
+    cancellation_context: CancellationContext,
+    logger: Logger,
 ) -> PrepareCloudInfraAbsStrategy:
+    strategy_class = STRATEGIES[aws_model.vpc_mode]
+
     # noinspection PyArgumentList
-    return STRATEGIES[aws_model.vpc_mode](  # pycharm fails to get correct params
+    return strategy_class(  # pycharm fails to get correct params
         vpc_service,
         security_group_service,
         aws_clients,
         aws_model,
         reservation,
         network_action,
         cancellation_context,
```

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/prepare_subnets.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/prepare_subnets.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import attr
 from typing_extensions import Protocol
 
 from cloudshell.cp.core.models import PrepareCloudInfraResult
 
 from cloudshell.cp.aws.common.cached_property import cached_property
+from cloudshell.cp.aws.common.subnet_service import get_subnet_id
 from cloudshell.cp.aws.domain.common.cancellation_service import check_if_cancelled
 from cloudshell.cp.aws.domain.handlers.ec2 import RouteTableHandler, TagsHandler
 from cloudshell.cp.aws.domain.handlers.ec2.cidr_block_handler import (
     CidrHandler,
     CidrListHandler,
 )
 from cloudshell.cp.aws.domain.services.ec2.subnet import get_subnet_reservation_name
@@ -371,19 +372,49 @@
                 self._aws_clients.ec2_session, self.vpc.vpc_id, sg_name
             )
             tags = TagsHandler.create_default_tags(sg_name, self._reservation)
             tags.add_tags_to_obj(sg)
             self._sg_service.set_subnet_sg_rules(sg)
 
 
+class PrepareSubnetsPredefinedNetworkingStrategy(PrepareSubnetsAbsStrategy):
+    def prepare(self) -> List["PrepareCloudInfraResult"]:
+        # we do not create subnets, add tags or route tables
+        action_items = list(map(ActionItem.from_action, self._subnet_actions))
+        for item in action_items:
+            subnet_id = get_subnet_id(item.action)
+            subnet = list(
+                self._aws_clients.ec2_session.subnets.filter(SubnetIds=[subnet_id])
+            )[0]
+            item.subnet = subnet
+
+        return list(map(self.create_result, action_items))
+
+    def _get_vpc(self):
+        pass
+
+    def _set_subnet_cidr(self, item: "ActionItem", is_multi_subnet_mode: bool):
+        pass
+
+    def _attach_route_table(self, item: "ActionItem"):
+        pass
+
+    def _connect_to_vgw(self, item: "ActionItem"):
+        pass
+
+    def _create_sg_for_subnet(self, item: "ActionItem"):
+        pass
+
+
 STRATEGIES = {
     VpcMode.DYNAMIC: PrepareSubnetsDynamicStrategy,
     VpcMode.STATIC: PrepareSubnetsStaticStrategy,
     VpcMode.SHARED: PrepareSubnetsSharedStrategy,
     VpcMode.SINGLE: PrepareSubnetsSingleStrategy,
+    VpcMode.PREDEFINED: PrepareSubnetsPredefinedNetworkingStrategy,
 }
 
 
 def get_prepare_subnet_strategy(
     vpc_service: "VPCService",
     subnet_service: "SubnetService",
     subnet_waiter: "SubnetWaiter",
@@ -392,16 +423,17 @@
     subnet_actions: List["PrepareSubnet"],
     aws_clients: "AwsApiClients",
     aws_model: "AWSEc2CloudProviderResourceModel",
     reservation: "ReservationModel",
     cancellation_context: "CancellationContext",
     logger: "Logger",
 ) -> PrepareSubnetsAbsStrategy:
+    strategy_class = STRATEGIES[aws_model.vpc_mode]
     # noinspection PyArgumentList
-    return STRATEGIES[aws_model.vpc_mode](  # pycharm fails to get correct params
+    return strategy_class(  # pycharm fails to get correct params
         vpc_service,
         subnet_service,
         subnet_waiter,
         cs_subnet_service,
         sg_service,
         cancellation_context,
         aws_model,
```

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/device_index.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/device_index.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/strategy/cleanup.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/strategy/cleanup.py`

 * *Files 5% similar despite different names*

```diff
@@ -325,32 +325,71 @@
             self.vpc, self._reservation_id
         )
 
     def _remove_vpc(self):
         """In the Single VPC mode we do not create the VPC."""
 
 
+class CleanupSandboxInfraPredefinedNetworkingStrategy(CleanupSandboxInfraAbsStrategy):
+    def cleanup(self):
+        # we remove only keys and instances
+        self.remove_keypair()
+        self.remove_security_groups()
+
+        if self._cleanup_exceptions:
+            raise CleanupSandboxInfraException(self._cleanup_exceptions)
+
+    def get_vpc(self) -> "Vpc":
+        pass
+
+    def _remove_instances(self):
+        pass
+
+    def _remove_igw(self):
+        pass
+
+    def _remove_security_groups(self):
+        pass
+
+    def _remove_subnets(self):
+        pass
+
+    def _remove_peerings(self):
+        pass
+
+    def _remove_blackhole_routes_mgt_vpc(self):
+        pass
+
+    def _remove_custom_route_tables(self):
+        pass
+
+    def _remove_vpc(self):
+        pass
+
+
 STRATEGIES = {
     VpcMode.DYNAMIC: CleanupSandboxInfraDynamicVpcStrategy,
     VpcMode.STATIC: CleanupSandboxInfraStaticVpcStrategy,
     VpcMode.SHARED: CleanupSandboxInfraSharedVpcStrategy,
     VpcMode.SINGLE: CleanupSandboxInfraSingleVpcStrategy,
+    VpcMode.PREDEFINED: CleanupSandboxInfraPredefinedNetworkingStrategy,
 }
 
 
 def get_strategy(
     vpc_service: "VPCService",
     key_pair_service: "KeyPairService",
     aws_clients: "AwsApiClients",
     aws_model: "AWSEc2CloudProviderResourceModel",
     reservation_id: "str",
     logger: "Logger",
 ) -> CleanupSandboxInfraAbsStrategy:
+    strategy_class = STRATEGIES[aws_model.vpc_mode]
     # noinspection PyArgumentList
-    return STRATEGIES[aws_model.vpc_mode](  # pycharm fails to get correct params
+    return strategy_class(  # pycharm fails to get correct params
         vpc_service,
         key_pair_service,
         aws_clients,
         aws_model,
         reservation_id,
         logger,
     )
```

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/session_providers/aws_session_provider.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/session_providers/aws_session_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,22 @@
         cloudshell_session: "CloudShellAPISession",
         aws_ec2_data_model: "AWSEc2CloudProviderResourceModel",
     ) -> AwsApiClients:
         default_session = self._get_aws_session(aws_ec2_data_model, cloudshell_session)
         if not default_session:
             raise ValueError("Could not create AWS Session")
 
-        if aws_ec2_data_model.vpc_mode is VpcMode.SHARED:
+        if aws_ec2_data_model.vpc_mode == VpcMode.SHARED:
+            aws_ec2_session = self._assume_shared_vpc_role(
+                default_session, aws_ec2_data_model
+            )
+        elif (
+            aws_ec2_data_model.vpc_mode == VpcMode.PREDEFINED
+            and aws_ec2_data_model.shared_vpc_role_arn
+        ):
             aws_ec2_session = self._assume_shared_vpc_role(
                 default_session, aws_ec2_data_model
             )
         else:
             aws_ec2_session = default_session
 
         return AwsApiClients(
```

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/security_group_parser.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/security_group_parser.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/aws_model_parser.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/aws_model_parser.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/command_results_parser.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/command_results_parser.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/port_group_attribute_parser.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/port_group_attribute_parser.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/parsers/custom_param_extractor.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/parsers/custom_param_extractor.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/s3/bucket.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/s3/bucket.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/instance.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/instance.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/vpc.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/vpc.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/password.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/password.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import os
 import time
 from multiprocessing import TimeoutError
 
 
 class PasswordWaiter:
-    def __init__(self, cancellation_service, delay=5, timeout=15):
+    TIMEOUT = int(os.getenv("QS_AWS_CRED_TIMEOUT", "15"))
+
+    def __init__(self, cancellation_service, delay=5, timeout=TIMEOUT):
         """# noqa
         :param delay: the time in seconds between each pull
         :type delay: int
         :param timeout: timeout in minutes until time out exception will raised
         :type timeout: int
         :param cancellation_service:
         :type cancellation_service: cloudshell.cp.aws.domain.common.cancellation_service.CommandCancellationService
```

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/subnet.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/subnet.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/waiters/ami.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/waiters/ami.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/network_interface.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/network_interface.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/elastic_ip.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/elastic_ip.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/instance.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/instance.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/instance_credentials.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/instance_credentials.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/vpc.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/vpc.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/mirroring.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/mirroring.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/subnet.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/subnet.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/ebs.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/ebs.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/security_group.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/security_group.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/ec2/keypair.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/ec2/keypair.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/cloudshell/traffic_mirror_pool_services.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/cloudshell/traffic_mirror_pool_services.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/services/cloudshell/cs_subnet_service.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/services/cloudshell/cs_subnet_service.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/traffic_mirror_cleaner.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/traffic_mirror_cleaner.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/traffic_mirroring_operation.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/traffic_mirroring_operation.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/cleanup.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/cleanup.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/conncetivity/operations/prepare.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/conncetivity/operations/prepare.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,35 @@
-from typing import TYPE_CHECKING, List
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
 import attr
 import jsonpickle
 
 from cloudshell.cp.core.models import (
     ActionResultBase,
     CreateKeys,
     CreateKeysActionResult,
     PrepareCloudInfra,
     PrepareCloudInfraResult,
     PrepareSubnet,
     RequestActionBase,
 )
 
+from cloudshell.cp.aws.common.subnet_service import SubnetServiceAttr, get_subnet_id
 from cloudshell.cp.aws.domain.services.strategy.prepare_cloud_infra import (
     get_prepare_infra_strategy,
 )
 from cloudshell.cp.aws.domain.services.strategy.prepare_subnets import (
     get_prepare_subnet_strategy,
 )
+from cloudshell.cp.aws.models.aws_ec2_cloud_provider_resource_model import (
+    AWSEc2CloudProviderResourceModel,
+    VpcMode,
+)
 
 if TYPE_CHECKING:
     from logging import Logger
 
     from mypy_boto3_ec2 import EC2ServiceResource  # noqa: I900
     from mypy_boto3_s3 import S3ServiceResource  # noqa: I900
 
@@ -35,53 +42,52 @@
     from cloudshell.cp.aws.domain.services.ec2.security_group import (
         SecurityGroupService,
     )
     from cloudshell.cp.aws.domain.services.ec2.subnet import SubnetService
     from cloudshell.cp.aws.domain.services.ec2.vpc import VPCService
     from cloudshell.cp.aws.domain.services.waiters.subnet import SubnetWaiter
     from cloudshell.cp.aws.models.aws_api import AwsApiClients
-    from cloudshell.cp.aws.models.aws_ec2_cloud_provider_resource_model import (
-        AWSEc2CloudProviderResourceModel,
-    )
     from cloudshell.cp.aws.models.reservation_model import ReservationModel
 
 
 @attr.s(auto_attribs=True)
 class PrepareSandboxInfraOperation:
-    vpc_service: "VPCService"
-    security_group_service: "SecurityGroupService"
-    key_pair_service: "KeyPairService"
-    subnet_service: "SubnetService"
-    subnet_waiter: "SubnetWaiter"
+    vpc_service: VPCService
+    security_group_service: SecurityGroupService
+    key_pair_service: KeyPairService
+    subnet_service: SubnetService
+    subnet_waiter: SubnetWaiter
 
     def prepare_connectivity(
         self,
-        aws_clients: "AwsApiClients",
-        reservation: "ReservationModel",
-        aws_model: "AWSEc2CloudProviderResourceModel",
-        actions: List["RequestActionBase"],
-        cancellation_context: "CancellationContext",
-        cs_subnet_service: "CsSubnetService",
-        logger: "Logger",
+        aws_clients: AwsApiClients,
+        reservation: ReservationModel,
+        aws_model: AWSEc2CloudProviderResourceModel,
+        actions: list[RequestActionBase],
+        cancellation_context: CancellationContext,
+        cs_subnet_service: CsSubnetService,
+        logger: Logger,
     ):
         actions_str = ",".join([jsonpickle.encode(a) for a in actions])
         logger.info(f"PrepareSandboxInfra actions: {actions_str}")
         results = []
 
         # Execute PrepareCloudInfra action first
         network_action = next(
             (a for a in actions if isinstance(a, PrepareCloudInfra)), None
         )
         create_keys_action = next(
             (a for a in actions if isinstance(a, CreateKeys)), None
         )
+        subnet_actions = [a for a in actions if isinstance(a, PrepareSubnet)]
         if not network_action:
             raise ValueError("Actions list must contain a PrepareCloudInfraAction.")
         if not create_keys_action:
             raise ValueError("Actions list must contain a CreateKeys.")
+        self._validate_subnet_actions(subnet_actions, aws_model)
 
         try:
             result = self._prepare_network(
                 aws_clients,
                 reservation,
                 aws_model,
                 network_action,
@@ -103,15 +109,14 @@
             )
             results.append(result)
         except Exception as e:
             logger.exception("Error in prepare key.")
             results.append(self._create_fault_action_result(create_keys_action, e))
 
         # Execute prepareSubnet actions
-        subnet_actions = [a for a in actions if isinstance(a, PrepareSubnet)]
         try:
             subnet_results = self._prepare_subnets(
                 cs_subnet_service,
                 subnet_actions,
                 aws_clients,
                 aws_model,
                 reservation,
@@ -125,54 +130,54 @@
                 results.append(self._create_fault_action_result(action, e))
 
         logger.info("Prepare Connectivity completed")
         return results
 
     def _prepare_key(
         self,
-        aws_clients: "AwsApiClients",
-        aws_model: "AWSEc2CloudProviderResourceModel",
-        reservation: "ReservationModel",
-        action: "CreateKeys",
-        logger: "Logger",
+        aws_clients: AwsApiClients,
+        aws_model: AWSEc2CloudProviderResourceModel,
+        reservation: ReservationModel,
+        action: CreateKeys,
+        logger: Logger,
     ):
         logger.info("Get or create existing key pair")
         access_key = self._get_or_create_key_pair(
             ec2_session=aws_clients.ec2_session,
             s3_session=aws_clients.s3_session,
             bucket=aws_model.key_pairs_location,
             reservation_id=reservation.reservation_id,
         )
         return self._create_prepare_create_keys_result(action, access_key)
 
     def _prepare_network(
         self,
-        aws_clients: "AwsApiClients",
-        reservation: "ReservationModel",
-        aws_model: "AWSEc2CloudProviderResourceModel",
-        action: "PrepareCloudInfra",
-        cancellation_context: "CancellationContext",
-        logger: "Logger",
-    ) -> "PrepareCloudInfraResult":
+        aws_clients: AwsApiClients,
+        reservation: ReservationModel,
+        aws_model: AWSEc2CloudProviderResourceModel,
+        action: PrepareCloudInfra,
+        cancellation_context: CancellationContext,
+        logger: Logger,
+    ) -> PrepareCloudInfraResult:
         strategy = get_prepare_infra_strategy(
             self.vpc_service,
             self.security_group_service,
             aws_clients,
             aws_model,
             reservation,
             action,
             cancellation_context,
             logger,
         )
         return strategy.prepare()
 
     def _get_or_create_key_pair(
         self,
-        ec2_session: "EC2ServiceResource",
-        s3_session: "S3ServiceResource",
+        ec2_session: EC2ServiceResource,
+        s3_session: S3ServiceResource,
         bucket: str,
         reservation_id: str,
     ) -> str:
         """Creates a keypair or retrieves an existing and returns the private key."""
         private_key = self.key_pair_service.load_key_pair_by_name(
             s3_session=s3_session, bucket_name=bucket, reservation_id=reservation_id
         )
@@ -185,22 +190,22 @@
             )
             private_key = key_pair.key_material
 
         return private_key
 
     def _prepare_subnets(
         self,
-        cs_subnet_service: "CsSubnetService",
-        subnet_actions: List["PrepareSubnet"],
-        aws_clients: "AwsApiClients",
-        aws_models: "AWSEc2CloudProviderResourceModel",
-        reservation: "ReservationModel",
-        cancellation_context: "CancellationContext",
-        logger: "Logger",
-    ) -> List["PrepareCloudInfraResult"]:
+        cs_subnet_service: CsSubnetService,
+        subnet_actions: list[PrepareSubnet],
+        aws_clients: AwsApiClients,
+        aws_models: AWSEc2CloudProviderResourceModel,
+        reservation: ReservationModel,
+        cancellation_context: CancellationContext,
+        logger: Logger,
+    ) -> list[PrepareCloudInfraResult]:
         strategy = get_prepare_subnet_strategy(
             self.vpc_service,
             self.subnet_service,
             self.subnet_waiter,
             cs_subnet_service,
             self.security_group_service,
             subnet_actions,
@@ -225,7 +230,19 @@
     @staticmethod
     def _create_fault_action_result(action, e):
         action_result = ActionResultBase()
         action_result.actionId = action.actionId
         action_result.success = False
         action_result.errorMessage = f"PrepareSandboxInfra ended with the error: {e}"
         return action_result
+
+    @staticmethod
+    def _validate_subnet_actions(
+        subnet_actions: list[PrepareSubnet],
+        aws_model: AWSEc2CloudProviderResourceModel,
+    ) -> None:
+        if aws_model.vpc_mode is VpcMode.PREDEFINED and not all(
+            map(get_subnet_id, subnet_actions)
+        ):
+            mode = aws_model.vpc_mode.PREDEFINED.value
+            attr_ = SubnetServiceAttr.SUBNET_ID.value
+            raise ValueError(f"In {mode} VPC mode, all subnets must have {attr_} set.")
```

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/operations/vm_details_operation.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/operations/vm_details_operation.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/operations/set_app_security_groups.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/operations/set_app_security_groups.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/deployed_app/operations/app_ports_operation.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/deployed_app/operations/app_ports_operation.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/route_table_handler.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/route_table_handler.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/cidr_block_handler.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/cidr_block_handler.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/tags_handler.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/tags_handler.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/route_handler.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/route_handler.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/cloudshell/cp/aws/domain/handlers/ec2/vpc_peering_handler.py` & `cloudshell-cp-aws-3.5.0/cloudshell/cp/aws/domain/handlers/ec2/vpc_peering_handler.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/conftest.py` & `cloudshell-cp-aws-3.5.0/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_aws_shell.py` & `cloudshell-cp-aws-3.5.0/tests/test_aws_shell.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/base.py` & `cloudshell-cp-aws-3.5.0/tests/base.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_connectivity/test_prepare_connectivity.py` & `cloudshell-cp-aws-3.5.0/tests/test_connectivity/test_prepare_connectivity.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_connectivity/test_cleanup_connectivity.py` & `cloudshell-cp-aws-3.5.0/tests/test_connectivity/test_cleanup_connectivity.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_connectivity/test_create_traffic_mirroring.py` & `cloudshell-cp-aws-3.5.0/tests/test_connectivity/test_create_traffic_mirroring.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/test_power_operation.py` & `cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/test_power_operation.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/test_deploy_operation.py` & `cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/test_deploy_operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,14 +496,15 @@
         ec2_session = Mock()
         ec2_session.Image = Mock(return_value=image)
         ami_model = Mock()
         ami_model.aws_ami_id = "asd"
         ami_model.storage_size = "0"
         ami_model.iam_role = ""
         ami_model.custom_tags = ""
+        ami_model.static_sg_id = ""
 
         network_actions = None
         vpc = Mock()
         self.deploy_operation._get_block_device_mappings = Mock()
 
         aws_model = self.deploy_operation._create_deployment_parameters(
             ec2_session=ec2_session,
```

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/test_delete_operation.py` & `cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/test_delete_operation.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_ami_management/test_operations/test_refresh_ip_operation.py` & `cloudshell-cp-aws-3.5.0/tests/test_ami_management/test_operations/test_refresh_ip_operation.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_deployed_app/test_operations/test_access_key_operation.py` & `cloudshell-cp-aws-3.5.0/tests/test_deployed_app/test_operations/test_access_key_operation.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_deployed_app/test_operations/test_set_app_security_groups_operation.py` & `cloudshell-cp-aws-3.5.0/tests/test_deployed_app/test_operations/test_set_app_security_groups_operation.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_deployed_app/test_operations/test_app_ports_operation.py` & `cloudshell-cp-aws-3.5.0/tests/test_deployed_app/test_operations/test_app_ports_operation.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_key_pair.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_key_pair.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_vpc.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_vpc.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_elastic_ip.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_elastic_ip.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_vm_custom_params_extractor.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_vm_custom_params_extractor.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_port_group_attribute_parser.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_port_group_attribute_parser.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_network_interface_service.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_network_interface_service.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_session_provider.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_session_provider.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_subnet.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_subnet.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_ami_waiter.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_ami_waiter.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_model_parser.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_model_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,19 @@
                 "type": "attribute",
             },
             {
                 "attributeName": f"{d_path}.Status Check Timeout",
                 "attributeValue": "100",
                 "type": "attribute",
             },
+            {
+                "attributeName": f"{d_path}.Static Security Group Id",
+                "attributeValue": "",
+                "type": "attribute",
+            },
         ]
         json_str = json.dumps(
             {
                 "driverRequest": {
                     "actions": [
                         {
                             "actionParams": {
```

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_security_groups.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_security_groups.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_instance_waiter.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_instance_waiter.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_ami_creds_service.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_ami_creds_service.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_device_index_strategy.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_device_index_strategy.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_vpc_waiter.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_vpc_waiter.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_instance_service.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_instance_service.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_subnet_waiter.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_subnet_waiter.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_bucket.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_bucket.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_domain_services/test_password_waiter.py` & `cloudshell-cp-aws-3.5.0/tests/test_domain_services/test_password_waiter.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_common/test_cancellation_service.py` & `cloudshell-cp-aws-3.5.0/tests/test_common/test_cancellation_service.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_common/test_get_vm_details.py` & `cloudshell-cp-aws-3.5.0/tests/test_common/test_get_vm_details.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_common/test_converters.py` & `cloudshell-cp-aws-3.5.0/tests/test_common/test_converters.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/test_common/test_vm_details_provider.py` & `cloudshell-cp-aws-3.5.0/tests/test_common/test_vm_details_provider.py`

 * *Files identical despite different names*

## Comparing `cloudshell-cp-aws-3.4.0/tests/handlers/test_route_table_handler.py` & `cloudshell-cp-aws-3.5.0/tests/handlers/test_route_table_handler.py`

 * *Files identical despite different names*

