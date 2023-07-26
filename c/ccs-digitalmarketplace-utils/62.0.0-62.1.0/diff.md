# Comparing `tmp/ccs-digitalmarketplace-utils-62.0.0.tar.gz` & `tmp/ccs-digitalmarketplace-utils-62.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-utils-62.0.0.tar", last modified: Tue Jul 25 08:40:28 2023, max compression
+gzip compressed data, was "ccs-digitalmarketplace-utils-62.1.0.tar", last modified: Wed Jul 26 09:18:50 2023, max compression
```

## Comparing `ccs-digitalmarketplace-utils-62.0.0.tar` & `ccs-digitalmarketplace-utils-62.1.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:40:28.160717 ccs-digitalmarketplace-utils-62.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-25 08:40:28.160717 ccs-digitalmarketplace-utils-62.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:40:28.156716 ccs-digitalmarketplace-utils-62.0.0/ccs_digitalmarketplace_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-25 08:40:28.000000 ccs-digitalmarketplace-utils-62.0.0/ccs_digitalmarketplace_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-25 08:40:28.000000 ccs-digitalmarketplace-utils-62.0.0/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:40:28.000000 ccs-digitalmarketplace-utils-62.0.0/ccs_digitalmarketplace_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-25 08:40:28.000000 ccs-digitalmarketplace-utils-62.0.0/ccs_digitalmarketplace_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 08:40:28.000000 ccs-digitalmarketplace-utils-62.0.0/ccs_digitalmarketplace_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:40:28.156716 ccs-digitalmarketplace-utils-62.0.0/dmutils/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/asset_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/cloudfoundry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/cookie_probe.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/csv_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/direct_plus_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/dmp_so_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/documents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:40:28.160717 ccs-digitalmarketplace-utils-62.0.0/dmutils/email/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/email/dm_mailchimp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/email/dm_notify.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/email/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/email/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/email/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/email/user_account_email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/env_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:40:28.160717 ccs-digitalmarketplace-utils-62.0.0/dmutils/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/errors/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/errors/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/external.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/flask_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:40:28.160717 ccs-digitalmarketplace-utils-62.0.0/dmutils/forms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/forms/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/forms/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/forms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/forms/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/forms/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/jinja2_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/ods.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/proxy_fix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:40:28.160717 ccs-digitalmarketplace-utils-62.0.0/dmutils/repoutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/repoutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/request_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/service_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/dmutils/views.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:40:28.160717 ccs-digitalmarketplace-utils-62.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-25 08:40:17.000000 ccs-digitalmarketplace-utils-62.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:18:50.349897 ccs-digitalmarketplace-utils-62.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-26 09:18:50.349897 ccs-digitalmarketplace-utils-62.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:18:50.345897 ccs-digitalmarketplace-utils-62.1.0/ccs_digitalmarketplace_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-26 09:18:50.000000 ccs-digitalmarketplace-utils-62.1.0/ccs_digitalmarketplace_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-26 09:18:50.000000 ccs-digitalmarketplace-utils-62.1.0/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:18:50.000000 ccs-digitalmarketplace-utils-62.1.0/ccs_digitalmarketplace_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-26 09:18:50.000000 ccs-digitalmarketplace-utils-62.1.0/ccs_digitalmarketplace_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 09:18:50.000000 ccs-digitalmarketplace-utils-62.1.0/ccs_digitalmarketplace_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:18:50.349897 ccs-digitalmarketplace-utils-62.1.0/dmutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/asset_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/cloudfoundry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/cookie_probe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/csv_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/direct_plus_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/dmp_so_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/documents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:18:50.349897 ccs-digitalmarketplace-utils-62.1.0/dmutils/email/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/email/dm_mailchimp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/email/dm_notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/email/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/email/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/email/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/email/user_account_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/env_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:18:50.349897 ccs-digitalmarketplace-utils-62.1.0/dmutils/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/errors/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/errors/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/flask_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:18:50.349897 ccs-digitalmarketplace-utils-62.1.0/dmutils/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/forms/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/forms/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/forms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/forms/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/forms/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/jinja2_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/ods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/proxy_fix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:18:50.349897 ccs-digitalmarketplace-utils-62.1.0/dmutils/repoutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/repoutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/request_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/service_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/dmutils/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 09:18:50.349897 ccs-digitalmarketplace-utils-62.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-26 09:18:38.000000 ccs-digitalmarketplace-utils-62.1.0/setup.py
```

### Comparing `ccs-digitalmarketplace-utils-62.0.0/LICENCE` & `ccs-digitalmarketplace-utils-62.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/README.md` & `ccs-digitalmarketplace-utils-62.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt` & `ccs-digitalmarketplace-utils-62.1.0/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/access_control.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/access_control.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/asset_fingerprint.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/asset_fingerprint.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/authentication.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/authentication.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/cloudfoundry.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/cloudfoundry.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/config.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/config.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/cookie_probe.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/cookie_probe.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/csv_generator.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/csv_generator.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/dates.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/dates.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/deprecation.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/deprecation.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/direct_plus_client.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/direct_plus_client.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/documents.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/documents.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/email/dm_mailchimp.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/email/dm_mailchimp.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/email/dm_notify.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/email/dm_notify.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/email/helpers.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/email/helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/email/tokens.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/email/tokens.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/email/user_account_email.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/email/user_account_email.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/env_helpers.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/env_helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/errors/api.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/errors/api.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/errors/frontend.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/errors/frontend.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/external.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/external.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/feature_flag.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/feature_flag.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/filters.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/filters.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/flask.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/flask.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/flask_init.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/flask_init.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/formats.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/formats.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/forms/errors.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/forms/errors.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/forms/fields.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/forms/fields.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/forms/helpers.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/forms/helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/forms/mixins.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/forms/mixins.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/forms/validators.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/forms/validators.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/forms/widgets.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/jinja2_environment.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/jinja2_environment.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/logging.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/logging.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/metrics.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/metrics.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/ods.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/ods.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/proxy_fix.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/proxy_fix.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/request_id.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/request_id.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/s3.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/s3.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/service_attribute.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/service_attribute.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/session.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/session.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/status.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/status.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/timing.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/timing.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/urls.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/urls.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/user.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/user.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/dmutils/views.py` & `ccs-digitalmarketplace-utils-62.1.0/dmutils/views.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-62.0.0/setup.py` & `ccs-digitalmarketplace-utils-62.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,9 +42,9 @@
          'notifications-python-client>=5.7.1,<9.0.0',
          'odfpy>=1.3.6',
          'python-json-logger>=0.1.11,<3.0.0',
          'pytz',
          'unicodecsv>=0.14.1',
          'workdays>=1.4',
     ],
-    python_requires="~=3.8",
+    python_requires="~=3.9",
 )
```

