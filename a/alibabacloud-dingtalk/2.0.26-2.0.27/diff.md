# Comparing `tmp/alibabacloud_dingtalk-2.0.26.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.26.tar", last modified: Fri Jul 21 10:56:53 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.27.tar", last modified: Wed Jul 26 02:26:48 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.26.tar` & `alibabacloud_dingtalk-2.0.27.tar`

### file list

```diff
@@ -1,381 +1,381 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/
--rw-r--r--   0 root         (0) root         (0)    20337 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8552 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15385 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27728 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90914 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   139242 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   165948 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   323041 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   205984 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   590436 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9614 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10132 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142048 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   346941 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39942 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   106288 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10446 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   126888 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   172646 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   297108 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   392984 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23872 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33155 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223914 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   552073 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13874 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16265 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    57073 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    75811 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   219916 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   278738 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269893 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   472940 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   731141 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8259 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8976 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   316592 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   439557 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13914 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21801 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4633 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4901 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    95111 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   139534 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302740 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   379213 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22430 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31875 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   610684 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   859772 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9852 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14366 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148979 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   177099 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   264898 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   419073 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8048 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    12289 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94300 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   106806 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53470 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89290 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148231 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19158 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32757 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130783 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32014 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    34941 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   179772 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   377816 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4490 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12583 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-21 10:56:53.000000 alibabacloud_dingtalk-2.0.26/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2023-07-21 10:56:52.000000 alibabacloud_dingtalk-2.0.26/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/
+-rw-r--r--   0 root         (0) root         (0)    20402 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15385 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27728 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90914 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   139242 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   165948 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   323041 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   205984 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   590436 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9614 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10132 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142048 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   346941 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39942 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   106288 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10446 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126888 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   172646 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297108 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   392984 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23872 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33155 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223914 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   552073 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16265 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    57073 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    75811 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   219916 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   278738 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269893 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   472940 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   731141 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8259 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8976 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   316592 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   439557 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13914 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21801 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4901 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    97319 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   141560 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302740 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   379213 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24693 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33901 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   610684 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   859772 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9852 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14366 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148979 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   177099 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   264898 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   419073 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    12289 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94300 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   106806 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65686 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92278 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   381194 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   542779 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53470 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89290 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148231 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19158 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32757 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130783 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32014 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    34941 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179772 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   377816 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4490 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12583 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2023-07-26 02:26:48.000000 alibabacloud_dingtalk-2.0.27/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.26/ChangeLog.md` & `alibabacloud_dingtalk-2.0.27/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-21 Version: 2.0.26
+- Update AddOfficialAccountFollower.
+
 2023-07-19 Version: 2.0.25
 - Update AddOfficialAccountFollower.
 
 2023-07-17 Version: 2.0.24
 - Update AddOfficialAccountFollower.
 
 2023-07-12 Version: 2.0.23
```

### Comparing `alibabacloud_dingtalk-2.0.26/LICENSE` & `alibabacloud_dingtalk-2.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/PKG-INFO` & `alibabacloud_dingtalk-2.0.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.26
+Version: 2.0.27
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.26/README-CN.md` & `alibabacloud_dingtalk-2.0.27/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/README.md` & `alibabacloud_dingtalk-2.0.27/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,72 @@
         return self.device_market_manager_with_options(headers, runtime)
 
     async def device_market_manager_async(self) -> dingtalkhrm__1__0_models.DeviceMarketManagerResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.device_market_manager_with_options_async(headers, runtime)
 
+    def device_market_order_manager_with_options(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkhrm__1__0_models.DeviceMarketOrderManagerResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='DeviceMarketOrderManager',
+            version='hrm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/hrm/device/market/order/manager',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkhrm__1__0_models.DeviceMarketOrderManagerResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def device_market_order_manager_with_options_async(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkhrm__1__0_models.DeviceMarketOrderManagerResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='DeviceMarketOrderManager',
+            version='hrm_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/hrm/device/market/order/manager',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkhrm__1__0_models.DeviceMarketOrderManagerResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def device_market_order_manager(self) -> dingtalkhrm__1__0_models.DeviceMarketOrderManagerResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.device_market_order_manager_with_options(headers, runtime)
+
+    async def device_market_order_manager_async(self) -> dingtalkhrm__1__0_models.DeviceMarketOrderManagerResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.device_market_order_manager_with_options_async(headers, runtime)
+
     def e_cert_query_with_options(
         self,
         request: dingtalkhrm__1__0_models.ECertQueryRequest,
         headers: dingtalkhrm__1__0_models.ECertQueryHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkhrm__1__0_models.ECertQueryResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,14 +355,85 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeviceMarketManagerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeviceMarketOrderManagerResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class DeviceMarketOrderManagerResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeviceMarketOrderManagerResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeviceMarketOrderManagerResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ECertQueryHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.core import TeaCore
+from typing import Dict
 
 from alibabacloud_gateway_spi.client import Client as SPIClient
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
 from alibabacloud_gateway_dingtalk.client import Client as GatewayClientClient
 from alibabacloud_tea_util.client import Client as UtilClient
 from alibabacloud_dingtalk.im_2_0 import models as dingtalkim__2__0_models
@@ -21,14 +22,15 @@
     def __init__(
         self, 
         config: open_api_models.Config,
     ):
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
+        self._signature_algorithm = 'v2'
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
     def close_topbox_with_options(
         self,
         request: dingtalkim__2__0_models.CloseTopboxRequest,
@@ -488,7 +490,65 @@
     async def create_topbox_async(
         self,
         request: dingtalkim__2__0_models.CreateTopboxRequest,
     ) -> dingtalkim__2__0_models.CreateTopboxResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkim__2__0_models.CreateTopboxHeaders()
         return await self.create_topbox_with_options_async(request, headers, runtime)
+
+    def group_manager_device_market_with_options(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__2__0_models.GroupManagerDeviceMarketResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='GroupManagerDeviceMarket',
+            version='im_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/im/group/device/market/manager',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__2__0_models.GroupManagerDeviceMarketResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def group_manager_device_market_with_options_async(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__2__0_models.GroupManagerDeviceMarketResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='GroupManagerDeviceMarket',
+            version='im_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/im/group/device/market/manager',
+            method='GET',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__2__0_models.GroupManagerDeviceMarketResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def group_manager_device_market(self) -> dingtalkim__2__0_models.GroupManagerDeviceMarketResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.group_manager_device_market_with_options(headers, runtime)
+
+    async def group_manager_device_market_async(self) -> dingtalkim__2__0_models.GroupManagerDeviceMarketResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.group_manager_device_market_with_options_async(headers, runtime)
```

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -965,7 +965,78 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateTopboxResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GroupManagerDeviceMarketResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class GroupManagerDeviceMarketResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GroupManagerDeviceMarketResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GroupManagerDeviceMarketResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1063,14 +1063,202 @@
         self,
         request: dingtalkrooms__1__0_models.QueryMeetingRoomListRequest,
     ) -> dingtalkrooms__1__0_models.QueryMeetingRoomListResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkrooms__1__0_models.QueryMeetingRoomListHeaders()
         return await self.query_meeting_room_list_with_options_async(request, headers, runtime)
 
+    def remove_super_user_meeting_room_with_options(
+        self,
+        request: dingtalkrooms__1__0_models.RemoveSuperUserMeetingRoomRequest,
+        headers: dingtalkrooms__1__0_models.RemoveSuperUserMeetingRoomHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkrooms__1__0_models.RemoveSuperUserMeetingRoomResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.room_id):
+            query['roomId'] = request.room_id
+        if not UtilClient.is_unset(request.union_id):
+            query['unionId'] = request.union_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RemoveSuperUserMeetingRoom',
+            version='rooms_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/rooms/meetingRooms/superUsers/remove',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkrooms__1__0_models.RemoveSuperUserMeetingRoomResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def remove_super_user_meeting_room_with_options_async(
+        self,
+        request: dingtalkrooms__1__0_models.RemoveSuperUserMeetingRoomRequest,
+        headers: dingtalkrooms__1__0_models.RemoveSuperUserMeetingRoomHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkrooms__1__0_models.RemoveSuperUserMeetingRoomResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.room_id):
+            query['roomId'] = request.room_id
+        if not UtilClient.is_unset(request.union_id):
+            query['unionId'] = request.union_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RemoveSuperUserMeetingRoom',
+            version='rooms_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/rooms/meetingRooms/superUsers/remove',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkrooms__1__0_models.RemoveSuperUserMeetingRoomResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def remove_super_user_meeting_room(
+        self,
+        request: dingtalkrooms__1__0_models.RemoveSuperUserMeetingRoomRequest,
+    ) -> dingtalkrooms__1__0_models.RemoveSuperUserMeetingRoomResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkrooms__1__0_models.RemoveSuperUserMeetingRoomHeaders()
+        return self.remove_super_user_meeting_room_with_options(request, headers, runtime)
+
+    async def remove_super_user_meeting_room_async(
+        self,
+        request: dingtalkrooms__1__0_models.RemoveSuperUserMeetingRoomRequest,
+    ) -> dingtalkrooms__1__0_models.RemoveSuperUserMeetingRoomResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkrooms__1__0_models.RemoveSuperUserMeetingRoomHeaders()
+        return await self.remove_super_user_meeting_room_with_options_async(request, headers, runtime)
+
+    def set_super_user_meeting_room_with_options(
+        self,
+        request: dingtalkrooms__1__0_models.SetSuperUserMeetingRoomRequest,
+        headers: dingtalkrooms__1__0_models.SetSuperUserMeetingRoomHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkrooms__1__0_models.SetSuperUserMeetingRoomResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.dept_id_white_list):
+            body['deptIdWhiteList'] = request.dept_id_white_list
+        if not UtilClient.is_unset(request.room_id):
+            body['roomId'] = request.room_id
+        if not UtilClient.is_unset(request.union_id):
+            body['unionId'] = request.union_id
+        if not UtilClient.is_unset(request.user_id_white_list):
+            body['userIdWhiteList'] = request.user_id_white_list
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SetSuperUserMeetingRoom',
+            version='rooms_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/rooms/meetingRooms/superUsers/set',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkrooms__1__0_models.SetSuperUserMeetingRoomResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def set_super_user_meeting_room_with_options_async(
+        self,
+        request: dingtalkrooms__1__0_models.SetSuperUserMeetingRoomRequest,
+        headers: dingtalkrooms__1__0_models.SetSuperUserMeetingRoomHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkrooms__1__0_models.SetSuperUserMeetingRoomResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.dept_id_white_list):
+            body['deptIdWhiteList'] = request.dept_id_white_list
+        if not UtilClient.is_unset(request.room_id):
+            body['roomId'] = request.room_id
+        if not UtilClient.is_unset(request.union_id):
+            body['unionId'] = request.union_id
+        if not UtilClient.is_unset(request.user_id_white_list):
+            body['userIdWhiteList'] = request.user_id_white_list
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SetSuperUserMeetingRoom',
+            version='rooms_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/rooms/meetingRooms/superUsers/set',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkrooms__1__0_models.SetSuperUserMeetingRoomResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def set_super_user_meeting_room(
+        self,
+        request: dingtalkrooms__1__0_models.SetSuperUserMeetingRoomRequest,
+    ) -> dingtalkrooms__1__0_models.SetSuperUserMeetingRoomResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkrooms__1__0_models.SetSuperUserMeetingRoomHeaders()
+        return self.set_super_user_meeting_room_with_options(request, headers, runtime)
+
+    async def set_super_user_meeting_room_async(
+        self,
+        request: dingtalkrooms__1__0_models.SetSuperUserMeetingRoomRequest,
+    ) -> dingtalkrooms__1__0_models.SetSuperUserMeetingRoomResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkrooms__1__0_models.SetSuperUserMeetingRoomHeaders()
+        return await self.set_super_user_meeting_room_with_options_async(request, headers, runtime)
+
     def update_meeting_room_with_options(
         self,
         request: dingtalkrooms__1__0_models.UpdateMeetingRoomRequest,
         headers: dingtalkrooms__1__0_models.UpdateMeetingRoomHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkrooms__1__0_models.UpdateMeetingRoomResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2349,14 +2349,300 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryMeetingRoomListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RemoveSuperUserMeetingRoomHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class RemoveSuperUserMeetingRoomRequest(TeaModel):
+    def __init__(
+        self,
+        room_id: str = None,
+        union_id: str = None,
+    ):
+        self.room_id = room_id
+        self.union_id = union_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.room_id is not None:
+            result['roomId'] = self.room_id
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('roomId') is not None:
+            self.room_id = m.get('roomId')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        return self
+
+
+class RemoveSuperUserMeetingRoomResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class RemoveSuperUserMeetingRoomResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: RemoveSuperUserMeetingRoomResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = RemoveSuperUserMeetingRoomResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SetSuperUserMeetingRoomHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SetSuperUserMeetingRoomRequest(TeaModel):
+    def __init__(
+        self,
+        dept_id_white_list: List[int] = None,
+        room_id: str = None,
+        union_id: str = None,
+        user_id_white_list: List[str] = None,
+    ):
+        self.dept_id_white_list = dept_id_white_list
+        self.room_id = room_id
+        self.union_id = union_id
+        self.user_id_white_list = user_id_white_list
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dept_id_white_list is not None:
+            result['deptIdWhiteList'] = self.dept_id_white_list
+        if self.room_id is not None:
+            result['roomId'] = self.room_id
+        if self.union_id is not None:
+            result['unionId'] = self.union_id
+        if self.user_id_white_list is not None:
+            result['userIdWhiteList'] = self.user_id_white_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('deptIdWhiteList') is not None:
+            self.dept_id_white_list = m.get('deptIdWhiteList')
+        if m.get('roomId') is not None:
+            self.room_id = m.get('roomId')
+        if m.get('unionId') is not None:
+            self.union_id = m.get('unionId')
+        if m.get('userIdWhiteList') is not None:
+            self.user_id_white_list = m.get('userIdWhiteList')
+        return self
+
+
+class SetSuperUserMeetingRoomResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class SetSuperUserMeetingRoomResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SetSuperUserMeetingRoomResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SetSuperUserMeetingRoomResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateMeetingRoomHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1219,14 +1219,128 @@
         self,
         request: dingtalkservice_group__1__0_models.BatchGetGroupSetConfigRequest,
     ) -> dingtalkservice_group__1__0_models.BatchGetGroupSetConfigResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkservice_group__1__0_models.BatchGetGroupSetConfigHeaders()
         return await self.batch_get_group_set_config_with_options_async(request, headers, runtime)
 
+    def batch_query_customer_send_task_with_options(
+        self,
+        request: dingtalkservice_group__1__0_models.BatchQueryCustomerSendTaskRequest,
+        headers: dingtalkservice_group__1__0_models.BatchQueryCustomerSendTaskHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkservice_group__1__0_models.BatchQueryCustomerSendTaskResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.gmt_create_end):
+            body['gmtCreateEnd'] = request.gmt_create_end
+        if not UtilClient.is_unset(request.gmt_create_start):
+            body['gmtCreateStart'] = request.gmt_create_start
+        if not UtilClient.is_unset(request.max_results):
+            body['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.need_rich_statistics):
+            body['needRichStatistics'] = request.need_rich_statistics
+        if not UtilClient.is_unset(request.next_token):
+            body['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.open_batch_task_ids):
+            body['openBatchTaskIds'] = request.open_batch_task_ids
+        if not UtilClient.is_unset(request.open_team_id):
+            body['openTeamId'] = request.open_team_id
+        if not UtilClient.is_unset(request.task_name):
+            body['taskName'] = request.task_name
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='BatchQueryCustomerSendTask',
+            version='serviceGroup_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/serviceGroup/customers/tasks/batchQuery',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkservice_group__1__0_models.BatchQueryCustomerSendTaskResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def batch_query_customer_send_task_with_options_async(
+        self,
+        request: dingtalkservice_group__1__0_models.BatchQueryCustomerSendTaskRequest,
+        headers: dingtalkservice_group__1__0_models.BatchQueryCustomerSendTaskHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkservice_group__1__0_models.BatchQueryCustomerSendTaskResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.gmt_create_end):
+            body['gmtCreateEnd'] = request.gmt_create_end
+        if not UtilClient.is_unset(request.gmt_create_start):
+            body['gmtCreateStart'] = request.gmt_create_start
+        if not UtilClient.is_unset(request.max_results):
+            body['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.need_rich_statistics):
+            body['needRichStatistics'] = request.need_rich_statistics
+        if not UtilClient.is_unset(request.next_token):
+            body['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.open_batch_task_ids):
+            body['openBatchTaskIds'] = request.open_batch_task_ids
+        if not UtilClient.is_unset(request.open_team_id):
+            body['openTeamId'] = request.open_team_id
+        if not UtilClient.is_unset(request.task_name):
+            body['taskName'] = request.task_name
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='BatchQueryCustomerSendTask',
+            version='serviceGroup_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/serviceGroup/customers/tasks/batchQuery',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkservice_group__1__0_models.BatchQueryCustomerSendTaskResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def batch_query_customer_send_task(
+        self,
+        request: dingtalkservice_group__1__0_models.BatchQueryCustomerSendTaskRequest,
+    ) -> dingtalkservice_group__1__0_models.BatchQueryCustomerSendTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkservice_group__1__0_models.BatchQueryCustomerSendTaskHeaders()
+        return self.batch_query_customer_send_task_with_options(request, headers, runtime)
+
+    async def batch_query_customer_send_task_async(
+        self,
+        request: dingtalkservice_group__1__0_models.BatchQueryCustomerSendTaskRequest,
+    ) -> dingtalkservice_group__1__0_models.BatchQueryCustomerSendTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkservice_group__1__0_models.BatchQueryCustomerSendTaskHeaders()
+        return await self.batch_query_customer_send_task_with_options_async(request, headers, runtime)
+
     def batch_query_group_member_with_options(
         self,
         request: dingtalkservice_group__1__0_models.BatchQueryGroupMemberRequest,
         headers: dingtalkservice_group__1__0_models.BatchQueryGroupMemberHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkservice_group__1__0_models.BatchQueryGroupMemberResponse:
         UtilClient.validate_model(request)
@@ -2907,14 +3021,116 @@
         self,
         request: dingtalkservice_group__1__0_models.CreateTicketRequest,
     ) -> dingtalkservice_group__1__0_models.CreateTicketResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkservice_group__1__0_models.CreateTicketHeaders()
         return await self.create_ticket_with_options_async(request, headers, runtime)
 
+    def customer_send_msg_task_with_options(
+        self,
+        request: dingtalkservice_group__1__0_models.CustomerSendMsgTaskRequest,
+        headers: dingtalkservice_group__1__0_models.CustomerSendMsgTaskHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkservice_group__1__0_models.CustomerSendMsgTaskResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.message_content):
+            body['messageContent'] = request.message_content
+        if not UtilClient.is_unset(request.open_team_id):
+            body['openTeamId'] = request.open_team_id
+        if not UtilClient.is_unset(request.query_customer):
+            body['queryCustomer'] = request.query_customer
+        if not UtilClient.is_unset(request.send_config):
+            body['sendConfig'] = request.send_config
+        if not UtilClient.is_unset(request.task_name):
+            body['taskName'] = request.task_name
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CustomerSendMsgTask',
+            version='serviceGroup_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/serviceGroup/customers/tasks/send',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkservice_group__1__0_models.CustomerSendMsgTaskResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def customer_send_msg_task_with_options_async(
+        self,
+        request: dingtalkservice_group__1__0_models.CustomerSendMsgTaskRequest,
+        headers: dingtalkservice_group__1__0_models.CustomerSendMsgTaskHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkservice_group__1__0_models.CustomerSendMsgTaskResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.message_content):
+            body['messageContent'] = request.message_content
+        if not UtilClient.is_unset(request.open_team_id):
+            body['openTeamId'] = request.open_team_id
+        if not UtilClient.is_unset(request.query_customer):
+            body['queryCustomer'] = request.query_customer
+        if not UtilClient.is_unset(request.send_config):
+            body['sendConfig'] = request.send_config
+        if not UtilClient.is_unset(request.task_name):
+            body['taskName'] = request.task_name
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CustomerSendMsgTask',
+            version='serviceGroup_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/serviceGroup/customers/tasks/send',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkservice_group__1__0_models.CustomerSendMsgTaskResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def customer_send_msg_task(
+        self,
+        request: dingtalkservice_group__1__0_models.CustomerSendMsgTaskRequest,
+    ) -> dingtalkservice_group__1__0_models.CustomerSendMsgTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkservice_group__1__0_models.CustomerSendMsgTaskHeaders()
+        return self.customer_send_msg_task_with_options(request, headers, runtime)
+
+    async def customer_send_msg_task_async(
+        self,
+        request: dingtalkservice_group__1__0_models.CustomerSendMsgTaskRequest,
+    ) -> dingtalkservice_group__1__0_models.CustomerSendMsgTaskResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkservice_group__1__0_models.CustomerSendMsgTaskHeaders()
+        return await self.customer_send_msg_task_with_options_async(request, headers, runtime)
+
     def delete_group_members_from_group_with_options(
         self,
         request: dingtalkservice_group__1__0_models.DeleteGroupMembersFromGroupRequest,
         headers: dingtalkservice_group__1__0_models.DeleteGroupMembersFromGroupHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkservice_group__1__0_models.DeleteGroupMembersFromGroupResponse:
         UtilClient.validate_model(request)
@@ -4805,14 +5021,116 @@
         self,
         request: dingtalkservice_group__1__0_models.QueryCustomerCardRequest,
     ) -> dingtalkservice_group__1__0_models.QueryCustomerCardResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkservice_group__1__0_models.QueryCustomerCardHeaders()
         return await self.query_customer_card_with_options_async(request, headers, runtime)
 
+    def query_customer_task_user_detail_with_options(
+        self,
+        request: dingtalkservice_group__1__0_models.QueryCustomerTaskUserDetailRequest,
+        headers: dingtalkservice_group__1__0_models.QueryCustomerTaskUserDetailHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkservice_group__1__0_models.QueryCustomerTaskUserDetailResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.max_results):
+            body['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            body['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.open_batch_task_id):
+            body['openBatchTaskId'] = request.open_batch_task_id
+        if not UtilClient.is_unset(request.open_team_id):
+            body['openTeamId'] = request.open_team_id
+        if not UtilClient.is_unset(request.receiver_union_ids):
+            body['receiverUnionIds'] = request.receiver_union_ids
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='QueryCustomerTaskUserDetail',
+            version='serviceGroup_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/serviceGroup/customers/tasks/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkservice_group__1__0_models.QueryCustomerTaskUserDetailResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def query_customer_task_user_detail_with_options_async(
+        self,
+        request: dingtalkservice_group__1__0_models.QueryCustomerTaskUserDetailRequest,
+        headers: dingtalkservice_group__1__0_models.QueryCustomerTaskUserDetailHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkservice_group__1__0_models.QueryCustomerTaskUserDetailResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.max_results):
+            body['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            body['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.open_batch_task_id):
+            body['openBatchTaskId'] = request.open_batch_task_id
+        if not UtilClient.is_unset(request.open_team_id):
+            body['openTeamId'] = request.open_team_id
+        if not UtilClient.is_unset(request.receiver_union_ids):
+            body['receiverUnionIds'] = request.receiver_union_ids
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='QueryCustomerTaskUserDetail',
+            version='serviceGroup_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/serviceGroup/customers/tasks/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkservice_group__1__0_models.QueryCustomerTaskUserDetailResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def query_customer_task_user_detail(
+        self,
+        request: dingtalkservice_group__1__0_models.QueryCustomerTaskUserDetailRequest,
+    ) -> dingtalkservice_group__1__0_models.QueryCustomerTaskUserDetailResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkservice_group__1__0_models.QueryCustomerTaskUserDetailHeaders()
+        return self.query_customer_task_user_detail_with_options(request, headers, runtime)
+
+    async def query_customer_task_user_detail_async(
+        self,
+        request: dingtalkservice_group__1__0_models.QueryCustomerTaskUserDetailRequest,
+    ) -> dingtalkservice_group__1__0_models.QueryCustomerTaskUserDetailResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkservice_group__1__0_models.QueryCustomerTaskUserDetailHeaders()
+        return await self.query_customer_task_user_detail_with_options_async(request, headers, runtime)
+
     def query_group_with_options(
         self,
         request: dingtalkservice_group__1__0_models.QueryGroupRequest,
         headers: dingtalkservice_group__1__0_models.QueryGroupHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkservice_group__1__0_models.QueryGroupResponse:
         UtilClient.validate_model(request)
@@ -6241,14 +6559,112 @@
         self,
         request: dingtalkservice_group__1__0_models.RobotMessageRecallRequest,
     ) -> dingtalkservice_group__1__0_models.RobotMessageRecallResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkservice_group__1__0_models.RobotMessageRecallHeaders()
         return await self.robot_message_recall_with_options_async(request, headers, runtime)
 
+    def save_form_instance_with_options(
+        self,
+        request: dingtalkservice_group__1__0_models.SaveFormInstanceRequest,
+        headers: dingtalkservice_group__1__0_models.SaveFormInstanceHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkservice_group__1__0_models.SaveFormInstanceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.form_data_list):
+            body['formDataList'] = request.form_data_list
+        if not UtilClient.is_unset(request.open_team_id):
+            body['openTeamId'] = request.open_team_id
+        if not UtilClient.is_unset(request.operator_union_id):
+            body['operatorUnionId'] = request.operator_union_id
+        if not UtilClient.is_unset(request.owner_union_id):
+            body['ownerUnionId'] = request.owner_union_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SaveFormInstance',
+            version='serviceGroup_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/serviceGroup/forms/instances',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkservice_group__1__0_models.SaveFormInstanceResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def save_form_instance_with_options_async(
+        self,
+        request: dingtalkservice_group__1__0_models.SaveFormInstanceRequest,
+        headers: dingtalkservice_group__1__0_models.SaveFormInstanceHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkservice_group__1__0_models.SaveFormInstanceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.form_data_list):
+            body['formDataList'] = request.form_data_list
+        if not UtilClient.is_unset(request.open_team_id):
+            body['openTeamId'] = request.open_team_id
+        if not UtilClient.is_unset(request.operator_union_id):
+            body['operatorUnionId'] = request.operator_union_id
+        if not UtilClient.is_unset(request.owner_union_id):
+            body['ownerUnionId'] = request.owner_union_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SaveFormInstance',
+            version='serviceGroup_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/serviceGroup/forms/instances',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkservice_group__1__0_models.SaveFormInstanceResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def save_form_instance(
+        self,
+        request: dingtalkservice_group__1__0_models.SaveFormInstanceRequest,
+    ) -> dingtalkservice_group__1__0_models.SaveFormInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkservice_group__1__0_models.SaveFormInstanceHeaders()
+        return self.save_form_instance_with_options(request, headers, runtime)
+
+    async def save_form_instance_async(
+        self,
+        request: dingtalkservice_group__1__0_models.SaveFormInstanceRequest,
+    ) -> dingtalkservice_group__1__0_models.SaveFormInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkservice_group__1__0_models.SaveFormInstanceHeaders()
+        return await self.save_form_instance_with_options_async(request, headers, runtime)
+
     def search_group_with_options(
         self,
         request: dingtalkservice_group__1__0_models.SearchGroupRequest,
         headers: dingtalkservice_group__1__0_models.SearchGroupHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkservice_group__1__0_models.SearchGroupResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2274,14 +2274,300 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = BatchGetGroupSetConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class BatchQueryCustomerSendTaskHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class BatchQueryCustomerSendTaskRequest(TeaModel):
+    def __init__(
+        self,
+        gmt_create_end: str = None,
+        gmt_create_start: str = None,
+        max_results: int = None,
+        need_rich_statistics: bool = None,
+        next_token: str = None,
+        open_batch_task_ids: List[str] = None,
+        open_team_id: str = None,
+        task_name: str = None,
+    ):
+        self.gmt_create_end = gmt_create_end
+        self.gmt_create_start = gmt_create_start
+        self.max_results = max_results
+        self.need_rich_statistics = need_rich_statistics
+        self.next_token = next_token
+        self.open_batch_task_ids = open_batch_task_ids
+        self.open_team_id = open_team_id
+        self.task_name = task_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.gmt_create_end is not None:
+            result['gmtCreateEnd'] = self.gmt_create_end
+        if self.gmt_create_start is not None:
+            result['gmtCreateStart'] = self.gmt_create_start
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.need_rich_statistics is not None:
+            result['needRichStatistics'] = self.need_rich_statistics
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.open_batch_task_ids is not None:
+            result['openBatchTaskIds'] = self.open_batch_task_ids
+        if self.open_team_id is not None:
+            result['openTeamId'] = self.open_team_id
+        if self.task_name is not None:
+            result['taskName'] = self.task_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('gmtCreateEnd') is not None:
+            self.gmt_create_end = m.get('gmtCreateEnd')
+        if m.get('gmtCreateStart') is not None:
+            self.gmt_create_start = m.get('gmtCreateStart')
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('needRichStatistics') is not None:
+            self.need_rich_statistics = m.get('needRichStatistics')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('openBatchTaskIds') is not None:
+            self.open_batch_task_ids = m.get('openBatchTaskIds')
+        if m.get('openTeamId') is not None:
+            self.open_team_id = m.get('openTeamId')
+        if m.get('taskName') is not None:
+            self.task_name = m.get('taskName')
+        return self
+
+
+class BatchQueryCustomerSendTaskResponseBodyRecords(TeaModel):
+    def __init__(
+        self,
+        create_name: str = None,
+        create_time_str: str = None,
+        create_union_id: str = None,
+        open_batch_task_id: str = None,
+        read_customer_inc: int = None,
+        read_user_inc: int = None,
+        send_customer_inc: int = None,
+        send_message_status: str = None,
+        send_task_time_str: str = None,
+        send_user_inc: int = None,
+        task_name: str = None,
+    ):
+        self.create_name = create_name
+        self.create_time_str = create_time_str
+        self.create_union_id = create_union_id
+        self.open_batch_task_id = open_batch_task_id
+        self.read_customer_inc = read_customer_inc
+        self.read_user_inc = read_user_inc
+        self.send_customer_inc = send_customer_inc
+        self.send_message_status = send_message_status
+        self.send_task_time_str = send_task_time_str
+        self.send_user_inc = send_user_inc
+        self.task_name = task_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_name is not None:
+            result['createName'] = self.create_name
+        if self.create_time_str is not None:
+            result['createTimeStr'] = self.create_time_str
+        if self.create_union_id is not None:
+            result['createUnionId'] = self.create_union_id
+        if self.open_batch_task_id is not None:
+            result['openBatchTaskId'] = self.open_batch_task_id
+        if self.read_customer_inc is not None:
+            result['readCustomerInc'] = self.read_customer_inc
+        if self.read_user_inc is not None:
+            result['readUserInc'] = self.read_user_inc
+        if self.send_customer_inc is not None:
+            result['sendCustomerInc'] = self.send_customer_inc
+        if self.send_message_status is not None:
+            result['sendMessageStatus'] = self.send_message_status
+        if self.send_task_time_str is not None:
+            result['sendTaskTimeStr'] = self.send_task_time_str
+        if self.send_user_inc is not None:
+            result['sendUserInc'] = self.send_user_inc
+        if self.task_name is not None:
+            result['taskName'] = self.task_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('createName') is not None:
+            self.create_name = m.get('createName')
+        if m.get('createTimeStr') is not None:
+            self.create_time_str = m.get('createTimeStr')
+        if m.get('createUnionId') is not None:
+            self.create_union_id = m.get('createUnionId')
+        if m.get('openBatchTaskId') is not None:
+            self.open_batch_task_id = m.get('openBatchTaskId')
+        if m.get('readCustomerInc') is not None:
+            self.read_customer_inc = m.get('readCustomerInc')
+        if m.get('readUserInc') is not None:
+            self.read_user_inc = m.get('readUserInc')
+        if m.get('sendCustomerInc') is not None:
+            self.send_customer_inc = m.get('sendCustomerInc')
+        if m.get('sendMessageStatus') is not None:
+            self.send_message_status = m.get('sendMessageStatus')
+        if m.get('sendTaskTimeStr') is not None:
+            self.send_task_time_str = m.get('sendTaskTimeStr')
+        if m.get('sendUserInc') is not None:
+            self.send_user_inc = m.get('sendUserInc')
+        if m.get('taskName') is not None:
+            self.task_name = m.get('taskName')
+        return self
+
+
+class BatchQueryCustomerSendTaskResponseBody(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        records: List[BatchQueryCustomerSendTaskResponseBodyRecords] = None,
+        total_count: int = None,
+    ):
+        self.max_results = max_results
+        self.next_token = next_token
+        self.records = records
+        self.total_count = total_count
+
+    def validate(self):
+        if self.records:
+            for k in self.records:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        result['records'] = []
+        if self.records is not None:
+            for k in self.records:
+                result['records'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['totalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        self.records = []
+        if m.get('records') is not None:
+            for k in m.get('records'):
+                temp_model = BatchQueryCustomerSendTaskResponseBodyRecords()
+                self.records.append(temp_model.from_map(k))
+        if m.get('totalCount') is not None:
+            self.total_count = m.get('totalCount')
+        return self
+
+
+class BatchQueryCustomerSendTaskResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: BatchQueryCustomerSendTaskResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = BatchQueryCustomerSendTaskResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class BatchQueryGroupMemberHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -5424,14 +5710,400 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateTicketResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CustomerSendMsgTaskHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class CustomerSendMsgTaskRequestMessageContentBtns(TeaModel):
+    def __init__(
+        self,
+        action_url: str = None,
+        title: str = None,
+    ):
+        self.action_url = action_url
+        self.title = title
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.action_url is not None:
+            result['actionURL'] = self.action_url
+        if self.title is not None:
+            result['title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('actionURL') is not None:
+            self.action_url = m.get('actionURL')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        return self
+
+
+class CustomerSendMsgTaskRequestMessageContent(TeaModel):
+    def __init__(
+        self,
+        btns: List[CustomerSendMsgTaskRequestMessageContentBtns] = None,
+        content: str = None,
+        message_type: str = None,
+        title: str = None,
+    ):
+        self.btns = btns
+        self.content = content
+        self.message_type = message_type
+        self.title = title
+
+    def validate(self):
+        if self.btns:
+            for k in self.btns:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['btns'] = []
+        if self.btns is not None:
+            for k in self.btns:
+                result['btns'].append(k.to_map() if k else None)
+        if self.content is not None:
+            result['content'] = self.content
+        if self.message_type is not None:
+            result['messageType'] = self.message_type
+        if self.title is not None:
+            result['title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.btns = []
+        if m.get('btns') is not None:
+            for k in m.get('btns'):
+                temp_model = CustomerSendMsgTaskRequestMessageContentBtns()
+                self.btns.append(temp_model.from_map(k))
+        if m.get('content') is not None:
+            self.content = m.get('content')
+        if m.get('messageType') is not None:
+            self.message_type = m.get('messageType')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        return self
+
+
+class CustomerSendMsgTaskRequestQueryCustomer(TeaModel):
+    def __init__(
+        self,
+        open_contact_ids: List[str] = None,
+        query_type: str = None,
+        search_contact_conditions: str = None,
+        search_customer_conditions: str = None,
+    ):
+        self.open_contact_ids = open_contact_ids
+        self.query_type = query_type
+        self.search_contact_conditions = search_contact_conditions
+        self.search_customer_conditions = search_customer_conditions
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.open_contact_ids is not None:
+            result['openContactIds'] = self.open_contact_ids
+        if self.query_type is not None:
+            result['queryType'] = self.query_type
+        if self.search_contact_conditions is not None:
+            result['searchContactConditions'] = self.search_contact_conditions
+        if self.search_customer_conditions is not None:
+            result['searchCustomerConditions'] = self.search_customer_conditions
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('openContactIds') is not None:
+            self.open_contact_ids = m.get('openContactIds')
+        if m.get('queryType') is not None:
+            self.query_type = m.get('queryType')
+        if m.get('searchContactConditions') is not None:
+            self.search_contact_conditions = m.get('searchContactConditions')
+        if m.get('searchCustomerConditions') is not None:
+            self.search_customer_conditions = m.get('searchCustomerConditions')
+        return self
+
+
+class CustomerSendMsgTaskRequestSendConfigUrlTrackConfig(TeaModel):
+    def __init__(
+        self,
+        title: str = None,
+        track_id: str = None,
+        track_url: str = None,
+    ):
+        self.title = title
+        self.track_id = track_id
+        self.track_url = track_url
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.title is not None:
+            result['title'] = self.title
+        if self.track_id is not None:
+            result['trackId'] = self.track_id
+        if self.track_url is not None:
+            result['trackUrl'] = self.track_url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        if m.get('trackId') is not None:
+            self.track_id = m.get('trackId')
+        if m.get('trackUrl') is not None:
+            self.track_url = m.get('trackUrl')
+        return self
+
+
+class CustomerSendMsgTaskRequestSendConfig(TeaModel):
+    def __init__(
+        self,
+        need_url_track: bool = None,
+        send_time: str = None,
+        send_type: str = None,
+        url_track_config: List[CustomerSendMsgTaskRequestSendConfigUrlTrackConfig] = None,
+    ):
+        self.need_url_track = need_url_track
+        self.send_time = send_time
+        self.send_type = send_type
+        self.url_track_config = url_track_config
+
+    def validate(self):
+        if self.url_track_config:
+            for k in self.url_track_config:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.need_url_track is not None:
+            result['needUrlTrack'] = self.need_url_track
+        if self.send_time is not None:
+            result['sendTime'] = self.send_time
+        if self.send_type is not None:
+            result['sendType'] = self.send_type
+        result['urlTrackConfig'] = []
+        if self.url_track_config is not None:
+            for k in self.url_track_config:
+                result['urlTrackConfig'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('needUrlTrack') is not None:
+            self.need_url_track = m.get('needUrlTrack')
+        if m.get('sendTime') is not None:
+            self.send_time = m.get('sendTime')
+        if m.get('sendType') is not None:
+            self.send_type = m.get('sendType')
+        self.url_track_config = []
+        if m.get('urlTrackConfig') is not None:
+            for k in m.get('urlTrackConfig'):
+                temp_model = CustomerSendMsgTaskRequestSendConfigUrlTrackConfig()
+                self.url_track_config.append(temp_model.from_map(k))
+        return self
+
+
+class CustomerSendMsgTaskRequest(TeaModel):
+    def __init__(
+        self,
+        message_content: CustomerSendMsgTaskRequestMessageContent = None,
+        open_team_id: str = None,
+        query_customer: CustomerSendMsgTaskRequestQueryCustomer = None,
+        send_config: CustomerSendMsgTaskRequestSendConfig = None,
+        task_name: str = None,
+    ):
+        self.message_content = message_content
+        self.open_team_id = open_team_id
+        self.query_customer = query_customer
+        self.send_config = send_config
+        self.task_name = task_name
+
+    def validate(self):
+        if self.message_content:
+            self.message_content.validate()
+        if self.query_customer:
+            self.query_customer.validate()
+        if self.send_config:
+            self.send_config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.message_content is not None:
+            result['messageContent'] = self.message_content.to_map()
+        if self.open_team_id is not None:
+            result['openTeamId'] = self.open_team_id
+        if self.query_customer is not None:
+            result['queryCustomer'] = self.query_customer.to_map()
+        if self.send_config is not None:
+            result['sendConfig'] = self.send_config.to_map()
+        if self.task_name is not None:
+            result['taskName'] = self.task_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('messageContent') is not None:
+            temp_model = CustomerSendMsgTaskRequestMessageContent()
+            self.message_content = temp_model.from_map(m['messageContent'])
+        if m.get('openTeamId') is not None:
+            self.open_team_id = m.get('openTeamId')
+        if m.get('queryCustomer') is not None:
+            temp_model = CustomerSendMsgTaskRequestQueryCustomer()
+            self.query_customer = temp_model.from_map(m['queryCustomer'])
+        if m.get('sendConfig') is not None:
+            temp_model = CustomerSendMsgTaskRequestSendConfig()
+            self.send_config = temp_model.from_map(m['sendConfig'])
+        if m.get('taskName') is not None:
+            self.task_name = m.get('taskName')
+        return self
+
+
+class CustomerSendMsgTaskResponseBody(TeaModel):
+    def __init__(
+        self,
+        open_batch_task_id: str = None,
+    ):
+        self.open_batch_task_id = open_batch_task_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.open_batch_task_id is not None:
+            result['openBatchTaskId'] = self.open_batch_task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('openBatchTaskId') is not None:
+            self.open_batch_task_id = m.get('openBatchTaskId')
+        return self
+
+
+class CustomerSendMsgTaskResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CustomerSendMsgTaskResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CustomerSendMsgTaskResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteGroupMembersFromGroupHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -9517,14 +10189,335 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryCustomerCardResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryCustomerTaskUserDetailHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class QueryCustomerTaskUserDetailRequest(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        open_batch_task_id: str = None,
+        open_team_id: str = None,
+        receiver_union_ids: List[str] = None,
+    ):
+        self.max_results = max_results
+        self.next_token = next_token
+        self.open_batch_task_id = open_batch_task_id
+        self.open_team_id = open_team_id
+        self.receiver_union_ids = receiver_union_ids
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.open_batch_task_id is not None:
+            result['openBatchTaskId'] = self.open_batch_task_id
+        if self.open_team_id is not None:
+            result['openTeamId'] = self.open_team_id
+        if self.receiver_union_ids is not None:
+            result['receiverUnionIds'] = self.receiver_union_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('openBatchTaskId') is not None:
+            self.open_batch_task_id = m.get('openBatchTaskId')
+        if m.get('openTeamId') is not None:
+            self.open_team_id = m.get('openTeamId')
+        if m.get('receiverUnionIds') is not None:
+            self.receiver_union_ids = m.get('receiverUnionIds')
+        return self
+
+
+class QueryCustomerTaskUserDetailResponseBodyRecordsEventTrackResponses(TeaModel):
+    def __init__(
+        self,
+        click_time: str = None,
+        event_track_id: str = None,
+        on_click: bool = None,
+        title: str = None,
+    ):
+        self.click_time = click_time
+        self.event_track_id = event_track_id
+        self.on_click = on_click
+        self.title = title
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.click_time is not None:
+            result['clickTime'] = self.click_time
+        if self.event_track_id is not None:
+            result['eventTrackId'] = self.event_track_id
+        if self.on_click is not None:
+            result['onClick'] = self.on_click
+        if self.title is not None:
+            result['title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('clickTime') is not None:
+            self.click_time = m.get('clickTime')
+        if m.get('eventTrackId') is not None:
+            self.event_track_id = m.get('eventTrackId')
+        if m.get('onClick') is not None:
+            self.on_click = m.get('onClick')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        return self
+
+
+class QueryCustomerTaskUserDetailResponseBodyRecords(TeaModel):
+    def __init__(
+        self,
+        customer_names: str = None,
+        error_code: str = None,
+        error_detail: str = None,
+        event_track_responses: List[QueryCustomerTaskUserDetailResponseBodyRecordsEventTrackResponses] = None,
+        open_batch_task_id: str = None,
+        read_status: int = None,
+        read_time: str = None,
+        receiver_name: str = None,
+        receiver_union_id: str = None,
+        send_time: str = None,
+        status: str = None,
+    ):
+        self.customer_names = customer_names
+        self.error_code = error_code
+        self.error_detail = error_detail
+        self.event_track_responses = event_track_responses
+        self.open_batch_task_id = open_batch_task_id
+        self.read_status = read_status
+        self.read_time = read_time
+        self.receiver_name = receiver_name
+        self.receiver_union_id = receiver_union_id
+        self.send_time = send_time
+        self.status = status
+
+    def validate(self):
+        if self.event_track_responses:
+            for k in self.event_track_responses:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.customer_names is not None:
+            result['customerNames'] = self.customer_names
+        if self.error_code is not None:
+            result['errorCode'] = self.error_code
+        if self.error_detail is not None:
+            result['errorDetail'] = self.error_detail
+        result['eventTrackResponses'] = []
+        if self.event_track_responses is not None:
+            for k in self.event_track_responses:
+                result['eventTrackResponses'].append(k.to_map() if k else None)
+        if self.open_batch_task_id is not None:
+            result['openBatchTaskId'] = self.open_batch_task_id
+        if self.read_status is not None:
+            result['readStatus'] = self.read_status
+        if self.read_time is not None:
+            result['readTime'] = self.read_time
+        if self.receiver_name is not None:
+            result['receiverName'] = self.receiver_name
+        if self.receiver_union_id is not None:
+            result['receiverUnionId'] = self.receiver_union_id
+        if self.send_time is not None:
+            result['sendTime'] = self.send_time
+        if self.status is not None:
+            result['status'] = self.status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('customerNames') is not None:
+            self.customer_names = m.get('customerNames')
+        if m.get('errorCode') is not None:
+            self.error_code = m.get('errorCode')
+        if m.get('errorDetail') is not None:
+            self.error_detail = m.get('errorDetail')
+        self.event_track_responses = []
+        if m.get('eventTrackResponses') is not None:
+            for k in m.get('eventTrackResponses'):
+                temp_model = QueryCustomerTaskUserDetailResponseBodyRecordsEventTrackResponses()
+                self.event_track_responses.append(temp_model.from_map(k))
+        if m.get('openBatchTaskId') is not None:
+            self.open_batch_task_id = m.get('openBatchTaskId')
+        if m.get('readStatus') is not None:
+            self.read_status = m.get('readStatus')
+        if m.get('readTime') is not None:
+            self.read_time = m.get('readTime')
+        if m.get('receiverName') is not None:
+            self.receiver_name = m.get('receiverName')
+        if m.get('receiverUnionId') is not None:
+            self.receiver_union_id = m.get('receiverUnionId')
+        if m.get('sendTime') is not None:
+            self.send_time = m.get('sendTime')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        return self
+
+
+class QueryCustomerTaskUserDetailResponseBody(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        records: List[QueryCustomerTaskUserDetailResponseBodyRecords] = None,
+        total_count: int = None,
+    ):
+        self.max_results = max_results
+        self.next_token = next_token
+        self.records = records
+        self.total_count = total_count
+
+    def validate(self):
+        if self.records:
+            for k in self.records:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        result['records'] = []
+        if self.records is not None:
+            for k in self.records:
+                result['records'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['totalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        self.records = []
+        if m.get('records') is not None:
+            for k in m.get('records'):
+                temp_model = QueryCustomerTaskUserDetailResponseBodyRecords()
+                self.records.append(temp_model.from_map(k))
+        if m.get('totalCount') is not None:
+            self.total_count = m.get('totalCount')
+        return self
+
+
+class QueryCustomerTaskUserDetailResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryCustomerTaskUserDetailResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryCustomerTaskUserDetailResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryGroupHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -12887,14 +13880,169 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RobotMessageRecallResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SaveFormInstanceHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class SaveFormInstanceRequest(TeaModel):
+    def __init__(
+        self,
+        form_data_list: str = None,
+        open_team_id: str = None,
+        operator_union_id: str = None,
+        owner_union_id: str = None,
+    ):
+        self.form_data_list = form_data_list
+        self.open_team_id = open_team_id
+        self.operator_union_id = operator_union_id
+        self.owner_union_id = owner_union_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.form_data_list is not None:
+            result['formDataList'] = self.form_data_list
+        if self.open_team_id is not None:
+            result['openTeamId'] = self.open_team_id
+        if self.operator_union_id is not None:
+            result['operatorUnionId'] = self.operator_union_id
+        if self.owner_union_id is not None:
+            result['ownerUnionId'] = self.owner_union_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('formDataList') is not None:
+            self.form_data_list = m.get('formDataList')
+        if m.get('openTeamId') is not None:
+            self.open_team_id = m.get('openTeamId')
+        if m.get('operatorUnionId') is not None:
+            self.operator_union_id = m.get('operatorUnionId')
+        if m.get('ownerUnionId') is not None:
+            self.owner_union_id = m.get('ownerUnionId')
+        return self
+
+
+class SaveFormInstanceResponseBody(TeaModel):
+    def __init__(
+        self,
+        open_contact_id: str = None,
+        open_customer_id: str = None,
+    ):
+        self.open_contact_id = open_contact_id
+        self.open_customer_id = open_customer_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.open_contact_id is not None:
+            result['openContactId'] = self.open_contact_id
+        if self.open_customer_id is not None:
+            result['openCustomerId'] = self.open_customer_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('openContactId') is not None:
+            self.open_contact_id = m.get('openContactId')
+        if m.get('openCustomerId') is not None:
+            self.open_customer_id = m.get('openCustomerId')
+        return self
+
+
+class SaveFormInstanceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SaveFormInstanceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SaveFormInstanceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SearchGroupHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.26
+Version: 2.0.27
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.26/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.27/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.26/setup.py` & `alibabacloud_dingtalk-2.0.27/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 21/07/2023
+Created on 26/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_tea_util>=0.3.10, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0",
     "alibabacloud_gateway_spi>=0.0.1, <1.0.0",
     "alibabacloud_gateway_dingtalk>=1.0.2, <2.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

