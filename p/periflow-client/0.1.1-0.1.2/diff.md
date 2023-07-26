# Comparing `tmp/periflow_client-0.1.1.tar.gz` & `tmp/periflow_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periflow_client-0.1.1.tar", max compression
+gzip compressed data, was "periflow_client-0.1.2.tar", max compression
```

## Comparing `periflow_client-0.1.1.tar` & `periflow_client-0.1.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     3501 2023-07-25 04:03:34.042855 periflow_client-0.1.1/LICENSE
--rw-r--r--   0        0        0     7948 2023-07-20 12:32:34.224165 periflow_client-0.1.1/README.md
--rw-r--r--   0        0        0      820 2023-07-20 12:32:34.262789 periflow_client-0.1.1/periflow/__init__.py
--rw-r--r--   0        0        0     4410 2023-07-20 12:32:34.262864 periflow_client-0.1.1/periflow/auth.py
--rw-r--r--   0        0        0      188 2023-07-20 12:32:34.262945 periflow_client-0.1.1/periflow/cli/__init__.py
--rw-r--r--   0        0        0    19009 2023-07-25 03:49:51.897018 periflow_client-0.1.1/periflow/cli/checkpoint.py
--rw-r--r--   0        0        0    10321 2023-07-20 12:32:34.263102 periflow_client-0.1.1/periflow/cli/credential.py
--rw-r--r--   0        0        0    18875 2023-07-25 03:49:56.899224 periflow_client-0.1.1/periflow/cli/deployment.py
--rw-r--r--   0        0        0     5700 2023-07-20 12:32:34.263272 periflow_client-0.1.1/periflow/cli/group.py
--rw-r--r--   0        0        0     2445 2023-07-20 12:32:34.263329 periflow_client-0.1.1/periflow/cli/key.py
--rw-r--r--   0        0        0     6077 2023-07-25 04:03:34.043963 periflow_client-0.1.1/periflow/cli/main.py
--rw-r--r--   0        0        0     9491 2023-07-20 12:32:34.263483 periflow_client-0.1.1/periflow/cli/project.py
--rw-r--r--   0        0        0     1676 2023-07-25 03:49:56.899466 periflow_client-0.1.1/periflow/cli/vm.py
--rw-r--r--   0        0        0      125 2023-07-20 12:32:34.263645 periflow_client-0.1.1/periflow/client/__init__.py
--rw-r--r--   0        0        0    15578 2023-07-20 12:32:34.263735 periflow_client-0.1.1/periflow/client/base.py
--rw-r--r--   0        0        0     2651 2023-07-20 12:32:34.263798 periflow_client-0.1.1/periflow/client/checkpoint.py
--rw-r--r--   0        0        0     2603 2023-07-20 12:32:34.263898 periflow_client-0.1.1/periflow/client/credential.py
--rw-r--r--   0        0        0     7402 2023-07-20 12:32:34.263972 periflow_client-0.1.1/periflow/client/deployment.py
--rw-r--r--   0        0        0     3069 2023-07-20 12:32:34.264036 periflow_client-0.1.1/periflow/client/file.py
--rw-r--r--   0        0        0     5904 2023-07-20 12:32:34.264109 periflow_client-0.1.1/periflow/client/group.py
--rw-r--r--   0        0        0     3581 2023-07-20 12:32:34.264158 periflow_client-0.1.1/periflow/client/project.py
--rw-r--r--   0        0        0     7361 2023-07-20 12:32:34.264235 periflow_client-0.1.1/periflow/client/user.py
--rw-r--r--   0        0        0       98 2023-07-20 12:32:34.264311 periflow_client-0.1.1/periflow/cloud/__init__.py
--rw-r--r--   0        0        0     9622 2023-07-20 12:32:34.264393 periflow_client-0.1.1/periflow/cloud/storage.py
--rw-r--r--   0        0        0      107 2023-07-20 12:32:34.264482 periflow_client-0.1.1/periflow/configurator/__init__.py
--rw-r--r--   0        0        0     1587 2023-07-20 12:32:34.264550 periflow_client-0.1.1/periflow/configurator/base.py
--rw-r--r--   0        0        0     4067 2023-07-20 12:32:34.264648 periflow_client-0.1.1/periflow/configurator/credential.py
--rw-r--r--   0        0        0     3112 2023-07-20 12:32:34.264715 periflow_client-0.1.1/periflow/configurator/deployment.py
--rw-r--r--   0        0        0     1753 2023-07-20 12:32:34.264778 periflow_client-0.1.1/periflow/context.py
--rw-r--r--   0        0        0      105 2023-07-20 12:32:34.264853 periflow_client-0.1.1/periflow/converter/__init__.py
--rw-r--r--   0        0        0    15051 2023-07-20 12:58:47.707975 periflow_client-0.1.1/periflow/converter/base.py
--rw-r--r--   0        0        0     5020 2023-07-20 12:32:34.265037 periflow_client-0.1.1/periflow/converter/interface.py
--rw-r--r--   0        0        0     2397 2023-07-20 12:32:34.265101 periflow_client-0.1.1/periflow/converter/maps.py
--rw-r--r--   0        0        0    13345 2023-07-20 12:32:34.265241 periflow_client-0.1.1/periflow/converter/models/blenderbot.py
--rw-r--r--   0        0        0     8689 2023-07-20 12:32:34.265314 periflow_client-0.1.1/periflow/converter/models/bloom.py
--rw-r--r--   0        0        0     7252 2023-07-20 12:32:34.265389 periflow_client-0.1.1/periflow/converter/models/codegen.py
--rw-r--r--   0        0        0     9706 2023-07-20 12:32:34.265458 periflow_client-0.1.1/periflow/converter/models/falcon.py
--rw-r--r--   0        0        0     7060 2023-07-20 12:32:34.265533 periflow_client-0.1.1/periflow/converter/models/gpt2.py
--rw-r--r--   0        0        0    10454 2023-07-20 12:32:34.265601 periflow_client-0.1.1/periflow/converter/models/gpt_neox.py
--rw-r--r--   0        0        0     7122 2023-07-20 12:32:34.265672 periflow_client-0.1.1/periflow/converter/models/gptj.py
--rw-r--r--   0        0        0     7916 2023-07-25 03:49:51.897974 periflow_client-0.1.1/periflow/converter/models/llama.py
--rw-r--r--   0        0        0     7316 2023-07-20 12:32:34.265844 periflow_client-0.1.1/periflow/converter/models/mpt.py
--rw-r--r--   0        0        0     9390 2023-07-20 12:32:34.265915 periflow_client-0.1.1/periflow/converter/models/opt.py
--rw-r--r--   0        0        0    12615 2023-07-20 12:32:34.265998 periflow_client-0.1.1/periflow/converter/models/t5.py
--rw-r--r--   0        0        0     4456 2023-07-20 12:32:34.266070 periflow_client-0.1.1/periflow/converter/utils.py
--rw-r--r--   0        0        0     3318 2023-07-25 03:49:56.899802 periflow_client-0.1.1/periflow/enums.py
--rw-r--r--   0        0        0     5404 2023-07-20 12:32:34.266214 periflow_client-0.1.1/periflow/errors.py
--rw-r--r--   0        0        0     9505 2023-07-20 12:32:34.266322 periflow_client-0.1.1/periflow/formatter.py
--rw-r--r--   0        0        0      660 2023-07-20 12:32:34.266385 periflow_client-0.1.1/periflow/logging.py
--rw-r--r--   0        0        0       92 2023-07-20 12:32:34.266497 periflow_client-0.1.1/periflow/schema/__init__.py
--rw-r--r--   0        0        0       96 2023-07-20 12:32:34.266643 periflow_client-0.1.1/periflow/schema/api/__init__.py
--rw-r--r--   0        0        0       99 2023-07-20 12:32:34.266768 periflow_client-0.1.1/periflow/schema/api/v1/__init__.py
--rw-r--r--   0        0        0     2828 2023-07-20 12:32:34.266844 periflow_client-0.1.1/periflow/schema/api/v1/completion.py
--rw-r--r--   0        0        0      101 2023-07-20 12:32:34.266958 periflow_client-0.1.1/periflow/schema/resource/__init__.py
--rw-r--r--   0        0        0      104 2023-07-20 12:32:34.267053 periflow_client-0.1.1/periflow/schema/resource/v1/__init__.py
--rw-r--r--   0        0        0     3912 2023-07-25 03:49:51.898529 periflow_client-0.1.1/periflow/schema/resource/v1/attributes.py
--rw-r--r--   0        0        0     2353 2023-07-20 12:32:34.267192 periflow_client-0.1.1/periflow/schema/resource/v1/checkpoint.py
--rw-r--r--   0        0        0     1358 2023-07-20 12:32:34.267258 periflow_client-0.1.1/periflow/schema/resource/v1/credential.py
--rw-r--r--   0        0        0     2027 2023-07-20 12:32:34.267312 periflow_client-0.1.1/periflow/schema/resource/v1/deployment.py
--rw-r--r--   0        0        0       88 2023-07-20 12:32:34.267397 periflow_client-0.1.1/periflow/sdk/__init__.py
--rw-r--r--   0        0        0      102 2023-07-20 12:32:34.267511 periflow_client-0.1.1/periflow/sdk/api/__init__.py
--rw-r--r--   0        0        0     5799 2023-07-20 12:32:34.267596 periflow_client-0.1.1/periflow/sdk/api/base.py
--rw-r--r--   0        0        0    25709 2023-07-20 12:32:34.267670 periflow_client-0.1.1/periflow/sdk/api/completion.py
--rw-r--r--   0        0        0     1836 2023-07-20 12:32:34.267758 periflow_client-0.1.1/periflow/sdk/init.py
--rw-r--r--   0        0        0      112 2023-07-20 12:32:34.267862 periflow_client-0.1.1/periflow/sdk/resource/__init__.py
--rw-r--r--   0        0        0      733 2023-07-20 12:32:34.267911 periflow_client-0.1.1/periflow/sdk/resource/base.py
--rw-r--r--   0        0        0    31401 2023-07-25 03:49:51.898894 periflow_client-0.1.1/periflow/sdk/resource/checkpoint.py
--rw-r--r--   0        0        0     4036 2023-07-20 12:32:34.268103 periflow_client-0.1.1/periflow/sdk/resource/credential.py
--rw-r--r--   0        0        0    17719 2023-07-25 03:49:56.900175 periflow_client-0.1.1/periflow/sdk/resource/deployment.py
--rw-r--r--   0        0        0       97 2023-07-20 12:32:34.268333 periflow_client-0.1.1/periflow/utils/__init__.py
--rw-r--r--   0        0        0     4232 2023-07-20 12:32:34.268415 periflow_client-0.1.1/periflow/utils/format.py
--rw-r--r--   0        0        0    14539 2023-07-20 12:32:34.268558 periflow_client-0.1.1/periflow/utils/fs.py
--rw-r--r--   0        0        0     1303 2023-07-25 03:49:56.900640 periflow_client-0.1.1/periflow/utils/maps.py
--rw-r--r--   0        0        0      666 2023-07-20 12:32:34.268678 periflow_client-0.1.1/periflow/utils/prompt.py
--rw-r--r--   0        0        0     2265 2023-07-20 12:32:34.268742 periflow_client-0.1.1/periflow/utils/request.py
--rw-r--r--   0        0        0     1384 2023-07-20 12:32:34.268808 periflow_client-0.1.1/periflow/utils/testing.py
--rw-r--r--   0        0        0     1485 2023-07-20 12:32:34.268869 periflow_client-0.1.1/periflow/utils/url.py
--rw-r--r--   0        0        0     3552 2023-07-20 12:32:34.268951 periflow_client-0.1.1/periflow/utils/validate.py
--rw-r--r--   0        0        0     1513 2023-07-20 12:32:34.269017 periflow_client-0.1.1/periflow/utils/version.py
--rw-r--r--   0        0        0     3339 2023-07-25 04:03:34.044242 periflow_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     9600 1970-01-01 00:00:00.000000 periflow_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3501 2023-07-25 04:03:34.042855 periflow_client-0.1.2/LICENSE
+-rw-r--r--   0        0        0     7948 2023-07-20 12:32:34.224165 periflow_client-0.1.2/README.md
+-rw-r--r--   0        0        0      820 2023-07-20 12:32:34.262789 periflow_client-0.1.2/periflow/__init__.py
+-rw-r--r--   0        0        0     4410 2023-07-20 12:32:34.262864 periflow_client-0.1.2/periflow/auth.py
+-rw-r--r--   0        0        0      188 2023-07-20 12:32:34.262945 periflow_client-0.1.2/periflow/cli/__init__.py
+-rw-r--r--   0        0        0    19009 2023-07-25 03:49:51.897018 periflow_client-0.1.2/periflow/cli/checkpoint.py
+-rw-r--r--   0        0        0    10321 2023-07-20 12:32:34.263102 periflow_client-0.1.2/periflow/cli/credential.py
+-rw-r--r--   0        0        0    18875 2023-07-25 03:49:56.899224 periflow_client-0.1.2/periflow/cli/deployment.py
+-rw-r--r--   0        0        0     5142 2023-07-26 09:29:06.022605 periflow_client-0.1.2/periflow/cli/group.py
+-rw-r--r--   0        0        0     2445 2023-07-20 12:32:34.263329 periflow_client-0.1.2/periflow/cli/key.py
+-rw-r--r--   0        0        0     6051 2023-07-26 09:29:06.022825 periflow_client-0.1.2/periflow/cli/main.py
+-rw-r--r--   0        0        0     9526 2023-07-26 09:29:06.023043 periflow_client-0.1.2/periflow/cli/project.py
+-rw-r--r--   0        0        0     1676 2023-07-25 03:49:56.899466 periflow_client-0.1.2/periflow/cli/vm.py
+-rw-r--r--   0        0        0      125 2023-07-20 12:32:34.263645 periflow_client-0.1.2/periflow/client/__init__.py
+-rw-r--r--   0        0        0    15578 2023-07-20 12:32:34.263735 periflow_client-0.1.2/periflow/client/base.py
+-rw-r--r--   0        0        0     2651 2023-07-20 12:32:34.263798 periflow_client-0.1.2/periflow/client/checkpoint.py
+-rw-r--r--   0        0        0     2603 2023-07-20 12:32:34.263898 periflow_client-0.1.2/periflow/client/credential.py
+-rw-r--r--   0        0        0     7402 2023-07-20 12:32:34.263972 periflow_client-0.1.2/periflow/client/deployment.py
+-rw-r--r--   0        0        0     3069 2023-07-20 12:32:34.264036 periflow_client-0.1.2/periflow/client/file.py
+-rw-r--r--   0        0        0     5332 2023-07-26 09:29:06.023358 periflow_client-0.1.2/periflow/client/group.py
+-rw-r--r--   0        0        0     3581 2023-07-20 12:32:34.264158 periflow_client-0.1.2/periflow/client/project.py
+-rw-r--r--   0        0        0     7003 2023-07-26 09:29:06.023578 periflow_client-0.1.2/periflow/client/user.py
+-rw-r--r--   0        0        0       98 2023-07-20 12:32:34.264311 periflow_client-0.1.2/periflow/cloud/__init__.py
+-rw-r--r--   0        0        0     9622 2023-07-20 12:32:34.264393 periflow_client-0.1.2/periflow/cloud/storage.py
+-rw-r--r--   0        0        0      107 2023-07-20 12:32:34.264482 periflow_client-0.1.2/periflow/configurator/__init__.py
+-rw-r--r--   0        0        0     1587 2023-07-20 12:32:34.264550 periflow_client-0.1.2/periflow/configurator/base.py
+-rw-r--r--   0        0        0     4067 2023-07-20 12:32:34.264648 periflow_client-0.1.2/periflow/configurator/credential.py
+-rw-r--r--   0        0        0     3112 2023-07-20 12:32:34.264715 periflow_client-0.1.2/periflow/configurator/deployment.py
+-rw-r--r--   0        0        0     1753 2023-07-20 12:32:34.264778 periflow_client-0.1.2/periflow/context.py
+-rw-r--r--   0        0        0      105 2023-07-20 12:32:34.264853 periflow_client-0.1.2/periflow/converter/__init__.py
+-rw-r--r--   0        0        0    15051 2023-07-20 12:58:47.707975 periflow_client-0.1.2/periflow/converter/base.py
+-rw-r--r--   0        0        0     5020 2023-07-20 12:32:34.265037 periflow_client-0.1.2/periflow/converter/interface.py
+-rw-r--r--   0        0        0     2397 2023-07-20 12:32:34.265101 periflow_client-0.1.2/periflow/converter/maps.py
+-rw-r--r--   0        0        0    13345 2023-07-20 12:32:34.265241 periflow_client-0.1.2/periflow/converter/models/blenderbot.py
+-rw-r--r--   0        0        0     8689 2023-07-20 12:32:34.265314 periflow_client-0.1.2/periflow/converter/models/bloom.py
+-rw-r--r--   0        0        0     7252 2023-07-20 12:32:34.265389 periflow_client-0.1.2/periflow/converter/models/codegen.py
+-rw-r--r--   0        0        0     9706 2023-07-20 12:32:34.265458 periflow_client-0.1.2/periflow/converter/models/falcon.py
+-rw-r--r--   0        0        0     7060 2023-07-20 12:32:34.265533 periflow_client-0.1.2/periflow/converter/models/gpt2.py
+-rw-r--r--   0        0        0    10454 2023-07-20 12:32:34.265601 periflow_client-0.1.2/periflow/converter/models/gpt_neox.py
+-rw-r--r--   0        0        0     7122 2023-07-20 12:32:34.265672 periflow_client-0.1.2/periflow/converter/models/gptj.py
+-rw-r--r--   0        0        0     7916 2023-07-25 03:49:51.897974 periflow_client-0.1.2/periflow/converter/models/llama.py
+-rw-r--r--   0        0        0     7316 2023-07-20 12:32:34.265844 periflow_client-0.1.2/periflow/converter/models/mpt.py
+-rw-r--r--   0        0        0     9390 2023-07-20 12:32:34.265915 periflow_client-0.1.2/periflow/converter/models/opt.py
+-rw-r--r--   0        0        0    12615 2023-07-20 12:32:34.265998 periflow_client-0.1.2/periflow/converter/models/t5.py
+-rw-r--r--   0        0        0     4456 2023-07-20 12:32:34.266070 periflow_client-0.1.2/periflow/converter/utils.py
+-rw-r--r--   0        0        0     3318 2023-07-25 03:49:56.899802 periflow_client-0.1.2/periflow/enums.py
+-rw-r--r--   0        0        0     5404 2023-07-20 12:32:34.266214 periflow_client-0.1.2/periflow/errors.py
+-rw-r--r--   0        0        0     9505 2023-07-20 12:32:34.266322 periflow_client-0.1.2/periflow/formatter.py
+-rw-r--r--   0        0        0      660 2023-07-20 12:32:34.266385 periflow_client-0.1.2/periflow/logging.py
+-rw-r--r--   0        0        0       92 2023-07-20 12:32:34.266497 periflow_client-0.1.2/periflow/schema/__init__.py
+-rw-r--r--   0        0        0       96 2023-07-20 12:32:34.266643 periflow_client-0.1.2/periflow/schema/api/__init__.py
+-rw-r--r--   0        0        0       99 2023-07-20 12:32:34.266768 periflow_client-0.1.2/periflow/schema/api/v1/__init__.py
+-rw-r--r--   0        0        0     2828 2023-07-20 12:32:34.266844 periflow_client-0.1.2/periflow/schema/api/v1/completion.py
+-rw-r--r--   0        0        0      101 2023-07-20 12:32:34.266958 periflow_client-0.1.2/periflow/schema/resource/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-20 12:32:34.267053 periflow_client-0.1.2/periflow/schema/resource/v1/__init__.py
+-rw-r--r--   0        0        0     3912 2023-07-25 03:49:51.898529 periflow_client-0.1.2/periflow/schema/resource/v1/attributes.py
+-rw-r--r--   0        0        0     2353 2023-07-20 12:32:34.267192 periflow_client-0.1.2/periflow/schema/resource/v1/checkpoint.py
+-rw-r--r--   0        0        0     1358 2023-07-20 12:32:34.267258 periflow_client-0.1.2/periflow/schema/resource/v1/credential.py
+-rw-r--r--   0        0        0     2027 2023-07-20 12:32:34.267312 periflow_client-0.1.2/periflow/schema/resource/v1/deployment.py
+-rw-r--r--   0        0        0       88 2023-07-20 12:32:34.267397 periflow_client-0.1.2/periflow/sdk/__init__.py
+-rw-r--r--   0        0        0      102 2023-07-20 12:32:34.267511 periflow_client-0.1.2/periflow/sdk/api/__init__.py
+-rw-r--r--   0        0        0     5799 2023-07-20 12:32:34.267596 periflow_client-0.1.2/periflow/sdk/api/base.py
+-rw-r--r--   0        0        0    25709 2023-07-20 12:32:34.267670 periflow_client-0.1.2/periflow/sdk/api/completion.py
+-rw-r--r--   0        0        0     1836 2023-07-20 12:32:34.267758 periflow_client-0.1.2/periflow/sdk/init.py
+-rw-r--r--   0        0        0      112 2023-07-20 12:32:34.267862 periflow_client-0.1.2/periflow/sdk/resource/__init__.py
+-rw-r--r--   0        0        0      733 2023-07-20 12:32:34.267911 periflow_client-0.1.2/periflow/sdk/resource/base.py
+-rw-r--r--   0        0        0    31619 2023-07-26 09:29:06.024041 periflow_client-0.1.2/periflow/sdk/resource/checkpoint.py
+-rw-r--r--   0        0        0     4036 2023-07-20 12:32:34.268103 periflow_client-0.1.2/periflow/sdk/resource/credential.py
+-rw-r--r--   0        0        0    17719 2023-07-25 03:49:56.900175 periflow_client-0.1.2/periflow/sdk/resource/deployment.py
+-rw-r--r--   0        0        0       97 2023-07-20 12:32:34.268333 periflow_client-0.1.2/periflow/utils/__init__.py
+-rw-r--r--   0        0        0     4232 2023-07-20 12:32:34.268415 periflow_client-0.1.2/periflow/utils/format.py
+-rw-r--r--   0        0        0    14539 2023-07-20 12:32:34.268558 periflow_client-0.1.2/periflow/utils/fs.py
+-rw-r--r--   0        0        0     1303 2023-07-25 03:49:56.900640 periflow_client-0.1.2/periflow/utils/maps.py
+-rw-r--r--   0        0        0      666 2023-07-20 12:32:34.268678 periflow_client-0.1.2/periflow/utils/prompt.py
+-rw-r--r--   0        0        0     2265 2023-07-20 12:32:34.268742 periflow_client-0.1.2/periflow/utils/request.py
+-rw-r--r--   0        0        0     1384 2023-07-20 12:32:34.268808 periflow_client-0.1.2/periflow/utils/testing.py
+-rw-r--r--   0        0        0     1485 2023-07-20 12:32:34.268869 periflow_client-0.1.2/periflow/utils/url.py
+-rw-r--r--   0        0        0     3552 2023-07-20 12:32:34.268951 periflow_client-0.1.2/periflow/utils/validate.py
+-rw-r--r--   0        0        0     1513 2023-07-20 12:32:34.269017 periflow_client-0.1.2/periflow/utils/version.py
+-rw-r--r--   0        0        0     3417 2023-07-26 09:37:06.718173 periflow_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     9683 1970-01-01 00:00:00.000000 periflow_client-0.1.2/PKG-INFO
```

### Comparing `periflow_client-0.1.1/LICENSE` & `periflow_client-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/README.md` & `periflow_client-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/__init__.py` & `periflow_client-0.1.2/periflow/__init__.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/auth.py` & `periflow_client-0.1.2/periflow/auth.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/cli/checkpoint.py` & `periflow_client-0.1.2/periflow/cli/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/cli/credential.py` & `periflow_client-0.1.2/periflow/cli/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/cli/deployment.py` & `periflow_client-0.1.2/periflow/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/cli/group.py` & `periflow_client-0.1.2/periflow/cli/group.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 org_panel_formatter = PanelFormatter(
     name="Organization Detail",
     fields=["id", "name", "status"],
     headers=["ID", "Name", "Status"],
 )
 member_table_formatter = TableFormatter(
     name="Members",
-    fields=["id", "username", "name", "email", "privilege_level"],
-    headers=["ID", "Username", "Name", "Email", "Role"],
+    fields=["id", "name", "email", "privilege_level"],
+    headers=["ID", "Name", "Email", "Role"],
 )
 
 
 @app.command()
 def invite(email: str = typer.Argument(..., help="Invitation recipient email address")):
     """Invite a new member to the organization.
 
@@ -53,35 +53,17 @@
     if org["privilege_level"] != "owner":
         secho_error_and_exit("Only the owner of the organization can invite/set-role.")
 
     group_client.invite_to_group(org["id"], email)
     typer.echo("Invitation Successfully Sent!")
 
 
-@app.command("accept-invite")
-def accept_invite(
-    token: str = typer.Option(..., prompt="Enter email token"),
-    key: str = typer.Option(..., prompt="Enter verification key"),
-):
-    """Accept organization invitation.
-
-    When the invitee accepts the invitation, the invitee becomes a **Member** of the invited
-    organization.
-
-    """
-    group_client = GroupClient()
-    group_client.accept_invite(token, key)
-    typer.echo("Verification Success!")
-    typer.echo("Please login again with: ", nl=False)
-    typer.secho("pf login", fg=typer.colors.BLUE)
-
-
 @app.command("set-role")
 def set_role(
-    username: str = typer.Argument(..., help="Username to set role"),
+    email: str = typer.Argument(..., help="Email of the user to assign a role"),
     role: GroupRole = typer.Argument(..., help="Organization role"),
 ):
     """Set organization role of the user.
 
     The organization-level roles and privileges are as follows:
 
     |                          | Owner | Member |
@@ -99,26 +81,26 @@
     org = get_current_org()
 
     if org["privilege_level"] != "owner":
         secho_error_and_exit(
             "Only the owner of the organization can invite/set-privilege."
         )
 
-    user_id = _get_org_user_id_by_name(org["id"], username)
+    user_id = get_org_user_id_by_email(org["id"], email)
     user_client.set_group_privilege(org["id"], user_id, role)
     typer.echo(
-        f"Organization role for user ({username}) successfully updated to {role.value}!"
+        f"Organization role for user '{email}' successfully updated to {role.value}!"
     )
 
 
 @app.command("delete-user")
 def delete_user(
-    username: str = typer.Argument(
+    email: str = typer.Argument(
         ...,
-        help="Username to delete from the organization",
+        help="Email of the user to delete from the organization",
     ),
     force: bool = typer.Option(
         False,
         "--force",
         "-f",
         help="Forcefully delete without confirmation prompt",
     ),
@@ -135,34 +117,35 @@
 
     if org["privilege_level"] != "owner":
         secho_error_and_exit(
             "Only the owner of the organization can invite/set-privilege."
         )
 
     org_id = org["id"]
-    user_id = _get_org_user_id_by_name(org_id, username)
+    user_id = get_org_user_id_by_email(org_id, email)
 
     if not force:
         do_delete = typer.confirm(
-            f"Are you sure to remove user({username}) from the organization?"
+            f"Are you sure to remove user '{email}' from the organization?"
         )
         if not do_delete:
             raise typer.Abort()
     user_client.delete_from_org(user_id, org_id)
 
     typer.secho("User is successfully deleted from organization", fg=typer.colors.BLUE)
 
 
-def _get_org_user_id_by_name(org_id: UUID, username: str) -> UUID:
+def get_org_user_id_by_email(org_id: UUID, email: str) -> UUID:
+    """Get ID of user by the email."""
     group_client = GroupClient()
-    users = group_client.get_users(org_id, username)
+    users = group_client.list_users(org_id)
     for user in users:
-        if user["username"] == username:
+        if user["email"] == email:
             return UUID(user["id"])
-    secho_error_and_exit(f"{username} is not a member of this organization.")
+    secho_error_and_exit(f"User '{email}' is not a member of this organization.")
 
 
 def get_current_org() -> Dict[str, Any]:
     """Get the current organization info."""
     user_group_client = UserGroupClient()
 
     curr_org_id = get_current_group_id()
```

### Comparing `periflow_client-0.1.1/periflow/cli/key.py` & `periflow_client-0.1.2/periflow/cli/key.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/cli/main.py` & `periflow_client-0.1.2/periflow/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,36 +41,36 @@
 app.add_typer(project.app, name="project", help="Manage projects")
 app.add_typer(group.app, name="org", help="Manage organizations")
 app.add_typer(key.app, name="key", help="Manage api keys")
 
 
 user_panel_formatter = PanelFormatter(
     name="My Info",
-    fields=["name", "username", "email"],
-    headers=["Name", "Username", "Email"],
+    fields=["name", "email"],
+    headers=["Name", "Email"],
 )
 
 
 @app.command()
 def whoami():
     """Show my user info."""
     client = UserClient()
     info = client.get_current_userinfo()
     user_panel_formatter.render([info])
 
 
 @app.command()
 def login(
-    username: str = typer.Option(..., prompt="Enter Username"),
-    password: str = typer.Option(..., prompt="Enter Password", hide_input=True),
+    email: str = typer.Option(..., prompt="Enter your email"),
+    password: str = typer.Option(..., prompt="Enter your password", hide_input=True),
 ):
     """Sign in."""
     r = requests.post(
         get_training_uri("token/"),
-        data={"username": username, "password": password},
+        data={"username": email, "password": password},
         timeout=DEFAULT_REQ_TIMEOUT,
     )
     resp = r.json()
     if "code" in resp and resp["code"] == "mfa_required":
         mfa_token = resp["mfa_token"]
         client = UserMFAClient()
         # TODO: MFA type currently defaults to totp, need changes when new options are added
@@ -168,9 +168,9 @@
         typer.echo(r"|_|   \___|_|  |_||_|   |_|\___/ \_/\_/  ")  # type: ignore
         typer.echo("\n\n")
     except HTTPError:
         if mfa:
             secho_error_and_exit("Login failed... Invalid MFA Code.")
         else:
             secho_error_and_exit(
-                "Login failed... Please check your username and password."
+                "Login failed... Please check your email and password."
             )
```

### Comparing `periflow_client-0.1.1/periflow/cli/project.py` & `periflow_client-0.1.2/periflow/cli/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 from typing import Optional, Tuple
 from uuid import UUID
 
 import typer
 
-from periflow.cli.group import _get_org_user_id_by_name, get_current_org
+from periflow.cli.group import get_current_org, get_org_user_id_by_email
 from periflow.client.group import GroupProjectClient
 from periflow.client.project import ProjectClient, find_project_id
 from periflow.client.user import UserClient, UserGroupProjectClient
 from periflow.context import (
     get_current_project_id,
     project_context_path,
     set_current_project_id,
@@ -33,16 +33,16 @@
 project_panel_formatter = PanelFormatter(
     name="Project Detail",
     fields=["pf_group_id", "id", "name"],
     headers=["Organization ID", "Project ID", "Name"],
 )
 member_table_formatter = TableFormatter(
     name="Members",
-    fields=["id", "username", "name", "email", "access_level"],
-    headers=["ID", "Username", "Name", "Email", "Role"],
+    fields=["id", "name", "email", "access_level"],
+    headers=["ID", "Name", "Email", "Role"],
 )
 
 
 # pylint: disable=redefined-builtin
 @app.command()
 def list(
     tail: Optional[int] = typer.Option(
@@ -176,17 +176,17 @@
         secho_error_and_exit("Only the admin of the project can add-user/set-role")
 
     return org["id"], project_id
 
 
 @app.command("add-user")
 def add_user(
-    username: str = typer.Argument(
+    email: str = typer.Argument(
         ...,
-        help="Username to add to the current working project",
+        help="Email of the user to add to the current working project",
     ),
     role: ProjectRole = typer.Argument(
         ...,
         help="Project role to assign",
     ),
 ):
     """Add user to project.
@@ -199,25 +199,27 @@
     inside the organization.
     :::
 
     """
     user_client = UserClient()
 
     org_id, project_id = _check_project_and_get_id()
-    user_id = _get_org_user_id_by_name(org_id, username)
+    user_id = get_org_user_id_by_email(org_id, email)
 
     user_client.add_to_project(user_id, project_id, role)
-    typer.secho("User is successfully added to project", fg=typer.colors.BLUE)
+    typer.secho(
+        f"User '{email}' is successfully added to project", fg=typer.colors.BLUE
+    )
 
 
 @app.command("delete-user")
 def delete_user(
-    username: str = typer.Argument(
+    email: str = typer.Argument(
         ...,
-        help="Username to delete from the current working project",
+        help="Email of the user to delete from the current working project",
     ),
     force: bool = typer.Option(
         False,
         "--force",
         "-f",
         help="Forcefully delete without confirmation prompt",
     ),
@@ -228,32 +230,34 @@
     Only organization **Owner** or project **Admin** can evict members from the project.
     :::
 
     """
     user_client = UserClient()
 
     org_id, project_id = _check_project_and_get_id()
-    user_id = _get_org_user_id_by_name(org_id, username)
+    user_id = get_org_user_id_by_email(org_id, email)
 
     if not force:
         do_delete = typer.confirm(
-            f"Are you sure to remove user({username}) from the project?"
+            f"Are you sure to remove user '{email}' from the project?"
         )
         if not do_delete:
             raise typer.Abort()
 
     user_client.delete_from_project(user_id, project_id)
-    typer.secho("User is successfully deleted from project", fg=typer.colors.BLUE)
+    typer.secho(
+        f"User '{email}' is successfully deleted from project", fg=typer.colors.BLUE
+    )
 
 
 @app.command("set-role")
 def set_role(
-    username: str = typer.Argument(
+    email: str = typer.Argument(
         ...,
-        help="Username to set project role",
+        help="Email of the user to assign a project role",
     ),
     role: ProjectRole = typer.Argument(
         ...,
         help="Project role",
     ),
 ):
     """Set project role for the user.
@@ -281,19 +285,19 @@
     projects inside the organization.
     :::
 
     """
     user_client = UserClient()
 
     org_id, project_id = _check_project_and_get_id()
-    user_id = _get_org_user_id_by_name(org_id, username)
+    user_id = get_org_user_id_by_email(org_id, email)
 
     user_client.set_project_privilege(user_id, project_id, role)
     typer.secho(
-        f"Project role for user ({username}) successfully updated to {role.value}!"
+        f"Project role for user '{email}' successfully updated to {role.value}!"
     )
 
 
 @app.command()
 def members():
     """List project members."""
     project_client = ProjectClient()
```

### Comparing `periflow_client-0.1.1/periflow/cli/vm.py` & `periflow_client-0.1.2/periflow/cli/vm.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/client/base.py` & `periflow_client-0.1.2/periflow/client/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/client/checkpoint.py` & `periflow_client-0.1.2/periflow/client/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/client/credential.py` & `periflow_client-0.1.2/periflow/client/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/client/deployment.py` & `periflow_client-0.1.2/periflow/client/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/client/file.py` & `periflow_client-0.1.2/periflow/client/file.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/client/group.py` & `periflow_client-0.1.2/periflow/client/group.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,30 +45,19 @@
             self.retrieve, err_prefix="Failed to get an organization."
         )(pk=pf_group_id)
         return response.json()
 
     def invite_to_group(self, pf_group_id: uuid.UUID, email: str) -> None:
         """Invite a new member to the organization by sending an email."""
         safe_request(self.post, err_prefix="Failed to send invitation")(
-            path=f"{pf_group_id}/invite", json={"email": email, "msg": ""}
-        )
-
-    def accept_invite(self, token: str, key: str) -> None:
-        """Accept the invitation by entering the token."""
-        safe_request(self.post, err_prefix="Invalid code... Please Try again.")(
-            path="invite/confirm", json={"email_token": token, "key": key}
-        )
-
-    def get_users(self, pf_group_id: uuid.UUID, username: str) -> List[Dict[str, Any]]:
-        """Search organization member info by username."""
-        get_response_dict = safe_request(
-            self.list, err_prefix="Failed to get user in organization"
-        )
-        return paginated_get(
-            get_response_dict, path=f"{pf_group_id}/pf_user", search=username
+            path=f"{pf_group_id}/invite/signup",
+            json={
+                "email": email,
+                "callback_path": "/api/auth/invite/callback",
+            },
         )
 
     def list_users(self, pf_group_id: uuid.UUID) -> List[Dict[str, Any]]:
         """List all organization member info."""
         get_response_dict = safe_request(
             self.list, err_prefix="Failed to list users in organization"
         )
```

### Comparing `periflow_client-0.1.1/periflow/client/project.py` & `periflow_client-0.1.2/periflow/client/project.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/client/user.py` & `periflow_client-0.1.2/periflow/client/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,25 +38,14 @@
     """User sign-up client."""
 
     @property
     def url_path(self) -> Template:
         """Get an URL path."""
         return Template(get_auth_uri("pf_user/self_signup"))
 
-    def sign_up(self, username: str, name: str, email: str, password: str) -> None:
-        """Sign up."""
-        safe_request(self.bare_post, err_prefix="Failed to signup")(
-            json={
-                "username": username,
-                "name": name,
-                "email": email,
-                "password": password,
-            }
-        )
-
     def verify(self, token: str, key: str) -> None:
         """Verify the email account with the token to sign up."""
         safe_request(self.bare_post, err_prefix="Failed to verify")(
             path="confirm", json={"email_token": token, "key": key}
         )
```

### Comparing `periflow_client-0.1.1/periflow/cloud/storage.py` & `periflow_client-0.1.2/periflow/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/configurator/base.py` & `periflow_client-0.1.2/periflow/configurator/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/configurator/credential.py` & `periflow_client-0.1.2/periflow/configurator/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/configurator/deployment.py` & `periflow_client-0.1.2/periflow/configurator/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/context.py` & `periflow_client-0.1.2/periflow/context.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/converter/base.py` & `periflow_client-0.1.2/periflow/converter/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/converter/interface.py` & `periflow_client-0.1.2/periflow/converter/interface.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/converter/maps.py` & `periflow_client-0.1.2/periflow/converter/maps.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/converter/models/blenderbot.py` & `periflow_client-0.1.2/periflow/converter/models/blenderbot.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/converter/models/bloom.py` & `periflow_client-0.1.2/periflow/converter/models/bloom.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/converter/models/codegen.py` & `periflow_client-0.1.2/periflow/converter/models/codegen.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/converter/models/falcon.py` & `periflow_client-0.1.2/periflow/converter/models/falcon.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/converter/models/gpt2.py` & `periflow_client-0.1.2/periflow/converter/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/converter/models/gpt_neox.py` & `periflow_client-0.1.2/periflow/converter/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/converter/models/gptj.py` & `periflow_client-0.1.2/periflow/converter/models/gptj.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/converter/models/llama.py` & `periflow_client-0.1.2/periflow/converter/models/llama.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/converter/models/mpt.py` & `periflow_client-0.1.2/periflow/converter/models/mpt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/converter/models/opt.py` & `periflow_client-0.1.2/periflow/converter/models/opt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/converter/models/t5.py` & `periflow_client-0.1.2/periflow/converter/models/t5.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/converter/utils.py` & `periflow_client-0.1.2/periflow/converter/utils.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/enums.py` & `periflow_client-0.1.2/periflow/enums.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/errors.py` & `periflow_client-0.1.2/periflow/errors.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/formatter.py` & `periflow_client-0.1.2/periflow/formatter.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/logging.py` & `periflow_client-0.1.2/periflow/logging.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/schema/api/v1/completion.py` & `periflow_client-0.1.2/periflow/schema/api/v1/completion.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/schema/resource/v1/attributes.py` & `periflow_client-0.1.2/periflow/schema/resource/v1/attributes.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/schema/resource/v1/checkpoint.py` & `periflow_client-0.1.2/periflow/schema/resource/v1/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/schema/resource/v1/credential.py` & `periflow_client-0.1.2/periflow/schema/resource/v1/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/schema/resource/v1/deployment.py` & `periflow_client-0.1.2/periflow/schema/resource/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/sdk/api/base.py` & `periflow_client-0.1.2/periflow/sdk/api/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/sdk/api/completion.py` & `periflow_client-0.1.2/periflow/sdk/api/completion.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/sdk/init.py` & `periflow_client-0.1.2/periflow/sdk/init.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/sdk/resource/base.py` & `periflow_client-0.1.2/periflow/sdk/resource/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/sdk/resource/checkpoint.py` & `periflow_client-0.1.2/periflow/sdk/resource/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -901,14 +901,15 @@
                 model_name_or_path,
             )
             state_dict = hf_factory.from_pretrained(
                 model_name_or_path,
                 torch_dtype=torch.float32,
                 cache_dir=cache_dir,
                 trust_remote_code=True,
+                low_cpu_mem_usage=True,  # For model loading faster and using ~1x model size CPU memory. https://huggingface.co/docs/transformers/main_classes/model#transformers.PreTrainedModel.from_pretrained.example
             ).state_dict()
             logger.info(
                 "Hugging Face checkpoint(%s) is successfully loaded!",
                 model_name_or_path,
             )
             converter.convert(state_dict=state_dict)
             logger.info(
```

### Comparing `periflow_client-0.1.1/periflow/sdk/resource/credential.py` & `periflow_client-0.1.2/periflow/sdk/resource/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/sdk/resource/deployment.py` & `periflow_client-0.1.2/periflow/sdk/resource/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/utils/format.py` & `periflow_client-0.1.2/periflow/utils/format.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/utils/fs.py` & `periflow_client-0.1.2/periflow/utils/fs.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/utils/maps.py` & `periflow_client-0.1.2/periflow/utils/maps.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/utils/prompt.py` & `periflow_client-0.1.2/periflow/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/utils/request.py` & `periflow_client-0.1.2/periflow/utils/request.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/utils/testing.py` & `periflow_client-0.1.2/periflow/utils/testing.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/utils/url.py` & `periflow_client-0.1.2/periflow/utils/url.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/utils/validate.py` & `periflow_client-0.1.2/periflow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/periflow/utils/version.py` & `periflow_client-0.1.2/periflow/utils/version.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.1/pyproject.toml` & `periflow_client-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "periflow-client"
-version = "0.1.1"
+version = "0.1.2"
 description = "Client of PeriFlow, the fastest generative AI serving available."
 license = "Apache-2.0"
 authors = ["PeriFlow teams <eng@friendli.ai>"]
 packages = [
     { include = "periflow" },
 ]
 readme = "README.md"
@@ -44,14 +44,15 @@
 mypy-boto3-s3 = "1.26.163"
 ruamel-yaml = "0.17.32"
 pydantic = {extras = ["email"], version = "2.0.2"}
 aiohttp = {extras = ["speedups"], version = "3.8.4"}
 transformers = { version = "^4.31.0", optional = true }
 h5py = { version = "3.9.0", optional = true }
 einops = { version = "0.6.1", optional = true }
+accelerate = { version = "^0.21.0", optional = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 typer = "0.9.0"
 pytest = "7.4.0"
@@ -76,15 +77,15 @@
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 typer = "0.9.0"
 docstring-parser = "0.15"
 
 [tool.poetry.extras]
-mllib = ["transformers", "h5py"]
+mllib = ["transformers", "h5py", "accelerate", "einops"]
 
 [tool.isort]
 profile = "black"
 known_local_folder = ["tests"]
 append_only = true
 add_imports = ["from __future__ import annotations"]
```

### Comparing `periflow_client-0.1.1/PKG-INFO` & `periflow_client-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periflow-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Client of PeriFlow, the fastest generative AI serving available.
 Home-page: https://docs.periflow.ai/
 License: Apache-2.0
 Keywords: generative-ai,serving,llm
 Author: PeriFlow teams
 Author-email: eng@friendli.ai
 Requires-Python: >=3.8,<4.0
@@ -12,21 +12,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: mllib
 Requires-Dist: PyYaml (==6.0.1)
+Requires-Dist: accelerate (>=0.21.0,<0.22.0) ; extra == "mllib"
 Requires-Dist: aiohttp[speedups] (==3.8.4)
 Requires-Dist: azure-mgmt-storage (==20.1.0)
 Requires-Dist: azure-storage-blob (==12.12.0)
 Requires-Dist: boto3 (==1.22.8)
 Requires-Dist: boto3-stubs (==1.26.90)
 Requires-Dist: botocore (==1.25.8)
-Requires-Dist: einops (==0.6.1)
+Requires-Dist: einops (==0.6.1) ; extra == "mllib"
 Requires-Dist: filelock (==3.12.2)
 Requires-Dist: h5py (==3.9.0) ; extra == "mllib"
 Requires-Dist: jsonschema (==4.17.3)
 Requires-Dist: mypy-boto3-s3 (==1.26.163)
 Requires-Dist: packaging (==23.1)
 Requires-Dist: pathspec (==0.9.0)
 Requires-Dist: pydantic[email] (==2.0.2)
```

#### html2text {}

```diff
@@ -1,29 +1,30 @@
-Metadata-Version: 2.1 Name: periflow-client Version: 0.1.1 Summary: Client of
+Metadata-Version: 2.1 Name: periflow-client Version: 0.1.2 Summary: Client of
 PeriFlow, the fastest generative AI serving available. Home-page: https://
 docs.periflow.ai/ License: Apache-2.0 Keywords: generative-ai,serving,llm
 Author: PeriFlow teams Author-email: eng@friendli.ai Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: mllib Requires-Dist: PyYaml
-(==6.0.1) Requires-Dist: aiohttp[speedups] (==3.8.4) Requires-Dist: azure-mgmt-
-storage (==20.1.0) Requires-Dist: azure-storage-blob (==12.12.0) Requires-Dist:
-boto3 (==1.22.8) Requires-Dist: boto3-stubs (==1.26.90) Requires-Dist: botocore
-(==1.25.8) Requires-Dist: einops (==0.6.1) Requires-Dist: filelock (==3.12.2)
-Requires-Dist: h5py (==3.9.0) ; extra == "mllib" Requires-Dist: jsonschema
-(==4.17.3) Requires-Dist: mypy-boto3-s3 (==1.26.163) Requires-Dist: packaging
-(==23.1) Requires-Dist: pathspec (==0.9.0) Requires-Dist: pydantic[email]
-(==2.0.2) Requires-Dist: requests (==2.31.0) Requires-Dist: rich (==12.2.0)
-Requires-Dist: ruamel-yaml (==0.17.32) Requires-Dist: tqdm (==4.64.0) Requires-
-Dist: transformers (>=4.31.0,<5.0.0) ; extra == "mllib" Requires-Dist: typer
-(==0.9.0) Requires-Dist: websockets (==10.1) Project-URL: Documentation, https:
-//docs.periflow.ai/ Project-URL: Repository, https://github.com/friendliai/
-periflow-client Description-Content-Type: text/markdown
+(==6.0.1) Requires-Dist: accelerate (>=0.21.0,<0.22.0) ; extra == "mllib"
+Requires-Dist: aiohttp[speedups] (==3.8.4) Requires-Dist: azure-mgmt-storage
+(==20.1.0) Requires-Dist: azure-storage-blob (==12.12.0) Requires-Dist: boto3
+(==1.22.8) Requires-Dist: boto3-stubs (==1.26.90) Requires-Dist: botocore
+(==1.25.8) Requires-Dist: einops (==0.6.1) ; extra == "mllib" Requires-Dist:
+filelock (==3.12.2) Requires-Dist: h5py (==3.9.0) ; extra == "mllib" Requires-
+Dist: jsonschema (==4.17.3) Requires-Dist: mypy-boto3-s3 (==1.26.163) Requires-
+Dist: packaging (==23.1) Requires-Dist: pathspec (==0.9.0) Requires-Dist:
+pydantic[email] (==2.0.2) Requires-Dist: requests (==2.31.0) Requires-Dist:
+rich (==12.2.0) Requires-Dist: ruamel-yaml (==0.17.32) Requires-Dist: tqdm
+(==4.64.0) Requires-Dist: transformers (>=4.31.0,<5.0.0) ; extra == "mllib"
+Requires-Dist: typer (==0.9.0) Requires-Dist: websockets (==10.1) Project-URL:
+Documentation, https://docs.periflow.ai/ Project-URL: Repository, https://
+github.com/friendliai/periflow-client Description-Content-Type: text/markdown
                                    [system]
 ***** Supercharge Generative AI Serving ð *****
  [CI_Status] [Python_Version] [PyPi_Package_Version] [Documentation] [License]
 PeriFlow is the fastest engine for serving generative AI models such as GPT-3.
 With PeriFlow, a company can significantly reduce the cost and environmental
 impact of running its generative AI models. Users can use PeriFlow in a
 container and run it on the infrastructure they manage. They can also use our
```

