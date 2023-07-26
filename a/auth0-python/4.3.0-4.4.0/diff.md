# Comparing `tmp/auth0-python-4.3.0.tar.gz` & `tmp/auth0-python-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth0-python-4.3.0.tar", last modified: Mon Jun 26 15:34:12 2023, max compression
+gzip compressed data, was "auth0-python-4.4.0.tar", last modified: Wed Jul 26 10:39:41 2023, max compression
```

## Comparing `auth0-python-4.3.0.tar` & `auth0-python-4.4.0.tar`

### file list

```diff
@@ -1,121 +1,122 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.106607 auth0-python-4.3.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1121 2023-06-26 15:34:11.000000 auth0-python-4.3.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-06-26 15:34:12.106607 auth0-python-4.3.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8039 2023-06-26 15:34:11.000000 auth0-python-4.3.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.094607 auth0-python-4.3.0/auth0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      169 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3138 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/asyncify.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.098607 auth0-python-4.3.0/auth0/authentication/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      408 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7385 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/async_token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2958 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2684 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/client_authentication.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3101 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/database.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1190 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/delegated.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      692 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/enterprise.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8511 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/get_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2397 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/passwordless.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      994 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/revoke_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1185 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/social.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16375 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1697 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/authentication/users.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      747 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/exceptions.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.102607 auth0-python-4.3.0/auth0/management/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1689 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7908 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/actions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1672 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/async_auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3762 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/attack_protection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3910 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2069 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/blacklists.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4670 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/branding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2818 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/client_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3447 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/client_grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5304 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/clients.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5716 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/connections.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2700 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/custom_domains.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3687 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/device_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2834 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/email_templates.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2831 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/emails.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2750 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5042 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/guardian.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5866 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/hooks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4551 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/jobs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2818 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/log_streams.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3742 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/logs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13772 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/organizations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2348 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/prompts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3473 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/resource_servers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7165 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/roles.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4877 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/rules.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2256 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/rules_configs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2039 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/stats.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2228 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/tenants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/tickets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2608 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/user_blocks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18274 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/users.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2048 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/management/users_by_email.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11953 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5710 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/rest_async.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.102607 auth0-python-4.3.0/auth0/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.102607 auth0-python-4.3.0/auth0/test/authentication/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11856 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2446 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_database.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2052 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_delegated.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      789 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_enterprise.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8743 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_get_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3038 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_passwordless.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      936 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_revoke_token.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1301 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_social.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    33387 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      433 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/authentication/test_users.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.106607 auth0-python-4.3.0/auth0/test/management/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8426 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_actions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3585 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_atack_protection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1578 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_blacklists.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4537 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_branding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1992 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_client_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3770 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_client_grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4428 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_clients.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6501 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_connections.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1989 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_custom_domains.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_device_credentials.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1674 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_email_endpoints.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_emails.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1449 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_grants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5181 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_guardian.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5649 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_hooks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3542 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_jobs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2781 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_log_streams.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1954 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_logs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15308 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_organizations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2168 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_prompts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2910 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_resource_servers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    30831 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_rest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6515 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_roles.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4115 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_rules.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1546 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_rules_configs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1364 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_stats.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1867 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_tenants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1236 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_tickets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_user_blocks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14460 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_users.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1398 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test/management/test_users_by_email.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.106607 auth0-python-4.3.0/auth0/test_async/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test_async/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2250 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test_async/test_async_auth0.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10099 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test_async/test_async_token_verifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7641 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/test_async/test_asyncify.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/types.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      186 2023-06-26 15:34:11.000000 auth0-python-4.3.0/auth0/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-26 15:34:12.106607 auth0-python-4.3.0/auth0_python.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-06-26 15:34:12.000000 auth0-python-4.3.0/auth0_python.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3765 2023-06-26 15:34:12.000000 auth0-python-4.3.0/auth0_python.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-26 15:34:12.000000 auth0-python-4.3.0/auth0_python.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2023-06-26 15:34:12.000000 auth0-python-4.3.0/auth0_python.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-06-26 15:34:12.000000 auth0-python-4.3.0/auth0_python.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-26 15:34:12.106607 auth0-python-4.3.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1454 2023-06-26 15:34:11.000000 auth0-python-4.3.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 10:39:41.943757 auth0-python-4.4.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1121 2023-07-26 10:39:41.000000 auth0-python-4.4.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-07-26 10:39:41.943757 auth0-python-4.4.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8039 2023-07-26 10:39:41.000000 auth0-python-4.4.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 10:39:41.931757 auth0-python-4.4.0/auth0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      169 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3620 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/asyncify.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 10:39:41.935757 auth0-python-4.4.0/auth0/authentication/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      408 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/authentication/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7416 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/authentication/async_token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2958 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/authentication/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2684 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/authentication/client_authentication.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3101 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/authentication/database.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1190 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/authentication/delegated.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      692 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/authentication/enterprise.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8511 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/authentication/get_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2397 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/authentication/passwordless.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      994 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/authentication/revoke_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1185 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/authentication/social.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17145 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/authentication/token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1696 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/authentication/users.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      747 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/exceptions.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 10:39:41.939757 auth0-python-4.4.0/auth0/management/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1717 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8741 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/actions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2067 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/async_auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4238 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/attack_protection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4096 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2414 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/blacklists.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5217 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/branding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3250 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/client_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3935 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/client_grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5907 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/clients.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6331 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/connections.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3131 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/custom_domains.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4151 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/device_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3245 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/email_templates.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3281 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/emails.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3209 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5627 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/guardian.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6529 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/hooks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5003 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/jobs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3276 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/log_streams.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4210 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/logs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15146 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/organizations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3108 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/prompts.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3995 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/resource_servers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8036 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/roles.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5445 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/rules.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2635 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/rules_configs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2418 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/stats.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2623 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/tenants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2267 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/tickets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/user_blocks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19741 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/users.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2420 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/management/users_by_email.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/py.typed
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11953 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5738 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/rest_async.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 10:39:41.939757 auth0-python-4.4.0/auth0/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 10:39:41.939757 auth0-python-4.4.0/auth0/test/authentication/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/authentication/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11856 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/authentication/test_base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2446 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/authentication/test_database.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2052 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/authentication/test_delegated.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      789 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/authentication/test_enterprise.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8743 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/authentication/test_get_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3038 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/authentication/test_passwordless.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      936 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/authentication/test_revoke_token.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1301 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/authentication/test_social.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    36028 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/authentication/test_token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      433 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/authentication/test_users.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 10:39:41.943757 auth0-python-4.4.0/auth0/test/management/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8426 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_actions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3585 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_atack_protection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1578 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_blacklists.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4537 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_branding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1992 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_client_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3770 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_client_grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4428 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_clients.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6501 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_connections.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1989 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_custom_domains.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2794 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_device_credentials.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1674 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_email_endpoints.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2271 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_emails.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1449 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_grants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5181 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_guardian.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5649 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_hooks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3542 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_jobs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2781 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_log_streams.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1954 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_logs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15308 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_organizations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2168 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_prompts.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2910 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_resource_servers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    30831 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_rest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6515 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_roles.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4115 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_rules.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1546 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_rules_configs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1364 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_stats.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1867 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_tenants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1236 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_tickets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_user_blocks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14460 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_users.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1398 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test/management/test_users_by_email.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 10:39:41.943757 auth0-python-4.4.0/auth0/test_async/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test_async/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2250 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test_async/test_async_auth0.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10099 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test_async/test_async_token_verifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8274 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/test_async/test_asyncify.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/types.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      186 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 10:39:41.943757 auth0-python-4.4.0/auth0_python.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8806 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0_python.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3780 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0_python.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0_python.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0_python.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-07-26 10:39:41.000000 auth0-python-4.4.0/auth0_python.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-07-26 10:39:41.943757 auth0-python-4.4.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1496 2023-07-26 10:39:41.000000 auth0-python-4.4.0/setup.py
```

### Comparing `auth0-python-4.3.0/LICENSE` & `auth0-python-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/PKG-INFO` & `auth0-python-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth0-python
-Version: 4.3.0
+Version: 4.4.0
 Summary: Auth0 Python SDK
 Home-page: https://github.com/auth0/auth0-python
 Author: Auth0
 Author-email: support@auth0.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auth0-python Version: 4.3.0 Summary: Auth0 Python
+Metadata-Version: 2.1 Name: auth0-python Version: 4.4.0 Summary: Auth0 Python
 SDK Home-page: https://github.com/auth0/auth0-python Author: Auth0 Author-
 email: support@auth0.com License: MIT Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `auth0-python-4.3.0/README.md` & `auth0-python-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/asyncify.py` & `auth0-python-4.4.0/auth0/asyncify.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import aiohttp
 
+from auth0.authentication import Users
 from auth0.authentication.base import AuthenticationBase
 from auth0.rest import RestClientOptions
 from auth0.rest_async import AsyncRestClient
 
 
 def _gen_async(client, method):
     m = getattr(client, method)
@@ -17,14 +18,25 @@
 def asyncify(cls):
     methods = [
         func
         for func in dir(cls)
         if callable(getattr(cls, func)) and not func.startswith("_")
     ]
 
+    class UsersAsyncClient(cls):
+        def __init__(
+            self,
+            domain,
+            telemetry=True,
+            timeout=5.0,
+            protocol="https",
+        ):
+            super().__init__(domain, telemetry, timeout, protocol)
+            self.client = AsyncRestClient(None, telemetry=telemetry, timeout=timeout)
+
     class AsyncManagementClient(cls):
         def __init__(
             self,
             domain,
             token,
             telemetry=True,
             timeout=5.0,
@@ -64,15 +76,17 @@
                     telemetry=telemetry, timeout=timeout, retries=0
                 ),
             )
 
     class Wrapper(cls):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
-            if AuthenticationBase in cls.__bases__:
+            if cls == Users:
+                self._async_client = UsersAsyncClient(*args, **kwargs)
+            elif AuthenticationBase in cls.__bases__:
                 self._async_client = AsyncAuthenticationClient(*args, **kwargs)
             else:
                 self._async_client = AsyncManagementClient(*args, **kwargs)
             for method in methods:
                 setattr(
                     self,
                     f"{method}_async",
```

### Comparing `auth0-python-4.3.0/auth0/authentication/async_token_verifier.py` & `auth0-python-4.4.0/auth0/authentication/async_token_verifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     ) -> dict[str, Any]:
         """Attempts to verify the given ID token, following the steps defined in the OpenID Connect spec.
 
         Args:
             token (str): The JWT to verify.
             nonce (str, optional): The nonce value sent during authentication.
             max_age (int, optional): The max_age value sent during authentication.
-            organization (str, optional): The expected organization ID (org_id) claim value. This should be specified
+            organization (str, optional): The expected organization ID (org_id) or orgnization name (org_name) claim value. This should be specified
             when logging in to an organization.
 
         Returns:
             the decoded payload from the token
 
         Raises:
             TokenValidationError: when the token cannot be decoded, the token signing algorithm is not the expected one,
```

### Comparing `auth0-python-4.3.0/auth0/authentication/base.py` & `auth0-python-4.4.0/auth0/authentication/base.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/authentication/client_authentication.py` & `auth0-python-4.4.0/auth0/authentication/client_authentication.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/authentication/database.py` & `auth0-python-4.4.0/auth0/authentication/database.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/authentication/delegated.py` & `auth0-python-4.4.0/auth0/authentication/delegated.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/authentication/enterprise.py` & `auth0-python-4.4.0/auth0/authentication/enterprise.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/authentication/get_token.py` & `auth0-python-4.4.0/auth0/authentication/get_token.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/authentication/passwordless.py` & `auth0-python-4.4.0/auth0/authentication/passwordless.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/authentication/revoke_token.py` & `auth0-python-4.4.0/auth0/authentication/revoke_token.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/authentication/social.py` & `auth0-python-4.4.0/auth0/authentication/social.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/authentication/token_verifier.py` & `auth0-python-4.4.0/auth0/authentication/token_verifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -295,15 +295,15 @@
     ) -> dict[str, Any]:
         """Attempts to verify the given ID token, following the steps defined in the OpenID Connect spec.
 
         Args:
             token (str): The JWT to verify.
             nonce (str, optional): The nonce value sent during authentication.
             max_age (int, optional): The max_age value sent during authentication.
-            organization (str, optional): The expected organization ID (org_id) claim value. This should be specified
+            organization (str, optional): The expected organization ID (org_id) or orgnization name (org_name) claim value. This should be specified
             when logging in to an organization.
 
         Returns:
             the decoded payload from the token
 
         Raises:
             TokenValidationError: when the token cannot be decoded, the token signing algorithm is not the expected one,
@@ -398,24 +398,38 @@
                 raise TokenValidationError(
                     'Nonce (nonce) claim mismatch in the ID token; expected "{}", '
                     'found "{}"'.format(nonce, payload["nonce"])
                 )
 
         # Organization
         if organization:
-            if "org_id" not in payload or not isinstance(payload["org_id"], str):
-                raise TokenValidationError(
-                    "Organization (org_id) claim must be a string present in the ID"
-                    " token"
-                )
-            if payload["org_id"] != organization:
-                raise TokenValidationError(
-                    "Organization (org_id) claim mismatch in the ID token; expected"
-                    ' "{}", found "{}"'.format(organization, payload["org_id"])
-                )
+            if organization.startswith("org_"):
+                if "org_id" not in payload or not isinstance(payload["org_id"], str):
+                    raise TokenValidationError(
+                        "Organization (org_id) claim must be a string present in the ID"
+                        " token"
+                    )
+                if payload["org_id"] != organization:
+                    raise TokenValidationError(
+                        "Organization (org_id) claim mismatch in the ID token; expected"
+                        ' "{}", found "{}"'.format(organization, payload["org_id"])
+                    )
+            else:
+                if "org_name" not in payload or not isinstance(
+                    payload["org_name"], str
+                ):
+                    raise TokenValidationError(
+                        "Organization (org_name) claim must be a string present in the ID"
+                        " token"
+                    )
+                if payload["org_name"] != organization.lower():
+                    raise TokenValidationError(
+                        "Organization (org_name) claim mismatch in the ID token; expected"
+                        ' "{}", found "{}"'.format(organization, payload["org_name"])
+                    )
 
         # Authorized party
         if isinstance(payload["aud"], list) and len(payload["aud"]) > 1:
             if "azp" not in payload or not isinstance(payload["azp"], str):
                 raise TokenValidationError(
                     "Authorized Party (azp) claim must be a string present in the ID"
                     " token when Audience (aud) claim has multiple values"
```

### Comparing `auth0-python-4.3.0/auth0/authentication/users.py` & `auth0-python-4.4.0/auth0/authentication/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,13 +42,12 @@
 
         Args:
             access_token (str): Auth0 access token (obtained during login).
 
         Returns:
             The user profile.
         """
-
         data: dict[str, Any] = self.client.get(
             url=f"{self.protocol}://{self.domain}/userinfo",
             headers={"Authorization": f"Bearer {access_token}"},
         )
         return data
```

### Comparing `auth0-python-4.3.0/auth0/exceptions.py` & `auth0-python-4.4.0/auth0/exceptions.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/management/__init__.py` & `auth0-python-4.4.0/auth0/management/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from .user_blocks import UserBlocks
 from .users import Users
 from .users_by_email import UsersByEmail
 
 if is_async_available():
     from .async_auth0 import AsyncAuth0 as Auth0
 else:  # pragma: no cover
-    from .auth0 import Auth0
+    from .auth0 import Auth0  # type: ignore[assignment]
 
 __all__ = (
     "Auth0",
     "Actions",
     "AttackProtection",
     "Blacklists",
     "Branding",
```

### Comparing `auth0-python-4.3.0/auth0/management/actions.py` & `auth0-python-4.4.0/auth0/management/actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Actions:
     """Auth0 Actions endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,51 +18,54 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
-        rest_options (RestClientOptions): Pass an instance of
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
+        rest_options (RestClientOptions, optional): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, *args):
+    def _url(self, *args: str | None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/actions"
         for p in args:
             if p is not None:
                 url = f"{url}/{p}"
         return url
 
     def get_actions(
         self,
-        trigger_id=None,
-        action_name=None,
-        deployed=None,
-        installed=False,
-        page=None,
-        per_page=None,
-    ):
+        trigger_id: str | None = None,
+        action_name: str | None = None,
+        deployed: bool | None = None,
+        installed: bool = False,
+        page: int | None = None,
+        per_page: int | None = None,
+    ) -> Any:
         """Get all actions.
 
         Args:
            trigger_id (str, optional): Filter the results to only actions associated
                  with this trigger ID.
 
            action_name (str, optional): Filter the results to only actions with this name.
@@ -73,101 +81,102 @@
 
            per_page (int, optional): The amount of entries per page. When not set,
                 the default value is up to the server.
 
         See: https://auth0.com/docs/api/management/v2#!/Actions/get_actions
         """
 
-        if deployed is not None:
-            deployed = str(deployed).lower()
+        deployed_str = str(deployed).lower() if deployed is not None else None
 
         params = {
             "triggerId": trigger_id,
             "actionName": action_name,
-            "deployed": deployed,
+            "deployed": deployed_str,
             "installed": str(installed).lower(),
             "page": page,
             "per_page": per_page,
         }
 
         return self.client.get(self._url("actions"), params=params)
 
-    def create_action(self, body):
+    def create_action(self, body: dict[str, Any]) -> dict[str, Any]:
         """Create a new action.
 
         Args:
            body (dict): Attributes for the new action.
 
         See: https://auth0.com/docs/api/management/v2#!/Actions/post_action
         """
 
         return self.client.post(self._url("actions"), data=body)
 
-    def update_action(self, id, body):
+    def update_action(self, id: str, body: dict[str, Any]) -> dict[str, Any]:
         """Updates an action.
 
         Args:
            id (str): the ID of the action.
 
            body (dict): Attributes to modify.
 
         See: https://auth0.com/docs/api/management/v2#!/Actions/patch_action
         """
 
         return self.client.patch(self._url("actions", id), data=body)
 
-    def get_action(self, id):
+    def get_action(self, id: str) -> dict[str, Any]:
         """Retrieves an action by its ID.
 
         Args:
            id (str): Id of action to retrieve.
 
         See: https://auth0.com/docs/api/management/v2#!/Actions/get_action
         """
         params = {}
 
         return self.client.get(self._url("actions", id), params=params)
 
-    def delete_action(self, id, force=False):
+    def delete_action(self, id: str, force: bool = False) -> Any:
         """Deletes an action and all of its associated versions.
 
         Args:
            id (str): ID of the action to delete.
 
            force (bool, optional): True to force action deletion detaching bindings,
                False otherwise. Defaults to False.
 
         See: https://auth0.com/docs/api/management/v2#!/Actions/delete_action
         """
         params = {"force": str(force).lower()}
 
         return self.client.delete(self._url("actions", id), params=params)
 
-    def get_triggers(self):
+    def get_triggers(self) -> dict[str, Any]:
         """Retrieve the set of triggers currently available within actions.
 
         See: https://auth0.com/docs/api/management/v2#!/Actions/get_triggers
         """
         params = {}
 
         return self.client.get(self._url("triggers"), params=params)
 
-    def get_execution(self, id):
+    def get_execution(self, id: str) -> dict[str, Any]:
         """Get information about a specific execution of a trigger.
 
         Args:
            id (str): The ID of the execution to retrieve.
 
         See: https://auth0.com/docs/api/management/v2#!/Actions/get_execution
         """
         params = {}
 
         return self.client.get(self._url("executions", id), params=params)
 
-    def get_action_versions(self, id, page=None, per_page=None):
+    def get_action_versions(
+        self, id: str, page: int | None = None, per_page: int | None = None
+    ) -> dict[str, Any]:
         """Get all of an action's versions.
 
         Args:
            id (str): The ID of the action.
 
            page (int, optional): The result's page number (zero based). When not set,
                 the default value is up to the server.
@@ -177,15 +186,17 @@
 
         See: https://auth0.com/docs/api/management/v2#!/Actions/get_action_versions
         """
         params = {"page": page, "per_page": per_page}
 
         return self.client.get(self._url("actions", id, "versions"), params=params)
 
-    def get_trigger_bindings(self, id, page=None, per_page=None):
+    def get_trigger_bindings(
+        self, id: str, page: int | None = None, per_page: int | None = None
+    ) -> dict[str, Any]:
         """Get the actions that are bound to a trigger.
 
         Args:
            id (str): The trigger ID.
 
            page (int, optional): The result's page number (zero based). When not set,
                 the default value is up to the server.
@@ -194,15 +205,15 @@
                 the default value is up to the server.
 
         See: https://auth0.com/docs/api/management/v2#!/Actions/get_bindings
         """
         params = {"page": page, "per_page": per_page}
         return self.client.get(self._url("triggers", id, "bindings"), params=params)
 
-    def get_action_version(self, action_id, version_id):
+    def get_action_version(self, action_id: str, version_id: str) -> dict[str, Any]:
         """Retrieve a specific version of an action.
 
         Args:
            action_id (str): The ID of the action.
 
            version_id (str): The ID of the version to retrieve.
 
@@ -210,39 +221,41 @@
         """
         params = {}
 
         return self.client.get(
             self._url("actions", action_id, "versions", version_id), params=params
         )
 
-    def deploy_action(self, id):
+    def deploy_action(self, id: str) -> dict[str, Any]:
         """Deploy an action.
 
         Args:
            id (str): The ID of the action to deploy.
 
         See: https://auth0.com/docs/api/management/v2#!/Actions/post_deploy_action
         """
         return self.client.post(self._url("actions", id, "deploy"))
 
-    def rollback_action_version(self, action_id, version_id):
+    def rollback_action_version(
+        self, action_id: str, version_id: str
+    ) -> dict[str, Any]:
         """Roll back to a previous version of an action.
 
         Args:
            action_id (str): The ID of the action.
 
            version_id (str): The ID of the version.
 
         See: https://auth0.com/docs/api/management/v2#!/Actions/post_deploy_draft_version
         """
         return self.client.post(
             self._url("actions", action_id, "versions", version_id, "deploy"), data={}
         )
 
-    def update_trigger_bindings(self, id, body):
+    def update_trigger_bindings(self, id: str, body: dict[str, Any]) -> dict[str, Any]:
         """Update a trigger's bindings.
 
         Args:
            id (str): The ID of the trigger to update.
 
            body (dict): Attributes for the updated trigger binding.
```

### Comparing `auth0-python-4.3.0/auth0/management/async_auth0.py` & `auth0-python-4.4.0/auth0/management/tickets.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,70 @@
-import aiohttp
+from __future__ import annotations
 
-from ..asyncify import asyncify
-from .auth0 import Auth0
+from typing import Any
 
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
-class AsyncAuth0:
-    """Provides easy access to all endpoint classes
+
+class Tickets:
+    """Auth0 tickets endpoints
 
     Args:
-        domain (str): Your Auth0 domain, for example 'username.auth0.com'
+        domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
 
         token (str): Management API v2 Token
 
+        telemetry (bool, optional): Enable or disable Telemetry
+            (defaults to True)
+
+        timeout (float or tuple, optional): Change the requests
+            connect and read timeout. Pass a tuple to specify
+            both values separately or a float to set both to it.
+            (defaults to 5.0 for both)
+
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
-    def __init__(self, domain, token, rest_options=None):
-        self._services = []
-        for name, attr in vars(Auth0(domain, token, rest_options=rest_options)).items():
-            cls = asyncify(attr.__class__)
-            service = cls(domain=domain, token=token, rest_options=rest_options)
-            self._services.append(service)
-            setattr(
-                self,
-                name,
-                service,
-            )
+    def __init__(
+        self,
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
+        self.domain = domain
+        self.protocol = protocol
+        self.client = RestClient(
+            jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
+        )
+
+    def _url(self, action: str) -> str:
+        return f"{self.protocol}://{self.domain}/api/v2/tickets/{action}"
 
-    def set_session(self, session):
-        """Set Client Session to improve performance by reusing session.
+    def create_email_verification(self, body: dict[str, Any]) -> dict[str, Any]:
+        """Create an email verification ticket.
 
         Args:
-            session (aiohttp.ClientSession): The client session which should be closed
-                manually or within context manager.
+            body (dict): attributes to set on the email verification request.
+
+        See: https://auth0.com/docs/api/v2#!/Tickets/post_email_verification
+        """
+        return self.client.post(self._url("email-verification"), data=body)
+
+    def create_pswd_change(self, body: dict[str, Any]) -> dict[str, Any]:
+        """Create password change ticket.
+
+        Args:
+            body (dict): attributes to set on the password change request.
+
+        See: https://auth0.com/docs/api/v2#!/Tickets/post_password_change
         """
-        self._session = session
-        for service in self._services:
-            service.set_session(self._session)
-
-    async def __aenter__(self):
-        """Automatically create and set session within context manager."""
-        self.set_session(aiohttp.ClientSession())
-        return self
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        """Automatically close session within context manager."""
-        await self._session.close()
+        return self.client.post(self._url("password-change"), data=body)
```

### Comparing `auth0-python-4.3.0/auth0/management/attack_protection.py` & `auth0-python-4.4.0/auth0/management/attack_protection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class AttackProtection:
     """Auth0 attack protection endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,99 +18,104 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, component):
+    def _url(self, component: str) -> str:
         return "{}://{}/api/v2/attack-protection/{}".format(
             self.protocol, self.domain, component
         )
 
-    def get_breached_password_detection(self):
+    def get_breached_password_detection(self) -> dict[str, Any]:
         """Get breached password detection settings.
 
         Returns the breached password detection settings.
 
         See: https://auth0.com/docs/api/management/v2#!/Attack_Protection/get_breached_password_detection
         """
         url = self._url("breached-password-detection")
         return self.client.get(url)
 
-    def update_breached_password_detection(self, body):
+    def update_breached_password_detection(
+        self, body: dict[str, Any]
+    ) -> dict[str, Any]:
         """Update breached password detection settings.
 
         Returns the breached password detection settings.
 
         Args:
 
            body (dict): breached password detection settings.
 
         See: https://auth0.com/docs/api/management/v2#!/Attack_Protection/patch_breached_password_detection
         """
         url = self._url("breached-password-detection")
         return self.client.patch(url, data=body)
 
-    def get_brute_force_protection(self):
+    def get_brute_force_protection(self) -> dict[str, Any]:
         """Get the brute force configuration.
 
         Returns the brute force configuration.
 
         See: https://auth0.com/docs/api/management/v2#!/Attack_Protection/get_brute_force_protection
         """
         url = self._url("brute-force-protection")
         return self.client.get(url)
 
-    def update_brute_force_protection(self, body):
+    def update_brute_force_protection(self, body: dict[str, Any]) -> dict[str, Any]:
         """Update the brute force configuration.
 
         Returns the brute force configuration.
 
         Args:
 
            body (dict): updates of the brute force configuration.
 
         See: https://auth0.com/docs/api/management/v2#!/Attack_Protection/patch_brute_force_protection
         """
         url = self._url("brute-force-protection")
         return self.client.patch(url, data=body)
 
-    def get_suspicious_ip_throttling(self):
+    def get_suspicious_ip_throttling(self) -> dict[str, Any]:
         """Get the suspicious IP throttling configuration.
 
         Returns the suspicious IP throttling configuration.
 
         See: https://auth0.com/docs/api/management/v2#!/Attack_Protection/get_suspicious_ip_throttling
         """
         url = self._url("suspicious-ip-throttling")
         return self.client.get(url)
 
-    def update_suspicious_ip_throttling(self, body):
+    def update_suspicious_ip_throttling(self, body: dict[str, Any]) -> dict[str, Any]:
         """Update the suspicious IP throttling configuration.
 
         Returns the suspicious IP throttling configuration.
 
         Args:
 
            body (dict): updates of the suspicious IP throttling configuration.
```

### Comparing `auth0-python-4.3.0/auth0/management/auth0.py` & `auth0-python-4.4.0/auth0/management/auth0.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from .actions import Actions
 from .attack_protection import AttackProtection
 from .blacklists import Blacklists
 from .branding import Branding
 from .client_credentials import ClientCredentials
 from .client_grants import ClientGrants
 from .clients import Clients
@@ -25,14 +29,17 @@
 from .stats import Stats
 from .tenants import Tenants
 from .tickets import Tickets
 from .user_blocks import UserBlocks
 from .users import Users
 from .users_by_email import UsersByEmail
 
+if TYPE_CHECKING:
+    from auth0.rest import RestClientOptions
+
 
 class Auth0:
     """Provides easy access to all endpoint classes
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
 
@@ -40,15 +47,17 @@
 
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
-    def __init__(self, domain, token, rest_options=None):
+    def __init__(
+        self, domain: str, token: str, rest_options: RestClientOptions | None = None
+    ):
         self.actions = Actions(domain, token, rest_options=rest_options)
         self.attack_protection = AttackProtection(
             domain, token, rest_options=rest_options
         )
         self.blacklists = Blacklists(domain, token, rest_options=rest_options)
         self.branding = Branding(domain, token, rest_options=rest_options)
         self.client_credentials = ClientCredentials(
```

### Comparing `auth0-python-4.3.0/auth0/management/blacklists.py` & `auth0-python-4.4.0/auth0/management/blacklists.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Blacklists:
     """Auth0 blacklists endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,50 +16,53 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.url = f"{protocol}://{domain}/api/v2/blacklists/tokens"
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def get(self, aud=None):
+    def get(self, aud: str | None = None) -> list[dict[str, str]]:
         """Retrieves the jti and aud of all tokens in the blacklist.
 
         Args:
             aud (str, optional): The JWT's aud claim. The client_id of the
                 application for which it was issued.
 
 
         See: https://auth0.com/docs/api/management/v2#!/Blacklists/get_tokens
         """
 
         params = {"aud": aud}
 
         return self.client.get(self.url, params=params)
 
-    def create(self, jti, aud=None):
+    def create(self, jti: str, aud: str | None = None) -> dict[str, str]:
         """Adds a token to the blacklist.
 
         Args:
             jti (str): the jti of the JWT to blacklist.
 
             aud (str, optional): The JWT's aud claim. The client_id of the
                 application for which it was issued.
```

### Comparing `auth0-python-4.3.0/auth0/management/branding.py` & `auth0-python-4.4.0/auth0/management/branding.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Branding:
     """Auth0 Branding endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,134 +18,139 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, *args):
+    def _url(self, *args: str) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/branding"
         for p in args:
             if p is not None:
                 url = f"{url}/{p}"
         return url
 
-    def get(self, aud=None):
+    def get(self) -> dict[str, Any]:
         """Retrieve branding settings. Requires "read:branding" scope.
 
         See: https://auth0.com/docs/api/management/v2#!/Branding/get_branding
         """
 
         return self.client.get(self._url())
 
-    def update(self, body):
+    def update(self, body: dict[str, Any]) -> dict[str, Any]:
         """Update branding settings. Requires "update:branding" scope.
 
         Args:
             body (dict): Attributes for the updated trigger binding.
 
         See: https://auth0.com/docs/api/management/v2#!/Branding/patch_branding
         """
 
         return self.client.patch(self._url(), data=body)
 
-    def get_template_universal_login(self):
+    def get_template_universal_login(self) -> dict[str, Any]:
         """Get template for New Universal Login Experience. Requires "read:branding" scope.
 
         See: https://auth0.com/docs/api/management/v2#!/Branding/get_universal_login
         """
 
         return self.client.get(self._url("templates", "universal-login"))
 
-    def delete_template_universal_login(self):
+    def delete_template_universal_login(self) -> Any:
         """Delete template for New Universal Login Experience. Requires "delete:branding" scope.
 
         See: https://auth0.com/docs/api/management/v2#!/Branding/delete_universal_login
         """
 
         return self.client.delete(self._url("templates", "universal-login"))
 
-    def update_template_universal_login(self, body):
+    def update_template_universal_login(self, body: dict[str, Any]) -> dict[str, Any]:
         """Update template for New Universal Login Experience. Requires "update:branding" scope.
 
         Args:
             body (str): Complete HTML content to assign to the template. See linked API documentation for example.
 
         See: https://auth0.com/docs/api/management/v2#!/Branding/put_universal_login
         """
 
         return self.client.put(
             self._url("templates", "universal-login"),
             data={"template": body},
         )
 
-    def get_default_branding_theme(self):
+    def get_default_branding_theme(self) -> dict[str, Any]:
         """Retrieve default branding theme.
 
         See: https://auth0.com/docs/api/management/v2#!/Branding/get_default_branding_theme
         """
 
         return self.client.get(self._url("themes", "default"))
 
-    def get_branding_theme(self, theme_id):
+    def get_branding_theme(self, theme_id: str) -> dict[str, Any]:
         """Retrieve branding theme.
 
         Args:
             theme_id (str): The theme_id to retrieve branding theme for.
 
         See: https://auth0.com/docs/api/management/v2#!/Branding/get_branding_theme
         """
 
         return self.client.get(self._url("themes", theme_id))
 
-    def delete_branding_theme(self, theme_id):
+    def delete_branding_theme(self, theme_id: str) -> Any:
         """Delete branding theme.
 
         Args:
             theme_id (str): The theme_id to delete branding theme for.
 
         See: https://auth0.com/docs/api/management/v2#!/Branding/delete_branding_theme
         """
 
         return self.client.delete(self._url("themes", theme_id))
 
-    def update_branding_theme(self, theme_id, body):
+    def update_branding_theme(
+        self, theme_id: str, body: dict[str, Any]
+    ) -> dict[str, Any]:
         """Update branding theme.
 
         Args:
             theme_id (str): The theme_id to update branding theme for.
             body (dict): The attributes to set on the theme.
 
         See: https://auth0.com/docs/api/management/v2#!/Branding/patch_branding_theme
         """
 
         return self.client.patch(self._url("themes", theme_id), data=body)
 
-    def create_branding_theme(self, body):
+    def create_branding_theme(self, body: dict[str, Any]) -> dict[str, Any]:
         """Create branding theme.
 
         Args:
             body (dict): The attributes to set on the theme.
 
         See: https://auth0.com/docs/api/management/v2#!/Branding/post_branding_theme
         """
```

### Comparing `auth0-python-4.3.0/auth0/management/client_credentials.py` & `auth0-python-4.4.0/auth0/management/log_streams.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,105 @@
-from ..rest import RestClient
+from __future__ import annotations
 
+from typing import Any
 
-class ClientCredentials:
-    """Auth0 client credentials endpoints.
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
+
+
+class LogStreams:
+    """Auth0 log streams endpoints
 
     Args:
-        domain (str): Your Auth0 domain, for example: 'my-domain.us.auth0.com'
+        domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
 
         token (str): Management API v2 Token
 
-        telemetry (bool, optional): Enable or disable telemetry
+        telemetry (bool, optional): Enable or disable Telemetry
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, client_id, id=None):
-        url = "{}://{}/api/v2/clients/{}/credentials".format(
-            self.protocol, self.domain, client_id
-        )
+    def _url(self, id: str | None = None) -> str:
+        url = f"{self.protocol}://{self.domain}/api/v2/log-streams"
         if id is not None:
             return f"{url}/{id}"
         return url
 
-    def all(self, client_id):
-        """Get a list of credentials associated with a client.
+    def list(self) -> list[dict[str, Any]]:
+        """Search log events.
 
         Args:
-            client_id (string): The id of a client that owns the credentials.
-
-        See: https://auth0.com/docs/api/management/v2#!/Client_Credentials/get_client_credentials
+        See: https://auth0.com/docs/api/management/v2/#!/Log_Streams/get_log_streams
         """
-        return self.client.get(self._url(client_id))
 
-    def get(self, client_id, id):
-        """Retrieve a specified client credential.
+        return self.client.get(self._url())
 
-        Args:
-            client_id (string): The id of a client that owns the credential.
+    def get(self, id: str) -> dict[str, Any]:
+        """Retrieves the data related to the log stream entry identified by id.
 
-            id (string): The id of the credential.
+        Args:
+            id (str): The id of the log stream to retrieve.
 
-        See: https://auth0.com/docs/api/management/v2#!/Client_Credentials/get_client_credentials_by_id
+        See: https://auth0.com/docs/api/management/v2/#!/Log_Streams/get_log_streams_by_id
         """
-        return self.client.get(self._url(client_id, id))
 
-    def create(self, client_id, body):
-        """Create a credential on a client.
+        return self.client.get(self._url(id))
+
+    def create(self, body: dict[str, Any]) -> dict[str, Any]:
+        """Creates a new log stream.
 
         Args:
-            client_id (string): The id of a client to create the credential for.
+            body (dict): the attributes for the role to create.
 
-        See: https://auth0.com/docs/api/management/v2#!/Client_Credentials/post_client_credentials
+        See: https://auth0.com/docs/api/management/v2/#!/Log_Streams/post_log_streams
         """
-        return self.client.post(self._url(client_id), data=body)
+        return self.client.post(self._url(), data=body)
 
-    def delete(self, client_id, id):
-        """Delete a client's credential.
+    def delete(self, id: str) -> dict[str, Any]:
+        """Delete a log stream.
 
         Args:
-           id (str): The id of credential to delete.
+            id (str): The id of the log ste to delete.
 
-        See: https://auth0.com/docs/api/management/v2#!/Client_Credentials/delete_client_credentials_by_id
+        See: https://auth0.com/docs/api/management/v2/#!/Log_Streams/delete_log_streams_by_id
         """
+        return self.client.delete(self._url(id))
+
+    def update(self, id: str, body: dict[str, Any]) -> dict[str, Any]:
+        """Update a log stream with the attributes passed in 'body'
+
+        Args:
+            id (str): The id of the log stream to update.
+
+            body (dict): the attributes to update on the log stream.
 
-        return self.client.delete(self._url(client_id, id))
+        See: https://auth0.com/docs/api/management/v2/#!/Log_Streams/patch_log_streams_by_id
+        """
+        return self.client.patch(self._url(id), data=body)
```

### Comparing `auth0-python-4.3.0/auth0/management/client_grants.py` & `auth0-python-4.4.0/auth0/management/client_grants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class ClientGrants:
     """Auth0 client grants endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,49 +18,52 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/client-grants"
         if id is not None:
             return f"{url}/{id}"
         return url
 
     def all(
         self,
-        audience=None,
-        page=None,
-        per_page=None,
-        include_totals=False,
-        client_id=None,
-    ):
+        audience: str | None = None,
+        page: int | None = None,
+        per_page: int | None = None,
+        include_totals: bool = False,
+        client_id: str | None = None,
+    ) -> list[dict[str, Any]]:
         """Retrieves all client grants.
 
         Args:
             audience (str, optional): URL encoded audience of a Resource Server
                 to filter.
 
             page (int, optional): The result's page number (zero based). When not set,
@@ -78,37 +86,37 @@
             "per_page": per_page,
             "include_totals": str(include_totals).lower(),
             "client_id": client_id,
         }
 
         return self.client.get(self._url(), params=params)
 
-    def create(self, body):
+    def create(self, body: dict[str, Any]) -> dict[str, Any]:
         """Creates a client grant.
 
         Args:
            body (dict): Attributes for the new client grant.
 
         See: https://auth0.com/docs/api/management/v2#!/Client_Grants/post_client_grants
         """
 
         return self.client.post(self._url(), data=body)
 
-    def delete(self, id):
+    def delete(self, id: str) -> Any:
         """Deletes a client grant.
 
         Args:
            id (str): Id of client grant to delete.
 
         See: https://auth0.com/docs/api/management/v2#!/Client_Grants/delete_client_grants_by_id
         """
 
         return self.client.delete(self._url(id))
 
-    def update(self, id, body):
+    def update(self, id: str, body: dict[str, Any]) -> dict[str, Any]:
         """Modifies a client grant.
 
         Args:
            id (str): The id of the client grant to modify.
 
            body (dict): Attributes to update.
```

### Comparing `auth0-python-4.3.0/auth0/management/clients.py` & `auth0-python-4.4.0/auth0/management/clients.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Clients:
     """Auth0 applications endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,63 +18,66 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/clients"
         if id is not None:
             return f"{url}/{id}"
         return url
 
     def all(
         self,
-        fields=None,
-        include_fields=True,
-        page=None,
-        per_page=None,
-        extra_params=None,
-    ):
+        fields: list[str] | None = None,
+        include_fields: bool = True,
+        page: int | None = None,
+        per_page: int | None = None,
+        extra_params: dict[str, Any] | None = None,
+    ) -> list[dict[str, Any]]:
         """Retrieves a list of all the applications.
 
         Important: The client_secret and encryption_key attributes can only be
         retrieved with the read:client_keys scope.
 
         Args:
            fields (list of str, optional): A list of fields to include or
               exclude from the result (depending on include_fields). Leave empty to
               retrieve all fields.
 
            include_fields (bool, optional): True if the fields specified are
               to be included in the result, False otherwise. Defaults to True.
 
-           page (int): The result's page number (zero based). When not set,
+           page (int, optional): The result's page number (zero based). When not set,
               the default value is up to the server.
 
            per_page (int, optional): The amount of entries per page. When not set,
               the default value is up to the server.
 
            extra_params (dictionary, optional): The extra parameters to add to
              the request. The fields, include_fields, page and per_page values
@@ -81,26 +89,28 @@
         params["fields"] = fields and ",".join(fields) or None
         params["include_fields"] = str(include_fields).lower()
         params["page"] = page
         params["per_page"] = per_page
 
         return self.client.get(self._url(), params=params)
 
-    def create(self, body):
+    def create(self, body: dict[str, Any]) -> dict[str, Any]:
         """Create a new application.
 
         Args:
            body (dict): Attributes for the new application.
 
         See: https://auth0.com/docs/api/v2#!/Clients/post_clients
         """
 
         return self.client.post(self._url(), data=body)
 
-    def get(self, id, fields=None, include_fields=True):
+    def get(
+        self, id: str, fields: list[str] | None = None, include_fields: bool = True
+    ) -> dict[str, Any]:
         """Retrieves an application by its id.
 
         Important: The client_secret, encryption_key and signing_keys
         attributes can only be retrieved with the read:client_keys scope.
 
         Args:
            id (str): Id of the application to get.
@@ -118,26 +128,26 @@
         params = {
             "fields": fields and ",".join(fields) or None,
             "include_fields": str(include_fields).lower(),
         }
 
         return self.client.get(self._url(id), params=params)
 
-    def delete(self, id):
+    def delete(self, id: str) -> Any:
         """Deletes an application and all its related assets.
 
         Args:
            id (str): Id of application to delete.
 
         See: https://auth0.com/docs/api/management/v2#!/Clients/delete_clients_by_id
         """
 
         return self.client.delete(self._url(id))
 
-    def update(self, id, body):
+    def update(self, id: str, body: dict[str, Any]) -> dict[str, Any]:
         """Modifies an application.
 
         Important: The client_secret, encryption_key and signing_keys
         attributes can only be updated with the update:client_keys scope.
 
         Args:
            id (str): Client ID of the application.
@@ -145,15 +155,15 @@
            body (dict): Attributes to modify.
 
         See: https://auth0.com/docs/api/management/v2#!/Clients/patch_clients_by_id
         """
 
         return self.client.patch(self._url(id), data=body)
 
-    def rotate_secret(self, id):
+    def rotate_secret(self, id: str) -> dict[str, Any]:
         """Rotate a client secret. The generated secret is NOT base64 encoded.
 
         Args:
            id (str): Client ID of the application.
 
         See: https://auth0.com/docs/api/management/v2#!/Clients/post_rotate_secret
         """
```

### Comparing `auth0-python-4.3.0/auth0/management/connections.py` & `auth0-python-4.4.0/auth0/management/connections.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Connections:
     """Auth0 connection endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,51 +18,54 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/connections"
         if id is not None:
             return f"{url}/{id}"
         return url
 
     def all(
         self,
-        strategy=None,
-        fields=None,
-        include_fields=True,
-        page=None,
-        per_page=None,
-        extra_params=None,
-        name=None,
-    ):
+        strategy: str | None = None,
+        fields: list[str] | None = None,
+        include_fields: bool = True,
+        page: int | None = None,
+        per_page: int | None = None,
+        extra_params: dict[str, Any] | None = None,
+        name: str | None = None,
+    ) -> list[dict[str, Any]]:
         """Retrieves all connections.
 
         Args:
            strategy (str, optional): Only retrieve connections of
               this strategy type. (e.g: strategy='amazon')
 
            fields (list of str, optional): A list of fields to include or
@@ -91,15 +99,17 @@
         params["include_fields"] = str(include_fields).lower()
         params["page"] = page
         params["per_page"] = per_page
         params["name"] = name
 
         return self.client.get(self._url(), params=params)
 
-    def get(self, id, fields=None, include_fields=True):
+    def get(
+        self, id: str, fields: list[str] | None = None, include_fields: bool = True
+    ) -> dict[str, Any]:
         """Retrieve connection by id.
 
         Args:
            id (str): Id of the connection to get.
 
            fields (list of str, optional): A list of fields to include or
               exclude from the result (depending on include_fields). Leave empty to
@@ -117,29 +127,29 @@
         params = {
             "fields": fields and ",".join(fields) or None,
             "include_fields": str(include_fields).lower(),
         }
 
         return self.client.get(self._url(id), params=params)
 
-    def delete(self, id):
+    def delete(self, id: str) -> Any:
         """Deletes a connection and all its users.
 
         Args:
            id: Id of the connection to delete.
 
         See: https://auth0.com/docs/api/management/v2#!/Connections/delete_connections_by_id
 
         Returns:
            An empty dict.
         """
 
         return self.client.delete(self._url(id))
 
-    def update(self, id, body):
+    def update(self, id: str, body: dict[str, Any]) -> dict[str, Any]:
         """Modifies a connection.
 
         Args:
            id: Id of the connection.
 
            body (dict): Specifies which fields are to be modified, and to what values.
 
@@ -147,27 +157,27 @@
 
         Returns:
            The modified connection object.
         """
 
         return self.client.patch(self._url(id), data=body)
 
-    def create(self, body):
+    def create(self, body: dict[str, Any]) -> dict[str, Any]:
         """Creates a new connection.
 
         Args:
             body (dict): Attributes used to create the connection. Mandatory
                 attributes are: 'name' and 'strategy'.
 
         See: https://auth0.com/docs/api/management/v2#!/Connections/post_connections
         """
 
         return self.client.post(self._url(), data=body)
 
-    def delete_user_by_email(self, id, email):
+    def delete_user_by_email(self, id: str, email: str) -> Any:
         """Deletes a specified connection user by its email.
 
         Args:
            id (str): The id of the connection (must be a database connection).
 
            email (str): The email of the user to delete.
```

### Comparing `auth0-python-4.3.0/auth0/management/custom_domains.py` & `auth0-python-4.4.0/auth0/management/custom_domains.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class CustomDomains:
     """Auth0 custom domains endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,78 +18,81 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/custom-domains"
         if id is not None:
             return url + "/" + id
         return url
 
-    def all(self):
+    def all(self) -> list[dict[str, Any]]:
         """Retrieves all custom domains.
 
         See: https://auth0.com/docs/api/management/v2#!/Custom_Domains/get_custom_domains
         """
         return self.client.get(self._url())
 
-    def get(self, id):
+    def get(self, id: str) -> dict[str, Any]:
         """Retrieves custom domain.
 
         See: https://auth0.com/docs/api/management/v2#!/Custom_Domains/get_custom_domains_by_id
         """
         url = self._url("%s" % (id))
         return self.client.get(url)
 
-    def delete(self, id):
+    def delete(self, id: str) -> Any:
         """Deletes a grant.
 
         Args:
            id (str): The id of the custom domain to delete.
 
         See: https://auth0.com/docs/api/management/v2#!/Custom_Domains/delete_custom_domains_by_id
         """
         url = self._url("%s" % (id))
         return self.client.delete(url)
 
-    def create_new(self, body):
+    def create_new(self, body: dict[str, Any]) -> dict[str, Any]:
         """Configure a new custom domain.
 
         Args:
            body (str): The domain, tye and verification method in json.
 
         See: https://auth0.com/docs/api/management/v2#!/Custom_Domains/post_custom_domains
         """
         return self.client.post(self._url(), data=body)
 
-    def verify(self, id):
+    def verify(self, id: str) -> dict[str, Any]:
         """Verify a custom domain.
 
         Args:
            id (str): The id of the custom domain to delete.
 
         See: https://auth0.com/docs/api/management/v2#!/Custom_Domains/post_verify
         """
```

### Comparing `auth0-python-4.3.0/auth0/management/device_credentials.py` & `auth0-python-4.4.0/auth0/management/device_credentials.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class DeviceCredentials:
     """Auth0 connection endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,52 +18,55 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/device-credentials"
         if id is not None:
             return f"{url}/{id}"
         return url
 
     def get(
         self,
-        user_id,
-        client_id,
-        type,
-        fields=None,
-        include_fields=True,
-        page=None,
-        per_page=None,
-        include_totals=False,
-    ):
+        user_id: str,
+        client_id: str,
+        type: str,
+        fields: list[str] | None = None,
+        include_fields: bool = True,
+        page: int | None = None,
+        per_page: int | None = None,
+        include_totals: bool = False,
+    ) -> list[dict[str, Any]]:
         """List device credentials.
 
         Args:
             user_id (str): The user_id of the devices to retrieve.
 
             client_id (str): The client_id of the devices to retrieve.
 
@@ -90,26 +98,26 @@
             "type": type,
             "page": page,
             "per_page": per_page,
             "include_totals": str(include_totals).lower(),
         }
         return self.client.get(self._url(), params=params)
 
-    def create(self, body):
+    def create(self, body: dict[str, Any]) -> dict[str, Any]:
         """Create a device public key.
 
         Args:
             body (dict): parameters for creating the public key (e.g: type,
                 device_name, client_id, etc).
 
         See: https://auth0.com/docs/api/v2#!/Device_Credentials/post_device_credentials
         """
         return self.client.post(self._url(), data=body)
 
-    def delete(self, id):
+    def delete(self, id: str) -> Any:
         """Delete credential.
 
         Args:
             id (str):  The id of the credential to delete.
 
         See: https://auth0.com/docs/api/management/v2#!/Device_Credentials/delete_device_credentials_by_id
         """
```

### Comparing `auth0-python-4.3.0/auth0/management/email_templates.py` & `auth0-python-4.4.0/auth0/management/email_templates.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class EmailTemplates:
     """Auth0 email templates endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,67 +18,70 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/email-templates"
         if id is not None:
             return f"{url}/{id}"
         return url
 
-    def create(self, body):
+    def create(self, body: dict[str, Any]) -> dict[str, Any]:
         """Create a new email template.
 
         Args:
            body (dict): Attributes for the new email template.
 
         See: https://auth0.com/docs/api/management/v2#!/Email_Templates/post_email_templates
         """
 
         return self.client.post(self._url(), data=body)
 
-    def get(self, template_name):
+    def get(self, template_name: str) -> dict[str, Any]:
         """Retrieves an email template by its name.
 
         Args:
            template_name (str): Name of the email template to get.
               Must be one of: 'verify_email', 'reset_email', 'welcome_email',
               'blocked_account', 'stolen_credentials', 'enrollment_email',
               'change_password', 'password_reset', 'mfa_oob_code'.
 
         See: https://auth0.com/docs/api/management/v2#!/Email_Templates/get_email_templates_by_templateName
         """
 
         return self.client.get(self._url(template_name))
 
-    def update(self, template_name, body):
+    def update(self, template_name: str, body: dict[str, Any]) -> dict[str, Any]:
         """Update an existing email template.
 
         Args:
            template_name (str): Name of the email template to update.
               Must be one of: 'verify_email', 'reset_email', 'welcome_email',
               'blocked_account', 'stolen_credentials', 'enrollment_email',
               'change_password', 'password_reset', 'mfa_oob_code'.
```

### Comparing `auth0-python-4.3.0/auth0/management/emails.py` & `auth0-python-4.4.0/auth0/management/emails.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Emails:
     """Auth0 email endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,42 +18,47 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/emails/provider"
         if id is not None:
             return f"{url}/{id}"
         return url
 
-    def get(self, fields=None, include_fields=True):
+    def get(
+        self, fields: list[str] | None = None, include_fields: bool = True
+    ) -> dict[str, Any]:
         """Get the email provider.
 
         Args:
             fields (list of str, optional): A list of fields to include or
                 exclude from the result (depending on include_fields). Leave empty to
                 retrieve all fields.
 
@@ -60,32 +70,32 @@
         params = {
             "fields": fields and ",".join(fields) or None,
             "include_fields": str(include_fields).lower(),
         }
 
         return self.client.get(self._url(), params=params)
 
-    def config(self, body):
+    def config(self, body: dict[str, Any]) -> dict[str, Any]:
         """Configure the email provider.
 
         Args:
             body (dict): attributes of the created email provider.
 
         See: https://auth0.com/docs/api/v2#!/Emails/post_provider
         """
         return self.client.post(self._url(), data=body)
 
-    def delete(self):
+    def delete(self) -> Any:
         """Delete the email provider. (USE WITH CAUTION)
 
         See: https://auth0.com/docs/api/management/v2#!/Emails/delete_provider
         """
         return self.client.delete(self._url())
 
-    def update(self, body):
+    def update(self, body: dict[str, Any]) -> dict[str, Any]:
         """Update the email provider.
 
         Args:
             body (dict): attributes to update on the email provider
 
         See: https://auth0.com/docs/api/v2#!/Emails/patch_provider
         """
```

### Comparing `auth0-python-4.3.0/auth0/management/grants.py` & `auth0-python-4.4.0/auth0/management/grants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Grants:
     """Auth0 grants endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,42 +18,51 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/grants"
         if id is not None:
             return url + "/" + id
         return url
 
-    def all(self, page=None, per_page=None, include_totals=False, extra_params=None):
+    def all(
+        self,
+        page: int | None = None,
+        per_page: int | None = None,
+        include_totals: bool = False,
+        extra_params: dict[str, Any] | None = None,
+    ) -> list[dict[str, Any]]:
         """Retrieves all grants.
 
         Args:
             page (int, optional): The result's page number (zero based). When not set,
                the default value is up to the server.
 
             per_page (int, optional): The amount of entries per page. When not set,
@@ -70,15 +84,15 @@
                 "per_page": per_page,
                 "include_totals": str(include_totals).lower(),
             }
         )
 
         return self.client.get(self._url(), params=params)
 
-    def delete(self, id):
+    def delete(self, id: str) -> Any:
         """Deletes a grant.
 
         Args:
            id (str): The id of the grant to delete.
 
         See: https://auth0.com/docs/api/management/v2#!/Grants/delete_grants_by_id
         """
```

### Comparing `auth0-python-4.3.0/auth0/management/guardian.py` & `auth0-python-4.4.0/auth0/management/guardian.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Guardian:
     """Auth0 guardian endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,127 +18,130 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/guardian"
         if id is not None:
             return f"{url}/{id}"
         return url
 
-    def all_factors(self):
+    def all_factors(self) -> list[dict[str, Any]]:
         """Retrieves all factors. Useful to check factor enablement and
              trial status.
 
         See: https://auth0.com/docs/api/management/v2#!/Guardian/get_factors
         """
 
         return self.client.get(self._url("factors"))
 
-    def update_factor(self, name, body):
+    def update_factor(self, name: str, body: dict[str, Any]) -> dict[str, Any]:
         """Update Guardian factor.
         Useful to enable / disable factor.
 
         Args:
             name (str): Either push-notification or sms.
 
             body (dict): Attributes to modify.
 
         See: https://auth0.com/docs/api/management/v2#!/Guardian/put_factors_by_name
         """
         url = self._url(f"factors/{name}")
         return self.client.put(url, data=body)
 
-    def update_templates(self, body):
+    def update_templates(self, body: dict[str, Any]) -> dict[str, Any]:
         """Update enrollment and verification SMS templates.
 
         Useful to send custom messages on sms enrollment and verification.
 
         Args:
             body (dict): Attributes to modify.
 
         See: https://auth0.com/docs/api/management/v2#!/Guardian/put_templates
         """
 
         return self.client.put(self._url("factors/sms/templates"), data=body)
 
-    def get_templates(self):
+    def get_templates(self) -> dict[str, Any]:
         """Get enrollment and verification templates.
 
         Retrieve both templates. Useful to check if a different template than
             default was set.
 
         See: https://auth0.com/docs/api/management/v2#!/Guardian/get_templates
         """
 
         return self.client.get(self._url("factors/sms/templates"))
 
-    def get_enrollment(self, id):
+    def get_enrollment(self, id: str) -> dict[str, Any]:
         """Retrieves an enrollment.
         Useful to check its type and related metadata.
 
         Args:
            id (str): The id of the device account to update.
 
         See: https://auth0.com/docs/api/management/v2#!/Guardian/get_enrollments_by_id
         """
         url = self._url(f"enrollments/{id}")
         return self.client.get(url)
 
-    def delete_enrollment(self, id):
+    def delete_enrollment(self, id: str) -> Any:
         """Deletes an enrollment.
 
         Useful when you want to force re-enroll.
 
         Args:
            id (str): The id of the device account to update.
 
         See: https://auth0.com/docs/api/management/v2#!/Guardian/delete_enrollments_by_id
         """
         url = self._url(f"enrollments/{id}")
         return self.client.delete(url)
 
-    def create_enrollment_ticket(self, body):
+    def create_enrollment_ticket(self, body: dict[str, Any]) -> dict[str, Any]:
         """Creates an enrollment ticket for user_id
 
         A useful way to send an email to a user, with a link that lead to
             start the enrollment process.
 
         Args:
             body (dict): Details of the user to send the ticket to.
 
         See: https://auth0.com/docs/api/management/v2#!/Guardian/post_ticket
         """
         return self.client.post(self._url("enrollments/ticket"), data=body)
 
-    def get_factor_providers(self, factor_name, name):
+    def get_factor_providers(self, factor_name: str, name: str) -> dict[str, Any]:
         """Get Guardian SNS or SMS factor providers.
 
         Returns provider configuration.
 
         Args:
            factor_name (str): Either push-notification or sms.
 
@@ -141,15 +149,17 @@
 
         See: https://auth0.com/docs/api/management/v2#!/Guardian/get_sns
              https://auth0.com/docs/api/management/v2#!/Guardian/get_twilio
         """
         url = self._url(f"factors/{factor_name}/providers/{name}")
         return self.client.get(url)
 
-    def update_factor_providers(self, factor_name, name, body):
+    def update_factor_providers(
+        self, factor_name: str, name: str, body: dict[str, Any]
+    ) -> dict[str, Any]:
         """Get Guardian factor providers.
 
         Returns provider configuration.
 
         Args:
            factor_name (str): Either push-notification or sms.
```

### Comparing `auth0-python-4.3.0/auth0/management/hooks.py` & `auth0-python-4.4.0/auth0/management/hooks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Hooks:
 
     """Hooks endpoint implementation.
 
     Args:
@@ -14,50 +19,53 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/hooks"
         if id is not None:
             return f"{url}/{id}"
         return url
 
     def all(
         self,
-        enabled=True,
-        fields=None,
-        include_fields=True,
-        page=None,
-        per_page=None,
-        include_totals=False,
-    ):
+        enabled: bool = True,
+        fields: list[str] | None = None,
+        include_fields: bool = True,
+        page: int | None = None,
+        per_page: int | None = None,
+        include_totals: bool = False,
+    ) -> list[dict[str, Any]]:
         """Retrieves a list of all hooks.
 
         Args:
             enabled (bool, optional): If provided, retrieves hooks that match
                 the value, otherwise all hooks are retrieved.
 
             fields (list, optional): A list of fields to include or exclude
@@ -88,24 +96,24 @@
 
         # since the default is True, this is here to disable the filter
         if enabled is not None:
             params["enabled"] = str(enabled).lower()
 
         return self.client.get(self._url(), params=params)
 
-    def create(self, body):
+    def create(self, body: dict[str, Any]) -> dict[str, Any]:
         """Creates a new Hook.
 
         Args:
             body (dict): Attributes for the newly created hook,
                 See: https://auth0.com/docs/api/v2#!/Hooks/post_hooks
         """
         return self.client.post(self._url(), data=body)
 
-    def get(self, id, fields=None):
+    def get(self, id: str, fields: list[str] | None = None) -> dict[str, Any]:
         """Retrieves a hook by its ID.
 
         Args:
             id (str): The id of the hook to retrieve.
 
             fields (list, optional): A list of fields to include or exclude
                 (depending on include_fields) from the result, empty to
@@ -114,72 +122,72 @@
         See: https://auth0.com/docs/api/management/v2#!/Hooks/get_hooks_by_id
         """
         params = {
             "fields": fields and ",".join(fields) or None,
         }
         return self.client.get(self._url(id), params=params)
 
-    def delete(self, id):
+    def delete(self, id: str) -> Any:
         """Deletes a hook.
 
         Args:
             id (str): The id of the hook to delete.
 
         See: https://auth0.com/docs/api/management/v2#!/Hooks/delete_hooks_by_id
         """
         return self.client.delete(self._url(id))
 
-    def update(self, id, body):
+    def update(self, id: str, body: dict[str, Any]) -> dict[str, Any]:
         """Updates an existing hook.
 
         Args:
             id (str): The id of the hook to modify.
 
             body (dict): Attributes to modify.
 
         See: https://auth0.com/docs/api/v2#!/Hooks/patch_hooks_by_id
         """
         return self.client.patch(self._url(id), data=body)
 
-    def get_secrets(self, id):
+    def get_secrets(self, id: str) -> dict[str, Any]:
         """Retrieves a hook's secrets.
 
         Args:
             id (str): The id of the hook to retrieve secrets from.
 
         See: https://auth0.com/docs/api/management/v2#!/Hooks/get_secrets
         """
 
         return self.client.get(self._url("%s/secrets" % id))
 
-    def add_secrets(self, id, body):
+    def add_secrets(self, id: str, body: dict[str, Any]) -> dict[str, Any]:
         """Add one or more secrets for an existing hook.
 
         Args:
             id (str): The id of the hook to add secrets to.
 
             body (dict): Dict of key-value pairs where the value must be a string.
 
         See: https://auth0.com/docs/api/management/v2#!/Hooks/post_secrets
         """
         return self.client.post(self._url("%s/secrets" % id), data=body)
 
-    def delete_secrets(self, id, body):
+    def delete_secrets(self, id: str, body: list[str]) -> Any:
         """Delete one or more existing secrets for an existing hook.
 
         Args:
             id (str): The id of the hook to add secrets to.
 
             body (list): List of secret names to delete.
 
         See: https://auth0.com/docs/api/management/v2#!/Hooks/delete_secrets
         """
         return self.client.delete(self._url("%s/secrets" % id), data=body)
 
-    def update_secrets(self, id, body):
+    def update_secrets(self, id: str, body: dict[str, Any]) -> dict[str, Any]:
         """Update one or more existing secrets for an existing hook.
 
         Args:
             id (str): The id of the hook to add secrets to.
 
             body (dict): Dict of key-value pairs where the value must be a string.
```

### Comparing `auth0-python-4.3.0/auth0/management/jobs.py` & `auth0-python-4.4.0/auth0/management/jobs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-import warnings
+from __future__ import annotations
 
-from ..rest import RestClient
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Jobs:
     """Auth0 jobs endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -15,83 +18,86 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, path=None):
+    def _url(self, path: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/jobs"
         if path is not None:
             return f"{url}/{path}"
         return url
 
-    def get(self, id):
+    def get(self, id: str) -> dict[str, Any]:
         """Retrieves a job. Useful to check its status.
 
         Args:
             id (str): The id of the job.
 
         See: https://auth0.com/docs/api/management/v2#!/Jobs/get_jobs_by_id
         """
         return self.client.get(self._url(id))
 
-    def get_failed_job(self, id):
+    def get_failed_job(self, id: str) -> dict[str, Any]:
         """Get failed job error details.
 
         Args:
             id (str): The id of the job.
 
         See: https://auth0.com/docs/api/management/v2#!/Jobs/get_errors
         """
         url = self._url(f"{id}/errors")
         return self.client.get(url)
 
-    def export_users(self, body):
+    def export_users(self, body: dict[str, Any]):
         """Export all users to a file using a long running job.
 
         Check job status with get(). URL pointing to the export file will be
         included in the status once the job is complete.
 
         Args:
             body (dict): The details of the export users request.
 
         See: https://auth0.com/docs/api/management/v2#!/Jobs/post_users_exports
         """
         return self.client.post(self._url("users-exports"), data=body)
 
     def import_users(
         self,
-        connection_id,
-        file_obj,
-        upsert=False,
-        send_completion_email=True,
-        external_id=None,
-    ):
+        connection_id: str,
+        file_obj: Any,
+        upsert: bool = False,
+        send_completion_email: bool = True,
+        external_id: str | None = None,
+    ) -> dict[str, Any]:
         """Imports users to a connection from a file.
 
         Args:
             connection_id (str): The connection id of the connection to which
                 users will be inserted.
 
             file_obj (file): A file-like object to upload. The format for
@@ -117,15 +123,15 @@
                 "upsert": str(upsert).lower(),
                 "send_completion_email": str(send_completion_email).lower(),
                 "external_id": external_id,
             },
             files={"users": file_obj},
         )
 
-    def send_verification_email(self, body):
+    def send_verification_email(self, body: dict[str, Any]) -> dict[str, Any]:
         """Send verification email.
 
         Send an email to the specified user that asks them to click a link to
         verify their email address.
 
         Args:
             body (dict): Details of verification email request.
```

### Comparing `auth0-python-4.3.0/auth0/management/log_streams.py` & `auth0-python-4.4.0/auth0/management/stats.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,79 @@
-from ..rest import RestClient
+from __future__ import annotations
 
+from typing import Any
 
-class LogStreams:
-    """Auth0 log streams endpoints
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
+
+
+class Stats:
+    """Auth0 stats endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
 
         token (str): Management API v2 Token
 
         telemetry (bool, optional): Enable or disable Telemetry
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
-        url = f"{self.protocol}://{self.domain}/api/v2/log-streams"
-        if id is not None:
-            return f"{url}/{id}"
-        return url
-
-    def list(self):
-        """Search log events.
-
-        Args:
-        See: https://auth0.com/docs/api/management/v2/#!/Log_Streams/get_log_streams
-        """
+    def _url(self, action: str) -> str:
+        return f"{self.protocol}://{self.domain}/api/v2/stats/{action}"
 
-        return self.client.get(self._url())
+    def active_users(self) -> int:
+        """Gets the active users count (logged in during the last 30 days).
 
-    def get(self, id):
-        """Retrieves the data related to the log stream entry identified by id.
+        Returns: An integer.
 
-        Args:
-            id (str): The id of the log stream to retrieve.
-
-        See: https://auth0.com/docs/api/management/v2/#!/Log_Streams/get_log_streams_by_id
+        See: https://auth0.com/docs/api/management/v2#!/Stats/get_active_users
         """
 
-        return self.client.get(self._url(id))
+        return self.client.get(self._url("active-users"))
 
-    def create(self, body):
-        """Creates a new log stream.
+    def daily_stats(
+        self, from_date: str | None = None, to_date: str | None = None
+    ) -> list[dict[str, Any]]:
+        """Gets the daily stats for a particular period.
 
         Args:
-            body (dict): the attributes for the role to create.
+           from_date (str, optional): The first day of the period (inclusive) in
+              YYYYMMDD format.
 
-        See: https://auth0.com/docs/api/management/v2/#!/Log_Streams/post_log_streams
-        """
-        return self.client.post(self._url(), data=body)
+           to_date (str, optional): The last day of the period (inclusive) in
+              YYYYMMDD format.
 
-    def delete(self, id):
-        """Delete a log stream.
-
-        Args:
-            id (str): The id of the log ste to delete.
-
-        See: https://auth0.com/docs/api/management/v2/#!/Log_Streams/delete_log_streams_by_id
+        See: https://auth0.com/docs/api/management/v2#!/Stats/get_daily
         """
-        return self.client.delete(self._url(id))
 
-    def update(self, id, body):
-        """Update a log stream with the attributes passed in 'body'
-
-        Args:
-            id (str): The id of the log stream to update.
-
-            body (dict): the attributes to update on the log stream.
-
-        See: https://auth0.com/docs/api/management/v2/#!/Log_Streams/patch_log_streams_by_id
-        """
-        return self.client.patch(self._url(id), data=body)
+        return self.client.get(
+            self._url("daily"), params={"from": from_date, "to": to_date}
+        )
```

### Comparing `auth0-python-4.3.0/auth0/management/logs.py` & `auth0-python-4.4.0/auth0/management/logs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Logs:
     """Auth0 logs endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,53 +18,56 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/logs"
         if id is not None:
             return f"{url}/{id}"
         return url
 
     def search(
         self,
-        page=0,
-        per_page=50,
-        sort=None,
-        q=None,
-        include_totals=True,
-        fields=None,
-        from_param=None,
-        take=None,
-        include_fields=True,
-    ):
+        page: int = 0,
+        per_page: int = 50,
+        sort: str | None = None,
+        q: str | None = None,
+        include_totals: bool = True,
+        fields: list[str] | None = None,
+        from_param: str | None = None,
+        take: int | None = None,
+        include_fields: bool = True,
+    ) -> list[dict[str, Any]]:
         """Search log events.
 
         Args:
             page (int, optional): The result's page number (zero based). By default,
                retrieves the first page of results.
 
             per_page (int, optional): The amount of entries per page. By default,
@@ -98,15 +106,15 @@
             "include_fields": str(include_fields).lower(),
             "q": q,
             "from": from_param,
             "take": take,
         }
         return self.client.get(self._url(), params=params)
 
-    def get(self, id):
+    def get(self, id: str) -> dict[str, Any]:
         """Retrieves the data related to the log entry identified by id.
 
         Args:
             id (str): The log_id of the log to retrieve.
 
         See: https://auth0.com/docs/api/management/v2#!/Logs/get_logs_by_id
         """
```

### Comparing `auth0-python-4.3.0/auth0/management/organizations.py` & `auth0-python-4.4.0/auth0/management/organizations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Organizations:
     """Auth0 organizations endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,46 +18,54 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, *args):
+    def _url(self, *args: str | None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/organizations"
         for p in args:
             if p is not None:
                 url = f"{url}/{p}"
         return url
 
     # Organizations
     def all_organizations(
-        self, page=None, per_page=None, include_totals=True, from_param=None, take=None
-    ):
+        self,
+        page: int | None = None,
+        per_page: int | None = None,
+        include_totals: bool = True,
+        from_param: str | None = None,
+        take: int | None = None,
+    ) -> list[dict[str, Any]]:
         """Retrieves a list of all the organizations.
 
         Args:
             page (int): The result's page number (zero based). When not set,
                 the default value is up to the server.
 
             per_page (int, optional): The amount of entries per page. When not set,
@@ -76,75 +89,77 @@
             "include_totals": str(include_totals).lower(),
             "from": from_param,
             "take": take,
         }
 
         return self.client.get(self._url(), params=params)
 
-    def get_organization_by_name(self, name=None):
+    def get_organization_by_name(self, name: str | None = None) -> dict[str, Any]:
         """Retrieves an organization given its name.
 
         Args:
            name (str): The name of the organization to retrieve.
 
         See: https://auth0.com/docs/api/management/v2#!/Organizations/get_name_by_name
         """
         params = {}
 
         return self.client.get(self._url("name", name), params=params)
 
-    def get_organization(self, id):
+    def get_organization(self, id: str) -> dict[str, Any]:
         """Retrieves an organization by its ID.
 
         Args:
            id (str): Id of organization to retrieve.
 
         See: https://auth0.com/docs/api/management/v2#!/Organizations/get_organizations_by_id
         """
         params = {}
 
         return self.client.get(self._url(id), params=params)
 
-    def create_organization(self, body):
+    def create_organization(self, body: dict[str, Any]) -> dict[str, Any]:
         """Create a new organization.
 
         Args:
            body (dict): Attributes for the new organization.
 
         See: https://auth0.com/docs/api/management/v2#!/Organizations/post_organizations
         """
 
         return self.client.post(self._url(), data=body)
 
-    def update_organization(self, id, body):
+    def update_organization(self, id: str, body: dict[str, Any]) -> dict[str, Any]:
         """Modifies an organization.
 
         Args:
            id (str): the ID of the organization.
 
            body (dict): Attributes to modify.
 
         See: https://auth0.com/docs/api/management/v2#!/Organizations/patch_organizations_by_id
         """
 
         return self.client.patch(self._url(id), data=body)
 
-    def delete_organization(self, id):
+    def delete_organization(self, id: str) -> Any:
         """Deletes an organization and all its related assets.
 
         Args:
            id (str): Id of organization to delete.
 
         See: https://auth0.com/docs/api/management/v2#!/Organizations/delete_organizations_by_id
         """
 
         return self.client.delete(self._url(id))
 
     # Organization Connections
-    def all_organization_connections(self, id, page=None, per_page=None):
+    def all_organization_connections(
+        self, id: str, page: int | None = None, per_page: int | None = None
+    ) -> list[dict[str, Any]]:
         """Retrieves a list of all the organization connections.
 
         Args:
            id (str): the ID of the organization.
 
            page (int): The result's page number (zero based). When not set,
               the default value is up to the server.
@@ -153,15 +168,17 @@
               the default value is up to the server.
 
         See: https://auth0.com/docs/api/management/v2#!/Organizations/get_enabled_connections
         """
         params = {"page": page, "per_page": per_page}
         return self.client.get(self._url(id, "enabled_connections"), params=params)
 
-    def get_organization_connection(self, id, connection_id):
+    def get_organization_connection(
+        self, id: str, connection_id: str
+    ) -> dict[str, Any]:
         """Retrieves an organization connection by its ID.
 
         Args:
            id (str): the ID of the organization.
 
            connection_id (str): the ID of the connection.
 
@@ -169,28 +186,32 @@
         """
         params = {}
 
         return self.client.get(
             self._url(id, "enabled_connections", connection_id), params=params
         )
 
-    def create_organization_connection(self, id, body):
+    def create_organization_connection(
+        self, id: str, body: dict[str, Any]
+    ) -> dict[str, Any]:
         """Adds a connection to an organization.
 
         Args:
            id (str): the ID of the organization.
 
            body (dict): Attributes for the connection to add.
 
         See: https://auth0.com/docs/api/management/v2#!/Organizations/post_enabled_connections
         """
 
         return self.client.post(self._url(id, "enabled_connections"), data=body)
 
-    def update_organization_connection(self, id, connection_id, body):
+    def update_organization_connection(
+        self, id: str, connection_id: str, body: dict[str, Any]
+    ) -> dict[str, Any]:
         """Modifies an organization.
 
         Args:
            id (str): the ID of the organization.
 
            connection_id (str): the ID of the connection to update.
 
@@ -199,15 +220,15 @@
         See: https://auth0.com/docs/api/management/v2#!/Organizations/patch_enabled_connections_by_connectionId
         """
 
         return self.client.patch(
             self._url(id, "enabled_connections", connection_id), data=body
         )
 
-    def delete_organization_connection(self, id, connection_id):
+    def delete_organization_connection(self, id: str, connection_id: str) -> Any:
         """Deletes a connection from the given organization.
 
         Args:
            id (str): Id of organization.
 
            connection_id (str): the ID of the connection to delete.
 
@@ -215,21 +236,21 @@
         """
 
         return self.client.delete(self._url(id, "enabled_connections", connection_id))
 
     # Organization Members
     def all_organization_members(
         self,
-        id,
-        page=None,
-        per_page=None,
-        include_totals=True,
-        from_param=None,
-        take=None,
-    ):
+        id: str,
+        page: int | None = None,
+        per_page: int | None = None,
+        include_totals: bool = True,
+        from_param: str | None = None,
+        take: int | None = None,
+    ) -> list[dict[str, Any]]:
         """Retrieves a list of all the organization members.
 
         Args:
             id (str): the ID of the organization.
 
             page (int): The result's page number (zero based). When not set,
                 the default value is up to the server.
@@ -255,42 +276,50 @@
             "include_totals": str(include_totals).lower(),
             "from": from_param,
             "take": take,
         }
 
         return self.client.get(self._url(id, "members"), params=params)
 
-    def create_organization_members(self, id, body):
+    def create_organization_members(
+        self, id: str, body: dict[str, Any]
+    ) -> dict[str, Any]:
         """Adds members to an organization.
 
         Args:
            id (str): the ID of the organization.
 
            body (dict): Attributes from the members to add.
 
         See: https://auth0.com/docs/api/management/v2#!/Organizations/post_members
         """
 
         return self.client.post(self._url(id, "members"), data=body)
 
-    def delete_organization_members(self, id, body):
+    def delete_organization_members(self, id: str, body: dict[str, Any]) -> Any:
         """Deletes members from the given organization.
 
         Args:
            id (str): Id of organization.
 
            body (dict): Attributes from the members to delete
 
         See: https://auth0.com/docs/api/management/v2#!/Organizations/delete_members
         """
 
         return self.client.delete(self._url(id, "members"), data=body)
 
     # Organization Member Roles
-    def all_organization_member_roles(self, id, user_id, page=None, per_page=None):
+    def all_organization_member_roles(
+        self,
+        id: str,
+        user_id: str,
+        page: int | None = None,
+        per_page: int | None = None,
+    ) -> list[dict[str, Any]]:
         """Retrieves a list of all the roles from the given organization member.
 
         Args:
            id (str): the ID of the organization.
 
            user_id (str): the ID of the user member of the organization.
 
@@ -303,30 +332,34 @@
         See: https://auth0.com/docs/api/management/v2#!/Organizations/get_organization_member_roles
         """
         params = {"page": page, "per_page": per_page}
         return self.client.get(
             self._url(id, "members", user_id, "roles"), params=params
         )
 
-    def create_organization_member_roles(self, id, user_id, body):
+    def create_organization_member_roles(
+        self, id: str, user_id: str, body: dict[str, Any]
+    ) -> dict[str, Any]:
         """Adds roles to a member of an organization.
 
         Args:
            id (str): the ID of the organization.
 
            user_id (str): the ID of the user member of the organization.
 
            body (dict): Attributes from the members to add.
 
         See: https://auth0.com/docs/api/management/v2#!/Organizations/post_organization_member_roles
         """
 
         return self.client.post(self._url(id, "members", user_id, "roles"), data=body)
 
-    def delete_organization_member_roles(self, id, user_id, body):
+    def delete_organization_member_roles(
+        self, id: str, user_id: str, body: dict[str, Any]
+    ) -> Any:
         """Deletes roles from a member of an organization.
 
         Args:
            id (str): Id of organization.
 
            user_id (str): the ID of the user member of the organization.
 
@@ -336,19 +369,19 @@
         """
 
         return self.client.delete(self._url(id, "members", user_id, "roles"), data=body)
 
     # Organization Invitations
     def all_organization_invitations(
         self,
-        id,
-        page=None,
-        per_page=None,
-        include_totals=False,
-    ):
+        id: str,
+        page: int | None = None,
+        per_page: int | None = None,
+        include_totals: bool = False,
+    ) -> list[dict[str, Any]]:
         """Retrieves a list of all the organization invitations.
 
         Args:
            id (str): the ID of the organization.
 
            page (int): The result's page number (zero based). When not set,
               the default value is up to the server.
@@ -366,15 +399,15 @@
             "page": page,
             "per_page": per_page,
             "include_totals": str(include_totals).lower(),
         }
 
         return self.client.get(self._url(id, "invitations"), params=params)
 
-    def get_organization_invitation(self, id, invitaton_id):
+    def get_organization_invitation(self, id: str, invitaton_id: str) -> dict[str, Any]:
         """Retrieves an organization invitation by its ID.
 
         Args:
            id (str): the ID of the organization.
 
            invitaton_id (str): the ID of the invitation.
 
@@ -382,28 +415,30 @@
         """
         params = {}
 
         return self.client.get(
             self._url(id, "invitations", invitaton_id), params=params
         )
 
-    def create_organization_invitation(self, id, body):
+    def create_organization_invitation(
+        self, id: str, body: dict[str, Any]
+    ) -> dict[str, Any]:
         """Create an invitation to an organization.
 
         Args:
            id (str): the ID of the organization.
 
            body (dict): Attributes for the invitation to create.
 
         See: https://auth0.com/docs/api/management/v2#!/Organizations/post_invitations
         """
 
         return self.client.post(self._url(id, "invitations"), data=body)
 
-    def delete_organization_invitation(self, id, invitation_id):
+    def delete_organization_invitation(self, id: str, invitation_id: str) -> Any:
         """Deletes an invitation from the given organization.
 
         Args:
            id (str): Id of organization.
 
            invitation_id (str): the ID of the invitation to delete.
```

### Comparing `auth0-python-4.3.0/auth0/management/prompts.py` & `auth0-python-4.4.0/auth0/management/prompts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Prompts:
     """Auth0 prompts endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,65 +18,82 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, prompt=None, language=None):
+    def _url(self, prompt: str | None = None, language: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/prompts"
         if prompt is not None and language is not None:
             return f"{url}/{prompt}/custom-text/{language}"
         return url
 
-    def get(self):
+    def get(self) -> dict[str, Any]:
         """Retrieves prompts settings.
 
         See: https://auth0.com/docs/api/management/v2#!/Prompts/get_prompts
         """
 
         return self.client.get(self._url())
 
-    def update(self, body):
+    def update(self, body: dict[str, Any]) -> dict[str, Any]:
         """Updates prompts settings.
 
         See: https://auth0.com/docs/api/management/v2#!/Prompts/patch_prompts
         """
 
         return self.client.patch(self._url(), data=body)
 
-    def get_custom_text(self, prompt, language):
+    def get_custom_text(self, prompt: str, language: str):
         """Retrieves custom text for a prompt in a specific language.
 
+        Args:
+            prompt (str): Name of the prompt.
+
+            language (str): Language to update.
+
         See: https://auth0.com/docs/api/management/v2#!/Prompts/get_custom_text_by_language
         """
 
         return self.client.get(self._url(prompt, language))
 
-    def update_custom_text(self, prompt, language, body):
+    def update_custom_text(
+        self, prompt: str, language: str, body: dict[str, Any]
+    ) -> dict[str, Any]:
         """Updates custom text for a prompt in a specific language.
 
+        Args:
+            prompt (str): Name of the prompt.
+
+            language (str): Language to update.
+
+            body (dict): An object containing custom dictionaries for a group of screens.
+
         See: https://auth0.com/docs/api/management/v2#!/Prompts/put_custom_text_by_language
         """
 
         return self.client.put(self._url(prompt, language), data=body)
```

### Comparing `auth0-python-4.3.0/auth0/management/resource_servers.py` & `auth0-python-4.4.0/auth0/management/resource_servers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class ResourceServers:
     """Auth0 resource servers endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,53 +18,61 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/resource-servers"
         if id is not None:
             return f"{url}/{id}"
         return url
 
-    def create(self, body):
+    def create(self, body: dict[str, Any]) -> dict[str, Any]:
         """Create a new resource server.
 
         Args:
            body (dict): Attributes for the new resource Server.
 
         See: https://auth0.com/docs/api/management/v2#!/Resource_Servers/post_resource_servers
         """
 
         return self.client.post(self._url(), data=body)
 
-    def get_all(self, page=None, per_page=None, include_totals=False):
+    def get_all(
+        self,
+        page: int | None = None,
+        per_page: int | None = None,
+        include_totals: bool = False,
+    ) -> list[dict[str, Any]]:
         """Retrieves all resource servers
 
         Args:
             page (int, optional): The result's page number (zero based). When not set,
               the default value is up to the server.
 
             per_page (int, optional): The amount of entries per page. When not set,
@@ -76,39 +89,39 @@
             "page": page,
             "per_page": per_page,
             "include_totals": str(include_totals).lower(),
         }
 
         return self.client.get(self._url(), params=params)
 
-    def get(self, id):
+    def get(self, id: str) -> dict[str, Any]:
         """Retrieves a resource server by its id.
 
         Args:
            id (str): id of the resource server to get.
 
 
         See: https://auth0.com/docs/api/management/v2#!/Resource_Servers/get_resource_servers_by_id
         """
 
         return self.client.get(self._url(id))
 
-    def delete(self, id):
+    def delete(self, id: str) -> Any:
         """Deletes a resource server.
 
         Args:
            id (str): Id of resource server to delete.
 
 
         See: https://auth0.com/docs/api/management/v2#!/Resource_Servers/delete_resource_servers_by_id
         """
 
         return self.client.delete(self._url(id))
 
-    def update(self, id, body):
+    def update(self, id: str, body: dict[str, Any]) -> dict[str, Any]:
         """Modifies a resource server.
 
         Args:
            id (str): The id of the resource server to update.
 
            body (dict): Attributes to modify.
```

### Comparing `auth0-python-4.3.0/auth0/management/roles.py` & `auth0-python-4.4.0/auth0/management/roles.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any, List  # List is being used as list is already a method.
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Roles:
     """Auth0 roles endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,42 +18,51 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/roles"
         if id is not None:
             return f"{url}/{id}"
         return url
 
-    def list(self, page=0, per_page=25, include_totals=True, name_filter=None):
+    def list(
+        self,
+        page: int = 0,
+        per_page: int = 25,
+        include_totals: bool = True,
+        name_filter: str | None = None,
+    ) -> List[dict[str, Any]]:
         """List or search roles.
 
         Args:
             page (int, optional): The result's page number (zero based). By default,
                retrieves the first page of results.
 
             per_page (int, optional): The amount of entries per page. By default,
@@ -66,60 +80,66 @@
             "per_page": per_page,
             "page": page,
             "include_totals": str(include_totals).lower(),
             "name_filter": name_filter,
         }
         return self.client.get(self._url(), params=params)
 
-    def create(self, body):
+    def create(self, body: dict[str, Any]) -> dict[str, Any]:
         """Creates a new role.
 
         Args:
             body (dict): the attributes for the role to create.
 
         See: https://auth0.com/docs/api/v2#!/Roles/post_roles
         """
         return self.client.post(self._url(), data=body)
 
-    def get(self, id):
+    def get(self, id: str) -> dict[str, Any]:
         """Get a role.
 
         Args:
             id (str): The id of the role to retrieve.
 
         See: https://auth0.com/docs/api/management/v2#!/Roles/get_roles_by_id
         """
 
         return self.client.get(self._url(id))
 
-    def delete(self, id):
+    def delete(self, id: str) -> Any:
         """Delete a role.
 
         Args:
             id (str): The id of the role to delete.
 
         See: https://auth0.com/docs/api/management/v2#!/Roles/delete_roles_by_id
         """
         return self.client.delete(self._url(id))
 
-    def update(self, id, body):
+    def update(self, id: str, body: dict[str, Any]) -> dict[str, Any]:
         """Update a role with the attributes passed in 'body'
 
         Args:
             id (str): The id of the role to update.
 
             body (dict): the attributes to update on the role.
 
         See: https://auth0.com/docs/api/management/v2#!/Roles/patch_roles_by_id
         """
         return self.client.patch(self._url(id), data=body)
 
     def list_users(
-        self, id, page=0, per_page=25, include_totals=True, from_param=None, take=None
-    ):
+        self,
+        id: str,
+        page: int = 0,
+        per_page: int = 25,
+        include_totals: bool = True,
+        from_param: str | None = None,
+        take: int | None = None,
+    ) -> List[dict[str, Any]]:
         """List the users that have been associated with a given role.
 
         Args:
             id (str): The role's id.
 
             page (int, optional): The result's page number (zero based). By default,
                retrieves the first page of results.
@@ -146,29 +166,31 @@
             "from": from_param,
             "take": take,
         }
 
         url = self._url(f"{id}/users")
         return self.client.get(url, params=params)
 
-    def add_users(self, id, users):
+    def add_users(self, id: str, users: List[str]) -> dict[str, Any]:
         """Assign users to a role.
 
         Args:
             id (str): The role's id.
 
             users (list of str): A list of users ids to add to this role.
 
         See https://auth0.com/docs/api/management/v2#!/Roles/post_role_users
         """
         url = self._url(f"{id}/users")
         body = {"users": users}
         return self.client.post(url, data=body)
 
-    def list_permissions(self, id, page=0, per_page=25, include_totals=True):
+    def list_permissions(
+        self, id: str, page: int = 0, per_page: int = 25, include_totals: bool = True
+    ) -> List[dict[str, Any]]:
         """List the permissions associated to a role.
 
         Args:
             id (str): The role's id.
 
             page (int, optional): The result's page number (zero based). By default,
                retrieves the first page of results.
@@ -185,29 +207,29 @@
             "per_page": per_page,
             "page": page,
             "include_totals": str(include_totals).lower(),
         }
         url = self._url(f"{id}/permissions")
         return self.client.get(url, params=params)
 
-    def remove_permissions(self, id, permissions):
+    def remove_permissions(self, id: str, permissions: List[str]) -> Any:
         """Unassociates permissions from a role.
 
         Args:
             id (str): The role's id.
 
             permissions (list of str): A list of permission ids to unassociate from the role.
 
         See https://auth0.com/docs/api/management/v2#!/Roles/delete_role_permission_assignment
         """
         url = self._url(f"{id}/permissions")
         body = {"permissions": permissions}
         return self.client.delete(url, data=body)
 
-    def add_permissions(self, id, permissions):
+    def add_permissions(self, id: str, permissions: List[str]) -> dict[str, Any]:
         """Associates permissions with a role.
 
         Args:
             id (str): The role's id.
 
             permissions (list of str): A list of permission ids to associate to the role.
```

### Comparing `auth0-python-4.3.0/auth0/management/rules.py` & `auth0-python-4.4.0/auth0/management/rules.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Rules:
     """Rules endpoint implementation.
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,51 +18,54 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/rules"
         if id is not None:
             return f"{url}/{id}"
         return url
 
     def all(
         self,
-        stage="login_success",
-        enabled=True,
-        fields=None,
-        include_fields=True,
-        page=None,
-        per_page=None,
-        include_totals=False,
-    ):
+        stage: str = "login_success",
+        enabled: bool = True,
+        fields: list[str] | None = None,
+        include_fields: bool = True,
+        page: int | None = None,
+        per_page: int | None = None,
+        include_totals: bool = False,
+    ) -> list[dict[str, Any]]:
         """Retrieves a list of all rules.
 
         Args:
             stage (str, optional):  Retrieves rules that match the execution stage.
                 Defaults to login_success.
 
             enabled (bool, optional): If provided, retrieves rules that match
@@ -93,25 +101,27 @@
 
         # since the default is True, this is here to disable the filter
         if enabled is not None:
             params["enabled"] = str(enabled).lower()
 
         return self.client.get(self._url(), params=params)
 
-    def create(self, body):
+    def create(self, body: dict[str, Any]) -> dict[str, Any]:
         """Creates a new rule.
 
         Args:
             body (dict): Attributes for the newly created rule.
 
         See: https://auth0.com/docs/api/v2#!/Rules/post_rules
         """
         return self.client.post(self._url(), data=body)
 
-    def get(self, id, fields=None, include_fields=True):
+    def get(
+        self, id: str, fields: list[str] | None = None, include_fields: bool = True
+    ) -> dict[str, Any]:
         """Retrieves a rule by its ID.
 
         Args:
             id (str): The id of the rule to retrieve.
 
             fields (list, optional): A list of fields to include or exclude
                 (depending on include_fields) from the result. Leave empty to
@@ -124,25 +134,25 @@
         """
         params = {
             "fields": fields and ",".join(fields) or None,
             "include_fields": str(include_fields).lower(),
         }
         return self.client.get(self._url(id), params=params)
 
-    def delete(self, id):
+    def delete(self, id: str) -> Any:
         """Delete a rule.
 
         Args:
             id (str): The id of the rule to delete.
 
         See: https://auth0.com/docs/api/management/v2#!/Rules/delete_rules_by_id
         """
         return self.client.delete(self._url(id))
 
-    def update(self, id, body):
+    def update(self, id: str, body: dict[str, Any]) -> dict[str, Any]:
         """Update an existing rule
 
         Args:
             id (str): The id of the rule to modify.
 
             body (dict): Attributes to modify.
```

### Comparing `auth0-python-4.3.0/auth0/management/rules_configs.py` & `auth0-python-4.4.0/auth0/management/rules_configs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class RulesConfigs:
     """RulesConfig endpoint implementation.
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,59 +18,62 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/rules-configs"
         if id is not None:
             return url + "/" + id
         return url
 
-    def all(self):
+    def all(self) -> list[dict[str, Any]]:
         """Lists the config variable keys for rules.
 
         See: https://auth0.com/docs/api/management/v2#!/Rules_Configs/get_rules_configs
         """
         return self.client.get(self._url())
 
-    def unset(self, key):
+    def unset(self, key: str) -> Any:
         """Removes the rules config for a given key.
 
         Args:
             key (str): rules config key to remove.
 
         See: https://auth0.com/docs/api/management/v2#!/Rules_Configs/delete_rules_configs_by_key
         """
         return self.client.delete(self._url(key))
 
-    def set(self, key, value):
+    def set(self, key: str, value: str) -> dict[str, Any]:
         """Sets the rules config for a given key.
 
         Args:
             key (str): rules config key to set.
 
             value (str): value to set for the rules config key.
```

### Comparing `auth0-python-4.3.0/auth0/management/tenants.py` & `auth0-python-4.4.0/auth0/management/tenants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Tenants:
     """Auth0 tenants endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,39 +18,44 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self):
+    def _url(self) -> str:
         return f"{self.protocol}://{self.domain}/api/v2/tenants/settings"
 
-    def get(self, fields=None, include_fields=True):
+    def get(
+        self, fields: list[str] | None = None, include_fields: bool = True
+    ) -> dict[str, Any]:
         """Get tenant settings.
 
         Args:
            fields (list of str, optional): A list of fields to include or
               exclude from the result (depending on include_fields). Leave empty to
               retrieve all fields.
 
@@ -58,15 +68,15 @@
         params = {
             "fields": fields and ",".join(fields) or None,
             "include_fields": str(include_fields).lower(),
         }
 
         return self.client.get(self._url(), params=params)
 
-    def update(self, body):
+    def update(self, body: dict[str, Any]) -> dict[str, Any]:
         """Update tenant settings.
 
         Args:
             body (dict): the attributes to update in the tenant.
 
         See: https://auth0.com/docs/api/v2#!/Tenants/patch_settings
         """
```

### Comparing `auth0-python-4.3.0/auth0/management/tickets.py` & `auth0-python-4.4.0/auth0/management/users_by_email.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,75 @@
-from ..rest import RestClient
+from __future__ import annotations
 
+from typing import Any
 
-class Tickets:
-    """Auth0 tickets endpoints
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
+
+
+class UsersByEmail:
+    """Auth0 users by email endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
 
         token (str): Management API v2 Token
 
         telemetry (bool, optional): Enable or disable Telemetry
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, action):
-        return f"{self.protocol}://{self.domain}/api/v2/tickets/{action}"
+    def _url(self) -> str:
+        return f"{self.protocol}://{self.domain}/api/v2/users-by-email"
 
-    def create_email_verification(self, body):
-        """Create an email verification ticket.
+    def search_users_by_email(
+        self, email: str, fields: list[str] | None = None, include_fields: bool = True
+    ) -> list[dict[str, Any]]:
+        """List or search users.
 
         Args:
-            body (dict): attributes to set on the email verification request.
 
-        See: https://auth0.com/docs/api/v2#!/Tickets/post_email_verification
-        """
-        return self.client.post(self._url("email-verification"), data=body)
+            email: Email to search.
 
-    def create_pswd_change(self, body):
-        """Create password change ticket.
+            fields (list of str, optional): A list of fields to include or
+                exclude from the result (depending on include_fields). Leave empty to
+                retrieve all fields.
 
-        Args:
-            body (dict): attributes to set on the password change request.
+            include_fields (bool, optional): True if the fields specified are
+                to be include in the result, False otherwise.
 
-        See: https://auth0.com/docs/api/v2#!/Tickets/post_password_change
+        See: https://auth0.com/docs/api/management/v2#!/Users_By_Email/get_users_by_email
         """
-        return self.client.post(self._url("password-change"), data=body)
+        params = {
+            "email": email,
+            "fields": fields and ",".join(fields) or None,
+            "include_fields": str(include_fields).lower(),
+        }
+        return self.client.get(self._url(), params=params)
```

### Comparing `auth0-python-4.3.0/auth0/management/user_blocks.py` & `auth0-python-4.4.0/auth0/management/user_blocks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ..rest import RestClient
+from __future__ import annotations
+
+from typing import Any
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class UserBlocks:
     """Auth0 user blocks endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -13,79 +18,82 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/user-blocks"
         if id is not None:
             return f"{url}/{id}"
         return url
 
-    def get_by_identifier(self, identifier):
+    def get_by_identifier(self, identifier: str) -> dict[str, Any]:
         """Gets blocks by identifier
 
         Args:
            identifier (str): Should be any of: username, phone_number, email.
 
         See: https://auth0.com/docs/api/management/v2#!/User_Blocks/get_user_blocks
         """
 
         params = {"identifier": identifier}
 
         return self.client.get(self._url(), params=params)
 
-    def unblock_by_identifier(self, identifier):
+    def unblock_by_identifier(self, identifier: dict[str, Any]) -> Any:
         """Unblocks by identifier
 
         Args:
            identifier (str): Should be any of: username, phone_number, email.
 
         See: https://auth0.com/docs/api/management/v2#!/User_Blocks/delete_user_blocks
         """
 
         params = {"identifier": identifier}
 
         return self.client.delete(self._url(), params=params)
 
-    def get(self, id):
+    def get(self, id: str) -> dict[str, Any]:
         """Get a user's blocks
 
         Args:
            id (str): The user_id of the user to retrieve.
 
         See: https://auth0.com/docs/api/management/v2#!/User_Blocks/get_user_blocks_by_id
         """
 
         return self.client.get(self._url(id))
 
-    def unblock(self, id):
+    def unblock(self, id: str) -> Any:
         """Unblock a user
 
         Args:
            id (str): The user_id of the user to update.
 
         See: https://auth0.com/docs/api/management/v2#!/User_Blocks/delete_user_blocks_by_id
         """
```

### Comparing `auth0-python-4.3.0/auth0/management/users.py` & `auth0-python-4.4.0/auth0/management/users.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-import warnings
+from __future__ import annotations
 
-from ..rest import RestClient
+from typing import Any, List  # List is being used as list is already a method.
+
+from ..rest import RestClient, RestClientOptions
+from ..types import TimeoutType
 
 
 class Users:
     """Auth0 users endpoints
 
     Args:
         domain (str): Your Auth0 domain, e.g: 'username.auth0.com'
@@ -15,53 +18,56 @@
             (defaults to True)
 
         timeout (float or tuple, optional): Change the requests
             connect and read timeout. Pass a tuple to specify
             both values separately or a float to set both to it.
             (defaults to 5.0 for both)
 
+        protocol (str, optional): Protocol to use when making requests.
+            (defaults to "https")
+
         rest_options (RestClientOptions): Pass an instance of
             RestClientOptions to configure additional RestClient
             options, such as rate-limit retries.
             (defaults to None)
     """
 
     def __init__(
         self,
-        domain,
-        token,
-        telemetry=True,
-        timeout=5.0,
-        protocol="https",
-        rest_options=None,
-    ):
+        domain: str,
+        token: str,
+        telemetry: bool = True,
+        timeout: TimeoutType = 5.0,
+        protocol: str = "https",
+        rest_options: RestClientOptions | None = None,
+    ) -> None:
         self.domain = domain
         self.protocol = protocol
         self.client = RestClient(
             jwt=token, telemetry=telemetry, timeout=timeout, options=rest_options
         )
 
-    def _url(self, id=None):
+    def _url(self, id: str | None = None) -> str:
         url = f"{self.protocol}://{self.domain}/api/v2/users"
         if id is not None:
             return f"{url}/{id}"
         return url
 
     def list(
         self,
-        page=0,
-        per_page=25,
-        sort=None,
-        connection=None,
-        q=None,
-        search_engine=None,
-        include_totals=True,
-        fields=None,
-        include_fields=True,
-    ):
+        page: int = 0,
+        per_page: int = 25,
+        sort: str | None = None,
+        connection: str | None = None,
+        q: str | None = None,
+        search_engine: str | None = None,
+        include_totals: bool = True,
+        fields: List[str] | None = None,
+        include_fields: bool = True,
+    ) -> List[dict[str, Any]]:
         """List or search users.
 
         Args:
             page (int, optional): The result's page number (zero based). By default,
                retrieves the first page of results.
 
             per_page (int, optional): The amount of entries per page. By default,
@@ -102,25 +108,27 @@
             "fields": fields and ",".join(fields) or None,
             "include_fields": str(include_fields).lower(),
             "q": q,
             "search_engine": search_engine,
         }
         return self.client.get(self._url(), params=params)
 
-    def create(self, body):
+    def create(self, body: dict[str, Any]) -> dict[str, Any]:
         """Creates a new user.
 
         Args:
             body (dict): the attributes to set on the user to create.
 
         See: https://auth0.com/docs/api/v2#!/Users/post_users
         """
         return self.client.post(self._url(), data=body)
 
-    def get(self, id, fields=None, include_fields=True):
+    def get(
+        self, id: str, fields: List[str] | None = None, include_fields: bool = True
+    ) -> dict[str, Any]:
         """Get a user.
 
         Args:
             id (str): The user_id of the user to retrieve.
 
             fields (list of str, optional): A list of fields to include or
                 exclude from the result (depending on include_fields). Leave empty to
@@ -134,37 +142,39 @@
         params = {
             "fields": fields and ",".join(fields) or None,
             "include_fields": str(include_fields).lower(),
         }
 
         return self.client.get(self._url(id), params=params)
 
-    def delete(self, id):
+    def delete(self, id: str) -> Any:
         """Delete a user.
 
         Args:
             id (str): The user_id of the user to delete.
 
         See: https://auth0.com/docs/api/management/v2#!/Users/delete_users_by_id
         """
         return self.client.delete(self._url(id))
 
-    def update(self, id, body):
+    def update(self, id: str, body: dict[str, Any]) -> dict[str, Any]:
         """Update a user with the attributes passed in 'body'
 
         Args:
             id (str): The user_id of the user to update.
 
             body (dict): The attributes of the user to update.
 
         See: https://auth0.com/docs/api/v2#!/Users/patch_users_by_id
         """
         return self.client.patch(self._url(id), data=body)
 
-    def list_organizations(self, id, page=0, per_page=25, include_totals=True):
+    def list_organizations(
+        self, id: str, page: int = 0, per_page: int = 25, include_totals: bool = True
+    ) -> List[dict[str, Any]]:
         """List the organizations that the user is member of.
 
         Args:
             id (str): The user's id.
 
             page (int, optional): The result's page number (zero based). By default,
                retrieves the first page of results.
@@ -182,15 +192,17 @@
             "page": page,
             "include_totals": str(include_totals).lower(),
         }
 
         url = self._url(f"{id}/organizations")
         return self.client.get(url, params=params)
 
-    def list_roles(self, id, page=0, per_page=25, include_totals=True):
+    def list_roles(
+        self, id: str, page: int = 0, per_page: int = 25, include_totals: bool = True
+    ) -> List[dict[str, Any]]:
         """List the roles associated with a user.
 
         Args:
             id (str): The user's id.
 
             page (int, optional): The result's page number (zero based). By default,
                retrieves the first page of results.
@@ -208,43 +220,45 @@
             "page": page,
             "include_totals": str(include_totals).lower(),
         }
 
         url = self._url(f"{id}/roles")
         return self.client.get(url, params=params)
 
-    def remove_roles(self, id, roles):
+    def remove_roles(self, id: str, roles: List[str]) -> Any:
         """Removes an array of roles from a user.
 
         Args:
             id (str): The user's id.
 
             roles (list of str): A list of roles ids to unassociate from the user.
 
         See https://auth0.com/docs/api/management/v2#!/Users/delete_user_roles
         """
         url = self._url(f"{id}/roles")
         body = {"roles": roles}
         return self.client.delete(url, data=body)
 
-    def add_roles(self, id, roles):
+    def add_roles(self, id: str, roles: List[str]) -> dict[str, Any]:
         """Associate an array of roles with a user.
 
         Args:
             id (str): The user's id.
 
             roles (list of str): A list of roles ids to associated with the user.
 
         See https://auth0.com/docs/api/management/v2#!/Users/post_user_roles
         """
         url = self._url(f"{id}/roles")
         body = {"roles": roles}
         return self.client.post(url, data=body)
 
-    def list_permissions(self, id, page=0, per_page=25, include_totals=True):
+    def list_permissions(
+        self, id: str, page: int = 0, per_page: int = 25, include_totals: bool = True
+    ) -> List[dict[str, Any]]:
         """List the permissions associated to the user.
 
         Args:
             id (str): The user's id.
 
             page (int, optional): The result's page number (zero based). By default,
                retrieves the first page of results.
@@ -262,83 +276,83 @@
             "per_page": per_page,
             "page": page,
             "include_totals": str(include_totals).lower(),
         }
         url = self._url(f"{id}/permissions")
         return self.client.get(url, params=params)
 
-    def remove_permissions(self, id, permissions):
+    def remove_permissions(self, id: str, permissions: List[str]) -> Any:
         """Removes permissions from a user.
 
         Args:
             id (str): The user's id.
 
             permissions (list of str): A list of permission ids to unassociate from the user.
 
         See https://auth0.com/docs/api/management/v2#!/Users/delete_permissions
         """
         url = self._url(f"{id}/permissions")
         body = {"permissions": permissions}
         return self.client.delete(url, data=body)
 
-    def add_permissions(self, id, permissions):
+    def add_permissions(self, id: str, permissions: List[str]) -> dict[str, Any]:
         """Assign permissions to a user.
 
         Args:
             id (str): The user's id.
 
             permissions (list of str): A list of permission ids to associated with the user.
 
         See https://auth0.com/docs/api/management/v2#!/Users/post_permissions
         """
         url = self._url(f"{id}/permissions")
         body = {"permissions": permissions}
         return self.client.post(url, data=body)
 
-    def delete_multifactor(self, id, provider):
+    def delete_multifactor(self, id: str, provider: str) -> Any:
         """Delete a user's multifactor provider.
 
         Args:
             id (str): The user's id.
 
             provider (str): The multifactor provider. Supported values 'duo'
                 or 'google-authenticator'.
 
         See: https://auth0.com/docs/api/management/v2#!/Users/delete_multifactor_by_provider
         """
         url = self._url(f"{id}/multifactor/{provider}")
         return self.client.delete(url)
 
-    def delete_authenticators(self, id):
+    def delete_authenticators(self, id: str) -> Any:
         """Delete a user's MFA enrollments.
 
         Args:
             id (str): The user's id.
 
         See: https://auth0.com/docs/api/management/v2#!/Users/delete_authenticators
         """
         url = self._url(f"{id}/authenticators")
         return self.client.delete(url)
 
-    def unlink_user_account(self, id, provider, user_id):
+    def unlink_user_account(self, id: str, provider: str, user_id: str) -> Any:
         """Unlink a user account
 
         Args:
             id (str): The user_id of the user identity.
 
             provider (str): The type of identity provider (e.g: facebook).
 
             user_id (str): The unique identifier for the user for the identity.
 
         See: https://auth0.com/docs/api/management/v2#!/Users/delete_user_identity_by_user_id
         """
         url = self._url(f"{id}/identities/{provider}/{user_id}")
         return self.client.delete(url)
 
-    def link_user_account(self, user_id, body):
+    def link_user_account(self, user_id: str, body: dict[str, Any]) -> dict[str, Any]:
         """Link user accounts.
 
         Links the account specified in the body (secondary account) to the
         account specified by the id param of the URL (primary account).
 
         Args:
             id (str): The user_id of the primary identity where you are linking
@@ -347,39 +361,44 @@
             body (dict): the attributes to send as part of this request.
 
         See: https://auth0.com/docs/api/v2#!/Users/post_identities
         """
         url = self._url(f"{user_id}/identities")
         return self.client.post(url, data=body)
 
-    def regenerate_recovery_code(self, user_id):
+    def regenerate_recovery_code(self, user_id: str) -> dict[str, Any]:
         """Removes the current recovery token, generates and returns a new one
 
         Args:
             user_id (str):  The user_id of the user identity.
 
         See: https://auth0.com/docs/api/management/v2#!/Users/post_recovery_code_regeneration
         """
         url = self._url(f"{user_id}/recovery-code-regeneration")
         return self.client.post(url)
 
-    def get_guardian_enrollments(self, user_id):
+    def get_guardian_enrollments(self, user_id: str) -> dict[str, Any]:
         """Retrieves all Guardian enrollments.
 
         Args:
             user_id (str):  The user_id of the user to retrieve.
 
         See: https://auth0.com/docs/api/management/v2#!/Users/get_enrollments
         """
         url = self._url(f"{user_id}/enrollments")
         return self.client.get(url)
 
     def get_log_events(
-        self, user_id, page=0, per_page=50, sort=None, include_totals=False
-    ):
+        self,
+        user_id: str,
+        page: int = 0,
+        per_page: int = 50,
+        sort: str | None = None,
+        include_totals: bool = False,
+    ) -> List[dict[str, Any]]:
         """Retrieve every log event for a specific user id.
 
         Args:
             user_id (str):  The user_id of the logs to retrieve.
 
             page (int, optional): The result's page number (zero based). By default,
                 retrieves the first page of results.
@@ -404,106 +423,114 @@
             "include_totals": str(include_totals).lower(),
             "sort": sort,
         }
 
         url = self._url(f"{user_id}/logs")
         return self.client.get(url, params=params)
 
-    def invalidate_remembered_browsers(self, user_id):
+    def invalidate_remembered_browsers(self, user_id: str) -> dict[str, Any]:
         """Invalidate all remembered browsers across all authentication factors for a user.
 
         Args:
             user_id (str):  The user_id to invalidate remembered browsers for.
 
         See: https://auth0.com/docs/api/management/v2#!/Users/post_invalidate_remember_browser
         """
 
         url = self._url(f"{user_id}/multifactor/actions/invalidate-remember-browser")
         return self.client.post(url)
 
-    def get_authentication_methods(self, user_id):
+    def get_authentication_methods(self, user_id: str) -> dict[str, Any]:
         """Gets a list of authentication methods
 
         Args:
             user_id (str):  The user_id to get a list of authentication methods for.
 
         See: https://auth0.com/docs/api/management/v2#!/Users/get_authentication_methods
         """
 
         url = self._url(f"{user_id}/authentication-methods")
         return self.client.get(url)
 
-    def get_authentication_method_by_id(self, user_id, authentication_method_id):
+    def get_authentication_method_by_id(
+        self, user_id: str, authentication_method_id: str
+    ) -> dict[str, Any]:
         """Gets an authentication method by ID.
 
         Args:
             user_id (str):  The user_id to get an authentication method by ID for.
             authentication_method_id (str):  The authentication_method_id to get an authentication method by ID for.
 
         See: https://auth0.com/docs/api/management/v2#!/Users/get_authentication_methods_by_authentication_method_id
         """
 
         url = self._url(f"{user_id}/authentication-methods/{authentication_method_id}")
         return self.client.get(url)
 
-    def create_authentication_method(self, user_id, body):
+    def create_authentication_method(
+        self, user_id: str, body: dict[str, Any]
+    ) -> dict[str, Any]:
         """Creates an authentication method for a given user.
 
         Args:
             user_id (str):  The user_id to create an authentication method for a given user.
             body (dict): the request body to create an authentication method for a given user.
 
         See: https://auth0.com/docs/api/management/v2#!/Users/post_authentication_methods
         """
 
         url = self._url(f"{user_id}/authentication-methods")
         return self.client.post(url, data=body)
 
-    def update_authentication_methods(self, user_id, body):
+    def update_authentication_methods(
+        self, user_id: str, body: dict[str, Any]
+    ) -> dict[str, Any]:
         """Updates all authentication methods for a user by replacing them with the given ones.
 
         Args:
             user_id (str):  The user_id to update all authentication methods for.
             body (dict): the request body to update all authentication methods with.
 
         See: https://auth0.com/docs/api/management/v2#!/Users/put_authentication_methods
         """
 
         url = self._url(f"{user_id}/authentication-methods")
         return self.client.put(url, data=body)
 
     def update_authentication_method_by_id(
-        self, user_id, authentication_method_id, body
-    ):
+        self, user_id: str, authentication_method_id: str, body: dict[str, Any]
+    ) -> dict[str, Any]:
         """Updates an authentication method.
 
         Args:
             user_id (str):  The user_id to update an authentication method.
             authentication_method_id (str):  The authentication_method_id to update an authentication method for.
             body (dict): the request body to update an authentication method.
 
         See: https://auth0.com/docs/api/management/v2#!/Users/patch_authentication_methods_by_authentication_method_id
         """
 
         url = self._url(f"{user_id}/authentication-methods/{authentication_method_id}")
         return self.client.patch(url, data=body)
 
-    def delete_authentication_methods(self, user_id):
+    def delete_authentication_methods(self, user_id: str) -> Any:
         """Deletes all authentication methods for the given user.
 
         Args:
             user_id (str):  The user_id to delete all authentication methods for the given user for.
 
         See: https://auth0.com/docs/api/management/v2#!/Users/delete_authentication_methods
         """
 
         url = self._url(f"{user_id}/authentication-methods")
         return self.client.delete(url)
 
-    def delete_authentication_method_by_id(self, user_id, authentication_method_id):
+    def delete_authentication_method_by_id(
+        self, user_id: str, authentication_method_id: str
+    ) -> Any:
         """Deletes an authentication method by ID.
 
         Args:
             user_id (str):  The user_id to delete an authentication method by ID for.
             authentication_method_id (str):  The authentication_method_id to delete an authentication method by ID for.
 
         See: https://auth0.com/docs/api/management/v2#!/Users/delete_authentication_methods_by_authentication_method_id
```

### Comparing `auth0-python-4.3.0/auth0/rest.py` & `auth0-python-4.4.0/auth0/rest.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/rest_async.py` & `auth0-python-4.4.0/auth0/rest_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         sock_connect, sock_read = (
             self.timeout
             if isinstance(self.timeout, tuple)
             else (self.timeout, self.timeout)
         )
         self.timeout = aiohttp.ClientTimeout(
             sock_connect=sock_connect, sock_read=sock_read
-        )
+        )  # type: ignore[assignment]
 
     def set_session(self, session: aiohttp.ClientSession) -> None:
         """Set Client Session to improve performance by reusing session.
         Session should be closed manually or within context manager.
         """
         self._session = session
```

### Comparing `auth0-python-4.3.0/auth0/test/authentication/test_base.py` & `auth0-python-4.4.0/auth0/test/authentication/test_base.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/authentication/test_database.py` & `auth0-python-4.4.0/auth0/test/authentication/test_database.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/authentication/test_delegated.py` & `auth0-python-4.4.0/auth0/test/authentication/test_delegated.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/authentication/test_enterprise.py` & `auth0-python-4.4.0/auth0/test/authentication/test_enterprise.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/authentication/test_get_token.py` & `auth0-python-4.4.0/auth0/test/authentication/test_get_token.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/authentication/test_passwordless.py` & `auth0-python-4.4.0/auth0/test/authentication/test_passwordless.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/authentication/test_revoke_token.py` & `auth0-python-4.4.0/auth0/test/authentication/test_revoke_token.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/authentication/test_social.py` & `auth0-python-4.4.0/auth0/test/authentication/test_social.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/authentication/test_token_verifier.py` & `auth0-python-4.4.0/auth0/test/authentication/test_token_verifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -502,33 +502,74 @@
             signature_verifier=sv,
             issuer=expectations["issuer"],
             audience=expectations["audience"],
         )
         tv._clock = MOCKED_CLOCK
         tv.verify(token, organization="org_123")
 
-    def test_fails_when_org_specified_but_not_present(self):
+    def test_fails_when_org_name_specified_but_not_present(self):
+        token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJhdXRoMHxzZGs0NThma3MiLCJhdWQiOiJ0b2tlbnMtdGVzdC0xMjMiLCJpc3MiOiJodHRwczovL3Rva2Vucy10ZXN0LmF1dGgwLmNvbS8iLCJleHAiOjE1ODc3NjUzNjEsImlhdCI6MTU4NzU5MjU2MX0.wotJnUdD5IfdZMewF_-BnHc0pI56uwzwr5qaSXvSu9w"
+        self.assert_fails_with_error(
+            token,
+            "Organization (org_name) claim must be a string present in the ID token",
+            signature_verifier=SymmetricSignatureVerifier(HMAC_SHARED_SECRET),
+            organization="org-123",
+        )
+
+    def test_fails_when_org_name_specified_but_not_string(self):
+        token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJhdXRoMHxzZGs0NThma3MiLCJhdWQiOiJ0b2tlbnMtdGVzdC0xMjMiLCJvcmdfbmFtZSI6NDIsImlzcyI6Imh0dHBzOi8vdG9rZW5zLXRlc3QuYXV0aDAuY29tLyIsImV4cCI6MTU4Nzc2NTM2MSwiaWF0IjoxNTg3NTkyNTYxfQ.RXu-dz1u2pftk_iInk1To8z9g1B6TVA-5FAwoCx85T0"
+        self.assert_fails_with_error(
+            token,
+            "Organization (org_name) claim must be a string present in the ID token",
+            signature_verifier=SymmetricSignatureVerifier(HMAC_SHARED_SECRET),
+            organization="org-123",
+        )
+
+    def test_fails_when_org_name_specified_but_does_not_match(self):
+        token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJhdXRoMHxzZGs0NThma3MiLCJhdWQiOiJ0b2tlbnMtdGVzdC0xMjMiLCJvcmdfbmFtZSI6Im9yZy1hYmMiLCJpc3MiOiJodHRwczovL3Rva2Vucy10ZXN0LmF1dGgwLmNvbS8iLCJleHAiOjE1ODc3NjUzNjEsImlhdCI6MTU4NzU5MjU2MX0.P_ldJGEaFg58cARwGMtog_KTsqv7cGJZXoS9xdTEkvQ"
+        self.assert_fails_with_error(
+            token,
+            'Organization (org_name) claim mismatch in the ID token; expected "org-123",'
+            ' found "org-abc"',
+            signature_verifier=SymmetricSignatureVerifier(HMAC_SHARED_SECRET),
+            organization="org-123",
+        )
+
+    def test_succeeds_when_org_name_specified_matches(self):
+        token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJhdXRoMHxzZGs0NThma3MiLCJhdWQiOiJ0b2tlbnMtdGVzdC0xMjMiLCJvcmdfbmFtZSI6Im9yZy0xMjMiLCJpc3MiOiJodHRwczovL3Rva2Vucy10ZXN0LmF1dGgwLmNvbS8iLCJleHAiOjE1ODc3NjUzNjEsImlhdCI6MTU4NzU5MjU2MX0.P8Kba8Fgamyiw1qw_lBfp2OAzWn6NOLL6fBCDQhGvyc"
+        sv = SymmetricSignatureVerifier(HMAC_SHARED_SECRET)
+        tv = TokenVerifier(
+            signature_verifier=sv,
+            issuer=expectations["issuer"],
+            audience=expectations["audience"],
+        )
+        tv._clock = MOCKED_CLOCK
+        response = tv.verify(token)
+        self.assertIn("org_name", response)
+        self.assertEqual("org-123", response["org_name"])
+
+    def test_fails_when_org_id_specified_but_not_present(self):
         token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJhdXRoMHxzZGs0NThma3MiLCJhdWQiOiJ0b2tlbnMtdGVzdC0xMjMiLCJpc3MiOiJodHRwczovL3Rva2Vucy10ZXN0LmF1dGgwLmNvbS8iLCJleHAiOjE1ODc3NjUzNjEsImlhdCI6MTU4NzU5MjU2MX0.wotJnUdD5IfdZMewF_-BnHc0pI56uwzwr5qaSXvSu9w"
         self.assert_fails_with_error(
             token,
             "Organization (org_id) claim must be a string present in the ID token",
             signature_verifier=SymmetricSignatureVerifier(HMAC_SHARED_SECRET),
             organization="org_123",
         )
 
-    def test_fails_when_org_specified_but_not_(self):
+    def test_fails_when_org_id_specified_but_not_string(self):
         token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJhdXRoMHxzZGs0NThma3MiLCJhdWQiOiJ0b2tlbnMtdGVzdC0xMjMiLCJvcmdfaWQiOjQyLCJpc3MiOiJodHRwczovL3Rva2Vucy10ZXN0LmF1dGgwLmNvbS8iLCJleHAiOjE1ODc3NjUzNjEsImlhdCI6MTU4NzU5MjU2MX0.fGL1_akaHikdovS7NRYla3flne1xdtCjP0ei_CRxO6k"
         self.assert_fails_with_error(
             token,
             "Organization (org_id) claim must be a string present in the ID token",
             signature_verifier=SymmetricSignatureVerifier(HMAC_SHARED_SECRET),
             organization="org_123",
         )
 
-    def test_fails_when_org_specified_but_does_not_match(self):
+    def test_fails_when_org_id_specified_but_does_not_match(self):
         token = "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJhdXRoMHxzZGs0NThma3MiLCJhdWQiOiJ0b2tlbnMtdGVzdC0xMjMiLCJvcmdfaWQiOiJvcmdfMTIzIiwiaXNzIjoiaHR0cHM6Ly90b2tlbnMtdGVzdC5hdXRoMC5jb20vIiwiZXhwIjoxNTg3NzY1MzYxLCJpYXQiOjE1ODc1OTI1NjF9.hjSPgJpg0Dn2z0giCdGqVLD5Kmqy_yMYlSkgwKD7ahQ"
         self.assert_fails_with_error(
             token,
             'Organization (org_id) claim mismatch in the ID token; expected "org_abc",'
             ' found "org_123"',
             signature_verifier=SymmetricSignatureVerifier(HMAC_SHARED_SECRET),
             organization="org_abc",
```

### Comparing `auth0-python-4.3.0/auth0/test/management/test_actions.py` & `auth0-python-4.4.0/auth0/test/management/test_actions.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_atack_protection.py` & `auth0-python-4.4.0/auth0/test/management/test_atack_protection.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_auth0.py` & `auth0-python-4.4.0/auth0/test/management/test_auth0.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_blacklists.py` & `auth0-python-4.4.0/auth0/test/management/test_blacklists.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_branding.py` & `auth0-python-4.4.0/auth0/test/management/test_branding.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_client_credentials.py` & `auth0-python-4.4.0/auth0/test/management/test_client_credentials.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_client_grants.py` & `auth0-python-4.4.0/auth0/test/management/test_client_grants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_clients.py` & `auth0-python-4.4.0/auth0/test/management/test_clients.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_connections.py` & `auth0-python-4.4.0/auth0/test/management/test_connections.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_custom_domains.py` & `auth0-python-4.4.0/auth0/test/management/test_custom_domains.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_device_credentials.py` & `auth0-python-4.4.0/auth0/test/management/test_device_credentials.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_email_endpoints.py` & `auth0-python-4.4.0/auth0/test/management/test_email_endpoints.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_emails.py` & `auth0-python-4.4.0/auth0/test/management/test_emails.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_grants.py` & `auth0-python-4.4.0/auth0/test/management/test_grants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_guardian.py` & `auth0-python-4.4.0/auth0/test/management/test_guardian.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_hooks.py` & `auth0-python-4.4.0/auth0/test/management/test_hooks.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_jobs.py` & `auth0-python-4.4.0/auth0/test/management/test_jobs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_log_streams.py` & `auth0-python-4.4.0/auth0/test/management/test_log_streams.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_logs.py` & `auth0-python-4.4.0/auth0/test/management/test_logs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_organizations.py` & `auth0-python-4.4.0/auth0/test/management/test_organizations.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_prompts.py` & `auth0-python-4.4.0/auth0/test/management/test_prompts.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_resource_servers.py` & `auth0-python-4.4.0/auth0/test/management/test_resource_servers.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_rest.py` & `auth0-python-4.4.0/auth0/test/management/test_rest.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_roles.py` & `auth0-python-4.4.0/auth0/test/management/test_roles.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_rules.py` & `auth0-python-4.4.0/auth0/test/management/test_rules.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_rules_configs.py` & `auth0-python-4.4.0/auth0/test/management/test_rules_configs.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_stats.py` & `auth0-python-4.4.0/auth0/test/management/test_stats.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_tenants.py` & `auth0-python-4.4.0/auth0/test/management/test_tenants.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_tickets.py` & `auth0-python-4.4.0/auth0/test/management/test_tickets.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_user_blocks.py` & `auth0-python-4.4.0/auth0/test/management/test_user_blocks.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_users.py` & `auth0-python-4.4.0/auth0/test/management/test_users.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test/management/test_users_by_email.py` & `auth0-python-4.4.0/auth0/test/management/test_users_by_email.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test_async/test_async_auth0.py` & `auth0-python-4.4.0/auth0/test_async/test_async_auth0.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test_async/test_async_token_verifier.py` & `auth0-python-4.4.0/auth0/test_async/test_async_token_verifier.py`

 * *Files identical despite different names*

### Comparing `auth0-python-4.3.0/auth0/test_async/test_asyncify.py` & `auth0-python-4.4.0/auth0/test_async/test_asyncify.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 from unittest.mock import ANY, MagicMock
 
 import aiohttp
 from aioresponses import CallbackResult, aioresponses
 from callee import Attrs
 
 from auth0.asyncify import asyncify
-from auth0.authentication import GetToken
+from auth0.authentication import GetToken, Users
 from auth0.management import Clients, Guardian, Jobs
 
 clients = re.compile(r"^https://example\.com/api/v2/clients.*")
 token = re.compile(r"^https://example\.com/oauth/token.*")
+user_info = re.compile(r"^https://example\.com/userinfo.*")
 factors = re.compile(r"^https://example\.com/api/v2/guardian/factors.*")
 users_imports = re.compile(r"^https://example\.com/api/v2/jobs/users-imports.*")
 payload = {"foo": "bar"}
 
 telemetry = base64.b64encode(
     json.dumps(
         {
@@ -108,14 +109,30 @@
                 "client_secret": "clsec",
             },
             headers={i: headers[i] for i in headers if i != "Authorization"},
             timeout=ANY,
         )
 
     @aioresponses()
+    async def test_user_info(self, mocked):
+        callback, mock = get_callback()
+        mocked.get(user_info, callback=callback)
+        c = asyncify(Users)(domain="example.com")
+        self.assertEqual(
+            await c.userinfo_async(access_token="access-token-example"), payload
+        )
+        mock.assert_called_with(
+            Attrs(path="/userinfo"),
+            headers={**headers, "Authorization": "Bearer access-token-example"},
+            timeout=ANY,
+            allow_redirects=True,
+            params=None,
+        )
+
+    @aioresponses()
     async def test_file_post(self, mocked):
         callback, mock = get_callback()
         mocked.post(users_imports, callback=callback)
         j = asyncify(Jobs)(domain="example.com", token="jwt")
         users = TemporaryFile()
         self.assertEqual(await j.import_users_async("connection-1", users), payload)
         file_port_headers = headers.copy()
```

### Comparing `auth0-python-4.3.0/auth0_python.egg-info/PKG-INFO` & `auth0-python-4.4.0/auth0_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth0-python
-Version: 4.3.0
+Version: 4.4.0
 Summary: Auth0 Python SDK
 Home-page: https://github.com/auth0/auth0-python
 Author: Auth0
 Author-email: support@auth0.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auth0-python Version: 4.3.0 Summary: Auth0 Python
+Metadata-Version: 2.1 Name: auth0-python Version: 4.4.0 Summary: Auth0 Python
 SDK Home-page: https://github.com/auth0/auth0-python Author: Auth0 Author-
 email: support@auth0.com License: MIT Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `auth0-python-4.3.0/auth0_python.egg-info/SOURCES.txt` & `auth0-python-4.4.0/auth0_python.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 auth0/__init__.py
 auth0/asyncify.py
 auth0/exceptions.py
+auth0/py.typed
 auth0/rest.py
 auth0/rest_async.py
 auth0/types.py
 auth0/utils.py
 auth0/authentication/__init__.py
 auth0/authentication/async_token_verifier.py
 auth0/authentication/base.py
```

### Comparing `auth0-python-4.3.0/setup.py` & `auth0-python-4.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     long_description_content_type="text/markdown",
     author="Auth0",
     author_email="support@auth0.com",
     license="MIT",
     packages=find_packages(),
     install_requires=["requests>=2.14.0", "pyjwt[crypto]>=2.6.0"],
     extras_require={"test": ["coverage", "pre-commit"]},
+    package_data={"auth0": ["py.typed"]},
     python_requires=">=3.7",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
```

