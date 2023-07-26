# Comparing `tmp/pulumi_signalfx-5.9.0a1678179334.tar.gz` & `tmp/pulumi_signalfx-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_signalfx-5.9.0a1678179334.tar", last modified: Tue Mar  7 09:00:07 2023, max compression
+gzip compressed data, was "pulumi_signalfx-6.0.0.tar", last modified: Wed Jul 26 20:20:00 2023, max compression
```

## Comparing `pulumi_signalfx-5.9.0a1678179334.tar` & `pulumi_signalfx-6.0.0.tar`

### file list

```diff
@@ -1,86 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.055112 pulumi_signalfx-5.9.0a1678179334/
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-07 09:00:07.055112 pulumi_signalfx-5.9.0a1678179334/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.047111 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   139415 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/alert_muting_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/external_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/get_services.py
--rw-r--r--   0 runner    (1001) docker     (123)    80393 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/token_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/get_services.py
--rw-r--r--   0 runner    (1001) docker     (123)    55951 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    60438 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    34779 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/dashboard_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    23028 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/data_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    62286 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/event_feed_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/get_services.py
--rw-r--r--   0 runner    (1001) docker     (123)    34418 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/get_aws_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/get_azure_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/get_dimension_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    42295 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/heatmap_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/jira/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32032 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/jira/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    62121 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/list_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28303 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/view.py
--rw-r--r--   0 runner    (1001) docker     (123)    17643 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/metric_ruleset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/opsgenie/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/opsgenie/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/org_token.py
--rw-r--r--   0 runner    (1001) docker     (123)   126160 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/pagerduty/get_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/pagerduty/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/servicenow/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/servicenow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27661 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/servicenow/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    40263 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/single_value_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.055112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/slack/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/slack/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    31617 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/table_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    27565 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/text_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    78926 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/time_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.055112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/victorops/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/victorops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/victorops/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/webhook_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:00:07.051112 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-07 09:00:07.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-03-07 09:00:07.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 09:00:07.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 09:00:07.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-07 09:00:07.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-07 09:00:07.000000 pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 09:00:07.055112 pulumi_signalfx-5.9.0a1678179334/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-03-07 09:00:06.000000 pulumi_signalfx-5.9.0a1678179334/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.626486 pulumi_signalfx-6.0.0/pulumi_signalfx/
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   140636 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19485 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/alert_muting_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.626486 pulumi_signalfx-6.0.0/pulumi_signalfx/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/aws/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19593 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/aws/external_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81078 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/aws/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/aws/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/aws/token_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.626486 pulumi_signalfx-6.0.0/pulumi_signalfx/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/azure/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53922 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/azure/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/azure/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.626486 pulumi_signalfx-6.0.0/pulumi_signalfx/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61578 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36715 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/dashboard_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23028 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/data_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63092 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/event_feed_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34425 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/get_dimension_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42295 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/heatmap_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/jira/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32032 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/jira/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62676 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/list_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/logs/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/logs/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28303 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/logs/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18758 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/metric_ruleset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/opsgenie/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23045 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/org_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127525 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/pagerduty/get_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/pagerduty/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/servicenow/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/servicenow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27661 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/servicenow/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40263 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/single_value_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/slack/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31617 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/table_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27565 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/text_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80156 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/time_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/pulumi_signalfx/victorops/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/victorops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/victorops/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx/webhook_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:20:00.626486 pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 20:20:00.630486 pulumi_signalfx-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-26 20:20:00.000000 pulumi_signalfx-6.0.0/setup.py
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/PKG-INFO` & `pulumi_signalfx-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pulumi_signalfx
-Version: 5.9.0a1678179334
+Version: 6.0.0
 Summary: A Pulumi package for creating and managing SignalFx resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi signalfx
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-signalfx/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-signalfx/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fsignalfx.svg)](https://www.npmjs.com/package/@pulumi/signalfx)
 [![Python version](https://badge.fury.io/py/pulumi-signalfx.svg)](https://pypi.org/project/pulumi-signalfx)
 [![NuGet version](https://badge.fury.io/nu/pulumi.signalfx.svg)](https://badge.fury.io/nu/pulumi.signalfx)
-[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-signalfx/sdk/v5/go)](https://pkg.go.dev/github.com/pulumi/pulumi-signalfx/sdk/v5/go)
+[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-signalfx/sdk/v6/go)](https://pkg.go.dev/github.com/pulumi/pulumi-signalfx/sdk/v6/go)
 [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-signalfx/blob/master/LICENSE)
 
 # SignalFx Resource Provider
 
 The SignalFx resource provider for Pulumi lets you manage SignalFx resources in your cloud programs. To use
 this package, please [install the Pulumi CLI first](https://pulumi.io/).
 
@@ -42,15 +43,15 @@
 
     $ pip install pulumi_signalfx
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-signalfx/sdk/v5
+    $ go get github.com/pulumi/pulumi-signalfx/sdk/v6
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Signalfx
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/README.md` & `pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,25 @@
+Metadata-Version: 2.1
+Name: pulumi-signalfx
+Version: 6.0.0
+Summary: A Pulumi package for creating and managing SignalFx resources.
+Home-page: https://pulumi.io
+License: Apache-2.0
+Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
+Keywords: pulumi signalfx
+Platform: UNKNOWN
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 [![Actions Status](https://github.com/pulumi/pulumi-signalfx/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-signalfx/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fsignalfx.svg)](https://www.npmjs.com/package/@pulumi/signalfx)
 [![Python version](https://badge.fury.io/py/pulumi-signalfx.svg)](https://pypi.org/project/pulumi-signalfx)
 [![NuGet version](https://badge.fury.io/nu/pulumi.signalfx.svg)](https://badge.fury.io/nu/pulumi.signalfx)
-[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-signalfx/sdk/v5/go)](https://pkg.go.dev/github.com/pulumi/pulumi-signalfx/sdk/v5/go)
+[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-signalfx/sdk/v6/go)](https://pkg.go.dev/github.com/pulumi/pulumi-signalfx/sdk/v6/go)
 [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-signalfx/blob/master/LICENSE)
 
 # SignalFx Resource Provider
 
 The SignalFx resource provider for Pulumi lets you manage SignalFx resources in your cloud programs. To use
 this package, please [install the Pulumi CLI first](https://pulumi.io/).
 
@@ -31,15 +43,15 @@
 
     $ pip install pulumi_signalfx
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-signalfx/sdk/v5
+    $ go get github.com/pulumi/pulumi-signalfx/sdk/v6
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Signalfx
 
@@ -53,7 +65,9 @@
   who need to set their Realm or use a proxy. Note: You likely want to change `customAppUrl` too!
 - `signalfx:customAppUrl` - (Optional) The application URL that users should use to interact with assets in the browser.
   This is used by organizations using specific realms or those with a custom SSO domain.
 
 ## Reference
 
 For further information, please visit [the SignalFx provider docs](https://www.pulumi.com/docs/intro/cloud-providers/signalfx) or for detailed reference documentation, please visit [the API docs](https://www.pulumi.com/docs/reference/pkg/signalfx).
+
+
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/__init__.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # Export this package's modules as members:
 from .alert_muting_rule import *
 from .dashboard import *
 from .dashboard_group import *
 from .data_link import *
 from .detector import *
 from .event_feed_chart import *
-from .get_aws_services import *
-from .get_azure_services import *
 from .get_dimension_values import *
 from .heatmap_chart import *
 from .list_chart import *
 from .metric_ruleset import *
 from .org_token import *
 from .provider import *
 from .single_value_chart import *
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/_inputs.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,14 @@
     'TimeChartAxisRightArgs',
     'TimeChartAxisRightWatermarkArgs',
     'TimeChartEventOptionArgs',
     'TimeChartHistogramOptionArgs',
     'TimeChartLegendOptionsFieldArgs',
     'TimeChartVizOptionArgs',
     'WebhookIntegrationHeaderArgs',
-    'GetAwsServicesServiceArgs',
-    'GetAzureServicesServiceArgs',
 ]
 
 @pulumi.input_type
 class AlertMutingRuleFilterArgs:
     def __init__(__self__, *,
                  property: pulumi.Input[str],
                  property_value: pulumi.Input[str],
@@ -1582,15 +1580,25 @@
                  value_suffix: Optional[pulumi.Input[str]] = None,
                  value_unit: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] label: Label used in the publish statement that displays the plot (metric time series data) you want to customize.
         :param pulumi.Input[str] color: Color to use : gray, blue, azure, navy, brown, orange, yellow, iris, magenta, pink, purple, violet, lilac, emerald, green, aquamarine.
         :param pulumi.Input[str] display_name: Specifies an alternate value for the Plot Name column of the Data Table associated with the chart.
         :param pulumi.Input[str] value_prefix: , `value_suffix` - (Optional) Arbitrary prefix/suffix to display with the value of this plot.
-        :param pulumi.Input[str] value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+               
+               **Notes**
+               
+               It is highly recommended that you use both `max_delay` in your detector configuration and an `extrapolation` policy in your program text to reduce false positives/negatives.
+               
+               `max_delay` allows SignalFx to continue with computation if there is a lag in receiving data points.
+               
+               `extrapolation` allows you to specify how to handle missing data. An extrapolation policy can be added to individual signals by updating the data block in your `program_text`.
+               
+               See [Delayed Datapoints](https://signalfx-product-docs.readthedocs-hosted.com/en/latest/charts/chart-builder.html#delayed-datapoints) for more info.
+        :param pulumi.Input[str] value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         pulumi.set(__self__, "label", label)
         if color is not None:
             pulumi.set(__self__, "color", color)
         if display_name is not None:
             pulumi.set(__self__, "display_name", display_name)
         if value_prefix is not None:
@@ -1637,14 +1645,24 @@
         pulumi.set(self, "display_name", value)
 
     @property
     @pulumi.getter(name="valuePrefix")
     def value_prefix(self) -> Optional[pulumi.Input[str]]:
         """
         , `value_suffix` - (Optional) Arbitrary prefix/suffix to display with the value of this plot.
+
+        **Notes**
+
+        It is highly recommended that you use both `max_delay` in your detector configuration and an `extrapolation` policy in your program text to reduce false positives/negatives.
+
+        `max_delay` allows SignalFx to continue with computation if there is a lag in receiving data points.
+
+        `extrapolation` allows you to specify how to handle missing data. An extrapolation policy can be added to individual signals by updating the data block in your `program_text`.
+
+        See [Delayed Datapoints](https://signalfx-product-docs.readthedocs-hosted.com/en/latest/charts/chart-builder.html#delayed-datapoints) for more info.
         """
         return pulumi.get(self, "value_prefix")
 
     @value_prefix.setter
     def value_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "value_prefix", value)
 
@@ -1657,15 +1675,15 @@
     def value_suffix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "value_suffix", value)
 
     @property
     @pulumi.getter(name="valueUnit")
     def value_unit(self) -> Optional[pulumi.Input[str]]:
         """
-        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         return pulumi.get(self, "value_unit")
 
     @value_unit.setter
     def value_unit(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "value_unit", value)
 
@@ -1944,15 +1962,15 @@
                  value_suffix: Optional[pulumi.Input[str]] = None,
                  value_unit: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] label: Label used in the publish statement that displays the plot (metric time series data) you want to customize.
         :param pulumi.Input[str] color: The color to use. Must be one of gray, blue, light_blue, navy, dark_orange, orange, dark_yellow, magenta, cerise, pink, violet, purple, gray_blue, dark_green, green, aquamarine, red, yellow, vivid_yellow, light_green, or lime_green.
         :param pulumi.Input[str] display_name: Specifies an alternate value for the Plot Name column of the Data Table associated with the chart.
         :param pulumi.Input[str] value_prefix: , `value_suffix` - (Optional) Arbitrary prefix/suffix to display with the value of this plot.
-        :param pulumi.Input[str] value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+        :param pulumi.Input[str] value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         pulumi.set(__self__, "label", label)
         if color is not None:
             pulumi.set(__self__, "color", color)
         if display_name is not None:
             pulumi.set(__self__, "display_name", display_name)
         if value_prefix is not None:
@@ -2019,15 +2037,15 @@
     def value_suffix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "value_suffix", value)
 
     @property
     @pulumi.getter(name="valueUnit")
     def value_unit(self) -> Optional[pulumi.Input[str]]:
         """
-        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         return pulumi.get(self, "value_unit")
 
     @value_unit.setter
     def value_unit(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "value_unit", value)
 
@@ -2039,14 +2057,15 @@
                  enabled: pulumi.Input[bool],
                  matchers: pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleMatcherArgs']]],
                  name: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleAggregatorArgs']]] aggregators: Aggregator object
         :param pulumi.Input[bool] enabled: When false, this rule will not generate aggregated MTSs
         :param pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleMatcherArgs']]] matchers: Matcher object
+        :param pulumi.Input[str] name: name of the aggregation rule
         """
         pulumi.set(__self__, "aggregators", aggregators)
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "matchers", matchers)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
@@ -2085,14 +2104,17 @@
     @matchers.setter
     def matchers(self, value: pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleMatcherArgs']]]):
         pulumi.set(self, "matchers", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        name of the aggregation rule
+        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
@@ -2254,23 +2276,23 @@
 
 
 @pulumi.input_type
 class MetricRulesetRoutingRuleArgs:
     def __init__(__self__, *,
                  destination: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] destination: end destination of the input metric
+        :param pulumi.Input[str] destination: end destination of the input metric. Must be `RealTime` or `Drop`
         """
         pulumi.set(__self__, "destination", destination)
 
     @property
     @pulumi.getter
     def destination(self) -> pulumi.Input[str]:
         """
-        end destination of the input metric
+        end destination of the input metric. Must be `RealTime` or `Drop`
         """
         return pulumi.get(self, "destination")
 
     @destination.setter
     def destination(self, value: pulumi.Input[str]):
         pulumi.set(self, "destination", value)
 
@@ -2544,15 +2566,15 @@
                  value_suffix: Optional[pulumi.Input[str]] = None,
                  value_unit: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] label: Label used in the publish statement that displays the plot (metric time series data) you want to customize.
         :param pulumi.Input[str] color: The color to use. Must be one of gray, blue, light_blue, navy, dark_orange, orange, dark_yellow, magenta, cerise, pink, violet, purple, gray_blue, dark_green, green, aquamarine, red, yellow, vivid_yellow, light_green, or lime_green.
         :param pulumi.Input[str] display_name: Specifies an alternate value for the Plot Name column of the Data Table associated with the chart.
         :param pulumi.Input[str] value_prefix: , `value_suffix` - (Optional) Arbitrary prefix/suffix to display with the value of this plot.
-        :param pulumi.Input[str] value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+        :param pulumi.Input[str] value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         pulumi.set(__self__, "label", label)
         if color is not None:
             pulumi.set(__self__, "color", color)
         if display_name is not None:
             pulumi.set(__self__, "display_name", display_name)
         if value_prefix is not None:
@@ -2619,15 +2641,15 @@
     def value_suffix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "value_suffix", value)
 
     @property
     @pulumi.getter(name="valueUnit")
     def value_unit(self) -> Optional[pulumi.Input[str]]:
         """
-        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         return pulumi.get(self, "value_unit")
 
     @value_unit.setter
     def value_unit(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "value_unit", value)
 
@@ -3167,15 +3189,15 @@
         """
         :param pulumi.Input[str] label: Label used in the publish statement that displays the event query you want to customize.
         :param pulumi.Input[str] axis: Y-axis associated with values for this plot. Must be either `right` or `left`.
         :param pulumi.Input[str] color: Color to use : gray, blue, azure, navy, brown, orange, yellow, iris, magenta, pink, purple, violet, lilac, emerald, green, aquamarine.
         :param pulumi.Input[str] display_name: Specifies an alternate value for the Plot Name column of the Data Table associated with the chart.
         :param pulumi.Input[str] plot_type: The visualization style to use. Must be `"LineChart"`, `"AreaChart"`, `"ColumnChart"`, or `"Histogram"`. Chart level `plot_type` by default.
         :param pulumi.Input[str] value_prefix: , `value_suffix` - (Optional) Arbitrary prefix/suffix to display with the value of this plot.
-        :param pulumi.Input[str] value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+        :param pulumi.Input[str] value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         pulumi.set(__self__, "label", label)
         if axis is not None:
             pulumi.set(__self__, "axis", axis)
         if color is not None:
             pulumi.set(__self__, "color", color)
         if display_name is not None:
@@ -3270,15 +3292,15 @@
     def value_suffix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "value_suffix", value)
 
     @property
     @pulumi.getter(name="valueUnit")
     def value_unit(self) -> Optional[pulumi.Input[str]]:
         """
-        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         return pulumi.get(self, "value_unit")
 
     @value_unit.setter
     def value_unit(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "value_unit", value)
 
@@ -3316,39 +3338,7 @@
         return pulumi.get(self, "header_value")
 
     @header_value.setter
     def header_value(self, value: pulumi.Input[str]):
         pulumi.set(self, "header_value", value)
 
 
-@pulumi.input_type
-class GetAwsServicesServiceArgs:
-    def __init__(__self__, *,
-                 name: str):
-        pulumi.set(__self__, "name", name)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: str):
-        pulumi.set(self, "name", value)
-
-
-@pulumi.input_type
-class GetAzureServicesServiceArgs:
-    def __init__(__self__, *,
-                 name: str):
-        pulumi.set(__self__, "name", name)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: str):
-        pulumi.set(self, "name", value)
-
-
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/_utilities.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/alert_muting_rule.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/alert_muting_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/_inputs.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/aws/_inputs.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,79 +9,78 @@
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
     'IntegrationCustomNamespaceSyncRuleArgs',
     'IntegrationMetricStatsToSyncArgs',
     'IntegrationNamespaceSyncRuleArgs',
-    'GetServicesServiceArgs',
 ]
 
 @pulumi.input_type
 class IntegrationCustomNamespaceSyncRuleArgs:
     def __init__(__self__, *,
                  namespace: pulumi.Input[str],
                  default_action: Optional[pulumi.Input[str]] = None,
                  filter_action: Optional[pulumi.Input[str]] = None,
                  filter_source: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] namespace: An AWS custom namespace having custom AWS metrics that you want to sync with SignalFx. See the AWS documentation on publishing metrics for more information.
-        :param pulumi.Input[str] default_action: Controls the SignalFx default behavior for processing data from an AWS namespace. If you do specify a filter, use this property to control how SignalFx treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
-        :param pulumi.Input[str] filter_action: Controls how SignalFx processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
-        :param pulumi.Input[str] filter_source: Expression that selects the data that SignalFx should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
+        :param pulumi.Input[str] namespace: An AWS custom namespace having custom AWS metrics that you want to sync with Splunk Observability. See `services` field description below for additional information.
+        :param pulumi.Input[str] default_action: Controls the Splunk Observability default behavior for processing data from an AWS namespace. Splunk Observability ignores this property unless you specify the `filter_action` and `filter_source` properties. If you do specify them, use this property to control how Splunk Observability treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
+        :param pulumi.Input[str] filter_action: Controls how Splunk Observability processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
+        :param pulumi.Input[str] filter_source: Expression that selects the data that Splunk Observability should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
         """
         pulumi.set(__self__, "namespace", namespace)
         if default_action is not None:
             pulumi.set(__self__, "default_action", default_action)
         if filter_action is not None:
             pulumi.set(__self__, "filter_action", filter_action)
         if filter_source is not None:
             pulumi.set(__self__, "filter_source", filter_source)
 
     @property
     @pulumi.getter
     def namespace(self) -> pulumi.Input[str]:
         """
-        An AWS custom namespace having custom AWS metrics that you want to sync with SignalFx. See the AWS documentation on publishing metrics for more information.
+        An AWS custom namespace having custom AWS metrics that you want to sync with Splunk Observability. See `services` field description below for additional information.
         """
         return pulumi.get(self, "namespace")
 
     @namespace.setter
     def namespace(self, value: pulumi.Input[str]):
         pulumi.set(self, "namespace", value)
 
     @property
     @pulumi.getter(name="defaultAction")
     def default_action(self) -> Optional[pulumi.Input[str]]:
         """
-        Controls the SignalFx default behavior for processing data from an AWS namespace. If you do specify a filter, use this property to control how SignalFx treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
+        Controls the Splunk Observability default behavior for processing data from an AWS namespace. Splunk Observability ignores this property unless you specify the `filter_action` and `filter_source` properties. If you do specify them, use this property to control how Splunk Observability treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
         """
         return pulumi.get(self, "default_action")
 
     @default_action.setter
     def default_action(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_action", value)
 
     @property
     @pulumi.getter(name="filterAction")
     def filter_action(self) -> Optional[pulumi.Input[str]]:
         """
-        Controls how SignalFx processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
+        Controls how Splunk Observability processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
         """
         return pulumi.get(self, "filter_action")
 
     @filter_action.setter
     def filter_action(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "filter_action", value)
 
     @property
     @pulumi.getter(name="filterSource")
     def filter_source(self) -> Optional[pulumi.Input[str]]:
         """
-        Expression that selects the data that SignalFx should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
+        Expression that selects the data that Splunk Observability should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
         """
         return pulumi.get(self, "filter_source")
 
     @filter_source.setter
     def filter_source(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "filter_source", value)
 
@@ -90,15 +89,15 @@
 class IntegrationMetricStatsToSyncArgs:
     def __init__(__self__, *,
                  metric: pulumi.Input[str],
                  namespace: pulumi.Input[str],
                  stats: pulumi.Input[Sequence[pulumi.Input[str]]]):
         """
         :param pulumi.Input[str] metric: AWS metric that you want to pick statistics for
-        :param pulumi.Input[str] namespace: An AWS custom namespace having custom AWS metrics that you want to sync with SignalFx. See the AWS documentation on publishing metrics for more information.
+        :param pulumi.Input[str] namespace: An AWS custom namespace having custom AWS metrics that you want to sync with Splunk Observability. See `services` field description below for additional information.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] stats: AWS statistics you want to collect
         """
         pulumi.set(__self__, "metric", metric)
         pulumi.set(__self__, "namespace", namespace)
         pulumi.set(__self__, "stats", stats)
 
     @property
@@ -113,15 +112,15 @@
     def metric(self, value: pulumi.Input[str]):
         pulumi.set(self, "metric", value)
 
     @property
     @pulumi.getter
     def namespace(self) -> pulumi.Input[str]:
         """
-        An AWS custom namespace having custom AWS metrics that you want to sync with SignalFx. See the AWS documentation on publishing metrics for more information.
+        An AWS custom namespace having custom AWS metrics that you want to sync with Splunk Observability. See `services` field description below for additional information.
         """
         return pulumi.get(self, "namespace")
 
     @namespace.setter
     def namespace(self, value: pulumi.Input[str]):
         pulumi.set(self, "namespace", value)
 
@@ -142,85 +141,69 @@
 class IntegrationNamespaceSyncRuleArgs:
     def __init__(__self__, *,
                  namespace: pulumi.Input[str],
                  default_action: Optional[pulumi.Input[str]] = None,
                  filter_action: Optional[pulumi.Input[str]] = None,
                  filter_source: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] namespace: An AWS custom namespace having custom AWS metrics that you want to sync with SignalFx. See the AWS documentation on publishing metrics for more information.
-        :param pulumi.Input[str] default_action: Controls the SignalFx default behavior for processing data from an AWS namespace. If you do specify a filter, use this property to control how SignalFx treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
-        :param pulumi.Input[str] filter_action: Controls how SignalFx processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
-        :param pulumi.Input[str] filter_source: Expression that selects the data that SignalFx should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
+        :param pulumi.Input[str] namespace: An AWS custom namespace having custom AWS metrics that you want to sync with Splunk Observability. See `services` field description below for additional information.
+        :param pulumi.Input[str] default_action: Controls the Splunk Observability default behavior for processing data from an AWS namespace. Splunk Observability ignores this property unless you specify the `filter_action` and `filter_source` properties. If you do specify them, use this property to control how Splunk Observability treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
+        :param pulumi.Input[str] filter_action: Controls how Splunk Observability processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
+        :param pulumi.Input[str] filter_source: Expression that selects the data that Splunk Observability should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
         """
         pulumi.set(__self__, "namespace", namespace)
         if default_action is not None:
             pulumi.set(__self__, "default_action", default_action)
         if filter_action is not None:
             pulumi.set(__self__, "filter_action", filter_action)
         if filter_source is not None:
             pulumi.set(__self__, "filter_source", filter_source)
 
     @property
     @pulumi.getter
     def namespace(self) -> pulumi.Input[str]:
         """
-        An AWS custom namespace having custom AWS metrics that you want to sync with SignalFx. See the AWS documentation on publishing metrics for more information.
+        An AWS custom namespace having custom AWS metrics that you want to sync with Splunk Observability. See `services` field description below for additional information.
         """
         return pulumi.get(self, "namespace")
 
     @namespace.setter
     def namespace(self, value: pulumi.Input[str]):
         pulumi.set(self, "namespace", value)
 
     @property
     @pulumi.getter(name="defaultAction")
     def default_action(self) -> Optional[pulumi.Input[str]]:
         """
-        Controls the SignalFx default behavior for processing data from an AWS namespace. If you do specify a filter, use this property to control how SignalFx treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
+        Controls the Splunk Observability default behavior for processing data from an AWS namespace. Splunk Observability ignores this property unless you specify the `filter_action` and `filter_source` properties. If you do specify them, use this property to control how Splunk Observability treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
         """
         return pulumi.get(self, "default_action")
 
     @default_action.setter
     def default_action(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_action", value)
 
     @property
     @pulumi.getter(name="filterAction")
     def filter_action(self) -> Optional[pulumi.Input[str]]:
         """
-        Controls how SignalFx processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
+        Controls how Splunk Observability processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
         """
         return pulumi.get(self, "filter_action")
 
     @filter_action.setter
     def filter_action(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "filter_action", value)
 
     @property
     @pulumi.getter(name="filterSource")
     def filter_source(self) -> Optional[pulumi.Input[str]]:
         """
-        Expression that selects the data that SignalFx should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
+        Expression that selects the data that Splunk Observability should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
         """
         return pulumi.get(self, "filter_source")
 
     @filter_source.setter
     def filter_source(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "filter_source", value)
 
 
-@pulumi.input_type
-class GetServicesServiceArgs:
-    def __init__(__self__, *,
-                 name: str):
-        pulumi.set(__self__, "name", name)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: str):
-        pulumi.set(self, "name", value)
-
-
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/external_integration.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/aws/external_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                  external_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  signalfx_aws_account: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ExternalIntegration resources.
         :param pulumi.Input[str] external_id: The external ID to use with your IAM role and with `aws.Integration`.
         :param pulumi.Input[str] name: The name of this integration
-        :param pulumi.Input[str] signalfx_aws_account: The AWS Account ARN to use with your policies/roles, provided by SignalFx.
+        :param pulumi.Input[str] signalfx_aws_account: The AWS Account ARN to use with your policies/roles, provided by Splunk Observability.
         """
         if external_id is not None:
             pulumi.set(__self__, "external_id", external_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if signalfx_aws_account is not None:
             pulumi.set(__self__, "signalfx_aws_account", signalfx_aws_account)
@@ -78,15 +78,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="signalfxAwsAccount")
     def signalfx_aws_account(self) -> Optional[pulumi.Input[str]]:
         """
-        The AWS Account ARN to use with your policies/roles, provided by SignalFx.
+        The AWS Account ARN to use with your policies/roles, provided by Splunk Observability.
         """
         return pulumi.get(self, "signalfx_aws_account")
 
     @signalfx_aws_account.setter
     def signalfx_aws_account(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "signalfx_aws_account", value)
 
@@ -95,19 +95,19 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        SignalFx AWS CloudWatch integrations using Role ARNs. For help with this integration see [Connect to AWS CloudWatch](https://docs.signalfx.com/en/latest/integrations/amazon-web-services.html#connect-to-aws).
+        Splunk Observability AWS CloudWatch integrations using Role ARNs. For help with this integration see [Connect to AWS CloudWatch](https://docs.signalfx.com/en/latest/integrations/amazon-web-services.html#connect-to-aws).
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the Splunk Observability provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
 
-        > **WARNING** This resource implements a part of a workflow. You must use it with `aws.Integration`. Check with SignalFx support for your realm's AWS account id.
+        > **WARNING** This resource implements a part of a workflow. You must use it with `aws.Integration`. Check with Splunk Observability support for your realm's AWS account id.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_aws as aws
         import pulumi_signalfx as signalfx
@@ -230,19 +230,19 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ExternalIntegrationArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        SignalFx AWS CloudWatch integrations using Role ARNs. For help with this integration see [Connect to AWS CloudWatch](https://docs.signalfx.com/en/latest/integrations/amazon-web-services.html#connect-to-aws).
+        Splunk Observability AWS CloudWatch integrations using Role ARNs. For help with this integration see [Connect to AWS CloudWatch](https://docs.signalfx.com/en/latest/integrations/amazon-web-services.html#connect-to-aws).
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the Splunk Observability provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
 
-        > **WARNING** This resource implements a part of a workflow. You must use it with `aws.Integration`. Check with SignalFx support for your realm's AWS account id.
+        > **WARNING** This resource implements a part of a workflow. You must use it with `aws.Integration`. Check with Splunk Observability support for your realm's AWS account id.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_aws as aws
         import pulumi_signalfx as signalfx
@@ -406,15 +406,15 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] external_id: The external ID to use with your IAM role and with `aws.Integration`.
         :param pulumi.Input[str] name: The name of this integration
-        :param pulumi.Input[str] signalfx_aws_account: The AWS Account ARN to use with your policies/roles, provided by SignalFx.
+        :param pulumi.Input[str] signalfx_aws_account: The AWS Account ARN to use with your policies/roles, provided by Splunk Observability.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ExternalIntegrationState.__new__(_ExternalIntegrationState)
 
         __props__.__dict__["external_id"] = external_id
         __props__.__dict__["name"] = name
@@ -437,11 +437,11 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="signalfxAwsAccount")
     def signalfx_aws_account(self) -> pulumi.Output[str]:
         """
-        The AWS Account ARN to use with your policies/roles, provided by SignalFx.
+        The AWS Account ARN to use with your policies/roles, provided by Splunk Observability.
         """
         return pulumi.get(self, "signalfx_aws_account")
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/integration.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/aws/integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,38 +31,36 @@
                  namespace_sync_rules: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationNamespaceSyncRuleArgs']]]] = None,
                  poll_rate: Optional[pulumi.Input[int]] = None,
                  regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  role_arn: Optional[pulumi.Input[str]] = None,
                  services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  sync_custom_namespaces_only: Optional[pulumi.Input[bool]] = None,
                  token: Optional[pulumi.Input[str]] = None,
-                 use_get_metric_data_method: Optional[pulumi.Input[bool]] = None,
                  use_metric_streams_sync: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Integration resource.
         :param pulumi.Input[bool] enabled: Whether the integration is enabled.
         :param pulumi.Input[str] integration_id: The id of one of a `aws.ExternalIntegration` or `aws.TokenIntegration`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_cloudwatch_namespaces: List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS; SignalFx imports the metrics so you can monitor them.
-        :param pulumi.Input[Sequence[pulumi.Input['IntegrationCustomNamespaceSyncRuleArgs']]] custom_namespace_sync_rules: Each element controls the data collected by SignalFx for the specified namespace. Conflicts with the `custom_cloudwatch_namespaces` property.
-        :param pulumi.Input[bool] enable_aws_usage: Flag that controls how SignalFx imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`, SignalFx imports the metrics.
-        :param pulumi.Input[bool] enable_check_large_volume: Controls how SignalFx checks for large amounts of data for this AWS integration. If `true`, SignalFx monitors the amount of data coming in from the integration.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_cloudwatch_namespaces: List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS; Splunk Observability imports the metrics so you can monitor them.
+        :param pulumi.Input[Sequence[pulumi.Input['IntegrationCustomNamespaceSyncRuleArgs']]] custom_namespace_sync_rules: Each element controls the data collected by Splunk Observability for the specified namespace. Conflicts with the `custom_cloudwatch_namespaces` property.
+        :param pulumi.Input[bool] enable_aws_usage: Flag that controls how Splunk Observability imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`, Splunk Observability imports the metrics.
+        :param pulumi.Input[bool] enable_check_large_volume: Controls how Splunk Observability checks for large amounts of data for this AWS integration. If `true`, Splunk Observability monitors the amount of data coming in from the integration.
         :param pulumi.Input[bool] enable_logs_sync: Enable the AWS logs synchronization. Note that this requires the inclusion of `"logs:DescribeLogGroups"`,  `"logs:DeleteSubscriptionFilter"`, `"logs:DescribeSubscriptionFilters"`, `"logs:PutSubscriptionFilter"`, and `"s3:GetBucketLogging"`,  `"s3:GetBucketNotification"`, `"s3:PutBucketNotification"` permissions. Additional permissions may be required to capture logs from specific AWS services.
         :param pulumi.Input[str] external_id: The `external_id` property from one of a `aws.ExternalIntegration` or `aws.TokenIntegration`
-        :param pulumi.Input[bool] import_cloud_watch: Flag that controls how SignalFx imports Cloud Watch metrics. If true, SignalFx imports Cloud Watch metrics from AWS.
+        :param pulumi.Input[bool] import_cloud_watch: Flag that controls how Splunk Observability imports Cloud Watch metrics. If true, Splunk Observability imports Cloud Watch metrics from AWS.
         :param pulumi.Input[str] key: If you specify `auth_method = \\"SecurityToken\\"` in your request to create an AWS integration object, use this property to specify the key (this is typically equivalent to the `AWS_SECRET_ACCESS_KEY` environment variable).
-        :param pulumi.Input[Sequence[pulumi.Input['IntegrationMetricStatsToSyncArgs']]] metric_stats_to_syncs: Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics that SignalFx collects for this metric. If you specify this property, SignalFx retrieves only specified AWS statistics when AWS metric streams are not used. When AWS metric streams are used this property specifies additional extended statistics to collect (please note that AWS metric streams API supports percentile stats only; other stats are ignored). If you don't specify this property, SignalFx retrieves the AWS standard set of statistics.
+        :param pulumi.Input[Sequence[pulumi.Input['IntegrationMetricStatsToSyncArgs']]] metric_stats_to_syncs: Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics that Splunk Observability collects for this metric. If you specify this property, Splunk Observability retrieves only specified AWS statistics when AWS metric streams are not used. When AWS metric streams are used this property specifies additional extended statistics to collect (please note that AWS metric streams API supports percentile stats only; other stats are ignored). If you don't specify this property, Splunk Observability retrieves the AWS standard set of statistics.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
-        :param pulumi.Input[Sequence[pulumi.Input['IntegrationNamespaceSyncRuleArgs']]] namespace_sync_rules: Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that SignalFx collects for the namespace. Conflicts with the `services` property. If you don't specify either property, SignalFx syncs all data in all AWS namespaces.
+        :param pulumi.Input[Sequence[pulumi.Input['IntegrationNamespaceSyncRuleArgs']]] namespace_sync_rules: Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that Splunk Observability collects for the namespace. Conflicts with the `services` property. If you don't specify either property, Splunk Observability syncs all data in all AWS namespaces.
         :param pulumi.Input[int] poll_rate: AWS poll rate (in seconds). Value between `60` and `600`. Default: `300`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: List of AWS regions that SignalFx should monitor.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: List of AWS regions that Splunk Observability should monitor.
         :param pulumi.Input[str] role_arn: Role ARN that you add to an existing AWS integration object. **Note**: Ensure you use the `arn` property of your role, not the id!
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of AWS services that you want SignalFx to monitor. Each element is a string designating an AWS service. Conflicts with `namespace_sync_rule`. See the documentation for [Creating Integrations](https://developers.signalfx.com/integrations_reference.html#operation/Create%20Integration) for valida values.
-        :param pulumi.Input[bool] sync_custom_namespaces_only: Indicates that SignalFx should sync metrics and metadata from custom AWS namespaces only (see the `custom_namespace_sync_rule` above). Defaults to `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of AWS services that you want Splunk Observability to monitor. Each element is a string designating an AWS service. Can be an empty list to import data for all supported services. Conflicts with `namespace_sync_rule`. See [Amazon Web Services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#amazon-web-services) for a list of valid values.
+        :param pulumi.Input[bool] sync_custom_namespaces_only: Indicates that Splunk Observability should sync metrics and metadata from custom AWS namespaces only (see the `custom_namespace_sync_rule` above). Defaults to `false`.
         :param pulumi.Input[str] token: If you specify `auth_method = \\"SecurityToken\\"` in your request to create an AWS integration object, use this property to specify the token (this is typically equivalent to the `AWS_ACCESS_KEY_ID` environment variable).
-        :param pulumi.Input[bool] use_get_metric_data_method: Enable the use of Amazon's `GetMetricData` for collecting metrics. Note that this requires the inclusion of the `"cloudwatch:GetMetricData"` permission.
         :param pulumi.Input[bool] use_metric_streams_sync: Enable the use of Amazon Cloudwatch Metric Streams for ingesting metrics.<br>
                Note that this requires the inclusion of `"cloudwatch:ListMetricStreams"`,`"cloudwatch:GetMetricStream"`, `"cloudwatch:PutMetricStream"`, `"cloudwatch:DeleteMetricStream"`, `"cloudwatch:StartMetricStreams"`, `"cloudwatch:StopMetricStreams"` and `"iam:PassRole"` permissions.<br>
                Note you need to deploy additional resources on your AWS account to enable CloudWatch metrics streaming. Select one of the [CloudFormation templates](https://docs.splunk.com/Observability/gdi/get-data-in/connect/aws/aws-cloudformation.html) to deploy all the required resources.
         """
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "integration_id", integration_id)
         if custom_cloudwatch_namespaces is not None:
@@ -95,16 +93,14 @@
             pulumi.set(__self__, "role_arn", role_arn)
         if services is not None:
             pulumi.set(__self__, "services", services)
         if sync_custom_namespaces_only is not None:
             pulumi.set(__self__, "sync_custom_namespaces_only", sync_custom_namespaces_only)
         if token is not None:
             pulumi.set(__self__, "token", token)
-        if use_get_metric_data_method is not None:
-            pulumi.set(__self__, "use_get_metric_data_method", use_get_metric_data_method)
         if use_metric_streams_sync is not None:
             pulumi.set(__self__, "use_metric_streams_sync", use_metric_streams_sync)
 
     @property
     @pulumi.getter
     def enabled(self) -> pulumi.Input[bool]:
         """
@@ -128,51 +124,51 @@
     def integration_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "integration_id", value)
 
     @property
     @pulumi.getter(name="customCloudwatchNamespaces")
     def custom_cloudwatch_namespaces(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS; SignalFx imports the metrics so you can monitor them.
+        List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS; Splunk Observability imports the metrics so you can monitor them.
         """
         return pulumi.get(self, "custom_cloudwatch_namespaces")
 
     @custom_cloudwatch_namespaces.setter
     def custom_cloudwatch_namespaces(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "custom_cloudwatch_namespaces", value)
 
     @property
     @pulumi.getter(name="customNamespaceSyncRules")
     def custom_namespace_sync_rules(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationCustomNamespaceSyncRuleArgs']]]]:
         """
-        Each element controls the data collected by SignalFx for the specified namespace. Conflicts with the `custom_cloudwatch_namespaces` property.
+        Each element controls the data collected by Splunk Observability for the specified namespace. Conflicts with the `custom_cloudwatch_namespaces` property.
         """
         return pulumi.get(self, "custom_namespace_sync_rules")
 
     @custom_namespace_sync_rules.setter
     def custom_namespace_sync_rules(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationCustomNamespaceSyncRuleArgs']]]]):
         pulumi.set(self, "custom_namespace_sync_rules", value)
 
     @property
     @pulumi.getter(name="enableAwsUsage")
     def enable_aws_usage(self) -> Optional[pulumi.Input[bool]]:
         """
-        Flag that controls how SignalFx imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`, SignalFx imports the metrics.
+        Flag that controls how Splunk Observability imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`, Splunk Observability imports the metrics.
         """
         return pulumi.get(self, "enable_aws_usage")
 
     @enable_aws_usage.setter
     def enable_aws_usage(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_aws_usage", value)
 
     @property
     @pulumi.getter(name="enableCheckLargeVolume")
     def enable_check_large_volume(self) -> Optional[pulumi.Input[bool]]:
         """
-        Controls how SignalFx checks for large amounts of data for this AWS integration. If `true`, SignalFx monitors the amount of data coming in from the integration.
+        Controls how Splunk Observability checks for large amounts of data for this AWS integration. If `true`, Splunk Observability monitors the amount of data coming in from the integration.
         """
         return pulumi.get(self, "enable_check_large_volume")
 
     @enable_check_large_volume.setter
     def enable_check_large_volume(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_check_large_volume", value)
 
@@ -200,15 +196,15 @@
     def external_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "external_id", value)
 
     @property
     @pulumi.getter(name="importCloudWatch")
     def import_cloud_watch(self) -> Optional[pulumi.Input[bool]]:
         """
-        Flag that controls how SignalFx imports Cloud Watch metrics. If true, SignalFx imports Cloud Watch metrics from AWS.
+        Flag that controls how Splunk Observability imports Cloud Watch metrics. If true, Splunk Observability imports Cloud Watch metrics from AWS.
         """
         return pulumi.get(self, "import_cloud_watch")
 
     @import_cloud_watch.setter
     def import_cloud_watch(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "import_cloud_watch", value)
 
@@ -224,15 +220,15 @@
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter(name="metricStatsToSyncs")
     def metric_stats_to_syncs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationMetricStatsToSyncArgs']]]]:
         """
-        Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics that SignalFx collects for this metric. If you specify this property, SignalFx retrieves only specified AWS statistics when AWS metric streams are not used. When AWS metric streams are used this property specifies additional extended statistics to collect (please note that AWS metric streams API supports percentile stats only; other stats are ignored). If you don't specify this property, SignalFx retrieves the AWS standard set of statistics.
+        Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics that Splunk Observability collects for this metric. If you specify this property, Splunk Observability retrieves only specified AWS statistics when AWS metric streams are not used. When AWS metric streams are used this property specifies additional extended statistics to collect (please note that AWS metric streams API supports percentile stats only; other stats are ignored). If you don't specify this property, Splunk Observability retrieves the AWS standard set of statistics.
         """
         return pulumi.get(self, "metric_stats_to_syncs")
 
     @metric_stats_to_syncs.setter
     def metric_stats_to_syncs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationMetricStatsToSyncArgs']]]]):
         pulumi.set(self, "metric_stats_to_syncs", value)
 
@@ -248,15 +244,15 @@
     def named_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "named_token", value)
 
     @property
     @pulumi.getter(name="namespaceSyncRules")
     def namespace_sync_rules(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationNamespaceSyncRuleArgs']]]]:
         """
-        Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that SignalFx collects for the namespace. Conflicts with the `services` property. If you don't specify either property, SignalFx syncs all data in all AWS namespaces.
+        Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that Splunk Observability collects for the namespace. Conflicts with the `services` property. If you don't specify either property, Splunk Observability syncs all data in all AWS namespaces.
         """
         return pulumi.get(self, "namespace_sync_rules")
 
     @namespace_sync_rules.setter
     def namespace_sync_rules(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationNamespaceSyncRuleArgs']]]]):
         pulumi.set(self, "namespace_sync_rules", value)
 
@@ -272,15 +268,15 @@
     def poll_rate(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "poll_rate", value)
 
     @property
     @pulumi.getter
     def regions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of AWS regions that SignalFx should monitor.
+        List of AWS regions that Splunk Observability should monitor.
         """
         return pulumi.get(self, "regions")
 
     @regions.setter
     def regions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "regions", value)
 
@@ -296,27 +292,27 @@
     def role_arn(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "role_arn", value)
 
     @property
     @pulumi.getter
     def services(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of AWS services that you want SignalFx to monitor. Each element is a string designating an AWS service. Conflicts with `namespace_sync_rule`. See the documentation for [Creating Integrations](https://developers.signalfx.com/integrations_reference.html#operation/Create%20Integration) for valida values.
+        List of AWS services that you want Splunk Observability to monitor. Each element is a string designating an AWS service. Can be an empty list to import data for all supported services. Conflicts with `namespace_sync_rule`. See [Amazon Web Services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#amazon-web-services) for a list of valid values.
         """
         return pulumi.get(self, "services")
 
     @services.setter
     def services(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "services", value)
 
     @property
     @pulumi.getter(name="syncCustomNamespacesOnly")
     def sync_custom_namespaces_only(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates that SignalFx should sync metrics and metadata from custom AWS namespaces only (see the `custom_namespace_sync_rule` above). Defaults to `false`.
+        Indicates that Splunk Observability should sync metrics and metadata from custom AWS namespaces only (see the `custom_namespace_sync_rule` above). Defaults to `false`.
         """
         return pulumi.get(self, "sync_custom_namespaces_only")
 
     @sync_custom_namespaces_only.setter
     def sync_custom_namespaces_only(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "sync_custom_namespaces_only", value)
 
@@ -329,26 +325,14 @@
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "token", value)
 
     @property
-    @pulumi.getter(name="useGetMetricDataMethod")
-    def use_get_metric_data_method(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable the use of Amazon's `GetMetricData` for collecting metrics. Note that this requires the inclusion of the `"cloudwatch:GetMetricData"` permission.
-        """
-        return pulumi.get(self, "use_get_metric_data_method")
-
-    @use_get_metric_data_method.setter
-    def use_get_metric_data_method(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "use_get_metric_data_method", value)
-
-    @property
     @pulumi.getter(name="useMetricStreamsSync")
     def use_metric_streams_sync(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable the use of Amazon Cloudwatch Metric Streams for ingesting metrics.<br>
         Note that this requires the inclusion of `"cloudwatch:ListMetricStreams"`,`"cloudwatch:GetMetricStream"`, `"cloudwatch:PutMetricStream"`, `"cloudwatch:DeleteMetricStream"`, `"cloudwatch:StartMetricStreams"`, `"cloudwatch:StopMetricStreams"` and `"iam:PassRole"` permissions.<br>
         Note you need to deploy additional resources on your AWS account to enable CloudWatch metrics streaming. Select one of the [CloudFormation templates](https://docs.splunk.com/Observability/gdi/get-data-in/connect/aws/aws-cloudformation.html) to deploy all the required resources.
         """
@@ -358,61 +342,66 @@
     def use_metric_streams_sync(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "use_metric_streams_sync", value)
 
 
 @pulumi.input_type
 class _IntegrationState:
     def __init__(__self__, *,
+                 auth_method: Optional[pulumi.Input[str]] = None,
                  custom_cloudwatch_namespaces: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  custom_namespace_sync_rules: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationCustomNamespaceSyncRuleArgs']]]] = None,
                  enable_aws_usage: Optional[pulumi.Input[bool]] = None,
                  enable_check_large_volume: Optional[pulumi.Input[bool]] = None,
                  enable_logs_sync: Optional[pulumi.Input[bool]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  external_id: Optional[pulumi.Input[str]] = None,
                  import_cloud_watch: Optional[pulumi.Input[bool]] = None,
                  integration_id: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  metric_stats_to_syncs: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationMetricStatsToSyncArgs']]]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
                  named_token: Optional[pulumi.Input[str]] = None,
                  namespace_sync_rules: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationNamespaceSyncRuleArgs']]]] = None,
                  poll_rate: Optional[pulumi.Input[int]] = None,
                  regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  role_arn: Optional[pulumi.Input[str]] = None,
                  services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  sync_custom_namespaces_only: Optional[pulumi.Input[bool]] = None,
                  token: Optional[pulumi.Input[str]] = None,
-                 use_get_metric_data_method: Optional[pulumi.Input[bool]] = None,
                  use_metric_streams_sync: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering Integration resources.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_cloudwatch_namespaces: List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS; SignalFx imports the metrics so you can monitor them.
-        :param pulumi.Input[Sequence[pulumi.Input['IntegrationCustomNamespaceSyncRuleArgs']]] custom_namespace_sync_rules: Each element controls the data collected by SignalFx for the specified namespace. Conflicts with the `custom_cloudwatch_namespaces` property.
-        :param pulumi.Input[bool] enable_aws_usage: Flag that controls how SignalFx imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`, SignalFx imports the metrics.
-        :param pulumi.Input[bool] enable_check_large_volume: Controls how SignalFx checks for large amounts of data for this AWS integration. If `true`, SignalFx monitors the amount of data coming in from the integration.
+        :param pulumi.Input[str] auth_method: The mechanism used to authenticate with AWS. Use one of `signalfx_aws_external_integration` or
+               `signalfx_aws_token_integration` to define this
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_cloudwatch_namespaces: List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS; Splunk Observability imports the metrics so you can monitor them.
+        :param pulumi.Input[Sequence[pulumi.Input['IntegrationCustomNamespaceSyncRuleArgs']]] custom_namespace_sync_rules: Each element controls the data collected by Splunk Observability for the specified namespace. Conflicts with the `custom_cloudwatch_namespaces` property.
+        :param pulumi.Input[bool] enable_aws_usage: Flag that controls how Splunk Observability imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`, Splunk Observability imports the metrics.
+        :param pulumi.Input[bool] enable_check_large_volume: Controls how Splunk Observability checks for large amounts of data for this AWS integration. If `true`, Splunk Observability monitors the amount of data coming in from the integration.
         :param pulumi.Input[bool] enable_logs_sync: Enable the AWS logs synchronization. Note that this requires the inclusion of `"logs:DescribeLogGroups"`,  `"logs:DeleteSubscriptionFilter"`, `"logs:DescribeSubscriptionFilters"`, `"logs:PutSubscriptionFilter"`, and `"s3:GetBucketLogging"`,  `"s3:GetBucketNotification"`, `"s3:PutBucketNotification"` permissions. Additional permissions may be required to capture logs from specific AWS services.
         :param pulumi.Input[bool] enabled: Whether the integration is enabled.
         :param pulumi.Input[str] external_id: The `external_id` property from one of a `aws.ExternalIntegration` or `aws.TokenIntegration`
-        :param pulumi.Input[bool] import_cloud_watch: Flag that controls how SignalFx imports Cloud Watch metrics. If true, SignalFx imports Cloud Watch metrics from AWS.
+        :param pulumi.Input[bool] import_cloud_watch: Flag that controls how Splunk Observability imports Cloud Watch metrics. If true, Splunk Observability imports Cloud Watch metrics from AWS.
         :param pulumi.Input[str] integration_id: The id of one of a `aws.ExternalIntegration` or `aws.TokenIntegration`.
         :param pulumi.Input[str] key: If you specify `auth_method = \\"SecurityToken\\"` in your request to create an AWS integration object, use this property to specify the key (this is typically equivalent to the `AWS_SECRET_ACCESS_KEY` environment variable).
-        :param pulumi.Input[Sequence[pulumi.Input['IntegrationMetricStatsToSyncArgs']]] metric_stats_to_syncs: Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics that SignalFx collects for this metric. If you specify this property, SignalFx retrieves only specified AWS statistics when AWS metric streams are not used. When AWS metric streams are used this property specifies additional extended statistics to collect (please note that AWS metric streams API supports percentile stats only; other stats are ignored). If you don't specify this property, SignalFx retrieves the AWS standard set of statistics.
+        :param pulumi.Input[Sequence[pulumi.Input['IntegrationMetricStatsToSyncArgs']]] metric_stats_to_syncs: Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics that Splunk Observability collects for this metric. If you specify this property, Splunk Observability retrieves only specified AWS statistics when AWS metric streams are not used. When AWS metric streams are used this property specifies additional extended statistics to collect (please note that AWS metric streams API supports percentile stats only; other stats are ignored). If you don't specify this property, Splunk Observability retrieves the AWS standard set of statistics.
+        :param pulumi.Input[str] name: Name of the integration.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
-        :param pulumi.Input[Sequence[pulumi.Input['IntegrationNamespaceSyncRuleArgs']]] namespace_sync_rules: Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that SignalFx collects for the namespace. Conflicts with the `services` property. If you don't specify either property, SignalFx syncs all data in all AWS namespaces.
+        :param pulumi.Input[Sequence[pulumi.Input['IntegrationNamespaceSyncRuleArgs']]] namespace_sync_rules: Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that Splunk Observability collects for the namespace. Conflicts with the `services` property. If you don't specify either property, Splunk Observability syncs all data in all AWS namespaces.
         :param pulumi.Input[int] poll_rate: AWS poll rate (in seconds). Value between `60` and `600`. Default: `300`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: List of AWS regions that SignalFx should monitor.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: List of AWS regions that Splunk Observability should monitor.
         :param pulumi.Input[str] role_arn: Role ARN that you add to an existing AWS integration object. **Note**: Ensure you use the `arn` property of your role, not the id!
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of AWS services that you want SignalFx to monitor. Each element is a string designating an AWS service. Conflicts with `namespace_sync_rule`. See the documentation for [Creating Integrations](https://developers.signalfx.com/integrations_reference.html#operation/Create%20Integration) for valida values.
-        :param pulumi.Input[bool] sync_custom_namespaces_only: Indicates that SignalFx should sync metrics and metadata from custom AWS namespaces only (see the `custom_namespace_sync_rule` above). Defaults to `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of AWS services that you want Splunk Observability to monitor. Each element is a string designating an AWS service. Can be an empty list to import data for all supported services. Conflicts with `namespace_sync_rule`. See [Amazon Web Services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#amazon-web-services) for a list of valid values.
+        :param pulumi.Input[bool] sync_custom_namespaces_only: Indicates that Splunk Observability should sync metrics and metadata from custom AWS namespaces only (see the `custom_namespace_sync_rule` above). Defaults to `false`.
         :param pulumi.Input[str] token: If you specify `auth_method = \\"SecurityToken\\"` in your request to create an AWS integration object, use this property to specify the token (this is typically equivalent to the `AWS_ACCESS_KEY_ID` environment variable).
-        :param pulumi.Input[bool] use_get_metric_data_method: Enable the use of Amazon's `GetMetricData` for collecting metrics. Note that this requires the inclusion of the `"cloudwatch:GetMetricData"` permission.
         :param pulumi.Input[bool] use_metric_streams_sync: Enable the use of Amazon Cloudwatch Metric Streams for ingesting metrics.<br>
                Note that this requires the inclusion of `"cloudwatch:ListMetricStreams"`,`"cloudwatch:GetMetricStream"`, `"cloudwatch:PutMetricStream"`, `"cloudwatch:DeleteMetricStream"`, `"cloudwatch:StartMetricStreams"`, `"cloudwatch:StopMetricStreams"` and `"iam:PassRole"` permissions.<br>
                Note you need to deploy additional resources on your AWS account to enable CloudWatch metrics streaming. Select one of the [CloudFormation templates](https://docs.splunk.com/Observability/gdi/get-data-in/connect/aws/aws-cloudformation.html) to deploy all the required resources.
         """
+        if auth_method is not None:
+            pulumi.set(__self__, "auth_method", auth_method)
         if custom_cloudwatch_namespaces is not None:
             pulumi.set(__self__, "custom_cloudwatch_namespaces", custom_cloudwatch_namespaces)
         if custom_namespace_sync_rules is not None:
             pulumi.set(__self__, "custom_namespace_sync_rules", custom_namespace_sync_rules)
         if enable_aws_usage is not None:
             pulumi.set(__self__, "enable_aws_usage", enable_aws_usage)
         if enable_check_large_volume is not None:
@@ -427,14 +416,16 @@
             pulumi.set(__self__, "import_cloud_watch", import_cloud_watch)
         if integration_id is not None:
             pulumi.set(__self__, "integration_id", integration_id)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if metric_stats_to_syncs is not None:
             pulumi.set(__self__, "metric_stats_to_syncs", metric_stats_to_syncs)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
         if named_token is not None:
             pulumi.set(__self__, "named_token", named_token)
         if namespace_sync_rules is not None:
             pulumi.set(__self__, "namespace_sync_rules", namespace_sync_rules)
         if poll_rate is not None:
             pulumi.set(__self__, "poll_rate", poll_rate)
         if regions is not None:
@@ -443,60 +434,71 @@
             pulumi.set(__self__, "role_arn", role_arn)
         if services is not None:
             pulumi.set(__self__, "services", services)
         if sync_custom_namespaces_only is not None:
             pulumi.set(__self__, "sync_custom_namespaces_only", sync_custom_namespaces_only)
         if token is not None:
             pulumi.set(__self__, "token", token)
-        if use_get_metric_data_method is not None:
-            pulumi.set(__self__, "use_get_metric_data_method", use_get_metric_data_method)
         if use_metric_streams_sync is not None:
             pulumi.set(__self__, "use_metric_streams_sync", use_metric_streams_sync)
 
     @property
+    @pulumi.getter(name="authMethod")
+    def auth_method(self) -> Optional[pulumi.Input[str]]:
+        """
+        The mechanism used to authenticate with AWS. Use one of `signalfx_aws_external_integration` or
+        `signalfx_aws_token_integration` to define this
+        """
+        return pulumi.get(self, "auth_method")
+
+    @auth_method.setter
+    def auth_method(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "auth_method", value)
+
+    @property
     @pulumi.getter(name="customCloudwatchNamespaces")
     def custom_cloudwatch_namespaces(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS; SignalFx imports the metrics so you can monitor them.
+        List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS; Splunk Observability imports the metrics so you can monitor them.
         """
         return pulumi.get(self, "custom_cloudwatch_namespaces")
 
     @custom_cloudwatch_namespaces.setter
     def custom_cloudwatch_namespaces(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "custom_cloudwatch_namespaces", value)
 
     @property
     @pulumi.getter(name="customNamespaceSyncRules")
     def custom_namespace_sync_rules(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationCustomNamespaceSyncRuleArgs']]]]:
         """
-        Each element controls the data collected by SignalFx for the specified namespace. Conflicts with the `custom_cloudwatch_namespaces` property.
+        Each element controls the data collected by Splunk Observability for the specified namespace. Conflicts with the `custom_cloudwatch_namespaces` property.
         """
         return pulumi.get(self, "custom_namespace_sync_rules")
 
     @custom_namespace_sync_rules.setter
     def custom_namespace_sync_rules(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationCustomNamespaceSyncRuleArgs']]]]):
         pulumi.set(self, "custom_namespace_sync_rules", value)
 
     @property
     @pulumi.getter(name="enableAwsUsage")
     def enable_aws_usage(self) -> Optional[pulumi.Input[bool]]:
         """
-        Flag that controls how SignalFx imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`, SignalFx imports the metrics.
+        Flag that controls how Splunk Observability imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`, Splunk Observability imports the metrics.
         """
         return pulumi.get(self, "enable_aws_usage")
 
     @enable_aws_usage.setter
     def enable_aws_usage(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_aws_usage", value)
 
     @property
     @pulumi.getter(name="enableCheckLargeVolume")
     def enable_check_large_volume(self) -> Optional[pulumi.Input[bool]]:
         """
-        Controls how SignalFx checks for large amounts of data for this AWS integration. If `true`, SignalFx monitors the amount of data coming in from the integration.
+        Controls how Splunk Observability checks for large amounts of data for this AWS integration. If `true`, Splunk Observability monitors the amount of data coming in from the integration.
         """
         return pulumi.get(self, "enable_check_large_volume")
 
     @enable_check_large_volume.setter
     def enable_check_large_volume(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_check_large_volume", value)
 
@@ -536,15 +538,15 @@
     def external_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "external_id", value)
 
     @property
     @pulumi.getter(name="importCloudWatch")
     def import_cloud_watch(self) -> Optional[pulumi.Input[bool]]:
         """
-        Flag that controls how SignalFx imports Cloud Watch metrics. If true, SignalFx imports Cloud Watch metrics from AWS.
+        Flag that controls how Splunk Observability imports Cloud Watch metrics. If true, Splunk Observability imports Cloud Watch metrics from AWS.
         """
         return pulumi.get(self, "import_cloud_watch")
 
     @import_cloud_watch.setter
     def import_cloud_watch(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "import_cloud_watch", value)
 
@@ -572,23 +574,35 @@
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter(name="metricStatsToSyncs")
     def metric_stats_to_syncs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationMetricStatsToSyncArgs']]]]:
         """
-        Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics that SignalFx collects for this metric. If you specify this property, SignalFx retrieves only specified AWS statistics when AWS metric streams are not used. When AWS metric streams are used this property specifies additional extended statistics to collect (please note that AWS metric streams API supports percentile stats only; other stats are ignored). If you don't specify this property, SignalFx retrieves the AWS standard set of statistics.
+        Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics that Splunk Observability collects for this metric. If you specify this property, Splunk Observability retrieves only specified AWS statistics when AWS metric streams are not used. When AWS metric streams are used this property specifies additional extended statistics to collect (please note that AWS metric streams API supports percentile stats only; other stats are ignored). If you don't specify this property, Splunk Observability retrieves the AWS standard set of statistics.
         """
         return pulumi.get(self, "metric_stats_to_syncs")
 
     @metric_stats_to_syncs.setter
     def metric_stats_to_syncs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationMetricStatsToSyncArgs']]]]):
         pulumi.set(self, "metric_stats_to_syncs", value)
 
     @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name of the integration.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
     @pulumi.getter(name="namedToken")
     def named_token(self) -> Optional[pulumi.Input[str]]:
         """
         Name of the org token to be used for data ingestion. If not specified then default access token is used.
         """
         return pulumi.get(self, "named_token")
 
@@ -596,15 +610,15 @@
     def named_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "named_token", value)
 
     @property
     @pulumi.getter(name="namespaceSyncRules")
     def namespace_sync_rules(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationNamespaceSyncRuleArgs']]]]:
         """
-        Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that SignalFx collects for the namespace. Conflicts with the `services` property. If you don't specify either property, SignalFx syncs all data in all AWS namespaces.
+        Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that Splunk Observability collects for the namespace. Conflicts with the `services` property. If you don't specify either property, Splunk Observability syncs all data in all AWS namespaces.
         """
         return pulumi.get(self, "namespace_sync_rules")
 
     @namespace_sync_rules.setter
     def namespace_sync_rules(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationNamespaceSyncRuleArgs']]]]):
         pulumi.set(self, "namespace_sync_rules", value)
 
@@ -620,15 +634,15 @@
     def poll_rate(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "poll_rate", value)
 
     @property
     @pulumi.getter
     def regions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of AWS regions that SignalFx should monitor.
+        List of AWS regions that Splunk Observability should monitor.
         """
         return pulumi.get(self, "regions")
 
     @regions.setter
     def regions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "regions", value)
 
@@ -644,27 +658,27 @@
     def role_arn(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "role_arn", value)
 
     @property
     @pulumi.getter
     def services(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of AWS services that you want SignalFx to monitor. Each element is a string designating an AWS service. Conflicts with `namespace_sync_rule`. See the documentation for [Creating Integrations](https://developers.signalfx.com/integrations_reference.html#operation/Create%20Integration) for valida values.
+        List of AWS services that you want Splunk Observability to monitor. Each element is a string designating an AWS service. Can be an empty list to import data for all supported services. Conflicts with `namespace_sync_rule`. See [Amazon Web Services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#amazon-web-services) for a list of valid values.
         """
         return pulumi.get(self, "services")
 
     @services.setter
     def services(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "services", value)
 
     @property
     @pulumi.getter(name="syncCustomNamespacesOnly")
     def sync_custom_namespaces_only(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates that SignalFx should sync metrics and metadata from custom AWS namespaces only (see the `custom_namespace_sync_rule` above). Defaults to `false`.
+        Indicates that Splunk Observability should sync metrics and metadata from custom AWS namespaces only (see the `custom_namespace_sync_rule` above). Defaults to `false`.
         """
         return pulumi.get(self, "sync_custom_namespaces_only")
 
     @sync_custom_namespaces_only.setter
     def sync_custom_namespaces_only(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "sync_custom_namespaces_only", value)
 
@@ -677,26 +691,14 @@
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "token", value)
 
     @property
-    @pulumi.getter(name="useGetMetricDataMethod")
-    def use_get_metric_data_method(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable the use of Amazon's `GetMetricData` for collecting metrics. Note that this requires the inclusion of the `"cloudwatch:GetMetricData"` permission.
-        """
-        return pulumi.get(self, "use_get_metric_data_method")
-
-    @use_get_metric_data_method.setter
-    def use_get_metric_data_method(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "use_get_metric_data_method", value)
-
-    @property
     @pulumi.getter(name="useMetricStreamsSync")
     def use_metric_streams_sync(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable the use of Amazon Cloudwatch Metric Streams for ingesting metrics.<br>
         Note that this requires the inclusion of `"cloudwatch:ListMetricStreams"`,`"cloudwatch:GetMetricStream"`, `"cloudwatch:PutMetricStream"`, `"cloudwatch:DeleteMetricStream"`, `"cloudwatch:StartMetricStreams"`, `"cloudwatch:StopMetricStreams"` and `"iam:PassRole"` permissions.<br>
         Note you need to deploy additional resources on your AWS account to enable CloudWatch metrics streaming. Select one of the [CloudFormation templates](https://docs.splunk.com/Observability/gdi/get-data-in/connect/aws/aws-cloudformation.html) to deploy all the required resources.
         """
@@ -727,21 +729,20 @@
                  namespace_sync_rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationNamespaceSyncRuleArgs']]]]] = None,
                  poll_rate: Optional[pulumi.Input[int]] = None,
                  regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  role_arn: Optional[pulumi.Input[str]] = None,
                  services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  sync_custom_namespaces_only: Optional[pulumi.Input[bool]] = None,
                  token: Optional[pulumi.Input[str]] = None,
-                 use_get_metric_data_method: Optional[pulumi.Input[bool]] = None,
                  use_metric_streams_sync: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
-        SignalFx AWS CloudWatch integrations. For help with this integration see [Monitoring Amazon Web Services](https://docs.signalfx.com/en/latest/integrations/amazon-web-services.html#monitor-amazon-web-services).
+        Splunk Observability AWS CloudWatch integrations. For help with this integration see [Monitoring Amazon Web Services](https://docs.signalfx.com/en/latest/integrations/amazon-web-services.html#monitor-amazon-web-services).
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the Splunk Observability provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
 
         > **WARNING** This resource implements a part of a workflow. You must use it with one of either `aws.ExternalIntegration` or `aws.TokenIntegration`.
 
         ## Example Usage
 
         ```python
         import pulumi
@@ -776,54 +777,50 @@
             )],
             metric_stats_to_syncs=[signalfx.aws.IntegrationMetricStatsToSyncArgs(
                 namespace="AWS/EC2",
                 metric="NetworkPacketsIn",
                 stats=["upper"],
             )])
         ```
-        ## Service Names
-
-        > **NOTE** You can use the data source _aws_get_services_ to specify all services.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_cloudwatch_namespaces: List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS; SignalFx imports the metrics so you can monitor them.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationCustomNamespaceSyncRuleArgs']]]] custom_namespace_sync_rules: Each element controls the data collected by SignalFx for the specified namespace. Conflicts with the `custom_cloudwatch_namespaces` property.
-        :param pulumi.Input[bool] enable_aws_usage: Flag that controls how SignalFx imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`, SignalFx imports the metrics.
-        :param pulumi.Input[bool] enable_check_large_volume: Controls how SignalFx checks for large amounts of data for this AWS integration. If `true`, SignalFx monitors the amount of data coming in from the integration.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_cloudwatch_namespaces: List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS; Splunk Observability imports the metrics so you can monitor them.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationCustomNamespaceSyncRuleArgs']]]] custom_namespace_sync_rules: Each element controls the data collected by Splunk Observability for the specified namespace. Conflicts with the `custom_cloudwatch_namespaces` property.
+        :param pulumi.Input[bool] enable_aws_usage: Flag that controls how Splunk Observability imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`, Splunk Observability imports the metrics.
+        :param pulumi.Input[bool] enable_check_large_volume: Controls how Splunk Observability checks for large amounts of data for this AWS integration. If `true`, Splunk Observability monitors the amount of data coming in from the integration.
         :param pulumi.Input[bool] enable_logs_sync: Enable the AWS logs synchronization. Note that this requires the inclusion of `"logs:DescribeLogGroups"`,  `"logs:DeleteSubscriptionFilter"`, `"logs:DescribeSubscriptionFilters"`, `"logs:PutSubscriptionFilter"`, and `"s3:GetBucketLogging"`,  `"s3:GetBucketNotification"`, `"s3:PutBucketNotification"` permissions. Additional permissions may be required to capture logs from specific AWS services.
         :param pulumi.Input[bool] enabled: Whether the integration is enabled.
         :param pulumi.Input[str] external_id: The `external_id` property from one of a `aws.ExternalIntegration` or `aws.TokenIntegration`
-        :param pulumi.Input[bool] import_cloud_watch: Flag that controls how SignalFx imports Cloud Watch metrics. If true, SignalFx imports Cloud Watch metrics from AWS.
+        :param pulumi.Input[bool] import_cloud_watch: Flag that controls how Splunk Observability imports Cloud Watch metrics. If true, Splunk Observability imports Cloud Watch metrics from AWS.
         :param pulumi.Input[str] integration_id: The id of one of a `aws.ExternalIntegration` or `aws.TokenIntegration`.
         :param pulumi.Input[str] key: If you specify `auth_method = \\"SecurityToken\\"` in your request to create an AWS integration object, use this property to specify the key (this is typically equivalent to the `AWS_SECRET_ACCESS_KEY` environment variable).
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationMetricStatsToSyncArgs']]]] metric_stats_to_syncs: Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics that SignalFx collects for this metric. If you specify this property, SignalFx retrieves only specified AWS statistics when AWS metric streams are not used. When AWS metric streams are used this property specifies additional extended statistics to collect (please note that AWS metric streams API supports percentile stats only; other stats are ignored). If you don't specify this property, SignalFx retrieves the AWS standard set of statistics.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationMetricStatsToSyncArgs']]]] metric_stats_to_syncs: Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics that Splunk Observability collects for this metric. If you specify this property, Splunk Observability retrieves only specified AWS statistics when AWS metric streams are not used. When AWS metric streams are used this property specifies additional extended statistics to collect (please note that AWS metric streams API supports percentile stats only; other stats are ignored). If you don't specify this property, Splunk Observability retrieves the AWS standard set of statistics.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationNamespaceSyncRuleArgs']]]] namespace_sync_rules: Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that SignalFx collects for the namespace. Conflicts with the `services` property. If you don't specify either property, SignalFx syncs all data in all AWS namespaces.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationNamespaceSyncRuleArgs']]]] namespace_sync_rules: Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that Splunk Observability collects for the namespace. Conflicts with the `services` property. If you don't specify either property, Splunk Observability syncs all data in all AWS namespaces.
         :param pulumi.Input[int] poll_rate: AWS poll rate (in seconds). Value between `60` and `600`. Default: `300`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: List of AWS regions that SignalFx should monitor.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: List of AWS regions that Splunk Observability should monitor.
         :param pulumi.Input[str] role_arn: Role ARN that you add to an existing AWS integration object. **Note**: Ensure you use the `arn` property of your role, not the id!
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of AWS services that you want SignalFx to monitor. Each element is a string designating an AWS service. Conflicts with `namespace_sync_rule`. See the documentation for [Creating Integrations](https://developers.signalfx.com/integrations_reference.html#operation/Create%20Integration) for valida values.
-        :param pulumi.Input[bool] sync_custom_namespaces_only: Indicates that SignalFx should sync metrics and metadata from custom AWS namespaces only (see the `custom_namespace_sync_rule` above). Defaults to `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of AWS services that you want Splunk Observability to monitor. Each element is a string designating an AWS service. Can be an empty list to import data for all supported services. Conflicts with `namespace_sync_rule`. See [Amazon Web Services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#amazon-web-services) for a list of valid values.
+        :param pulumi.Input[bool] sync_custom_namespaces_only: Indicates that Splunk Observability should sync metrics and metadata from custom AWS namespaces only (see the `custom_namespace_sync_rule` above). Defaults to `false`.
         :param pulumi.Input[str] token: If you specify `auth_method = \\"SecurityToken\\"` in your request to create an AWS integration object, use this property to specify the token (this is typically equivalent to the `AWS_ACCESS_KEY_ID` environment variable).
-        :param pulumi.Input[bool] use_get_metric_data_method: Enable the use of Amazon's `GetMetricData` for collecting metrics. Note that this requires the inclusion of the `"cloudwatch:GetMetricData"` permission.
         :param pulumi.Input[bool] use_metric_streams_sync: Enable the use of Amazon Cloudwatch Metric Streams for ingesting metrics.<br>
                Note that this requires the inclusion of `"cloudwatch:ListMetricStreams"`,`"cloudwatch:GetMetricStream"`, `"cloudwatch:PutMetricStream"`, `"cloudwatch:DeleteMetricStream"`, `"cloudwatch:StartMetricStreams"`, `"cloudwatch:StopMetricStreams"` and `"iam:PassRole"` permissions.<br>
                Note you need to deploy additional resources on your AWS account to enable CloudWatch metrics streaming. Select one of the [CloudFormation templates](https://docs.splunk.com/Observability/gdi/get-data-in/connect/aws/aws-cloudformation.html) to deploy all the required resources.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IntegrationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        SignalFx AWS CloudWatch integrations. For help with this integration see [Monitoring Amazon Web Services](https://docs.signalfx.com/en/latest/integrations/amazon-web-services.html#monitor-amazon-web-services).
+        Splunk Observability AWS CloudWatch integrations. For help with this integration see [Monitoring Amazon Web Services](https://docs.signalfx.com/en/latest/integrations/amazon-web-services.html#monitor-amazon-web-services).
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the Splunk Observability provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
 
         > **WARNING** This resource implements a part of a workflow. You must use it with one of either `aws.ExternalIntegration` or `aws.TokenIntegration`.
 
         ## Example Usage
 
         ```python
         import pulumi
@@ -858,17 +855,14 @@
             )],
             metric_stats_to_syncs=[signalfx.aws.IntegrationMetricStatsToSyncArgs(
                 namespace="AWS/EC2",
                 metric="NetworkPacketsIn",
                 stats=["upper"],
             )])
         ```
-        ## Service Names
-
-        > **NOTE** You can use the data source _aws_get_services_ to specify all services.
 
         :param str resource_name: The name of the resource.
         :param IntegrationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -896,15 +890,14 @@
                  namespace_sync_rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationNamespaceSyncRuleArgs']]]]] = None,
                  poll_rate: Optional[pulumi.Input[int]] = None,
                  regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  role_arn: Optional[pulumi.Input[str]] = None,
                  services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  sync_custom_namespaces_only: Optional[pulumi.Input[bool]] = None,
                  token: Optional[pulumi.Input[str]] = None,
-                 use_get_metric_data_method: Optional[pulumi.Input[bool]] = None,
                  use_metric_streams_sync: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
@@ -930,136 +923,150 @@
             __props__.__dict__["namespace_sync_rules"] = namespace_sync_rules
             __props__.__dict__["poll_rate"] = poll_rate
             __props__.__dict__["regions"] = regions
             __props__.__dict__["role_arn"] = role_arn
             __props__.__dict__["services"] = services
             __props__.__dict__["sync_custom_namespaces_only"] = sync_custom_namespaces_only
             __props__.__dict__["token"] = token
-            __props__.__dict__["use_get_metric_data_method"] = use_get_metric_data_method
             __props__.__dict__["use_metric_streams_sync"] = use_metric_streams_sync
+            __props__.__dict__["auth_method"] = None
+            __props__.__dict__["name"] = None
         secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["externalId", "key"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Integration, __self__).__init__(
             'signalfx:aws/integration:Integration',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            auth_method: Optional[pulumi.Input[str]] = None,
             custom_cloudwatch_namespaces: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             custom_namespace_sync_rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationCustomNamespaceSyncRuleArgs']]]]] = None,
             enable_aws_usage: Optional[pulumi.Input[bool]] = None,
             enable_check_large_volume: Optional[pulumi.Input[bool]] = None,
             enable_logs_sync: Optional[pulumi.Input[bool]] = None,
             enabled: Optional[pulumi.Input[bool]] = None,
             external_id: Optional[pulumi.Input[str]] = None,
             import_cloud_watch: Optional[pulumi.Input[bool]] = None,
             integration_id: Optional[pulumi.Input[str]] = None,
             key: Optional[pulumi.Input[str]] = None,
             metric_stats_to_syncs: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationMetricStatsToSyncArgs']]]]] = None,
+            name: Optional[pulumi.Input[str]] = None,
             named_token: Optional[pulumi.Input[str]] = None,
             namespace_sync_rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationNamespaceSyncRuleArgs']]]]] = None,
             poll_rate: Optional[pulumi.Input[int]] = None,
             regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             role_arn: Optional[pulumi.Input[str]] = None,
             services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             sync_custom_namespaces_only: Optional[pulumi.Input[bool]] = None,
             token: Optional[pulumi.Input[str]] = None,
-            use_get_metric_data_method: Optional[pulumi.Input[bool]] = None,
             use_metric_streams_sync: Optional[pulumi.Input[bool]] = None) -> 'Integration':
         """
         Get an existing Integration resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_cloudwatch_namespaces: List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS; SignalFx imports the metrics so you can monitor them.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationCustomNamespaceSyncRuleArgs']]]] custom_namespace_sync_rules: Each element controls the data collected by SignalFx for the specified namespace. Conflicts with the `custom_cloudwatch_namespaces` property.
-        :param pulumi.Input[bool] enable_aws_usage: Flag that controls how SignalFx imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`, SignalFx imports the metrics.
-        :param pulumi.Input[bool] enable_check_large_volume: Controls how SignalFx checks for large amounts of data for this AWS integration. If `true`, SignalFx monitors the amount of data coming in from the integration.
+        :param pulumi.Input[str] auth_method: The mechanism used to authenticate with AWS. Use one of `signalfx_aws_external_integration` or
+               `signalfx_aws_token_integration` to define this
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] custom_cloudwatch_namespaces: List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS; Splunk Observability imports the metrics so you can monitor them.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationCustomNamespaceSyncRuleArgs']]]] custom_namespace_sync_rules: Each element controls the data collected by Splunk Observability for the specified namespace. Conflicts with the `custom_cloudwatch_namespaces` property.
+        :param pulumi.Input[bool] enable_aws_usage: Flag that controls how Splunk Observability imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`, Splunk Observability imports the metrics.
+        :param pulumi.Input[bool] enable_check_large_volume: Controls how Splunk Observability checks for large amounts of data for this AWS integration. If `true`, Splunk Observability monitors the amount of data coming in from the integration.
         :param pulumi.Input[bool] enable_logs_sync: Enable the AWS logs synchronization. Note that this requires the inclusion of `"logs:DescribeLogGroups"`,  `"logs:DeleteSubscriptionFilter"`, `"logs:DescribeSubscriptionFilters"`, `"logs:PutSubscriptionFilter"`, and `"s3:GetBucketLogging"`,  `"s3:GetBucketNotification"`, `"s3:PutBucketNotification"` permissions. Additional permissions may be required to capture logs from specific AWS services.
         :param pulumi.Input[bool] enabled: Whether the integration is enabled.
         :param pulumi.Input[str] external_id: The `external_id` property from one of a `aws.ExternalIntegration` or `aws.TokenIntegration`
-        :param pulumi.Input[bool] import_cloud_watch: Flag that controls how SignalFx imports Cloud Watch metrics. If true, SignalFx imports Cloud Watch metrics from AWS.
+        :param pulumi.Input[bool] import_cloud_watch: Flag that controls how Splunk Observability imports Cloud Watch metrics. If true, Splunk Observability imports Cloud Watch metrics from AWS.
         :param pulumi.Input[str] integration_id: The id of one of a `aws.ExternalIntegration` or `aws.TokenIntegration`.
         :param pulumi.Input[str] key: If you specify `auth_method = \\"SecurityToken\\"` in your request to create an AWS integration object, use this property to specify the key (this is typically equivalent to the `AWS_SECRET_ACCESS_KEY` environment variable).
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationMetricStatsToSyncArgs']]]] metric_stats_to_syncs: Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics that SignalFx collects for this metric. If you specify this property, SignalFx retrieves only specified AWS statistics when AWS metric streams are not used. When AWS metric streams are used this property specifies additional extended statistics to collect (please note that AWS metric streams API supports percentile stats only; other stats are ignored). If you don't specify this property, SignalFx retrieves the AWS standard set of statistics.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationMetricStatsToSyncArgs']]]] metric_stats_to_syncs: Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics that Splunk Observability collects for this metric. If you specify this property, Splunk Observability retrieves only specified AWS statistics when AWS metric streams are not used. When AWS metric streams are used this property specifies additional extended statistics to collect (please note that AWS metric streams API supports percentile stats only; other stats are ignored). If you don't specify this property, Splunk Observability retrieves the AWS standard set of statistics.
+        :param pulumi.Input[str] name: Name of the integration.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationNamespaceSyncRuleArgs']]]] namespace_sync_rules: Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that SignalFx collects for the namespace. Conflicts with the `services` property. If you don't specify either property, SignalFx syncs all data in all AWS namespaces.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationNamespaceSyncRuleArgs']]]] namespace_sync_rules: Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that Splunk Observability collects for the namespace. Conflicts with the `services` property. If you don't specify either property, Splunk Observability syncs all data in all AWS namespaces.
         :param pulumi.Input[int] poll_rate: AWS poll rate (in seconds). Value between `60` and `600`. Default: `300`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: List of AWS regions that SignalFx should monitor.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] regions: List of AWS regions that Splunk Observability should monitor.
         :param pulumi.Input[str] role_arn: Role ARN that you add to an existing AWS integration object. **Note**: Ensure you use the `arn` property of your role, not the id!
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of AWS services that you want SignalFx to monitor. Each element is a string designating an AWS service. Conflicts with `namespace_sync_rule`. See the documentation for [Creating Integrations](https://developers.signalfx.com/integrations_reference.html#operation/Create%20Integration) for valida values.
-        :param pulumi.Input[bool] sync_custom_namespaces_only: Indicates that SignalFx should sync metrics and metadata from custom AWS namespaces only (see the `custom_namespace_sync_rule` above). Defaults to `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of AWS services that you want Splunk Observability to monitor. Each element is a string designating an AWS service. Can be an empty list to import data for all supported services. Conflicts with `namespace_sync_rule`. See [Amazon Web Services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#amazon-web-services) for a list of valid values.
+        :param pulumi.Input[bool] sync_custom_namespaces_only: Indicates that Splunk Observability should sync metrics and metadata from custom AWS namespaces only (see the `custom_namespace_sync_rule` above). Defaults to `false`.
         :param pulumi.Input[str] token: If you specify `auth_method = \\"SecurityToken\\"` in your request to create an AWS integration object, use this property to specify the token (this is typically equivalent to the `AWS_ACCESS_KEY_ID` environment variable).
-        :param pulumi.Input[bool] use_get_metric_data_method: Enable the use of Amazon's `GetMetricData` for collecting metrics. Note that this requires the inclusion of the `"cloudwatch:GetMetricData"` permission.
         :param pulumi.Input[bool] use_metric_streams_sync: Enable the use of Amazon Cloudwatch Metric Streams for ingesting metrics.<br>
                Note that this requires the inclusion of `"cloudwatch:ListMetricStreams"`,`"cloudwatch:GetMetricStream"`, `"cloudwatch:PutMetricStream"`, `"cloudwatch:DeleteMetricStream"`, `"cloudwatch:StartMetricStreams"`, `"cloudwatch:StopMetricStreams"` and `"iam:PassRole"` permissions.<br>
                Note you need to deploy additional resources on your AWS account to enable CloudWatch metrics streaming. Select one of the [CloudFormation templates](https://docs.splunk.com/Observability/gdi/get-data-in/connect/aws/aws-cloudformation.html) to deploy all the required resources.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _IntegrationState.__new__(_IntegrationState)
 
+        __props__.__dict__["auth_method"] = auth_method
         __props__.__dict__["custom_cloudwatch_namespaces"] = custom_cloudwatch_namespaces
         __props__.__dict__["custom_namespace_sync_rules"] = custom_namespace_sync_rules
         __props__.__dict__["enable_aws_usage"] = enable_aws_usage
         __props__.__dict__["enable_check_large_volume"] = enable_check_large_volume
         __props__.__dict__["enable_logs_sync"] = enable_logs_sync
         __props__.__dict__["enabled"] = enabled
         __props__.__dict__["external_id"] = external_id
         __props__.__dict__["import_cloud_watch"] = import_cloud_watch
         __props__.__dict__["integration_id"] = integration_id
         __props__.__dict__["key"] = key
         __props__.__dict__["metric_stats_to_syncs"] = metric_stats_to_syncs
+        __props__.__dict__["name"] = name
         __props__.__dict__["named_token"] = named_token
         __props__.__dict__["namespace_sync_rules"] = namespace_sync_rules
         __props__.__dict__["poll_rate"] = poll_rate
         __props__.__dict__["regions"] = regions
         __props__.__dict__["role_arn"] = role_arn
         __props__.__dict__["services"] = services
         __props__.__dict__["sync_custom_namespaces_only"] = sync_custom_namespaces_only
         __props__.__dict__["token"] = token
-        __props__.__dict__["use_get_metric_data_method"] = use_get_metric_data_method
         __props__.__dict__["use_metric_streams_sync"] = use_metric_streams_sync
         return Integration(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter(name="authMethod")
+    def auth_method(self) -> pulumi.Output[str]:
+        """
+        The mechanism used to authenticate with AWS. Use one of `signalfx_aws_external_integration` or
+        `signalfx_aws_token_integration` to define this
+        """
+        return pulumi.get(self, "auth_method")
+
+    @property
     @pulumi.getter(name="customCloudwatchNamespaces")
     def custom_cloudwatch_namespaces(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS; SignalFx imports the metrics so you can monitor them.
+        List of custom AWS CloudWatch namespaces to monitor. Custom namespaces contain custom metrics that you define in AWS; Splunk Observability imports the metrics so you can monitor them.
         """
         return pulumi.get(self, "custom_cloudwatch_namespaces")
 
     @property
     @pulumi.getter(name="customNamespaceSyncRules")
     def custom_namespace_sync_rules(self) -> pulumi.Output[Optional[Sequence['outputs.IntegrationCustomNamespaceSyncRule']]]:
         """
-        Each element controls the data collected by SignalFx for the specified namespace. Conflicts with the `custom_cloudwatch_namespaces` property.
+        Each element controls the data collected by Splunk Observability for the specified namespace. Conflicts with the `custom_cloudwatch_namespaces` property.
         """
         return pulumi.get(self, "custom_namespace_sync_rules")
 
     @property
     @pulumi.getter(name="enableAwsUsage")
     def enable_aws_usage(self) -> pulumi.Output[Optional[bool]]:
         """
-        Flag that controls how SignalFx imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`, SignalFx imports the metrics.
+        Flag that controls how Splunk Observability imports usage metrics from AWS to use with AWS Cost Optimizer. If `true`, Splunk Observability imports the metrics.
         """
         return pulumi.get(self, "enable_aws_usage")
 
     @property
     @pulumi.getter(name="enableCheckLargeVolume")
     def enable_check_large_volume(self) -> pulumi.Output[Optional[bool]]:
         """
-        Controls how SignalFx checks for large amounts of data for this AWS integration. If `true`, SignalFx monitors the amount of data coming in from the integration.
+        Controls how Splunk Observability checks for large amounts of data for this AWS integration. If `true`, Splunk Observability monitors the amount of data coming in from the integration.
         """
         return pulumi.get(self, "enable_check_large_volume")
 
     @property
     @pulumi.getter(name="enableLogsSync")
     def enable_logs_sync(self) -> pulumi.Output[bool]:
         """
@@ -1083,15 +1090,15 @@
         """
         return pulumi.get(self, "external_id")
 
     @property
     @pulumi.getter(name="importCloudWatch")
     def import_cloud_watch(self) -> pulumi.Output[Optional[bool]]:
         """
-        Flag that controls how SignalFx imports Cloud Watch metrics. If true, SignalFx imports Cloud Watch metrics from AWS.
+        Flag that controls how Splunk Observability imports Cloud Watch metrics. If true, Splunk Observability imports Cloud Watch metrics from AWS.
         """
         return pulumi.get(self, "import_cloud_watch")
 
     @property
     @pulumi.getter(name="integrationId")
     def integration_id(self) -> pulumi.Output[str]:
         """
@@ -1107,31 +1114,39 @@
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter(name="metricStatsToSyncs")
     def metric_stats_to_syncs(self) -> pulumi.Output[Optional[Sequence['outputs.IntegrationMetricStatsToSync']]]:
         """
-        Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics that SignalFx collects for this metric. If you specify this property, SignalFx retrieves only specified AWS statistics when AWS metric streams are not used. When AWS metric streams are used this property specifies additional extended statistics to collect (please note that AWS metric streams API supports percentile stats only; other stats are ignored). If you don't specify this property, SignalFx retrieves the AWS standard set of statistics.
+        Each element in the array is an object that contains an AWS namespace name, AWS metric name and a list of statistics that Splunk Observability collects for this metric. If you specify this property, Splunk Observability retrieves only specified AWS statistics when AWS metric streams are not used. When AWS metric streams are used this property specifies additional extended statistics to collect (please note that AWS metric streams API supports percentile stats only; other stats are ignored). If you don't specify this property, Splunk Observability retrieves the AWS standard set of statistics.
         """
         return pulumi.get(self, "metric_stats_to_syncs")
 
     @property
+    @pulumi.getter
+    def name(self) -> pulumi.Output[str]:
+        """
+        Name of the integration.
+        """
+        return pulumi.get(self, "name")
+
+    @property
     @pulumi.getter(name="namedToken")
     def named_token(self) -> pulumi.Output[Optional[str]]:
         """
         Name of the org token to be used for data ingestion. If not specified then default access token is used.
         """
         return pulumi.get(self, "named_token")
 
     @property
     @pulumi.getter(name="namespaceSyncRules")
     def namespace_sync_rules(self) -> pulumi.Output[Optional[Sequence['outputs.IntegrationNamespaceSyncRule']]]:
         """
-        Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that SignalFx collects for the namespace. Conflicts with the `services` property. If you don't specify either property, SignalFx syncs all data in all AWS namespaces.
+        Each element in the array is an object that contains an AWS namespace name and a filter that controls the data that Splunk Observability collects for the namespace. Conflicts with the `services` property. If you don't specify either property, Splunk Observability syncs all data in all AWS namespaces.
         """
         return pulumi.get(self, "namespace_sync_rules")
 
     @property
     @pulumi.getter(name="pollRate")
     def poll_rate(self) -> pulumi.Output[Optional[int]]:
         """
@@ -1139,15 +1154,15 @@
         """
         return pulumi.get(self, "poll_rate")
 
     @property
     @pulumi.getter
     def regions(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of AWS regions that SignalFx should monitor.
+        List of AWS regions that Splunk Observability should monitor.
         """
         return pulumi.get(self, "regions")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> pulumi.Output[Optional[str]]:
         """
@@ -1155,43 +1170,35 @@
         """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter
     def services(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of AWS services that you want SignalFx to monitor. Each element is a string designating an AWS service. Conflicts with `namespace_sync_rule`. See the documentation for [Creating Integrations](https://developers.signalfx.com/integrations_reference.html#operation/Create%20Integration) for valida values.
+        List of AWS services that you want Splunk Observability to monitor. Each element is a string designating an AWS service. Can be an empty list to import data for all supported services. Conflicts with `namespace_sync_rule`. See [Amazon Web Services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#amazon-web-services) for a list of valid values.
         """
         return pulumi.get(self, "services")
 
     @property
     @pulumi.getter(name="syncCustomNamespacesOnly")
     def sync_custom_namespaces_only(self) -> pulumi.Output[Optional[bool]]:
         """
-        Indicates that SignalFx should sync metrics and metadata from custom AWS namespaces only (see the `custom_namespace_sync_rule` above). Defaults to `false`.
+        Indicates that Splunk Observability should sync metrics and metadata from custom AWS namespaces only (see the `custom_namespace_sync_rule` above). Defaults to `false`.
         """
         return pulumi.get(self, "sync_custom_namespaces_only")
 
     @property
     @pulumi.getter
     def token(self) -> pulumi.Output[Optional[str]]:
         """
         If you specify `auth_method = \\"SecurityToken\\"` in your request to create an AWS integration object, use this property to specify the token (this is typically equivalent to the `AWS_ACCESS_KEY_ID` environment variable).
         """
         return pulumi.get(self, "token")
 
     @property
-    @pulumi.getter(name="useGetMetricDataMethod")
-    def use_get_metric_data_method(self) -> pulumi.Output[Optional[bool]]:
-        """
-        Enable the use of Amazon's `GetMetricData` for collecting metrics. Note that this requires the inclusion of the `"cloudwatch:GetMetricData"` permission.
-        """
-        return pulumi.get(self, "use_get_metric_data_method")
-
-    @property
     @pulumi.getter(name="useMetricStreamsSync")
     def use_metric_streams_sync(self) -> pulumi.Output[bool]:
         """
         Enable the use of Amazon Cloudwatch Metric Streams for ingesting metrics.<br>
         Note that this requires the inclusion of `"cloudwatch:ListMetricStreams"`,`"cloudwatch:GetMetricStream"`, `"cloudwatch:PutMetricStream"`, `"cloudwatch:DeleteMetricStream"`, `"cloudwatch:StartMetricStreams"`, `"cloudwatch:StopMetricStreams"` and `"iam:PassRole"` permissions.<br>
         Note you need to deploy additional resources on your AWS account to enable CloudWatch metrics streaming. Select one of the [CloudFormation templates](https://docs.splunk.com/Observability/gdi/get-data-in/connect/aws/aws-cloudformation.html) to deploy all the required resources.
         """
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/outputs.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/aws/outputs.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
     'IntegrationCustomNamespaceSyncRule',
     'IntegrationMetricStatsToSync',
     'IntegrationNamespaceSyncRule',
-    'GetServicesServiceResult',
 ]
 
 @pulumi.output_type
 class IntegrationCustomNamespaceSyncRule(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
@@ -41,69 +40,69 @@
 
     def __init__(__self__, *,
                  namespace: str,
                  default_action: Optional[str] = None,
                  filter_action: Optional[str] = None,
                  filter_source: Optional[str] = None):
         """
-        :param str namespace: An AWS custom namespace having custom AWS metrics that you want to sync with SignalFx. See the AWS documentation on publishing metrics for more information.
-        :param str default_action: Controls the SignalFx default behavior for processing data from an AWS namespace. If you do specify a filter, use this property to control how SignalFx treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
-        :param str filter_action: Controls how SignalFx processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
-        :param str filter_source: Expression that selects the data that SignalFx should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
+        :param str namespace: An AWS custom namespace having custom AWS metrics that you want to sync with Splunk Observability. See `services` field description below for additional information.
+        :param str default_action: Controls the Splunk Observability default behavior for processing data from an AWS namespace. Splunk Observability ignores this property unless you specify the `filter_action` and `filter_source` properties. If you do specify them, use this property to control how Splunk Observability treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
+        :param str filter_action: Controls how Splunk Observability processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
+        :param str filter_source: Expression that selects the data that Splunk Observability should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
         """
         pulumi.set(__self__, "namespace", namespace)
         if default_action is not None:
             pulumi.set(__self__, "default_action", default_action)
         if filter_action is not None:
             pulumi.set(__self__, "filter_action", filter_action)
         if filter_source is not None:
             pulumi.set(__self__, "filter_source", filter_source)
 
     @property
     @pulumi.getter
     def namespace(self) -> str:
         """
-        An AWS custom namespace having custom AWS metrics that you want to sync with SignalFx. See the AWS documentation on publishing metrics for more information.
+        An AWS custom namespace having custom AWS metrics that you want to sync with Splunk Observability. See `services` field description below for additional information.
         """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter(name="defaultAction")
     def default_action(self) -> Optional[str]:
         """
-        Controls the SignalFx default behavior for processing data from an AWS namespace. If you do specify a filter, use this property to control how SignalFx treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
+        Controls the Splunk Observability default behavior for processing data from an AWS namespace. Splunk Observability ignores this property unless you specify the `filter_action` and `filter_source` properties. If you do specify them, use this property to control how Splunk Observability treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
         """
         return pulumi.get(self, "default_action")
 
     @property
     @pulumi.getter(name="filterAction")
     def filter_action(self) -> Optional[str]:
         """
-        Controls how SignalFx processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
+        Controls how Splunk Observability processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
         """
         return pulumi.get(self, "filter_action")
 
     @property
     @pulumi.getter(name="filterSource")
     def filter_source(self) -> Optional[str]:
         """
-        Expression that selects the data that SignalFx should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
+        Expression that selects the data that Splunk Observability should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
         """
         return pulumi.get(self, "filter_source")
 
 
 @pulumi.output_type
 class IntegrationMetricStatsToSync(dict):
     def __init__(__self__, *,
                  metric: str,
                  namespace: str,
                  stats: Sequence[str]):
         """
         :param str metric: AWS metric that you want to pick statistics for
-        :param str namespace: An AWS custom namespace having custom AWS metrics that you want to sync with SignalFx. See the AWS documentation on publishing metrics for more information.
+        :param str namespace: An AWS custom namespace having custom AWS metrics that you want to sync with Splunk Observability. See `services` field description below for additional information.
         :param Sequence[str] stats: AWS statistics you want to collect
         """
         pulumi.set(__self__, "metric", metric)
         pulumi.set(__self__, "namespace", namespace)
         pulumi.set(__self__, "stats", stats)
 
     @property
@@ -114,15 +113,15 @@
         """
         return pulumi.get(self, "metric")
 
     @property
     @pulumi.getter
     def namespace(self) -> str:
         """
-        An AWS custom namespace having custom AWS metrics that you want to sync with SignalFx. See the AWS documentation on publishing metrics for more information.
+        An AWS custom namespace having custom AWS metrics that you want to sync with Splunk Observability. See `services` field description below for additional information.
         """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter
     def stats(self) -> Sequence[str]:
         """
@@ -156,65 +155,53 @@
 
     def __init__(__self__, *,
                  namespace: str,
                  default_action: Optional[str] = None,
                  filter_action: Optional[str] = None,
                  filter_source: Optional[str] = None):
         """
-        :param str namespace: An AWS custom namespace having custom AWS metrics that you want to sync with SignalFx. See the AWS documentation on publishing metrics for more information.
-        :param str default_action: Controls the SignalFx default behavior for processing data from an AWS namespace. If you do specify a filter, use this property to control how SignalFx treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
-        :param str filter_action: Controls how SignalFx processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
-        :param str filter_source: Expression that selects the data that SignalFx should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
+        :param str namespace: An AWS custom namespace having custom AWS metrics that you want to sync with Splunk Observability. See `services` field description below for additional information.
+        :param str default_action: Controls the Splunk Observability default behavior for processing data from an AWS namespace. Splunk Observability ignores this property unless you specify the `filter_action` and `filter_source` properties. If you do specify them, use this property to control how Splunk Observability treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
+        :param str filter_action: Controls how Splunk Observability processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
+        :param str filter_source: Expression that selects the data that Splunk Observability should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
         """
         pulumi.set(__self__, "namespace", namespace)
         if default_action is not None:
             pulumi.set(__self__, "default_action", default_action)
         if filter_action is not None:
             pulumi.set(__self__, "filter_action", filter_action)
         if filter_source is not None:
             pulumi.set(__self__, "filter_source", filter_source)
 
     @property
     @pulumi.getter
     def namespace(self) -> str:
         """
-        An AWS custom namespace having custom AWS metrics that you want to sync with SignalFx. See the AWS documentation on publishing metrics for more information.
+        An AWS custom namespace having custom AWS metrics that you want to sync with Splunk Observability. See `services` field description below for additional information.
         """
         return pulumi.get(self, "namespace")
 
     @property
     @pulumi.getter(name="defaultAction")
     def default_action(self) -> Optional[str]:
         """
-        Controls the SignalFx default behavior for processing data from an AWS namespace. If you do specify a filter, use this property to control how SignalFx treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
+        Controls the Splunk Observability default behavior for processing data from an AWS namespace. Splunk Observability ignores this property unless you specify the `filter_action` and `filter_source` properties. If you do specify them, use this property to control how Splunk Observability treats data that doesn't match the filter. The available actions are one of `"Include"` or `"Exclude"`.
         """
         return pulumi.get(self, "default_action")
 
     @property
     @pulumi.getter(name="filterAction")
     def filter_action(self) -> Optional[str]:
         """
-        Controls how SignalFx processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
+        Controls how Splunk Observability processes data from a custom AWS namespace. The available actions are one of `"Include"` or `"Exclude"`.
         """
         return pulumi.get(self, "filter_action")
 
     @property
     @pulumi.getter(name="filterSource")
     def filter_source(self) -> Optional[str]:
         """
-        Expression that selects the data that SignalFx should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
+        Expression that selects the data that Splunk Observability should sync for the custom namespace associated with this sync rule. The expression uses the syntax defined for the SignalFlow `filter()` function; it can be any valid SignalFlow filter expression.
         """
         return pulumi.get(self, "filter_source")
 
 
-@pulumi.output_type
-class GetServicesServiceResult(dict):
-    def __init__(__self__, *,
-                 name: str):
-        pulumi.set(__self__, "name", name)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
-
-
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/aws/token_integration.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/aws/token_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     def __init__(__self__, *,
                  name: Optional[pulumi.Input[str]] = None,
                  signalfx_aws_account: Optional[pulumi.Input[str]] = None,
                  token_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering TokenIntegration resources.
         :param pulumi.Input[str] name: The name of this integration
-        :param pulumi.Input[str] signalfx_aws_account: The AWS Account ARN to use with your policies/roles, provided by SignalFx.
+        :param pulumi.Input[str] signalfx_aws_account: The AWS Account ARN to use with your policies/roles, provided by Splunk Observability.
         :param pulumi.Input[str] token_id: The SignalFx-generated AWS token to use with an AWS integration.
         """
         if name is not None:
             pulumi.set(__self__, "name", name)
         if signalfx_aws_account is not None:
             pulumi.set(__self__, "signalfx_aws_account", signalfx_aws_account)
         if token_id is not None:
@@ -66,15 +66,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="signalfxAwsAccount")
     def signalfx_aws_account(self) -> Optional[pulumi.Input[str]]:
         """
-        The AWS Account ARN to use with your policies/roles, provided by SignalFx.
+        The AWS Account ARN to use with your policies/roles, provided by Splunk Observability.
         """
         return pulumi.get(self, "signalfx_aws_account")
 
     @signalfx_aws_account.setter
     def signalfx_aws_account(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "signalfx_aws_account", value)
 
@@ -95,17 +95,17 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        SignalFx AWS CloudWatch integrations using security tokens. For help with this integration see [Connect to AWS CloudWatch](https://docs.signalfx.com/en/latest/integrations/amazon-web-services.html#connect-to-aws).
+        Splunk Observability AWS CloudWatch integrations using security tokens. For help with this integration see [Connect to AWS CloudWatch](https://docs.signalfx.com/en/latest/integrations/amazon-web-services.html#connect-to-aws).
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the Splunk Observability provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
 
         > **WARNING** This resource implements a part of a workflow. You must use it with `aws.Integration`.
 
         ## Example Usage
 
         ```python
         import pulumi
@@ -146,17 +146,17 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[TokenIntegrationArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        SignalFx AWS CloudWatch integrations using security tokens. For help with this integration see [Connect to AWS CloudWatch](https://docs.signalfx.com/en/latest/integrations/amazon-web-services.html#connect-to-aws).
+        Splunk Observability AWS CloudWatch integrations using security tokens. For help with this integration see [Connect to AWS CloudWatch](https://docs.signalfx.com/en/latest/integrations/amazon-web-services.html#connect-to-aws).
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the Splunk Observability provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
 
         > **WARNING** This resource implements a part of a workflow. You must use it with `aws.Integration`.
 
         ## Example Usage
 
         ```python
         import pulumi
@@ -237,15 +237,15 @@
         Get an existing TokenIntegration resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: The name of this integration
-        :param pulumi.Input[str] signalfx_aws_account: The AWS Account ARN to use with your policies/roles, provided by SignalFx.
+        :param pulumi.Input[str] signalfx_aws_account: The AWS Account ARN to use with your policies/roles, provided by Splunk Observability.
         :param pulumi.Input[str] token_id: The SignalFx-generated AWS token to use with an AWS integration.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _TokenIntegrationState.__new__(_TokenIntegrationState)
 
         __props__.__dict__["name"] = name
@@ -261,15 +261,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="signalfxAwsAccount")
     def signalfx_aws_account(self) -> pulumi.Output[str]:
         """
-        The AWS Account ARN to use with your policies/roles, provided by SignalFx.
+        The AWS Account ARN to use with your policies/roles, provided by Splunk Observability.
         """
         return pulumi.get(self, "signalfx_aws_account")
 
     @property
     @pulumi.getter(name="tokenId")
     def token_id(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/azure/integration.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/azure/integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,27 +32,25 @@
                  resource_filter_rules: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationResourceFilterRuleArgs']]]] = None,
                  sync_guest_os_namespaces: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Integration resource.
         :param pulumi.Input[str] app_id: Azure application ID for the SignalFx app. To learn how to get this ID, see the topic [Connect to Microsoft Azure](https://docs.signalfx.com/en/latest/getting-started/send-data.html#connect-to-microsoft-azure) in the product documentation.
         :param pulumi.Input[bool] enabled: Whether the integration is enabled.
         :param pulumi.Input[str] secret_key: Azure secret key that associates the SignalFx app in Azure with the Azure tenant ID. To learn how to get this ID, see the topic [Connect to Microsoft Azure](https://docs.signalfx.com/en/latest/integrations/azure-info.html#connect-to-azure) in the product documentation.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of Microsoft Azure service names for the Azure services you want SignalFx to monitor. See the documentation for [Creating Integrations](https://developers.signalfx.com/integrations_reference.html#operation/Create%20Integration) for valida values.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of Microsoft Azure service names for the Azure services you want SignalFx to monitor. Can be an empty list to import data for all supported services. See [Microsoft Azure services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#azure-integrations) for a list of valid values.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] subscriptions: List of Azure subscriptions that SignalFx should monitor.
         :param pulumi.Input[str] tenant_id: Azure ID of the Azure tenant. To learn how to get this ID, see the topic [Connect to Microsoft Azure](https://docs.signalfx.com/en/latest/integrations/azure-info.html#connect-to-azure) in the product documentation.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] additional_services: Additional Azure resource types that you want to sync with Observability Cloud.
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationCustomNamespacesPerServiceArgs']]] custom_namespaces_per_services: Allows for more fine-grained control of syncing of custom namespaces, should the boolean convenience parameter `sync_guest_os_namespaces` be not enough. The customer may specify a map of services to custom namespaces. If they do so, for each service which is a key in this map, we will attempt to sync metrics from namespaces in the value list in addition to the default namespaces.
         :param pulumi.Input[str] environment: What type of Azure integration this is. The allowed values are `\\"azure_us_government\\"` and `\\"azure\\"`. Defaults to `\\"azure\\"`.
         :param pulumi.Input[bool] import_azure_monitor: If enabled, SignalFx will sync also Azure Monitor data. If disabled, SignalFx will import only metadata. Defaults to true.
         :param pulumi.Input[str] name: Name of the integration.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
         :param pulumi.Input[int] poll_rate: Azure poll rate (in seconds). Value between `60` and `600`. Default: `300`.
-        :param pulumi.Input[Sequence[pulumi.Input['IntegrationResourceFilterRuleArgs']]] resource_filter_rules: List of rules for filtering Azure resources by their tags. The source of each filter rule must be in the form
-               filter('key', 'value'). You can join multiple filter statements using the and and or operators. Referenced keys are
-               limited to tags and must start with the azure_tag_ prefix..
+        :param pulumi.Input[Sequence[pulumi.Input['IntegrationResourceFilterRuleArgs']]] resource_filter_rules: List of rules for filtering Azure resources by their tags.
         :param pulumi.Input[bool] sync_guest_os_namespaces: If enabled, SignalFx will try to sync additional namespaces for VMs (including VMs in scale sets): telegraf/mem, telegraf/cpu, azure.vm.windows.guest (these are namespaces recommended by Azure when enabling their Diagnostic Extension). If there are no metrics there, no new datapoints will be ingested. Defaults to false.
         """
         pulumi.set(__self__, "app_id", app_id)
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "secret_key", secret_key)
         pulumi.set(__self__, "services", services)
         pulumi.set(__self__, "subscriptions", subscriptions)
@@ -112,15 +110,15 @@
     def secret_key(self, value: pulumi.Input[str]):
         pulumi.set(self, "secret_key", value)
 
     @property
     @pulumi.getter
     def services(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        List of Microsoft Azure service names for the Azure services you want SignalFx to monitor. See the documentation for [Creating Integrations](https://developers.signalfx.com/integrations_reference.html#operation/Create%20Integration) for valida values.
+        List of Microsoft Azure service names for the Azure services you want SignalFx to monitor. Can be an empty list to import data for all supported services. See [Microsoft Azure services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#azure-integrations) for a list of valid values.
         """
         return pulumi.get(self, "services")
 
     @services.setter
     def services(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "services", value)
 
@@ -232,17 +230,15 @@
     def poll_rate(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "poll_rate", value)
 
     @property
     @pulumi.getter(name="resourceFilterRules")
     def resource_filter_rules(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationResourceFilterRuleArgs']]]]:
         """
-        List of rules for filtering Azure resources by their tags. The source of each filter rule must be in the form
-        filter('key', 'value'). You can join multiple filter statements using the and and or operators. Referenced keys are
-        limited to tags and must start with the azure_tag_ prefix..
+        List of rules for filtering Azure resources by their tags.
         """
         return pulumi.get(self, "resource_filter_rules")
 
     @resource_filter_rules.setter
     def resource_filter_rules(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationResourceFilterRuleArgs']]]]):
         pulumi.set(self, "resource_filter_rules", value)
 
@@ -284,19 +280,17 @@
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationCustomNamespacesPerServiceArgs']]] custom_namespaces_per_services: Allows for more fine-grained control of syncing of custom namespaces, should the boolean convenience parameter `sync_guest_os_namespaces` be not enough. The customer may specify a map of services to custom namespaces. If they do so, for each service which is a key in this map, we will attempt to sync metrics from namespaces in the value list in addition to the default namespaces.
         :param pulumi.Input[bool] enabled: Whether the integration is enabled.
         :param pulumi.Input[str] environment: What type of Azure integration this is. The allowed values are `\\"azure_us_government\\"` and `\\"azure\\"`. Defaults to `\\"azure\\"`.
         :param pulumi.Input[bool] import_azure_monitor: If enabled, SignalFx will sync also Azure Monitor data. If disabled, SignalFx will import only metadata. Defaults to true.
         :param pulumi.Input[str] name: Name of the integration.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
         :param pulumi.Input[int] poll_rate: Azure poll rate (in seconds). Value between `60` and `600`. Default: `300`.
-        :param pulumi.Input[Sequence[pulumi.Input['IntegrationResourceFilterRuleArgs']]] resource_filter_rules: List of rules for filtering Azure resources by their tags. The source of each filter rule must be in the form
-               filter('key', 'value'). You can join multiple filter statements using the and and or operators. Referenced keys are
-               limited to tags and must start with the azure_tag_ prefix..
+        :param pulumi.Input[Sequence[pulumi.Input['IntegrationResourceFilterRuleArgs']]] resource_filter_rules: List of rules for filtering Azure resources by their tags.
         :param pulumi.Input[str] secret_key: Azure secret key that associates the SignalFx app in Azure with the Azure tenant ID. To learn how to get this ID, see the topic [Connect to Microsoft Azure](https://docs.signalfx.com/en/latest/integrations/azure-info.html#connect-to-azure) in the product documentation.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of Microsoft Azure service names for the Azure services you want SignalFx to monitor. See the documentation for [Creating Integrations](https://developers.signalfx.com/integrations_reference.html#operation/Create%20Integration) for valida values.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of Microsoft Azure service names for the Azure services you want SignalFx to monitor. Can be an empty list to import data for all supported services. See [Microsoft Azure services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#azure-integrations) for a list of valid values.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] subscriptions: List of Azure subscriptions that SignalFx should monitor.
         :param pulumi.Input[bool] sync_guest_os_namespaces: If enabled, SignalFx will try to sync additional namespaces for VMs (including VMs in scale sets): telegraf/mem, telegraf/cpu, azure.vm.windows.guest (these are namespaces recommended by Azure when enabling their Diagnostic Extension). If there are no metrics there, no new datapoints will be ingested. Defaults to false.
         :param pulumi.Input[str] tenant_id: Azure ID of the Azure tenant. To learn how to get this ID, see the topic [Connect to Microsoft Azure](https://docs.signalfx.com/en/latest/integrations/azure-info.html#connect-to-azure) in the product documentation.
         """
         if additional_services is not None:
             pulumi.set(__self__, "additional_services", additional_services)
         if app_id is not None:
@@ -436,17 +430,15 @@
     def poll_rate(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "poll_rate", value)
 
     @property
     @pulumi.getter(name="resourceFilterRules")
     def resource_filter_rules(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationResourceFilterRuleArgs']]]]:
         """
-        List of rules for filtering Azure resources by their tags. The source of each filter rule must be in the form
-        filter('key', 'value'). You can join multiple filter statements using the and and or operators. Referenced keys are
-        limited to tags and must start with the azure_tag_ prefix..
+        List of rules for filtering Azure resources by their tags.
         """
         return pulumi.get(self, "resource_filter_rules")
 
     @resource_filter_rules.setter
     def resource_filter_rules(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationResourceFilterRuleArgs']]]]):
         pulumi.set(self, "resource_filter_rules", value)
 
@@ -462,15 +454,15 @@
     def secret_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_key", value)
 
     @property
     @pulumi.getter
     def services(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of Microsoft Azure service names for the Azure services you want SignalFx to monitor. See the documentation for [Creating Integrations](https://developers.signalfx.com/integrations_reference.html#operation/Create%20Integration) for valida values.
+        List of Microsoft Azure service names for the Azure services you want SignalFx to monitor. Can be an empty list to import data for all supported services. See [Microsoft Azure services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#azure-integrations) for a list of valid values.
         """
         return pulumi.get(self, "services")
 
     @services.setter
     def services(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "services", value)
 
@@ -531,15 +523,15 @@
                  subscriptions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  sync_guest_os_namespaces: Optional[pulumi.Input[bool]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         SignalFx Azure integrations. For help with this integration see [Monitoring Microsoft Azure](https://docs.signalfx.com/en/latest/integrations/azure-info.html#connect-to-azure).
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
@@ -557,63 +549,54 @@
                 service="Microsoft.Compute/virtualMachines",
             )],
             enabled=True,
             environment="azure",
             poll_rate=300,
             resource_filter_rules=[
                 signalfx.azure.IntegrationResourceFilterRuleArgs(
-                    filter=signalfx.azure.IntegrationResourceFilterRuleFilterArgs(
-                        source="filter('azure_tag_service', 'payment') and (filter('azure_tag_env', 'prod-us') or filter('azure_tag_env', 'prod-eu'))",
-                    ),
+                    filter_source="filter('azure_tag_service', 'payment') and (filter('azure_tag_env', 'prod-us') or filter('azure_tag_env', 'prod-eu'))",
                 ),
                 signalfx.azure.IntegrationResourceFilterRuleArgs(
-                    filter=signalfx.azure.IntegrationResourceFilterRuleFilterArgs(
-                        source="filter('azure_tag_service', 'notification') and (filter('azure_tag_env', 'prod-us') or filter('azure_tag_env', 'prod-eu'))",
-                    ),
+                    filter_source="filter('azure_tag_service', 'notification') and (filter('azure_tag_env', 'prod-us') or filter('azure_tag_env', 'prod-eu'))",
                 ),
             ],
             secret_key="XXX",
             services=["microsoft.sql/servers/elasticpools"],
             subscriptions=["sub-guid-here"],
             tenant_id="ZZZ")
         ```
-        ## Service Names
-
-        > **NOTE** You can use the data source _azure_get_services_ to specify all services.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] additional_services: Additional Azure resource types that you want to sync with Observability Cloud.
         :param pulumi.Input[str] app_id: Azure application ID for the SignalFx app. To learn how to get this ID, see the topic [Connect to Microsoft Azure](https://docs.signalfx.com/en/latest/getting-started/send-data.html#connect-to-microsoft-azure) in the product documentation.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationCustomNamespacesPerServiceArgs']]]] custom_namespaces_per_services: Allows for more fine-grained control of syncing of custom namespaces, should the boolean convenience parameter `sync_guest_os_namespaces` be not enough. The customer may specify a map of services to custom namespaces. If they do so, for each service which is a key in this map, we will attempt to sync metrics from namespaces in the value list in addition to the default namespaces.
         :param pulumi.Input[bool] enabled: Whether the integration is enabled.
         :param pulumi.Input[str] environment: What type of Azure integration this is. The allowed values are `\\"azure_us_government\\"` and `\\"azure\\"`. Defaults to `\\"azure\\"`.
         :param pulumi.Input[bool] import_azure_monitor: If enabled, SignalFx will sync also Azure Monitor data. If disabled, SignalFx will import only metadata. Defaults to true.
         :param pulumi.Input[str] name: Name of the integration.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
         :param pulumi.Input[int] poll_rate: Azure poll rate (in seconds). Value between `60` and `600`. Default: `300`.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationResourceFilterRuleArgs']]]] resource_filter_rules: List of rules for filtering Azure resources by their tags. The source of each filter rule must be in the form
-               filter('key', 'value'). You can join multiple filter statements using the and and or operators. Referenced keys are
-               limited to tags and must start with the azure_tag_ prefix..
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationResourceFilterRuleArgs']]]] resource_filter_rules: List of rules for filtering Azure resources by their tags.
         :param pulumi.Input[str] secret_key: Azure secret key that associates the SignalFx app in Azure with the Azure tenant ID. To learn how to get this ID, see the topic [Connect to Microsoft Azure](https://docs.signalfx.com/en/latest/integrations/azure-info.html#connect-to-azure) in the product documentation.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of Microsoft Azure service names for the Azure services you want SignalFx to monitor. See the documentation for [Creating Integrations](https://developers.signalfx.com/integrations_reference.html#operation/Create%20Integration) for valida values.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of Microsoft Azure service names for the Azure services you want SignalFx to monitor. Can be an empty list to import data for all supported services. See [Microsoft Azure services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#azure-integrations) for a list of valid values.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] subscriptions: List of Azure subscriptions that SignalFx should monitor.
         :param pulumi.Input[bool] sync_guest_os_namespaces: If enabled, SignalFx will try to sync additional namespaces for VMs (including VMs in scale sets): telegraf/mem, telegraf/cpu, azure.vm.windows.guest (these are namespaces recommended by Azure when enabling their Diagnostic Extension). If there are no metrics there, no new datapoints will be ingested. Defaults to false.
         :param pulumi.Input[str] tenant_id: Azure ID of the Azure tenant. To learn how to get this ID, see the topic [Connect to Microsoft Azure](https://docs.signalfx.com/en/latest/integrations/azure-info.html#connect-to-azure) in the product documentation.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IntegrationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         SignalFx Azure integrations. For help with this integration see [Monitoring Microsoft Azure](https://docs.signalfx.com/en/latest/integrations/azure-info.html#connect-to-azure).
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
@@ -631,32 +614,25 @@
                 service="Microsoft.Compute/virtualMachines",
             )],
             enabled=True,
             environment="azure",
             poll_rate=300,
             resource_filter_rules=[
                 signalfx.azure.IntegrationResourceFilterRuleArgs(
-                    filter=signalfx.azure.IntegrationResourceFilterRuleFilterArgs(
-                        source="filter('azure_tag_service', 'payment') and (filter('azure_tag_env', 'prod-us') or filter('azure_tag_env', 'prod-eu'))",
-                    ),
+                    filter_source="filter('azure_tag_service', 'payment') and (filter('azure_tag_env', 'prod-us') or filter('azure_tag_env', 'prod-eu'))",
                 ),
                 signalfx.azure.IntegrationResourceFilterRuleArgs(
-                    filter=signalfx.azure.IntegrationResourceFilterRuleFilterArgs(
-                        source="filter('azure_tag_service', 'notification') and (filter('azure_tag_env', 'prod-us') or filter('azure_tag_env', 'prod-eu'))",
-                    ),
+                    filter_source="filter('azure_tag_service', 'notification') and (filter('azure_tag_env', 'prod-us') or filter('azure_tag_env', 'prod-eu'))",
                 ),
             ],
             secret_key="XXX",
             services=["microsoft.sql/servers/elasticpools"],
             subscriptions=["sub-guid-here"],
             tenant_id="ZZZ")
         ```
-        ## Service Names
-
-        > **NOTE** You can use the data source _azure_get_services_ to specify all services.
 
         :param str resource_name: The name of the resource.
         :param IntegrationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -759,19 +735,17 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationCustomNamespacesPerServiceArgs']]]] custom_namespaces_per_services: Allows for more fine-grained control of syncing of custom namespaces, should the boolean convenience parameter `sync_guest_os_namespaces` be not enough. The customer may specify a map of services to custom namespaces. If they do so, for each service which is a key in this map, we will attempt to sync metrics from namespaces in the value list in addition to the default namespaces.
         :param pulumi.Input[bool] enabled: Whether the integration is enabled.
         :param pulumi.Input[str] environment: What type of Azure integration this is. The allowed values are `\\"azure_us_government\\"` and `\\"azure\\"`. Defaults to `\\"azure\\"`.
         :param pulumi.Input[bool] import_azure_monitor: If enabled, SignalFx will sync also Azure Monitor data. If disabled, SignalFx will import only metadata. Defaults to true.
         :param pulumi.Input[str] name: Name of the integration.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
         :param pulumi.Input[int] poll_rate: Azure poll rate (in seconds). Value between `60` and `600`. Default: `300`.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationResourceFilterRuleArgs']]]] resource_filter_rules: List of rules for filtering Azure resources by their tags. The source of each filter rule must be in the form
-               filter('key', 'value'). You can join multiple filter statements using the and and or operators. Referenced keys are
-               limited to tags and must start with the azure_tag_ prefix..
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationResourceFilterRuleArgs']]]] resource_filter_rules: List of rules for filtering Azure resources by their tags.
         :param pulumi.Input[str] secret_key: Azure secret key that associates the SignalFx app in Azure with the Azure tenant ID. To learn how to get this ID, see the topic [Connect to Microsoft Azure](https://docs.signalfx.com/en/latest/integrations/azure-info.html#connect-to-azure) in the product documentation.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of Microsoft Azure service names for the Azure services you want SignalFx to monitor. See the documentation for [Creating Integrations](https://developers.signalfx.com/integrations_reference.html#operation/Create%20Integration) for valida values.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: List of Microsoft Azure service names for the Azure services you want SignalFx to monitor. Can be an empty list to import data for all supported services. See [Microsoft Azure services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#azure-integrations) for a list of valid values.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] subscriptions: List of Azure subscriptions that SignalFx should monitor.
         :param pulumi.Input[bool] sync_guest_os_namespaces: If enabled, SignalFx will try to sync additional namespaces for VMs (including VMs in scale sets): telegraf/mem, telegraf/cpu, azure.vm.windows.guest (these are namespaces recommended by Azure when enabling their Diagnostic Extension). If there are no metrics there, no new datapoints will be ingested. Defaults to false.
         :param pulumi.Input[str] tenant_id: Azure ID of the Azure tenant. To learn how to get this ID, see the topic [Connect to Microsoft Azure](https://docs.signalfx.com/en/latest/integrations/azure-info.html#connect-to-azure) in the product documentation.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _IntegrationState.__new__(_IntegrationState)
@@ -865,17 +839,15 @@
         """
         return pulumi.get(self, "poll_rate")
 
     @property
     @pulumi.getter(name="resourceFilterRules")
     def resource_filter_rules(self) -> pulumi.Output[Optional[Sequence['outputs.IntegrationResourceFilterRule']]]:
         """
-        List of rules for filtering Azure resources by their tags. The source of each filter rule must be in the form
-        filter('key', 'value'). You can join multiple filter statements using the and and or operators. Referenced keys are
-        limited to tags and must start with the azure_tag_ prefix..
+        List of rules for filtering Azure resources by their tags.
         """
         return pulumi.get(self, "resource_filter_rules")
 
     @property
     @pulumi.getter(name="secretKey")
     def secret_key(self) -> pulumi.Output[str]:
         """
@@ -883,15 +855,15 @@
         """
         return pulumi.get(self, "secret_key")
 
     @property
     @pulumi.getter
     def services(self) -> pulumi.Output[Sequence[str]]:
         """
-        List of Microsoft Azure service names for the Azure services you want SignalFx to monitor. See the documentation for [Creating Integrations](https://developers.signalfx.com/integrations_reference.html#operation/Create%20Integration) for valida values.
+        List of Microsoft Azure service names for the Azure services you want SignalFx to monitor. Can be an empty list to import data for all supported services. See [Microsoft Azure services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#azure-integrations) for a list of valid values.
         """
         return pulumi.get(self, "services")
 
     @property
     @pulumi.getter
     def subscriptions(self) -> pulumi.Output[Sequence[str]]:
         """
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/config/vars.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/dashboard.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/dashboard.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,26 +117,32 @@
 
     @property
     @pulumi.getter(name="authorizedWriterTeams")
     def authorized_writer_teams(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Team IDs that have write access to this dashboard group. Remember to use an admin's token if using this feature and to include that admin's team (or user id in `authorized_writer_teams`). **Note:** Deprecated use `permissions` instead.
         """
+        warnings.warn("""Please use permissions_* fields now""", DeprecationWarning)
+        pulumi.log.warn("""authorized_writer_teams is deprecated: Please use permissions_* fields now""")
+
         return pulumi.get(self, "authorized_writer_teams")
 
     @authorized_writer_teams.setter
     def authorized_writer_teams(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "authorized_writer_teams", value)
 
     @property
     @pulumi.getter(name="authorizedWriterUsers")
     def authorized_writer_users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         User IDs that have write access to this dashboard group. Remember to use an admin's token if using this feature and to include that admin's user id (or team id in `authorized_writer_teams`). **Note:** Deprecated use `permissions` instead.
         """
+        warnings.warn("""Please use permissions fields now""", DeprecationWarning)
+        pulumi.log.warn("""authorized_writer_users is deprecated: Please use permissions fields now""")
+
         return pulumi.get(self, "authorized_writer_users")
 
     @authorized_writer_users.setter
     def authorized_writer_users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "authorized_writer_users", value)
 
     @property
@@ -435,26 +441,32 @@
 
     @property
     @pulumi.getter(name="authorizedWriterTeams")
     def authorized_writer_teams(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Team IDs that have write access to this dashboard group. Remember to use an admin's token if using this feature and to include that admin's team (or user id in `authorized_writer_teams`). **Note:** Deprecated use `permissions` instead.
         """
+        warnings.warn("""Please use permissions_* fields now""", DeprecationWarning)
+        pulumi.log.warn("""authorized_writer_teams is deprecated: Please use permissions_* fields now""")
+
         return pulumi.get(self, "authorized_writer_teams")
 
     @authorized_writer_teams.setter
     def authorized_writer_teams(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "authorized_writer_teams", value)
 
     @property
     @pulumi.getter(name="authorizedWriterUsers")
     def authorized_writer_users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         User IDs that have write access to this dashboard group. Remember to use an admin's token if using this feature and to include that admin's user id (or team id in `authorized_writer_teams`). **Note:** Deprecated use `permissions` instead.
         """
+        warnings.warn("""Please use permissions fields now""", DeprecationWarning)
+        pulumi.log.warn("""authorized_writer_users is deprecated: Please use permissions fields now""")
+
         return pulumi.get(self, "authorized_writer_users")
 
     @authorized_writer_users.setter
     def authorized_writer_users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "authorized_writer_users", value)
 
     @property
@@ -897,22 +909,28 @@
 
     @property
     @pulumi.getter(name="authorizedWriterTeams")
     def authorized_writer_teams(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         Team IDs that have write access to this dashboard group. Remember to use an admin's token if using this feature and to include that admin's team (or user id in `authorized_writer_teams`). **Note:** Deprecated use `permissions` instead.
         """
+        warnings.warn("""Please use permissions_* fields now""", DeprecationWarning)
+        pulumi.log.warn("""authorized_writer_teams is deprecated: Please use permissions_* fields now""")
+
         return pulumi.get(self, "authorized_writer_teams")
 
     @property
     @pulumi.getter(name="authorizedWriterUsers")
     def authorized_writer_users(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         User IDs that have write access to this dashboard group. Remember to use an admin's token if using this feature and to include that admin's user id (or team id in `authorized_writer_teams`). **Note:** Deprecated use `permissions` instead.
         """
+        warnings.warn("""Please use permissions fields now""", DeprecationWarning)
+        pulumi.log.warn("""authorized_writer_users is deprecated: Please use permissions fields now""")
+
         return pulumi.get(self, "authorized_writer_users")
 
     @property
     @pulumi.getter
     def charts(self) -> pulumi.Output[Optional[Sequence['outputs.DashboardChart']]]:
         """
         Chart ID and layout information for the charts in the dashboard.
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/dashboard_group.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/dashboard_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,26 +59,32 @@
 
     @property
     @pulumi.getter(name="authorizedWriterTeams")
     def authorized_writer_teams(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Team IDs that have write access to this dashboard group. Remember to use an admin's token if using this feature and to include that admin's team (or user id in `authorized_writer_teams`). **Note:** Deprecated use `permissions` instead.
         """
+        warnings.warn("""Please use permissions field now""", DeprecationWarning)
+        pulumi.log.warn("""authorized_writer_teams is deprecated: Please use permissions field now""")
+
         return pulumi.get(self, "authorized_writer_teams")
 
     @authorized_writer_teams.setter
     def authorized_writer_teams(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "authorized_writer_teams", value)
 
     @property
     @pulumi.getter(name="authorizedWriterUsers")
     def authorized_writer_users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         User IDs that have write access to this dashboard group. Remember to use an admin's token if using this feature and to include that admin's user id (or team id in `authorized_writer_teams`). **Note:** Deprecated use `permissions` instead.
         """
+        warnings.warn("""Please use permissions field now""", DeprecationWarning)
+        pulumi.log.warn("""authorized_writer_users is deprecated: Please use permissions field now""")
+
         return pulumi.get(self, "authorized_writer_users")
 
     @authorized_writer_users.setter
     def authorized_writer_users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "authorized_writer_users", value)
 
     @property
@@ -197,26 +203,32 @@
 
     @property
     @pulumi.getter(name="authorizedWriterTeams")
     def authorized_writer_teams(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Team IDs that have write access to this dashboard group. Remember to use an admin's token if using this feature and to include that admin's team (or user id in `authorized_writer_teams`). **Note:** Deprecated use `permissions` instead.
         """
+        warnings.warn("""Please use permissions field now""", DeprecationWarning)
+        pulumi.log.warn("""authorized_writer_teams is deprecated: Please use permissions field now""")
+
         return pulumi.get(self, "authorized_writer_teams")
 
     @authorized_writer_teams.setter
     def authorized_writer_teams(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "authorized_writer_teams", value)
 
     @property
     @pulumi.getter(name="authorizedWriterUsers")
     def authorized_writer_users(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         User IDs that have write access to this dashboard group. Remember to use an admin's token if using this feature and to include that admin's user id (or team id in `authorized_writer_teams`). **Note:** Deprecated use `permissions` instead.
         """
+        warnings.warn("""Please use permissions field now""", DeprecationWarning)
+        pulumi.log.warn("""authorized_writer_users is deprecated: Please use permissions field now""")
+
         return pulumi.get(self, "authorized_writer_users")
 
     @authorized_writer_users.setter
     def authorized_writer_users(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "authorized_writer_users", value)
 
     @property
@@ -304,14 +316,16 @@
                  teams: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         In the SignalFx web UI, a [dashboard group](https://developers.signalfx.com/dashboard_groups_reference.html) is a collection of dashboards.
 
         > **NOTE** Dashboard groups cannot be accessed directly, but just via a dashboard contained in them. This is the reason why make show won't show any of yours dashboard groups.
 
+        > **NOTE** When you want to "Change or remove write permissions for a user other than yourself" regarding dashboard groups, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
         mydashboardgroup0 = signalfx.DashboardGroup("mydashboardgroup0",
@@ -388,14 +402,16 @@
                  args: Optional[DashboardGroupArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         In the SignalFx web UI, a [dashboard group](https://developers.signalfx.com/dashboard_groups_reference.html) is a collection of dashboards.
 
         > **NOTE** Dashboard groups cannot be accessed directly, but just via a dashboard contained in them. This is the reason why make show won't show any of yours dashboard groups.
 
+        > **NOTE** When you want to "Change or remove write permissions for a user other than yourself" regarding dashboard groups, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
         mydashboardgroup0 = signalfx.DashboardGroup("mydashboardgroup0",
@@ -550,22 +566,28 @@
 
     @property
     @pulumi.getter(name="authorizedWriterTeams")
     def authorized_writer_teams(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         Team IDs that have write access to this dashboard group. Remember to use an admin's token if using this feature and to include that admin's team (or user id in `authorized_writer_teams`). **Note:** Deprecated use `permissions` instead.
         """
+        warnings.warn("""Please use permissions field now""", DeprecationWarning)
+        pulumi.log.warn("""authorized_writer_teams is deprecated: Please use permissions field now""")
+
         return pulumi.get(self, "authorized_writer_teams")
 
     @property
     @pulumi.getter(name="authorizedWriterUsers")
     def authorized_writer_users(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         User IDs that have write access to this dashboard group. Remember to use an admin's token if using this feature and to include that admin's user id (or team id in `authorized_writer_teams`). **Note:** Deprecated use `permissions` instead.
         """
+        warnings.warn("""Please use permissions field now""", DeprecationWarning)
+        pulumi.log.warn("""authorized_writer_users is deprecated: Please use permissions field now""")
+
         return pulumi.get(self, "authorized_writer_users")
 
     @property
     @pulumi.getter
     def dashboards(self) -> pulumi.Output[Optional[Sequence['outputs.DashboardGroupDashboard']]]:
         """
         [Mirrored dashboards](https://docs.signalfx.com/en/latest/dashboards/dashboard-mirrors.html) in this dashboard group. **Note:** This feature is not present in all accounts. Please contact support if you are unsure.
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/data_link.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/data_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/detector.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -660,14 +660,16 @@
                  viz_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DetectorVizOptionArgs']]]]] = None,
                  __props__=None):
         """
         Provides a SignalFx detector resource. This can be used to create and manage detectors.
 
         > **NOTE** If you're interested in using SignalFx detector features such as Historical Anomaly, Resource Running Out, or others then consider building them in the UI first then using the "Show SignalFlow" feature to extract the value for `program_text`. You may also consult the [documentation for detector functions in signalflow-library](https://github.com/signalfx/signalflow-library/tree/master/library/signalfx/detectors).
 
+        > **NOTE** When you want to "Change or remove write permissions for a user other than yourself" regarding detectors, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
         config = pulumi.Config()
@@ -825,14 +827,16 @@
                  args: DetectorArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a SignalFx detector resource. This can be used to create and manage detectors.
 
         > **NOTE** If you're interested in using SignalFx detector features such as Historical Anomaly, Resource Running Out, or others then consider building them in the UI first then using the "Show SignalFlow" feature to extract the value for `program_text`. You may also consult the [documentation for detector functions in signalflow-library](https://github.com/signalfx/signalflow-library/tree/master/library/signalfx/detectors).
 
+        > **NOTE** When you want to "Change or remove write permissions for a user other than yourself" regarding detectors, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
         config = pulumi.Config()
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/event_feed_chart.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/event_feed_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/_inputs.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/_inputs.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
     'IntegrationProjectServiceKeyArgs',
-    'GetServicesServiceArgs',
 ]
 
 @pulumi.input_type
 class IntegrationProjectServiceKeyArgs:
     def __init__(__self__, *,
                  project_id: pulumi.Input[str],
                  project_key: pulumi.Input[str]):
@@ -37,23 +36,7 @@
         return pulumi.get(self, "project_key")
 
     @project_key.setter
     def project_key(self, value: pulumi.Input[str]):
         pulumi.set(self, "project_key", value)
 
 
-@pulumi.input_type
-class GetServicesServiceArgs:
-    def __init__(__self__, *,
-                 name: str):
-        pulumi.set(__self__, "name", name)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: str):
-        pulumi.set(self, "name", value)
-
-
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/integration.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         :param pulumi.Input[bool] import_gcp_metrics: If enabled, SignalFx will sync also Google Cloud Metrics data. If disabled, SignalFx will import only metadata. Defaults
                to true.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] include_lists: [Compute Metadata Include List](https://dev.splunk.com/observability/docs/integrations/gcp_integration_overview/).
         :param pulumi.Input[str] name: Name of the integration.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
         :param pulumi.Input[int] poll_rate: GCP integration poll rate (in seconds). Value between `60` and `600`. Default: `300`.
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationProjectServiceKeyArgs']]] project_service_keys: GCP projects to add.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See the documentation for [Creating Integrations](https://dev.splunk.com/observability/reference/api/integrations/latest#endpoint-create-integration) for valid values.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See [Google Cloud Platform services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#google-cloud-platform-services) for a list of valid values.
         :param pulumi.Input[bool] use_metric_source_project_for_quota: When this value is set to true Observability Cloud will force usage of a quota from the project where metrics are stored. For this to work the service account provided for the project needs to be provided with serviceusage.services.use permission or Service Usage Consumer role in this project. When set to false default quota settings are used.
         """
         pulumi.set(__self__, "enabled", enabled)
         if custom_metric_type_domains is not None:
             pulumi.set(__self__, "custom_metric_type_domains", custom_metric_type_domains)
         if import_gcp_metrics is not None:
             pulumi.set(__self__, "import_gcp_metrics", import_gcp_metrics)
@@ -157,15 +157,15 @@
     def project_service_keys(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationProjectServiceKeyArgs']]]]):
         pulumi.set(self, "project_service_keys", value)
 
     @property
     @pulumi.getter
     def services(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See the documentation for [Creating Integrations](https://dev.splunk.com/observability/reference/api/integrations/latest#endpoint-create-integration) for valid values.
+        GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See [Google Cloud Platform services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#google-cloud-platform-services) for a list of valid values.
         """
         return pulumi.get(self, "services")
 
     @services.setter
     def services(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "services", value)
 
@@ -202,15 +202,15 @@
         :param pulumi.Input[bool] import_gcp_metrics: If enabled, SignalFx will sync also Google Cloud Metrics data. If disabled, SignalFx will import only metadata. Defaults
                to true.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] include_lists: [Compute Metadata Include List](https://dev.splunk.com/observability/docs/integrations/gcp_integration_overview/).
         :param pulumi.Input[str] name: Name of the integration.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
         :param pulumi.Input[int] poll_rate: GCP integration poll rate (in seconds). Value between `60` and `600`. Default: `300`.
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationProjectServiceKeyArgs']]] project_service_keys: GCP projects to add.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See the documentation for [Creating Integrations](https://dev.splunk.com/observability/reference/api/integrations/latest#endpoint-create-integration) for valid values.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See [Google Cloud Platform services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#google-cloud-platform-services) for a list of valid values.
         :param pulumi.Input[bool] use_metric_source_project_for_quota: When this value is set to true Observability Cloud will force usage of a quota from the project where metrics are stored. For this to work the service account provided for the project needs to be provided with serviceusage.services.use permission or Service Usage Consumer role in this project. When set to false default quota settings are used.
         """
         if custom_metric_type_domains is not None:
             pulumi.set(__self__, "custom_metric_type_domains", custom_metric_type_domains)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if import_gcp_metrics is not None:
@@ -327,15 +327,15 @@
     def project_service_keys(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationProjectServiceKeyArgs']]]]):
         pulumi.set(self, "project_service_keys", value)
 
     @property
     @pulumi.getter
     def services(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See the documentation for [Creating Integrations](https://dev.splunk.com/observability/reference/api/integrations/latest#endpoint-create-integration) for valid values.
+        GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See [Google Cloud Platform services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#google-cloud-platform-services) for a list of valid values.
         """
         return pulumi.get(self, "services")
 
     @services.setter
     def services(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "services", value)
 
@@ -367,15 +367,15 @@
                  project_service_keys: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationProjectServiceKeyArgs']]]]] = None,
                  services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  use_metric_source_project_for_quota: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         SignalFx GCP Integration
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
@@ -402,27 +402,27 @@
         :param pulumi.Input[bool] import_gcp_metrics: If enabled, SignalFx will sync also Google Cloud Metrics data. If disabled, SignalFx will import only metadata. Defaults
                to true.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] include_lists: [Compute Metadata Include List](https://dev.splunk.com/observability/docs/integrations/gcp_integration_overview/).
         :param pulumi.Input[str] name: Name of the integration.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
         :param pulumi.Input[int] poll_rate: GCP integration poll rate (in seconds). Value between `60` and `600`. Default: `300`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationProjectServiceKeyArgs']]]] project_service_keys: GCP projects to add.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See the documentation for [Creating Integrations](https://dev.splunk.com/observability/reference/api/integrations/latest#endpoint-create-integration) for valid values.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See [Google Cloud Platform services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#google-cloud-platform-services) for a list of valid values.
         :param pulumi.Input[bool] use_metric_source_project_for_quota: When this value is set to true Observability Cloud will force usage of a quota from the project where metrics are stored. For this to work the service account provided for the project needs to be provided with serviceusage.services.use permission or Service Usage Consumer role in this project. When set to false default quota settings are used.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IntegrationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         SignalFx GCP Integration
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
@@ -522,15 +522,15 @@
         :param pulumi.Input[bool] import_gcp_metrics: If enabled, SignalFx will sync also Google Cloud Metrics data. If disabled, SignalFx will import only metadata. Defaults
                to true.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] include_lists: [Compute Metadata Include List](https://dev.splunk.com/observability/docs/integrations/gcp_integration_overview/).
         :param pulumi.Input[str] name: Name of the integration.
         :param pulumi.Input[str] named_token: Name of the org token to be used for data ingestion. If not specified then default access token is used.
         :param pulumi.Input[int] poll_rate: GCP integration poll rate (in seconds). Value between `60` and `600`. Default: `300`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['IntegrationProjectServiceKeyArgs']]]] project_service_keys: GCP projects to add.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See the documentation for [Creating Integrations](https://dev.splunk.com/observability/reference/api/integrations/latest#endpoint-create-integration) for valid values.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] services: GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See [Google Cloud Platform services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#google-cloud-platform-services) for a list of valid values.
         :param pulumi.Input[bool] use_metric_source_project_for_quota: When this value is set to true Observability Cloud will force usage of a quota from the project where metrics are stored. For this to work the service account provided for the project needs to be provided with serviceusage.services.use permission or Service Usage Consumer role in this project. When set to false default quota settings are used.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _IntegrationState.__new__(_IntegrationState)
 
         __props__.__dict__["custom_metric_type_domains"] = custom_metric_type_domains
@@ -610,15 +610,15 @@
         """
         return pulumi.get(self, "project_service_keys")
 
     @property
     @pulumi.getter
     def services(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See the documentation for [Creating Integrations](https://dev.splunk.com/observability/reference/api/integrations/latest#endpoint-create-integration) for valid values.
+        GCP service metrics to import. Can be an empty list, or not included, to import 'All services'. See [Google Cloud Platform services](https://docs.splunk.com/Observability/gdi/get-data-in/integrations.html#google-cloud-platform-services) for a list of valid values.
         """
         return pulumi.get(self, "services")
 
     @property
     @pulumi.getter(name="useMetricSourceProjectForQuota")
     def use_metric_source_project_for_quota(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/gcp/outputs.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/gcp/outputs.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 
 __all__ = [
     'IntegrationProjectServiceKey',
-    'GetServicesServiceResult',
 ]
 
 @pulumi.output_type
 class IntegrationProjectServiceKey(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
@@ -48,19 +47,7 @@
 
     @property
     @pulumi.getter(name="projectKey")
     def project_key(self) -> str:
         return pulumi.get(self, "project_key")
 
 
-@pulumi.output_type
-class GetServicesServiceResult(dict):
-    def __init__(__self__, *,
-                 name: str):
-        pulumi.set(__self__, "name", name)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
-
-
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/get_dimension_values.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/get_dimension_values.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     """
     __args__ = dict()
     __args__['query'] = query
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('signalfx:index/getDimensionValues:getDimensionValues', __args__, opts=opts, typ=GetDimensionValuesResult).value
 
     return AwaitableGetDimensionValuesResult(
-        id=__ret__.id,
-        query=__ret__.query,
-        values=__ret__.values)
+        id=pulumi.get(__ret__, 'id'),
+        query=pulumi.get(__ret__, 'query'),
+        values=pulumi.get(__ret__, 'values'))
 
 
 @_utilities.lift_output_func(get_dimension_values)
 def get_dimension_values_output(query: Optional[pulumi.Input[str]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDimensionValuesResult]:
     """
     Use this data source to get a list of dimension values matching the provided query.
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/heatmap_chart.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/heatmap_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/jira/integration.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/jira/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,15 @@
                  project_key: Optional[pulumi.Input[str]] = None,
                  user_email: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         SignalFx Jira integrations. For help with this integration see [Integration with Jira](https://docs.signalfx.com/en/latest/admin-guide/integrate-notifications.html#integrate-with-jira).
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
@@ -466,15 +466,15 @@
     def __init__(__self__,
                  resource_name: str,
                  args: IntegrationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         SignalFx Jira integrations. For help with this integration see [Integration with Jira](https://docs.signalfx.com/en/latest/admin-guide/integrate-notifications.html#integrate-with-jira).
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/list_chart.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/list_chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,17 @@
 
     @property
     @pulumi.getter(name="legendFieldsToHides")
     def legend_fields_to_hides(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         List of properties that should not be displayed in the chart legend (i.e. dimension names). All the properties are visible by default. Deprecated, please use `legend_options_fields`.
         """
+        warnings.warn("""Please use legend_options_fields""", DeprecationWarning)
+        pulumi.log.warn("""legend_fields_to_hides is deprecated: Please use legend_options_fields""")
+
         return pulumi.get(self, "legend_fields_to_hides")
 
     @legend_fields_to_hides.setter
     def legend_fields_to_hides(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "legend_fields_to_hides", value)
 
     @property
@@ -511,14 +514,17 @@
 
     @property
     @pulumi.getter(name="legendFieldsToHides")
     def legend_fields_to_hides(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         List of properties that should not be displayed in the chart legend (i.e. dimension names). All the properties are visible by default. Deprecated, please use `legend_options_fields`.
         """
+        warnings.warn("""Please use legend_options_fields""", DeprecationWarning)
+        pulumi.log.warn("""legend_fields_to_hides is deprecated: Please use legend_options_fields""")
+
         return pulumi.get(self, "legend_fields_to_hides")
 
     @legend_fields_to_hides.setter
     def legend_fields_to_hides(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "legend_fields_to_hides", value)
 
     @property
@@ -1050,14 +1056,17 @@
 
     @property
     @pulumi.getter(name="legendFieldsToHides")
     def legend_fields_to_hides(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         List of properties that should not be displayed in the chart legend (i.e. dimension names). All the properties are visible by default. Deprecated, please use `legend_options_fields`.
         """
+        warnings.warn("""Please use legend_options_fields""", DeprecationWarning)
+        pulumi.log.warn("""legend_fields_to_hides is deprecated: Please use legend_options_fields""")
+
         return pulumi.get(self, "legend_fields_to_hides")
 
     @property
     @pulumi.getter(name="legendOptionsFields")
     def legend_options_fields(self) -> pulumi.Output[Optional[Sequence['outputs.ListChartLegendOptionsField']]]:
         """
         List of property names and enabled flags that should be displayed in the data table for the chart, in the order provided. This option cannot be used with `legend_fields_to_hide`.
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/_inputs.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/logs/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/outputs.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/logs/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/logs/view.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/logs/view.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/metric_ruleset.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/metric_ruleset.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
 __all__ = ['MetricRulesetArgs', 'MetricRuleset']
 
 @pulumi.input_type
 class MetricRulesetArgs:
     def __init__(__self__, *,
                  metric_name: pulumi.Input[str],
-                 routing_rule: pulumi.Input['MetricRulesetRoutingRuleArgs'],
+                 routing_rules: pulumi.Input[Sequence[pulumi.Input['MetricRulesetRoutingRuleArgs']]],
                  aggregation_rules: Optional[pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleArgs']]]] = None):
         """
         The set of arguments for constructing a MetricRuleset resource.
         :param pulumi.Input[str] metric_name: Name of the input metric
-        :param pulumi.Input['MetricRulesetRoutingRuleArgs'] routing_rule: Routing Rule object
+        :param pulumi.Input[Sequence[pulumi.Input['MetricRulesetRoutingRuleArgs']]] routing_rules: Routing Rule object
         :param pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleArgs']]] aggregation_rules: List of aggregation rules for the metric
         """
         pulumi.set(__self__, "metric_name", metric_name)
-        pulumi.set(__self__, "routing_rule", routing_rule)
+        pulumi.set(__self__, "routing_rules", routing_rules)
         if aggregation_rules is not None:
             pulumi.set(__self__, "aggregation_rules", aggregation_rules)
 
     @property
     @pulumi.getter(name="metricName")
     def metric_name(self) -> pulumi.Input[str]:
         """
@@ -39,24 +39,24 @@
         return pulumi.get(self, "metric_name")
 
     @metric_name.setter
     def metric_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "metric_name", value)
 
     @property
-    @pulumi.getter(name="routingRule")
-    def routing_rule(self) -> pulumi.Input['MetricRulesetRoutingRuleArgs']:
+    @pulumi.getter(name="routingRules")
+    def routing_rules(self) -> pulumi.Input[Sequence[pulumi.Input['MetricRulesetRoutingRuleArgs']]]:
         """
         Routing Rule object
         """
-        return pulumi.get(self, "routing_rule")
+        return pulumi.get(self, "routing_rules")
 
-    @routing_rule.setter
-    def routing_rule(self, value: pulumi.Input['MetricRulesetRoutingRuleArgs']):
-        pulumi.set(self, "routing_rule", value)
+    @routing_rules.setter
+    def routing_rules(self, value: pulumi.Input[Sequence[pulumi.Input['MetricRulesetRoutingRuleArgs']]]):
+        pulumi.set(self, "routing_rules", value)
 
     @property
     @pulumi.getter(name="aggregationRules")
     def aggregation_rules(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleArgs']]]]:
         """
         List of aggregation rules for the metric
         """
@@ -73,26 +73,26 @@
                  aggregation_rules: Optional[pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleArgs']]]] = None,
                  created: Optional[pulumi.Input[str]] = None,
                  creator: Optional[pulumi.Input[str]] = None,
                  last_updated: Optional[pulumi.Input[str]] = None,
                  last_updated_by: Optional[pulumi.Input[str]] = None,
                  last_updated_by_name: Optional[pulumi.Input[str]] = None,
                  metric_name: Optional[pulumi.Input[str]] = None,
-                 routing_rule: Optional[pulumi.Input['MetricRulesetRoutingRuleArgs']] = None,
+                 routing_rules: Optional[pulumi.Input[Sequence[pulumi.Input['MetricRulesetRoutingRuleArgs']]]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering MetricRuleset resources.
         :param pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleArgs']]] aggregation_rules: List of aggregation rules for the metric
         :param pulumi.Input[str] created: Timestamp of when the metric ruleset was created
         :param pulumi.Input[str] creator: ID of the creator of the metric ruleset
         :param pulumi.Input[str] last_updated: Timestamp of when the metric ruleset was last updated
         :param pulumi.Input[str] last_updated_by: ID of user who last updated the metric ruleset
         :param pulumi.Input[str] last_updated_by_name: Name of user who last updated this metric ruleset
         :param pulumi.Input[str] metric_name: Name of the input metric
-        :param pulumi.Input['MetricRulesetRoutingRuleArgs'] routing_rule: Routing Rule object
+        :param pulumi.Input[Sequence[pulumi.Input['MetricRulesetRoutingRuleArgs']]] routing_rules: Routing Rule object
         :param pulumi.Input[str] version: Version of the ruleset
         """
         if aggregation_rules is not None:
             pulumi.set(__self__, "aggregation_rules", aggregation_rules)
         if created is not None:
             pulumi.set(__self__, "created", created)
         if creator is not None:
@@ -101,16 +101,16 @@
             pulumi.set(__self__, "last_updated", last_updated)
         if last_updated_by is not None:
             pulumi.set(__self__, "last_updated_by", last_updated_by)
         if last_updated_by_name is not None:
             pulumi.set(__self__, "last_updated_by_name", last_updated_by_name)
         if metric_name is not None:
             pulumi.set(__self__, "metric_name", metric_name)
-        if routing_rule is not None:
-            pulumi.set(__self__, "routing_rule", routing_rule)
+        if routing_rules is not None:
+            pulumi.set(__self__, "routing_rules", routing_rules)
         if version is not None:
             pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter(name="aggregationRules")
     def aggregation_rules(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['MetricRulesetAggregationRuleArgs']]]]:
         """
@@ -191,24 +191,24 @@
         return pulumi.get(self, "metric_name")
 
     @metric_name.setter
     def metric_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "metric_name", value)
 
     @property
-    @pulumi.getter(name="routingRule")
-    def routing_rule(self) -> Optional[pulumi.Input['MetricRulesetRoutingRuleArgs']]:
+    @pulumi.getter(name="routingRules")
+    def routing_rules(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['MetricRulesetRoutingRuleArgs']]]]:
         """
         Routing Rule object
         """
-        return pulumi.get(self, "routing_rule")
+        return pulumi.get(self, "routing_rules")
 
-    @routing_rule.setter
-    def routing_rule(self, value: Optional[pulumi.Input['MetricRulesetRoutingRuleArgs']]):
-        pulumi.set(self, "routing_rule", value)
+    @routing_rules.setter
+    def routing_rules(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['MetricRulesetRoutingRuleArgs']]]]):
+        pulumi.set(self, "routing_rules", value)
 
     @property
     @pulumi.getter
     def version(self) -> Optional[pulumi.Input[str]]:
         """
         Version of the ruleset
         """
@@ -222,34 +222,38 @@
 class MetricRuleset(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  aggregation_rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MetricRulesetAggregationRuleArgs']]]]] = None,
                  metric_name: Optional[pulumi.Input[str]] = None,
-                 routing_rule: Optional[pulumi.Input[pulumi.InputType['MetricRulesetRoutingRuleArgs']]] = None,
+                 routing_rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MetricRulesetRoutingRuleArgs']]]]] = None,
                  __props__=None):
         """
         Provides an Observability Cloud resource for managing metric rulesets
 
+        > **NOTE** When managing metric rulesets to drop data use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MetricRulesetAggregationRuleArgs']]]] aggregation_rules: List of aggregation rules for the metric
         :param pulumi.Input[str] metric_name: Name of the input metric
-        :param pulumi.Input[pulumi.InputType['MetricRulesetRoutingRuleArgs']] routing_rule: Routing Rule object
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MetricRulesetRoutingRuleArgs']]]] routing_rules: Routing Rule object
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: MetricRulesetArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides an Observability Cloud resource for managing metric rulesets
 
+        > **NOTE** When managing metric rulesets to drop data use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+
         :param str resource_name: The name of the resource.
         :param MetricRulesetArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(MetricRulesetArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -259,31 +263,31 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  aggregation_rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MetricRulesetAggregationRuleArgs']]]]] = None,
                  metric_name: Optional[pulumi.Input[str]] = None,
-                 routing_rule: Optional[pulumi.Input[pulumi.InputType['MetricRulesetRoutingRuleArgs']]] = None,
+                 routing_rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MetricRulesetRoutingRuleArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = MetricRulesetArgs.__new__(MetricRulesetArgs)
 
             __props__.__dict__["aggregation_rules"] = aggregation_rules
             if metric_name is None and not opts.urn:
                 raise TypeError("Missing required property 'metric_name'")
             __props__.__dict__["metric_name"] = metric_name
-            if routing_rule is None and not opts.urn:
-                raise TypeError("Missing required property 'routing_rule'")
-            __props__.__dict__["routing_rule"] = routing_rule
+            if routing_rules is None and not opts.urn:
+                raise TypeError("Missing required property 'routing_rules'")
+            __props__.__dict__["routing_rules"] = routing_rules
             __props__.__dict__["created"] = None
             __props__.__dict__["creator"] = None
             __props__.__dict__["last_updated"] = None
             __props__.__dict__["last_updated_by"] = None
             __props__.__dict__["last_updated_by_name"] = None
             __props__.__dict__["version"] = None
         super(MetricRuleset, __self__).__init__(
@@ -299,15 +303,15 @@
             aggregation_rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MetricRulesetAggregationRuleArgs']]]]] = None,
             created: Optional[pulumi.Input[str]] = None,
             creator: Optional[pulumi.Input[str]] = None,
             last_updated: Optional[pulumi.Input[str]] = None,
             last_updated_by: Optional[pulumi.Input[str]] = None,
             last_updated_by_name: Optional[pulumi.Input[str]] = None,
             metric_name: Optional[pulumi.Input[str]] = None,
-            routing_rule: Optional[pulumi.Input[pulumi.InputType['MetricRulesetRoutingRuleArgs']]] = None,
+            routing_rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MetricRulesetRoutingRuleArgs']]]]] = None,
             version: Optional[pulumi.Input[str]] = None) -> 'MetricRuleset':
         """
         Get an existing MetricRuleset resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
@@ -315,29 +319,29 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MetricRulesetAggregationRuleArgs']]]] aggregation_rules: List of aggregation rules for the metric
         :param pulumi.Input[str] created: Timestamp of when the metric ruleset was created
         :param pulumi.Input[str] creator: ID of the creator of the metric ruleset
         :param pulumi.Input[str] last_updated: Timestamp of when the metric ruleset was last updated
         :param pulumi.Input[str] last_updated_by: ID of user who last updated the metric ruleset
         :param pulumi.Input[str] last_updated_by_name: Name of user who last updated this metric ruleset
         :param pulumi.Input[str] metric_name: Name of the input metric
-        :param pulumi.Input[pulumi.InputType['MetricRulesetRoutingRuleArgs']] routing_rule: Routing Rule object
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MetricRulesetRoutingRuleArgs']]]] routing_rules: Routing Rule object
         :param pulumi.Input[str] version: Version of the ruleset
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _MetricRulesetState.__new__(_MetricRulesetState)
 
         __props__.__dict__["aggregation_rules"] = aggregation_rules
         __props__.__dict__["created"] = created
         __props__.__dict__["creator"] = creator
         __props__.__dict__["last_updated"] = last_updated
         __props__.__dict__["last_updated_by"] = last_updated_by
         __props__.__dict__["last_updated_by_name"] = last_updated_by_name
         __props__.__dict__["metric_name"] = metric_name
-        __props__.__dict__["routing_rule"] = routing_rule
+        __props__.__dict__["routing_rules"] = routing_rules
         __props__.__dict__["version"] = version
         return MetricRuleset(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="aggregationRules")
     def aggregation_rules(self) -> pulumi.Output[Optional[Sequence['outputs.MetricRulesetAggregationRule']]]:
         """
@@ -390,20 +394,20 @@
     def metric_name(self) -> pulumi.Output[str]:
         """
         Name of the input metric
         """
         return pulumi.get(self, "metric_name")
 
     @property
-    @pulumi.getter(name="routingRule")
-    def routing_rule(self) -> pulumi.Output['outputs.MetricRulesetRoutingRule']:
+    @pulumi.getter(name="routingRules")
+    def routing_rules(self) -> pulumi.Output[Sequence['outputs.MetricRulesetRoutingRule']]:
         """
         Routing Rule object
         """
-        return pulumi.get(self, "routing_rule")
+        return pulumi.get(self, "routing_rules")
 
     @property
     @pulumi.getter
     def version(self) -> pulumi.Output[str]:
         """
         Version of the ruleset
         """
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/opsgenie/integration.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/opsgenie/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
                  api_url: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         SignalFx Opsgenie integration.
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
@@ -192,15 +192,15 @@
     def __init__(__self__,
                  resource_name: str,
                  args: IntegrationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         SignalFx Opsgenie integration.
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/org_token.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/org_token.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,16 +27,15 @@
         The set of arguments for constructing a OrgToken resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] auth_scopes: Authentication scope, ex: INGEST, API, RUM ... (Optional)
         :param pulumi.Input[str] description: Description of the token.
         :param pulumi.Input[bool] disabled: Flag that controls enabling the token. If set to `true`, the token is disabled, and you can't use it for authentication. Defaults to `false`.
         :param pulumi.Input['OrgTokenDpmLimitsArgs'] dpm_limits: Specify DPM-based limits for this token.
         :param pulumi.Input['OrgTokenHostOrUsageLimitsArgs'] host_or_usage_limits: Specify Usage-based limits for this token.
         :param pulumi.Input[str] name: Name of the token.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] notifications: List of strings specifying where notifications will be sent when an incident occurs. See
-               https://developers.signalfx.com/v2/docs/detector-model#notifications-models for more info
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notifications: Where to send notifications about this token's limits. Please consult the Notification Format laid out in detectors.
         """
         if auth_scopes is not None:
             pulumi.set(__self__, "auth_scopes", auth_scopes)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if disabled is not None:
             pulumi.set(__self__, "disabled", disabled)
@@ -121,16 +120,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def notifications(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of strings specifying where notifications will be sent when an incident occurs. See
-        https://developers.signalfx.com/v2/docs/detector-model#notifications-models for more info
+        Where to send notifications about this token's limits. Please consult the Notification Format laid out in detectors.
         """
         return pulumi.get(self, "notifications")
 
     @notifications.setter
     def notifications(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "notifications", value)
 
@@ -150,16 +148,15 @@
         Input properties used for looking up and filtering OrgToken resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] auth_scopes: Authentication scope, ex: INGEST, API, RUM ... (Optional)
         :param pulumi.Input[str] description: Description of the token.
         :param pulumi.Input[bool] disabled: Flag that controls enabling the token. If set to `true`, the token is disabled, and you can't use it for authentication. Defaults to `false`.
         :param pulumi.Input['OrgTokenDpmLimitsArgs'] dpm_limits: Specify DPM-based limits for this token.
         :param pulumi.Input['OrgTokenHostOrUsageLimitsArgs'] host_or_usage_limits: Specify Usage-based limits for this token.
         :param pulumi.Input[str] name: Name of the token.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] notifications: List of strings specifying where notifications will be sent when an incident occurs. See
-               https://developers.signalfx.com/v2/docs/detector-model#notifications-models for more info
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notifications: Where to send notifications about this token's limits. Please consult the Notification Format laid out in detectors.
         :param pulumi.Input[str] secret: The secret token created by the API. You cannot set this value.
         """
         if auth_scopes is not None:
             pulumi.set(__self__, "auth_scopes", auth_scopes)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if disabled is not None:
@@ -247,16 +244,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def notifications(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of strings specifying where notifications will be sent when an incident occurs. See
-        https://developers.signalfx.com/v2/docs/detector-model#notifications-models for more info
+        Where to send notifications about this token's limits. Please consult the Notification Format laid out in detectors.
         """
         return pulumi.get(self, "notifications")
 
     @notifications.setter
     def notifications(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "notifications", value)
 
@@ -285,14 +281,16 @@
                  host_or_usage_limits: Optional[pulumi.Input[pulumi.InputType['OrgTokenHostOrUsageLimitsArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  notifications: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Manage SignalFx org tokens.
 
+        > **NOTE** When managing Org tokens, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
         myteamkey0 = signalfx.OrgToken("myteamkey0",
@@ -314,26 +312,27 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] auth_scopes: Authentication scope, ex: INGEST, API, RUM ... (Optional)
         :param pulumi.Input[str] description: Description of the token.
         :param pulumi.Input[bool] disabled: Flag that controls enabling the token. If set to `true`, the token is disabled, and you can't use it for authentication. Defaults to `false`.
         :param pulumi.Input[pulumi.InputType['OrgTokenDpmLimitsArgs']] dpm_limits: Specify DPM-based limits for this token.
         :param pulumi.Input[pulumi.InputType['OrgTokenHostOrUsageLimitsArgs']] host_or_usage_limits: Specify Usage-based limits for this token.
         :param pulumi.Input[str] name: Name of the token.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] notifications: List of strings specifying where notifications will be sent when an incident occurs. See
-               https://developers.signalfx.com/v2/docs/detector-model#notifications-models for more info
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notifications: Where to send notifications about this token's limits. Please consult the Notification Format laid out in detectors.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[OrgTokenArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manage SignalFx org tokens.
 
+        > **NOTE** When managing Org tokens, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
+
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
         myteamkey0 = signalfx.OrgToken("myteamkey0",
@@ -419,16 +418,15 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] auth_scopes: Authentication scope, ex: INGEST, API, RUM ... (Optional)
         :param pulumi.Input[str] description: Description of the token.
         :param pulumi.Input[bool] disabled: Flag that controls enabling the token. If set to `true`, the token is disabled, and you can't use it for authentication. Defaults to `false`.
         :param pulumi.Input[pulumi.InputType['OrgTokenDpmLimitsArgs']] dpm_limits: Specify DPM-based limits for this token.
         :param pulumi.Input[pulumi.InputType['OrgTokenHostOrUsageLimitsArgs']] host_or_usage_limits: Specify Usage-based limits for this token.
         :param pulumi.Input[str] name: Name of the token.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] notifications: List of strings specifying where notifications will be sent when an incident occurs. See
-               https://developers.signalfx.com/v2/docs/detector-model#notifications-models for more info
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] notifications: Where to send notifications about this token's limits. Please consult the Notification Format laid out in detectors.
         :param pulumi.Input[str] secret: The secret token created by the API. You cannot set this value.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _OrgTokenState.__new__(_OrgTokenState)
 
         __props__.__dict__["auth_scopes"] = auth_scopes
@@ -489,16 +487,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def notifications(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        List of strings specifying where notifications will be sent when an incident occurs. See
-        https://developers.signalfx.com/v2/docs/detector-model#notifications-models for more info
+        Where to send notifications about this token's limits. Please consult the Notification Format laid out in detectors.
         """
         return pulumi.get(self, "notifications")
 
     @property
     @pulumi.getter
     def secret(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/outputs.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,14 @@
     'TimeChartAxisRight',
     'TimeChartAxisRightWatermark',
     'TimeChartEventOption',
     'TimeChartHistogramOption',
     'TimeChartLegendOptionsField',
     'TimeChartVizOption',
     'WebhookIntegrationHeader',
-    'GetAwsServicesServiceResult',
-    'GetAzureServicesServiceResult',
 ]
 
 @pulumi.output_type
 class AlertMutingRuleFilter(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
@@ -1528,15 +1526,25 @@
                  value_suffix: Optional[str] = None,
                  value_unit: Optional[str] = None):
         """
         :param str label: Label used in the publish statement that displays the plot (metric time series data) you want to customize.
         :param str color: Color to use : gray, blue, azure, navy, brown, orange, yellow, iris, magenta, pink, purple, violet, lilac, emerald, green, aquamarine.
         :param str display_name: Specifies an alternate value for the Plot Name column of the Data Table associated with the chart.
         :param str value_prefix: , `value_suffix` - (Optional) Arbitrary prefix/suffix to display with the value of this plot.
-        :param str value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+               
+               **Notes**
+               
+               It is highly recommended that you use both `max_delay` in your detector configuration and an `extrapolation` policy in your program text to reduce false positives/negatives.
+               
+               `max_delay` allows SignalFx to continue with computation if there is a lag in receiving data points.
+               
+               `extrapolation` allows you to specify how to handle missing data. An extrapolation policy can be added to individual signals by updating the data block in your `program_text`.
+               
+               See [Delayed Datapoints](https://signalfx-product-docs.readthedocs-hosted.com/en/latest/charts/chart-builder.html#delayed-datapoints) for more info.
+        :param str value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         pulumi.set(__self__, "label", label)
         if color is not None:
             pulumi.set(__self__, "color", color)
         if display_name is not None:
             pulumi.set(__self__, "display_name", display_name)
         if value_prefix is not None:
@@ -1571,27 +1579,37 @@
         return pulumi.get(self, "display_name")
 
     @property
     @pulumi.getter(name="valuePrefix")
     def value_prefix(self) -> Optional[str]:
         """
         , `value_suffix` - (Optional) Arbitrary prefix/suffix to display with the value of this plot.
+
+        **Notes**
+
+        It is highly recommended that you use both `max_delay` in your detector configuration and an `extrapolation` policy in your program text to reduce false positives/negatives.
+
+        `max_delay` allows SignalFx to continue with computation if there is a lag in receiving data points.
+
+        `extrapolation` allows you to specify how to handle missing data. An extrapolation policy can be added to individual signals by updating the data block in your `program_text`.
+
+        See [Delayed Datapoints](https://signalfx-product-docs.readthedocs-hosted.com/en/latest/charts/chart-builder.html#delayed-datapoints) for more info.
         """
         return pulumi.get(self, "value_prefix")
 
     @property
     @pulumi.getter(name="valueSuffix")
     def value_suffix(self) -> Optional[str]:
         return pulumi.get(self, "value_suffix")
 
     @property
     @pulumi.getter(name="valueUnit")
     def value_unit(self) -> Optional[str]:
         """
-        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         return pulumi.get(self, "value_unit")
 
 
 @pulumi.output_type
 class HeatmapChartColorRange(dict):
     @staticmethod
@@ -1848,15 +1866,15 @@
                  value_suffix: Optional[str] = None,
                  value_unit: Optional[str] = None):
         """
         :param str label: Label used in the publish statement that displays the plot (metric time series data) you want to customize.
         :param str color: The color to use. Must be one of gray, blue, light_blue, navy, dark_orange, orange, dark_yellow, magenta, cerise, pink, violet, purple, gray_blue, dark_green, green, aquamarine, red, yellow, vivid_yellow, light_green, or lime_green.
         :param str display_name: Specifies an alternate value for the Plot Name column of the Data Table associated with the chart.
         :param str value_prefix: , `value_suffix` - (Optional) Arbitrary prefix/suffix to display with the value of this plot.
-        :param str value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+        :param str value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         pulumi.set(__self__, "label", label)
         if color is not None:
             pulumi.set(__self__, "color", color)
         if display_name is not None:
             pulumi.set(__self__, "display_name", display_name)
         if value_prefix is not None:
@@ -1903,15 +1921,15 @@
     def value_suffix(self) -> Optional[str]:
         return pulumi.get(self, "value_suffix")
 
     @property
     @pulumi.getter(name="valueUnit")
     def value_unit(self) -> Optional[str]:
         """
-        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         return pulumi.get(self, "value_unit")
 
 
 @pulumi.output_type
 class MetricRulesetAggregationRule(dict):
     def __init__(__self__, *,
@@ -1919,14 +1937,15 @@
                  enabled: bool,
                  matchers: Sequence['outputs.MetricRulesetAggregationRuleMatcher'],
                  name: Optional[str] = None):
         """
         :param Sequence['MetricRulesetAggregationRuleAggregatorArgs'] aggregators: Aggregator object
         :param bool enabled: When false, this rule will not generate aggregated MTSs
         :param Sequence['MetricRulesetAggregationRuleMatcherArgs'] matchers: Matcher object
+        :param str name: name of the aggregation rule
         """
         pulumi.set(__self__, "aggregators", aggregators)
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "matchers", matchers)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
@@ -1953,14 +1972,17 @@
         Matcher object
         """
         return pulumi.get(self, "matchers")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
+        """
+        name of the aggregation rule
+        """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
 class MetricRulesetAggregationRuleAggregator(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -2120,23 +2142,23 @@
 
 
 @pulumi.output_type
 class MetricRulesetRoutingRule(dict):
     def __init__(__self__, *,
                  destination: str):
         """
-        :param str destination: end destination of the input metric
+        :param str destination: end destination of the input metric. Must be `RealTime` or `Drop`
         """
         pulumi.set(__self__, "destination", destination)
 
     @property
     @pulumi.getter
     def destination(self) -> str:
         """
-        end destination of the input metric
+        end destination of the input metric. Must be `RealTime` or `Drop`
         """
         return pulumi.get(self, "destination")
 
 
 @pulumi.output_type
 class OrgTokenDpmLimits(dict):
     @staticmethod
@@ -2419,15 +2441,15 @@
                  value_suffix: Optional[str] = None,
                  value_unit: Optional[str] = None):
         """
         :param str label: Label used in the publish statement that displays the plot (metric time series data) you want to customize.
         :param str color: The color to use. Must be one of gray, blue, light_blue, navy, dark_orange, orange, dark_yellow, magenta, cerise, pink, violet, purple, gray_blue, dark_green, green, aquamarine, red, yellow, vivid_yellow, light_green, or lime_green.
         :param str display_name: Specifies an alternate value for the Plot Name column of the Data Table associated with the chart.
         :param str value_prefix: , `value_suffix` - (Optional) Arbitrary prefix/suffix to display with the value of this plot.
-        :param str value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+        :param str value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         pulumi.set(__self__, "label", label)
         if color is not None:
             pulumi.set(__self__, "color", color)
         if display_name is not None:
             pulumi.set(__self__, "display_name", display_name)
         if value_prefix is not None:
@@ -2474,15 +2496,15 @@
     def value_suffix(self) -> Optional[str]:
         return pulumi.get(self, "value_suffix")
 
     @property
     @pulumi.getter(name="valueUnit")
     def value_unit(self) -> Optional[str]:
         """
-        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         return pulumi.get(self, "value_unit")
 
 
 @pulumi.output_type
 class TableChartVizOption(dict):
     @staticmethod
@@ -3026,15 +3048,15 @@
         """
         :param str label: Label used in the publish statement that displays the event query you want to customize.
         :param str axis: Y-axis associated with values for this plot. Must be either `right` or `left`.
         :param str color: Color to use : gray, blue, azure, navy, brown, orange, yellow, iris, magenta, pink, purple, violet, lilac, emerald, green, aquamarine.
         :param str display_name: Specifies an alternate value for the Plot Name column of the Data Table associated with the chart.
         :param str plot_type: The visualization style to use. Must be `"LineChart"`, `"AreaChart"`, `"ColumnChart"`, or `"Histogram"`. Chart level `plot_type` by default.
         :param str value_prefix: , `value_suffix` - (Optional) Arbitrary prefix/suffix to display with the value of this plot.
-        :param str value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+        :param str value_unit: A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         pulumi.set(__self__, "label", label)
         if axis is not None:
             pulumi.set(__self__, "axis", axis)
         if color is not None:
             pulumi.set(__self__, "color", color)
         if display_name is not None:
@@ -3101,15 +3123,15 @@
     def value_suffix(self) -> Optional[str]:
         return pulumi.get(self, "value_suffix")
 
     @property
     @pulumi.getter(name="valueUnit")
     def value_unit(self) -> Optional[str]:
         """
-        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gigibyte, Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
+        A unit to attach to this plot. Units support automatic scaling (eg thousands of bytes will be displayed as kilobytes). Values values are `Bit, Kilobit, Megabit, Gigabit, Terabit, Petabit, Exabit, Zettabit, Yottabit, Byte, Kibibyte, Mebibyte, Gibibyte (note: this was previously typoed as Gigibyte), Tebibyte, Pebibyte, Exbibyte, Zebibyte, Yobibyte, Nanosecond, Microsecond, Millisecond, Second, Minute, Hour, Day, Week`.
         """
         return pulumi.get(self, "value_unit")
 
 
 @pulumi.output_type
 class WebhookIntegrationHeader(dict):
     @staticmethod
@@ -3154,31 +3176,7 @@
     def header_value(self) -> str:
         """
         The value of the header to send
         """
         return pulumi.get(self, "header_value")
 
 
-@pulumi.output_type
-class GetAwsServicesServiceResult(dict):
-    def __init__(__self__, *,
-                 name: str):
-        pulumi.set(__self__, "name", name)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
-
-
-@pulumi.output_type
-class GetAzureServicesServiceResult(dict):
-    def __init__(__self__, *,
-                 name: str):
-        pulumi.set(__self__, "name", name)
-
-    @property
-    @pulumi.getter
-    def name(self) -> str:
-        return pulumi.get(self, "name")
-
-
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/pagerduty/get_integration.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/pagerduty/get_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,17 +87,17 @@
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('signalfx:pagerduty/getIntegration:getIntegration', __args__, opts=opts, typ=GetIntegrationResult).value
 
     return AwaitableGetIntegrationResult(
-        enabled=__ret__.enabled,
-        id=__ret__.id,
-        name=__ret__.name)
+        enabled=pulumi.get(__ret__, 'enabled'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'))
 
 
 @_utilities.lift_output_func(get_integration)
 def get_integration_output(name: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetIntegrationResult]:
     """
     Use this data source to get information on an existing PagerDuty integration.
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/pagerduty/integration.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/pagerduty/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                  api_key: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         SignalFx PagerDuty integrations
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
@@ -158,15 +158,15 @@
     def __init__(__self__,
                  resource_name: str,
                  args: IntegrationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         SignalFx PagerDuty integrations
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/provider.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/servicenow/integration.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/servicenow/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
                  name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Observability Cloud ServiceNow integrations. For help with this integration see [Integration with ServiceNow](https://docs.splunk.com/Observability/admin/notif-services/servicenow.html).
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the Observability Cloud provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the Observability Cloud provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
@@ -329,15 +329,15 @@
     def __init__(__self__,
                  resource_name: str,
                  args: IntegrationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Observability Cloud ServiceNow integrations. For help with this integration see [Integration with ServiceNow](https://docs.splunk.com/Observability/admin/notif-services/servicenow.html).
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the Observability Cloud provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the Observability Cloud provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/single_value_chart.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/single_value_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/slack/integration.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/slack/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
                  enabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  webhook_url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         SignalFx Slack integration.
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
@@ -157,15 +157,15 @@
     def __init__(__self__,
                  resource_name: str,
                  args: IntegrationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         SignalFx Slack integration.
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/table_chart.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/table_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/team.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/team.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
                  notifications_warnings: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Handles management of SignalFx teams.
 
         You can configure [team notification policies](https://docs.signalfx.com/en/latest/managing/teams/team-notifications.html) using this resource and the various `notifications_*` properties.
 
-        > **NOTE** When managing teams use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
+        > **NOTE** When managing teams, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
@@ -388,15 +388,15 @@
                  args: Optional[TeamArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Handles management of SignalFx teams.
 
         You can configure [team notification policies](https://docs.signalfx.com/en/latest/managing/teams/team-notifications.html) using this resource and the various `notifications_*` properties.
 
-        > **NOTE** When managing teams use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
+        > **NOTE** When managing teams, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/text_chart.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/text_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/time_chart.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/time_chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,14 +267,17 @@
 
     @property
     @pulumi.getter(name="legendFieldsToHides")
     def legend_fields_to_hides(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         List of properties that should not be displayed in the chart legend (i.e. dimension names). All the properties are visible by default. Deprecated, please use `legend_options_fields`.
         """
+        warnings.warn("""Please use legend_options_fields""", DeprecationWarning)
+        pulumi.log.warn("""legend_fields_to_hides is deprecated: Please use legend_options_fields""")
+
         return pulumi.get(self, "legend_fields_to_hides")
 
     @legend_fields_to_hides.setter
     def legend_fields_to_hides(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "legend_fields_to_hides", value)
 
     @property
@@ -399,14 +402,17 @@
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Tags associated with the chart
         """
+        warnings.warn("""signalfx_time_chart.tags is being removed in the next release""", DeprecationWarning)
+        pulumi.log.warn("""tags is deprecated: signalfx_time_chart.tags is being removed in the next release""")
+
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
@@ -705,14 +711,17 @@
 
     @property
     @pulumi.getter(name="legendFieldsToHides")
     def legend_fields_to_hides(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         List of properties that should not be displayed in the chart legend (i.e. dimension names). All the properties are visible by default. Deprecated, please use `legend_options_fields`.
         """
+        warnings.warn("""Please use legend_options_fields""", DeprecationWarning)
+        pulumi.log.warn("""legend_fields_to_hides is deprecated: Please use legend_options_fields""")
+
         return pulumi.get(self, "legend_fields_to_hides")
 
     @legend_fields_to_hides.setter
     def legend_fields_to_hides(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "legend_fields_to_hides", value)
 
     @property
@@ -849,14 +858,17 @@
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         Tags associated with the chart
         """
+        warnings.warn("""signalfx_time_chart.tags is being removed in the next release""", DeprecationWarning)
+        pulumi.log.warn("""tags is deprecated: signalfx_time_chart.tags is being removed in the next release""")
+
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
@@ -1344,14 +1356,17 @@
 
     @property
     @pulumi.getter(name="legendFieldsToHides")
     def legend_fields_to_hides(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         List of properties that should not be displayed in the chart legend (i.e. dimension names). All the properties are visible by default. Deprecated, please use `legend_options_fields`.
         """
+        warnings.warn("""Please use legend_options_fields""", DeprecationWarning)
+        pulumi.log.warn("""legend_fields_to_hides is deprecated: Please use legend_options_fields""")
+
         return pulumi.get(self, "legend_fields_to_hides")
 
     @property
     @pulumi.getter(name="legendOptionsFields")
     def legend_options_fields(self) -> pulumi.Output[Optional[Sequence['outputs.TimeChartLegendOptionsField']]]:
         """
         List of property names and enabled flags that should be displayed in the data table for the chart, in the order provided. This option cannot be used with `legend_fields_to_hide`.
@@ -1440,14 +1455,17 @@
 
     @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         Tags associated with the chart
         """
+        warnings.warn("""signalfx_time_chart.tags is being removed in the next release""", DeprecationWarning)
+        pulumi.log.warn("""tags is deprecated: signalfx_time_chart.tags is being removed in the next release""")
+
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="timeRange")
     def time_range(self) -> pulumi.Output[Optional[int]]:
         """
         How many seconds ago from which to display data. For example, the last hour would be `3600`, etc. Conflicts with `start_time` and `end_time`.
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/victorops/integration.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/victorops/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                  enabled: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  post_url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         SignalFx VictorOps integration.
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
@@ -158,15 +158,15 @@
     def __init__(__self__,
                  resource_name: str,
                  args: IntegrationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         SignalFx VictorOps integration.
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx/webhook_integration.py` & `pulumi_signalfx-6.0.0/pulumi_signalfx/webhook_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
                  name: Optional[pulumi.Input[str]] = None,
                  shared_secret: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         SignalFx Webhook integration.
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
 
@@ -224,15 +224,15 @@
     def __init__(__self__,
                  resource_name: str,
                  args: WebhookIntegrationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         SignalFx Webhook integration.
 
-        > **NOTE** When managing integrations use a session token for an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
+        > **NOTE** When managing integrations, use a session token of an administrator to authenticate the SignalFx provider. See [Operations that require a session token for an administrator](https://dev.splunk.com/observability/docs/administration/authtokens#Operations-that-require-a-session-token-for-an-administrator). Otherwise you'll receive a 4xx error.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_signalfx as signalfx
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/PKG-INFO` & `pulumi_signalfx-6.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,13 @@
-Metadata-Version: 2.1
-Name: pulumi-signalfx
-Version: 5.9.0a1678179334
-Summary: A Pulumi package for creating and managing SignalFx resources.
-Home-page: https://pulumi.io
-License: Apache-2.0
-Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
-Keywords: pulumi signalfx
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 [![Actions Status](https://github.com/pulumi/pulumi-signalfx/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-signalfx/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fsignalfx.svg)](https://www.npmjs.com/package/@pulumi/signalfx)
 [![Python version](https://badge.fury.io/py/pulumi-signalfx.svg)](https://pypi.org/project/pulumi-signalfx)
 [![NuGet version](https://badge.fury.io/nu/pulumi.signalfx.svg)](https://badge.fury.io/nu/pulumi.signalfx)
-[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-signalfx/sdk/v5/go)](https://pkg.go.dev/github.com/pulumi/pulumi-signalfx/sdk/v5/go)
+[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-signalfx/sdk/v6/go)](https://pkg.go.dev/github.com/pulumi/pulumi-signalfx/sdk/v6/go)
 [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-signalfx/blob/master/LICENSE)
 
 # SignalFx Resource Provider
 
 The SignalFx resource provider for Pulumi lets you manage SignalFx resources in your cloud programs. To use
 this package, please [install the Pulumi CLI first](https://pulumi.io/).
 
@@ -42,15 +31,15 @@
 
     $ pip install pulumi_signalfx
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-signalfx/sdk/v5
+    $ go get github.com/pulumi/pulumi-signalfx/sdk/v6
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Signalfx
 
@@ -64,9 +53,7 @@
   who need to set their Realm or use a proxy. Note: You likely want to change `customAppUrl` too!
 - `signalfx:customAppUrl` - (Optional) The application URL that users should use to interact with assets in the browser.
   This is used by organizations using specific realms or those with a custom SSO domain.
 
 ## Reference
 
 For further information, please visit [the SignalFx provider docs](https://www.pulumi.com/docs/intro/cloud-providers/signalfx) or for detailed reference documentation, please visit [the API docs](https://www.pulumi.com/docs/reference/pkg/signalfx).
-
-
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/pulumi_signalfx.egg-info/SOURCES.txt` & `pulumi_signalfx-6.0.0/pulumi_signalfx.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 pulumi_signalfx/_utilities.py
 pulumi_signalfx/alert_muting_rule.py
 pulumi_signalfx/dashboard.py
 pulumi_signalfx/dashboard_group.py
 pulumi_signalfx/data_link.py
 pulumi_signalfx/detector.py
 pulumi_signalfx/event_feed_chart.py
-pulumi_signalfx/get_aws_services.py
-pulumi_signalfx/get_azure_services.py
 pulumi_signalfx/get_dimension_values.py
 pulumi_signalfx/heatmap_chart.py
 pulumi_signalfx/list_chart.py
 pulumi_signalfx/metric_ruleset.py
 pulumi_signalfx/org_token.py
 pulumi_signalfx/outputs.py
 pulumi_signalfx/provider.py
@@ -31,28 +29,25 @@
 pulumi_signalfx.egg-info/dependency_links.txt
 pulumi_signalfx.egg-info/not-zip-safe
 pulumi_signalfx.egg-info/requires.txt
 pulumi_signalfx.egg-info/top_level.txt
 pulumi_signalfx/aws/__init__.py
 pulumi_signalfx/aws/_inputs.py
 pulumi_signalfx/aws/external_integration.py
-pulumi_signalfx/aws/get_services.py
 pulumi_signalfx/aws/integration.py
 pulumi_signalfx/aws/outputs.py
 pulumi_signalfx/aws/token_integration.py
 pulumi_signalfx/azure/__init__.py
 pulumi_signalfx/azure/_inputs.py
-pulumi_signalfx/azure/get_services.py
 pulumi_signalfx/azure/integration.py
 pulumi_signalfx/azure/outputs.py
 pulumi_signalfx/config/__init__.py
 pulumi_signalfx/config/vars.py
 pulumi_signalfx/gcp/__init__.py
 pulumi_signalfx/gcp/_inputs.py
-pulumi_signalfx/gcp/get_services.py
 pulumi_signalfx/gcp/integration.py
 pulumi_signalfx/gcp/outputs.py
 pulumi_signalfx/jira/__init__.py
 pulumi_signalfx/jira/integration.py
 pulumi_signalfx/logs/__init__.py
 pulumi_signalfx/logs/_inputs.py
 pulumi_signalfx/logs/outputs.py
```

### Comparing `pulumi_signalfx-5.9.0a1678179334/setup.py` & `pulumi_signalfx-6.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.9.0a1678179334"
-PLUGIN_VERSION = "5.9.0-alpha.1678179334+e6d600fc"
+VERSION = "6.0.0"
+PLUGIN_VERSION = "6.0.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'signalfx', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "signalfx Pulumi Package - Development Version"
 
 
 setup(name='pulumi_signalfx',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing SignalFx resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

