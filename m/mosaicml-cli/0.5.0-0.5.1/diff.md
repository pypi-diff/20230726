# Comparing `tmp/mosaicml-cli-0.5.0.tar.gz` & `tmp/mosaicml-cli-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.5.0.tar", last modified: Mon Jul 24 21:45:35 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.5.1.tar", last modified: Wed Jul 26 00:37:20 2023, max compression
```

## Comparing `mosaicml-cli-0.5.0.tar` & `mosaicml-cli-0.5.1.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.364976 mosaicml-cli-0.5.0/
--rw-r--r--   0 wai.wu     (502) staff       (20)      696 2023-07-24 21:45:35.364815 mosaicml-cli-0.5.0/PKG-INFO
--rw-r--r--   0 wai.wu     (502) staff       (20)     7089 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/README.md
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.317674 mosaicml-cli-0.5.0/mcli/
--rw-r--r--   0 wai.wu     (502) staff       (20)     2122 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/__init__.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.318870 mosaicml-cli-0.5.0/mcli/api/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/__init__.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.319529 mosaicml-cli-0.5.0/mcli/api/cluster/
--rw-r--r--   0 wai.wu     (502) staff       (20)      134 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/cluster/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     4990 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.320126 mosaicml-cli-0.5.0/mcli/api/engine/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/engine/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)    26027 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/engine/engine.py
--rw-r--r--   0 wai.wu     (502) staff       (20)    13444 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/exceptions.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.322658 mosaicml-cli-0.5.0/mcli/api/inference_deployments/
--rw-r--r--   0 wai.wu     (502) staff       (20)     1521 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     3297 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     5045 2023-07-24 21:17:12.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     3744 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     8413 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2294 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_ping.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2746 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_predict_inference_deployment.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     6499 2023-07-24 21:17:12.000000 mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_update_inference_deployments.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.323499 mosaicml-cli-0.5.0/mcli/api/mint/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/mint/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     7840 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/mint/shell.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2676 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/mint/tty.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.324680 mosaicml-cli-0.5.0/mcli/api/model/
--rw-r--r--   0 wai.wu     (502) staff       (20)     1114 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/model/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     9386 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/api/model/cluster_details.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     4583 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/model/inference_deployment.py
--rw-r--r--   0 wai.wu     (502) staff       (20)    14890 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/model/run.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.331004 mosaicml-cli-0.5.0/mcli/api/runs/
--rw-r--r--   0 wai.wu     (502) staff       (20)     1269 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     3814 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_create_interactive_run.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     3034 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_create_run.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     4365 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     8796 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 wai.wu     (502) staff       (20)    12239 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     5366 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_start_run.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     5559 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     5573 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_update_run.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     4091 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 wai.wu     (502) staff       (20)    10414 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.331633 mosaicml-cli-0.5.0/mcli/api/schema/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/schema/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)      636 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.332698 mosaicml-cli-0.5.0/mcli/api/secrets/
--rw-r--r--   0 wai.wu     (502) staff       (20)      309 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/secrets/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2386 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2943 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     3665 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2354 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/typing_future.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.333154 mosaicml-cli-0.5.0/mcli/api/users/
--rw-r--r--   0 wai.wu     (502) staff       (20)      139 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/users/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2715 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/users/api_get_users.py
--rw-r--r--   0 wai.wu     (502) staff       (20)      920 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/api/utils.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.333811 mosaicml-cli-0.5.0/mcli/cli/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/cli/__init__.py
--rwxr-xr-x   0 wai.wu     (502) staff       (20)     6069 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/cli.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.334813 mosaicml-cli-0.5.0/mcli/cli/common/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/cli/common/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2560 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     7499 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.335327 mosaicml-cli-0.5.0/mcli/cli/m_connect/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:47.000000 mosaicml-cli-0.5.0/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     6426 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.336166 mosaicml-cli-0.5.0/mcli/cli/m_create/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_create/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2385 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_create/m_create.py
--rw-r--r--   0 wai.wu     (502) staff       (20)    16900 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.336921 mosaicml-cli-0.5.0/mcli/cli/m_delete/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     6448 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_delete/delete.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     5838 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.337447 mosaicml-cli-0.5.0/mcli/cli/m_deploy/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     4253 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.338322 mosaicml-cli-0.5.0/mcli/cli/m_describe/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     3929 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 wai.wu     (502) staff       (20)    13495 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2259 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.340633 mosaicml-cli-0.5.0/mcli/cli/m_get/
--rw-r--r--   0 wai.wu     (502) staff       (20)      467 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     7068 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/clusters.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     6459 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/display.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     5807 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     4804 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/m_get.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     8967 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/runs.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2189 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/secrets.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     1580 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_get/users.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.341264 mosaicml-cli-0.5.0/mcli/cli/m_init/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_init/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     3908 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_init/m_init.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.341830 mosaicml-cli-0.5.0/mcli/cli/m_interactive/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     8423 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.343367 mosaicml-cli-0.5.0/mcli/cli/m_kube/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_kube/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     5523 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_kube/m_get_config.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     1398 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_kube/m_kube.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2050 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_kube/m_merge_config.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     6946 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_kube/utils.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.343917 mosaicml-cli-0.5.0/mcli/cli/m_log/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_log/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)    11354 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.344588 mosaicml-cli-0.5.0/mcli/cli/m_ping/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     1411 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.345230 mosaicml-cli-0.5.0/mcli/cli/m_predict/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     1905 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.345587 mosaicml-cli-0.5.0/mcli/cli/m_root/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_root/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)      536 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.346081 mosaicml-cli-0.5.0/mcli/cli/m_run/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_run/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)    10779 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.347762 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2964 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     1793 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2267 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     1656 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 wai.wu     (502) staff       (20)      840 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/organization.py
--rw-r--r--   0 wai.wu     (502) staff       (20)      745 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.348260 mosaicml-cli-0.5.0/mcli/cli/m_stop/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     4062 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.348691 mosaicml-cli-0.5.0/mcli/cli/m_update/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_update/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     6222 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_update/m_update.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.349788 mosaicml-cli-0.5.0/mcli/cli/m_util/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_util/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)      797 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_util/m_util.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     9034 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/cli/m_util/util.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.350171 mosaicml-cli-0.5.0/mcli/cli/m_watchdog/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_watchdog/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     3544 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/cli/m_watchdog/m_watchdog.py
--rw-r--r--   0 wai.wu     (502) staff       (20)    13108 2023-07-24 20:29:09.000000 mosaicml-cli-0.5.0/mcli/config.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.352011 mosaicml-cli-0.5.0/mcli/models/
--rw-r--r--   0 wai.wu     (502) staff       (20)     1047 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/models/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2103 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/models/gpu_type.py
--rw-r--r--   0 wai.wu     (502) staff       (20)    12287 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/models/inference_deployment_config.py
--rw-r--r--   0 wai.wu     (502) staff       (20)      427 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/models/mcli_cluster.py
--rw-r--r--   0 wai.wu     (502) staff       (20)      456 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/models/mcli_envvar.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     6728 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/models/mcli_secret.py
--rw-r--r--   0 wai.wu     (502) staff       (20)    17205 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/models/run_config.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.352286 mosaicml-cli-0.5.0/mcli/objects/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/__init__.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.354354 mosaicml-cli-0.5.0/mcli/objects/secrets/
--rw-r--r--   0 wai.wu     (502) staff       (20)     1090 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.356313 mosaicml-cli-0.5.0/mcli/objects/secrets/create/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     1646 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/base.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2244 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2408 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     6377 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     3858 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     3001 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     5342 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 wai.wu     (502) staff       (20)      783 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     1017 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/env_var.py
--rw-r--r--   0 wai.wu     (502) staff       (20)      556 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/gcp.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     1267 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/mounted.py
--rw-r--r--   0 wai.wu     (502) staff       (20)      967 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/oci.py
--rw-r--r--   0 wai.wu     (502) staff       (20)      961 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/s3.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     1718 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.356847 mosaicml-cli-0.5.0/mcli/proto/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/proto/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     1477 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.357156 mosaicml-cli-0.5.0/mcli/sdk/
--rw-r--r--   0 wai.wu     (502) staff       (20)     2006 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/sdk/__init__.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.362248 mosaicml-cli-0.5.0/mcli/utils/
--rw-r--r--   0 wai.wu     (502) staff       (20)        0 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/__init__.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     6318 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/utils/utils_cli.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     4409 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/utils/utils_completers.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     7047 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_config.py
--rw-r--r--   0 wai.wu     (502) staff       (20)      740 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_date.py
--rw-r--r--   0 wai.wu     (502) staff       (20)    10749 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_docker.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2225 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_epilog.py
--rw-r--r--   0 wai.wu     (502) staff       (20)    10774 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_interactive.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     4527 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_logging.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     2160 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     1087 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/utils/utils_model.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     6605 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_pypi.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     3115 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_rich.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     5358 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/utils/utils_run_status.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     4350 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     1103 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_spinner.py
--rw-r--r--   0 wai.wu     (502) staff       (20)    10751 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_string_functions.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     1677 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_types.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     1001 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/mcli/utils/utils_yaml.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     3876 2023-07-24 21:43:55.000000 mosaicml-cli-0.5.0/mcli/version.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.363791 mosaicml-cli-0.5.0/mosaicml_cli.egg-info/
--rw-r--r--   0 wai.wu     (502) staff       (20)      696 2023-07-24 21:45:35.000000 mosaicml-cli-0.5.0/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 wai.wu     (502) staff       (20)     5106 2023-07-24 21:45:35.000000 mosaicml-cli-0.5.0/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 wai.wu     (502) staff       (20)        1 2023-07-24 21:45:35.000000 mosaicml-cli-0.5.0/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 wai.wu     (502) staff       (20)       75 2023-07-24 21:45:35.000000 mosaicml-cli-0.5.0/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 wai.wu     (502) staff       (20)     1654 2023-07-24 21:45:35.000000 mosaicml-cli-0.5.0/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 wai.wu     (502) staff       (20)        5 2023-07-24 21:45:35.000000 mosaicml-cli-0.5.0/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 wai.wu     (502) staff       (20)    31087 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/pyproject.toml
--rw-r--r--   0 wai.wu     (502) staff       (20)       38 2023-07-24 21:45:35.365020 mosaicml-cli-0.5.0/setup.cfg
--rw-r--r--   0 wai.wu     (502) staff       (20)     3056 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/setup.py
-drwxr-xr-x   0 wai.wu     (502) staff       (20)        0 2023-07-24 21:45:35.364535 mosaicml-cli-0.5.0/tests/
--rw-r--r--   0 wai.wu     (502) staff       (20)     6449 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/tests/test_config.py
--rw-r--r--   0 wai.wu     (502) staff       (20)       62 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/tests/test_simple.py
--rw-r--r--   0 wai.wu     (502) staff       (20)     6116 2023-07-15 01:20:48.000000 mosaicml-cli-0.5.0/tests/test_upgrade.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.217841 mosaicml-cli-0.5.1/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      696 2023-07-26 00:37:20.217704 mosaicml-cli-0.5.1/PKG-INFO
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     7089 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/README.md
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.190041 mosaicml-cli-0.5.1/mcli/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2122 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/__init__.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.190847 mosaicml-cli-0.5.1/mcli/api/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/__init__.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.191125 mosaicml-cli-0.5.1/mcli/api/cluster/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      134 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/cluster/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4990 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.191482 mosaicml-cli-0.5.1/mcli/api/engine/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/engine/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    26027 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/engine/engine.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    13444 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/exceptions.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.192696 mosaicml-cli-0.5.1/mcli/api/inference_deployments/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1521 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3297 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5045 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3992 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     8413 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2294 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_ping.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2746 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_predict_inference_deployment.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6499 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_update_inference_deployments.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.193084 mosaicml-cli-0.5.1/mcli/api/mint/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/mint/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     7840 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/mint/shell.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2676 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/mint/tty.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.193632 mosaicml-cli-0.5.1/mcli/api/model/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1114 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/model/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     9386 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/api/model/cluster_details.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4583 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    14890 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/api/model/run.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.195122 mosaicml-cli-0.5.1/mcli/api/runs/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1269 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3785 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_create_interactive_run.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3034 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4365 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     8796 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    12239 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5366 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5559 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5916 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_update_run.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4091 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    10414 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.195464 mosaicml-cli-0.5.1/mcli/api/schema/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/schema/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      636 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.195942 mosaicml-cli-0.5.1/mcli/api/secrets/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      309 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/secrets/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2386 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2943 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3665 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2354 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/typing_future.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.196210 mosaicml-cli-0.5.1/mcli/api/users/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      139 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/users/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2715 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/users/api_get_users.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      920 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/api/utils.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.196420 mosaicml-cli-0.5.1/mcli/cli/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/__init__.py
+-rwxr-xr-x   0 margaret.qian   (502) staff       (20)     6069 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/cli.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.196761 mosaicml-cli-0.5.1/mcli/cli/common/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/common/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2560 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     7499 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.196993 mosaicml-cli-0.5.1/mcli/cli/m_connect/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6426 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.197339 mosaicml-cli-0.5.1/mcli/cli/m_create/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2385 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    16900 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.197814 mosaicml-cli-0.5.1/mcli/cli/m_delete/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6448 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5838 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.198073 mosaicml-cli-0.5.1/mcli/cli/m_deploy/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4253 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.198630 mosaicml-cli-0.5.1/mcli/cli/m_describe/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3929 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    13495 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2259 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.199789 mosaicml-cli-0.5.1/mcli/cli/m_get/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      467 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     7068 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6459 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/display.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5807 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4804 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     8967 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/runs.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2189 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1580 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_get/users.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.204124 mosaicml-cli-0.5.1/mcli/cli/m_init/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3908 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_init/m_init.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.204468 mosaicml-cli-0.5.1/mcli/cli/m_interactive/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     9036 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.205155 mosaicml-cli-0.5.1/mcli/cli/m_kube/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_kube/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5523 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_kube/m_get_config.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1398 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_kube/m_kube.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2050 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_kube/m_merge_config.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6946 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_kube/utils.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.205413 mosaicml-cli-0.5.1/mcli/cli/m_log/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    11756 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.205658 mosaicml-cli-0.5.1/mcli/cli/m_ping/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1411 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.206037 mosaicml-cli-0.5.1/mcli/cli/m_predict/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1905 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.206425 mosaicml-cli-0.5.1/mcli/cli/m_root/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      536 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.206678 mosaicml-cli-0.5.1/mcli/cli/m_run/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    11501 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.207840 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2964 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1793 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2267 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1656 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      840 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/organization.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      745 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.208106 mosaicml-cli-0.5.1/mcli/cli/m_stop/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4062 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.208362 mosaicml-cli-0.5.1/mcli/cli/m_update/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_update/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6568 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/cli/m_update/m_update.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.208778 mosaicml-cli-0.5.1/mcli/cli/m_util/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      797 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     9034 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/cli/m_util/util.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.209036 mosaicml-cli-0.5.1/mcli/cli/m_watchdog/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/cli/m_watchdog/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3544 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/cli/m_watchdog/m_watchdog.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    13108 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/config.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.210159 mosaicml-cli-0.5.1/mcli/models/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1047 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/models/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2103 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/models/gpu_type.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    12287 2023-07-26 00:26:41.000000 mosaicml-cli-0.5.1/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      427 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/models/mcli_cluster.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      456 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/models/mcli_envvar.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6728 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/models/mcli_secret.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    17258 2023-07-26 00:36:22.000000 mosaicml-cli-0.5.1/mcli/models/run_config.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.210283 mosaicml-cli-0.5.1/mcli/objects/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/__init__.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.211336 mosaicml-cli-0.5.1/mcli/objects/secrets/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1090 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.212626 mosaicml-cli-0.5.1/mcli/objects/secrets/create/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1646 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2244 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2408 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6377 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3858 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3001 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5342 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      783 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1017 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      556 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1267 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      967 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/oci.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      961 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/s3.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1718 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.212903 mosaicml-cli-0.5.1/mcli/proto/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/proto/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1477 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.213067 mosaicml-cli-0.5.1/mcli/sdk/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2006 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/sdk/__init__.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.216058 mosaicml-cli-0.5.1/mcli/utils/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        0 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/__init__.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6318 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/utils/utils_cli.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4409 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/utils/utils_completers.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     7047 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_config.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      740 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_date.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    10749 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_docker.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2225 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_epilog.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    10774 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_interactive.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4527 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_logging.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     2160 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1087 2023-07-25 07:52:25.000000 mosaicml-cli-0.5.1/mcli/utils/utils_model.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6605 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_pypi.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3115 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_rich.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5358 2023-07-19 21:06:33.000000 mosaicml-cli-0.5.1/mcli/utils/utils_run_status.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     4350 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1103 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_spinner.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    10751 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1677 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_types.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1001 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/mcli/utils/utils_yaml.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3876 2023-07-26 00:36:38.000000 mosaicml-cli-0.5.1/mcli/version.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.216784 mosaicml-cli-0.5.1/mosaicml_cli.egg-info/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)      696 2023-07-26 00:37:20.000000 mosaicml-cli-0.5.1/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     5106 2023-07-26 00:37:20.000000 mosaicml-cli-0.5.1/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        1 2023-07-26 00:37:20.000000 mosaicml-cli-0.5.1/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 margaret.qian   (502) staff       (20)       75 2023-07-26 00:37:20.000000 mosaicml-cli-0.5.1/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     1654 2023-07-26 00:37:20.000000 mosaicml-cli-0.5.1/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 margaret.qian   (502) staff       (20)        5 2023-07-26 00:37:20.000000 mosaicml-cli-0.5.1/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 margaret.qian   (502) staff       (20)    31087 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/pyproject.toml
+-rw-r--r--   0 margaret.qian   (502) staff       (20)       38 2023-07-26 00:37:20.217879 mosaicml-cli-0.5.1/setup.cfg
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     3056 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/setup.py
+drwxr-xr-x   0 margaret.qian   (502) staff       (20)        0 2023-07-26 00:37:20.217426 mosaicml-cli-0.5.1/tests/
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6449 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/tests/test_config.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)       62 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/tests/test_simple.py
+-rw-r--r--   0 margaret.qian   (502) staff       (20)     6116 2023-07-18 07:46:23.000000 mosaicml-cli-0.5.1/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.5.0/PKG-INFO` & `mosaicml-cli-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.5.0
+Version: 0.5.1
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.5.0/README.md` & `mosaicml-cli-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/__init__.py` & `mosaicml-cli-0.5.1/mcli/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.5.1/mcli/api/cluster/api_get_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/engine/engine.py` & `mosaicml-cli-0.5.1/mcli/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/exceptions.py` & `mosaicml-cli-0.5.1/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.5.1/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_get_inference_deployment_logs.py` & `mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_get_inference_deployment_logs.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,35 +21,38 @@
 @overload
 def get_inference_deployment_logs(
     deployment: Union[str, InferenceDeployment],
     *,
     restart: Optional[int] = None,
     timeout: Optional[float] = None,
     future: Literal[False] = False,
+    failed: Optional[bool] = False,
 ) -> Generator[str, None, None]:
     ...
 
 
 @overload
 def get_inference_deployment_logs(
     deployment: Union[str, InferenceDeployment],
     *,
     restart: Optional[int] = None,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
+    failed: Optional[bool] = False,
 ) -> Generator[Future[str], None, None]:
     ...
 
 
 def get_inference_deployment_logs(
     deployment: Union[str, InferenceDeployment],
     *,
     restart: Optional[int] = None,
     timeout: Optional[float] = None,
     future: bool = False,
+    failed: Optional[bool] = False,
 ) -> Union[Generator[str, None, None], Generator[Future[str], None, None]]:
     """Get the current logs for an active or completed inference deployment
 
     Get the current logs for an active or completed inference deployment in the MosaicML platform.
     This returns the full logs as a ``str``, as they exist at the time the request is
     made.
 
@@ -63,25 +66,27 @@
             If the the call takes too long, a :exc:`~concurrent.futures.TimeoutError`
             will be raised. If ``future`` is ``True``, this value will be ignored.
         future (``bool``): Return the output as a :class:`~concurrent.futures.Future` . If True, the
             call to :func:`get_inference_deployment_logs` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the log text, use ``return_value.result()`` with an optional
             ``timeout`` argument.
+        failed (``bool``): Return the logs of the latest failed deployment if ``True``.
+            ``False`` by default.
 
     Returns:
         If future is False:
             The full log text for a inference deployment at the time of the request as a :obj:`str`
         Otherwise:
             A :class:`~concurrent.futures.Future` for the log text
     """
     # Convert to strings
     deployment_name = deployment.name if isinstance(deployment, InferenceDeployment) else deployment
 
-    filters: Dict[str, Any] = {'name': deployment_name}
+    filters: Dict[str, Any] = {'name': deployment_name, 'failed': failed}
     if restart:
         filters['restartCount'] = restart
 
     variables = {VARIABLE_DATA_NAME: filters}
 
     cfg = MCLIConfig.load_config()
     cfg.update_entity(variables[VARIABLE_DATA_NAME], set_user=False)
```

### Comparing `mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_ping.py` & `mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/inference_deployments/api_update_inference_deployments.py` & `mosaicml-cli-0.5.1/mcli/api/inference_deployments/api_update_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/mint/shell.py` & `mosaicml-cli-0.5.1/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/mint/tty.py` & `mosaicml-cli-0.5.1/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/model/__init__.py` & `mosaicml-cli-0.5.1/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.5.1/mcli/api/model/cluster_details.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.5.1/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/model/run.py` & `mosaicml-cli-0.5.1/mcli/api/model/run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/runs/__init__.py` & `mosaicml-cli-0.5.1/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/runs/api_create_interactive_run.py` & `mosaicml-cli-0.5.1/mcli/api/runs/api_create_interactive_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,33 +49,33 @@
   }}
 }}"""
 
 
 @overload
 def create_interactive_run(run: Union[RunConfig, FinalRunConfig],
                            *,
-                           hours: Optional[float] = None,
                            timeout: Optional[float] = 10,
+                           seconds: Optional[int] = None,
                            future: Literal[False] = False) -> Run:
     ...
 
 
 @overload
 def create_interactive_run(run: Union[RunConfig, FinalRunConfig],
                            *,
-                           hours: Optional[float] = None,
                            timeout: Optional[float] = None,
+                           seconds: Optional[int] = None,
                            future: Literal[True] = True) -> Future[Run]:
     ...
 
 
 def create_interactive_run(run: Union[RunConfig, FinalRunConfig],
                            *,
-                           hours: Optional[float] = None,
                            timeout: Optional[float] = 10,
+                           seconds: Optional[int] = None,
                            future: bool = False) -> Union[Run, Future[Run]]:
     """Launch an interactive run in the MosaicML platform
 
     Users are not required to provide a name, image, or 'hours' variable for an interactive 
     run. If these variables are not provided, they will be filled in with defaults. If the 
     user provides a value for the 'command' variable, this will be overwritten with 
     `sleep <hours>`, where <hours> is the value of the 'hours' variable.
@@ -99,15 +99,15 @@
     """
 
     if isinstance(run, RunConfig):
         run = FinalRunConfig.finalize_config(run)
 
     variables = {
         VARIABLE_DATA_NAME: {
-            **run.to_create_run_api_input(), "seconds": int(3600 * hours) if hours else None
+            **run.to_create_run_api_input(), "seconds": seconds
         },
     }
 
     response = run_singular_mapi_request(
         query=QUERY,
         query_function=QUERY_FUNCTION,
         return_model_type=Run,
```

### Comparing `mosaicml-cli-0.5.0/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.5.1/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.5.1/mcli/api/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.5.1/mcli/api/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.5.1/mcli/api/runs/api_get_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.5.1/mcli/api/runs/api_start_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.5.1/mcli/api/runs/api_stop_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/runs/api_update_run.py` & `mosaicml-cli-0.5.1/mcli/api/runs/api_update_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,40 +51,43 @@
                update_run_data: Optional[Dict[str, Any]] = None,
                *,
                preemptible: Optional[bool] = None,
                priority: Optional[str] = None,
                max_retries: Optional[int] = None,
                retry_on_system_failure: Optional[bool] = None,
                timeout: Optional[float] = 10,
-               future: Literal[False] = False) -> Run:
+               future: Literal[False] = False,
+               max_duration: Optional[float] = None) -> Run:
     ...
 
 
 @overload
 def update_run(run: Union[str, Run],
                update_run_data: Optional[Dict[str, Any]] = None,
                *,
                preemptible: Optional[bool] = None,
                priority: Optional[str] = None,
                max_retries: Optional[int] = None,
                retry_on_system_failure: Optional[bool] = None,
                timeout: Optional[float] = None,
-               future: Literal[True] = True) -> Future[Run]:
+               future: Literal[True] = True,
+               max_duration: Optional[float] = None) -> Future[Run]:
     ...
 
 
 def update_run(run: Union[str, Run],
                update_run_data: Optional[Dict[str, Any]] = None,
                *,
                preemptible: Optional[bool] = None,
                priority: Optional[str] = None,
                max_retries: Optional[int] = None,
                retry_on_system_failure: Optional[bool] = None,
                timeout: Optional[float] = 10,
-               future: bool = False):
+               future: bool = False,
+               max_duration: Optional[float] = None):
     """Update a run's data in the MosaicML platform.
 
     Any values that are not specified will not be modified.
 
     Args:
         run (``Optional[str | ``:class:`~mcli.api.model.run.Run` ``]``):
             A run or run name to update. Using :class:`~mcli.api.model.run.Run` objects is most
@@ -97,14 +100,15 @@
         priority (str): Update the priority of the run to `low`, `medium`, or `high`; default is `medium`
         max_retries (int): Update the max number of times the run can be retried; default is 0
         retry_on_system_failure (bool): Update whether the run should be retried on system failure
             (i.e. a node failure); default is False
         timeout (``Optional[float]``): Time, in seconds, in which the call should complete.
             If the call takes too long, a :exc:`~concurrent.futures.TimeoutError`
             will be raised. If ``future`` is ``True``, this value will be ignored.
+        max_duration: Update the max time that a run can run for (in hours). 
         future (``bool``): Return the output as a :class:`~concurrent.futures.Future`. If True, the
             call to :func:`update_run` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the list of :class:`~mcli.api.model.run.Run` output,
             use ``return_value.result()`` with an optional ``timeout`` argument.
 
     Raises:
@@ -123,14 +127,16 @@
         update_run_data['preemptible'] = preemptible
     if priority is not None:
         update_run_data['priority'] = priority
     if max_retries is not None:
         update_run_data['maxRetries'] = max_retries
     if retry_on_system_failure is not None:
         update_run_data['retryOnSystemFailure'] = retry_on_system_failure
+    if max_duration is not None:
+        update_run_data['maxDurationSeconds'] = int(3600 * max_duration)
 
     variables = {
         VARIABLE_DATA_GET_RUNS: {
             'filters': {
                 'name': {
                     'in': [run.name if isinstance(run, Run) else run]
                 },
```

### Comparing `mosaicml-cli-0.5.0/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.5.1/mcli/api/runs/api_update_run_metadata.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.5.1/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.5.1/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.5.1/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.5.1/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.5.1/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/typing_future.py` & `mosaicml-cli-0.5.1/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.5.1/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/api/utils.py` & `mosaicml-cli-0.5.1/mcli/api/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/cli.py` & `mosaicml-cli-0.5.1/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.5.1/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.5.1/mcli/cli/common/run_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.5.1/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.5.1/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.5.1/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.5.1/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.5.1/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.5.1/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.5.1/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.5.1/mcli/cli/m_describe/describe_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.5.1/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.5.1/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_get/display.py` & `mosaicml-cli-0.5.1/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.5.1/mcli/cli/m_get/inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.5.1/mcli/cli/m_get/m_get.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.5.1/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.5.1/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_get/users.py` & `mosaicml-cli-0.5.1/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.5.1/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.5.1/mcli/cli/m_interactive/m_interactive.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,19 +47,19 @@
 
 
 def interactive(
     name: Optional[str] = None,
     cluster: Optional[str] = None,
     gpu_type: Optional[str] = None,
     gpus: Optional[int] = None,
-    hours: Optional[float] = None,
     image: Optional[str] = None,
     rank: int = 0,
     connect: bool = True,
     command: Optional[str] = None,
+    seconds: Optional[int] = None,
     **kwargs,
 ) -> int:
     del kwargs
 
     if not cluster:
         clusters = get_clusters()
         if not clusters:
@@ -82,15 +82,15 @@
             name=name,
             image=image,
             gpu_num=gpus,
             gpu_type=gpu_type,
             cluster=cluster,
         )
 
-        run = create_interactive_run(run_config, hours=hours)
+        run = create_interactive_run(run_config, seconds=seconds)
         ready = wait_for_run(run)
         if not ready:
             return 1
 
         if not connect:
             return 0
 
@@ -115,47 +115,54 @@
     hrs: Optional[float] = None,
     hours: Optional[float] = None,
     image: str = 'mosaicml/pytorch',
     connect: bool = True,
     rank: int = 0,
     command: Optional[str] = None,
     tmux: Optional[bool] = None,
+    max_duration: Optional[float] = None,
     **kwargs,
 ) -> int:
     del kwargs
 
     # Hours can be specified as a positional argument (hrs) or named argument (hours)
     if hours and hrs:
         logger.error(f'{FAIL} The duration of your interactive session was specified twice. '
                      'Please use only the positional argument or --hours. '
                      'See mcli interactive --help for more details.')
 
-    hours = hrs or hours
-    if hours is None:
+    seconds = None
+    hours = hrs or hours or max_duration
+    if hours is not None:
+        seconds = int(hours * 3600)
+
+    if seconds is None:
         logger.error(f"{FAIL} Please specify the duration of your interactive session. "
                      'See mcli interactive --help for details')
         return 1
 
+    if seconds <= 0:
+        logger.error(f"{FAIL} Please specify a nonzero value for your run's max duration. "
+                     'See mcli interactive --help for details')
+        return 1
+
     if tmux:
         command = get_tmux_command()
 
-    return interactive(
-        name=name,
-        cluster=cluster,
-        gpu_type=gpu_type,
-        gpus=gpus,
-        hours=hours,
-        image=image,
-        rank=rank,
-        connect=connect,
-        command=command,
-    )
+    return interactive(name=name,
+                       cluster=cluster,
+                       gpu_type=gpu_type,
+                       gpus=gpus,
+                       image=image,
+                       rank=rank,
+                       connect=connect,
+                       command=command,
+                       seconds=seconds)
 
 
-# TODO: Move into mcli/cli/m_interactive/m_interactive.py once kube mcli deprecated
 def configure_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
 
     hrs_grp = parser.add_mutually_exclusive_group()
     hrs_grp.add_argument(
         'hrs',
         metavar='HOURS',
         nargs='?',
@@ -180,14 +187,19 @@
 
     parser.add_argument(
         '--image',
         default='mosaicml/pytorch',
         help='Docker image to use',
     )
 
+    parser.add_argument('--max-duration',
+                        type=float,
+                        help='The maximum time that a run should run for (in hours). If the run exceeds this '
+                        'duration, it will be stopped.')
+
     cluster_arguments = parser.add_argument_group(
         'Compute settings',
         'These settings are used to determine the cluster and compute resources to use for your interactive session',
     )
     cluster_parser = cluster_arguments.add_argument(
         '--cluster',
         default=None,
```

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_kube/m_get_config.py` & `mosaicml-cli-0.5.1/mcli/cli/m_kube/m_get_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_kube/m_kube.py` & `mosaicml-cli-0.5.1/mcli/cli/m_kube/m_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_kube/m_merge_config.py` & `mosaicml-cli-0.5.1/mcli/cli/m_kube/m_merge_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_kube/utils.py` & `mosaicml-cli-0.5.1/mcli/cli/m_kube/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.5.1/mcli/cli/m_log/m_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,17 @@
 > mcli get deployment logs deploy-1234
 
 # By default, the logs for the latest deployment will be retrieved
 > mcli get deployment logs
 
 # View the logs of a specific restart in a deployment
 > mcli get deployment logs deploy-1234 --restart 5
+
+# View the logs for a failed deployment
+> mcli get deployment logs deploy-1234 --failed
 """
 
 
 def _get_run_logs(run: Run, follow: bool, rank: Optional[int], failed: bool,
                   resumption: Optional[int]) -> Tuple[Optional[str], int]:
 
     if run.status == RunStatus.FAILED and not failed and rank is None:
@@ -108,16 +111,16 @@
             # replicated in `follow_run_logs`. We'll do that here for parity
             if line:
                 last_line = line
                 print(line, end='')
         return last_line, int(0)
 
 
-def _get_deployment_logs(deploy: InferenceDeployment, restart) -> Tuple[Optional[str], int]:
-    log_lines = get_inference_deployment_logs(deploy, restart=restart)
+def _get_deployment_logs(deploy: InferenceDeployment, restart, failed) -> Tuple[Optional[str], int]:
+    log_lines = get_inference_deployment_logs(deploy, restart=restart, failed=failed)
     last_line: Optional[str] = None
     for line in log_lines:
         # When using progress bars we randomly get newlines added. By default,
         # kubernetes does not return empty lines when streaming, which is
         # replicated in `follow_run_logs`. We'll do that here for parity
         if line:
             last_line = line
@@ -168,15 +171,15 @@
         last_line: Optional[str] = None
         #Have to check type to satisfy pyright
         if isinstance(submissions[0], Run):
             last_line, err = _get_run_logs(submissions[0], follow, rank, failed, resumption)
             if err == 1:
                 return 1
         elif isinstance(submissions[0], InferenceDeployment):
-            last_line, err = _get_deployment_logs(submissions[0], restart)
+            last_line, err = _get_deployment_logs(submissions[0], restart, failed)
             if err == 1:
                 return 1
 
         # Progress bars are weird. Let's add a final newline so that if the printing
         # ends on an incompleted progress bar, it isn't erased
         if last_line:
             print('', file=sys.stderr)
@@ -204,19 +207,25 @@
 
     submission_parser = parser.add_argument(
         'submission_name',
         metavar='DEPLOYMENT',
         help='The name of the inference deployment to fetch logs for.',
     )
     submission_parser.completer = utils_completers.DeploymentNameCompleter()  # pyright: ignore
-    parser.add_argument('--restart',
-                        type=int,
-                        default=None,
-                        help='Which restart to fetch logs for. If not provided, will fetch logs of most recent restart')
-
+    restart_grp = parser.add_mutually_exclusive_group()
+    restart_grp.add_argument(
+        '--restart',
+        type=int,
+        default=None,
+        help='Which restart to fetch logs for. If not provided, will fetch logs of most recent restart')
+    restart_grp.add_argument('--failed',
+                             action='store_true',
+                             dest='failed',
+                             default=False,
+                             help='Get the logs of the latest failed deployment')
     return parser
 
 
 def configure_runs_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
     parser.set_defaults(func=partial(get_logs, SubmissionType.TRAINING))
     submimssion_name_parser = parser.add_argument(
         'submission_name',
```

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.5.1/mcli/cli/m_ping/m_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.5.1/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.5.1/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.5.1/mcli/cli/m_run/m_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,63 +99,71 @@
     override_image: Optional[str] = None,
     override_name: Optional[str] = None,
     override_priority: Optional[str] = None,
     override_preemptible: Optional[bool] = None,
     override_max_retries: Optional[int] = None,
     override_nodes: Optional[int] = None,
     override_instance: Optional[str] = None,
+    override_max_duration: Optional[float] = None,
     **kwargs,
 ) -> int:
     del kwargs
 
     runs_to_modify = sum([file is not None, clone is not None, restart_run is not None])
     if runs_to_modify != 1:
         print_help()
         raise MAPIException(HTTPStatus.BAD_REQUEST, "Must specify a file, a run to clone, or a run to restart.")
     if file:
         run_config = RunConfig.from_file(path=file)
+
     elif clone:
         run = get_run(clone)
         if run.submitted_config is None:
             raise MAPIException(HTTPStatus.NOT_FOUND, f"Could not retrieve configuration from run {clone}")
         run_config = run.submitted_config
     elif restart_run:
         configs = any([
             override_cluster is not None,
             override_gpu_type is not None,
             override_gpu_num is not None,
             override_instance is not None,
             override_image is not None,
             override_name is not None,
             override_nodes is not None,
+            override_max_duration is not None,
         ])
         if configs:
             logger.info(f'{WARN} New configurations will be ignored when restarting a run.')
             restart_to_clone = query_yes_no(f'Would you like to clone {restart_run} with these configurations instead?')
             if not restart_to_clone:
                 return 0
             run = get_run(restart_run)
             if run.submitted_config is None:
                 raise MAPIException(HTTPStatus.NOT_FOUND, f"Could not retrieve configuration from run {restart_run}")
             run_config = run.submitted_config
         else:
-            scheduling_config = any(
-                [override_priority is not None, override_preemptible is not None, override_max_retries is not None])
+            scheduling_config = any([
+                override_priority is not None, override_preemptible is not None, override_max_retries is not None,
+                override_max_duration is not None
+            ])
             if scheduling_config:
                 update_string = ''
                 if override_preemptible is not None:
                     update_string += f" Set preemptible to {override_preemptible}."
                 if override_priority is not None:
                     update_string += f" Set priority to {override_priority}."
                 if override_max_retries is not None:
                     update_string += f" Set max_retries to {override_max_retries}."
+                if override_max_duration is not None:
+                    update_string += f"Set max-duration to ${override_max_duration}"
                 update_run(restart_run,
                            preemptible=override_preemptible,
                            priority=override_priority,
-                           max_retries=override_max_retries)
+                           max_retries=override_max_retries,
+                           max_duration=override_max_duration)
                 logger.info(f'{OK} Updated {restart_run}.{update_string}')
             with console_status('Restarting run...'):
                 run = start_run(restart_run, timeout=None)
 
             return finish_run(run, follow, restarted=True)
     else:
         return print_help()
@@ -182,14 +190,17 @@
 
     if override_preemptible is not None:
         run_config.scheduling['preemptible'] = override_preemptible
 
     if override_max_retries is not None:
         run_config.scheduling['max_retries'] = override_max_retries
 
+    if override_max_duration is not None:
+        run_config.scheduling["max_duration_seconds"] = int(3600 * override_max_duration)
+
     if override_instance is not None:
         run_config.compute['instance'] = override_instance
 
     if override_nodes is not None:
         run_config.compute['nodes'] = override_nodes
 
     with console_status('Submitting run...'):
@@ -304,8 +315,13 @@
     )
 
     instance_parser = parser.add_argument(
         '--instance',
         dest='override_instance',
         help='Optional override for instance type',
     )
+
+    parser.add_argument('--max-duration',
+                        type=float,
+                        dest="override_max_duration",
+                        help="Optional override for the max duration (in hours) of a run")
     instance_parser.completer = utils_completers.InstanceNameCompleter()  # pyright: ignore
```

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.5.1/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.5.1/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.5.1/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.5.1/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_set_unset/organization.py` & `mosaicml-cli-0.5.1/mcli/cli/m_set_unset/organization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.5.1/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.5.1/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_update/m_update.py` & `mosaicml-cli-0.5.1/mcli/cli/m_update/m_update.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,31 +34,35 @@
     parser.print_help()
     return 0
 
 
 @cli_error_handler('mcli update run')
 def _update_run(
     run_name: str,
-    priority: Optional[str] = None,  # Default to None to not change value
-    preemptible: Optional[bool] = None,  # Default to None to not change value
-    max_retries: Optional[int] = None,  # Default to None to not change value
+    priority: Optional[str] = None,
+    preemptible: Optional[bool] = None,
+    max_retries: Optional[int] = None,
+    max_duration: Optional[float] = None,
     **kwargs,
 ) -> int:
     del kwargs
-    update_fields = any([preemptible is not None, priority is not None, max_retries is not None])
+    update_fields = any(
+        [preemptible is not None, priority is not None, max_retries is not None, max_duration is not None])
     if not update_fields:
         raise MAPIException(HTTPStatus.BAD_REQUEST, "Must specify preemptible, priority, or max_retries to update")
     update_string = ""
     if preemptible is not None:
         update_string += f"Set preemptible to {preemptible}.\n"
     if priority is not None:
         update_string += f"Set priority to {priority}.\n"
     if max_retries is not None:
         update_string += f"Set max_retries to {max_retries}.\n"
-    update_run(run_name, preemptible=preemptible, priority=priority, max_retries=max_retries)
+    if max_duration is not None:
+        update_string += f"Set max-duration to {int(3600 * max_duration)}"
+    update_run(run_name, preemptible=preemptible, priority=priority, max_retries=max_retries, max_duration=max_duration)
 
     logger.info(f'{OK} Updated {run_name}.\n{update_string}')
     return 0
 
 
 @cli_error_handler('mcli update deployment')
 def _update_deployment(
@@ -103,15 +107,16 @@
                                              formatter_class=argparse.RawDescriptionHelpFormatter,
                                              epilog=UPDATE_DEPLOYMENT_EXAMPLE)
     deployment_name_parser = deployment_parser.add_argument(
         'deployment_name',
         type=str,
         help='The name of the deployment',
     )
-    deployment_name_parser.completer = utils_completers.DeploymentNameCompleter()  # pyright: ignore
+    # pyright: ignore
+    deployment_name_parser.completer = utils_completers.DeploymentNameCompleter()
     deployment_parser.add_argument('--image', dest='image', help='Update deployment image file')
     deployment_parser.add_argument('--replicas', dest='replicas', type=int, help='Update deployment replica count')
     deployment_parser.set_defaults(func=_update_deployment)
 
 
 def run_argparser(subparser: argparse._SubParsersAction) -> None:
     run_parser = subparser.add_parser(
@@ -136,14 +141,21 @@
                        variable_name='preemptible',
                        true_description='Allows runs to be stopped and re-queued by higher priority jobs',
                        false_description='Disallows runs from being stopped and re-queued by higher priority jobs')
     run_parser.add_argument('--max-retries',
                             type=int,
                             dest='max_retries',
                             help='Update max number of times a run should be retried (default 0)')
+    run_parser.add_argument(
+        '--max-duration',
+        type=float,
+        dest='max_duration',
+        help='Update the maximum time that a run should run for (in hours). If the run exceeds this '
+        'duration, it will be stopped.')
+
     run_parser.set_defaults(func=_update_run)
 
 
 def _configure_argparser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
     subparsers = parser.add_subparsers(title='MCLI Updates', help='DESCRIPTION', metavar='OBJECT')
     parser.set_defaults(func=update_entrypoint, parser=parser)
     run_argparser(subparsers)
```

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.5.1/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_util/util.py` & `mosaicml-cli-0.5.1/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/cli/m_watchdog/m_watchdog.py` & `mosaicml-cli-0.5.1/mcli/cli/m_watchdog/m_watchdog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/config.py` & `mosaicml-cli-0.5.1/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/models/__init__.py` & `mosaicml-cli-0.5.1/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/models/gpu_type.py` & `mosaicml-cli-0.5.1/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.5.1/mcli/models/inference_deployment_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/models/mcli_secret.py` & `mosaicml-cli-0.5.1/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/models/run_config.py` & `mosaicml-cli-0.5.1/mcli/models/run_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """Typed dictionary for nested scheduling configurations"""
     priority: Optional[str]
     resumable: Optional[bool]  # TODO: deprecate resumable
     preemptible: Optional[bool]
     retryOnSystemFailure: Optional[bool]
     max_retries: Optional[int]
     retry_on_system_failure: Optional[bool]
+    max_duration_seconds: Optional[int]
 
 
 def strip_nones(d: Dict[str, Any]) -> Dict[str, Any]:
     """Remove all keys with None values from a dictionary"""
     return {k: v for k, v in d.items() if v is not None}
 
 
@@ -98,20 +99,15 @@
         'command': 'command',
         'entrypoint': 'entrypoint',
         'scheduling': 'scheduling',
         'compute': 'compute',
         'metadata': 'metadata',
     }
 
-    _optional_properties = {
-        'partitions',
-        'scheduling',
-        'compute',
-        'metadata',
-    }
+    _optional_properties = {'partitions', 'scheduling', 'compute', 'metadata'}
 
     def __str__(self) -> str:
         return yaml.safe_dump(asdict(self))
 
     def __post_init__(self):
         self.cluster = self.cluster or self.platform
 
@@ -338,14 +334,15 @@
 
 class SchedulingTranslation(Translation[SchedulingConfig, Dict[str, Any]]):
     """Translate scheduling configs to and from MAPI"""
 
     translations = {
         "maxRetries": "max_retries",
         "retryOnSystemFailure": "retry_on_system_failure",
+        "maxDurationSeconds": "max_duration_seconds"
     }
 
     @classmethod
     def from_mapi(cls, value: Dict[str, Any]) -> SchedulingConfig:
         extracted = SchedulingConfig(**{cls.translations.get(k, k): v for k, v in value.items() if k != "priorityInt"})
         return extracted
 
@@ -408,15 +405,14 @@
     partitions: Optional[List[str]] = None
     optimization_level: Optional[int] = None  # deprecated
     integrations: List[Dict[str, Any]] = field(default_factory=list)
     env_variables: List[Dict[str, str]] = field(default_factory=list)
     scheduling: SchedulingConfig = field(default_factory=SchedulingConfig)
     compute: ComputeConfig = field(default_factory=ComputeConfig)
     metadata: Dict[str, Any] = field(default_factory=dict)
-
     command: str = ''
     parameters: Dict[str, Any] = field(default_factory=dict)
     entrypoint: str = ''
 
     _property_translations = {
         'runName': 'name',
         'gpuNum': 'gpu_num',
```

### Comparing `mosaicml-cli-0.5.0/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.5.1/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.5.1/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.5.1/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.5.1/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.5.1/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.5.1/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.5.1/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.5.1/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.5.1/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.5.1/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.5.1/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.5.1/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.5.1/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.5.1/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.5.1/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.5.1/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/sdk/__init__.py` & `mosaicml-cli-0.5.1/mcli/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_cli.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_completers.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_completers.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_config.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_date.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_docker.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_logging.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_model.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_rich.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_types.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.5.1/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mcli/version.py` & `mosaicml-cli-0.5.1/mcli/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.5.0/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.5.1/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.5.0
+Version: 0.5.1
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.5.0/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.5.1/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.5.1/mosaicml_cli.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -9,47 +9,47 @@
 questionary>=1.10.0
 rich>=12.6.0
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 validators>=0.20.0
 
 [all]
-sphinxext-opengraph==0.8.2
-build>=0.10.0
-sphinx-panels==0.6.0
-sphinxcontrib-serializinghtml==1.1.5
-docutils>=0.17.0
-pytest-cov>=4.0.0
-pre-commit>=2.17.0
-pyright==1.1.256
-sphinxcontrib-devhelp>=1.0.2
+sphinxcontrib-qthelp>=1.0.3
 sphinxcontrib-htmlhelp>=2.0.0
-sphinxcontrib-applehelp>=1.0.2
-furo==2022.9.29
-yapf>=0.33.0
+toml>=0.10.2
+sphinx-markdown-tables==0.0.17
+myst-parser>=0.16.1
 pylint>=2.12.2
+sphinx==4.4.0
+sphinxcontrib-devhelp>=1.0.2
+sphinx-argparse==0.4.0
 pytest-mock>=3.7.0
+sphinx-panels==0.6.0
+pyright==1.1.256
+sphinx-rtd-theme==1.0.0
+twine>=4.0.2
 radon>=5.1.0
-sphinx==4.4.0
-sphinxemoji==0.2.0
-sphinxcontrib-qthelp>=1.0.3
+pytest-cov>=4.0.0
+sphinxcontrib-jsmath>=1.0.1
+sphinxext-opengraph==0.8.2
+yapf>=0.33.0
+sphinx-design
 sphinx-copybutton==0.5.2
-sphinx-argparse==0.4.0
+pre-commit>=2.17.0
 sphinxcontrib-katex==0.9.4
-sphinxcontrib-images>=0.9.4
-sphinxcontrib-jsmath>=1.0.1
-myst-parser>=0.16.1
-sphinx-markdown-tables==0.0.17
-toml>=0.10.2
-sphinx-rtd-theme==1.0.0
+docutils>=0.17.0
 pytest>=6.2.5
+build>=0.10.0
+sphinxcontrib-applehelp>=1.0.2
 isort>=5.9.3
-twine>=4.0.2
-sphinx-design
+sphinxcontrib-serializinghtml==1.1.5
 sphinx_external_toc==0.3.0
+sphinxcontrib-images>=0.9.4
+furo==2022.9.29
+sphinxemoji==0.2.0
 
 [dev]
 build>=0.10.0
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright==1.1.256
```

### Comparing `mosaicml-cli-0.5.0/pyproject.toml` & `mosaicml-cli-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/setup.py` & `mosaicml-cli-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/tests/test_config.py` & `mosaicml-cli-0.5.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.5.0/tests/test_upgrade.py` & `mosaicml-cli-0.5.1/tests/test_upgrade.py`

 * *Files identical despite different names*

