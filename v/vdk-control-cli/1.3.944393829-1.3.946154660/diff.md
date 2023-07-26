# Comparing `tmp/vdk-control-cli-1.3.944393829.tar.gz` & `tmp/vdk-control-cli-1.3.946154660.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-control-cli-1.3.944393829.tar", last modified: Tue Jul 25 09:00:59 2023, max compression
+gzip compressed data, was "dist/vdk-control-cli-1.3.946154660.tar", last modified: Wed Jul 26 14:08:41 2023, max compression
```

## Comparing `vdk-control-cli-1.3.944393829.tar` & `vdk-control-cli-1.3.946154660.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5153 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1747 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/api/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/api/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/api/control/plugin/markers.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/api/control/plugin/specs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/common_group/
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/common_group/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/info_group/
--rw-rw-rw-   0 root         (0) root         (0)     1868 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/info_group/info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/
--rw-rw-rw-   0 root         (0) root         (0)    12776 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/create.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/delete.py
--rw-rw-rw-   0 root         (0) root         (0)     7121 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/deploy_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14343 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     5129 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/download_job.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/download_key.py
--rw-rw-rw-   0 root         (0) root         (0)    12207 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/execute.py
--rw-rw-rw-   0 root         (0) root         (0)     8735 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/list.py
--rw-rw-rw-   0 root         (0) root         (0)    11314 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/properties.py
--rw-rw-rw-   0 root         (0) root         (0)    11433 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/secrets.py
--rw-rw-rw-   0 root         (0) root         (0)     3403 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/show.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/login_group/
--rw-rw-rw-   0 root         (0) root         (0)     6510 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/login_group/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/logout_group/
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/logout_group/logout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/version_group/
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/version_group/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/default_options.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/defaults_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)     9551 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/vdk_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/exception/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/exception/vdk_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/job_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     4871 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/job_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/10_sql_step.sql
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/20_python_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2902 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/config.ini
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     3666 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     3715 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/plugin/control_plugin_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/rest_lib/
--rw-rw-rw-   0 root         (0) root         (0)     3239 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/rest_lib/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3845 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/rest_lib/rest_client_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/
--rw-rw-rw-   0 root         (0) root         (0)     7297 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/cli_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/control_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3690 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/output_printer.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-25 09:00:41.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/version_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-25 09:00:46.000000 vdk-control-cli-1.3.944393829/src/vdk/internal/control/vdk_control_build_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5153 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2426 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      185 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-25 09:00:59.000000 vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-25 09:00:46.000000 vdk-control-cli-1.3.944393829/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/api/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/api/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/api/control/plugin/markers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/api/control/plugin/specs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/common_group/
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/common_group/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/info_group/
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/info_group/info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/
+-rw-rw-rw-   0 root         (0) root         (0)    12776 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/create.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     7206 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/deploy_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14285 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     5129 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/download_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/download_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    12207 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     8735 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/list.py
+-rw-rw-rw-   0 root         (0) root         (0)    11314 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)    11433 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     3403 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/show.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/login_group/
+-rw-rw-rw-   0 root         (0) root         (0)     6510 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/login_group/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/logout_group/
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/logout_group/logout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/version_group/
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/version_group/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/configuration/default_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/configuration/defaults_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/configuration/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9551 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/configuration/vdk_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/exception/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/exception/vdk_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/job/
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/job/job_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/job/job_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/job/sample_job/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/job/sample_job/10_sql_step.sql
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/job/sample_job/20_python_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/job/sample_job/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2902 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/job/sample_job/config.ini
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/job/sample_job/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3666 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     3715 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/plugin/control_plugin_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/rest_lib/
+-rw-rw-rw-   0 root         (0) root         (0)     3239 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/rest_lib/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/rest_lib/rest_client_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     7297 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/utils/cli_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/utils/control_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4587 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/utils/output_printer.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-26 14:08:23.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/utils/version_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-26 14:08:27.000000 vdk-control-cli-1.3.946154660/src/vdk/internal/control/vdk_control_build_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk_control_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-07-26 14:08:40.000000 vdk-control-cli-1.3.946154660/src/vdk_control_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-07-26 14:08:41.000000 vdk-control-cli-1.3.946154660/src/vdk_control_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 14:08:40.000000 vdk-control-cli-1.3.946154660/src/vdk_control_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-07-26 14:08:40.000000 vdk-control-cli-1.3.946154660/src/vdk_control_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 14:08:40.000000 vdk-control-cli-1.3.946154660/src/vdk_control_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      185 2023-07-26 14:08:40.000000 vdk-control-cli-1.3.946154660/src/vdk_control_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-26 14:08:40.000000 vdk-control-cli-1.3.946154660/src/vdk_control_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-26 14:08:27.000000 vdk-control-cli-1.3.946154660/version.txt
```

### Comparing `vdk-control-cli-1.3.944393829/PKG-INFO` & `vdk-control-cli-1.3.946154660/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.944393829
+Version: 1.3.946154660
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.944393829/README.md` & `vdk-control-cli-1.3.946154660/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/setup.cfg` & `vdk-control-cli-1.3.946154660/setup.cfg`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/api/control/plugin/markers.py` & `vdk-control-cli-1.3.946154660/src/vdk/api/control/plugin/markers.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/api/control/plugin/specs.py` & `vdk-control-cli-1.3.946154660/src/vdk/api/control/plugin/specs.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/common_group/default.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/common_group/default.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/info_group/info.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/info_group/info.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/create.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/create.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/delete.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/deploy_cli.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/deploy_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from enum import unique
 from typing import Optional
 
 import click
 from vdk.internal.control.command_groups.job.deploy_cli_impl import JobDeploy
 from vdk.internal.control.configuration.defaults_config import load_default_team_name
 from vdk.internal.control.utils import cli_utils
+from vdk.internal.control.utils import output_printer
 from vdk.internal.control.utils.cli_utils import get_or_prompt
 
 
 @unique
 class DeployOperation(Enum):
     """
     An enum used to store the types of deploy operations
@@ -165,15 +166,15 @@
     enabled: Optional[bool],
     job_path: Optional[str],
     operation: str,
     reason: Optional[str],
     rest_api_url: str,
     output: str,
 ):
-    cmd = JobDeploy(rest_api_url, output)
+    cmd = JobDeploy(rest_api_url, output_printer.create_printer(output))
     if operation == DeployOperation.UPDATE.value or enabled is not None:
         name = get_or_prompt("Job Name", name)
         team = get_or_prompt("Job Team", team)
         # default to ask for job version to update
         if not vdk_version and not job_version and enabled is None:
             job_version = get_or_prompt("Job Version", job_version)
         if job_path:
```

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,35 +15,35 @@
 from taurus_datajob_api import DataJobSchedule
 from vdk.internal.control.configuration.defaults_config import load_default_team_name
 from vdk.internal.control.exception.vdk_exception import VDKException
 from vdk.internal.control.job.job_archive import JobArchive
 from vdk.internal.control.job.job_config import JobConfig
 from vdk.internal.control.rest_lib.factory import ApiClientFactory
 from vdk.internal.control.rest_lib.rest_client_errors import ApiClientErrorDecorator
-from vdk.internal.control.utils import output_printer
 from vdk.internal.control.utils.cli_utils import get_or_prompt
-from vdk.internal.control.utils.output_printer import OutputFormat
+from vdk.internal.control.utils.output_printer import Printer
+from vdk.internal.control.utils.output_printer import PrinterJson
+from vdk.internal.control.utils.output_printer import PrinterText
 
 log = logging.getLogger(__name__)
 
 
 class JobDeploy:
     ZIP_ARCHIVE_TYPE = "zip"
     ARCHIVE_SUFFIX = "-archive"
 
-    def __init__(self, rest_api_url: str, output_format: str):
+    def __init__(self, rest_api_url: str, printer: Printer):
         self.deploy_api = ApiClientFactory(rest_api_url).get_deploy_api()
         self.jobs_api = ApiClientFactory(rest_api_url).get_jobs_api()
         self.job_sources_api = ApiClientFactory(rest_api_url).get_jobs_sources_api()
         # support for multiple deployments is not implemented yet so we can put anything here.
         # Ultimately this will be user facing parameter (possibly fetched from config.ini)
         self.__deployment_id = "production"
         self.__job_archive = JobArchive()
-        self.__output_format = output_format
-        self.__printer = output_printer.create_printer(self.__output_format)
+        self.__printer = printer
 
     @staticmethod
     def __detect_keytab_files_in_job_directory(job_path: str) -> None:
         keytab_glob = os.path.join(job_path, "**/*.keytab")
         keytab_files = glob.glob(keytab_glob, recursive=True)
         if keytab_files:
             raise VDKException(
@@ -189,15 +189,15 @@
     def __update_deployment(self, name: str, team: str, deployment: DataJobDeployment):
         log.debug(
             f"Update Deployment version of a job {name} of team {team} : {deployment}"
         )
         self.deploy_api.deployment_update(
             team_name=team, job_name=name, data_job_deployment=deployment
         )
-        if self.__output_format == OutputFormat.TEXT.value:
+        if isinstance(self.__printer, PrinterText):
             log.info(
                 f"Request to deploy Data Job {name} using version {deployment.job_version} finished successfully.\n"
                 f"It would take a few minutes for the Data Job to be deployed in the server.\n"
                 f"If notified_on_job_deploy option in config.ini is configured then "
                 f"notification will be sent on successful deploy or in case of an error.\n\n"
                 f"You can also execute `vdk deploy --show -t '{team}' -n '{name}'` and compare the printed version "
                 f"to the one of the newly deployed job - {deployment.job_version} - to verify that the deployment "
@@ -235,15 +235,15 @@
                     last_deployed_by=d.last_deployed_by,
                     last_deployed_date=d.last_deployed_date,
                     python_version=d.python_version,
                     enabled=d.enabled,
                 ),
                 deployments,
             )
-            if self.__output_format == OutputFormat.TEXT.value:
+            if isinstance(self.__printer, PrinterText):
                 click.echo(
                     "You can compare the version seen here to the one seen when "
                     "deploying to verify your deployment was successful."
                 )
                 click.echo("")
                 self.__printer.print_table(list(deployments))
             else:
@@ -279,29 +279,29 @@
         job_config = JobConfig(job_path)
 
         self.__validate_datajob(job_path=job_path, job_config=job_config, team=team)
         team = get_or_prompt(
             "Team Name", team or job_config.get_team() or load_default_team_name()
         )
 
-        if self.__output_format == OutputFormat.TEXT.value:
+        if isinstance(self.__printer, PrinterText):
             log.info(
                 f"Deploy Data Job with name {name} from directory {job_path} ... \n"
             )
 
         archive_path = self.__job_archive.archive_data_job(
             job_name=name, job_archive_path=job_path
         )
         try:
             job_archive_binary = self.__archive_binary(archive_path)
 
-            if self.__output_format == OutputFormat.TEXT.value:
+            if isinstance(self.__printer, PrinterText):
                 log.info("Uploading the data job might take some time ...")
             with click_spinner.spinner(
-                disable=(self.__output_format == OutputFormat.JSON.value)
+                disable=(isinstance(self.__printer, PrinterJson))
             ):
                 data_job_version = self.job_sources_api.sources_upload(
                     team_name=team,
                     job_name=name,
                     body=job_archive_binary,
                     reason=reason,
                 )
```

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/download_job.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/download_job.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/download_key.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/download_key.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/execute.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/execute.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/list.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/list.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/properties.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/properties.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/secrets.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/secrets.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/job/show.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/job/show.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/login_group/login.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/login_group/login.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/command_groups/version_group/version.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/command_groups/version_group/version.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/defaults_config.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/configuration/defaults_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/log_config.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/configuration/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/configuration/vdk_config.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/configuration/vdk_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/exception/vdk_exception.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/exception/vdk_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/job_archive.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/job/job_archive.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/job_config.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/job/job_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/10_sql_step.sql` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/job/sample_job/10_sql_step.sql`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/20_python_step.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/job/sample_job/20_python_step.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/README.md` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/job/sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/job/sample_job/config.ini` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/job/sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/main.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/main.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/plugin/control_plugin_manager.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/plugin/control_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/rest_lib/factory.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/rest_lib/factory.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/rest_lib/rest_client_errors.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/rest_lib/rest_client_errors.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/cli_utils.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/control_utils.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/utils/control_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/output_printer.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/utils/output_printer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright 2023-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import abc
+import io
 import json
 from enum import Enum
 from enum import unique
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
@@ -56,15 +57,15 @@
         _registered_printers[output_format.lower()] = cls
         return cls
 
     return decorator
 
 
 @printer("text")
-class _PrinterText(Printer):
+class PrinterText(Printer):
     def print_table(self, table: Optional[List[Dict[str, Any]]]) -> None:
         if table and len(table) > 0:
             click.echo(tabulate(table, headers="keys", tablefmt="fancy_grid"))
         else:
             click.echo("No Data.")
 
     def print_dict(self, data: Optional[Dict[str, Any]]) -> None:
@@ -89,28 +90,57 @@
             return obj.isoformat()
         raise TypeError("Type %s not serializable" % type(obj))
 
     return json.dumps(data, default=json_serial, indent=indent)
 
 
 @printer("json")
-class _PrinterJson(Printer):
+class PrinterJson(Printer):
     def print_table(self, data: List[Dict[str, Any]]) -> None:
         if data:
             click.echo(json_format(data))
         else:
             click.echo("[]")
 
     def print_dict(self, data: Dict[str, Any]) -> None:
         if data:
             click.echo(json_format(data))
         else:
             click.echo("{}")
 
 
+class InMemoryTextPrinter(Printer):
+    def __init__(self):
+        self.__output_buffer = io.StringIO()
+
+    def print_table(self, table: Optional[List[Dict[str, Any]]]) -> None:
+        if table and len(table) > 0:
+            print(
+                tabulate(table, headers="keys", tablefmt="fancy_grid"),
+                file=self.__output_buffer,
+            )
+        else:
+            print("No Data.", file=self.__output_buffer)
+
+    def print_dict(self, data: Optional[Dict[str, Any]]) -> None:
+        if data:
+            print(
+                tabulate(
+                    [[k, v] for k, v in data.items()],
+                    headers=("key", "value"),
+                ),
+                file=self.__output_buffer,
+            )
+        else:
+            print("No Data.", file=self.__output_buffer)
+
+    def get_memory(self):
+        return self.__output_buffer.getvalue()
+
+
 def create_printer(output_format: str) -> Printer:
     """
     Creates a printer instance for the given output format.
 
     :param output_format: the desired output format
     :return: An instance of a Printer subclass that can print data in the desired format.
```

### Comparing `vdk-control-cli-1.3.944393829/src/vdk/internal/control/utils/version_utils.py` & `vdk-control-cli-1.3.946154660/src/vdk/internal/control/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/PKG-INFO` & `vdk-control-cli-1.3.946154660/src/vdk_control_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.944393829
+Version: 1.3.946154660
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.944393829/src/vdk_control_cli.egg-info/SOURCES.txt` & `vdk-control-cli-1.3.946154660/src/vdk_control_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

