# Comparing `tmp/periflow_client-0.1.2.tar.gz` & `tmp/periflow_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periflow_client-0.1.2.tar", max compression
+gzip compressed data, was "periflow_client-0.1.3.tar", max compression
```

## Comparing `periflow_client-0.1.2.tar` & `periflow_client-0.1.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     3501 2023-07-25 04:03:34.042855 periflow_client-0.1.2/LICENSE
--rw-r--r--   0        0        0     7948 2023-07-20 12:32:34.224165 periflow_client-0.1.2/README.md
--rw-r--r--   0        0        0      820 2023-07-20 12:32:34.262789 periflow_client-0.1.2/periflow/__init__.py
--rw-r--r--   0        0        0     4410 2023-07-20 12:32:34.262864 periflow_client-0.1.2/periflow/auth.py
--rw-r--r--   0        0        0      188 2023-07-20 12:32:34.262945 periflow_client-0.1.2/periflow/cli/__init__.py
--rw-r--r--   0        0        0    19009 2023-07-25 03:49:51.897018 periflow_client-0.1.2/periflow/cli/checkpoint.py
--rw-r--r--   0        0        0    10321 2023-07-20 12:32:34.263102 periflow_client-0.1.2/periflow/cli/credential.py
--rw-r--r--   0        0        0    18875 2023-07-25 03:49:56.899224 periflow_client-0.1.2/periflow/cli/deployment.py
--rw-r--r--   0        0        0     5142 2023-07-26 09:29:06.022605 periflow_client-0.1.2/periflow/cli/group.py
--rw-r--r--   0        0        0     2445 2023-07-20 12:32:34.263329 periflow_client-0.1.2/periflow/cli/key.py
--rw-r--r--   0        0        0     6051 2023-07-26 09:29:06.022825 periflow_client-0.1.2/periflow/cli/main.py
--rw-r--r--   0        0        0     9526 2023-07-26 09:29:06.023043 periflow_client-0.1.2/periflow/cli/project.py
--rw-r--r--   0        0        0     1676 2023-07-25 03:49:56.899466 periflow_client-0.1.2/periflow/cli/vm.py
--rw-r--r--   0        0        0      125 2023-07-20 12:32:34.263645 periflow_client-0.1.2/periflow/client/__init__.py
--rw-r--r--   0        0        0    15578 2023-07-20 12:32:34.263735 periflow_client-0.1.2/periflow/client/base.py
--rw-r--r--   0        0        0     2651 2023-07-20 12:32:34.263798 periflow_client-0.1.2/periflow/client/checkpoint.py
--rw-r--r--   0        0        0     2603 2023-07-20 12:32:34.263898 periflow_client-0.1.2/periflow/client/credential.py
--rw-r--r--   0        0        0     7402 2023-07-20 12:32:34.263972 periflow_client-0.1.2/periflow/client/deployment.py
--rw-r--r--   0        0        0     3069 2023-07-20 12:32:34.264036 periflow_client-0.1.2/periflow/client/file.py
--rw-r--r--   0        0        0     5332 2023-07-26 09:29:06.023358 periflow_client-0.1.2/periflow/client/group.py
--rw-r--r--   0        0        0     3581 2023-07-20 12:32:34.264158 periflow_client-0.1.2/periflow/client/project.py
--rw-r--r--   0        0        0     7003 2023-07-26 09:29:06.023578 periflow_client-0.1.2/periflow/client/user.py
--rw-r--r--   0        0        0       98 2023-07-20 12:32:34.264311 periflow_client-0.1.2/periflow/cloud/__init__.py
--rw-r--r--   0        0        0     9622 2023-07-20 12:32:34.264393 periflow_client-0.1.2/periflow/cloud/storage.py
--rw-r--r--   0        0        0      107 2023-07-20 12:32:34.264482 periflow_client-0.1.2/periflow/configurator/__init__.py
--rw-r--r--   0        0        0     1587 2023-07-20 12:32:34.264550 periflow_client-0.1.2/periflow/configurator/base.py
--rw-r--r--   0        0        0     4067 2023-07-20 12:32:34.264648 periflow_client-0.1.2/periflow/configurator/credential.py
--rw-r--r--   0        0        0     3112 2023-07-20 12:32:34.264715 periflow_client-0.1.2/periflow/configurator/deployment.py
--rw-r--r--   0        0        0     1753 2023-07-20 12:32:34.264778 periflow_client-0.1.2/periflow/context.py
--rw-r--r--   0        0        0      105 2023-07-20 12:32:34.264853 periflow_client-0.1.2/periflow/converter/__init__.py
--rw-r--r--   0        0        0    15051 2023-07-20 12:58:47.707975 periflow_client-0.1.2/periflow/converter/base.py
--rw-r--r--   0        0        0     5020 2023-07-20 12:32:34.265037 periflow_client-0.1.2/periflow/converter/interface.py
--rw-r--r--   0        0        0     2397 2023-07-20 12:32:34.265101 periflow_client-0.1.2/periflow/converter/maps.py
--rw-r--r--   0        0        0    13345 2023-07-20 12:32:34.265241 periflow_client-0.1.2/periflow/converter/models/blenderbot.py
--rw-r--r--   0        0        0     8689 2023-07-20 12:32:34.265314 periflow_client-0.1.2/periflow/converter/models/bloom.py
--rw-r--r--   0        0        0     7252 2023-07-20 12:32:34.265389 periflow_client-0.1.2/periflow/converter/models/codegen.py
--rw-r--r--   0        0        0     9706 2023-07-20 12:32:34.265458 periflow_client-0.1.2/periflow/converter/models/falcon.py
--rw-r--r--   0        0        0     7060 2023-07-20 12:32:34.265533 periflow_client-0.1.2/periflow/converter/models/gpt2.py
--rw-r--r--   0        0        0    10454 2023-07-20 12:32:34.265601 periflow_client-0.1.2/periflow/converter/models/gpt_neox.py
--rw-r--r--   0        0        0     7122 2023-07-20 12:32:34.265672 periflow_client-0.1.2/periflow/converter/models/gptj.py
--rw-r--r--   0        0        0     7916 2023-07-25 03:49:51.897974 periflow_client-0.1.2/periflow/converter/models/llama.py
--rw-r--r--   0        0        0     7316 2023-07-20 12:32:34.265844 periflow_client-0.1.2/periflow/converter/models/mpt.py
--rw-r--r--   0        0        0     9390 2023-07-20 12:32:34.265915 periflow_client-0.1.2/periflow/converter/models/opt.py
--rw-r--r--   0        0        0    12615 2023-07-20 12:32:34.265998 periflow_client-0.1.2/periflow/converter/models/t5.py
--rw-r--r--   0        0        0     4456 2023-07-20 12:32:34.266070 periflow_client-0.1.2/periflow/converter/utils.py
--rw-r--r--   0        0        0     3318 2023-07-25 03:49:56.899802 periflow_client-0.1.2/periflow/enums.py
--rw-r--r--   0        0        0     5404 2023-07-20 12:32:34.266214 periflow_client-0.1.2/periflow/errors.py
--rw-r--r--   0        0        0     9505 2023-07-20 12:32:34.266322 periflow_client-0.1.2/periflow/formatter.py
--rw-r--r--   0        0        0      660 2023-07-20 12:32:34.266385 periflow_client-0.1.2/periflow/logging.py
--rw-r--r--   0        0        0       92 2023-07-20 12:32:34.266497 periflow_client-0.1.2/periflow/schema/__init__.py
--rw-r--r--   0        0        0       96 2023-07-20 12:32:34.266643 periflow_client-0.1.2/periflow/schema/api/__init__.py
--rw-r--r--   0        0        0       99 2023-07-20 12:32:34.266768 periflow_client-0.1.2/periflow/schema/api/v1/__init__.py
--rw-r--r--   0        0        0     2828 2023-07-20 12:32:34.266844 periflow_client-0.1.2/periflow/schema/api/v1/completion.py
--rw-r--r--   0        0        0      101 2023-07-20 12:32:34.266958 periflow_client-0.1.2/periflow/schema/resource/__init__.py
--rw-r--r--   0        0        0      104 2023-07-20 12:32:34.267053 periflow_client-0.1.2/periflow/schema/resource/v1/__init__.py
--rw-r--r--   0        0        0     3912 2023-07-25 03:49:51.898529 periflow_client-0.1.2/periflow/schema/resource/v1/attributes.py
--rw-r--r--   0        0        0     2353 2023-07-20 12:32:34.267192 periflow_client-0.1.2/periflow/schema/resource/v1/checkpoint.py
--rw-r--r--   0        0        0     1358 2023-07-20 12:32:34.267258 periflow_client-0.1.2/periflow/schema/resource/v1/credential.py
--rw-r--r--   0        0        0     2027 2023-07-20 12:32:34.267312 periflow_client-0.1.2/periflow/schema/resource/v1/deployment.py
--rw-r--r--   0        0        0       88 2023-07-20 12:32:34.267397 periflow_client-0.1.2/periflow/sdk/__init__.py
--rw-r--r--   0        0        0      102 2023-07-20 12:32:34.267511 periflow_client-0.1.2/periflow/sdk/api/__init__.py
--rw-r--r--   0        0        0     5799 2023-07-20 12:32:34.267596 periflow_client-0.1.2/periflow/sdk/api/base.py
--rw-r--r--   0        0        0    25709 2023-07-20 12:32:34.267670 periflow_client-0.1.2/periflow/sdk/api/completion.py
--rw-r--r--   0        0        0     1836 2023-07-20 12:32:34.267758 periflow_client-0.1.2/periflow/sdk/init.py
--rw-r--r--   0        0        0      112 2023-07-20 12:32:34.267862 periflow_client-0.1.2/periflow/sdk/resource/__init__.py
--rw-r--r--   0        0        0      733 2023-07-20 12:32:34.267911 periflow_client-0.1.2/periflow/sdk/resource/base.py
--rw-r--r--   0        0        0    31619 2023-07-26 09:29:06.024041 periflow_client-0.1.2/periflow/sdk/resource/checkpoint.py
--rw-r--r--   0        0        0     4036 2023-07-20 12:32:34.268103 periflow_client-0.1.2/periflow/sdk/resource/credential.py
--rw-r--r--   0        0        0    17719 2023-07-25 03:49:56.900175 periflow_client-0.1.2/periflow/sdk/resource/deployment.py
--rw-r--r--   0        0        0       97 2023-07-20 12:32:34.268333 periflow_client-0.1.2/periflow/utils/__init__.py
--rw-r--r--   0        0        0     4232 2023-07-20 12:32:34.268415 periflow_client-0.1.2/periflow/utils/format.py
--rw-r--r--   0        0        0    14539 2023-07-20 12:32:34.268558 periflow_client-0.1.2/periflow/utils/fs.py
--rw-r--r--   0        0        0     1303 2023-07-25 03:49:56.900640 periflow_client-0.1.2/periflow/utils/maps.py
--rw-r--r--   0        0        0      666 2023-07-20 12:32:34.268678 periflow_client-0.1.2/periflow/utils/prompt.py
--rw-r--r--   0        0        0     2265 2023-07-20 12:32:34.268742 periflow_client-0.1.2/periflow/utils/request.py
--rw-r--r--   0        0        0     1384 2023-07-20 12:32:34.268808 periflow_client-0.1.2/periflow/utils/testing.py
--rw-r--r--   0        0        0     1485 2023-07-20 12:32:34.268869 periflow_client-0.1.2/periflow/utils/url.py
--rw-r--r--   0        0        0     3552 2023-07-20 12:32:34.268951 periflow_client-0.1.2/periflow/utils/validate.py
--rw-r--r--   0        0        0     1513 2023-07-20 12:32:34.269017 periflow_client-0.1.2/periflow/utils/version.py
--rw-r--r--   0        0        0     3417 2023-07-26 09:37:06.718173 periflow_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     9683 1970-01-01 00:00:00.000000 periflow_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3501 2023-07-25 04:03:34.042855 periflow_client-0.1.3/LICENSE
+-rw-r--r--   0        0        0     7965 2023-07-26 11:08:22.666762 periflow_client-0.1.3/README.md
+-rw-r--r--   0        0        0      820 2023-07-20 12:32:34.262789 periflow_client-0.1.3/periflow/__init__.py
+-rw-r--r--   0        0        0     4410 2023-07-20 12:32:34.262864 periflow_client-0.1.3/periflow/auth.py
+-rw-r--r--   0        0        0      188 2023-07-20 12:32:34.262945 periflow_client-0.1.3/periflow/cli/__init__.py
+-rw-r--r--   0        0        0    19009 2023-07-25 03:49:51.897018 periflow_client-0.1.3/periflow/cli/checkpoint.py
+-rw-r--r--   0        0        0    10321 2023-07-20 12:32:34.263102 periflow_client-0.1.3/periflow/cli/credential.py
+-rw-r--r--   0        0        0    18875 2023-07-26 11:08:22.668089 periflow_client-0.1.3/periflow/cli/deployment.py
+-rw-r--r--   0        0        0     5142 2023-07-26 09:29:06.022605 periflow_client-0.1.3/periflow/cli/group.py
+-rw-r--r--   0        0        0     2445 2023-07-20 12:32:34.263329 periflow_client-0.1.3/periflow/cli/key.py
+-rw-r--r--   0        0        0     6051 2023-07-26 09:29:06.022825 periflow_client-0.1.3/periflow/cli/main.py
+-rw-r--r--   0        0        0     9526 2023-07-26 09:29:06.023043 periflow_client-0.1.3/periflow/cli/project.py
+-rw-r--r--   0        0        0     1676 2023-07-25 03:49:56.899466 periflow_client-0.1.3/periflow/cli/vm.py
+-rw-r--r--   0        0        0      125 2023-07-20 12:32:34.263645 periflow_client-0.1.3/periflow/client/__init__.py
+-rw-r--r--   0        0        0    15578 2023-07-20 12:32:34.263735 periflow_client-0.1.3/periflow/client/base.py
+-rw-r--r--   0        0        0     2651 2023-07-20 12:32:34.263798 periflow_client-0.1.3/periflow/client/checkpoint.py
+-rw-r--r--   0        0        0     2603 2023-07-20 12:32:34.263898 periflow_client-0.1.3/periflow/client/credential.py
+-rw-r--r--   0        0        0     7402 2023-07-20 12:32:34.263972 periflow_client-0.1.3/periflow/client/deployment.py
+-rw-r--r--   0        0        0     3069 2023-07-20 12:32:34.264036 periflow_client-0.1.3/periflow/client/file.py
+-rw-r--r--   0        0        0     5332 2023-07-26 09:29:06.023358 periflow_client-0.1.3/periflow/client/group.py
+-rw-r--r--   0        0        0     3581 2023-07-20 12:32:34.264158 periflow_client-0.1.3/periflow/client/project.py
+-rw-r--r--   0        0        0     7003 2023-07-26 09:29:06.023578 periflow_client-0.1.3/periflow/client/user.py
+-rw-r--r--   0        0        0       98 2023-07-20 12:32:34.264311 periflow_client-0.1.3/periflow/cloud/__init__.py
+-rw-r--r--   0        0        0     9622 2023-07-20 12:32:34.264393 periflow_client-0.1.3/periflow/cloud/storage.py
+-rw-r--r--   0        0        0      107 2023-07-20 12:32:34.264482 periflow_client-0.1.3/periflow/configurator/__init__.py
+-rw-r--r--   0        0        0     1587 2023-07-20 12:32:34.264550 periflow_client-0.1.3/periflow/configurator/base.py
+-rw-r--r--   0        0        0     4067 2023-07-20 12:32:34.264648 periflow_client-0.1.3/periflow/configurator/credential.py
+-rw-r--r--   0        0        0     3112 2023-07-20 12:32:34.264715 periflow_client-0.1.3/periflow/configurator/deployment.py
+-rw-r--r--   0        0        0     1753 2023-07-20 12:32:34.264778 periflow_client-0.1.3/periflow/context.py
+-rw-r--r--   0        0        0      105 2023-07-20 12:32:34.264853 periflow_client-0.1.3/periflow/converter/__init__.py
+-rw-r--r--   0        0        0    15051 2023-07-20 12:58:47.707975 periflow_client-0.1.3/periflow/converter/base.py
+-rw-r--r--   0        0        0     5020 2023-07-20 12:32:34.265037 periflow_client-0.1.3/periflow/converter/interface.py
+-rw-r--r--   0        0        0     2397 2023-07-20 12:32:34.265101 periflow_client-0.1.3/periflow/converter/maps.py
+-rw-r--r--   0        0        0    13345 2023-07-20 12:32:34.265241 periflow_client-0.1.3/periflow/converter/models/blenderbot.py
+-rw-r--r--   0        0        0     8689 2023-07-20 12:32:34.265314 periflow_client-0.1.3/periflow/converter/models/bloom.py
+-rw-r--r--   0        0        0     7252 2023-07-20 12:32:34.265389 periflow_client-0.1.3/periflow/converter/models/codegen.py
+-rw-r--r--   0        0        0     9706 2023-07-20 12:32:34.265458 periflow_client-0.1.3/periflow/converter/models/falcon.py
+-rw-r--r--   0        0        0     7060 2023-07-20 12:32:34.265533 periflow_client-0.1.3/periflow/converter/models/gpt2.py
+-rw-r--r--   0        0        0    10454 2023-07-20 12:32:34.265601 periflow_client-0.1.3/periflow/converter/models/gpt_neox.py
+-rw-r--r--   0        0        0     7122 2023-07-20 12:32:34.265672 periflow_client-0.1.3/periflow/converter/models/gptj.py
+-rw-r--r--   0        0        0     7916 2023-07-25 03:49:51.897974 periflow_client-0.1.3/periflow/converter/models/llama.py
+-rw-r--r--   0        0        0     7316 2023-07-20 12:32:34.265844 periflow_client-0.1.3/periflow/converter/models/mpt.py
+-rw-r--r--   0        0        0     9390 2023-07-20 12:32:34.265915 periflow_client-0.1.3/periflow/converter/models/opt.py
+-rw-r--r--   0        0        0    12615 2023-07-20 12:32:34.265998 periflow_client-0.1.3/periflow/converter/models/t5.py
+-rw-r--r--   0        0        0     4456 2023-07-20 12:32:34.266070 periflow_client-0.1.3/periflow/converter/utils.py
+-rw-r--r--   0        0        0     3318 2023-07-25 03:49:56.899802 periflow_client-0.1.3/periflow/enums.py
+-rw-r--r--   0        0        0     5404 2023-07-20 12:32:34.266214 periflow_client-0.1.3/periflow/errors.py
+-rw-r--r--   0        0        0     9505 2023-07-20 12:32:34.266322 periflow_client-0.1.3/periflow/formatter.py
+-rw-r--r--   0        0        0      660 2023-07-20 12:32:34.266385 periflow_client-0.1.3/periflow/logging.py
+-rw-r--r--   0        0        0       92 2023-07-20 12:32:34.266497 periflow_client-0.1.3/periflow/schema/__init__.py
+-rw-r--r--   0        0        0       96 2023-07-20 12:32:34.266643 periflow_client-0.1.3/periflow/schema/api/__init__.py
+-rw-r--r--   0        0        0       99 2023-07-20 12:32:34.266768 periflow_client-0.1.3/periflow/schema/api/v1/__init__.py
+-rw-r--r--   0        0        0     2828 2023-07-20 12:32:34.266844 periflow_client-0.1.3/periflow/schema/api/v1/completion.py
+-rw-r--r--   0        0        0      101 2023-07-20 12:32:34.266958 periflow_client-0.1.3/periflow/schema/resource/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-20 12:32:34.267053 periflow_client-0.1.3/periflow/schema/resource/v1/__init__.py
+-rw-r--r--   0        0        0     3912 2023-07-25 03:49:51.898529 periflow_client-0.1.3/periflow/schema/resource/v1/attributes.py
+-rw-r--r--   0        0        0     2353 2023-07-20 12:32:34.267192 periflow_client-0.1.3/periflow/schema/resource/v1/checkpoint.py
+-rw-r--r--   0        0        0     1358 2023-07-20 12:32:34.267258 periflow_client-0.1.3/periflow/schema/resource/v1/credential.py
+-rw-r--r--   0        0        0     2027 2023-07-20 12:32:34.267312 periflow_client-0.1.3/periflow/schema/resource/v1/deployment.py
+-rw-r--r--   0        0        0       88 2023-07-20 12:32:34.267397 periflow_client-0.1.3/periflow/sdk/__init__.py
+-rw-r--r--   0        0        0      102 2023-07-20 12:32:34.267511 periflow_client-0.1.3/periflow/sdk/api/__init__.py
+-rw-r--r--   0        0        0     5757 2023-07-26 11:08:22.668388 periflow_client-0.1.3/periflow/sdk/api/base.py
+-rw-r--r--   0        0        0    25710 2023-07-26 11:08:22.668715 periflow_client-0.1.3/periflow/sdk/api/completion.py
+-rw-r--r--   0        0        0     1836 2023-07-20 12:32:34.267758 periflow_client-0.1.3/periflow/sdk/init.py
+-rw-r--r--   0        0        0      112 2023-07-20 12:32:34.267862 periflow_client-0.1.3/periflow/sdk/resource/__init__.py
+-rw-r--r--   0        0        0      733 2023-07-20 12:32:34.267911 periflow_client-0.1.3/periflow/sdk/resource/base.py
+-rw-r--r--   0        0        0    31619 2023-07-26 09:29:06.024041 periflow_client-0.1.3/periflow/sdk/resource/checkpoint.py
+-rw-r--r--   0        0        0     4036 2023-07-20 12:32:34.268103 periflow_client-0.1.3/periflow/sdk/resource/credential.py
+-rw-r--r--   0        0        0    17721 2023-07-26 11:08:22.669040 periflow_client-0.1.3/periflow/sdk/resource/deployment.py
+-rw-r--r--   0        0        0       97 2023-07-20 12:32:34.268333 periflow_client-0.1.3/periflow/utils/__init__.py
+-rw-r--r--   0        0        0     4232 2023-07-20 12:32:34.268415 periflow_client-0.1.3/periflow/utils/format.py
+-rw-r--r--   0        0        0    14539 2023-07-20 12:32:34.268558 periflow_client-0.1.3/periflow/utils/fs.py
+-rw-r--r--   0        0        0     1303 2023-07-25 03:49:56.900640 periflow_client-0.1.3/periflow/utils/maps.py
+-rw-r--r--   0        0        0      666 2023-07-20 12:32:34.268678 periflow_client-0.1.3/periflow/utils/prompt.py
+-rw-r--r--   0        0        0     2265 2023-07-20 12:32:34.268742 periflow_client-0.1.3/periflow/utils/request.py
+-rw-r--r--   0        0        0     1384 2023-07-20 12:32:34.268808 periflow_client-0.1.3/periflow/utils/testing.py
+-rw-r--r--   0        0        0     1485 2023-07-20 12:32:34.268869 periflow_client-0.1.3/periflow/utils/url.py
+-rw-r--r--   0        0        0     3552 2023-07-20 12:32:34.268951 periflow_client-0.1.3/periflow/utils/validate.py
+-rw-r--r--   0        0        0     1513 2023-07-20 12:32:34.269017 periflow_client-0.1.3/periflow/utils/version.py
+-rw-r--r--   0        0        0     3417 2023-07-26 11:08:22.669323 periflow_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9700 1970-01-01 00:00:00.000000 periflow_client-0.1.3/PKG-INFO
```

### Comparing `periflow_client-0.1.2/LICENSE` & `periflow_client-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/README.md` & `periflow_client-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,17 @@
     project_name="my-project",
 )
 
 # Create a deployment at GCP asia-northest3 region wtih one A100 GPU.
 deployment = pf.Deployment.create(
     checkpoint_id="YOUR_CHECKPOINT_ID",
     name="my-deployment",
-    gpu_type="a100",
     cloud="gcp",
     region="asia-northeast3",
+    vm_type="a2-highgpu-1g",
     ...
 )
 ```
 
 When the deployment becomes the "Healthy" status and ready to process inference requests, you can generate a completion with:
 
 ```python
@@ -123,25 +123,25 @@
 # Switch CLI context to target project
 pf project switch my-project
 
 # Create a deployment
 pf deployment create \
   --checkpoint-id $YOUR_CHECKPOINT_ID \
   --name my-deployment \
-  --gpu-type a100 \
   --cloud gcp \
   --region asia-northeast3 \
+  --vm-type a2-highgpu-1g \
   --config-file config.yaml
 ```
 
 When the deployment is ready, you can send a request with `curl`.
 
 ```sh
 # Send a inference request to the deployment.
-curl -X POST https://gcp-asia-northeast3.periflow.ai/$DEPLOYMENT_ID/v1/completion \
+curl -X POST https://gcp-asia-northeast3.periflow.ai/$DEPLOYMENT_ID/v1/completions \
   -d '{"prompt": "Python is a popular language for", "max_tokens": 100, "top_p": 0.8, "temperature": 0.5, "no_repeat_ngram": 3}'
 ```
 
 The response will be like:
 
 ```txt
 {
```

#### html2text {}

```diff
@@ -53,35 +53,36 @@
 [PeriFlow Client Docs](https://docs.periflow.ai/) to learn more. ##
 Installation ```sh pip install periflow-client ``` ## Examples This example
 shows how to create a deployment and send a completion API request to the
 created deployment with Python SDK. ```python import periflow as pf # Set up
 PeriFlow context. pf.init( api_key="YOUR_PERIFLOW_API_KEY", project_name="my-
 project", ) # Create a deployment at GCP asia-northest3 region wtih one A100
 GPU. deployment = pf.Deployment.create( checkpoint_id="YOUR_CHECKPOINT_ID",
-name="my-deployment", gpu_type="a100", cloud="gcp", region="asia-northeast3",
-... ) ``` When the deployment becomes the "Healthy" status and ready to process
-inference requests, you can generate a completion with: ```python # Generate a
-completion by sending an inference request to the deployment created above. api
-= pf.Completion(deployment_id=deployment.deployment_id) completion = api.create
+name="my-deployment", cloud="gcp", region="asia-northeast3", vm_type="a2-
+highgpu-1g", ... ) ``` When the deployment becomes the "Healthy" status and
+ready to process inference requests, you can generate a completion with:
+```python # Generate a completion by sending an inference request to the
+deployment created above. api = pf.Completion
+(deployment_id=deployment.deployment_id) completion = api.create
 ( options=pf.V1CompletionOptions( prompt="Python is a popular language for",
 max_tokens=100, top_p=0.8, temperature=0.5, no_repeat_ngram=3, ) ) print
 (completion.choices[0].text) """ >>> Example Output: web development. It is
 also used for a variety of other applications. Python can be used to create
 desktop applications, web applications and mobile applications as well. Python
 is one of the most popular languages for data science. Data scientists use
 Python to analyze data. The Python ecosystem is very diverse. There are many
 libraries that can help you with your Python projects. You can also find many
 Python tutorials online. """ ``` You can also do the same with CLI. ```sh #
 Switch CLI context to target project pf project switch my-project # Create a
 deployment pf deployment create \ --checkpoint-id $YOUR_CHECKPOINT_ID \ --name
-my-deployment \ --gpu-type a100 \ --cloud gcp \ --region asia-northeast3 \ --
-config-file config.yaml ``` When the deployment is ready, you can send a
+my-deployment \ --cloud gcp \ --region asia-northeast3 \ --vm-type a2-highgpu-
+1g \ --config-file config.yaml ``` When the deployment is ready, you can send a
 request with `curl`. ```sh # Send a inference request to the deployment. curl -
-X POST https://gcp-asia-northeast3.periflow.ai/$DEPLOYMENT_ID/v1/completion \ -
-d '{"prompt": "Python is a popular language for", "max_tokens": 100, "top_p":
+X POST https://gcp-asia-northeast3.periflow.ai/$DEPLOYMENT_ID/v1/completions \
+-d '{"prompt": "Python is a popular language for", "max_tokens": 100, "top_p":
 0.8, "temperature": 0.5, "no_repeat_ngram": 3}' ``` The response will be like:
 ```txt { "choices": [ { "index": 0, "seed": 18337142367832222086, "text": " web
 development. It is also used for a variety of other applications.\nPython can
 be used to create desktop applications, web applications and mobile
 applications as well.\nPython is one of the most popular languages for data
 science.\nData scientists use Python to analyze data.\nThe Python ecosystem is
 very diverse.\nThere are many libraries that can help you with your Python
```

### Comparing `periflow_client-0.1.2/periflow/__init__.py` & `periflow_client-0.1.3/periflow/__init__.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/auth.py` & `periflow_client-0.1.3/periflow/auth.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/cli/checkpoint.py` & `periflow_client-0.1.3/periflow/cli/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/cli/credential.py` & `periflow_client-0.1.3/periflow/cli/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/cli/deployment.py` & `periflow_client-0.1.3/periflow/cli/deployment.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -412,19 +412,19 @@
 def create(
     checkpoint_id: UUID = typer.Option(
         ..., "--checkpoint-id", "-i", help="Checkpoint id to deploy."
     ),
     deployment_name: str = typer.Option(
         ..., "--name", "-n", help="The name of deployment. "
     ),
+    cloud: CloudType = typer.Option(..., "--cloud", "-c", help="Type of cloud."),
+    region: str = typer.Option(..., "--region", "-r", help="Region of cloud."),
     vm_type: VMType = typer.Option(
         ..., "--vm-type", "-v", help="The VM type for the deployment."
     ),
-    cloud: CloudType = typer.Option(..., "--cloud", "-c", help="Type of cloud."),
-    region: str = typer.Option(..., "--region", "-r", help="Region of cloud."),
     config_file: Optional[typer.FileText] = typer.Option(
         None, "--config-file", "-f", help="Path to configuration file."
     ),
     deployment_type: DeploymentType = typer.Option(
         DeploymentType.PROD, "--type", "-t", help="Type of deployment."
     ),
     description: Optional[str] = typer.Option(
```

### Comparing `periflow_client-0.1.2/periflow/cli/group.py` & `periflow_client-0.1.3/periflow/cli/group.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/cli/key.py` & `periflow_client-0.1.3/periflow/cli/key.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/cli/main.py` & `periflow_client-0.1.3/periflow/cli/main.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/cli/project.py` & `periflow_client-0.1.3/periflow/cli/project.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/cli/vm.py` & `periflow_client-0.1.3/periflow/cli/vm.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/client/base.py` & `periflow_client-0.1.3/periflow/client/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/client/checkpoint.py` & `periflow_client-0.1.3/periflow/client/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/client/credential.py` & `periflow_client-0.1.3/periflow/client/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/client/deployment.py` & `periflow_client-0.1.3/periflow/client/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/client/file.py` & `periflow_client-0.1.3/periflow/client/file.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/client/group.py` & `periflow_client-0.1.3/periflow/client/group.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/client/project.py` & `periflow_client-0.1.3/periflow/client/project.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/client/user.py` & `periflow_client-0.1.3/periflow/client/user.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/cloud/storage.py` & `periflow_client-0.1.3/periflow/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/configurator/base.py` & `periflow_client-0.1.3/periflow/configurator/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/configurator/credential.py` & `periflow_client-0.1.3/periflow/configurator/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/configurator/deployment.py` & `periflow_client-0.1.3/periflow/configurator/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/context.py` & `periflow_client-0.1.3/periflow/context.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/converter/base.py` & `periflow_client-0.1.3/periflow/converter/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/converter/interface.py` & `periflow_client-0.1.3/periflow/converter/interface.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/converter/maps.py` & `periflow_client-0.1.3/periflow/converter/maps.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/converter/models/blenderbot.py` & `periflow_client-0.1.3/periflow/converter/models/blenderbot.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/converter/models/bloom.py` & `periflow_client-0.1.3/periflow/converter/models/bloom.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/converter/models/codegen.py` & `periflow_client-0.1.3/periflow/converter/models/codegen.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/converter/models/falcon.py` & `periflow_client-0.1.3/periflow/converter/models/falcon.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/converter/models/gpt2.py` & `periflow_client-0.1.3/periflow/converter/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/converter/models/gpt_neox.py` & `periflow_client-0.1.3/periflow/converter/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/converter/models/gptj.py` & `periflow_client-0.1.3/periflow/converter/models/gptj.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/converter/models/llama.py` & `periflow_client-0.1.3/periflow/converter/models/llama.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/converter/models/mpt.py` & `periflow_client-0.1.3/periflow/converter/models/mpt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/converter/models/opt.py` & `periflow_client-0.1.3/periflow/converter/models/opt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/converter/models/t5.py` & `periflow_client-0.1.3/periflow/converter/models/t5.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/converter/utils.py` & `periflow_client-0.1.3/periflow/converter/utils.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/enums.py` & `periflow_client-0.1.3/periflow/enums.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/errors.py` & `periflow_client-0.1.3/periflow/errors.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/formatter.py` & `periflow_client-0.1.3/periflow/formatter.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/logging.py` & `periflow_client-0.1.3/periflow/logging.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/schema/api/v1/completion.py` & `periflow_client-0.1.3/periflow/schema/api/v1/completion.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/schema/resource/v1/attributes.py` & `periflow_client-0.1.3/periflow/schema/resource/v1/attributes.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/schema/resource/v1/checkpoint.py` & `periflow_client-0.1.3/periflow/schema/resource/v1/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/schema/resource/v1/credential.py` & `periflow_client-0.1.3/periflow/schema/resource/v1/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/schema/resource/v1/deployment.py` & `periflow_client-0.1.3/periflow/schema/resource/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/sdk/api/base.py` & `periflow_client-0.1.3/periflow/sdk/api/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,17 +105,15 @@
             deployment = client.get_deployment(deployment_id)
             endpoint = deployment["endpoint"]
             if not endpoint:
                 raise NotFoundError("Active endpoint for the deployment is not found.")
             self._endpoint = urljoin(
                 get_baseurl(endpoint), os.path.join(deployment_id, self._api_path)
             )
-            self._auth_required = (
-                deployment["type"] == DeploymentSecurityLevel.PROTECTED
-            )
+            self._auth_required = deployment["config"]["infrequest_perm_check"]
         elif endpoint is not None:
             if deployment_security_level is None:
                 raise InvalidConfigError(
                     "'deployment_security_level' should be provided."
                 )
             self._endpoint = endpoint
             self._auth_required = (
```

### Comparing `periflow_client-0.1.2/periflow/sdk/api/completion.py` & `periflow_client-0.1.3/periflow/sdk/api/completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         V1CompletionOptions,
     ]
 ):
     """PeriFlow Completion API."""
 
     @property
     def _api_path(self) -> str:
-        return "v1/completion"
+        return "v1/completions"
 
     @overload
     def create(
         self, options: V1CompletionOptions, *, stream: Literal[True]
     ) -> V1CompletionStream:
         """[skip-doc]."""
```

### Comparing `periflow_client-0.1.2/periflow/sdk/init.py` & `periflow_client-0.1.3/periflow/sdk/init.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/sdk/resource/base.py` & `periflow_client-0.1.3/periflow/sdk/resource/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/sdk/resource/checkpoint.py` & `periflow_client-0.1.3/periflow/sdk/resource/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/sdk/resource/credential.py` & `periflow_client-0.1.3/periflow/sdk/resource/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/sdk/resource/deployment.py` & `periflow_client-0.1.3/periflow/sdk/resource/deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,17 +109,17 @@
             config = {
                 "max_batch_size": 256,
                 "max_token_count": 8146,
             }
             deployment = pf.Deployment.create(
                 checkpoint_id=UUID(190c117a-30ef-4c33-aad7-16f21bca0d63),
                 name="my-deployment",
-                gpu_type=GpuType.A100,
                 cloud=CloudType.GCP,
                 region="asia-northeast3",
+                vm_type="a2-highgpu-1g",
                 config=config,
             )
             ```
 
             The format of `config` should be:
 
             ```python
```

### Comparing `periflow_client-0.1.2/periflow/utils/format.py` & `periflow_client-0.1.3/periflow/utils/format.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/utils/fs.py` & `periflow_client-0.1.3/periflow/utils/fs.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/utils/maps.py` & `periflow_client-0.1.3/periflow/utils/maps.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/utils/prompt.py` & `periflow_client-0.1.3/periflow/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/utils/request.py` & `periflow_client-0.1.3/periflow/utils/request.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/utils/testing.py` & `periflow_client-0.1.3/periflow/utils/testing.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/utils/url.py` & `periflow_client-0.1.3/periflow/utils/url.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/utils/validate.py` & `periflow_client-0.1.3/periflow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/periflow/utils/version.py` & `periflow_client-0.1.3/periflow/utils/version.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.1.2/pyproject.toml` & `periflow_client-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "periflow-client"
-version = "0.1.2"
+version = "0.1.3"
 description = "Client of PeriFlow, the fastest generative AI serving available."
 license = "Apache-2.0"
 authors = ["PeriFlow teams <eng@friendli.ai>"]
 packages = [
     { include = "periflow" },
 ]
 readme = "README.md"
```

### Comparing `periflow_client-0.1.2/PKG-INFO` & `periflow_client-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periflow-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Client of PeriFlow, the fastest generative AI serving available.
 Home-page: https://docs.periflow.ai/
 License: Apache-2.0
 Keywords: generative-ai,serving,llm
 Author: PeriFlow teams
 Author-email: eng@friendli.ai
 Requires-Python: >=3.8,<4.0
@@ -121,17 +121,17 @@
     project_name="my-project",
 )
 
 # Create a deployment at GCP asia-northest3 region wtih one A100 GPU.
 deployment = pf.Deployment.create(
     checkpoint_id="YOUR_CHECKPOINT_ID",
     name="my-deployment",
-    gpu_type="a100",
     cloud="gcp",
     region="asia-northeast3",
+    vm_type="a2-highgpu-1g",
     ...
 )
 ```
 
 When the deployment becomes the "Healthy" status and ready to process inference requests, you can generate a completion with:
 
 ```python
@@ -167,25 +167,25 @@
 # Switch CLI context to target project
 pf project switch my-project
 
 # Create a deployment
 pf deployment create \
   --checkpoint-id $YOUR_CHECKPOINT_ID \
   --name my-deployment \
-  --gpu-type a100 \
   --cloud gcp \
   --region asia-northeast3 \
+  --vm-type a2-highgpu-1g \
   --config-file config.yaml
 ```
 
 When the deployment is ready, you can send a request with `curl`.
 
 ```sh
 # Send a inference request to the deployment.
-curl -X POST https://gcp-asia-northeast3.periflow.ai/$DEPLOYMENT_ID/v1/completion \
+curl -X POST https://gcp-asia-northeast3.periflow.ai/$DEPLOYMENT_ID/v1/completions \
   -d '{"prompt": "Python is a popular language for", "max_tokens": 100, "top_p": 0.8, "temperature": 0.5, "no_repeat_ngram": 3}'
 ```
 
 The response will be like:
 
 ```txt
 {
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: periflow-client Version: 0.1.2 Summary: Client of
+Metadata-Version: 2.1 Name: periflow-client Version: 0.1.3 Summary: Client of
 PeriFlow, the fastest generative AI serving available. Home-page: https://
 docs.periflow.ai/ License: Apache-2.0 Keywords: generative-ai,serving,llm
 Author: PeriFlow teams Author-email: eng@friendli.ai Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
@@ -76,35 +76,36 @@
 [PeriFlow Client Docs](https://docs.periflow.ai/) to learn more. ##
 Installation ```sh pip install periflow-client ``` ## Examples This example
 shows how to create a deployment and send a completion API request to the
 created deployment with Python SDK. ```python import periflow as pf # Set up
 PeriFlow context. pf.init( api_key="YOUR_PERIFLOW_API_KEY", project_name="my-
 project", ) # Create a deployment at GCP asia-northest3 region wtih one A100
 GPU. deployment = pf.Deployment.create( checkpoint_id="YOUR_CHECKPOINT_ID",
-name="my-deployment", gpu_type="a100", cloud="gcp", region="asia-northeast3",
-... ) ``` When the deployment becomes the "Healthy" status and ready to process
-inference requests, you can generate a completion with: ```python # Generate a
-completion by sending an inference request to the deployment created above. api
-= pf.Completion(deployment_id=deployment.deployment_id) completion = api.create
+name="my-deployment", cloud="gcp", region="asia-northeast3", vm_type="a2-
+highgpu-1g", ... ) ``` When the deployment becomes the "Healthy" status and
+ready to process inference requests, you can generate a completion with:
+```python # Generate a completion by sending an inference request to the
+deployment created above. api = pf.Completion
+(deployment_id=deployment.deployment_id) completion = api.create
 ( options=pf.V1CompletionOptions( prompt="Python is a popular language for",
 max_tokens=100, top_p=0.8, temperature=0.5, no_repeat_ngram=3, ) ) print
 (completion.choices[0].text) """ >>> Example Output: web development. It is
 also used for a variety of other applications. Python can be used to create
 desktop applications, web applications and mobile applications as well. Python
 is one of the most popular languages for data science. Data scientists use
 Python to analyze data. The Python ecosystem is very diverse. There are many
 libraries that can help you with your Python projects. You can also find many
 Python tutorials online. """ ``` You can also do the same with CLI. ```sh #
 Switch CLI context to target project pf project switch my-project # Create a
 deployment pf deployment create \ --checkpoint-id $YOUR_CHECKPOINT_ID \ --name
-my-deployment \ --gpu-type a100 \ --cloud gcp \ --region asia-northeast3 \ --
-config-file config.yaml ``` When the deployment is ready, you can send a
+my-deployment \ --cloud gcp \ --region asia-northeast3 \ --vm-type a2-highgpu-
+1g \ --config-file config.yaml ``` When the deployment is ready, you can send a
 request with `curl`. ```sh # Send a inference request to the deployment. curl -
-X POST https://gcp-asia-northeast3.periflow.ai/$DEPLOYMENT_ID/v1/completion \ -
-d '{"prompt": "Python is a popular language for", "max_tokens": 100, "top_p":
+X POST https://gcp-asia-northeast3.periflow.ai/$DEPLOYMENT_ID/v1/completions \
+-d '{"prompt": "Python is a popular language for", "max_tokens": 100, "top_p":
 0.8, "temperature": 0.5, "no_repeat_ngram": 3}' ``` The response will be like:
 ```txt { "choices": [ { "index": 0, "seed": 18337142367832222086, "text": " web
 development. It is also used for a variety of other applications.\nPython can
 be used to create desktop applications, web applications and mobile
 applications as well.\nPython is one of the most popular languages for data
 science.\nData scientists use Python to analyze data.\nThe Python ecosystem is
 very diverse.\nThere are many libraries that can help you with your Python
```

