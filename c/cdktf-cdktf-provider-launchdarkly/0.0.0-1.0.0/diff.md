# Comparing `tmp/cdktf-cdktf-provider-launchdarkly-0.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-launchdarkly-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-launchdarkly-0.0.0.tar", last modified: Wed Jul 26 09:30:01 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-launchdarkly-1.0.0.tar", last modified: Wed Jul 26 14:12:26 2023, max compression
```

## Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0.tar` & `cdktf-cdktf-provider-launchdarkly-1.0.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.612438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.616438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   397284 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/_jsii/provider-launchdarkly@0.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/access_token/
--rw-r--r--   0 runner    (1001) docker     (123)    83629 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/access_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/audit_log_subscription/
--rw-r--r--   0 runner    (1001) docker     (123)    52937 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/audit_log_subscription/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/custom_role/
--rw-r--r--   0 runner    (1001) docker     (123)    69533 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/custom_role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_audit_log_subscription/
--rw-r--r--   0 runner    (1001) docker     (123)    55147 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_audit_log_subscription/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_environment/
--rw-r--r--   0 runner    (1001) docker     (123)    70008 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag/
--rw-r--r--   0 runner    (1001) docker     (123)   111540 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag_environment/
--rw-r--r--   0 runner    (1001) docker     (123)   159121 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag_environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_flag_trigger/
--rw-r--r--   0 runner    (1001) docker     (123)    38208 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_flag_trigger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_metric/
--rw-r--r--   0 runner    (1001) docker     (123)    74402 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_project/
--rw-r--r--   0 runner    (1001) docker     (123)    40119 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_relay_proxy_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    42763 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_relay_proxy_configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_segment/
--rw-r--r--   0 runner    (1001) docker     (123)   118998 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_segment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team/
--rw-r--r--   0 runner    (1001) docker     (123)    35527 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_member/
--rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_members/
--rw-r--r--   0 runner    (1001) docker     (123)    31524 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_members/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_webhook/
--rw-r--r--   0 runner    (1001) docker     (123)    48997 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_webhook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/destination/
--rw-r--r--   0 runner    (1001) docker     (123)    32620 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/destination/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/environment/
--rw-r--r--   0 runner    (1001) docker     (123)    72476 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/feature_flag/
--rw-r--r--   0 runner    (1001) docker     (123)   112294 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/feature_flag/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/feature_flag_environment/
--rw-r--r--   0 runner    (1001) docker     (123)   153553 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/feature_flag_environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/flag_trigger/
--rw-r--r--   0 runner    (1001) docker     (123)    36212 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/flag_trigger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/metric/
--rw-r--r--   0 runner    (1001) docker     (123)    72106 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/project/
--rw-r--r--   0 runner    (1001) docker     (123)   109119 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/relay_proxy_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    43692 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/relay_proxy_configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/segment/
--rw-r--r--   0 runner    (1001) docker     (123)   117251 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/segment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/team/
--rw-r--r--   0 runner    (1001) docker     (123)    30096 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/team/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/team_member/
--rw-r--r--   0 runner    (1001) docker     (123)    28110 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/team_member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/team_role_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/team_role_mapping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.624439 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/webhook/
--rw-r--r--   0 runner    (1001) docker     (123)    52330 2023-07-26 09:29:46.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/webhook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:30:01.620438 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-26 09:30:01.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-26 09:30:01.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:30:01.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 09:30:01.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-26 09:30:01.000000 cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.210775 cdktf-cdktf-provider-launchdarkly-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-26 14:12:26.210775 cdktf-cdktf-provider-launchdarkly-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:12:26.210775 cdktf-cdktf-provider-launchdarkly-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.198774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.202774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.202774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   397272 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/_jsii/provider-launchdarkly@1.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.202774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/access_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    83629 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/access_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.202774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/audit_log_subscription/
+-rw-r--r--   0 runner    (1001) docker     (123)    52937 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/audit_log_subscription/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.202774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/custom_role/
+-rw-r--r--   0 runner    (1001) docker     (123)    69533 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/custom_role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.202774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_audit_log_subscription/
+-rw-r--r--   0 runner    (1001) docker     (123)    55147 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_audit_log_subscription/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.202774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_environment/
+-rw-r--r--   0 runner    (1001) docker     (123)    70008 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.202774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag/
+-rw-r--r--   0 runner    (1001) docker     (123)   111540 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag_environment/
+-rw-r--r--   0 runner    (1001) docker     (123)   159121 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag_environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_flag_trigger/
+-rw-r--r--   0 runner    (1001) docker     (123)    38208 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_flag_trigger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_metric/
+-rw-r--r--   0 runner    (1001) docker     (123)    74402 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_project/
+-rw-r--r--   0 runner    (1001) docker     (123)    40119 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_relay_proxy_configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    42763 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_relay_proxy_configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_segment/
+-rw-r--r--   0 runner    (1001) docker     (123)   118998 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_segment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team/
+-rw-r--r--   0 runner    (1001) docker     (123)    35527 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_members/
+-rw-r--r--   0 runner    (1001) docker     (123)    31524 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_members/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_webhook/
+-rw-r--r--   0 runner    (1001) docker     (123)    48997 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_webhook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/destination/
+-rw-r--r--   0 runner    (1001) docker     (123)    32620 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/destination/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)    72476 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/feature_flag/
+-rw-r--r--   0 runner    (1001) docker     (123)   112294 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/feature_flag/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/feature_flag_environment/
+-rw-r--r--   0 runner    (1001) docker     (123)   153553 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/feature_flag_environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/flag_trigger/
+-rw-r--r--   0 runner    (1001) docker     (123)    36212 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/flag_trigger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)    72106 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/project/
+-rw-r--r--   0 runner    (1001) docker     (123)   109119 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/relay_proxy_configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    43692 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/relay_proxy_configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.206774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)   117251 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/segment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.210775 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/team/
+-rw-r--r--   0 runner    (1001) docker     (123)    30096 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/team/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.210775 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/team_member/
+-rw-r--r--   0 runner    (1001) docker     (123)    28110 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/team_member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.210775 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/team_role_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/team_role_mapping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.210775 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/webhook/
+-rw-r--r--   0 runner    (1001) docker     (123)    52330 2023-07-26 14:12:14.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/webhook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:12:26.202774 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-26 14:12:26.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-26 14:12:26.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:12:26.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 14:12:26.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-26 14:12:26.000000 cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/LICENSE` & `cdktf-cdktf-provider-launchdarkly-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/PKG-INFO` & `cdktf-cdktf-provider-launchdarkly-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-launchdarkly
-Version: 0.0.0
+Version: 1.0.0
 Summary: Prebuilt launchdarkly Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-launchdarkly.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-launchdarkly.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/README.md` & `cdktf-cdktf-provider-launchdarkly-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/setup.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-launchdarkly",
-    "version": "0.0.0",
+    "version": "1.0.0",
     "description": "Prebuilt launchdarkly Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-launchdarkly.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -52,15 +52,15 @@
         "cdktf_cdktf_provider_launchdarkly.team",
         "cdktf_cdktf_provider_launchdarkly.team_member",
         "cdktf_cdktf_provider_launchdarkly.team_role_mapping",
         "cdktf_cdktf_provider_launchdarkly.webhook"
     ],
     "package_data": {
         "cdktf_cdktf_provider_launchdarkly._jsii": [
-            "provider-launchdarkly@0.0.0.jsii.tgz"
+            "provider-launchdarkly@1.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_launchdarkly": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/access_token/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/access_token/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_access_token`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_access_token`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token).
+Refer to the Terraform Registory for docs: [`launchdarkly_access_token`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class AccessToken(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.accessToken.AccessToken",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token launchdarkly_access_token}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token launchdarkly_access_token}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         custom_roles: typing.Optional[typing.Sequence[builtins.str]] = None,
@@ -46,27 +46,27 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token launchdarkly_access_token} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token launchdarkly_access_token} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param custom_roles: A list of custom role IDs to use as access limits for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#custom_roles AccessToken#custom_roles}
-        :param default_api_version: The default API version for this token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#default_api_version AccessToken#default_api_version}
-        :param expire: Replace the computed token secret with a new value. The expired secret will no longer be able to authorize usage of the LaunchDarkly API. Should be an expiration time for the current token secret, expressed as a Unix epoch time in milliseconds. Setting this to a negative value will expire the existing token immediately. To reset the token value again, change 'expire' to a new value. Setting this field at resource creation time WILL NOT set an expiration time for the token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#expire AccessToken#expire}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#id AccessToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param inline_roles: inline_roles block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#inline_roles AccessToken#inline_roles}
-        :param name: A human-friendly name for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#name AccessToken#name}
-        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#policy_statements AccessToken#policy_statements}
-        :param role: The default built-in role for the token. Available options are "reader", "writer", and "admin". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#role AccessToken#role}
-        :param service_token: Whether the token is a service token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#service_token AccessToken#service_token}
+        :param custom_roles: A list of custom role IDs to use as access limits for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#custom_roles AccessToken#custom_roles}
+        :param default_api_version: The default API version for this token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#default_api_version AccessToken#default_api_version}
+        :param expire: Replace the computed token secret with a new value. The expired secret will no longer be able to authorize usage of the LaunchDarkly API. Should be an expiration time for the current token secret, expressed as a Unix epoch time in milliseconds. Setting this to a negative value will expire the existing token immediately. To reset the token value again, change 'expire' to a new value. Setting this field at resource creation time WILL NOT set an expiration time for the token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#expire AccessToken#expire}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#id AccessToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param inline_roles: inline_roles block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#inline_roles AccessToken#inline_roles}
+        :param name: A human-friendly name for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#name AccessToken#name}
+        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#policy_statements AccessToken#policy_statements}
+        :param role: The default built-in role for the token. Available options are "reader", "writer", and "admin". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#role AccessToken#role}
+        :param service_token: Whether the token is a service token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#service_token AccessToken#service_token}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -368,23 +368,23 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param custom_roles: A list of custom role IDs to use as access limits for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#custom_roles AccessToken#custom_roles}
-        :param default_api_version: The default API version for this token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#default_api_version AccessToken#default_api_version}
-        :param expire: Replace the computed token secret with a new value. The expired secret will no longer be able to authorize usage of the LaunchDarkly API. Should be an expiration time for the current token secret, expressed as a Unix epoch time in milliseconds. Setting this to a negative value will expire the existing token immediately. To reset the token value again, change 'expire' to a new value. Setting this field at resource creation time WILL NOT set an expiration time for the token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#expire AccessToken#expire}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#id AccessToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param inline_roles: inline_roles block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#inline_roles AccessToken#inline_roles}
-        :param name: A human-friendly name for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#name AccessToken#name}
-        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#policy_statements AccessToken#policy_statements}
-        :param role: The default built-in role for the token. Available options are "reader", "writer", and "admin". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#role AccessToken#role}
-        :param service_token: Whether the token is a service token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#service_token AccessToken#service_token}
+        :param custom_roles: A list of custom role IDs to use as access limits for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#custom_roles AccessToken#custom_roles}
+        :param default_api_version: The default API version for this token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#default_api_version AccessToken#default_api_version}
+        :param expire: Replace the computed token secret with a new value. The expired secret will no longer be able to authorize usage of the LaunchDarkly API. Should be an expiration time for the current token secret, expressed as a Unix epoch time in milliseconds. Setting this to a negative value will expire the existing token immediately. To reset the token value again, change 'expire' to a new value. Setting this field at resource creation time WILL NOT set an expiration time for the token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#expire AccessToken#expire}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#id AccessToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param inline_roles: inline_roles block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#inline_roles AccessToken#inline_roles}
+        :param name: A human-friendly name for the access token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#name AccessToken#name}
+        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#policy_statements AccessToken#policy_statements}
+        :param role: The default built-in role for the token. Available options are "reader", "writer", and "admin". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#role AccessToken#role}
+        :param service_token: Whether the token is a service token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#service_token AccessToken#service_token}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2057e14f74a5d72eae1bfd306b184f12411fbbd7712def89d264547c92f1ea09)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -500,96 +500,96 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def custom_roles(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of custom role IDs to use as access limits for the access token.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#custom_roles AccessToken#custom_roles}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#custom_roles AccessToken#custom_roles}
         '''
         result = self._values.get("custom_roles")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def default_api_version(self) -> typing.Optional[jsii.Number]:
         '''The default API version for this token.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#default_api_version AccessToken#default_api_version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#default_api_version AccessToken#default_api_version}
         '''
         result = self._values.get("default_api_version")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def expire(self) -> typing.Optional[jsii.Number]:
         '''Replace the computed token secret with a new value.
 
         The expired secret will no longer be able to authorize usage of the LaunchDarkly API. Should be an expiration time for the current token secret, expressed as a Unix epoch time in milliseconds. Setting this to a negative value will expire the existing token immediately. To reset the token value again, change 'expire' to a new value. Setting this field at resource creation time WILL NOT set an expiration time for the token.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#expire AccessToken#expire}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#expire AccessToken#expire}
         '''
         result = self._values.get("expire")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#id AccessToken#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#id AccessToken#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def inline_roles(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AccessTokenInlineRoles"]]]:
         '''inline_roles block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#inline_roles AccessToken#inline_roles}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#inline_roles AccessToken#inline_roles}
         '''
         result = self._values.get("inline_roles")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AccessTokenInlineRoles"]]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''A human-friendly name for the access token.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#name AccessToken#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#name AccessToken#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def policy_statements(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AccessTokenPolicyStatements"]]]:
         '''policy_statements block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#policy_statements AccessToken#policy_statements}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#policy_statements AccessToken#policy_statements}
         '''
         result = self._values.get("policy_statements")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AccessTokenPolicyStatements"]]], result)
 
     @builtins.property
     def role(self) -> typing.Optional[builtins.str]:
         '''The default built-in role for the token. Available options are "reader", "writer", and "admin".
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#role AccessToken#role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#role AccessToken#role}
         '''
         result = self._values.get("role")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def service_token(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether the token is a service token.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#service_token AccessToken#service_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#service_token AccessToken#service_token}
         '''
         result = self._values.get("service_token")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -620,19 +620,19 @@
         effect: builtins.str,
         actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
         resources: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#effect AccessToken#effect}.
-        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#actions AccessToken#actions}
-        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#not_actions AccessToken#not_actions}
-        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#not_resources AccessToken#not_resources}
-        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#resources AccessToken#resources}
+        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#effect AccessToken#effect}.
+        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#actions AccessToken#actions}
+        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#not_actions AccessToken#not_actions}
+        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#not_resources AccessToken#not_resources}
+        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#resources AccessToken#resources}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6bf777dc854b3453cf4763366a000825853d9755645cbb159247ac5859373423)
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument not_actions", value=not_actions, expected_type=type_hints["not_actions"])
             check_type(argname="argument not_resources", value=not_resources, expected_type=type_hints["not_resources"])
@@ -647,55 +647,55 @@
         if not_resources is not None:
             self._values["not_resources"] = not_resources
         if resources is not None:
             self._values["resources"] = resources
 
     @builtins.property
     def effect(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#effect AccessToken#effect}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#effect AccessToken#effect}.'''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''An action to perform on a resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#actions AccessToken#actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#actions AccessToken#actions}
         '''
         result = self._values.get("actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted actions will be those actions NOT in this list.
 
         The 'actions' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#not_actions AccessToken#not_actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#not_actions AccessToken#not_actions}
         '''
         result = self._values.get("not_actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted resources will be those resources NOT in this list.
 
         The 'resources' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#not_resources AccessToken#not_resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#not_resources AccessToken#not_resources}
         '''
         result = self._values.get("not_resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of LaunchDarkly resource specifiers.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#resources AccessToken#resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#resources AccessToken#resources}
         '''
         result = self._values.get("resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -961,19 +961,19 @@
         effect: builtins.str,
         actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
         resources: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#effect AccessToken#effect}.
-        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#actions AccessToken#actions}
-        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#not_actions AccessToken#not_actions}
-        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#not_resources AccessToken#not_resources}
-        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#resources AccessToken#resources}
+        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#effect AccessToken#effect}.
+        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#actions AccessToken#actions}
+        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#not_actions AccessToken#not_actions}
+        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#not_resources AccessToken#not_resources}
+        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#resources AccessToken#resources}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__69536178ec1dc81c007afab784c9a2f1c87f74bac4ab24e4995657c04b64bc4a)
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument not_actions", value=not_actions, expected_type=type_hints["not_actions"])
             check_type(argname="argument not_resources", value=not_resources, expected_type=type_hints["not_resources"])
@@ -988,55 +988,55 @@
         if not_resources is not None:
             self._values["not_resources"] = not_resources
         if resources is not None:
             self._values["resources"] = resources
 
     @builtins.property
     def effect(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#effect AccessToken#effect}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#effect AccessToken#effect}.'''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''An action to perform on a resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#actions AccessToken#actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#actions AccessToken#actions}
         '''
         result = self._values.get("actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted actions will be those actions NOT in this list.
 
         The 'actions' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#not_actions AccessToken#not_actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#not_actions AccessToken#not_actions}
         '''
         result = self._values.get("not_actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted resources will be those resources NOT in this list.
 
         The 'resources' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#not_resources AccessToken#not_resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#not_resources AccessToken#not_resources}
         '''
         result = self._values.get("not_resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of LaunchDarkly resource specifiers.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/access_token#resources AccessToken#resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/access_token#resources AccessToken#resources}
         '''
         result = self._values.get("resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/audit_log_subscription/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/audit_log_subscription/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_audit_log_subscription`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_audit_log_subscription`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription).
+Refer to the Terraform Registory for docs: [`launchdarkly_audit_log_subscription`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class AuditLogSubscription(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.auditLogSubscription.AuditLogSubscription",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription launchdarkly_audit_log_subscription}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription launchdarkly_audit_log_subscription}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         config: typing.Mapping[builtins.str, builtins.str],
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription launchdarkly_audit_log_subscription} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription launchdarkly_audit_log_subscription} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param config: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#config AuditLogSubscription#config}.
-        :param integration_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#integration_key AuditLogSubscription#integration_key}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#name AuditLogSubscription#name}.
-        :param on: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#on AuditLogSubscription#on}.
-        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#statements AuditLogSubscription#statements}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#id AuditLogSubscription#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#tags AuditLogSubscription#tags}
+        :param config: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#config AuditLogSubscription#config}.
+        :param integration_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#integration_key AuditLogSubscription#integration_key}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#name AuditLogSubscription#name}.
+        :param on: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#on AuditLogSubscription#on}.
+        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#statements AuditLogSubscription#statements}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#id AuditLogSubscription#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#tags AuditLogSubscription#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -285,21 +285,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param config: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#config AuditLogSubscription#config}.
-        :param integration_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#integration_key AuditLogSubscription#integration_key}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#name AuditLogSubscription#name}.
-        :param on: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#on AuditLogSubscription#on}.
-        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#statements AuditLogSubscription#statements}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#id AuditLogSubscription#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#tags AuditLogSubscription#tags}
+        :param config: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#config AuditLogSubscription#config}.
+        :param integration_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#integration_key AuditLogSubscription#integration_key}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#name AuditLogSubscription#name}.
+        :param on: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#on AuditLogSubscription#on}.
+        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#statements AuditLogSubscription#statements}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#id AuditLogSubscription#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#tags AuditLogSubscription#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ef1e41a2cdac9756b56ce790ba595e5e76b13fcfd9f0a7f2d71efe562ae45ed6)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -403,67 +403,67 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def config(self) -> typing.Mapping[builtins.str, builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#config AuditLogSubscription#config}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#config AuditLogSubscription#config}.'''
         result = self._values.get("config")
         assert result is not None, "Required property 'config' is missing"
         return typing.cast(typing.Mapping[builtins.str, builtins.str], result)
 
     @builtins.property
     def integration_key(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#integration_key AuditLogSubscription#integration_key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#integration_key AuditLogSubscription#integration_key}.'''
         result = self._values.get("integration_key")
         assert result is not None, "Required property 'integration_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#name AuditLogSubscription#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#name AuditLogSubscription#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def on(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#on AuditLogSubscription#on}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#on AuditLogSubscription#on}.'''
         result = self._values.get("on")
         assert result is not None, "Required property 'on' is missing"
         return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], result)
 
     @builtins.property
     def statements(
         self,
     ) -> typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AuditLogSubscriptionStatements"]]:
         '''statements block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#statements AuditLogSubscription#statements}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#statements AuditLogSubscription#statements}
         '''
         result = self._values.get("statements")
         assert result is not None, "Required property 'statements' is missing"
         return typing.cast(typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["AuditLogSubscriptionStatements"]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#id AuditLogSubscription#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#id AuditLogSubscription#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#tags AuditLogSubscription#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#tags AuditLogSubscription#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -494,19 +494,19 @@
         effect: builtins.str,
         actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
         resources: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#effect AuditLogSubscription#effect}.
-        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#actions AuditLogSubscription#actions}
-        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#not_actions AuditLogSubscription#not_actions}
-        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#not_resources AuditLogSubscription#not_resources}
-        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#resources AuditLogSubscription#resources}
+        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#effect AuditLogSubscription#effect}.
+        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#actions AuditLogSubscription#actions}
+        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#not_actions AuditLogSubscription#not_actions}
+        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#not_resources AuditLogSubscription#not_resources}
+        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#resources AuditLogSubscription#resources}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7eafab4833c3c1fd2c0d9c87f5e7f4b213057774377a08fc698b07c04d741b68)
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument not_actions", value=not_actions, expected_type=type_hints["not_actions"])
             check_type(argname="argument not_resources", value=not_resources, expected_type=type_hints["not_resources"])
@@ -521,55 +521,55 @@
         if not_resources is not None:
             self._values["not_resources"] = not_resources
         if resources is not None:
             self._values["resources"] = resources
 
     @builtins.property
     def effect(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#effect AuditLogSubscription#effect}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#effect AuditLogSubscription#effect}.'''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''An action to perform on a resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#actions AuditLogSubscription#actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#actions AuditLogSubscription#actions}
         '''
         result = self._values.get("actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted actions will be those actions NOT in this list.
 
         The 'actions' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#not_actions AuditLogSubscription#not_actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#not_actions AuditLogSubscription#not_actions}
         '''
         result = self._values.get("not_actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted resources will be those resources NOT in this list.
 
         The 'resources' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#not_resources AuditLogSubscription#not_resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#not_resources AuditLogSubscription#not_resources}
         '''
         result = self._values.get("not_resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of LaunchDarkly resource specifiers.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/audit_log_subscription#resources AuditLogSubscription#resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/audit_log_subscription#resources AuditLogSubscription#resources}
         '''
         result = self._values.get("resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/custom_role/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/custom_role/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_custom_role`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_custom_role`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role).
+Refer to the Terraform Registory for docs: [`launchdarkly_custom_role`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class CustomRole(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.customRole.CustomRole",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role launchdarkly_custom_role}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role launchdarkly_custom_role}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role launchdarkly_custom_role} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role launchdarkly_custom_role} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: A unique key that will be used to reference the custom role in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#key CustomRole#key}
-        :param name: A name for the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#name CustomRole#name}
-        :param base_permissions: The base permission level - either reader or no_access. Defaults to reader. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#base_permissions CustomRole#base_permissions}
-        :param description: Description of the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#description CustomRole#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#id CustomRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#policy CustomRole#policy}
-        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#policy_statements CustomRole#policy_statements}
+        :param key: A unique key that will be used to reference the custom role in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#key CustomRole#key}
+        :param name: A name for the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#name CustomRole#name}
+        :param base_permissions: The base permission level - either reader or no_access. Defaults to reader. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#base_permissions CustomRole#base_permissions}
+        :param description: Description of the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#description CustomRole#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#id CustomRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#policy CustomRole#policy}
+        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#policy_statements CustomRole#policy_statements}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -298,21 +298,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: A unique key that will be used to reference the custom role in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#key CustomRole#key}
-        :param name: A name for the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#name CustomRole#name}
-        :param base_permissions: The base permission level - either reader or no_access. Defaults to reader. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#base_permissions CustomRole#base_permissions}
-        :param description: Description of the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#description CustomRole#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#id CustomRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#policy CustomRole#policy}
-        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#policy_statements CustomRole#policy_statements}
+        :param key: A unique key that will be used to reference the custom role in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#key CustomRole#key}
+        :param name: A name for the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#name CustomRole#name}
+        :param base_permissions: The base permission level - either reader or no_access. Defaults to reader. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#base_permissions CustomRole#base_permissions}
+        :param description: Description of the custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#description CustomRole#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#id CustomRole#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#policy CustomRole#policy}
+        :param policy_statements: policy_statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#policy_statements CustomRole#policy_statements}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__07c8f74a83c7759d8c01598cfa8dc958eb71b3c4c22021be7d2d89ce6c766d90)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -421,76 +421,76 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''A unique key that will be used to reference the custom role in your code.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#key CustomRole#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#key CustomRole#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''A name for the custom role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#name CustomRole#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#name CustomRole#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def base_permissions(self) -> typing.Optional[builtins.str]:
         '''The base permission level - either reader or no_access. Defaults to reader.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#base_permissions CustomRole#base_permissions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#base_permissions CustomRole#base_permissions}
         '''
         result = self._values.get("base_permissions")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''Description of the custom role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#description CustomRole#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#description CustomRole#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#id CustomRole#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#id CustomRole#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def policy(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["CustomRolePolicy"]]]:
         '''policy block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#policy CustomRole#policy}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#policy CustomRole#policy}
         '''
         result = self._values.get("policy")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["CustomRolePolicy"]]], result)
 
     @builtins.property
     def policy_statements(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["CustomRolePolicyStatements"]]]:
         '''policy_statements block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#policy_statements CustomRole#policy_statements}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#policy_statements CustomRole#policy_statements}
         '''
         result = self._values.get("policy_statements")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["CustomRolePolicyStatements"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -513,46 +513,46 @@
         self,
         *,
         actions: typing.Sequence[builtins.str],
         effect: builtins.str,
         resources: typing.Sequence[builtins.str],
     ) -> None:
         '''
-        :param actions: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#actions CustomRole#actions}.
-        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#effect CustomRole#effect}.
-        :param resources: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#resources CustomRole#resources}.
+        :param actions: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#actions CustomRole#actions}.
+        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#effect CustomRole#effect}.
+        :param resources: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#resources CustomRole#resources}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e0fff094e247e8f703f81b4e9562b0b46c16f58d75ce567d9573162aae6ea0e0)
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument resources", value=resources, expected_type=type_hints["resources"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "actions": actions,
             "effect": effect,
             "resources": resources,
         }
 
     @builtins.property
     def actions(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#actions CustomRole#actions}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#actions CustomRole#actions}.'''
         result = self._values.get("actions")
         assert result is not None, "Required property 'actions' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def effect(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#effect CustomRole#effect}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#effect CustomRole#effect}.'''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def resources(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#resources CustomRole#resources}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#resources CustomRole#resources}.'''
         result = self._values.get("resources")
         assert result is not None, "Required property 'resources' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -768,19 +768,19 @@
         effect: builtins.str,
         actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
         resources: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#effect CustomRole#effect}.
-        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#actions CustomRole#actions}
-        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#not_actions CustomRole#not_actions}
-        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#not_resources CustomRole#not_resources}
-        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#resources CustomRole#resources}
+        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#effect CustomRole#effect}.
+        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#actions CustomRole#actions}
+        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#not_actions CustomRole#not_actions}
+        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#not_resources CustomRole#not_resources}
+        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#resources CustomRole#resources}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7176f75a37625f31b0c968054092a5d514a83466831576d24355e3e80666e824)
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument not_actions", value=not_actions, expected_type=type_hints["not_actions"])
             check_type(argname="argument not_resources", value=not_resources, expected_type=type_hints["not_resources"])
@@ -795,55 +795,55 @@
         if not_resources is not None:
             self._values["not_resources"] = not_resources
         if resources is not None:
             self._values["resources"] = resources
 
     @builtins.property
     def effect(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#effect CustomRole#effect}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#effect CustomRole#effect}.'''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''An action to perform on a resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#actions CustomRole#actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#actions CustomRole#actions}
         '''
         result = self._values.get("actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted actions will be those actions NOT in this list.
 
         The 'actions' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#not_actions CustomRole#not_actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#not_actions CustomRole#not_actions}
         '''
         result = self._values.get("not_actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted resources will be those resources NOT in this list.
 
         The 'resources' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#not_resources CustomRole#not_resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#not_resources CustomRole#not_resources}
         '''
         result = self._values.get("not_resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of LaunchDarkly resource specifiers.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/custom_role#resources CustomRole#resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/custom_role#resources CustomRole#resources}
         '''
         result = self._values.get("resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_audit_log_subscription/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_audit_log_subscription/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_audit_log_subscription`
 
-Refer to the Terraform Registory for docs: [`data_launchdarkly_audit_log_subscription`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription).
+Refer to the Terraform Registory for docs: [`data_launchdarkly_audit_log_subscription`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataLaunchdarklyAuditLogSubscription(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyAuditLogSubscription.DataLaunchdarklyAuditLogSubscription",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription launchdarkly_audit_log_subscription}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription launchdarkly_audit_log_subscription}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription launchdarkly_audit_log_subscription} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription launchdarkly_audit_log_subscription} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: The audit log subscription ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#id DataLaunchdarklyAuditLogSubscription#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param integration_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#integration_key DataLaunchdarklyAuditLogSubscription#integration_key}.
-        :param config: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#config DataLaunchdarklyAuditLogSubscription#config}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#name DataLaunchdarklyAuditLogSubscription#name}.
-        :param on: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#on DataLaunchdarklyAuditLogSubscription#on}.
-        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#statements DataLaunchdarklyAuditLogSubscription#statements}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#tags DataLaunchdarklyAuditLogSubscription#tags}
+        :param id: The audit log subscription ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#id DataLaunchdarklyAuditLogSubscription#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param integration_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#integration_key DataLaunchdarklyAuditLogSubscription#integration_key}.
+        :param config: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#config DataLaunchdarklyAuditLogSubscription#config}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#name DataLaunchdarklyAuditLogSubscription#name}.
+        :param on: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#on DataLaunchdarklyAuditLogSubscription#on}.
+        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#statements DataLaunchdarklyAuditLogSubscription#statements}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#tags DataLaunchdarklyAuditLogSubscription#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -299,21 +299,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: The audit log subscription ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#id DataLaunchdarklyAuditLogSubscription#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param integration_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#integration_key DataLaunchdarklyAuditLogSubscription#integration_key}.
-        :param config: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#config DataLaunchdarklyAuditLogSubscription#config}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#name DataLaunchdarklyAuditLogSubscription#name}.
-        :param on: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#on DataLaunchdarklyAuditLogSubscription#on}.
-        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#statements DataLaunchdarklyAuditLogSubscription#statements}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#tags DataLaunchdarklyAuditLogSubscription#tags}
+        :param id: The audit log subscription ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#id DataLaunchdarklyAuditLogSubscription#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param integration_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#integration_key DataLaunchdarklyAuditLogSubscription#integration_key}.
+        :param config: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#config DataLaunchdarklyAuditLogSubscription#config}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#name DataLaunchdarklyAuditLogSubscription#name}.
+        :param on: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#on DataLaunchdarklyAuditLogSubscription#on}.
+        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#statements DataLaunchdarklyAuditLogSubscription#statements}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#tags DataLaunchdarklyAuditLogSubscription#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__10868b98900046cc2261e2c194d4755bb088a829c32d6db63109a63b17d26f89)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -422,66 +422,66 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> builtins.str:
         '''The audit log subscription ID.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#id DataLaunchdarklyAuditLogSubscription#id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#id DataLaunchdarklyAuditLogSubscription#id}
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         assert result is not None, "Required property 'id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def integration_key(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#integration_key DataLaunchdarklyAuditLogSubscription#integration_key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#integration_key DataLaunchdarklyAuditLogSubscription#integration_key}.'''
         result = self._values.get("integration_key")
         assert result is not None, "Required property 'integration_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def config(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#config DataLaunchdarklyAuditLogSubscription#config}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#config DataLaunchdarklyAuditLogSubscription#config}.'''
         result = self._values.get("config")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#name DataLaunchdarklyAuditLogSubscription#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#name DataLaunchdarklyAuditLogSubscription#name}.'''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def on(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#on DataLaunchdarklyAuditLogSubscription#on}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#on DataLaunchdarklyAuditLogSubscription#on}.'''
         result = self._values.get("on")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def statements(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyAuditLogSubscriptionStatements"]]]:
         '''statements block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#statements DataLaunchdarklyAuditLogSubscription#statements}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#statements DataLaunchdarklyAuditLogSubscription#statements}
         '''
         result = self._values.get("statements")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyAuditLogSubscriptionStatements"]]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#tags DataLaunchdarklyAuditLogSubscription#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#tags DataLaunchdarklyAuditLogSubscription#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -512,19 +512,19 @@
         effect: builtins.str,
         actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
         resources: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#effect DataLaunchdarklyAuditLogSubscription#effect}.
-        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#actions DataLaunchdarklyAuditLogSubscription#actions}
-        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#not_actions DataLaunchdarklyAuditLogSubscription#not_actions}
-        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#not_resources DataLaunchdarklyAuditLogSubscription#not_resources}
-        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#resources DataLaunchdarklyAuditLogSubscription#resources}
+        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#effect DataLaunchdarklyAuditLogSubscription#effect}.
+        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#actions DataLaunchdarklyAuditLogSubscription#actions}
+        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#not_actions DataLaunchdarklyAuditLogSubscription#not_actions}
+        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#not_resources DataLaunchdarklyAuditLogSubscription#not_resources}
+        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#resources DataLaunchdarklyAuditLogSubscription#resources}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d84fab502e6754284d5141445739f97e145562d2a1ffea5314ce1fcaf1f57ab4)
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument not_actions", value=not_actions, expected_type=type_hints["not_actions"])
             check_type(argname="argument not_resources", value=not_resources, expected_type=type_hints["not_resources"])
@@ -539,55 +539,55 @@
         if not_resources is not None:
             self._values["not_resources"] = not_resources
         if resources is not None:
             self._values["resources"] = resources
 
     @builtins.property
     def effect(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#effect DataLaunchdarklyAuditLogSubscription#effect}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#effect DataLaunchdarklyAuditLogSubscription#effect}.'''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''An action to perform on a resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#actions DataLaunchdarklyAuditLogSubscription#actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#actions DataLaunchdarklyAuditLogSubscription#actions}
         '''
         result = self._values.get("actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted actions will be those actions NOT in this list.
 
         The 'actions' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#not_actions DataLaunchdarklyAuditLogSubscription#not_actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#not_actions DataLaunchdarklyAuditLogSubscription#not_actions}
         '''
         result = self._values.get("not_actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted resources will be those resources NOT in this list.
 
         The 'resources' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#not_resources DataLaunchdarklyAuditLogSubscription#not_resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#not_resources DataLaunchdarklyAuditLogSubscription#not_resources}
         '''
         result = self._values.get("not_resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of LaunchDarkly resource specifiers.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/audit_log_subscription#resources DataLaunchdarklyAuditLogSubscription#resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/audit_log_subscription#resources DataLaunchdarklyAuditLogSubscription#resources}
         '''
         result = self._values.get("resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_environment/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_environment/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_environment`
 
-Refer to the Terraform Registory for docs: [`data_launchdarkly_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment).
+Refer to the Terraform Registory for docs: [`data_launchdarkly_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataLaunchdarklyEnvironment(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyEnvironment.DataLaunchdarklyEnvironment",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment launchdarkly_environment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment launchdarkly_environment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -47,28 +47,28 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment launchdarkly_environment} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment launchdarkly_environment} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: A project-unique key for the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#key DataLaunchdarklyEnvironment#key}
-        :param project_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#project_key DataLaunchdarklyEnvironment#project_key}.
-        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#approval_settings DataLaunchdarklyEnvironment#approval_settings}
-        :param confirm_changes: Whether or not to require confirmation for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#confirm_changes DataLaunchdarklyEnvironment#confirm_changes}
-        :param default_track_events: Whether or not to default to sending data export events for flags created in the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#default_track_events DataLaunchdarklyEnvironment#default_track_events}
-        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#default_ttl DataLaunchdarklyEnvironment#default_ttl}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#id DataLaunchdarklyEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param require_comments: Whether or not to require comments for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#require_comments DataLaunchdarklyEnvironment#require_comments}
-        :param secure_mode: Whether or not to use secure mode. Secure mode ensures a user of the client-side SDK cannot impersonate another user Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#secure_mode DataLaunchdarklyEnvironment#secure_mode}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#tags DataLaunchdarklyEnvironment#tags}
+        :param key: A project-unique key for the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#key DataLaunchdarklyEnvironment#key}
+        :param project_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#project_key DataLaunchdarklyEnvironment#project_key}.
+        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#approval_settings DataLaunchdarklyEnvironment#approval_settings}
+        :param confirm_changes: Whether or not to require confirmation for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#confirm_changes DataLaunchdarklyEnvironment#confirm_changes}
+        :param default_track_events: Whether or not to default to sending data export events for flags created in the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#default_track_events DataLaunchdarklyEnvironment#default_track_events}
+        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#default_ttl DataLaunchdarklyEnvironment#default_ttl}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#id DataLaunchdarklyEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param require_comments: Whether or not to require comments for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#require_comments DataLaunchdarklyEnvironment#require_comments}
+        :param secure_mode: Whether or not to use secure mode. Secure mode ensures a user of the client-side SDK cannot impersonate another user Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#secure_mode DataLaunchdarklyEnvironment#secure_mode}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#tags DataLaunchdarklyEnvironment#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -388,19 +388,19 @@
         can_apply_declined_changes: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         can_review_own_request: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         min_num_approvals: typing.Optional[jsii.Number] = None,
         required: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         required_approval_tags: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param can_apply_declined_changes: Whether changes can be applied as long as minNumApprovals is met, regardless of whether any reviewers have declined a request. Defaults to true Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#can_apply_declined_changes DataLaunchdarklyEnvironment#can_apply_declined_changes}
-        :param can_review_own_request: Whether requesters can approve or decline their own request. They may always comment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#can_review_own_request DataLaunchdarklyEnvironment#can_review_own_request}
-        :param min_num_approvals: The number of approvals required before an approval request can be applied. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#min_num_approvals DataLaunchdarklyEnvironment#min_num_approvals}
-        :param required: Whether any changes to flags in this environment will require approval. You may only set required or requiredApprovalTags, not both. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#required DataLaunchdarklyEnvironment#required}
-        :param required_approval_tags: An array of tags used to specify which flags with those tags require approval. You may only set requiredApprovalTags or required, not both. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#required_approval_tags DataLaunchdarklyEnvironment#required_approval_tags}
+        :param can_apply_declined_changes: Whether changes can be applied as long as minNumApprovals is met, regardless of whether any reviewers have declined a request. Defaults to true Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#can_apply_declined_changes DataLaunchdarklyEnvironment#can_apply_declined_changes}
+        :param can_review_own_request: Whether requesters can approve or decline their own request. They may always comment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#can_review_own_request DataLaunchdarklyEnvironment#can_review_own_request}
+        :param min_num_approvals: The number of approvals required before an approval request can be applied. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#min_num_approvals DataLaunchdarklyEnvironment#min_num_approvals}
+        :param required: Whether any changes to flags in this environment will require approval. You may only set required or requiredApprovalTags, not both. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#required DataLaunchdarklyEnvironment#required}
+        :param required_approval_tags: An array of tags used to specify which flags with those tags require approval. You may only set requiredApprovalTags or required, not both. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#required_approval_tags DataLaunchdarklyEnvironment#required_approval_tags}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e644e3d96291796ef3c860101dd3069ffac4d5b86a21ec0e22038ff7d565ccaa)
             check_type(argname="argument can_apply_declined_changes", value=can_apply_declined_changes, expected_type=type_hints["can_apply_declined_changes"])
             check_type(argname="argument can_review_own_request", value=can_review_own_request, expected_type=type_hints["can_review_own_request"])
             check_type(argname="argument min_num_approvals", value=min_num_approvals, expected_type=type_hints["min_num_approvals"])
             check_type(argname="argument required", value=required, expected_type=type_hints["required"])
@@ -421,59 +421,59 @@
     def can_apply_declined_changes(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether changes can be applied as long as minNumApprovals is met, regardless of whether any reviewers have declined a request.
 
         Defaults to true
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#can_apply_declined_changes DataLaunchdarklyEnvironment#can_apply_declined_changes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#can_apply_declined_changes DataLaunchdarklyEnvironment#can_apply_declined_changes}
         '''
         result = self._values.get("can_apply_declined_changes")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def can_review_own_request(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether requesters can approve or decline their own request. They may always comment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#can_review_own_request DataLaunchdarklyEnvironment#can_review_own_request}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#can_review_own_request DataLaunchdarklyEnvironment#can_review_own_request}
         '''
         result = self._values.get("can_review_own_request")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def min_num_approvals(self) -> typing.Optional[jsii.Number]:
         '''The number of approvals required before an approval request can be applied.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#min_num_approvals DataLaunchdarklyEnvironment#min_num_approvals}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#min_num_approvals DataLaunchdarklyEnvironment#min_num_approvals}
         '''
         result = self._values.get("min_num_approvals")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def required(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether any changes to flags in this environment will require approval.
 
         You may only set required or requiredApprovalTags, not both.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#required DataLaunchdarklyEnvironment#required}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#required DataLaunchdarklyEnvironment#required}
         '''
         result = self._values.get("required")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def required_approval_tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''An array of tags used to specify which flags with those tags require approval.
 
         You may only set requiredApprovalTags or required, not both.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#required_approval_tags DataLaunchdarklyEnvironment#required_approval_tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#required_approval_tags DataLaunchdarklyEnvironment#required_approval_tags}
         '''
         result = self._values.get("required_approval_tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -798,24 +798,24 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: A project-unique key for the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#key DataLaunchdarklyEnvironment#key}
-        :param project_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#project_key DataLaunchdarklyEnvironment#project_key}.
-        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#approval_settings DataLaunchdarklyEnvironment#approval_settings}
-        :param confirm_changes: Whether or not to require confirmation for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#confirm_changes DataLaunchdarklyEnvironment#confirm_changes}
-        :param default_track_events: Whether or not to default to sending data export events for flags created in the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#default_track_events DataLaunchdarklyEnvironment#default_track_events}
-        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#default_ttl DataLaunchdarklyEnvironment#default_ttl}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#id DataLaunchdarklyEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param require_comments: Whether or not to require comments for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#require_comments DataLaunchdarklyEnvironment#require_comments}
-        :param secure_mode: Whether or not to use secure mode. Secure mode ensures a user of the client-side SDK cannot impersonate another user Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#secure_mode DataLaunchdarklyEnvironment#secure_mode}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#tags DataLaunchdarklyEnvironment#tags}
+        :param key: A project-unique key for the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#key DataLaunchdarklyEnvironment#key}
+        :param project_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#project_key DataLaunchdarklyEnvironment#project_key}.
+        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#approval_settings DataLaunchdarklyEnvironment#approval_settings}
+        :param confirm_changes: Whether or not to require confirmation for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#confirm_changes DataLaunchdarklyEnvironment#confirm_changes}
+        :param default_track_events: Whether or not to default to sending data export events for flags created in the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#default_track_events DataLaunchdarklyEnvironment#default_track_events}
+        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#default_ttl DataLaunchdarklyEnvironment#default_ttl}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#id DataLaunchdarklyEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param require_comments: Whether or not to require comments for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#require_comments DataLaunchdarklyEnvironment#require_comments}
+        :param secure_mode: Whether or not to use secure mode. Secure mode ensures a user of the client-side SDK cannot impersonate another user Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#secure_mode DataLaunchdarklyEnvironment#secure_mode}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#tags DataLaunchdarklyEnvironment#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4ee324addf376c393e15f834298d163e79f6d102ae082c6a94d0c21841045aae)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -933,110 +933,110 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''A project-unique key for the new environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#key DataLaunchdarklyEnvironment#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#key DataLaunchdarklyEnvironment#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#project_key DataLaunchdarklyEnvironment#project_key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#project_key DataLaunchdarklyEnvironment#project_key}.'''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def approval_settings(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataLaunchdarklyEnvironmentApprovalSettings]]]:
         '''approval_settings block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#approval_settings DataLaunchdarklyEnvironment#approval_settings}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#approval_settings DataLaunchdarklyEnvironment#approval_settings}
         '''
         result = self._values.get("approval_settings")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataLaunchdarklyEnvironmentApprovalSettings]]], result)
 
     @builtins.property
     def confirm_changes(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not to require confirmation for flag and segment changes in this environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#confirm_changes DataLaunchdarklyEnvironment#confirm_changes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#confirm_changes DataLaunchdarklyEnvironment#confirm_changes}
         '''
         result = self._values.get("confirm_changes")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def default_track_events(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not to default to sending data export events for flags created in the environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#default_track_events DataLaunchdarklyEnvironment#default_track_events}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#default_track_events DataLaunchdarklyEnvironment#default_track_events}
         '''
         result = self._values.get("default_track_events")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def default_ttl(self) -> typing.Optional[jsii.Number]:
         '''The TTL for the environment.
 
         This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#default_ttl DataLaunchdarklyEnvironment#default_ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#default_ttl DataLaunchdarklyEnvironment#default_ttl}
         '''
         result = self._values.get("default_ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#id DataLaunchdarklyEnvironment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#id DataLaunchdarklyEnvironment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def require_comments(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not to require comments for flag and segment changes in this environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#require_comments DataLaunchdarklyEnvironment#require_comments}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#require_comments DataLaunchdarklyEnvironment#require_comments}
         '''
         result = self._values.get("require_comments")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def secure_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not to use secure mode.
 
         Secure mode ensures a user of the client-side SDK cannot impersonate another user
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#secure_mode DataLaunchdarklyEnvironment#secure_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#secure_mode DataLaunchdarklyEnvironment#secure_mode}
         '''
         result = self._values.get("secure_mode")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/environment#tags DataLaunchdarklyEnvironment#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/environment#tags DataLaunchdarklyEnvironment#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_feature_flag`
 
-Refer to the Terraform Registory for docs: [`data_launchdarkly_feature_flag`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag).
+Refer to the Terraform Registory for docs: [`data_launchdarkly_feature_flag`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataLaunchdarklyFeatureFlag(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyFeatureFlag.DataLaunchdarklyFeatureFlag",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag launchdarkly_feature_flag}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag launchdarkly_feature_flag}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -50,31 +50,31 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag launchdarkly_feature_flag} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag launchdarkly_feature_flag} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: A unique key that will be used to reference the flag in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#project_key DataLaunchdarklyFeatureFlag#project_key}
-        :param archived: Whether to archive the flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#archived DataLaunchdarklyFeatureFlag#archived}
-        :param client_side_availability: client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#client_side_availability DataLaunchdarklyFeatureFlag#client_side_availability}
-        :param custom_properties: custom_properties block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#custom_properties DataLaunchdarklyFeatureFlag#custom_properties}
-        :param defaults: defaults block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#defaults DataLaunchdarklyFeatureFlag#defaults}
-        :param description: A short description of what the flag will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#description DataLaunchdarklyFeatureFlag#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#id DataLaunchdarklyFeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param include_in_snippet: Whether or not this flag should be made available to the client-side JavaScript SDK. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#include_in_snippet DataLaunchdarklyFeatureFlag#include_in_snippet}
-        :param maintainer_id: The LaunchDarkly id of the user who will maintain the flag. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#maintainer_id DataLaunchdarklyFeatureFlag#maintainer_id}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#tags DataLaunchdarklyFeatureFlag#tags}
-        :param temporary: Whether or not the flag is a temporary flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#temporary DataLaunchdarklyFeatureFlag#temporary}
-        :param variations: variations block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#variations DataLaunchdarklyFeatureFlag#variations}
+        :param key: A unique key that will be used to reference the flag in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#project_key DataLaunchdarklyFeatureFlag#project_key}
+        :param archived: Whether to archive the flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#archived DataLaunchdarklyFeatureFlag#archived}
+        :param client_side_availability: client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#client_side_availability DataLaunchdarklyFeatureFlag#client_side_availability}
+        :param custom_properties: custom_properties block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#custom_properties DataLaunchdarklyFeatureFlag#custom_properties}
+        :param defaults: defaults block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#defaults DataLaunchdarklyFeatureFlag#defaults}
+        :param description: A short description of what the flag will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#description DataLaunchdarklyFeatureFlag#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#id DataLaunchdarklyFeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param include_in_snippet: Whether or not this flag should be made available to the client-side JavaScript SDK. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#include_in_snippet DataLaunchdarklyFeatureFlag#include_in_snippet}
+        :param maintainer_id: The LaunchDarkly id of the user who will maintain the flag. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#maintainer_id DataLaunchdarklyFeatureFlag#maintainer_id}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#tags DataLaunchdarklyFeatureFlag#tags}
+        :param temporary: Whether or not the flag is a temporary flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#temporary DataLaunchdarklyFeatureFlag#temporary}
+        :param variations: variations block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#variations DataLaunchdarklyFeatureFlag#variations}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -138,16 +138,16 @@
     def put_defaults(
         self,
         *,
         off_variation: jsii.Number,
         on_variation: jsii.Number,
     ) -> None:
         '''
-        :param off_variation: The index of the variation served when the flag is off for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#off_variation DataLaunchdarklyFeatureFlag#off_variation}
-        :param on_variation: The index of the variation served when the flag is on for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#on_variation DataLaunchdarklyFeatureFlag#on_variation}
+        :param off_variation: The index of the variation served when the flag is off for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#off_variation DataLaunchdarklyFeatureFlag#off_variation}
+        :param on_variation: The index of the variation served when the flag is on for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#on_variation DataLaunchdarklyFeatureFlag#on_variation}
         '''
         value = DataLaunchdarklyFeatureFlagDefaults(
             off_variation=off_variation, on_variation=on_variation
         )
 
         return typing.cast(None, jsii.invoke(self, "putDefaults", [value]))
 
@@ -458,16 +458,16 @@
     def __init__(
         self,
         *,
         using_environment_id: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         using_mobile_key: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     ) -> None:
         '''
-        :param using_environment_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#using_environment_id DataLaunchdarklyFeatureFlag#using_environment_id}.
-        :param using_mobile_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#using_mobile_key DataLaunchdarklyFeatureFlag#using_mobile_key}.
+        :param using_environment_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#using_environment_id DataLaunchdarklyFeatureFlag#using_environment_id}.
+        :param using_mobile_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#using_mobile_key DataLaunchdarklyFeatureFlag#using_mobile_key}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__21cd26f7fc51c38849f49fa9d1746fab0fea8c58ff001a7d341289b26dfb2d41)
             check_type(argname="argument using_environment_id", value=using_environment_id, expected_type=type_hints["using_environment_id"])
             check_type(argname="argument using_mobile_key", value=using_mobile_key, expected_type=type_hints["using_mobile_key"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if using_environment_id is not None:
@@ -475,23 +475,23 @@
         if using_mobile_key is not None:
             self._values["using_mobile_key"] = using_mobile_key
 
     @builtins.property
     def using_environment_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#using_environment_id DataLaunchdarklyFeatureFlag#using_environment_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#using_environment_id DataLaunchdarklyFeatureFlag#using_environment_id}.'''
         result = self._values.get("using_environment_id")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def using_mobile_key(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#using_mobile_key DataLaunchdarklyFeatureFlag#using_mobile_key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#using_mobile_key DataLaunchdarklyFeatureFlag#using_mobile_key}.'''
         result = self._values.get("using_mobile_key")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -751,27 +751,27 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: A unique key that will be used to reference the flag in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#project_key DataLaunchdarklyFeatureFlag#project_key}
-        :param archived: Whether to archive the flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#archived DataLaunchdarklyFeatureFlag#archived}
-        :param client_side_availability: client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#client_side_availability DataLaunchdarklyFeatureFlag#client_side_availability}
-        :param custom_properties: custom_properties block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#custom_properties DataLaunchdarklyFeatureFlag#custom_properties}
-        :param defaults: defaults block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#defaults DataLaunchdarklyFeatureFlag#defaults}
-        :param description: A short description of what the flag will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#description DataLaunchdarklyFeatureFlag#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#id DataLaunchdarklyFeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param include_in_snippet: Whether or not this flag should be made available to the client-side JavaScript SDK. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#include_in_snippet DataLaunchdarklyFeatureFlag#include_in_snippet}
-        :param maintainer_id: The LaunchDarkly id of the user who will maintain the flag. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#maintainer_id DataLaunchdarklyFeatureFlag#maintainer_id}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#tags DataLaunchdarklyFeatureFlag#tags}
-        :param temporary: Whether or not the flag is a temporary flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#temporary DataLaunchdarklyFeatureFlag#temporary}
-        :param variations: variations block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#variations DataLaunchdarklyFeatureFlag#variations}
+        :param key: A unique key that will be used to reference the flag in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#project_key DataLaunchdarklyFeatureFlag#project_key}
+        :param archived: Whether to archive the flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#archived DataLaunchdarklyFeatureFlag#archived}
+        :param client_side_availability: client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#client_side_availability DataLaunchdarklyFeatureFlag#client_side_availability}
+        :param custom_properties: custom_properties block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#custom_properties DataLaunchdarklyFeatureFlag#custom_properties}
+        :param defaults: defaults block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#defaults DataLaunchdarklyFeatureFlag#defaults}
+        :param description: A short description of what the flag will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#description DataLaunchdarklyFeatureFlag#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#id DataLaunchdarklyFeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param include_in_snippet: Whether or not this flag should be made available to the client-side JavaScript SDK. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#include_in_snippet DataLaunchdarklyFeatureFlag#include_in_snippet}
+        :param maintainer_id: The LaunchDarkly id of the user who will maintain the flag. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#maintainer_id DataLaunchdarklyFeatureFlag#maintainer_id}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#tags DataLaunchdarklyFeatureFlag#tags}
+        :param temporary: Whether or not the flag is a temporary flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#temporary DataLaunchdarklyFeatureFlag#temporary}
+        :param variations: variations block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#variations DataLaunchdarklyFeatureFlag#variations}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(defaults, dict):
             defaults = DataLaunchdarklyFeatureFlagDefaults(**defaults)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__530b455bc63811ba078aa401a86b5e682619333c87f8c2405c03d404a47fc2b1)
@@ -900,140 +900,140 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''A unique key that will be used to reference the flag in your code.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The LaunchDarkly project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#project_key DataLaunchdarklyFeatureFlag#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#project_key DataLaunchdarklyFeatureFlag#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def archived(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether to archive the flag.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#archived DataLaunchdarklyFeatureFlag#archived}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#archived DataLaunchdarklyFeatureFlag#archived}
         '''
         result = self._values.get("archived")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def client_side_availability(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataLaunchdarklyFeatureFlagClientSideAvailability]]]:
         '''client_side_availability block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#client_side_availability DataLaunchdarklyFeatureFlag#client_side_availability}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#client_side_availability DataLaunchdarklyFeatureFlag#client_side_availability}
         '''
         result = self._values.get("client_side_availability")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataLaunchdarklyFeatureFlagClientSideAvailability]]], result)
 
     @builtins.property
     def custom_properties(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyFeatureFlagCustomProperties"]]]:
         '''custom_properties block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#custom_properties DataLaunchdarklyFeatureFlag#custom_properties}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#custom_properties DataLaunchdarklyFeatureFlag#custom_properties}
         '''
         result = self._values.get("custom_properties")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyFeatureFlagCustomProperties"]]], result)
 
     @builtins.property
     def defaults(self) -> typing.Optional["DataLaunchdarklyFeatureFlagDefaults"]:
         '''defaults block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#defaults DataLaunchdarklyFeatureFlag#defaults}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#defaults DataLaunchdarklyFeatureFlag#defaults}
         '''
         result = self._values.get("defaults")
         return typing.cast(typing.Optional["DataLaunchdarklyFeatureFlagDefaults"], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''A short description of what the flag will be used for.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#description DataLaunchdarklyFeatureFlag#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#description DataLaunchdarklyFeatureFlag#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#id DataLaunchdarklyFeatureFlag#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#id DataLaunchdarklyFeatureFlag#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def include_in_snippet(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not this flag should be made available to the client-side JavaScript SDK.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#include_in_snippet DataLaunchdarklyFeatureFlag#include_in_snippet}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#include_in_snippet DataLaunchdarklyFeatureFlag#include_in_snippet}
         '''
         result = self._values.get("include_in_snippet")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def maintainer_id(self) -> typing.Optional[builtins.str]:
         '''The LaunchDarkly id of the user who will maintain the flag.
 
         If not set, the API will automatically apply the member associated with your Terraform API key or the most recently set maintainer
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#maintainer_id DataLaunchdarklyFeatureFlag#maintainer_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#maintainer_id DataLaunchdarklyFeatureFlag#maintainer_id}
         '''
         result = self._values.get("maintainer_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#tags DataLaunchdarklyFeatureFlag#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#tags DataLaunchdarklyFeatureFlag#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def temporary(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not the flag is a temporary flag.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#temporary DataLaunchdarklyFeatureFlag#temporary}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#temporary DataLaunchdarklyFeatureFlag#temporary}
         '''
         result = self._values.get("temporary")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def variations(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyFeatureFlagVariations"]]]:
         '''variations block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#variations DataLaunchdarklyFeatureFlag#variations}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#variations DataLaunchdarklyFeatureFlag#variations}
         '''
         result = self._values.get("variations")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyFeatureFlagVariations"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1056,46 +1056,46 @@
         self,
         *,
         key: builtins.str,
         name: builtins.str,
         value: typing.Sequence[builtins.str],
     ) -> None:
         '''
-        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#name DataLaunchdarklyFeatureFlag#name}.
-        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#value DataLaunchdarklyFeatureFlag#value}.
+        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#name DataLaunchdarklyFeatureFlag#name}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#value DataLaunchdarklyFeatureFlag#value}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__42e42db02f544188671c0861f3beff790c418b9d8e73e20a305d630ecba5801c)
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "key": key,
             "name": name,
             "value": value,
         }
 
     @builtins.property
     def key(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#key DataLaunchdarklyFeatureFlag#key}.'''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#name DataLaunchdarklyFeatureFlag#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#name DataLaunchdarklyFeatureFlag#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def value(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#value DataLaunchdarklyFeatureFlag#value}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#value DataLaunchdarklyFeatureFlag#value}.'''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1305,41 +1305,41 @@
     def __init__(
         self,
         *,
         off_variation: jsii.Number,
         on_variation: jsii.Number,
     ) -> None:
         '''
-        :param off_variation: The index of the variation served when the flag is off for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#off_variation DataLaunchdarklyFeatureFlag#off_variation}
-        :param on_variation: The index of the variation served when the flag is on for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#on_variation DataLaunchdarklyFeatureFlag#on_variation}
+        :param off_variation: The index of the variation served when the flag is off for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#off_variation DataLaunchdarklyFeatureFlag#off_variation}
+        :param on_variation: The index of the variation served when the flag is on for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#on_variation DataLaunchdarklyFeatureFlag#on_variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4cbf815ad275e20880fdcfc26ad6fd4d1f34e3ab1be7f85c83f8301d748cfaf8)
             check_type(argname="argument off_variation", value=off_variation, expected_type=type_hints["off_variation"])
             check_type(argname="argument on_variation", value=on_variation, expected_type=type_hints["on_variation"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "off_variation": off_variation,
             "on_variation": on_variation,
         }
 
     @builtins.property
     def off_variation(self) -> jsii.Number:
         '''The index of the variation served when the flag is off for new environments.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#off_variation DataLaunchdarklyFeatureFlag#off_variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#off_variation DataLaunchdarklyFeatureFlag#off_variation}
         '''
         result = self._values.get("off_variation")
         assert result is not None, "Required property 'off_variation' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def on_variation(self) -> jsii.Number:
         '''The index of the variation served when the flag is on for new environments.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#on_variation DataLaunchdarklyFeatureFlag#on_variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#on_variation DataLaunchdarklyFeatureFlag#on_variation}
         '''
         result = self._values.get("on_variation")
         assert result is not None, "Required property 'on_variation' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1433,17 +1433,17 @@
         self,
         *,
         value: builtins.str,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param value: The value of the flag for this variation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#value DataLaunchdarklyFeatureFlag#value}
-        :param description: A description for the variation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#description DataLaunchdarklyFeatureFlag#description}
-        :param name: A name for the variation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#name DataLaunchdarklyFeatureFlag#name}
+        :param value: The value of the flag for this variation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#value DataLaunchdarklyFeatureFlag#value}
+        :param description: A description for the variation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#description DataLaunchdarklyFeatureFlag#description}
+        :param name: A name for the variation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#name DataLaunchdarklyFeatureFlag#name}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0eaafa5c7c7a2001b8907dba35797b6eb51ddd99d4e9963356a2b2f14541a8ca)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -1454,34 +1454,34 @@
         if name is not None:
             self._values["name"] = name
 
     @builtins.property
     def value(self) -> builtins.str:
         '''The value of the flag for this variation.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#value DataLaunchdarklyFeatureFlag#value}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#value DataLaunchdarklyFeatureFlag#value}
         '''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''A description for the variation.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#description DataLaunchdarklyFeatureFlag#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#description DataLaunchdarklyFeatureFlag#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''A name for the variation.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag#name DataLaunchdarklyFeatureFlag#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag#name DataLaunchdarklyFeatureFlag#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag_environment/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag_environment/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_feature_flag_environment`
 
-Refer to the Terraform Registory for docs: [`data_launchdarkly_feature_flag_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment).
+Refer to the Terraform Registory for docs: [`data_launchdarkly_feature_flag_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataLaunchdarklyFeatureFlagEnvironment(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyFeatureFlagEnvironment.DataLaunchdarklyFeatureFlagEnvironment",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment launchdarkly_feature_flag_environment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment launchdarkly_feature_flag_environment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         env_key: builtins.str,
@@ -48,29 +48,29 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment launchdarkly_feature_flag_environment} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment launchdarkly_feature_flag_environment} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#env_key DataLaunchdarklyFeatureFlagEnvironment#env_key}
-        :param flag_id: The global feature flag's unique id in the format ``<project_key>/<flag_key>``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#flag_id DataLaunchdarklyFeatureFlagEnvironment#flag_id}
-        :param context_targets: context_targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#context_targets DataLaunchdarklyFeatureFlagEnvironment#context_targets}
-        :param fallthrough: fallthrough block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#fallthrough DataLaunchdarklyFeatureFlagEnvironment#fallthrough}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#id DataLaunchdarklyFeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param off_variation: The index of the variation to serve if targeting is disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#off_variation DataLaunchdarklyFeatureFlagEnvironment#off_variation}
-        :param on: Whether targeting is enabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#on DataLaunchdarklyFeatureFlagEnvironment#on}
-        :param prerequisites: prerequisites block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#prerequisites DataLaunchdarklyFeatureFlagEnvironment#prerequisites}
-        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#rules DataLaunchdarklyFeatureFlagEnvironment#rules}
-        :param targets: targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#targets DataLaunchdarklyFeatureFlagEnvironment#targets}
-        :param track_events: Whether to send event data back to LaunchDarkly. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#track_events DataLaunchdarklyFeatureFlagEnvironment#track_events}
+        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#env_key DataLaunchdarklyFeatureFlagEnvironment#env_key}
+        :param flag_id: The global feature flag's unique id in the format ``<project_key>/<flag_key>``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#flag_id DataLaunchdarklyFeatureFlagEnvironment#flag_id}
+        :param context_targets: context_targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#context_targets DataLaunchdarklyFeatureFlagEnvironment#context_targets}
+        :param fallthrough: fallthrough block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#fallthrough DataLaunchdarklyFeatureFlagEnvironment#fallthrough}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#id DataLaunchdarklyFeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param off_variation: The index of the variation to serve if targeting is disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#off_variation DataLaunchdarklyFeatureFlagEnvironment#off_variation}
+        :param on: Whether targeting is enabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#on DataLaunchdarklyFeatureFlagEnvironment#on}
+        :param prerequisites: prerequisites block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#prerequisites DataLaunchdarklyFeatureFlagEnvironment#prerequisites}
+        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#rules DataLaunchdarklyFeatureFlagEnvironment#rules}
+        :param targets: targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#targets DataLaunchdarklyFeatureFlagEnvironment#targets}
+        :param track_events: Whether to send event data back to LaunchDarkly. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#track_events DataLaunchdarklyFeatureFlagEnvironment#track_events}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -121,18 +121,18 @@
         *,
         bucket_by: typing.Optional[builtins.str] = None,
         context_kind: typing.Optional[builtins.str] = None,
         rollout_weights: typing.Optional[typing.Sequence[jsii.Number]] = None,
         variation: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#bucket_by DataLaunchdarklyFeatureFlagEnvironment#bucket_by}
-        :param context_kind: The context kind associated with the specified rollout. This argument is only valid if rollout_weights is also specified. If omitted, defaults to 'user' Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#context_kind DataLaunchdarklyFeatureFlagEnvironment#context_kind}
-        :param rollout_weights: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#rollout_weights DataLaunchdarklyFeatureFlagEnvironment#rollout_weights}.
-        :param variation: The integer variation index to serve in case of fallthrough. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
+        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#bucket_by DataLaunchdarklyFeatureFlagEnvironment#bucket_by}
+        :param context_kind: The context kind associated with the specified rollout. This argument is only valid if rollout_weights is also specified. If omitted, defaults to 'user' Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#context_kind DataLaunchdarklyFeatureFlagEnvironment#context_kind}
+        :param rollout_weights: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#rollout_weights DataLaunchdarklyFeatureFlagEnvironment#rollout_weights}.
+        :param variation: The integer variation index to serve in case of fallthrough. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
         '''
         value = DataLaunchdarklyFeatureFlagEnvironmentFallthrough(
             bucket_by=bucket_by,
             context_kind=context_kind,
             rollout_weights=rollout_weights,
             variation=variation,
         )
@@ -455,25 +455,25 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#env_key DataLaunchdarklyFeatureFlagEnvironment#env_key}
-        :param flag_id: The global feature flag's unique id in the format ``<project_key>/<flag_key>``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#flag_id DataLaunchdarklyFeatureFlagEnvironment#flag_id}
-        :param context_targets: context_targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#context_targets DataLaunchdarklyFeatureFlagEnvironment#context_targets}
-        :param fallthrough: fallthrough block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#fallthrough DataLaunchdarklyFeatureFlagEnvironment#fallthrough}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#id DataLaunchdarklyFeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param off_variation: The index of the variation to serve if targeting is disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#off_variation DataLaunchdarklyFeatureFlagEnvironment#off_variation}
-        :param on: Whether targeting is enabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#on DataLaunchdarklyFeatureFlagEnvironment#on}
-        :param prerequisites: prerequisites block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#prerequisites DataLaunchdarklyFeatureFlagEnvironment#prerequisites}
-        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#rules DataLaunchdarklyFeatureFlagEnvironment#rules}
-        :param targets: targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#targets DataLaunchdarklyFeatureFlagEnvironment#targets}
-        :param track_events: Whether to send event data back to LaunchDarkly. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#track_events DataLaunchdarklyFeatureFlagEnvironment#track_events}
+        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#env_key DataLaunchdarklyFeatureFlagEnvironment#env_key}
+        :param flag_id: The global feature flag's unique id in the format ``<project_key>/<flag_key>``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#flag_id DataLaunchdarklyFeatureFlagEnvironment#flag_id}
+        :param context_targets: context_targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#context_targets DataLaunchdarklyFeatureFlagEnvironment#context_targets}
+        :param fallthrough: fallthrough block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#fallthrough DataLaunchdarklyFeatureFlagEnvironment#fallthrough}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#id DataLaunchdarklyFeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param off_variation: The index of the variation to serve if targeting is disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#off_variation DataLaunchdarklyFeatureFlagEnvironment#off_variation}
+        :param on: Whether targeting is enabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#on DataLaunchdarklyFeatureFlagEnvironment#on}
+        :param prerequisites: prerequisites block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#prerequisites DataLaunchdarklyFeatureFlagEnvironment#prerequisites}
+        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#rules DataLaunchdarklyFeatureFlagEnvironment#rules}
+        :param targets: targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#targets DataLaunchdarklyFeatureFlagEnvironment#targets}
+        :param track_events: Whether to send event data back to LaunchDarkly. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#track_events DataLaunchdarklyFeatureFlagEnvironment#track_events}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(fallthrough, dict):
             fallthrough = DataLaunchdarklyFeatureFlagEnvironmentFallthrough(**fallthrough)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3887b8a55bec50ce0052798f0dc17b208c0f50312a4ba4a1a14d0afb5a2ac31c)
@@ -596,122 +596,122 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def env_key(self) -> builtins.str:
         '''The LaunchDarkly environment key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#env_key DataLaunchdarklyFeatureFlagEnvironment#env_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#env_key DataLaunchdarklyFeatureFlagEnvironment#env_key}
         '''
         result = self._values.get("env_key")
         assert result is not None, "Required property 'env_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def flag_id(self) -> builtins.str:
         '''The global feature flag's unique id in the format ``<project_key>/<flag_key>``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#flag_id DataLaunchdarklyFeatureFlagEnvironment#flag_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#flag_id DataLaunchdarklyFeatureFlagEnvironment#flag_id}
         '''
         result = self._values.get("flag_id")
         assert result is not None, "Required property 'flag_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def context_targets(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyFeatureFlagEnvironmentContextTargets"]]]:
         '''context_targets block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#context_targets DataLaunchdarklyFeatureFlagEnvironment#context_targets}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#context_targets DataLaunchdarklyFeatureFlagEnvironment#context_targets}
         '''
         result = self._values.get("context_targets")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyFeatureFlagEnvironmentContextTargets"]]], result)
 
     @builtins.property
     def fallthrough(
         self,
     ) -> typing.Optional["DataLaunchdarklyFeatureFlagEnvironmentFallthrough"]:
         '''fallthrough block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#fallthrough DataLaunchdarklyFeatureFlagEnvironment#fallthrough}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#fallthrough DataLaunchdarklyFeatureFlagEnvironment#fallthrough}
         '''
         result = self._values.get("fallthrough")
         return typing.cast(typing.Optional["DataLaunchdarklyFeatureFlagEnvironmentFallthrough"], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#id DataLaunchdarklyFeatureFlagEnvironment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#id DataLaunchdarklyFeatureFlagEnvironment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def off_variation(self) -> typing.Optional[jsii.Number]:
         '''The index of the variation to serve if targeting is disabled.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#off_variation DataLaunchdarklyFeatureFlagEnvironment#off_variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#off_variation DataLaunchdarklyFeatureFlagEnvironment#off_variation}
         '''
         result = self._values.get("off_variation")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def on(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether targeting is enabled.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#on DataLaunchdarklyFeatureFlagEnvironment#on}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#on DataLaunchdarklyFeatureFlagEnvironment#on}
         '''
         result = self._values.get("on")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def prerequisites(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyFeatureFlagEnvironmentPrerequisites"]]]:
         '''prerequisites block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#prerequisites DataLaunchdarklyFeatureFlagEnvironment#prerequisites}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#prerequisites DataLaunchdarklyFeatureFlagEnvironment#prerequisites}
         '''
         result = self._values.get("prerequisites")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyFeatureFlagEnvironmentPrerequisites"]]], result)
 
     @builtins.property
     def rules(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyFeatureFlagEnvironmentRules"]]]:
         '''rules block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#rules DataLaunchdarklyFeatureFlagEnvironment#rules}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#rules DataLaunchdarklyFeatureFlagEnvironment#rules}
         '''
         result = self._values.get("rules")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyFeatureFlagEnvironmentRules"]]], result)
 
     @builtins.property
     def targets(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyFeatureFlagEnvironmentTargets"]]]:
         '''targets block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#targets DataLaunchdarklyFeatureFlagEnvironment#targets}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#targets DataLaunchdarklyFeatureFlagEnvironment#targets}
         '''
         result = self._values.get("targets")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyFeatureFlagEnvironmentTargets"]]], result)
 
     @builtins.property
     def track_events(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether to send event data back to LaunchDarkly.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#track_events DataLaunchdarklyFeatureFlagEnvironment#track_events}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#track_events DataLaunchdarklyFeatureFlagEnvironment#track_events}
         '''
         result = self._values.get("track_events")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -738,17 +738,17 @@
         self,
         *,
         context_kind: builtins.str,
         values: typing.Sequence[builtins.str],
         variation: jsii.Number,
     ) -> None:
         '''
-        :param context_kind: The context kind on which the flag should target in this environment. If the context_kind has not been previously specified at the project level, it will be automatically created on the project. User targets should be specified as targets attribute blocks. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#context_kind DataLaunchdarklyFeatureFlagEnvironment#context_kind}
-        :param values: List of user strings to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#values DataLaunchdarklyFeatureFlagEnvironment#values}
-        :param variation: Index of the variation to serve if a user_target is matched. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
+        :param context_kind: The context kind on which the flag should target in this environment. If the context_kind has not been previously specified at the project level, it will be automatically created on the project. User targets should be specified as targets attribute blocks. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#context_kind DataLaunchdarklyFeatureFlagEnvironment#context_kind}
+        :param values: List of user strings to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#values DataLaunchdarklyFeatureFlagEnvironment#values}
+        :param variation: Index of the variation to serve if a user_target is matched. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__99bd5d9c2e613d9db4ae3ca3493dfbc81dab0115207eff4272d188b6b6a50829)
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
             check_type(argname="argument variation", value=variation, expected_type=type_hints["variation"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -759,35 +759,35 @@
 
     @builtins.property
     def context_kind(self) -> builtins.str:
         '''The context kind on which the flag should target in this environment.
 
         If the context_kind has not been previously specified at the project level, it will be automatically created on the project. User targets should be specified as targets attribute blocks.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#context_kind DataLaunchdarklyFeatureFlagEnvironment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#context_kind DataLaunchdarklyFeatureFlagEnvironment#context_kind}
         '''
         result = self._values.get("context_kind")
         assert result is not None, "Required property 'context_kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''List of user strings to target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#values DataLaunchdarklyFeatureFlagEnvironment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#values DataLaunchdarklyFeatureFlagEnvironment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def variation(self) -> jsii.Number:
         '''Index of the variation to serve if a user_target is matched.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
         '''
         result = self._values.get("variation")
         assert result is not None, "Required property 'variation' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1005,18 +1005,18 @@
         *,
         bucket_by: typing.Optional[builtins.str] = None,
         context_kind: typing.Optional[builtins.str] = None,
         rollout_weights: typing.Optional[typing.Sequence[jsii.Number]] = None,
         variation: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#bucket_by DataLaunchdarklyFeatureFlagEnvironment#bucket_by}
-        :param context_kind: The context kind associated with the specified rollout. This argument is only valid if rollout_weights is also specified. If omitted, defaults to 'user' Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#context_kind DataLaunchdarklyFeatureFlagEnvironment#context_kind}
-        :param rollout_weights: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#rollout_weights DataLaunchdarklyFeatureFlagEnvironment#rollout_weights}.
-        :param variation: The integer variation index to serve in case of fallthrough. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
+        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#bucket_by DataLaunchdarklyFeatureFlagEnvironment#bucket_by}
+        :param context_kind: The context kind associated with the specified rollout. This argument is only valid if rollout_weights is also specified. If omitted, defaults to 'user' Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#context_kind DataLaunchdarklyFeatureFlagEnvironment#context_kind}
+        :param rollout_weights: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#rollout_weights DataLaunchdarklyFeatureFlagEnvironment#rollout_weights}.
+        :param variation: The integer variation index to serve in case of fallthrough. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5dd35911240626a0307f449f70c6ec7d35e046146500f2b7c3e36879d33ef46d)
             check_type(argname="argument bucket_by", value=bucket_by, expected_type=type_hints["bucket_by"])
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
             check_type(argname="argument rollout_weights", value=rollout_weights, expected_type=type_hints["rollout_weights"])
             check_type(argname="argument variation", value=variation, expected_type=type_hints["variation"])
@@ -1030,41 +1030,41 @@
         if variation is not None:
             self._values["variation"] = variation
 
     @builtins.property
     def bucket_by(self) -> typing.Optional[builtins.str]:
         '''Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#bucket_by DataLaunchdarklyFeatureFlagEnvironment#bucket_by}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#bucket_by DataLaunchdarklyFeatureFlagEnvironment#bucket_by}
         '''
         result = self._values.get("bucket_by")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def context_kind(self) -> typing.Optional[builtins.str]:
         '''The context kind associated with the specified rollout.
 
         This argument is only valid if rollout_weights is also specified. If omitted, defaults to 'user'
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#context_kind DataLaunchdarklyFeatureFlagEnvironment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#context_kind DataLaunchdarklyFeatureFlagEnvironment#context_kind}
         '''
         result = self._values.get("context_kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def rollout_weights(self) -> typing.Optional[typing.List[jsii.Number]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#rollout_weights DataLaunchdarklyFeatureFlagEnvironment#rollout_weights}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#rollout_weights DataLaunchdarklyFeatureFlagEnvironment#rollout_weights}.'''
         result = self._values.get("rollout_weights")
         return typing.cast(typing.Optional[typing.List[jsii.Number]], result)
 
     @builtins.property
     def variation(self) -> typing.Optional[jsii.Number]:
         '''The integer variation index to serve in case of fallthrough.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
         '''
         result = self._values.get("variation")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1203,41 +1203,41 @@
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyFeatureFlagEnvironment.DataLaunchdarklyFeatureFlagEnvironmentPrerequisites",
     jsii_struct_bases=[],
     name_mapping={"flag_key": "flagKey", "variation": "variation"},
 )
 class DataLaunchdarklyFeatureFlagEnvironmentPrerequisites:
     def __init__(self, *, flag_key: builtins.str, variation: jsii.Number) -> None:
         '''
-        :param flag_key: The prerequisite feature flag's key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#flag_key DataLaunchdarklyFeatureFlagEnvironment#flag_key}
-        :param variation: The index of the prerequisite feature flag's variation to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
+        :param flag_key: The prerequisite feature flag's key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#flag_key DataLaunchdarklyFeatureFlagEnvironment#flag_key}
+        :param variation: The index of the prerequisite feature flag's variation to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c67bd97fe0637405ab67046c763cd52428047d5bb6d1fd751672379fd4161e02)
             check_type(argname="argument flag_key", value=flag_key, expected_type=type_hints["flag_key"])
             check_type(argname="argument variation", value=variation, expected_type=type_hints["variation"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "flag_key": flag_key,
             "variation": variation,
         }
 
     @builtins.property
     def flag_key(self) -> builtins.str:
         '''The prerequisite feature flag's key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#flag_key DataLaunchdarklyFeatureFlagEnvironment#flag_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#flag_key DataLaunchdarklyFeatureFlagEnvironment#flag_key}
         '''
         result = self._values.get("flag_key")
         assert result is not None, "Required property 'flag_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def variation(self) -> jsii.Number:
         '''The index of the prerequisite feature flag's variation to target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
         '''
         result = self._values.get("variation")
         assert result is not None, "Required property 'variation' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1440,19 +1440,19 @@
         bucket_by: typing.Optional[builtins.str] = None,
         clauses: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataLaunchdarklyFeatureFlagEnvironmentRulesClauses", typing.Dict[builtins.str, typing.Any]]]]] = None,
         description: typing.Optional[builtins.str] = None,
         rollout_weights: typing.Optional[typing.Sequence[jsii.Number]] = None,
         variation: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#bucket_by DataLaunchdarklyFeatureFlagEnvironment#bucket_by}
-        :param clauses: clauses block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#clauses DataLaunchdarklyFeatureFlagEnvironment#clauses}
-        :param description: A human-readable description of the targeting rule. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#description DataLaunchdarklyFeatureFlagEnvironment#description}
-        :param rollout_weights: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#rollout_weights DataLaunchdarklyFeatureFlagEnvironment#rollout_weights}.
-        :param variation: The integer variation index to serve if the rule clauses evaluate to true. This argument is only valid if clauses are also specified Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
+        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#bucket_by DataLaunchdarklyFeatureFlagEnvironment#bucket_by}
+        :param clauses: clauses block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#clauses DataLaunchdarklyFeatureFlagEnvironment#clauses}
+        :param description: A human-readable description of the targeting rule. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#description DataLaunchdarklyFeatureFlagEnvironment#description}
+        :param rollout_weights: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#rollout_weights DataLaunchdarklyFeatureFlagEnvironment#rollout_weights}.
+        :param variation: The integer variation index to serve if the rule clauses evaluate to true. This argument is only valid if clauses are also specified Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__707b0657af96d6231b89013d858f53a155af294cc4d7dd98b453c24a68e2344a)
             check_type(argname="argument bucket_by", value=bucket_by, expected_type=type_hints["bucket_by"])
             check_type(argname="argument clauses", value=clauses, expected_type=type_hints["clauses"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument rollout_weights", value=rollout_weights, expected_type=type_hints["rollout_weights"])
@@ -1469,52 +1469,52 @@
         if variation is not None:
             self._values["variation"] = variation
 
     @builtins.property
     def bucket_by(self) -> typing.Optional[builtins.str]:
         '''Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#bucket_by DataLaunchdarklyFeatureFlagEnvironment#bucket_by}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#bucket_by DataLaunchdarklyFeatureFlagEnvironment#bucket_by}
         '''
         result = self._values.get("bucket_by")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def clauses(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyFeatureFlagEnvironmentRulesClauses"]]]:
         '''clauses block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#clauses DataLaunchdarklyFeatureFlagEnvironment#clauses}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#clauses DataLaunchdarklyFeatureFlagEnvironment#clauses}
         '''
         result = self._values.get("clauses")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyFeatureFlagEnvironmentRulesClauses"]]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''A human-readable description of the targeting rule.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#description DataLaunchdarklyFeatureFlagEnvironment#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#description DataLaunchdarklyFeatureFlagEnvironment#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def rollout_weights(self) -> typing.Optional[typing.List[jsii.Number]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#rollout_weights DataLaunchdarklyFeatureFlagEnvironment#rollout_weights}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#rollout_weights DataLaunchdarklyFeatureFlagEnvironment#rollout_weights}.'''
         result = self._values.get("rollout_weights")
         return typing.cast(typing.Optional[typing.List[jsii.Number]], result)
 
     @builtins.property
     def variation(self) -> typing.Optional[jsii.Number]:
         '''The integer variation index to serve if the rule clauses evaluate to true.
 
         This argument is only valid if clauses are also specified
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
         '''
         result = self._values.get("variation")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1547,20 +1547,20 @@
         op: builtins.str,
         values: typing.Sequence[builtins.str],
         context_kind: typing.Optional[builtins.str] = None,
         negate: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         value_type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param attribute: The user attribute to operate on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#attribute DataLaunchdarklyFeatureFlagEnvironment#attribute}
-        :param op: The operator associated with the rule clause. Available options are in, endsWith, startsWith, matches, contains, lessThan, lessThanOrEqual, greaterThanOrEqual, before, after, segmentMatch, semVerEqual, semVerLessThan, and semVerGreaterThan Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#op DataLaunchdarklyFeatureFlagEnvironment#op}
-        :param values: The list of values associated with the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#values DataLaunchdarklyFeatureFlagEnvironment#values}
-        :param context_kind: The context kind associated with this rule clause. If omitted, defaults to user. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#context_kind DataLaunchdarklyFeatureFlagEnvironment#context_kind}
-        :param negate: Whether to negate the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#negate DataLaunchdarklyFeatureFlagEnvironment#negate}
-        :param value_type: The type for each of the clause's values. Available types are boolean, string, and number. If omitted, value_type defaults to string Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#value_type DataLaunchdarklyFeatureFlagEnvironment#value_type}
+        :param attribute: The user attribute to operate on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#attribute DataLaunchdarklyFeatureFlagEnvironment#attribute}
+        :param op: The operator associated with the rule clause. Available options are in, endsWith, startsWith, matches, contains, lessThan, lessThanOrEqual, greaterThanOrEqual, before, after, segmentMatch, semVerEqual, semVerLessThan, and semVerGreaterThan Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#op DataLaunchdarklyFeatureFlagEnvironment#op}
+        :param values: The list of values associated with the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#values DataLaunchdarklyFeatureFlagEnvironment#values}
+        :param context_kind: The context kind associated with this rule clause. If omitted, defaults to user. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#context_kind DataLaunchdarklyFeatureFlagEnvironment#context_kind}
+        :param negate: Whether to negate the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#negate DataLaunchdarklyFeatureFlagEnvironment#negate}
+        :param value_type: The type for each of the clause's values. Available types are boolean, string, and number. If omitted, value_type defaults to string Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#value_type DataLaunchdarklyFeatureFlagEnvironment#value_type}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3a9c6da1ea595f6b5beb74fd493993178a3f9066a7b4ae13cd29029ee7b53e01)
             check_type(argname="argument attribute", value=attribute, expected_type=type_hints["attribute"])
             check_type(argname="argument op", value=op, expected_type=type_hints["op"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
@@ -1578,69 +1578,69 @@
         if value_type is not None:
             self._values["value_type"] = value_type
 
     @builtins.property
     def attribute(self) -> builtins.str:
         '''The user attribute to operate on.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#attribute DataLaunchdarklyFeatureFlagEnvironment#attribute}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#attribute DataLaunchdarklyFeatureFlagEnvironment#attribute}
         '''
         result = self._values.get("attribute")
         assert result is not None, "Required property 'attribute' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def op(self) -> builtins.str:
         '''The operator associated with the rule clause.
 
         Available options are in, endsWith, startsWith, matches, contains, lessThan, lessThanOrEqual, greaterThanOrEqual, before, after, segmentMatch, semVerEqual, semVerLessThan, and semVerGreaterThan
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#op DataLaunchdarklyFeatureFlagEnvironment#op}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#op DataLaunchdarklyFeatureFlagEnvironment#op}
         '''
         result = self._values.get("op")
         assert result is not None, "Required property 'op' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''The list of values associated with the rule clause.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#values DataLaunchdarklyFeatureFlagEnvironment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#values DataLaunchdarklyFeatureFlagEnvironment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def context_kind(self) -> typing.Optional[builtins.str]:
         '''The context kind associated with this rule clause. If omitted, defaults to user.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#context_kind DataLaunchdarklyFeatureFlagEnvironment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#context_kind DataLaunchdarklyFeatureFlagEnvironment#context_kind}
         '''
         result = self._values.get("context_kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def negate(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether to negate the rule clause.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#negate DataLaunchdarklyFeatureFlagEnvironment#negate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#negate DataLaunchdarklyFeatureFlagEnvironment#negate}
         '''
         result = self._values.get("negate")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def value_type(self) -> typing.Optional[builtins.str]:
         '''The type for each of the clause's values.
 
         Available types are boolean, string, and number. If omitted, value_type defaults to string
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#value_type DataLaunchdarklyFeatureFlagEnvironment#value_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#value_type DataLaunchdarklyFeatureFlagEnvironment#value_type}
         '''
         result = self._values.get("value_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -2168,41 +2168,41 @@
     def __init__(
         self,
         *,
         values: typing.Sequence[builtins.str],
         variation: jsii.Number,
     ) -> None:
         '''
-        :param values: List of user strings to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#values DataLaunchdarklyFeatureFlagEnvironment#values}
-        :param variation: Index of the variation to serve if a user_target is matched. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
+        :param values: List of user strings to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#values DataLaunchdarklyFeatureFlagEnvironment#values}
+        :param variation: Index of the variation to serve if a user_target is matched. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1aba7a0b86e349809185aeca650c0e7f1023822ec9638134c6bb285922e641a7)
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
             check_type(argname="argument variation", value=variation, expected_type=type_hints["variation"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "values": values,
             "variation": variation,
         }
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''List of user strings to target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#values DataLaunchdarklyFeatureFlagEnvironment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#values DataLaunchdarklyFeatureFlagEnvironment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def variation(self) -> jsii.Number:
         '''Index of the variation to serve if a user_target is matched.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/feature_flag_environment#variation DataLaunchdarklyFeatureFlagEnvironment#variation}
         '''
         result = self._values.get("variation")
         assert result is not None, "Required property 'variation' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_flag_trigger/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_flag_trigger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_flag_trigger`
 
-Refer to the Terraform Registory for docs: [`data_launchdarkly_flag_trigger`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger).
+Refer to the Terraform Registory for docs: [`data_launchdarkly_flag_trigger`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataLaunchdarklyFlagTrigger(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyFlagTrigger.DataLaunchdarklyFlagTrigger",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger launchdarkly_flag_trigger}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger launchdarkly_flag_trigger}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         env_key: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger launchdarkly_flag_trigger} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger launchdarkly_flag_trigger} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#env_key DataLaunchdarklyFlagTrigger#env_key}
-        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#flag_key DataLaunchdarklyFlagTrigger#flag_key}
-        :param id: The flag trigger resource ID. This can be found on your trigger URL - please see docs for more info Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#id DataLaunchdarklyFlagTrigger#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#project_key DataLaunchdarklyFlagTrigger#project_key}
-        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#enabled DataLaunchdarklyFlagTrigger#enabled}
-        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#instructions DataLaunchdarklyFlagTrigger#instructions}
-        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#integration_key DataLaunchdarklyFlagTrigger#integration_key}
+        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#env_key DataLaunchdarklyFlagTrigger#env_key}
+        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#flag_key DataLaunchdarklyFlagTrigger#flag_key}
+        :param id: The flag trigger resource ID. This can be found on your trigger URL - please see docs for more info Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#id DataLaunchdarklyFlagTrigger#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#project_key DataLaunchdarklyFlagTrigger#project_key}
+        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#enabled DataLaunchdarklyFlagTrigger#enabled}
+        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#instructions DataLaunchdarklyFlagTrigger#instructions}
+        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#integration_key DataLaunchdarklyFlagTrigger#integration_key}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -89,15 +89,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putInstructions")
     def put_instructions(self, *, kind: builtins.str) -> None:
         '''
-        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#kind DataLaunchdarklyFlagTrigger#kind}
+        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#kind DataLaunchdarklyFlagTrigger#kind}
         '''
         value = DataLaunchdarklyFlagTriggerInstructions(kind=kind)
 
         return typing.cast(None, jsii.invoke(self, "putInstructions", [value]))
 
     @jsii.member(jsii_name="resetEnabled")
     def reset_enabled(self) -> None:
@@ -293,21 +293,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#env_key DataLaunchdarklyFlagTrigger#env_key}
-        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#flag_key DataLaunchdarklyFlagTrigger#flag_key}
-        :param id: The flag trigger resource ID. This can be found on your trigger URL - please see docs for more info Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#id DataLaunchdarklyFlagTrigger#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#project_key DataLaunchdarklyFlagTrigger#project_key}
-        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#enabled DataLaunchdarklyFlagTrigger#enabled}
-        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#instructions DataLaunchdarklyFlagTrigger#instructions}
-        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#integration_key DataLaunchdarklyFlagTrigger#integration_key}
+        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#env_key DataLaunchdarklyFlagTrigger#env_key}
+        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#flag_key DataLaunchdarklyFlagTrigger#flag_key}
+        :param id: The flag trigger resource ID. This can be found on your trigger URL - please see docs for more info Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#id DataLaunchdarklyFlagTrigger#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#project_key DataLaunchdarklyFlagTrigger#project_key}
+        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#enabled DataLaunchdarklyFlagTrigger#enabled}
+        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#instructions DataLaunchdarklyFlagTrigger#instructions}
+        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#integration_key DataLaunchdarklyFlagTrigger#integration_key}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(instructions, dict):
             instructions = DataLaunchdarklyFlagTriggerInstructions(**instructions)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5035f89f2d6f39b0055a9fa8c745d6fd8d07edb45d3058407584bfb25fc0ac54)
@@ -416,84 +416,84 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def env_key(self) -> builtins.str:
         '''The LaunchDarkly environment key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#env_key DataLaunchdarklyFlagTrigger#env_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#env_key DataLaunchdarklyFlagTrigger#env_key}
         '''
         result = self._values.get("env_key")
         assert result is not None, "Required property 'env_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def flag_key(self) -> builtins.str:
         '''The key of the feature flag the trigger acts upon.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#flag_key DataLaunchdarklyFlagTrigger#flag_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#flag_key DataLaunchdarklyFlagTrigger#flag_key}
         '''
         result = self._values.get("flag_key")
         assert result is not None, "Required property 'flag_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> builtins.str:
         '''The flag trigger resource ID.
 
         This can be found on your trigger URL - please see docs for more info
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#id DataLaunchdarklyFlagTrigger#id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#id DataLaunchdarklyFlagTrigger#id}
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         assert result is not None, "Required property 'id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The LaunchDarkly project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#project_key DataLaunchdarklyFlagTrigger#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#project_key DataLaunchdarklyFlagTrigger#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether the trigger is currently active or not. This property defaults to true upon creation.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#enabled DataLaunchdarklyFlagTrigger#enabled}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#enabled DataLaunchdarklyFlagTrigger#enabled}
         '''
         result = self._values.get("enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def instructions(
         self,
     ) -> typing.Optional["DataLaunchdarklyFlagTriggerInstructions"]:
         '''instructions block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#instructions DataLaunchdarklyFlagTrigger#instructions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#instructions DataLaunchdarklyFlagTrigger#instructions}
         '''
         result = self._values.get("instructions")
         return typing.cast(typing.Optional["DataLaunchdarklyFlagTriggerInstructions"], result)
 
     @builtins.property
     def integration_key(self) -> typing.Optional[builtins.str]:
         '''The unique identifier of the integration you intend to set your trigger up with.
 
         "generic-trigger" should be used for integrations not explicitly supported.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#integration_key DataLaunchdarklyFlagTrigger#integration_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#integration_key DataLaunchdarklyFlagTrigger#integration_key}
         '''
         result = self._values.get("integration_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -510,28 +510,28 @@
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyFlagTrigger.DataLaunchdarklyFlagTriggerInstructions",
     jsii_struct_bases=[],
     name_mapping={"kind": "kind"},
 )
 class DataLaunchdarklyFlagTriggerInstructions:
     def __init__(self, *, kind: builtins.str) -> None:
         '''
-        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#kind DataLaunchdarklyFlagTrigger#kind}
+        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#kind DataLaunchdarklyFlagTrigger#kind}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__427f08c549989595caa6db049131fa89e8c1d630b31e68b677cbd3f1109dce0d)
             check_type(argname="argument kind", value=kind, expected_type=type_hints["kind"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "kind": kind,
         }
 
     @builtins.property
     def kind(self) -> builtins.str:
         '''The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff".
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/flag_trigger#kind DataLaunchdarklyFlagTrigger#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/flag_trigger#kind DataLaunchdarklyFlagTrigger#kind}
         '''
         result = self._values.get("kind")
         assert result is not None, "Required property 'kind' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_metric/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_metric/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_metric`
 
-Refer to the Terraform Registory for docs: [`data_launchdarkly_metric`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric).
+Refer to the Terraform Registory for docs: [`data_launchdarkly_metric`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataLaunchdarklyMetric(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyMetric.DataLaunchdarklyMetric",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric launchdarkly_metric}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric launchdarkly_metric}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -53,34 +53,34 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric launchdarkly_metric} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric launchdarkly_metric} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#key DataLaunchdarklyMetric#key}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#project_key DataLaunchdarklyMetric#project_key}
-        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#description DataLaunchdarklyMetric#description}
-        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#event_key DataLaunchdarklyMetric#event_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#id DataLaunchdarklyMetric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#is_active DataLaunchdarklyMetric#is_active}
-        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#is_numeric DataLaunchdarklyMetric#is_numeric}
-        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
-        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#maintainer_id DataLaunchdarklyMetric#maintainer_id}
-        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#name DataLaunchdarklyMetric#name}
-        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#randomization_units DataLaunchdarklyMetric#randomization_units}
-        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#selector DataLaunchdarklyMetric#selector}
-        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#success_criteria DataLaunchdarklyMetric#success_criteria}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#tags DataLaunchdarklyMetric#tags}
-        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#unit DataLaunchdarklyMetric#unit}
-        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#urls DataLaunchdarklyMetric#urls}
+        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#key DataLaunchdarklyMetric#key}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#project_key DataLaunchdarklyMetric#project_key}
+        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#description DataLaunchdarklyMetric#description}
+        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#event_key DataLaunchdarklyMetric#event_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#id DataLaunchdarklyMetric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#is_active DataLaunchdarklyMetric#is_active}
+        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#is_numeric DataLaunchdarklyMetric#is_numeric}
+        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
+        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#maintainer_id DataLaunchdarklyMetric#maintainer_id}
+        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#name DataLaunchdarklyMetric#name}
+        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#randomization_units DataLaunchdarklyMetric#randomization_units}
+        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#selector DataLaunchdarklyMetric#selector}
+        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#success_criteria DataLaunchdarklyMetric#success_criteria}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#tags DataLaunchdarklyMetric#tags}
+        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#unit DataLaunchdarklyMetric#unit}
+        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#urls DataLaunchdarklyMetric#urls}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -534,30 +534,30 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#key DataLaunchdarklyMetric#key}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#project_key DataLaunchdarklyMetric#project_key}
-        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#description DataLaunchdarklyMetric#description}
-        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#event_key DataLaunchdarklyMetric#event_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#id DataLaunchdarklyMetric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#is_active DataLaunchdarklyMetric#is_active}
-        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#is_numeric DataLaunchdarklyMetric#is_numeric}
-        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
-        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#maintainer_id DataLaunchdarklyMetric#maintainer_id}
-        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#name DataLaunchdarklyMetric#name}
-        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#randomization_units DataLaunchdarklyMetric#randomization_units}
-        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#selector DataLaunchdarklyMetric#selector}
-        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#success_criteria DataLaunchdarklyMetric#success_criteria}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#tags DataLaunchdarklyMetric#tags}
-        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#unit DataLaunchdarklyMetric#unit}
-        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#urls DataLaunchdarklyMetric#urls}
+        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#key DataLaunchdarklyMetric#key}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#project_key DataLaunchdarklyMetric#project_key}
+        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#description DataLaunchdarklyMetric#description}
+        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#event_key DataLaunchdarklyMetric#event_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#id DataLaunchdarklyMetric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#is_active DataLaunchdarklyMetric#is_active}
+        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#is_numeric DataLaunchdarklyMetric#is_numeric}
+        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
+        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#maintainer_id DataLaunchdarklyMetric#maintainer_id}
+        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#name DataLaunchdarklyMetric#name}
+        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#randomization_units DataLaunchdarklyMetric#randomization_units}
+        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#selector DataLaunchdarklyMetric#selector}
+        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#success_criteria DataLaunchdarklyMetric#success_criteria}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#tags DataLaunchdarklyMetric#tags}
+        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#unit DataLaunchdarklyMetric#unit}
+        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#urls DataLaunchdarklyMetric#urls}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c4e7dd175594ceed19a99d810c24f0f6258ee9cd02779a36f8dc3326a139dca9)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -693,161 +693,161 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''A unique key that will be used to reference the metric in your code.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#key DataLaunchdarklyMetric#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#key DataLaunchdarklyMetric#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The LaunchDarkly project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#project_key DataLaunchdarklyMetric#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#project_key DataLaunchdarklyMetric#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''A short description of what the metric will be used for.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#description DataLaunchdarklyMetric#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#description DataLaunchdarklyMetric#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def event_key(self) -> typing.Optional[builtins.str]:
         '''The event key for your metric (if custom metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#event_key DataLaunchdarklyMetric#event_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#event_key DataLaunchdarklyMetric#event_key}
         '''
         result = self._values.get("event_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#id DataLaunchdarklyMetric#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#id DataLaunchdarklyMetric#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def is_active(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether the metric is active.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#is_active DataLaunchdarklyMetric#is_active}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#is_active DataLaunchdarklyMetric#is_active}
         '''
         result = self._values.get("is_active")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def is_numeric(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether the metric is numeric.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#is_numeric DataLaunchdarklyMetric#is_numeric}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#is_numeric DataLaunchdarklyMetric#is_numeric}
         '''
         result = self._values.get("is_numeric")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def kind(self) -> typing.Optional[builtins.str]:
         '''The metric type -available choices are 'pageview', 'click', and 'custom'.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
         '''
         result = self._values.get("kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def maintainer_id(self) -> typing.Optional[builtins.str]:
         '''The LaunchDarkly ID of the user who will maintain the metric.
 
         If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#maintainer_id DataLaunchdarklyMetric#maintainer_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#maintainer_id DataLaunchdarklyMetric#maintainer_id}
         '''
         result = self._values.get("maintainer_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''A human-readable name for your metric.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#name DataLaunchdarklyMetric#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#name DataLaunchdarklyMetric#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def randomization_units(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A set of one or more context kinds that this metric can measure events from.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#randomization_units DataLaunchdarklyMetric#randomization_units}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#randomization_units DataLaunchdarklyMetric#randomization_units}
         '''
         result = self._values.get("randomization_units")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def selector(self) -> typing.Optional[builtins.str]:
         '''The CSS selector for your metric (if click metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#selector DataLaunchdarklyMetric#selector}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#selector DataLaunchdarklyMetric#selector}
         '''
         result = self._values.get("selector")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def success_criteria(self) -> typing.Optional[builtins.str]:
         '''The success criteria for your metric (if numeric metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#success_criteria DataLaunchdarklyMetric#success_criteria}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#success_criteria DataLaunchdarklyMetric#success_criteria}
         '''
         result = self._values.get("success_criteria")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#tags DataLaunchdarklyMetric#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#tags DataLaunchdarklyMetric#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def unit(self) -> typing.Optional[builtins.str]:
         '''The unit for your metric (if numeric metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#unit DataLaunchdarklyMetric#unit}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#unit DataLaunchdarklyMetric#unit}
         '''
         result = self._values.get("unit")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def urls(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyMetricUrls"]]]:
         '''urls block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#urls DataLaunchdarklyMetric#urls}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#urls DataLaunchdarklyMetric#urls}
         '''
         result = self._values.get("urls")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyMetricUrls"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -876,18 +876,18 @@
         *,
         kind: builtins.str,
         pattern: typing.Optional[builtins.str] = None,
         substring: typing.Optional[builtins.str] = None,
         url: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param kind: The url type - available choices are 'exact', 'canonical', 'substring' and 'regex'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
-        :param pattern: The URL-matching regex. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#pattern DataLaunchdarklyMetric#pattern}
-        :param substring: The URL substring. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#substring DataLaunchdarklyMetric#substring}
-        :param url: The exact or canonical URL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#url DataLaunchdarklyMetric#url}
+        :param kind: The url type - available choices are 'exact', 'canonical', 'substring' and 'regex'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
+        :param pattern: The URL-matching regex. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#pattern DataLaunchdarklyMetric#pattern}
+        :param substring: The URL substring. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#substring DataLaunchdarklyMetric#substring}
+        :param url: The exact or canonical URL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#url DataLaunchdarklyMetric#url}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c17be6f52ff7b594d336bd7722da74adc4c2ebbae3659610d20c305cddd8aa1e)
             check_type(argname="argument kind", value=kind, expected_type=type_hints["kind"])
             check_type(argname="argument pattern", value=pattern, expected_type=type_hints["pattern"])
             check_type(argname="argument substring", value=substring, expected_type=type_hints["substring"])
             check_type(argname="argument url", value=url, expected_type=type_hints["url"])
@@ -901,43 +901,43 @@
         if url is not None:
             self._values["url"] = url
 
     @builtins.property
     def kind(self) -> builtins.str:
         '''The url type - available choices are 'exact', 'canonical', 'substring' and 'regex'.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#kind DataLaunchdarklyMetric#kind}
         '''
         result = self._values.get("kind")
         assert result is not None, "Required property 'kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def pattern(self) -> typing.Optional[builtins.str]:
         '''The URL-matching regex.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#pattern DataLaunchdarklyMetric#pattern}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#pattern DataLaunchdarklyMetric#pattern}
         '''
         result = self._values.get("pattern")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def substring(self) -> typing.Optional[builtins.str]:
         '''The URL substring.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#substring DataLaunchdarklyMetric#substring}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#substring DataLaunchdarklyMetric#substring}
         '''
         result = self._values.get("substring")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def url(self) -> typing.Optional[builtins.str]:
         '''The exact or canonical URL.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/metric#url DataLaunchdarklyMetric#url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/metric#url DataLaunchdarklyMetric#url}
         '''
         result = self._values.get("url")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_project/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_project/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_project`
 
-Refer to the Terraform Registory for docs: [`data_launchdarkly_project`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/project).
+Refer to the Terraform Registory for docs: [`data_launchdarkly_project`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/project).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataLaunchdarklyProject(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyProject.DataLaunchdarklyProject",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/project launchdarkly_project}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/project launchdarkly_project}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/project launchdarkly_project} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/project launchdarkly_project} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/project#key DataLaunchdarklyProject#key}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/project#id DataLaunchdarklyProject#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/project#tags DataLaunchdarklyProject#tags}
+        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/project#key DataLaunchdarklyProject#key}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/project#id DataLaunchdarklyProject#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/project#tags DataLaunchdarklyProject#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -352,17 +352,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/project#key DataLaunchdarklyProject#key}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/project#id DataLaunchdarklyProject#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/project#tags DataLaunchdarklyProject#tags}
+        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/project#key DataLaunchdarklyProject#key}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/project#id DataLaunchdarklyProject#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/project#tags DataLaunchdarklyProject#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f677daac99e59cdf82ec5988e548c38ce1342b3e3d28a5ff2fd218aba3a04e0d)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -458,34 +458,34 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/project#key DataLaunchdarklyProject#key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/project#key DataLaunchdarklyProject#key}.'''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/project#id DataLaunchdarklyProject#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/project#id DataLaunchdarklyProject#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/project#tags DataLaunchdarklyProject#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/project#tags DataLaunchdarklyProject#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_relay_proxy_configuration/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_relay_proxy_configuration/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_relay_proxy_configuration`
 
-Refer to the Terraform Registory for docs: [`data_launchdarkly_relay_proxy_configuration`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration).
+Refer to the Terraform Registory for docs: [`data_launchdarkly_relay_proxy_configuration`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataLaunchdarklyRelayProxyConfiguration(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyRelayProxyConfiguration.DataLaunchdarklyRelayProxyConfiguration",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration launchdarkly_relay_proxy_configuration}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration launchdarkly_relay_proxy_configuration}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: builtins.str,
@@ -39,20 +39,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration launchdarkly_relay_proxy_configuration} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration launchdarkly_relay_proxy_configuration} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: The Relay Proxy configuration's unique 24 character ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#id DataLaunchdarklyRelayProxyConfiguration#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#policy DataLaunchdarklyRelayProxyConfiguration#policy}
+        :param id: The Relay Proxy configuration's unique 24 character ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#id DataLaunchdarklyRelayProxyConfiguration#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#policy DataLaunchdarklyRelayProxyConfiguration#policy}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -176,16 +176,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: The Relay Proxy configuration's unique 24 character ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#id DataLaunchdarklyRelayProxyConfiguration#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#policy DataLaunchdarklyRelayProxyConfiguration#policy}
+        :param id: The Relay Proxy configuration's unique 24 character ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#id DataLaunchdarklyRelayProxyConfiguration#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#policy DataLaunchdarklyRelayProxyConfiguration#policy}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1583f398ed928478045304696977a511501bb413634c7326cb91b8d838efddcb)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -280,30 +280,30 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> builtins.str:
         '''The Relay Proxy configuration's unique 24 character ID.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#id DataLaunchdarklyRelayProxyConfiguration#id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#id DataLaunchdarklyRelayProxyConfiguration#id}
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         assert result is not None, "Required property 'id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def policy(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyRelayProxyConfigurationPolicy"]]]:
         '''policy block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#policy DataLaunchdarklyRelayProxyConfiguration#policy}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#policy DataLaunchdarklyRelayProxyConfiguration#policy}
         '''
         result = self._values.get("policy")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyRelayProxyConfigurationPolicy"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -334,19 +334,19 @@
         effect: builtins.str,
         actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
         resources: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#effect DataLaunchdarklyRelayProxyConfiguration#effect}.
-        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#actions DataLaunchdarklyRelayProxyConfiguration#actions}
-        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#not_actions DataLaunchdarklyRelayProxyConfiguration#not_actions}
-        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#not_resources DataLaunchdarklyRelayProxyConfiguration#not_resources}
-        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#resources DataLaunchdarklyRelayProxyConfiguration#resources}
+        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#effect DataLaunchdarklyRelayProxyConfiguration#effect}.
+        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#actions DataLaunchdarklyRelayProxyConfiguration#actions}
+        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#not_actions DataLaunchdarklyRelayProxyConfiguration#not_actions}
+        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#not_resources DataLaunchdarklyRelayProxyConfiguration#not_resources}
+        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#resources DataLaunchdarklyRelayProxyConfiguration#resources}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2635c70bf92d7811c20155c446d26984b5c659b621dcfc03c517b1eed4c8a5ef)
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument not_actions", value=not_actions, expected_type=type_hints["not_actions"])
             check_type(argname="argument not_resources", value=not_resources, expected_type=type_hints["not_resources"])
@@ -361,55 +361,55 @@
         if not_resources is not None:
             self._values["not_resources"] = not_resources
         if resources is not None:
             self._values["resources"] = resources
 
     @builtins.property
     def effect(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#effect DataLaunchdarklyRelayProxyConfiguration#effect}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#effect DataLaunchdarklyRelayProxyConfiguration#effect}.'''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''An action to perform on a resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#actions DataLaunchdarklyRelayProxyConfiguration#actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#actions DataLaunchdarklyRelayProxyConfiguration#actions}
         '''
         result = self._values.get("actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted actions will be those actions NOT in this list.
 
         The 'actions' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#not_actions DataLaunchdarklyRelayProxyConfiguration#not_actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#not_actions DataLaunchdarklyRelayProxyConfiguration#not_actions}
         '''
         result = self._values.get("not_actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted resources will be those resources NOT in this list.
 
         The 'resources' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#not_resources DataLaunchdarklyRelayProxyConfiguration#not_resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#not_resources DataLaunchdarklyRelayProxyConfiguration#not_resources}
         '''
         result = self._values.get("not_resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of LaunchDarkly resource specifiers.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/relay_proxy_configuration#resources DataLaunchdarklyRelayProxyConfiguration#resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/relay_proxy_configuration#resources DataLaunchdarklyRelayProxyConfiguration#resources}
         '''
         result = self._values.get("resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_segment/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_segment/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_segment`
 
-Refer to the Terraform Registory for docs: [`data_launchdarkly_segment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment).
+Refer to the Terraform Registory for docs: [`data_launchdarkly_segment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataLaunchdarklySegment(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklySegment.DataLaunchdarklySegment",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment launchdarkly_segment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment launchdarkly_segment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         env_key: builtins.str,
@@ -48,29 +48,29 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment launchdarkly_segment} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment launchdarkly_segment} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param env_key: The segment's environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#env_key DataLaunchdarklySegment#env_key}
-        :param key: The unique key that references the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#key DataLaunchdarklySegment#key}
-        :param project_key: The segment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#project_key DataLaunchdarklySegment#project_key}
-        :param description: The description of the segment's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#description DataLaunchdarklySegment#description}
-        :param excluded: List of user keys excluded from the segment. To target on other context kinds, use the excluded_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#excluded DataLaunchdarklySegment#excluded}
-        :param excluded_contexts: excluded_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#excluded_contexts DataLaunchdarklySegment#excluded_contexts}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#id DataLaunchdarklySegment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param included: List of user keys included in the segment. To target on other context kinds, use the included_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#included DataLaunchdarklySegment#included}
-        :param included_contexts: included_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#included_contexts DataLaunchdarklySegment#included_contexts}
-        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#rules DataLaunchdarklySegment#rules}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#tags DataLaunchdarklySegment#tags}
+        :param env_key: The segment's environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#env_key DataLaunchdarklySegment#env_key}
+        :param key: The unique key that references the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#key DataLaunchdarklySegment#key}
+        :param project_key: The segment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#project_key DataLaunchdarklySegment#project_key}
+        :param description: The description of the segment's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#description DataLaunchdarklySegment#description}
+        :param excluded: List of user keys excluded from the segment. To target on other context kinds, use the excluded_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#excluded DataLaunchdarklySegment#excluded}
+        :param excluded_contexts: excluded_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#excluded_contexts DataLaunchdarklySegment#excluded_contexts}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#id DataLaunchdarklySegment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param included: List of user keys included in the segment. To target on other context kinds, use the included_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#included DataLaunchdarklySegment#included}
+        :param included_contexts: included_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#included_contexts DataLaunchdarklySegment#included_contexts}
+        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#rules DataLaunchdarklySegment#rules}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#tags DataLaunchdarklySegment#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -416,25 +416,25 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param env_key: The segment's environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#env_key DataLaunchdarklySegment#env_key}
-        :param key: The unique key that references the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#key DataLaunchdarklySegment#key}
-        :param project_key: The segment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#project_key DataLaunchdarklySegment#project_key}
-        :param description: The description of the segment's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#description DataLaunchdarklySegment#description}
-        :param excluded: List of user keys excluded from the segment. To target on other context kinds, use the excluded_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#excluded DataLaunchdarklySegment#excluded}
-        :param excluded_contexts: excluded_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#excluded_contexts DataLaunchdarklySegment#excluded_contexts}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#id DataLaunchdarklySegment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param included: List of user keys included in the segment. To target on other context kinds, use the included_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#included DataLaunchdarklySegment#included}
-        :param included_contexts: included_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#included_contexts DataLaunchdarklySegment#included_contexts}
-        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#rules DataLaunchdarklySegment#rules}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#tags DataLaunchdarklySegment#tags}
+        :param env_key: The segment's environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#env_key DataLaunchdarklySegment#env_key}
+        :param key: The unique key that references the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#key DataLaunchdarklySegment#key}
+        :param project_key: The segment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#project_key DataLaunchdarklySegment#project_key}
+        :param description: The description of the segment's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#description DataLaunchdarklySegment#description}
+        :param excluded: List of user keys excluded from the segment. To target on other context kinds, use the excluded_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#excluded DataLaunchdarklySegment#excluded}
+        :param excluded_contexts: excluded_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#excluded_contexts DataLaunchdarklySegment#excluded_contexts}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#id DataLaunchdarklySegment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param included: List of user keys included in the segment. To target on other context kinds, use the included_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#included DataLaunchdarklySegment#included}
+        :param included_contexts: included_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#included_contexts DataLaunchdarklySegment#included_contexts}
+        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#rules DataLaunchdarklySegment#rules}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#tags DataLaunchdarklySegment#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4968e8cf106963aaca9d99652b60495322567d70543e75826303606d06a6f0ab)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -554,115 +554,115 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def env_key(self) -> builtins.str:
         '''The segment's environment key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#env_key DataLaunchdarklySegment#env_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#env_key DataLaunchdarklySegment#env_key}
         '''
         result = self._values.get("env_key")
         assert result is not None, "Required property 'env_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The unique key that references the segment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#key DataLaunchdarklySegment#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#key DataLaunchdarklySegment#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The segment's project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#project_key DataLaunchdarklySegment#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#project_key DataLaunchdarklySegment#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The description of the segment's purpose.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#description DataLaunchdarklySegment#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#description DataLaunchdarklySegment#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def excluded(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of user keys excluded from the segment. To target on other context kinds, use the excluded_contexts block attribute.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#excluded DataLaunchdarklySegment#excluded}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#excluded DataLaunchdarklySegment#excluded}
         '''
         result = self._values.get("excluded")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def excluded_contexts(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklySegmentExcludedContexts"]]]:
         '''excluded_contexts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#excluded_contexts DataLaunchdarklySegment#excluded_contexts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#excluded_contexts DataLaunchdarklySegment#excluded_contexts}
         '''
         result = self._values.get("excluded_contexts")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklySegmentExcludedContexts"]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#id DataLaunchdarklySegment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#id DataLaunchdarklySegment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def included(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of user keys included in the segment. To target on other context kinds, use the included_contexts block attribute.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#included DataLaunchdarklySegment#included}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#included DataLaunchdarklySegment#included}
         '''
         result = self._values.get("included")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def included_contexts(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklySegmentIncludedContexts"]]]:
         '''included_contexts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#included_contexts DataLaunchdarklySegment#included_contexts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#included_contexts DataLaunchdarklySegment#included_contexts}
         '''
         result = self._values.get("included_contexts")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklySegmentIncludedContexts"]]], result)
 
     @builtins.property
     def rules(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklySegmentRules"]]]:
         '''rules block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#rules DataLaunchdarklySegment#rules}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#rules DataLaunchdarklySegment#rules}
         '''
         result = self._values.get("rules")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklySegmentRules"]]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#tags DataLaunchdarklySegment#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#tags DataLaunchdarklySegment#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -684,41 +684,41 @@
     def __init__(
         self,
         *,
         context_kind: builtins.str,
         values: typing.Sequence[builtins.str],
     ) -> None:
         '''
-        :param context_kind: The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#context_kind DataLaunchdarklySegment#context_kind}
-        :param values: List of target object keys included in or excluded from the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#values DataLaunchdarklySegment#values}
+        :param context_kind: The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#context_kind DataLaunchdarklySegment#context_kind}
+        :param values: List of target object keys included in or excluded from the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#values DataLaunchdarklySegment#values}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__43895aa1918d204f8a9fa02178bd67bf98f115a50c784448a8ef3482177c0c94)
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "context_kind": context_kind,
             "values": values,
         }
 
     @builtins.property
     def context_kind(self) -> builtins.str:
         '''The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#context_kind DataLaunchdarklySegment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#context_kind DataLaunchdarklySegment#context_kind}
         '''
         result = self._values.get("context_kind")
         assert result is not None, "Required property 'context_kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''List of target object keys included in or excluded from the segment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#values DataLaunchdarklySegment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#values DataLaunchdarklySegment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -912,41 +912,41 @@
     def __init__(
         self,
         *,
         context_kind: builtins.str,
         values: typing.Sequence[builtins.str],
     ) -> None:
         '''
-        :param context_kind: The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#context_kind DataLaunchdarklySegment#context_kind}
-        :param values: List of target object keys included in or excluded from the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#values DataLaunchdarklySegment#values}
+        :param context_kind: The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#context_kind DataLaunchdarklySegment#context_kind}
+        :param values: List of target object keys included in or excluded from the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#values DataLaunchdarklySegment#values}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6209c8fae46aa3d0de8df79171086bdaed2add2b58568c64baf810fe770981f4)
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "context_kind": context_kind,
             "values": values,
         }
 
     @builtins.property
     def context_kind(self) -> builtins.str:
         '''The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#context_kind DataLaunchdarklySegment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#context_kind DataLaunchdarklySegment#context_kind}
         '''
         result = self._values.get("context_kind")
         assert result is not None, "Required property 'context_kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''List of target object keys included in or excluded from the segment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#values DataLaunchdarklySegment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#values DataLaunchdarklySegment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1147,18 +1147,18 @@
         *,
         bucket_by: typing.Optional[builtins.str] = None,
         clauses: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataLaunchdarklySegmentRulesClauses", typing.Dict[builtins.str, typing.Any]]]]] = None,
         rollout_context_kind: typing.Optional[builtins.str] = None,
         weight: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param bucket_by: The attribute by which to group users together. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#bucket_by DataLaunchdarklySegment#bucket_by}
-        :param clauses: clauses block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#clauses DataLaunchdarklySegment#clauses}
-        :param rollout_context_kind: The context kind associated with this segment rule. This argument is only valid if weight is also specified. If omitted, defaults to 'user' Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#rollout_context_kind DataLaunchdarklySegment#rollout_context_kind}
-        :param weight: The integer weight of the rule (between 1 and 100000). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#weight DataLaunchdarklySegment#weight}
+        :param bucket_by: The attribute by which to group users together. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#bucket_by DataLaunchdarklySegment#bucket_by}
+        :param clauses: clauses block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#clauses DataLaunchdarklySegment#clauses}
+        :param rollout_context_kind: The context kind associated with this segment rule. This argument is only valid if weight is also specified. If omitted, defaults to 'user' Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#rollout_context_kind DataLaunchdarklySegment#rollout_context_kind}
+        :param weight: The integer weight of the rule (between 1 and 100000). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#weight DataLaunchdarklySegment#weight}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__07f4f03d68b887f06222b642ffd079b9152f7d52848f03ead9ca6a86780556f7)
             check_type(argname="argument bucket_by", value=bucket_by, expected_type=type_hints["bucket_by"])
             check_type(argname="argument clauses", value=clauses, expected_type=type_hints["clauses"])
             check_type(argname="argument rollout_context_kind", value=rollout_context_kind, expected_type=type_hints["rollout_context_kind"])
             check_type(argname="argument weight", value=weight, expected_type=type_hints["weight"])
@@ -1172,46 +1172,46 @@
         if weight is not None:
             self._values["weight"] = weight
 
     @builtins.property
     def bucket_by(self) -> typing.Optional[builtins.str]:
         '''The attribute by which to group users together.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#bucket_by DataLaunchdarklySegment#bucket_by}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#bucket_by DataLaunchdarklySegment#bucket_by}
         '''
         result = self._values.get("bucket_by")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def clauses(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklySegmentRulesClauses"]]]:
         '''clauses block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#clauses DataLaunchdarklySegment#clauses}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#clauses DataLaunchdarklySegment#clauses}
         '''
         result = self._values.get("clauses")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklySegmentRulesClauses"]]], result)
 
     @builtins.property
     def rollout_context_kind(self) -> typing.Optional[builtins.str]:
         '''The context kind associated with this segment rule.
 
         This argument is only valid if weight is also specified. If omitted, defaults to 'user'
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#rollout_context_kind DataLaunchdarklySegment#rollout_context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#rollout_context_kind DataLaunchdarklySegment#rollout_context_kind}
         '''
         result = self._values.get("rollout_context_kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def weight(self) -> typing.Optional[jsii.Number]:
         '''The integer weight of the rule (between 1 and 100000).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#weight DataLaunchdarklySegment#weight}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#weight DataLaunchdarklySegment#weight}
         '''
         result = self._values.get("weight")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1244,20 +1244,20 @@
         op: builtins.str,
         values: typing.Sequence[builtins.str],
         context_kind: typing.Optional[builtins.str] = None,
         negate: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         value_type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param attribute: The user attribute to operate on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#attribute DataLaunchdarklySegment#attribute}
-        :param op: The operator associated with the rule clause. Available options are in, endsWith, startsWith, matches, contains, lessThan, lessThanOrEqual, greaterThanOrEqual, before, after, segmentMatch, semVerEqual, semVerLessThan, and semVerGreaterThan Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#op DataLaunchdarklySegment#op}
-        :param values: The list of values associated with the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#values DataLaunchdarklySegment#values}
-        :param context_kind: The context kind associated with this rule clause. If omitted, defaults to user. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#context_kind DataLaunchdarklySegment#context_kind}
-        :param negate: Whether to negate the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#negate DataLaunchdarklySegment#negate}
-        :param value_type: The type for each of the clause's values. Available types are boolean, string, and number. If omitted, value_type defaults to string Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#value_type DataLaunchdarklySegment#value_type}
+        :param attribute: The user attribute to operate on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#attribute DataLaunchdarklySegment#attribute}
+        :param op: The operator associated with the rule clause. Available options are in, endsWith, startsWith, matches, contains, lessThan, lessThanOrEqual, greaterThanOrEqual, before, after, segmentMatch, semVerEqual, semVerLessThan, and semVerGreaterThan Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#op DataLaunchdarklySegment#op}
+        :param values: The list of values associated with the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#values DataLaunchdarklySegment#values}
+        :param context_kind: The context kind associated with this rule clause. If omitted, defaults to user. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#context_kind DataLaunchdarklySegment#context_kind}
+        :param negate: Whether to negate the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#negate DataLaunchdarklySegment#negate}
+        :param value_type: The type for each of the clause's values. Available types are boolean, string, and number. If omitted, value_type defaults to string Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#value_type DataLaunchdarklySegment#value_type}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__779e2e4abca72771dd965b3afcebbcd0e575524822f4e39a990b1acf55258917)
             check_type(argname="argument attribute", value=attribute, expected_type=type_hints["attribute"])
             check_type(argname="argument op", value=op, expected_type=type_hints["op"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
@@ -1275,69 +1275,69 @@
         if value_type is not None:
             self._values["value_type"] = value_type
 
     @builtins.property
     def attribute(self) -> builtins.str:
         '''The user attribute to operate on.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#attribute DataLaunchdarklySegment#attribute}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#attribute DataLaunchdarklySegment#attribute}
         '''
         result = self._values.get("attribute")
         assert result is not None, "Required property 'attribute' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def op(self) -> builtins.str:
         '''The operator associated with the rule clause.
 
         Available options are in, endsWith, startsWith, matches, contains, lessThan, lessThanOrEqual, greaterThanOrEqual, before, after, segmentMatch, semVerEqual, semVerLessThan, and semVerGreaterThan
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#op DataLaunchdarklySegment#op}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#op DataLaunchdarklySegment#op}
         '''
         result = self._values.get("op")
         assert result is not None, "Required property 'op' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''The list of values associated with the rule clause.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#values DataLaunchdarklySegment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#values DataLaunchdarklySegment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def context_kind(self) -> typing.Optional[builtins.str]:
         '''The context kind associated with this rule clause. If omitted, defaults to user.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#context_kind DataLaunchdarklySegment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#context_kind DataLaunchdarklySegment#context_kind}
         '''
         result = self._values.get("context_kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def negate(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether to negate the rule clause.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#negate DataLaunchdarklySegment#negate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#negate DataLaunchdarklySegment#negate}
         '''
         result = self._values.get("negate")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def value_type(self) -> typing.Optional[builtins.str]:
         '''The type for each of the clause's values.
 
         Available types are boolean, string, and number. If omitted, value_type defaults to string
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/segment#value_type DataLaunchdarklySegment#value_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/segment#value_type DataLaunchdarklySegment#value_type}
         '''
         result = self._values.get("value_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_team`
 
-Refer to the Terraform Registory for docs: [`data_launchdarkly_team`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team).
+Refer to the Terraform Registory for docs: [`data_launchdarkly_team`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataLaunchdarklyTeam(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyTeam.DataLaunchdarklyTeam",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team launchdarkly_team}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team launchdarkly_team}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team launchdarkly_team} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team launchdarkly_team} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team#key DataLaunchdarklyTeam#key}
-        :param custom_role_keys: A list of keys for custom roles the team has. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team#custom_role_keys DataLaunchdarklyTeam#custom_role_keys}
-        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team#description DataLaunchdarklyTeam#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team#id DataLaunchdarklyTeam#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team#name DataLaunchdarklyTeam#name}
+        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team#key DataLaunchdarklyTeam#key}
+        :param custom_role_keys: A list of keys for custom roles the team has. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team#custom_role_keys DataLaunchdarklyTeam#custom_role_keys}
+        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team#description DataLaunchdarklyTeam#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team#id DataLaunchdarklyTeam#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team#name DataLaunchdarklyTeam#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -244,19 +244,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team#key DataLaunchdarklyTeam#key}
-        :param custom_role_keys: A list of keys for custom roles the team has. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team#custom_role_keys DataLaunchdarklyTeam#custom_role_keys}
-        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team#description DataLaunchdarklyTeam#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team#id DataLaunchdarklyTeam#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team#name DataLaunchdarklyTeam#name}
+        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team#key DataLaunchdarklyTeam#key}
+        :param custom_role_keys: A list of keys for custom roles the team has. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team#custom_role_keys DataLaunchdarklyTeam#custom_role_keys}
+        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team#description DataLaunchdarklyTeam#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team#id DataLaunchdarklyTeam#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team#name DataLaunchdarklyTeam#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7badedbfe7425728bb984aea443d446b602f67e9c6bef983bb86976600624516)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -360,53 +360,53 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The team's unique key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team#key DataLaunchdarklyTeam#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team#key DataLaunchdarklyTeam#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def custom_role_keys(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of keys for custom roles the team has.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team#custom_role_keys DataLaunchdarklyTeam#custom_role_keys}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team#custom_role_keys DataLaunchdarklyTeam#custom_role_keys}
         '''
         result = self._values.get("custom_role_keys")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The team's description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team#description DataLaunchdarklyTeam#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team#description DataLaunchdarklyTeam#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team#id DataLaunchdarklyTeam#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team#id DataLaunchdarklyTeam#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The team's human-readable name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team#name DataLaunchdarklyTeam#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team#name DataLaunchdarklyTeam#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_member/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_member/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_team_member`
 
-Refer to the Terraform Registory for docs: [`data_launchdarkly_team_member`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_member).
+Refer to the Terraform Registory for docs: [`data_launchdarkly_team_member`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_member).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataLaunchdarklyTeamMember(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyTeamMember.DataLaunchdarklyTeamMember",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_member launchdarkly_team_member}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_member launchdarkly_team_member}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         email: builtins.str,
@@ -39,20 +39,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_member launchdarkly_team_member} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_member launchdarkly_team_member} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_member#email DataLaunchdarklyTeamMember#email}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_member#id DataLaunchdarklyTeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_member#email DataLaunchdarklyTeamMember#email}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_member#id DataLaunchdarklyTeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -176,16 +176,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_member#email DataLaunchdarklyTeamMember#email}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_member#id DataLaunchdarklyTeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_member#email DataLaunchdarklyTeamMember#email}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_member#id DataLaunchdarklyTeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7a6edd1e638b44c7b98e955269c9bca5af17547ada027c5912fee47e117b60da)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -278,22 +278,22 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def email(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_member#email DataLaunchdarklyTeamMember#email}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_member#email DataLaunchdarklyTeamMember#email}.'''
         result = self._values.get("email")
         assert result is not None, "Required property 'email' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_member#id DataLaunchdarklyTeamMember#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_member#id DataLaunchdarklyTeamMember#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_members/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_team_members/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_team_members`
 
-Refer to the Terraform Registory for docs: [`data_launchdarkly_team_members`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_members).
+Refer to the Terraform Registory for docs: [`data_launchdarkly_team_members`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_members).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataLaunchdarklyTeamMembers(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyTeamMembers.DataLaunchdarklyTeamMembers",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_members launchdarkly_team_members}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_members launchdarkly_team_members}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         emails: typing.Sequence[builtins.str],
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_members launchdarkly_team_members} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_members launchdarkly_team_members} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param emails: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_members#emails DataLaunchdarklyTeamMembers#emails}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_members#id DataLaunchdarklyTeamMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ignore_missing: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_members#ignore_missing DataLaunchdarklyTeamMembers#ignore_missing}.
+        :param emails: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_members#emails DataLaunchdarklyTeamMembers#emails}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_members#id DataLaunchdarklyTeamMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param ignore_missing: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_members#ignore_missing DataLaunchdarklyTeamMembers#ignore_missing}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -194,17 +194,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param emails: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_members#emails DataLaunchdarklyTeamMembers#emails}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_members#id DataLaunchdarklyTeamMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param ignore_missing: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_members#ignore_missing DataLaunchdarklyTeamMembers#ignore_missing}.
+        :param emails: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_members#emails DataLaunchdarklyTeamMembers#emails}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_members#id DataLaunchdarklyTeamMembers#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param ignore_missing: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_members#ignore_missing DataLaunchdarklyTeamMembers#ignore_missing}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c3f21dd6b852fbc99de16a75ccb5b53977e93aeed01a891b5de7ba8d9a5ab7f5)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -300,34 +300,34 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def emails(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_members#emails DataLaunchdarklyTeamMembers#emails}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_members#emails DataLaunchdarklyTeamMembers#emails}.'''
         result = self._values.get("emails")
         assert result is not None, "Required property 'emails' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_members#id DataLaunchdarklyTeamMembers#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_members#id DataLaunchdarklyTeamMembers#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ignore_missing(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/team_members#ignore_missing DataLaunchdarklyTeamMembers#ignore_missing}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/team_members#ignore_missing DataLaunchdarklyTeamMembers#ignore_missing}.'''
         result = self._values.get("ignore_missing")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_webhook/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_webhook/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_launchdarkly_webhook`
 
-Refer to the Terraform Registory for docs: [`data_launchdarkly_webhook`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook).
+Refer to the Terraform Registory for docs: [`data_launchdarkly_webhook`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataLaunchdarklyWebhook(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.dataLaunchdarklyWebhook.DataLaunchdarklyWebhook",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook launchdarkly_webhook}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook launchdarkly_webhook}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook launchdarkly_webhook} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook launchdarkly_webhook} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: The ID of the webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#id DataLaunchdarklyWebhook#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#name DataLaunchdarklyWebhook#name}
-        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#secret DataLaunchdarklyWebhook#secret}
-        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#statements DataLaunchdarklyWebhook#statements}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#tags DataLaunchdarklyWebhook#tags}
+        :param id: The ID of the webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#id DataLaunchdarklyWebhook#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#name DataLaunchdarklyWebhook#name}
+        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#secret DataLaunchdarklyWebhook#secret}
+        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#statements DataLaunchdarklyWebhook#statements}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#tags DataLaunchdarklyWebhook#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -252,19 +252,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: The ID of the webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#id DataLaunchdarklyWebhook#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#name DataLaunchdarklyWebhook#name}
-        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#secret DataLaunchdarklyWebhook#secret}
-        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#statements DataLaunchdarklyWebhook#statements}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#tags DataLaunchdarklyWebhook#tags}
+        :param id: The ID of the webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#id DataLaunchdarklyWebhook#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#name DataLaunchdarklyWebhook#name}
+        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#secret DataLaunchdarklyWebhook#secret}
+        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#statements DataLaunchdarklyWebhook#statements}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#tags DataLaunchdarklyWebhook#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bb8e55aee311f83a83024803098694418c396805f00a0f1c480e08c2c444b0fd)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -368,57 +368,57 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> builtins.str:
         '''The ID of the webhook.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#id DataLaunchdarklyWebhook#id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#id DataLaunchdarklyWebhook#id}
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         assert result is not None, "Required property 'id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''A human-readable name for your webhook.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#name DataLaunchdarklyWebhook#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#name DataLaunchdarklyWebhook#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def secret(self) -> typing.Optional[builtins.str]:
         '''If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#secret DataLaunchdarklyWebhook#secret}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#secret DataLaunchdarklyWebhook#secret}
         '''
         result = self._values.get("secret")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def statements(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyWebhookStatements"]]]:
         '''statements block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#statements DataLaunchdarklyWebhook#statements}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#statements DataLaunchdarklyWebhook#statements}
         '''
         result = self._values.get("statements")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataLaunchdarklyWebhookStatements"]]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#tags DataLaunchdarklyWebhook#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#tags DataLaunchdarklyWebhook#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -449,19 +449,19 @@
         effect: builtins.str,
         actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
         resources: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#effect DataLaunchdarklyWebhook#effect}.
-        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#actions DataLaunchdarklyWebhook#actions}
-        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#not_actions DataLaunchdarklyWebhook#not_actions}
-        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#not_resources DataLaunchdarklyWebhook#not_resources}
-        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#resources DataLaunchdarklyWebhook#resources}
+        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#effect DataLaunchdarklyWebhook#effect}.
+        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#actions DataLaunchdarklyWebhook#actions}
+        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#not_actions DataLaunchdarklyWebhook#not_actions}
+        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#not_resources DataLaunchdarklyWebhook#not_resources}
+        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#resources DataLaunchdarklyWebhook#resources}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ccaa0ae14c4d889ad591a1fbdb09bf249446e281dab1d0662cafd40eee36eb09)
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument not_actions", value=not_actions, expected_type=type_hints["not_actions"])
             check_type(argname="argument not_resources", value=not_resources, expected_type=type_hints["not_resources"])
@@ -476,55 +476,55 @@
         if not_resources is not None:
             self._values["not_resources"] = not_resources
         if resources is not None:
             self._values["resources"] = resources
 
     @builtins.property
     def effect(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#effect DataLaunchdarklyWebhook#effect}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#effect DataLaunchdarklyWebhook#effect}.'''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''An action to perform on a resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#actions DataLaunchdarklyWebhook#actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#actions DataLaunchdarklyWebhook#actions}
         '''
         result = self._values.get("actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted actions will be those actions NOT in this list.
 
         The 'actions' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#not_actions DataLaunchdarklyWebhook#not_actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#not_actions DataLaunchdarklyWebhook#not_actions}
         '''
         result = self._values.get("not_actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted resources will be those resources NOT in this list.
 
         The 'resources' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#not_resources DataLaunchdarklyWebhook#not_resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#not_resources DataLaunchdarklyWebhook#not_resources}
         '''
         result = self._values.get("not_resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of LaunchDarkly resource specifiers.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/data-sources/webhook#resources DataLaunchdarklyWebhook#resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/data-sources/webhook#resources DataLaunchdarklyWebhook#resources}
         '''
         result = self._values.get("resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/destination/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/destination/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_destination`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_destination`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination).
+Refer to the Terraform Registory for docs: [`launchdarkly_destination`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Destination(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.destination.Destination",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination launchdarkly_destination}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination launchdarkly_destination}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         config: typing.Mapping[builtins.str, builtins.str],
@@ -45,26 +45,26 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination launchdarkly_destination} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination launchdarkly_destination} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param config: The destination-specific configuration object corresponding to your data export kind - see documentation for required fields for each kind. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#config Destination#config}
-        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#env_key Destination#env_key}
-        :param kind: The data export destination type. Available choices are 'kinesis', 'google-pubsub', 'segment', 'azure-event-hubs', and 'mparticle'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#kind Destination#kind}
-        :param name: A human-readable name for your data export destination. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#name Destination#name}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#project_key Destination#project_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#id Destination#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param on: Whether the data export destination is on or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#on Destination#on}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#tags Destination#tags}
+        :param config: The destination-specific configuration object corresponding to your data export kind - see documentation for required fields for each kind. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#config Destination#config}
+        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#env_key Destination#env_key}
+        :param kind: The data export destination type. Available choices are 'kinesis', 'google-pubsub', 'segment', 'azure-event-hubs', and 'mparticle'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#kind Destination#kind}
+        :param name: A human-readable name for your data export destination. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#name Destination#name}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#project_key Destination#project_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#id Destination#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param on: Whether the data export destination is on or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#on Destination#on}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#tags Destination#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -303,22 +303,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param config: The destination-specific configuration object corresponding to your data export kind - see documentation for required fields for each kind. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#config Destination#config}
-        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#env_key Destination#env_key}
-        :param kind: The data export destination type. Available choices are 'kinesis', 'google-pubsub', 'segment', 'azure-event-hubs', and 'mparticle'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#kind Destination#kind}
-        :param name: A human-readable name for your data export destination. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#name Destination#name}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#project_key Destination#project_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#id Destination#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param on: Whether the data export destination is on or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#on Destination#on}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#tags Destination#tags}
+        :param config: The destination-specific configuration object corresponding to your data export kind - see documentation for required fields for each kind. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#config Destination#config}
+        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#env_key Destination#env_key}
+        :param kind: The data export destination type. Available choices are 'kinesis', 'google-pubsub', 'segment', 'azure-event-hubs', and 'mparticle'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#kind Destination#kind}
+        :param name: A human-readable name for your data export destination. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#name Destination#name}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#project_key Destination#project_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#id Destination#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param on: Whether the data export destination is on or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#on Destination#on}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#tags Destination#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__466ca569c4ac44df79406165ee289e41c545d765b1fe3b6a01178b89a9ec74e8)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -427,86 +427,86 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def config(self) -> typing.Mapping[builtins.str, builtins.str]:
         '''The destination-specific configuration object corresponding to your data export kind - see documentation for required fields for each kind.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#config Destination#config}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#config Destination#config}
         '''
         result = self._values.get("config")
         assert result is not None, "Required property 'config' is missing"
         return typing.cast(typing.Mapping[builtins.str, builtins.str], result)
 
     @builtins.property
     def env_key(self) -> builtins.str:
         '''The LaunchDarkly environment key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#env_key Destination#env_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#env_key Destination#env_key}
         '''
         result = self._values.get("env_key")
         assert result is not None, "Required property 'env_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def kind(self) -> builtins.str:
         '''The data export destination type. Available choices are 'kinesis', 'google-pubsub', 'segment', 'azure-event-hubs', and 'mparticle'.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#kind Destination#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#kind Destination#kind}
         '''
         result = self._values.get("kind")
         assert result is not None, "Required property 'kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''A human-readable name for your data export destination.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#name Destination#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#name Destination#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The LaunchDarkly project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#project_key Destination#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#project_key Destination#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#id Destination#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#id Destination#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def on(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether the data export destination is on or not.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#on Destination#on}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#on Destination#on}
         '''
         result = self._values.get("on")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/destination#tags Destination#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/destination#tags Destination#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/environment/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/environment/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_environment`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment).
+Refer to the Terraform Registory for docs: [`launchdarkly_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Environment(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.environment.Environment",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment launchdarkly_environment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment launchdarkly_environment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         color: builtins.str,
@@ -49,30 +49,30 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment launchdarkly_environment} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment launchdarkly_environment} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param color: A color swatch (as an RGB hex value with no leading '#', e.g. C8C8C8). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#color Environment#color}
-        :param key: A project-unique key for the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#key Environment#key}
-        :param name: The name of the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#name Environment#name}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#project_key Environment#project_key}
-        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#approval_settings Environment#approval_settings}
-        :param confirm_changes: Whether or not to require confirmation for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#confirm_changes Environment#confirm_changes}
-        :param default_track_events: Whether or not to default to sending data export events for flags created in the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#default_track_events Environment#default_track_events}
-        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#default_ttl Environment#default_ttl}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#id Environment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param require_comments: Whether or not to require comments for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#require_comments Environment#require_comments}
-        :param secure_mode: Whether or not to use secure mode. Secure mode ensures a user of the client-side SDK cannot impersonate another user Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#secure_mode Environment#secure_mode}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#tags Environment#tags}
+        :param color: A color swatch (as an RGB hex value with no leading '#', e.g. C8C8C8). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#color Environment#color}
+        :param key: A project-unique key for the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#key Environment#key}
+        :param name: The name of the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#name Environment#name}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#project_key Environment#project_key}
+        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#approval_settings Environment#approval_settings}
+        :param confirm_changes: Whether or not to require confirmation for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#confirm_changes Environment#confirm_changes}
+        :param default_track_events: Whether or not to default to sending data export events for flags created in the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#default_track_events Environment#default_track_events}
+        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#default_ttl Environment#default_ttl}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#id Environment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param require_comments: Whether or not to require comments for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#require_comments Environment#require_comments}
+        :param secure_mode: Whether or not to use secure mode. Secure mode ensures a user of the client-side SDK cannot impersonate another user Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#secure_mode Environment#secure_mode}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#tags Environment#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -418,19 +418,19 @@
         can_apply_declined_changes: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         can_review_own_request: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         min_num_approvals: typing.Optional[jsii.Number] = None,
         required: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         required_approval_tags: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param can_apply_declined_changes: Whether changes can be applied as long as minNumApprovals is met, regardless of whether any reviewers have declined a request. Defaults to true Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#can_apply_declined_changes Environment#can_apply_declined_changes}
-        :param can_review_own_request: Whether requesters can approve or decline their own request. They may always comment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#can_review_own_request Environment#can_review_own_request}
-        :param min_num_approvals: The number of approvals required before an approval request can be applied. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#min_num_approvals Environment#min_num_approvals}
-        :param required: Whether any changes to flags in this environment will require approval. You may only set required or requiredApprovalTags, not both. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#required Environment#required}
-        :param required_approval_tags: An array of tags used to specify which flags with those tags require approval. You may only set requiredApprovalTags or required, not both. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#required_approval_tags Environment#required_approval_tags}
+        :param can_apply_declined_changes: Whether changes can be applied as long as minNumApprovals is met, regardless of whether any reviewers have declined a request. Defaults to true Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#can_apply_declined_changes Environment#can_apply_declined_changes}
+        :param can_review_own_request: Whether requesters can approve or decline their own request. They may always comment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#can_review_own_request Environment#can_review_own_request}
+        :param min_num_approvals: The number of approvals required before an approval request can be applied. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#min_num_approvals Environment#min_num_approvals}
+        :param required: Whether any changes to flags in this environment will require approval. You may only set required or requiredApprovalTags, not both. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#required Environment#required}
+        :param required_approval_tags: An array of tags used to specify which flags with those tags require approval. You may only set requiredApprovalTags or required, not both. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#required_approval_tags Environment#required_approval_tags}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fde5aff1deb87cd21c5ca5b96f9ed75728472d55dc6c7e315edff7452e2f09dd)
             check_type(argname="argument can_apply_declined_changes", value=can_apply_declined_changes, expected_type=type_hints["can_apply_declined_changes"])
             check_type(argname="argument can_review_own_request", value=can_review_own_request, expected_type=type_hints["can_review_own_request"])
             check_type(argname="argument min_num_approvals", value=min_num_approvals, expected_type=type_hints["min_num_approvals"])
             check_type(argname="argument required", value=required, expected_type=type_hints["required"])
@@ -451,59 +451,59 @@
     def can_apply_declined_changes(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether changes can be applied as long as minNumApprovals is met, regardless of whether any reviewers have declined a request.
 
         Defaults to true
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#can_apply_declined_changes Environment#can_apply_declined_changes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#can_apply_declined_changes Environment#can_apply_declined_changes}
         '''
         result = self._values.get("can_apply_declined_changes")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def can_review_own_request(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether requesters can approve or decline their own request. They may always comment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#can_review_own_request Environment#can_review_own_request}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#can_review_own_request Environment#can_review_own_request}
         '''
         result = self._values.get("can_review_own_request")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def min_num_approvals(self) -> typing.Optional[jsii.Number]:
         '''The number of approvals required before an approval request can be applied.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#min_num_approvals Environment#min_num_approvals}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#min_num_approvals Environment#min_num_approvals}
         '''
         result = self._values.get("min_num_approvals")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def required(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether any changes to flags in this environment will require approval.
 
         You may only set required or requiredApprovalTags, not both.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#required Environment#required}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#required Environment#required}
         '''
         result = self._values.get("required")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def required_approval_tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''An array of tags used to specify which flags with those tags require approval.
 
         You may only set requiredApprovalTags or required, not both.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#required_approval_tags Environment#required_approval_tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#required_approval_tags Environment#required_approval_tags}
         '''
         result = self._values.get("required_approval_tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -829,26 +829,26 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param color: A color swatch (as an RGB hex value with no leading '#', e.g. C8C8C8). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#color Environment#color}
-        :param key: A project-unique key for the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#key Environment#key}
-        :param name: The name of the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#name Environment#name}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#project_key Environment#project_key}
-        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#approval_settings Environment#approval_settings}
-        :param confirm_changes: Whether or not to require confirmation for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#confirm_changes Environment#confirm_changes}
-        :param default_track_events: Whether or not to default to sending data export events for flags created in the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#default_track_events Environment#default_track_events}
-        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#default_ttl Environment#default_ttl}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#id Environment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param require_comments: Whether or not to require comments for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#require_comments Environment#require_comments}
-        :param secure_mode: Whether or not to use secure mode. Secure mode ensures a user of the client-side SDK cannot impersonate another user Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#secure_mode Environment#secure_mode}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#tags Environment#tags}
+        :param color: A color swatch (as an RGB hex value with no leading '#', e.g. C8C8C8). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#color Environment#color}
+        :param key: A project-unique key for the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#key Environment#key}
+        :param name: The name of the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#name Environment#name}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#project_key Environment#project_key}
+        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#approval_settings Environment#approval_settings}
+        :param confirm_changes: Whether or not to require confirmation for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#confirm_changes Environment#confirm_changes}
+        :param default_track_events: Whether or not to default to sending data export events for flags created in the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#default_track_events Environment#default_track_events}
+        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#default_ttl Environment#default_ttl}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#id Environment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param require_comments: Whether or not to require comments for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#require_comments Environment#require_comments}
+        :param secure_mode: Whether or not to use secure mode. Secure mode ensures a user of the client-side SDK cannot impersonate another user Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#secure_mode Environment#secure_mode}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#tags Environment#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6e0608c2d3a8c4886786970a153e9cd6eadb59d4a6053f51e829a03f3de98831)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -970,133 +970,133 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def color(self) -> builtins.str:
         '''A color swatch (as an RGB hex value with no leading '#', e.g. C8C8C8).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#color Environment#color}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#color Environment#color}
         '''
         result = self._values.get("color")
         assert result is not None, "Required property 'color' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''A project-unique key for the new environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#key Environment#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#key Environment#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the new environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#name Environment#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#name Environment#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The LaunchDarkly project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#project_key Environment#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#project_key Environment#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def approval_settings(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[EnvironmentApprovalSettings]]]:
         '''approval_settings block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#approval_settings Environment#approval_settings}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#approval_settings Environment#approval_settings}
         '''
         result = self._values.get("approval_settings")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[EnvironmentApprovalSettings]]], result)
 
     @builtins.property
     def confirm_changes(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not to require confirmation for flag and segment changes in this environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#confirm_changes Environment#confirm_changes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#confirm_changes Environment#confirm_changes}
         '''
         result = self._values.get("confirm_changes")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def default_track_events(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not to default to sending data export events for flags created in the environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#default_track_events Environment#default_track_events}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#default_track_events Environment#default_track_events}
         '''
         result = self._values.get("default_track_events")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def default_ttl(self) -> typing.Optional[jsii.Number]:
         '''The TTL for the environment.
 
         This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#default_ttl Environment#default_ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#default_ttl Environment#default_ttl}
         '''
         result = self._values.get("default_ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#id Environment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#id Environment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def require_comments(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not to require comments for flag and segment changes in this environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#require_comments Environment#require_comments}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#require_comments Environment#require_comments}
         '''
         result = self._values.get("require_comments")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def secure_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not to use secure mode.
 
         Secure mode ensures a user of the client-side SDK cannot impersonate another user
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#secure_mode Environment#secure_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#secure_mode Environment#secure_mode}
         '''
         result = self._values.get("secure_mode")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/environment#tags Environment#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/environment#tags Environment#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/feature_flag/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/feature_flag/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_feature_flag`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_feature_flag`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag).
+Refer to the Terraform Registory for docs: [`launchdarkly_feature_flag`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class FeatureFlag(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.featureFlag.FeatureFlag",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag launchdarkly_feature_flag}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag launchdarkly_feature_flag}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -52,33 +52,33 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag launchdarkly_feature_flag} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag launchdarkly_feature_flag} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: A unique key that will be used to reference the flag in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#key FeatureFlag#key}
-        :param name: A human-friendly name for the feature flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#name FeatureFlag#name}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#project_key FeatureFlag#project_key}
-        :param variation_type: The uniform type for all variations. Can be either "boolean", "string", "number", or "json". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#variation_type FeatureFlag#variation_type}
-        :param archived: Whether to archive the flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#archived FeatureFlag#archived}
-        :param client_side_availability: client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#client_side_availability FeatureFlag#client_side_availability}
-        :param custom_properties: custom_properties block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#custom_properties FeatureFlag#custom_properties}
-        :param defaults: defaults block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#defaults FeatureFlag#defaults}
-        :param description: A short description of what the flag will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#description FeatureFlag#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#id FeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param include_in_snippet: Whether or not this flag should be made available to the client-side JavaScript SDK. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#include_in_snippet FeatureFlag#include_in_snippet}
-        :param maintainer_id: The LaunchDarkly id of the user who will maintain the flag. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#maintainer_id FeatureFlag#maintainer_id}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#tags FeatureFlag#tags}
-        :param temporary: Whether or not the flag is a temporary flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#temporary FeatureFlag#temporary}
-        :param variations: variations block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#variations FeatureFlag#variations}
+        :param key: A unique key that will be used to reference the flag in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#key FeatureFlag#key}
+        :param name: A human-friendly name for the feature flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#name FeatureFlag#name}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#project_key FeatureFlag#project_key}
+        :param variation_type: The uniform type for all variations. Can be either "boolean", "string", "number", or "json". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#variation_type FeatureFlag#variation_type}
+        :param archived: Whether to archive the flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#archived FeatureFlag#archived}
+        :param client_side_availability: client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#client_side_availability FeatureFlag#client_side_availability}
+        :param custom_properties: custom_properties block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#custom_properties FeatureFlag#custom_properties}
+        :param defaults: defaults block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#defaults FeatureFlag#defaults}
+        :param description: A short description of what the flag will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#description FeatureFlag#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#id FeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param include_in_snippet: Whether or not this flag should be made available to the client-side JavaScript SDK. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#include_in_snippet FeatureFlag#include_in_snippet}
+        :param maintainer_id: The LaunchDarkly id of the user who will maintain the flag. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#maintainer_id FeatureFlag#maintainer_id}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#tags FeatureFlag#tags}
+        :param temporary: Whether or not the flag is a temporary flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#temporary FeatureFlag#temporary}
+        :param variations: variations block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#variations FeatureFlag#variations}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -144,16 +144,16 @@
     def put_defaults(
         self,
         *,
         off_variation: jsii.Number,
         on_variation: jsii.Number,
     ) -> None:
         '''
-        :param off_variation: The index of the variation served when the flag is off for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#off_variation FeatureFlag#off_variation}
-        :param on_variation: The index of the variation served when the flag is on for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#on_variation FeatureFlag#on_variation}
+        :param off_variation: The index of the variation served when the flag is off for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#off_variation FeatureFlag#off_variation}
+        :param on_variation: The index of the variation served when the flag is on for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#on_variation FeatureFlag#on_variation}
         '''
         value = FeatureFlagDefaults(
             off_variation=off_variation, on_variation=on_variation
         )
 
         return typing.cast(None, jsii.invoke(self, "putDefaults", [value]))
 
@@ -486,16 +486,16 @@
     def __init__(
         self,
         *,
         using_environment_id: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         using_mobile_key: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     ) -> None:
         '''
-        :param using_environment_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#using_environment_id FeatureFlag#using_environment_id}.
-        :param using_mobile_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#using_mobile_key FeatureFlag#using_mobile_key}.
+        :param using_environment_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#using_environment_id FeatureFlag#using_environment_id}.
+        :param using_mobile_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#using_mobile_key FeatureFlag#using_mobile_key}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__07f14cdaea6f10e022a6d396c287ff71ccbe0531800c60eed40fcce76ed2098e)
             check_type(argname="argument using_environment_id", value=using_environment_id, expected_type=type_hints["using_environment_id"])
             check_type(argname="argument using_mobile_key", value=using_mobile_key, expected_type=type_hints["using_mobile_key"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if using_environment_id is not None:
@@ -503,23 +503,23 @@
         if using_mobile_key is not None:
             self._values["using_mobile_key"] = using_mobile_key
 
     @builtins.property
     def using_environment_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#using_environment_id FeatureFlag#using_environment_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#using_environment_id FeatureFlag#using_environment_id}.'''
         result = self._values.get("using_environment_id")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def using_mobile_key(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#using_mobile_key FeatureFlag#using_mobile_key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#using_mobile_key FeatureFlag#using_mobile_key}.'''
         result = self._values.get("using_mobile_key")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -783,29 +783,29 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: A unique key that will be used to reference the flag in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#key FeatureFlag#key}
-        :param name: A human-friendly name for the feature flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#name FeatureFlag#name}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#project_key FeatureFlag#project_key}
-        :param variation_type: The uniform type for all variations. Can be either "boolean", "string", "number", or "json". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#variation_type FeatureFlag#variation_type}
-        :param archived: Whether to archive the flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#archived FeatureFlag#archived}
-        :param client_side_availability: client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#client_side_availability FeatureFlag#client_side_availability}
-        :param custom_properties: custom_properties block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#custom_properties FeatureFlag#custom_properties}
-        :param defaults: defaults block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#defaults FeatureFlag#defaults}
-        :param description: A short description of what the flag will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#description FeatureFlag#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#id FeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param include_in_snippet: Whether or not this flag should be made available to the client-side JavaScript SDK. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#include_in_snippet FeatureFlag#include_in_snippet}
-        :param maintainer_id: The LaunchDarkly id of the user who will maintain the flag. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#maintainer_id FeatureFlag#maintainer_id}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#tags FeatureFlag#tags}
-        :param temporary: Whether or not the flag is a temporary flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#temporary FeatureFlag#temporary}
-        :param variations: variations block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#variations FeatureFlag#variations}
+        :param key: A unique key that will be used to reference the flag in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#key FeatureFlag#key}
+        :param name: A human-friendly name for the feature flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#name FeatureFlag#name}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#project_key FeatureFlag#project_key}
+        :param variation_type: The uniform type for all variations. Can be either "boolean", "string", "number", or "json". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#variation_type FeatureFlag#variation_type}
+        :param archived: Whether to archive the flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#archived FeatureFlag#archived}
+        :param client_side_availability: client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#client_side_availability FeatureFlag#client_side_availability}
+        :param custom_properties: custom_properties block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#custom_properties FeatureFlag#custom_properties}
+        :param defaults: defaults block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#defaults FeatureFlag#defaults}
+        :param description: A short description of what the flag will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#description FeatureFlag#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#id FeatureFlag#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param include_in_snippet: Whether or not this flag should be made available to the client-side JavaScript SDK. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#include_in_snippet FeatureFlag#include_in_snippet}
+        :param maintainer_id: The LaunchDarkly id of the user who will maintain the flag. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#maintainer_id FeatureFlag#maintainer_id}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#tags FeatureFlag#tags}
+        :param temporary: Whether or not the flag is a temporary flag. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#temporary FeatureFlag#temporary}
+        :param variations: variations block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#variations FeatureFlag#variations}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(defaults, dict):
             defaults = FeatureFlagDefaults(**defaults)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a2b024440d957862712c9755f97389f4b688ffe513bf440a776f2367528a7e9f)
@@ -938,160 +938,160 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''A unique key that will be used to reference the flag in your code.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#key FeatureFlag#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#key FeatureFlag#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''A human-friendly name for the feature flag.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#name FeatureFlag#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#name FeatureFlag#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The LaunchDarkly project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#project_key FeatureFlag#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#project_key FeatureFlag#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def variation_type(self) -> builtins.str:
         '''The uniform type for all variations. Can be either "boolean", "string", "number", or "json".
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#variation_type FeatureFlag#variation_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#variation_type FeatureFlag#variation_type}
         '''
         result = self._values.get("variation_type")
         assert result is not None, "Required property 'variation_type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def archived(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether to archive the flag.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#archived FeatureFlag#archived}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#archived FeatureFlag#archived}
         '''
         result = self._values.get("archived")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def client_side_availability(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[FeatureFlagClientSideAvailability]]]:
         '''client_side_availability block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#client_side_availability FeatureFlag#client_side_availability}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#client_side_availability FeatureFlag#client_side_availability}
         '''
         result = self._values.get("client_side_availability")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[FeatureFlagClientSideAvailability]]], result)
 
     @builtins.property
     def custom_properties(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagCustomProperties"]]]:
         '''custom_properties block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#custom_properties FeatureFlag#custom_properties}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#custom_properties FeatureFlag#custom_properties}
         '''
         result = self._values.get("custom_properties")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagCustomProperties"]]], result)
 
     @builtins.property
     def defaults(self) -> typing.Optional["FeatureFlagDefaults"]:
         '''defaults block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#defaults FeatureFlag#defaults}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#defaults FeatureFlag#defaults}
         '''
         result = self._values.get("defaults")
         return typing.cast(typing.Optional["FeatureFlagDefaults"], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''A short description of what the flag will be used for.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#description FeatureFlag#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#description FeatureFlag#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#id FeatureFlag#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#id FeatureFlag#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def include_in_snippet(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not this flag should be made available to the client-side JavaScript SDK.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#include_in_snippet FeatureFlag#include_in_snippet}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#include_in_snippet FeatureFlag#include_in_snippet}
         '''
         result = self._values.get("include_in_snippet")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def maintainer_id(self) -> typing.Optional[builtins.str]:
         '''The LaunchDarkly id of the user who will maintain the flag.
 
         If not set, the API will automatically apply the member associated with your Terraform API key or the most recently set maintainer
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#maintainer_id FeatureFlag#maintainer_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#maintainer_id FeatureFlag#maintainer_id}
         '''
         result = self._values.get("maintainer_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#tags FeatureFlag#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#tags FeatureFlag#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def temporary(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not the flag is a temporary flag.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#temporary FeatureFlag#temporary}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#temporary FeatureFlag#temporary}
         '''
         result = self._values.get("temporary")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def variations(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagVariations"]]]:
         '''variations block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#variations FeatureFlag#variations}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#variations FeatureFlag#variations}
         '''
         result = self._values.get("variations")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagVariations"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1114,46 +1114,46 @@
         self,
         *,
         key: builtins.str,
         name: builtins.str,
         value: typing.Sequence[builtins.str],
     ) -> None:
         '''
-        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#key FeatureFlag#key}.
-        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#name FeatureFlag#name}.
-        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#value FeatureFlag#value}.
+        :param key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#key FeatureFlag#key}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#name FeatureFlag#name}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#value FeatureFlag#value}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c7766b6ff19cff676147d8e598ddf37d57f59672f44b15e80616fff490f0023e)
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "key": key,
             "name": name,
             "value": value,
         }
 
     @builtins.property
     def key(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#key FeatureFlag#key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#key FeatureFlag#key}.'''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#name FeatureFlag#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#name FeatureFlag#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def value(self) -> typing.List[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#value FeatureFlag#value}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#value FeatureFlag#value}.'''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1360,41 +1360,41 @@
     def __init__(
         self,
         *,
         off_variation: jsii.Number,
         on_variation: jsii.Number,
     ) -> None:
         '''
-        :param off_variation: The index of the variation served when the flag is off for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#off_variation FeatureFlag#off_variation}
-        :param on_variation: The index of the variation served when the flag is on for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#on_variation FeatureFlag#on_variation}
+        :param off_variation: The index of the variation served when the flag is off for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#off_variation FeatureFlag#off_variation}
+        :param on_variation: The index of the variation served when the flag is on for new environments. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#on_variation FeatureFlag#on_variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2c66a4687bbd5a78f091fc125765bf2a56a6b71c8a235252b256684c9a8aa2f1)
             check_type(argname="argument off_variation", value=off_variation, expected_type=type_hints["off_variation"])
             check_type(argname="argument on_variation", value=on_variation, expected_type=type_hints["on_variation"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "off_variation": off_variation,
             "on_variation": on_variation,
         }
 
     @builtins.property
     def off_variation(self) -> jsii.Number:
         '''The index of the variation served when the flag is off for new environments.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#off_variation FeatureFlag#off_variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#off_variation FeatureFlag#off_variation}
         '''
         result = self._values.get("off_variation")
         assert result is not None, "Required property 'off_variation' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def on_variation(self) -> jsii.Number:
         '''The index of the variation served when the flag is on for new environments.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#on_variation FeatureFlag#on_variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#on_variation FeatureFlag#on_variation}
         '''
         result = self._values.get("on_variation")
         assert result is not None, "Required property 'on_variation' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1485,17 +1485,17 @@
         self,
         *,
         value: builtins.str,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param value: The value of the flag for this variation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#value FeatureFlag#value}
-        :param description: A description for the variation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#description FeatureFlag#description}
-        :param name: A name for the variation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#name FeatureFlag#name}
+        :param value: The value of the flag for this variation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#value FeatureFlag#value}
+        :param description: A description for the variation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#description FeatureFlag#description}
+        :param name: A name for the variation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#name FeatureFlag#name}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__190f28e6db25553ffb3b995e566038ac05cac527b1eb46d2227cd70af5c912fa)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -1506,34 +1506,34 @@
         if name is not None:
             self._values["name"] = name
 
     @builtins.property
     def value(self) -> builtins.str:
         '''The value of the flag for this variation.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#value FeatureFlag#value}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#value FeatureFlag#value}
         '''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''A description for the variation.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#description FeatureFlag#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#description FeatureFlag#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''A name for the variation.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag#name FeatureFlag#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag#name FeatureFlag#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/feature_flag_environment/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/feature_flag_environment/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_feature_flag_environment`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_feature_flag_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment).
+Refer to the Terraform Registory for docs: [`launchdarkly_feature_flag_environment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class FeatureFlagEnvironment(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.featureFlagEnvironment.FeatureFlagEnvironment",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment launchdarkly_feature_flag_environment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment launchdarkly_feature_flag_environment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         env_key: builtins.str,
@@ -48,29 +48,29 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment launchdarkly_feature_flag_environment} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment launchdarkly_feature_flag_environment} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#env_key FeatureFlagEnvironment#env_key}
-        :param fallthrough: fallthrough block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#fallthrough FeatureFlagEnvironment#fallthrough}
-        :param flag_id: The global feature flag's unique id in the format ``<project_key>/<flag_key>``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#flag_id FeatureFlagEnvironment#flag_id}
-        :param off_variation: The index of the variation to serve if targeting is disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#off_variation FeatureFlagEnvironment#off_variation}
-        :param context_targets: context_targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#context_targets FeatureFlagEnvironment#context_targets}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#id FeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param on: Whether targeting is enabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#on FeatureFlagEnvironment#on}
-        :param prerequisites: prerequisites block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#prerequisites FeatureFlagEnvironment#prerequisites}
-        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#rules FeatureFlagEnvironment#rules}
-        :param targets: targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#targets FeatureFlagEnvironment#targets}
-        :param track_events: Whether to send event data back to LaunchDarkly. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#track_events FeatureFlagEnvironment#track_events}
+        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#env_key FeatureFlagEnvironment#env_key}
+        :param fallthrough: fallthrough block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#fallthrough FeatureFlagEnvironment#fallthrough}
+        :param flag_id: The global feature flag's unique id in the format ``<project_key>/<flag_key>``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#flag_id FeatureFlagEnvironment#flag_id}
+        :param off_variation: The index of the variation to serve if targeting is disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#off_variation FeatureFlagEnvironment#off_variation}
+        :param context_targets: context_targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#context_targets FeatureFlagEnvironment#context_targets}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#id FeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param on: Whether targeting is enabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#on FeatureFlagEnvironment#on}
+        :param prerequisites: prerequisites block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#prerequisites FeatureFlagEnvironment#prerequisites}
+        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#rules FeatureFlagEnvironment#rules}
+        :param targets: targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#targets FeatureFlagEnvironment#targets}
+        :param track_events: Whether to send event data back to LaunchDarkly. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#track_events FeatureFlagEnvironment#track_events}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -121,18 +121,18 @@
         *,
         bucket_by: typing.Optional[builtins.str] = None,
         context_kind: typing.Optional[builtins.str] = None,
         rollout_weights: typing.Optional[typing.Sequence[jsii.Number]] = None,
         variation: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
-        :param context_kind: The context kind associated with the specified rollout. This argument is only valid if rollout_weights is also specified. If omitted, defaults to 'user' Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
-        :param rollout_weights: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}.
-        :param variation: The integer variation index to serve in case of fallthrough. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
+        :param context_kind: The context kind associated with the specified rollout. This argument is only valid if rollout_weights is also specified. If omitted, defaults to 'user' Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
+        :param rollout_weights: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}.
+        :param variation: The integer variation index to serve in case of fallthrough. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         value = FeatureFlagEnvironmentFallthrough(
             bucket_by=bucket_by,
             context_kind=context_kind,
             rollout_weights=rollout_weights,
             variation=variation,
         )
@@ -437,25 +437,25 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#env_key FeatureFlagEnvironment#env_key}
-        :param fallthrough: fallthrough block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#fallthrough FeatureFlagEnvironment#fallthrough}
-        :param flag_id: The global feature flag's unique id in the format ``<project_key>/<flag_key>``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#flag_id FeatureFlagEnvironment#flag_id}
-        :param off_variation: The index of the variation to serve if targeting is disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#off_variation FeatureFlagEnvironment#off_variation}
-        :param context_targets: context_targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#context_targets FeatureFlagEnvironment#context_targets}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#id FeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param on: Whether targeting is enabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#on FeatureFlagEnvironment#on}
-        :param prerequisites: prerequisites block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#prerequisites FeatureFlagEnvironment#prerequisites}
-        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#rules FeatureFlagEnvironment#rules}
-        :param targets: targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#targets FeatureFlagEnvironment#targets}
-        :param track_events: Whether to send event data back to LaunchDarkly. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#track_events FeatureFlagEnvironment#track_events}
+        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#env_key FeatureFlagEnvironment#env_key}
+        :param fallthrough: fallthrough block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#fallthrough FeatureFlagEnvironment#fallthrough}
+        :param flag_id: The global feature flag's unique id in the format ``<project_key>/<flag_key>``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#flag_id FeatureFlagEnvironment#flag_id}
+        :param off_variation: The index of the variation to serve if targeting is disabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#off_variation FeatureFlagEnvironment#off_variation}
+        :param context_targets: context_targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#context_targets FeatureFlagEnvironment#context_targets}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#id FeatureFlagEnvironment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param on: Whether targeting is enabled. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#on FeatureFlagEnvironment#on}
+        :param prerequisites: prerequisites block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#prerequisites FeatureFlagEnvironment#prerequisites}
+        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#rules FeatureFlagEnvironment#rules}
+        :param targets: targets block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#targets FeatureFlagEnvironment#targets}
+        :param track_events: Whether to send event data back to LaunchDarkly. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#track_events FeatureFlagEnvironment#track_events}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(fallthrough, dict):
             fallthrough = FeatureFlagEnvironmentFallthrough(**fallthrough)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7906af57752c788e0f057973f44c65cc16cb2d8bdf337d01f76caefb9503b806)
@@ -576,122 +576,122 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def env_key(self) -> builtins.str:
         '''The LaunchDarkly environment key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#env_key FeatureFlagEnvironment#env_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#env_key FeatureFlagEnvironment#env_key}
         '''
         result = self._values.get("env_key")
         assert result is not None, "Required property 'env_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def fallthrough(self) -> "FeatureFlagEnvironmentFallthrough":
         '''fallthrough block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#fallthrough FeatureFlagEnvironment#fallthrough}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#fallthrough FeatureFlagEnvironment#fallthrough}
         '''
         result = self._values.get("fallthrough")
         assert result is not None, "Required property 'fallthrough' is missing"
         return typing.cast("FeatureFlagEnvironmentFallthrough", result)
 
     @builtins.property
     def flag_id(self) -> builtins.str:
         '''The global feature flag's unique id in the format ``<project_key>/<flag_key>``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#flag_id FeatureFlagEnvironment#flag_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#flag_id FeatureFlagEnvironment#flag_id}
         '''
         result = self._values.get("flag_id")
         assert result is not None, "Required property 'flag_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def off_variation(self) -> jsii.Number:
         '''The index of the variation to serve if targeting is disabled.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#off_variation FeatureFlagEnvironment#off_variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#off_variation FeatureFlagEnvironment#off_variation}
         '''
         result = self._values.get("off_variation")
         assert result is not None, "Required property 'off_variation' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def context_targets(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentContextTargets"]]]:
         '''context_targets block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#context_targets FeatureFlagEnvironment#context_targets}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#context_targets FeatureFlagEnvironment#context_targets}
         '''
         result = self._values.get("context_targets")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentContextTargets"]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#id FeatureFlagEnvironment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#id FeatureFlagEnvironment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def on(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether targeting is enabled.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#on FeatureFlagEnvironment#on}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#on FeatureFlagEnvironment#on}
         '''
         result = self._values.get("on")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def prerequisites(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentPrerequisites"]]]:
         '''prerequisites block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#prerequisites FeatureFlagEnvironment#prerequisites}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#prerequisites FeatureFlagEnvironment#prerequisites}
         '''
         result = self._values.get("prerequisites")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentPrerequisites"]]], result)
 
     @builtins.property
     def rules(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentRules"]]]:
         '''rules block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#rules FeatureFlagEnvironment#rules}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#rules FeatureFlagEnvironment#rules}
         '''
         result = self._values.get("rules")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentRules"]]], result)
 
     @builtins.property
     def targets(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentTargets"]]]:
         '''targets block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#targets FeatureFlagEnvironment#targets}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#targets FeatureFlagEnvironment#targets}
         '''
         result = self._values.get("targets")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentTargets"]]], result)
 
     @builtins.property
     def track_events(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether to send event data back to LaunchDarkly.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#track_events FeatureFlagEnvironment#track_events}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#track_events FeatureFlagEnvironment#track_events}
         '''
         result = self._values.get("track_events")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -718,17 +718,17 @@
         self,
         *,
         context_kind: builtins.str,
         values: typing.Sequence[builtins.str],
         variation: jsii.Number,
     ) -> None:
         '''
-        :param context_kind: The context kind on which the flag should target in this environment. If the context_kind has not been previously specified at the project level, it will be automatically created on the project. User targets should be specified as targets attribute blocks. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
-        :param values: List of user strings to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
-        :param variation: Index of the variation to serve if a user_target is matched. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        :param context_kind: The context kind on which the flag should target in this environment. If the context_kind has not been previously specified at the project level, it will be automatically created on the project. User targets should be specified as targets attribute blocks. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
+        :param values: List of user strings to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
+        :param variation: Index of the variation to serve if a user_target is matched. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__34b5642f26bcae6d4dc7221ef36abd376437c6e3e3763e1e7abb20f783bf5eba)
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
             check_type(argname="argument variation", value=variation, expected_type=type_hints["variation"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
@@ -739,35 +739,35 @@
 
     @builtins.property
     def context_kind(self) -> builtins.str:
         '''The context kind on which the flag should target in this environment.
 
         If the context_kind has not been previously specified at the project level, it will be automatically created on the project. User targets should be specified as targets attribute blocks.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
         '''
         result = self._values.get("context_kind")
         assert result is not None, "Required property 'context_kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''List of user strings to target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def variation(self) -> jsii.Number:
         '''Index of the variation to serve if a user_target is matched.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         result = self._values.get("variation")
         assert result is not None, "Required property 'variation' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -985,18 +985,18 @@
         *,
         bucket_by: typing.Optional[builtins.str] = None,
         context_kind: typing.Optional[builtins.str] = None,
         rollout_weights: typing.Optional[typing.Sequence[jsii.Number]] = None,
         variation: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
-        :param context_kind: The context kind associated with the specified rollout. This argument is only valid if rollout_weights is also specified. If omitted, defaults to 'user' Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
-        :param rollout_weights: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}.
-        :param variation: The integer variation index to serve in case of fallthrough. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
+        :param context_kind: The context kind associated with the specified rollout. This argument is only valid if rollout_weights is also specified. If omitted, defaults to 'user' Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
+        :param rollout_weights: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}.
+        :param variation: The integer variation index to serve in case of fallthrough. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__daf881e63563456bfb70bbbeb289ea98f58d399b5ee497dbb67f9a344a45c1c2)
             check_type(argname="argument bucket_by", value=bucket_by, expected_type=type_hints["bucket_by"])
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
             check_type(argname="argument rollout_weights", value=rollout_weights, expected_type=type_hints["rollout_weights"])
             check_type(argname="argument variation", value=variation, expected_type=type_hints["variation"])
@@ -1010,41 +1010,41 @@
         if variation is not None:
             self._values["variation"] = variation
 
     @builtins.property
     def bucket_by(self) -> typing.Optional[builtins.str]:
         '''Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
         '''
         result = self._values.get("bucket_by")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def context_kind(self) -> typing.Optional[builtins.str]:
         '''The context kind associated with the specified rollout.
 
         This argument is only valid if rollout_weights is also specified. If omitted, defaults to 'user'
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
         '''
         result = self._values.get("context_kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def rollout_weights(self) -> typing.Optional[typing.List[jsii.Number]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}.'''
         result = self._values.get("rollout_weights")
         return typing.cast(typing.Optional[typing.List[jsii.Number]], result)
 
     @builtins.property
     def variation(self) -> typing.Optional[jsii.Number]:
         '''The integer variation index to serve in case of fallthrough.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         result = self._values.get("variation")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1181,41 +1181,41 @@
     jsii_type="@cdktf/provider-launchdarkly.featureFlagEnvironment.FeatureFlagEnvironmentPrerequisites",
     jsii_struct_bases=[],
     name_mapping={"flag_key": "flagKey", "variation": "variation"},
 )
 class FeatureFlagEnvironmentPrerequisites:
     def __init__(self, *, flag_key: builtins.str, variation: jsii.Number) -> None:
         '''
-        :param flag_key: The prerequisite feature flag's key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#flag_key FeatureFlagEnvironment#flag_key}
-        :param variation: The index of the prerequisite feature flag's variation to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        :param flag_key: The prerequisite feature flag's key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#flag_key FeatureFlagEnvironment#flag_key}
+        :param variation: The index of the prerequisite feature flag's variation to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__63941fb4c9cc7227c52d5626c12b2db316dd5ebb1ca55a101e171dbb2a76bc08)
             check_type(argname="argument flag_key", value=flag_key, expected_type=type_hints["flag_key"])
             check_type(argname="argument variation", value=variation, expected_type=type_hints["variation"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "flag_key": flag_key,
             "variation": variation,
         }
 
     @builtins.property
     def flag_key(self) -> builtins.str:
         '''The prerequisite feature flag's key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#flag_key FeatureFlagEnvironment#flag_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#flag_key FeatureFlagEnvironment#flag_key}
         '''
         result = self._values.get("flag_key")
         assert result is not None, "Required property 'flag_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def variation(self) -> jsii.Number:
         '''The index of the prerequisite feature flag's variation to target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         result = self._values.get("variation")
         assert result is not None, "Required property 'variation' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1418,19 +1418,19 @@
         bucket_by: typing.Optional[builtins.str] = None,
         clauses: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["FeatureFlagEnvironmentRulesClauses", typing.Dict[builtins.str, typing.Any]]]]] = None,
         description: typing.Optional[builtins.str] = None,
         rollout_weights: typing.Optional[typing.Sequence[jsii.Number]] = None,
         variation: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
-        :param clauses: clauses block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#clauses FeatureFlagEnvironment#clauses}
-        :param description: A human-readable description of the targeting rule. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#description FeatureFlagEnvironment#description}
-        :param rollout_weights: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}.
-        :param variation: The integer variation index to serve if the rule clauses evaluate to true. This argument is only valid if clauses are also specified Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        :param bucket_by: Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
+        :param clauses: clauses block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#clauses FeatureFlagEnvironment#clauses}
+        :param description: A human-readable description of the targeting rule. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#description FeatureFlagEnvironment#description}
+        :param rollout_weights: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}.
+        :param variation: The integer variation index to serve if the rule clauses evaluate to true. This argument is only valid if clauses are also specified Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__79fd8592ed8cb3c1d7ae89faf7fa874caef359c1bef31b4e19682af92accaf76)
             check_type(argname="argument bucket_by", value=bucket_by, expected_type=type_hints["bucket_by"])
             check_type(argname="argument clauses", value=clauses, expected_type=type_hints["clauses"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument rollout_weights", value=rollout_weights, expected_type=type_hints["rollout_weights"])
@@ -1447,52 +1447,52 @@
         if variation is not None:
             self._values["variation"] = variation
 
     @builtins.property
     def bucket_by(self) -> typing.Optional[builtins.str]:
         '''Group percentage rollout by a custom attribute. This argument is only valid if rollout_weights is also specified.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#bucket_by FeatureFlagEnvironment#bucket_by}
         '''
         result = self._values.get("bucket_by")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def clauses(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentRulesClauses"]]]:
         '''clauses block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#clauses FeatureFlagEnvironment#clauses}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#clauses FeatureFlagEnvironment#clauses}
         '''
         result = self._values.get("clauses")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["FeatureFlagEnvironmentRulesClauses"]]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''A human-readable description of the targeting rule.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#description FeatureFlagEnvironment#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#description FeatureFlagEnvironment#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def rollout_weights(self) -> typing.Optional[typing.List[jsii.Number]]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#rollout_weights FeatureFlagEnvironment#rollout_weights}.'''
         result = self._values.get("rollout_weights")
         return typing.cast(typing.Optional[typing.List[jsii.Number]], result)
 
     @builtins.property
     def variation(self) -> typing.Optional[jsii.Number]:
         '''The integer variation index to serve if the rule clauses evaluate to true.
 
         This argument is only valid if clauses are also specified
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         result = self._values.get("variation")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1525,20 +1525,20 @@
         op: builtins.str,
         values: typing.Sequence[builtins.str],
         context_kind: typing.Optional[builtins.str] = None,
         negate: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         value_type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param attribute: The user attribute to operate on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#attribute FeatureFlagEnvironment#attribute}
-        :param op: The operator associated with the rule clause. Available options are in, endsWith, startsWith, matches, contains, lessThan, lessThanOrEqual, greaterThanOrEqual, before, after, segmentMatch, semVerEqual, semVerLessThan, and semVerGreaterThan Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#op FeatureFlagEnvironment#op}
-        :param values: The list of values associated with the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
-        :param context_kind: The context kind associated with this rule clause. If omitted, defaults to user. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
-        :param negate: Whether to negate the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#negate FeatureFlagEnvironment#negate}
-        :param value_type: The type for each of the clause's values. Available types are boolean, string, and number. If omitted, value_type defaults to string Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#value_type FeatureFlagEnvironment#value_type}
+        :param attribute: The user attribute to operate on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#attribute FeatureFlagEnvironment#attribute}
+        :param op: The operator associated with the rule clause. Available options are in, endsWith, startsWith, matches, contains, lessThan, lessThanOrEqual, greaterThanOrEqual, before, after, segmentMatch, semVerEqual, semVerLessThan, and semVerGreaterThan Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#op FeatureFlagEnvironment#op}
+        :param values: The list of values associated with the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
+        :param context_kind: The context kind associated with this rule clause. If omitted, defaults to user. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
+        :param negate: Whether to negate the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#negate FeatureFlagEnvironment#negate}
+        :param value_type: The type for each of the clause's values. Available types are boolean, string, and number. If omitted, value_type defaults to string Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#value_type FeatureFlagEnvironment#value_type}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c3764dc1ebdf1737e8cb1806314d82ed5209be7d9cb0f28615542c981b19fcf3)
             check_type(argname="argument attribute", value=attribute, expected_type=type_hints["attribute"])
             check_type(argname="argument op", value=op, expected_type=type_hints["op"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
@@ -1556,69 +1556,69 @@
         if value_type is not None:
             self._values["value_type"] = value_type
 
     @builtins.property
     def attribute(self) -> builtins.str:
         '''The user attribute to operate on.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#attribute FeatureFlagEnvironment#attribute}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#attribute FeatureFlagEnvironment#attribute}
         '''
         result = self._values.get("attribute")
         assert result is not None, "Required property 'attribute' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def op(self) -> builtins.str:
         '''The operator associated with the rule clause.
 
         Available options are in, endsWith, startsWith, matches, contains, lessThan, lessThanOrEqual, greaterThanOrEqual, before, after, segmentMatch, semVerEqual, semVerLessThan, and semVerGreaterThan
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#op FeatureFlagEnvironment#op}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#op FeatureFlagEnvironment#op}
         '''
         result = self._values.get("op")
         assert result is not None, "Required property 'op' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''The list of values associated with the rule clause.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def context_kind(self) -> typing.Optional[builtins.str]:
         '''The context kind associated with this rule clause. If omitted, defaults to user.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#context_kind FeatureFlagEnvironment#context_kind}
         '''
         result = self._values.get("context_kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def negate(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether to negate the rule clause.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#negate FeatureFlagEnvironment#negate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#negate FeatureFlagEnvironment#negate}
         '''
         result = self._values.get("negate")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def value_type(self) -> typing.Optional[builtins.str]:
         '''The type for each of the clause's values.
 
         Available types are boolean, string, and number. If omitted, value_type defaults to string
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#value_type FeatureFlagEnvironment#value_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#value_type FeatureFlagEnvironment#value_type}
         '''
         result = self._values.get("value_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -2143,41 +2143,41 @@
     def __init__(
         self,
         *,
         values: typing.Sequence[builtins.str],
         variation: jsii.Number,
     ) -> None:
         '''
-        :param values: List of user strings to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
-        :param variation: Index of the variation to serve if a user_target is matched. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        :param values: List of user strings to target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
+        :param variation: Index of the variation to serve if a user_target is matched. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c72fbcaf4343839fe9804c08d329a29b09af1ba31b7c68d3c1dd452b24ef3b9e)
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
             check_type(argname="argument variation", value=variation, expected_type=type_hints["variation"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "values": values,
             "variation": variation,
         }
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''List of user strings to target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#values FeatureFlagEnvironment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def variation(self) -> jsii.Number:
         '''Index of the variation to serve if a user_target is matched.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/feature_flag_environment#variation FeatureFlagEnvironment#variation}
         '''
         result = self._values.get("variation")
         assert result is not None, "Required property 'variation' is missing"
         return typing.cast(jsii.Number, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/flag_trigger/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/flag_trigger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_flag_trigger`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_flag_trigger`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger).
+Refer to the Terraform Registory for docs: [`launchdarkly_flag_trigger`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class FlagTrigger(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.flagTrigger.FlagTrigger",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger launchdarkly_flag_trigger}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger launchdarkly_flag_trigger}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         enabled: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger launchdarkly_flag_trigger} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger launchdarkly_flag_trigger} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#enabled FlagTrigger#enabled}
-        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#env_key FlagTrigger#env_key}
-        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#flag_key FlagTrigger#flag_key}
-        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#instructions FlagTrigger#instructions}
-        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#integration_key FlagTrigger#integration_key}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#project_key FlagTrigger#project_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#id FlagTrigger#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#enabled FlagTrigger#enabled}
+        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#env_key FlagTrigger#env_key}
+        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#flag_key FlagTrigger#flag_key}
+        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#instructions FlagTrigger#instructions}
+        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#integration_key FlagTrigger#integration_key}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#project_key FlagTrigger#project_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#id FlagTrigger#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -89,15 +89,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putInstructions")
     def put_instructions(self, *, kind: builtins.str) -> None:
         '''
-        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#kind FlagTrigger#kind}
+        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#kind FlagTrigger#kind}
         '''
         value = FlagTriggerInstructions(kind=kind)
 
         return typing.cast(None, jsii.invoke(self, "putInstructions", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -283,21 +283,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#enabled FlagTrigger#enabled}
-        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#env_key FlagTrigger#env_key}
-        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#flag_key FlagTrigger#flag_key}
-        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#instructions FlagTrigger#instructions}
-        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#integration_key FlagTrigger#integration_key}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#project_key FlagTrigger#project_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#id FlagTrigger#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param enabled: Whether the trigger is currently active or not. This property defaults to true upon creation. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#enabled FlagTrigger#enabled}
+        :param env_key: The LaunchDarkly environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#env_key FlagTrigger#env_key}
+        :param flag_key: The key of the feature flag the trigger acts upon. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#flag_key FlagTrigger#flag_key}
+        :param instructions: instructions block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#instructions FlagTrigger#instructions}
+        :param integration_key: The unique identifier of the integration you intend to set your trigger up with. "generic-trigger" should be used for integrations not explicitly supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#integration_key FlagTrigger#integration_key}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#project_key FlagTrigger#project_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#id FlagTrigger#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(instructions, dict):
             instructions = FlagTriggerInstructions(**instructions)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9f039e9efaf534fc0f33df3e00c8730b5e945d57b2562f833b651905cca539a0)
@@ -404,75 +404,75 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def enabled(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
         '''Whether the trigger is currently active or not. This property defaults to true upon creation.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#enabled FlagTrigger#enabled}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#enabled FlagTrigger#enabled}
         '''
         result = self._values.get("enabled")
         assert result is not None, "Required property 'enabled' is missing"
         return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], result)
 
     @builtins.property
     def env_key(self) -> builtins.str:
         '''The LaunchDarkly environment key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#env_key FlagTrigger#env_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#env_key FlagTrigger#env_key}
         '''
         result = self._values.get("env_key")
         assert result is not None, "Required property 'env_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def flag_key(self) -> builtins.str:
         '''The key of the feature flag the trigger acts upon.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#flag_key FlagTrigger#flag_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#flag_key FlagTrigger#flag_key}
         '''
         result = self._values.get("flag_key")
         assert result is not None, "Required property 'flag_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def instructions(self) -> "FlagTriggerInstructions":
         '''instructions block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#instructions FlagTrigger#instructions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#instructions FlagTrigger#instructions}
         '''
         result = self._values.get("instructions")
         assert result is not None, "Required property 'instructions' is missing"
         return typing.cast("FlagTriggerInstructions", result)
 
     @builtins.property
     def integration_key(self) -> builtins.str:
         '''The unique identifier of the integration you intend to set your trigger up with.
 
         "generic-trigger" should be used for integrations not explicitly supported.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#integration_key FlagTrigger#integration_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#integration_key FlagTrigger#integration_key}
         '''
         result = self._values.get("integration_key")
         assert result is not None, "Required property 'integration_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The LaunchDarkly project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#project_key FlagTrigger#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#project_key FlagTrigger#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#id FlagTrigger#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#id FlagTrigger#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -492,28 +492,28 @@
     jsii_type="@cdktf/provider-launchdarkly.flagTrigger.FlagTriggerInstructions",
     jsii_struct_bases=[],
     name_mapping={"kind": "kind"},
 )
 class FlagTriggerInstructions:
     def __init__(self, *, kind: builtins.str) -> None:
         '''
-        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#kind FlagTrigger#kind}
+        :param kind: The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#kind FlagTrigger#kind}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ba70d50fd1e0e0d95e46d625c8ddbc57458fddb83adaef40237b6c7c0673be92)
             check_type(argname="argument kind", value=kind, expected_type=type_hints["kind"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "kind": kind,
         }
 
     @builtins.property
     def kind(self) -> builtins.str:
         '''The action to perform when triggering. Currently supported flag actions are "turnFlagOn" and "turnFlagOff".
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/flag_trigger#kind FlagTrigger#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/flag_trigger#kind FlagTrigger#kind}
         '''
         result = self._values.get("kind")
         assert result is not None, "Required property 'kind' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/metric/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/metric/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_metric`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_metric`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric).
+Refer to the Terraform Registory for docs: [`launchdarkly_metric`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Metric(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.metric.Metric",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric launchdarkly_metric}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric launchdarkly_metric}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -53,34 +53,34 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric launchdarkly_metric} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric launchdarkly_metric} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#key Metric#key}
-        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#kind Metric#kind}
-        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#name Metric#name}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#project_key Metric#project_key}
-        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#description Metric#description}
-        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#event_key Metric#event_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#id Metric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#is_active Metric#is_active}
-        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#is_numeric Metric#is_numeric}
-        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#maintainer_id Metric#maintainer_id}
-        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#randomization_units Metric#randomization_units}
-        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#selector Metric#selector}
-        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#success_criteria Metric#success_criteria}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#tags Metric#tags}
-        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#unit Metric#unit}
-        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#urls Metric#urls}
+        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#key Metric#key}
+        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#kind Metric#kind}
+        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#name Metric#name}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#project_key Metric#project_key}
+        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#description Metric#description}
+        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#event_key Metric#event_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#id Metric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#is_active Metric#is_active}
+        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#is_numeric Metric#is_numeric}
+        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#maintainer_id Metric#maintainer_id}
+        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#randomization_units Metric#randomization_units}
+        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#selector Metric#selector}
+        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#success_criteria Metric#success_criteria}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#tags Metric#tags}
+        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#unit Metric#unit}
+        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#urls Metric#urls}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -526,30 +526,30 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#key Metric#key}
-        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#kind Metric#kind}
-        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#name Metric#name}
-        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#project_key Metric#project_key}
-        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#description Metric#description}
-        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#event_key Metric#event_key}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#id Metric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#is_active Metric#is_active}
-        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#is_numeric Metric#is_numeric}
-        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#maintainer_id Metric#maintainer_id}
-        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#randomization_units Metric#randomization_units}
-        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#selector Metric#selector}
-        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#success_criteria Metric#success_criteria}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#tags Metric#tags}
-        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#unit Metric#unit}
-        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#urls Metric#urls}
+        :param key: A unique key that will be used to reference the metric in your code. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#key Metric#key}
+        :param kind: The metric type -available choices are 'pageview', 'click', and 'custom'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#kind Metric#kind}
+        :param name: A human-readable name for your metric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#name Metric#name}
+        :param project_key: The LaunchDarkly project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#project_key Metric#project_key}
+        :param description: A short description of what the metric will be used for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#description Metric#description}
+        :param event_key: The event key for your metric (if custom metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#event_key Metric#event_key}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#id Metric#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param is_active: Whether the metric is active. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#is_active Metric#is_active}
+        :param is_numeric: Whether the metric is numeric. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#is_numeric Metric#is_numeric}
+        :param maintainer_id: The LaunchDarkly ID of the user who will maintain the metric. If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#maintainer_id Metric#maintainer_id}
+        :param randomization_units: A set of one or more context kinds that this metric can measure events from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#randomization_units Metric#randomization_units}
+        :param selector: The CSS selector for your metric (if click metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#selector Metric#selector}
+        :param success_criteria: The success criteria for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#success_criteria Metric#success_criteria}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#tags Metric#tags}
+        :param unit: The unit for your metric (if numeric metric). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#unit Metric#unit}
+        :param urls: urls block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#urls Metric#urls}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__aa7cac13f5219f12a99cd83049cfcaff852eed75dcf965f55118e2d716bd2eda)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -683,163 +683,163 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''A unique key that will be used to reference the metric in your code.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#key Metric#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#key Metric#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def kind(self) -> builtins.str:
         '''The metric type -available choices are 'pageview', 'click', and 'custom'.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#kind Metric#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#kind Metric#kind}
         '''
         result = self._values.get("kind")
         assert result is not None, "Required property 'kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''A human-readable name for your metric.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#name Metric#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#name Metric#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The LaunchDarkly project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#project_key Metric#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#project_key Metric#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''A short description of what the metric will be used for.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#description Metric#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#description Metric#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def event_key(self) -> typing.Optional[builtins.str]:
         '''The event key for your metric (if custom metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#event_key Metric#event_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#event_key Metric#event_key}
         '''
         result = self._values.get("event_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#id Metric#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#id Metric#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def is_active(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether the metric is active.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#is_active Metric#is_active}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#is_active Metric#is_active}
         '''
         result = self._values.get("is_active")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def is_numeric(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether the metric is numeric.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#is_numeric Metric#is_numeric}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#is_numeric Metric#is_numeric}
         '''
         result = self._values.get("is_numeric")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def maintainer_id(self) -> typing.Optional[builtins.str]:
         '''The LaunchDarkly ID of the user who will maintain the metric.
 
         If not set, the API will automatically apply the member associated with your Terraform API key or the most recently-set maintainer
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#maintainer_id Metric#maintainer_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#maintainer_id Metric#maintainer_id}
         '''
         result = self._values.get("maintainer_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def randomization_units(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A set of one or more context kinds that this metric can measure events from.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#randomization_units Metric#randomization_units}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#randomization_units Metric#randomization_units}
         '''
         result = self._values.get("randomization_units")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def selector(self) -> typing.Optional[builtins.str]:
         '''The CSS selector for your metric (if click metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#selector Metric#selector}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#selector Metric#selector}
         '''
         result = self._values.get("selector")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def success_criteria(self) -> typing.Optional[builtins.str]:
         '''The success criteria for your metric (if numeric metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#success_criteria Metric#success_criteria}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#success_criteria Metric#success_criteria}
         '''
         result = self._values.get("success_criteria")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#tags Metric#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#tags Metric#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def unit(self) -> typing.Optional[builtins.str]:
         '''The unit for your metric (if numeric metric).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#unit Metric#unit}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#unit Metric#unit}
         '''
         result = self._values.get("unit")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def urls(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["MetricUrls"]]]:
         '''urls block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#urls Metric#urls}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#urls Metric#urls}
         '''
         result = self._values.get("urls")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["MetricUrls"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -868,18 +868,18 @@
         *,
         kind: builtins.str,
         pattern: typing.Optional[builtins.str] = None,
         substring: typing.Optional[builtins.str] = None,
         url: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param kind: The url type - available choices are 'exact', 'canonical', 'substring' and 'regex'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#kind Metric#kind}
-        :param pattern: The URL-matching regex. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#pattern Metric#pattern}
-        :param substring: The URL substring. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#substring Metric#substring}
-        :param url: The exact or canonical URL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#url Metric#url}
+        :param kind: The url type - available choices are 'exact', 'canonical', 'substring' and 'regex'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#kind Metric#kind}
+        :param pattern: The URL-matching regex. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#pattern Metric#pattern}
+        :param substring: The URL substring. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#substring Metric#substring}
+        :param url: The exact or canonical URL. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#url Metric#url}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__941ff69f5b9f18fc592a8e5b1561eb5a1ba864e6cf32bab45cb6df1623b19842)
             check_type(argname="argument kind", value=kind, expected_type=type_hints["kind"])
             check_type(argname="argument pattern", value=pattern, expected_type=type_hints["pattern"])
             check_type(argname="argument substring", value=substring, expected_type=type_hints["substring"])
             check_type(argname="argument url", value=url, expected_type=type_hints["url"])
@@ -893,43 +893,43 @@
         if url is not None:
             self._values["url"] = url
 
     @builtins.property
     def kind(self) -> builtins.str:
         '''The url type - available choices are 'exact', 'canonical', 'substring' and 'regex'.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#kind Metric#kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#kind Metric#kind}
         '''
         result = self._values.get("kind")
         assert result is not None, "Required property 'kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def pattern(self) -> typing.Optional[builtins.str]:
         '''The URL-matching regex.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#pattern Metric#pattern}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#pattern Metric#pattern}
         '''
         result = self._values.get("pattern")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def substring(self) -> typing.Optional[builtins.str]:
         '''The URL substring.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#substring Metric#substring}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#substring Metric#substring}
         '''
         result = self._values.get("substring")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def url(self) -> typing.Optional[builtins.str]:
         '''The exact or canonical URL.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/metric#url Metric#url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/metric#url Metric#url}
         '''
         result = self._values.get("url")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/project/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/project/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_project`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_project`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project).
+Refer to the Terraform Registory for docs: [`launchdarkly_project`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Project(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.project.Project",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project launchdarkly_project}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project launchdarkly_project}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         environments: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ProjectEnvironments", typing.Dict[builtins.str, typing.Any]]]],
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project launchdarkly_project} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project launchdarkly_project} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param environments: environments block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#environments Project#environments}
-        :param key: The project's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#key Project#key}
-        :param name: A human-readable name for your project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#name Project#name}
-        :param default_client_side_availability: default_client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#default_client_side_availability Project#default_client_side_availability}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#id Project#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param include_in_snippet: Whether feature flags created under the project should be available to client-side SDKs by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#include_in_snippet Project#include_in_snippet}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#tags Project#tags}
+        :param environments: environments block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#environments Project#environments}
+        :param key: The project's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#key Project#key}
+        :param name: A human-readable name for your project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#name Project#name}
+        :param default_client_side_availability: default_client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#default_client_side_availability Project#default_client_side_availability}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#id Project#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param include_in_snippet: Whether feature flags created under the project should be available to client-side SDKs by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#include_in_snippet Project#include_in_snippet}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#tags Project#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -303,21 +303,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param environments: environments block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#environments Project#environments}
-        :param key: The project's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#key Project#key}
-        :param name: A human-readable name for your project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#name Project#name}
-        :param default_client_side_availability: default_client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#default_client_side_availability Project#default_client_side_availability}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#id Project#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param include_in_snippet: Whether feature flags created under the project should be available to client-side SDKs by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#include_in_snippet Project#include_in_snippet}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#tags Project#tags}
+        :param environments: environments block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#environments Project#environments}
+        :param key: The project's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#key Project#key}
+        :param name: A human-readable name for your project. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#name Project#name}
+        :param default_client_side_availability: default_client_side_availability block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#default_client_side_availability Project#default_client_side_availability}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#id Project#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param include_in_snippet: Whether feature flags created under the project should be available to client-side SDKs by default. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#include_in_snippet Project#include_in_snippet}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#tags Project#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8ae07973b215950e642bea0cd54fd02ef332024a996adeefa1d83b0c07431b53)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -427,77 +427,77 @@
 
     @builtins.property
     def environments(
         self,
     ) -> typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ProjectEnvironments"]]:
         '''environments block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#environments Project#environments}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#environments Project#environments}
         '''
         result = self._values.get("environments")
         assert result is not None, "Required property 'environments' is missing"
         return typing.cast(typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ProjectEnvironments"]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The project's unique key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#key Project#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#key Project#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''A human-readable name for your project.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#name Project#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#name Project#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def default_client_side_availability(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ProjectDefaultClientSideAvailability"]]]:
         '''default_client_side_availability block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#default_client_side_availability Project#default_client_side_availability}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#default_client_side_availability Project#default_client_side_availability}
         '''
         result = self._values.get("default_client_side_availability")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ProjectDefaultClientSideAvailability"]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#id Project#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#id Project#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def include_in_snippet(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether feature flags created under the project should be available to client-side SDKs by default.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#include_in_snippet Project#include_in_snippet}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#include_in_snippet Project#include_in_snippet}
         '''
         result = self._values.get("include_in_snippet")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#tags Project#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#tags Project#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -522,40 +522,40 @@
     def __init__(
         self,
         *,
         using_environment_id: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
         using_mobile_key: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
     ) -> None:
         '''
-        :param using_environment_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#using_environment_id Project#using_environment_id}.
-        :param using_mobile_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#using_mobile_key Project#using_mobile_key}.
+        :param using_environment_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#using_environment_id Project#using_environment_id}.
+        :param using_mobile_key: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#using_mobile_key Project#using_mobile_key}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c7874d920a1b7a98a3f26d393bb93580676cb36ccecceef747b568340945c93c)
             check_type(argname="argument using_environment_id", value=using_environment_id, expected_type=type_hints["using_environment_id"])
             check_type(argname="argument using_mobile_key", value=using_mobile_key, expected_type=type_hints["using_mobile_key"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "using_environment_id": using_environment_id,
             "using_mobile_key": using_mobile_key,
         }
 
     @builtins.property
     def using_environment_id(
         self,
     ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#using_environment_id Project#using_environment_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#using_environment_id Project#using_environment_id}.'''
         result = self._values.get("using_environment_id")
         assert result is not None, "Required property 'using_environment_id' is missing"
         return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], result)
 
     @builtins.property
     def using_mobile_key(
         self,
     ) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#using_mobile_key Project#using_mobile_key}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#using_mobile_key Project#using_mobile_key}.'''
         result = self._values.get("using_mobile_key")
         assert result is not None, "Required property 'using_mobile_key' is missing"
         return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -781,24 +781,24 @@
         default_track_events: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         default_ttl: typing.Optional[jsii.Number] = None,
         require_comments: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         secure_mode: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         tags: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param color: A color swatch (as an RGB hex value with no leading '#', e.g. C8C8C8). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#color Project#color}
-        :param key: A project-unique key for the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#key Project#key}
-        :param name: The name of the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#name Project#name}
-        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#approval_settings Project#approval_settings}
-        :param confirm_changes: Whether or not to require confirmation for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#confirm_changes Project#confirm_changes}
-        :param default_track_events: Whether or not to default to sending data export events for flags created in the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#default_track_events Project#default_track_events}
-        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#default_ttl Project#default_ttl}
-        :param require_comments: Whether or not to require comments for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#require_comments Project#require_comments}
-        :param secure_mode: Whether or not to use secure mode. Secure mode ensures a user of the client-side SDK cannot impersonate another user Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#secure_mode Project#secure_mode}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#tags Project#tags}
+        :param color: A color swatch (as an RGB hex value with no leading '#', e.g. C8C8C8). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#color Project#color}
+        :param key: A project-unique key for the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#key Project#key}
+        :param name: The name of the new environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#name Project#name}
+        :param approval_settings: approval_settings block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#approval_settings Project#approval_settings}
+        :param confirm_changes: Whether or not to require confirmation for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#confirm_changes Project#confirm_changes}
+        :param default_track_events: Whether or not to default to sending data export events for flags created in the environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#default_track_events Project#default_track_events}
+        :param default_ttl: The TTL for the environment. This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#default_ttl Project#default_ttl}
+        :param require_comments: Whether or not to require comments for flag and segment changes in this environment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#require_comments Project#require_comments}
+        :param secure_mode: Whether or not to use secure mode. Secure mode ensures a user of the client-side SDK cannot impersonate another user Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#secure_mode Project#secure_mode}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#tags Project#tags}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ac2ed1b079b68cb919a5a6db7a4c230b9465cd2b936b69294e4e02637b01c6c4)
             check_type(argname="argument color", value=color, expected_type=type_hints["color"])
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument approval_settings", value=approval_settings, expected_type=type_hints["approval_settings"])
@@ -828,113 +828,113 @@
         if tags is not None:
             self._values["tags"] = tags
 
     @builtins.property
     def color(self) -> builtins.str:
         '''A color swatch (as an RGB hex value with no leading '#', e.g. C8C8C8).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#color Project#color}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#color Project#color}
         '''
         result = self._values.get("color")
         assert result is not None, "Required property 'color' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''A project-unique key for the new environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#key Project#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#key Project#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the new environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#name Project#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#name Project#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def approval_settings(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ProjectEnvironmentsApprovalSettings"]]]:
         '''approval_settings block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#approval_settings Project#approval_settings}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#approval_settings Project#approval_settings}
         '''
         result = self._values.get("approval_settings")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ProjectEnvironmentsApprovalSettings"]]], result)
 
     @builtins.property
     def confirm_changes(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not to require confirmation for flag and segment changes in this environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#confirm_changes Project#confirm_changes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#confirm_changes Project#confirm_changes}
         '''
         result = self._values.get("confirm_changes")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def default_track_events(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not to default to sending data export events for flags created in the environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#default_track_events Project#default_track_events}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#default_track_events Project#default_track_events}
         '''
         result = self._values.get("default_track_events")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def default_ttl(self) -> typing.Optional[jsii.Number]:
         '''The TTL for the environment.
 
         This must be between 0 and 60 minutes. The TTL setting only applies to environments using the PHP SDK
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#default_ttl Project#default_ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#default_ttl Project#default_ttl}
         '''
         result = self._values.get("default_ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def require_comments(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not to require comments for flag and segment changes in this environment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#require_comments Project#require_comments}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#require_comments Project#require_comments}
         '''
         result = self._values.get("require_comments")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def secure_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not to use secure mode.
 
         Secure mode ensures a user of the client-side SDK cannot impersonate another user
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#secure_mode Project#secure_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#secure_mode Project#secure_mode}
         '''
         result = self._values.get("secure_mode")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#tags Project#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#tags Project#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -965,19 +965,19 @@
         can_apply_declined_changes: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         can_review_own_request: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         min_num_approvals: typing.Optional[jsii.Number] = None,
         required: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         required_approval_tags: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param can_apply_declined_changes: Whether changes can be applied as long as minNumApprovals is met, regardless of whether any reviewers have declined a request. Defaults to true Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#can_apply_declined_changes Project#can_apply_declined_changes}
-        :param can_review_own_request: Whether requesters can approve or decline their own request. They may always comment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#can_review_own_request Project#can_review_own_request}
-        :param min_num_approvals: The number of approvals required before an approval request can be applied. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#min_num_approvals Project#min_num_approvals}
-        :param required: Whether any changes to flags in this environment will require approval. You may only set required or requiredApprovalTags, not both. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#required Project#required}
-        :param required_approval_tags: An array of tags used to specify which flags with those tags require approval. You may only set requiredApprovalTags or required, not both. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#required_approval_tags Project#required_approval_tags}
+        :param can_apply_declined_changes: Whether changes can be applied as long as minNumApprovals is met, regardless of whether any reviewers have declined a request. Defaults to true Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#can_apply_declined_changes Project#can_apply_declined_changes}
+        :param can_review_own_request: Whether requesters can approve or decline their own request. They may always comment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#can_review_own_request Project#can_review_own_request}
+        :param min_num_approvals: The number of approvals required before an approval request can be applied. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#min_num_approvals Project#min_num_approvals}
+        :param required: Whether any changes to flags in this environment will require approval. You may only set required or requiredApprovalTags, not both. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#required Project#required}
+        :param required_approval_tags: An array of tags used to specify which flags with those tags require approval. You may only set requiredApprovalTags or required, not both. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#required_approval_tags Project#required_approval_tags}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7e0da4efd35c7e9a11f3765c4e842e83118be30fc18f2d3a933612b6d1f5eebf)
             check_type(argname="argument can_apply_declined_changes", value=can_apply_declined_changes, expected_type=type_hints["can_apply_declined_changes"])
             check_type(argname="argument can_review_own_request", value=can_review_own_request, expected_type=type_hints["can_review_own_request"])
             check_type(argname="argument min_num_approvals", value=min_num_approvals, expected_type=type_hints["min_num_approvals"])
             check_type(argname="argument required", value=required, expected_type=type_hints["required"])
@@ -998,59 +998,59 @@
     def can_apply_declined_changes(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether changes can be applied as long as minNumApprovals is met, regardless of whether any reviewers have declined a request.
 
         Defaults to true
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#can_apply_declined_changes Project#can_apply_declined_changes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#can_apply_declined_changes Project#can_apply_declined_changes}
         '''
         result = self._values.get("can_apply_declined_changes")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def can_review_own_request(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether requesters can approve or decline their own request. They may always comment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#can_review_own_request Project#can_review_own_request}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#can_review_own_request Project#can_review_own_request}
         '''
         result = self._values.get("can_review_own_request")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def min_num_approvals(self) -> typing.Optional[jsii.Number]:
         '''The number of approvals required before an approval request can be applied.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#min_num_approvals Project#min_num_approvals}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#min_num_approvals Project#min_num_approvals}
         '''
         result = self._values.get("min_num_approvals")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def required(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether any changes to flags in this environment will require approval.
 
         You may only set required or requiredApprovalTags, not both.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#required Project#required}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#required Project#required}
         '''
         result = self._values.get("required")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def required_approval_tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''An array of tags used to specify which flags with those tags require approval.
 
         You may only set requiredApprovalTags or required, not both.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/project#required_approval_tags Project#required_approval_tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/project#required_approval_tags Project#required_approval_tags}
         '''
         result = self._values.get("required_approval_tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/provider/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/provider/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`launchdarkly`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs).
+Refer to the Terraform Registory for docs: [`launchdarkly`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,34 +22,34 @@
 
 
 class LaunchdarklyProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.provider.LaunchdarklyProvider",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs launchdarkly}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs launchdarkly}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         access_token: typing.Optional[builtins.str] = None,
         alias: typing.Optional[builtins.str] = None,
         api_host: typing.Optional[builtins.str] = None,
         oauth_token: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs launchdarkly} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs launchdarkly} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param access_token: The LaunchDarkly API key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs#access_token LaunchdarklyProvider#access_token}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs#alias LaunchdarklyProvider#alias}
-        :param api_host: The LaunchDarkly host address, e.g. https://app.launchdarkly.com. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs#api_host LaunchdarklyProvider#api_host}
-        :param oauth_token: The LaunchDarkly OAuth token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs#oauth_token LaunchdarklyProvider#oauth_token}
+        :param access_token: The LaunchDarkly API key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs#access_token LaunchdarklyProvider#access_token}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs#alias LaunchdarklyProvider#alias}
+        :param api_host: The LaunchDarkly host address, e.g. https://app.launchdarkly.com. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs#api_host LaunchdarklyProvider#api_host}
+        :param oauth_token: The LaunchDarkly OAuth token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs#oauth_token LaunchdarklyProvider#oauth_token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__361329afd854bf518b4157de0781ee1d4b0e0a1ed34515261d7ac92f9008aa00)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = LaunchdarklyProviderConfig(
             access_token=access_token,
@@ -170,18 +170,18 @@
         *,
         access_token: typing.Optional[builtins.str] = None,
         alias: typing.Optional[builtins.str] = None,
         api_host: typing.Optional[builtins.str] = None,
         oauth_token: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param access_token: The LaunchDarkly API key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs#access_token LaunchdarklyProvider#access_token}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs#alias LaunchdarklyProvider#alias}
-        :param api_host: The LaunchDarkly host address, e.g. https://app.launchdarkly.com. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs#api_host LaunchdarklyProvider#api_host}
-        :param oauth_token: The LaunchDarkly OAuth token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs#oauth_token LaunchdarklyProvider#oauth_token}
+        :param access_token: The LaunchDarkly API key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs#access_token LaunchdarklyProvider#access_token}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs#alias LaunchdarklyProvider#alias}
+        :param api_host: The LaunchDarkly host address, e.g. https://app.launchdarkly.com. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs#api_host LaunchdarklyProvider#api_host}
+        :param oauth_token: The LaunchDarkly OAuth token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs#oauth_token LaunchdarklyProvider#oauth_token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__63a271634d8257ba9984a180dcb9f63b6327bde59eac52f68c8ec5802d84c5e8)
             check_type(argname="argument access_token", value=access_token, expected_type=type_hints["access_token"])
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument api_host", value=api_host, expected_type=type_hints["api_host"])
             check_type(argname="argument oauth_token", value=oauth_token, expected_type=type_hints["oauth_token"])
@@ -195,42 +195,42 @@
         if oauth_token is not None:
             self._values["oauth_token"] = oauth_token
 
     @builtins.property
     def access_token(self) -> typing.Optional[builtins.str]:
         '''The LaunchDarkly API key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs#access_token LaunchdarklyProvider#access_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs#access_token LaunchdarklyProvider#access_token}
         '''
         result = self._values.get("access_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs#alias LaunchdarklyProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs#alias LaunchdarklyProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def api_host(self) -> typing.Optional[builtins.str]:
         '''The LaunchDarkly host address, e.g. https://app.launchdarkly.com.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs#api_host LaunchdarklyProvider#api_host}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs#api_host LaunchdarklyProvider#api_host}
         '''
         result = self._values.get("api_host")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def oauth_token(self) -> typing.Optional[builtins.str]:
         '''The LaunchDarkly OAuth token.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs#oauth_token LaunchdarklyProvider#oauth_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs#oauth_token LaunchdarklyProvider#oauth_token}
         '''
         result = self._values.get("oauth_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/relay_proxy_configuration/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/relay_proxy_configuration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_relay_proxy_configuration`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_relay_proxy_configuration`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration).
+Refer to the Terraform Registory for docs: [`launchdarkly_relay_proxy_configuration`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class RelayProxyConfiguration(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.relayProxyConfiguration.RelayProxyConfiguration",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration launchdarkly_relay_proxy_configuration}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration launchdarkly_relay_proxy_configuration}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         name: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration launchdarkly_relay_proxy_configuration} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration launchdarkly_relay_proxy_configuration} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: A human-friendly name for the Relay Proxy configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#name RelayProxyConfiguration#name}
-        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#policy RelayProxyConfiguration#policy}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#id RelayProxyConfiguration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: A human-friendly name for the Relay Proxy configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#name RelayProxyConfiguration#name}
+        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#policy RelayProxyConfiguration#policy}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#id RelayProxyConfiguration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -196,17 +196,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: A human-friendly name for the Relay Proxy configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#name RelayProxyConfiguration#name}
-        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#policy RelayProxyConfiguration#policy}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#id RelayProxyConfiguration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: A human-friendly name for the Relay Proxy configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#name RelayProxyConfiguration#name}
+        :param policy: policy block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#policy RelayProxyConfiguration#policy}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#id RelayProxyConfiguration#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0a19f1f503f6b1f5ddbf46ca888b21aec2f7acd97e05b698fbf9dbe43f51df88)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -303,35 +303,35 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''A human-friendly name for the Relay Proxy configuration.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#name RelayProxyConfiguration#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#name RelayProxyConfiguration#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def policy(
         self,
     ) -> typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["RelayProxyConfigurationPolicy"]]:
         '''policy block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#policy RelayProxyConfiguration#policy}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#policy RelayProxyConfiguration#policy}
         '''
         result = self._values.get("policy")
         assert result is not None, "Required property 'policy' is missing"
         return typing.cast(typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["RelayProxyConfigurationPolicy"]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#id RelayProxyConfiguration#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#id RelayProxyConfiguration#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -365,19 +365,19 @@
         effect: builtins.str,
         actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
         resources: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#effect RelayProxyConfiguration#effect}.
-        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#actions RelayProxyConfiguration#actions}
-        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#not_actions RelayProxyConfiguration#not_actions}
-        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#not_resources RelayProxyConfiguration#not_resources}
-        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#resources RelayProxyConfiguration#resources}
+        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#effect RelayProxyConfiguration#effect}.
+        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#actions RelayProxyConfiguration#actions}
+        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#not_actions RelayProxyConfiguration#not_actions}
+        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#not_resources RelayProxyConfiguration#not_resources}
+        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#resources RelayProxyConfiguration#resources}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ce59738af437ef56ab261cdc60e9461286fbfe18e1bf4f4ae1d8288dcf85c147)
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument not_actions", value=not_actions, expected_type=type_hints["not_actions"])
             check_type(argname="argument not_resources", value=not_resources, expected_type=type_hints["not_resources"])
@@ -392,55 +392,55 @@
         if not_resources is not None:
             self._values["not_resources"] = not_resources
         if resources is not None:
             self._values["resources"] = resources
 
     @builtins.property
     def effect(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#effect RelayProxyConfiguration#effect}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#effect RelayProxyConfiguration#effect}.'''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''An action to perform on a resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#actions RelayProxyConfiguration#actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#actions RelayProxyConfiguration#actions}
         '''
         result = self._values.get("actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted actions will be those actions NOT in this list.
 
         The 'actions' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#not_actions RelayProxyConfiguration#not_actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#not_actions RelayProxyConfiguration#not_actions}
         '''
         result = self._values.get("not_actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted resources will be those resources NOT in this list.
 
         The 'resources' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#not_resources RelayProxyConfiguration#not_resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#not_resources RelayProxyConfiguration#not_resources}
         '''
         result = self._values.get("not_resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of LaunchDarkly resource specifiers.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/relay_proxy_configuration#resources RelayProxyConfiguration#resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/relay_proxy_configuration#resources RelayProxyConfiguration#resources}
         '''
         result = self._values.get("resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/segment/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/segment/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_segment`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_segment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment).
+Refer to the Terraform Registory for docs: [`launchdarkly_segment`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Segment(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.segment.Segment",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment launchdarkly_segment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment launchdarkly_segment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         env_key: builtins.str,
@@ -49,30 +49,30 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment launchdarkly_segment} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment launchdarkly_segment} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param env_key: The segment's environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#env_key Segment#env_key}
-        :param key: The unique key that references the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#key Segment#key}
-        :param name: The human-friendly name for the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#name Segment#name}
-        :param project_key: The segment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#project_key Segment#project_key}
-        :param description: The description of the segment's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#description Segment#description}
-        :param excluded: List of user keys excluded from the segment. To target on other context kinds, use the excluded_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#excluded Segment#excluded}
-        :param excluded_contexts: excluded_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#excluded_contexts Segment#excluded_contexts}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#id Segment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param included: List of user keys included in the segment. To target on other context kinds, use the included_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#included Segment#included}
-        :param included_contexts: included_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#included_contexts Segment#included_contexts}
-        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#rules Segment#rules}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#tags Segment#tags}
+        :param env_key: The segment's environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#env_key Segment#env_key}
+        :param key: The unique key that references the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#key Segment#key}
+        :param name: The human-friendly name for the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#name Segment#name}
+        :param project_key: The segment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#project_key Segment#project_key}
+        :param description: The description of the segment's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#description Segment#description}
+        :param excluded: List of user keys excluded from the segment. To target on other context kinds, use the excluded_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#excluded Segment#excluded}
+        :param excluded_contexts: excluded_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#excluded_contexts Segment#excluded_contexts}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#id Segment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param included: List of user keys included in the segment. To target on other context kinds, use the included_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#included Segment#included}
+        :param included_contexts: included_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#included_contexts Segment#included_contexts}
+        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#rules Segment#rules}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#tags Segment#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -433,26 +433,26 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param env_key: The segment's environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#env_key Segment#env_key}
-        :param key: The unique key that references the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#key Segment#key}
-        :param name: The human-friendly name for the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#name Segment#name}
-        :param project_key: The segment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#project_key Segment#project_key}
-        :param description: The description of the segment's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#description Segment#description}
-        :param excluded: List of user keys excluded from the segment. To target on other context kinds, use the excluded_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#excluded Segment#excluded}
-        :param excluded_contexts: excluded_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#excluded_contexts Segment#excluded_contexts}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#id Segment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param included: List of user keys included in the segment. To target on other context kinds, use the included_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#included Segment#included}
-        :param included_contexts: included_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#included_contexts Segment#included_contexts}
-        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#rules Segment#rules}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#tags Segment#tags}
+        :param env_key: The segment's environment key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#env_key Segment#env_key}
+        :param key: The unique key that references the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#key Segment#key}
+        :param name: The human-friendly name for the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#name Segment#name}
+        :param project_key: The segment's project key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#project_key Segment#project_key}
+        :param description: The description of the segment's purpose. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#description Segment#description}
+        :param excluded: List of user keys excluded from the segment. To target on other context kinds, use the excluded_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#excluded Segment#excluded}
+        :param excluded_contexts: excluded_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#excluded_contexts Segment#excluded_contexts}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#id Segment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param included: List of user keys included in the segment. To target on other context kinds, use the included_contexts block attribute. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#included Segment#included}
+        :param included_contexts: included_contexts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#included_contexts Segment#included_contexts}
+        :param rules: rules block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#rules Segment#rules}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#tags Segment#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ed6a1b3a85766111d2daacda6a12b49796357a0f41632344015ce3d5effeb417)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -574,125 +574,125 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def env_key(self) -> builtins.str:
         '''The segment's environment key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#env_key Segment#env_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#env_key Segment#env_key}
         '''
         result = self._values.get("env_key")
         assert result is not None, "Required property 'env_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The unique key that references the segment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#key Segment#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#key Segment#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The human-friendly name for the segment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#name Segment#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#name Segment#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def project_key(self) -> builtins.str:
         '''The segment's project key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#project_key Segment#project_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#project_key Segment#project_key}
         '''
         result = self._values.get("project_key")
         assert result is not None, "Required property 'project_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The description of the segment's purpose.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#description Segment#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#description Segment#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def excluded(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of user keys excluded from the segment. To target on other context kinds, use the excluded_contexts block attribute.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#excluded Segment#excluded}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#excluded Segment#excluded}
         '''
         result = self._values.get("excluded")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def excluded_contexts(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentExcludedContexts"]]]:
         '''excluded_contexts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#excluded_contexts Segment#excluded_contexts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#excluded_contexts Segment#excluded_contexts}
         '''
         result = self._values.get("excluded_contexts")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentExcludedContexts"]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#id Segment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#id Segment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def included(self) -> typing.Optional[typing.List[builtins.str]]:
         '''List of user keys included in the segment. To target on other context kinds, use the included_contexts block attribute.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#included Segment#included}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#included Segment#included}
         '''
         result = self._values.get("included")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def included_contexts(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentIncludedContexts"]]]:
         '''included_contexts block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#included_contexts Segment#included_contexts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#included_contexts Segment#included_contexts}
         '''
         result = self._values.get("included_contexts")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentIncludedContexts"]]], result)
 
     @builtins.property
     def rules(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentRules"]]]:
         '''rules block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#rules Segment#rules}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#rules Segment#rules}
         '''
         result = self._values.get("rules")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentRules"]]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#tags Segment#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#tags Segment#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -714,41 +714,41 @@
     def __init__(
         self,
         *,
         context_kind: builtins.str,
         values: typing.Sequence[builtins.str],
     ) -> None:
         '''
-        :param context_kind: The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#context_kind Segment#context_kind}
-        :param values: List of target object keys included in or excluded from the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#values Segment#values}
+        :param context_kind: The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#context_kind Segment#context_kind}
+        :param values: List of target object keys included in or excluded from the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#values Segment#values}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__28d6778735b2a7d16c2528dd49eb754dcee6d745bbd461138a998db1616f9b68)
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "context_kind": context_kind,
             "values": values,
         }
 
     @builtins.property
     def context_kind(self) -> builtins.str:
         '''The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#context_kind Segment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#context_kind Segment#context_kind}
         '''
         result = self._values.get("context_kind")
         assert result is not None, "Required property 'context_kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''List of target object keys included in or excluded from the segment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#values Segment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#values Segment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -939,41 +939,41 @@
     def __init__(
         self,
         *,
         context_kind: builtins.str,
         values: typing.Sequence[builtins.str],
     ) -> None:
         '''
-        :param context_kind: The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#context_kind Segment#context_kind}
-        :param values: List of target object keys included in or excluded from the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#values Segment#values}
+        :param context_kind: The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#context_kind Segment#context_kind}
+        :param values: List of target object keys included in or excluded from the segment. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#values Segment#values}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e25981c1c68a641a81bb8e7eb2bb2fd8444e6a3614ea2665574f3e24bb8f63f3)
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "context_kind": context_kind,
             "values": values,
         }
 
     @builtins.property
     def context_kind(self) -> builtins.str:
         '''The context kind associated with this segment target. To target on user contexts, use the included and excluded attributes.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#context_kind Segment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#context_kind Segment#context_kind}
         '''
         result = self._values.get("context_kind")
         assert result is not None, "Required property 'context_kind' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''List of target object keys included in or excluded from the segment.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#values Segment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#values Segment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1171,18 +1171,18 @@
         *,
         bucket_by: typing.Optional[builtins.str] = None,
         clauses: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["SegmentRulesClauses", typing.Dict[builtins.str, typing.Any]]]]] = None,
         rollout_context_kind: typing.Optional[builtins.str] = None,
         weight: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param bucket_by: The attribute by which to group users together. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#bucket_by Segment#bucket_by}
-        :param clauses: clauses block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#clauses Segment#clauses}
-        :param rollout_context_kind: The context kind associated with this segment rule. This argument is only valid if weight is also specified. If omitted, defaults to 'user' Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#rollout_context_kind Segment#rollout_context_kind}
-        :param weight: The integer weight of the rule (between 1 and 100000). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#weight Segment#weight}
+        :param bucket_by: The attribute by which to group users together. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#bucket_by Segment#bucket_by}
+        :param clauses: clauses block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#clauses Segment#clauses}
+        :param rollout_context_kind: The context kind associated with this segment rule. This argument is only valid if weight is also specified. If omitted, defaults to 'user' Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#rollout_context_kind Segment#rollout_context_kind}
+        :param weight: The integer weight of the rule (between 1 and 100000). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#weight Segment#weight}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0e16d3fe1514553328b2d7b966d78da4ae66991478e0688d26bf0bfb77386c3a)
             check_type(argname="argument bucket_by", value=bucket_by, expected_type=type_hints["bucket_by"])
             check_type(argname="argument clauses", value=clauses, expected_type=type_hints["clauses"])
             check_type(argname="argument rollout_context_kind", value=rollout_context_kind, expected_type=type_hints["rollout_context_kind"])
             check_type(argname="argument weight", value=weight, expected_type=type_hints["weight"])
@@ -1196,46 +1196,46 @@
         if weight is not None:
             self._values["weight"] = weight
 
     @builtins.property
     def bucket_by(self) -> typing.Optional[builtins.str]:
         '''The attribute by which to group users together.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#bucket_by Segment#bucket_by}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#bucket_by Segment#bucket_by}
         '''
         result = self._values.get("bucket_by")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def clauses(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentRulesClauses"]]]:
         '''clauses block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#clauses Segment#clauses}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#clauses Segment#clauses}
         '''
         result = self._values.get("clauses")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["SegmentRulesClauses"]]], result)
 
     @builtins.property
     def rollout_context_kind(self) -> typing.Optional[builtins.str]:
         '''The context kind associated with this segment rule.
 
         This argument is only valid if weight is also specified. If omitted, defaults to 'user'
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#rollout_context_kind Segment#rollout_context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#rollout_context_kind Segment#rollout_context_kind}
         '''
         result = self._values.get("rollout_context_kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def weight(self) -> typing.Optional[jsii.Number]:
         '''The integer weight of the rule (between 1 and 100000).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#weight Segment#weight}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#weight Segment#weight}
         '''
         result = self._values.get("weight")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1268,20 +1268,20 @@
         op: builtins.str,
         values: typing.Sequence[builtins.str],
         context_kind: typing.Optional[builtins.str] = None,
         negate: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         value_type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param attribute: The user attribute to operate on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#attribute Segment#attribute}
-        :param op: The operator associated with the rule clause. Available options are in, endsWith, startsWith, matches, contains, lessThan, lessThanOrEqual, greaterThanOrEqual, before, after, segmentMatch, semVerEqual, semVerLessThan, and semVerGreaterThan Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#op Segment#op}
-        :param values: The list of values associated with the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#values Segment#values}
-        :param context_kind: The context kind associated with this rule clause. If omitted, defaults to user. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#context_kind Segment#context_kind}
-        :param negate: Whether to negate the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#negate Segment#negate}
-        :param value_type: The type for each of the clause's values. Available types are boolean, string, and number. If omitted, value_type defaults to string Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#value_type Segment#value_type}
+        :param attribute: The user attribute to operate on. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#attribute Segment#attribute}
+        :param op: The operator associated with the rule clause. Available options are in, endsWith, startsWith, matches, contains, lessThan, lessThanOrEqual, greaterThanOrEqual, before, after, segmentMatch, semVerEqual, semVerLessThan, and semVerGreaterThan Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#op Segment#op}
+        :param values: The list of values associated with the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#values Segment#values}
+        :param context_kind: The context kind associated with this rule clause. If omitted, defaults to user. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#context_kind Segment#context_kind}
+        :param negate: Whether to negate the rule clause. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#negate Segment#negate}
+        :param value_type: The type for each of the clause's values. Available types are boolean, string, and number. If omitted, value_type defaults to string Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#value_type Segment#value_type}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7311c90332c47a9e3d1696d4575bebbeef73a3698887bf8aaab7fd21a18d62c3)
             check_type(argname="argument attribute", value=attribute, expected_type=type_hints["attribute"])
             check_type(argname="argument op", value=op, expected_type=type_hints["op"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
             check_type(argname="argument context_kind", value=context_kind, expected_type=type_hints["context_kind"])
@@ -1299,69 +1299,69 @@
         if value_type is not None:
             self._values["value_type"] = value_type
 
     @builtins.property
     def attribute(self) -> builtins.str:
         '''The user attribute to operate on.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#attribute Segment#attribute}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#attribute Segment#attribute}
         '''
         result = self._values.get("attribute")
         assert result is not None, "Required property 'attribute' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def op(self) -> builtins.str:
         '''The operator associated with the rule clause.
 
         Available options are in, endsWith, startsWith, matches, contains, lessThan, lessThanOrEqual, greaterThanOrEqual, before, after, segmentMatch, semVerEqual, semVerLessThan, and semVerGreaterThan
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#op Segment#op}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#op Segment#op}
         '''
         result = self._values.get("op")
         assert result is not None, "Required property 'op' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''The list of values associated with the rule clause.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#values Segment#values}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#values Segment#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def context_kind(self) -> typing.Optional[builtins.str]:
         '''The context kind associated with this rule clause. If omitted, defaults to user.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#context_kind Segment#context_kind}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#context_kind Segment#context_kind}
         '''
         result = self._values.get("context_kind")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def negate(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether to negate the rule clause.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#negate Segment#negate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#negate Segment#negate}
         '''
         result = self._values.get("negate")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def value_type(self) -> typing.Optional[builtins.str]:
         '''The type for each of the clause's values.
 
         Available types are boolean, string, and number. If omitted, value_type defaults to string
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/segment#value_type Segment#value_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/segment#value_type Segment#value_type}
         '''
         result = self._values.get("value_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/team/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/team/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_team`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_team`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team).
+Refer to the Terraform Registory for docs: [`launchdarkly_team`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Team(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.team.Team",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team launchdarkly_team}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team launchdarkly_team}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         key: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team launchdarkly_team} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team launchdarkly_team} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#key Team#key}
-        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#name Team#name}
-        :param custom_role_keys: A list of custom role keys for the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#custom_role_keys Team#custom_role_keys}
-        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#description Team#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#id Team#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param maintainers: A list of team maintainer IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#maintainers Team#maintainers}
-        :param member_ids: A list of team member IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#member_ids Team#member_ids}
+        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#key Team#key}
+        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#name Team#name}
+        :param custom_role_keys: A list of custom role keys for the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#custom_role_keys Team#custom_role_keys}
+        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#description Team#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#id Team#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param maintainers: A list of team maintainer IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#maintainers Team#maintainers}
+        :param member_ids: A list of team member IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#member_ids Team#member_ids}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -282,21 +282,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#key Team#key}
-        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#name Team#name}
-        :param custom_role_keys: A list of custom role keys for the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#custom_role_keys Team#custom_role_keys}
-        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#description Team#description}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#id Team#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param maintainers: A list of team maintainer IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#maintainers Team#maintainers}
-        :param member_ids: A list of team member IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#member_ids Team#member_ids}
+        :param key: The team's unique key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#key Team#key}
+        :param name: The team's human-readable name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#name Team#name}
+        :param custom_role_keys: A list of custom role keys for the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#custom_role_keys Team#custom_role_keys}
+        :param description: The team's description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#description Team#description}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#id Team#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param maintainers: A list of team maintainer IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#maintainers Team#maintainers}
+        :param member_ids: A list of team member IDs as strings. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#member_ids Team#member_ids}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9af27aa374696620d0758031d237c56fb5f86bc739a7a6c4ad6d9fb431f22917)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -405,72 +405,72 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def key(self) -> builtins.str:
         '''The team's unique key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#key Team#key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#key Team#key}
         '''
         result = self._values.get("key")
         assert result is not None, "Required property 'key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The team's human-readable name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#name Team#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#name Team#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def custom_role_keys(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of custom role keys for the team.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#custom_role_keys Team#custom_role_keys}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#custom_role_keys Team#custom_role_keys}
         '''
         result = self._values.get("custom_role_keys")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The team's description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#description Team#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#description Team#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#id Team#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#id Team#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def maintainers(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of team maintainer IDs as strings.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#maintainers Team#maintainers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#maintainers Team#maintainers}
         '''
         result = self._values.get("maintainers")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def member_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of team member IDs as strings.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team#member_ids Team#member_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team#member_ids Team#member_ids}
         '''
         result = self._values.get("member_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/team_member/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/team_member/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_team_member`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_team_member`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member).
+Refer to the Terraform Registory for docs: [`launchdarkly_team_member`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class TeamMember(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.teamMember.TeamMember",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member launchdarkly_team_member}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member launchdarkly_team_member}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         email: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member launchdarkly_team_member} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member launchdarkly_team_member} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param email: The team member's email address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#email TeamMember#email}
-        :param custom_roles: IDs or keys of custom roles. Team members must have either a role or custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#custom_roles TeamMember#custom_roles}
-        :param first_name: The team member's first name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#first_name TeamMember#first_name}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#id TeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param last_name: The team member's last name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#last_name TeamMember#last_name}
-        :param role: The team member's role. This must be reader, writer, admin, or no_access. Team members must have either a role or custom role Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#role TeamMember#role}
+        :param email: The team member's email address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#email TeamMember#email}
+        :param custom_roles: IDs or keys of custom roles. Team members must have either a role or custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#custom_roles TeamMember#custom_roles}
+        :param first_name: The team member's first name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#first_name TeamMember#first_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#id TeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param last_name: The team member's last name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#last_name TeamMember#last_name}
+        :param role: The team member's role. This must be reader, writer, admin, or no_access. Team members must have either a role or custom role Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#role TeamMember#role}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -260,20 +260,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param email: The team member's email address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#email TeamMember#email}
-        :param custom_roles: IDs or keys of custom roles. Team members must have either a role or custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#custom_roles TeamMember#custom_roles}
-        :param first_name: The team member's first name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#first_name TeamMember#first_name}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#id TeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param last_name: The team member's last name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#last_name TeamMember#last_name}
-        :param role: The team member's role. This must be reader, writer, admin, or no_access. Team members must have either a role or custom role Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#role TeamMember#role}
+        :param email: The team member's email address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#email TeamMember#email}
+        :param custom_roles: IDs or keys of custom roles. Team members must have either a role or custom role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#custom_roles TeamMember#custom_roles}
+        :param first_name: The team member's first name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#first_name TeamMember#first_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#id TeamMember#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param last_name: The team member's last name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#last_name TeamMember#last_name}
+        :param role: The team member's role. This must be reader, writer, admin, or no_access. Team members must have either a role or custom role Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#role TeamMember#role}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b534a86927249425d58d28a1f89f74621ad1937c60a2bb4e04e33f522e9edb38)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -380,64 +380,64 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def email(self) -> builtins.str:
         '''The team member's email address.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#email TeamMember#email}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#email TeamMember#email}
         '''
         result = self._values.get("email")
         assert result is not None, "Required property 'email' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def custom_roles(self) -> typing.Optional[typing.List[builtins.str]]:
         '''IDs or keys of custom roles. Team members must have either a role or custom role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#custom_roles TeamMember#custom_roles}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#custom_roles TeamMember#custom_roles}
         '''
         result = self._values.get("custom_roles")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def first_name(self) -> typing.Optional[builtins.str]:
         '''The team member's first name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#first_name TeamMember#first_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#first_name TeamMember#first_name}
         '''
         result = self._values.get("first_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#id TeamMember#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#id TeamMember#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def last_name(self) -> typing.Optional[builtins.str]:
         '''The team member's last name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#last_name TeamMember#last_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#last_name TeamMember#last_name}
         '''
         result = self._values.get("last_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def role(self) -> typing.Optional[builtins.str]:
         '''The team member's role.
 
         This must be reader, writer, admin, or no_access. Team members must have either a role or custom role
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_member#role TeamMember#role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_member#role TeamMember#role}
         '''
         result = self._values.get("role")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/team_role_mapping/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/team_role_mapping/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_team_role_mapping`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_team_role_mapping`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_role_mapping).
+Refer to the Terraform Registory for docs: [`launchdarkly_team_role_mapping`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_role_mapping).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class TeamRoleMapping(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.teamRoleMapping.TeamRoleMapping",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_role_mapping launchdarkly_team_role_mapping}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_role_mapping launchdarkly_team_role_mapping}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         custom_role_keys: typing.Sequence[builtins.str],
@@ -39,20 +39,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_role_mapping launchdarkly_team_role_mapping} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_role_mapping launchdarkly_team_role_mapping} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param custom_role_keys: A set of custom role keys to assign to the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_role_mapping#custom_role_keys TeamRoleMapping#custom_role_keys}
-        :param team_key: The LaunchDarkly team key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_role_mapping#team_key TeamRoleMapping#team_key}
+        :param custom_role_keys: A set of custom role keys to assign to the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_role_mapping#custom_role_keys TeamRoleMapping#custom_role_keys}
+        :param team_key: The LaunchDarkly team key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_role_mapping#team_key TeamRoleMapping#team_key}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -157,16 +157,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param custom_role_keys: A set of custom role keys to assign to the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_role_mapping#custom_role_keys TeamRoleMapping#custom_role_keys}
-        :param team_key: The LaunchDarkly team key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_role_mapping#team_key TeamRoleMapping#team_key}
+        :param custom_role_keys: A set of custom role keys to assign to the team. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_role_mapping#custom_role_keys TeamRoleMapping#custom_role_keys}
+        :param team_key: The LaunchDarkly team key. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_role_mapping#team_key TeamRoleMapping#team_key}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9147ec9b8844034fd9f3d58395a40af6381c81e08480e78ab70f8cc136547ea3)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -260,25 +260,25 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def custom_role_keys(self) -> typing.List[builtins.str]:
         '''A set of custom role keys to assign to the team.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_role_mapping#custom_role_keys TeamRoleMapping#custom_role_keys}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_role_mapping#custom_role_keys TeamRoleMapping#custom_role_keys}
         '''
         result = self._values.get("custom_role_keys")
         assert result is not None, "Required property 'custom_role_keys' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def team_key(self) -> builtins.str:
         '''The LaunchDarkly team key.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/team_role_mapping#team_key TeamRoleMapping#team_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/team_role_mapping#team_key TeamRoleMapping#team_key}
         '''
         result = self._values.get("team_key")
         assert result is not None, "Required property 'team_key' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly/webhook/__init__.py` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly/webhook/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `launchdarkly_webhook`
 
-Refer to the Terraform Registory for docs: [`launchdarkly_webhook`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook).
+Refer to the Terraform Registory for docs: [`launchdarkly_webhook`](https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Webhook(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-launchdarkly.webhook.Webhook",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook launchdarkly_webhook}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook launchdarkly_webhook}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         url: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook launchdarkly_webhook} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook launchdarkly_webhook} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param url: The URL of the remote webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#url Webhook#url}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#id Webhook#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#name Webhook#name}
-        :param on: Whether this webhook is enabled or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#on Webhook#on}
-        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#secret Webhook#secret}
-        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#statements Webhook#statements}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#tags Webhook#tags}
+        :param url: The URL of the remote webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#url Webhook#url}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#id Webhook#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#name Webhook#name}
+        :param on: Whether this webhook is enabled or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#on Webhook#on}
+        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#secret Webhook#secret}
+        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#statements Webhook#statements}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#tags Webhook#tags}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -299,21 +299,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param url: The URL of the remote webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#url Webhook#url}
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#id Webhook#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#name Webhook#name}
-        :param on: Whether this webhook is enabled or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#on Webhook#on}
-        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#secret Webhook#secret}
-        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#statements Webhook#statements}
-        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#tags Webhook#tags}
+        :param url: The URL of the remote webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#url Webhook#url}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#id Webhook#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param name: A human-readable name for your webhook. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#name Webhook#name}
+        :param on: Whether this webhook is enabled or not. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#on Webhook#on}
+        :param secret: If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#secret Webhook#secret}
+        :param statements: statements block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#statements Webhook#statements}
+        :param tags: Tags associated with your resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#tags Webhook#tags}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5c9e9a4f0e4faed0d39cbe1a077065dc1cbc3b6ddcf7bbe8cfa422156560bb7a)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -423,75 +423,75 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def url(self) -> builtins.str:
         '''The URL of the remote webhook.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#url Webhook#url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#url Webhook#url}
         '''
         result = self._values.get("url")
         assert result is not None, "Required property 'url' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#id Webhook#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#id Webhook#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''A human-readable name for your webhook.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#name Webhook#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#name Webhook#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def on(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether this webhook is enabled or not.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#on Webhook#on}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#on Webhook#on}
         '''
         result = self._values.get("on")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def secret(self) -> typing.Optional[builtins.str]:
         '''If sign is true, and the secret attribute is omitted, LaunchDarkly will automatically generate a secret for you.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#secret Webhook#secret}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#secret Webhook#secret}
         '''
         result = self._values.get("secret")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def statements(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["WebhookStatements"]]]:
         '''statements block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#statements Webhook#statements}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#statements Webhook#statements}
         '''
         result = self._values.get("statements")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["WebhookStatements"]]], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Tags associated with your resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#tags Webhook#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#tags Webhook#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -522,19 +522,19 @@
         effect: builtins.str,
         actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_actions: typing.Optional[typing.Sequence[builtins.str]] = None,
         not_resources: typing.Optional[typing.Sequence[builtins.str]] = None,
         resources: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> None:
         '''
-        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#effect Webhook#effect}.
-        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#actions Webhook#actions}
-        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#not_actions Webhook#not_actions}
-        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#not_resources Webhook#not_resources}
-        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#resources Webhook#resources}
+        :param effect: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#effect Webhook#effect}.
+        :param actions: An action to perform on a resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#actions Webhook#actions}
+        :param not_actions: Targeted actions will be those actions NOT in this list. The 'actions' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#not_actions Webhook#not_actions}
+        :param not_resources: Targeted resources will be those resources NOT in this list. The 'resources' field must be empty to use this field Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#not_resources Webhook#not_resources}
+        :param resources: A list of LaunchDarkly resource specifiers. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#resources Webhook#resources}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0e3266808ccabb579be833fba2bff85febd8cdca8c3a5bab6b83eef5b88c78d8)
             check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             check_type(argname="argument actions", value=actions, expected_type=type_hints["actions"])
             check_type(argname="argument not_actions", value=not_actions, expected_type=type_hints["not_actions"])
             check_type(argname="argument not_resources", value=not_resources, expected_type=type_hints["not_resources"])
@@ -549,55 +549,55 @@
         if not_resources is not None:
             self._values["not_resources"] = not_resources
         if resources is not None:
             self._values["resources"] = resources
 
     @builtins.property
     def effect(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#effect Webhook#effect}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#effect Webhook#effect}.'''
         result = self._values.get("effect")
         assert result is not None, "Required property 'effect' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''An action to perform on a resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#actions Webhook#actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#actions Webhook#actions}
         '''
         result = self._values.get("actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_actions(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted actions will be those actions NOT in this list.
 
         The 'actions' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#not_actions Webhook#not_actions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#not_actions Webhook#not_actions}
         '''
         result = self._values.get("not_actions")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def not_resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Targeted resources will be those resources NOT in this list.
 
         The 'resources' field must be empty to use this field
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#not_resources Webhook#not_resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#not_resources Webhook#not_resources}
         '''
         result = self._values.get("not_resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def resources(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of LaunchDarkly resource specifiers.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.2/docs/resources/webhook#resources Webhook#resources}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/launchdarkly/launchdarkly/2.13.3/docs/resources/webhook#resources Webhook#resources}
         '''
         result = self._values.get("resources")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/PKG-INFO` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-launchdarkly
-Version: 0.0.0
+Version: 1.0.0
 Summary: Prebuilt launchdarkly Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-launchdarkly.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-launchdarkly.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-launchdarkly-0.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-launchdarkly-1.0.0/src/cdktf_cdktf_provider_launchdarkly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_launchdarkly/py.typed
 src/cdktf_cdktf_provider_launchdarkly.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_launchdarkly.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_launchdarkly.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_launchdarkly.egg-info/requires.txt
 src/cdktf_cdktf_provider_launchdarkly.egg-info/top_level.txt
 src/cdktf_cdktf_provider_launchdarkly/_jsii/__init__.py
-src/cdktf_cdktf_provider_launchdarkly/_jsii/provider-launchdarkly@0.0.0.jsii.tgz
+src/cdktf_cdktf_provider_launchdarkly/_jsii/provider-launchdarkly@1.0.0.jsii.tgz
 src/cdktf_cdktf_provider_launchdarkly/access_token/__init__.py
 src/cdktf_cdktf_provider_launchdarkly/audit_log_subscription/__init__.py
 src/cdktf_cdktf_provider_launchdarkly/custom_role/__init__.py
 src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_audit_log_subscription/__init__.py
 src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_environment/__init__.py
 src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag/__init__.py
 src/cdktf_cdktf_provider_launchdarkly/data_launchdarkly_feature_flag_environment/__init__.py
```

