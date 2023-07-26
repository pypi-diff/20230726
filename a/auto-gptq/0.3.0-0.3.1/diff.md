# Comparing `tmp/auto_gptq-0.3.0.tar.gz` & `tmp/auto_gptq-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_gptq-0.3.0.tar", last modified: Sun Jul 16 08:03:38 2023, max compression
+gzip compressed data, was "auto_gptq-0.3.1.tar", last modified: Wed Jul 26 10:22:07 2023, max compression
```

## Comparing `auto_gptq-0.3.0.tar` & `auto_gptq-0.3.1.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.628584 auto_gptq-0.3.0/
--rw-rw-rw-   0        0        0     1096 2023-04-13 14:32:51.000000 auto_gptq-0.3.0/LICENSE
--rw-rw-rw-   0        0        0    16857 2023-07-16 08:03:38.628584 auto_gptq-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    15955 2023-07-16 06:23:10.000000 auto_gptq-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.566062 auto_gptq-0.3.0/auto_gptq/
--rw-rw-rw-   0        0        0      136 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.581685 auto_gptq-0.3.0/auto_gptq/eval_tasks/
--rw-rw-rw-   0        0        0      124 2023-04-28 14:56:43.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/__init__.py
--rw-rw-rw-   0        0        0     2259 2023-04-28 14:56:43.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/_base.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.581685 auto_gptq-0.3.0/auto_gptq/eval_tasks/_utils/
--rw-rw-rw-   0        0        0        0 2023-04-23 15:46:04.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/_utils/__init__.py
--rw-rw-rw-   0        0        0     1165 2023-04-23 15:46:04.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/_utils/classification_utils.py
--rw-rw-rw-   0        0        0     1486 2023-04-23 15:46:04.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/_utils/generation_utils.py
--rw-rw-rw-   0        0        0     1262 2023-04-23 15:46:04.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/language_modeling_task.py
--rw-rw-rw-   0        0        0     3760 2023-04-23 15:46:04.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/sequence_classification_task.py
--rw-rw-rw-   0        0        0     2646 2023-04-24 12:51:09.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/text_summarization_task.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.581685 auto_gptq-0.3.0/auto_gptq/modeling/
--rw-rw-rw-   0        0        0      354 2023-07-16 06:23:10.000000 auto_gptq-0.3.0/auto_gptq/modeling/__init__.py
--rw-rw-rw-   0        0        0    39011 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/modeling/_base.py
--rw-rw-rw-   0        0        0      562 2023-07-16 06:23:10.000000 auto_gptq-0.3.0/auto_gptq/modeling/_const.py
--rw-rw-rw-   0        0        0     7387 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/modeling/_utils.py
--rw-rw-rw-   0        0        0     4314 2023-07-16 06:23:10.000000 auto_gptq-0.3.0/auto_gptq/modeling/auto.py
--rw-rw-rw-   0        0        0      430 2023-06-19 02:37:40.000000 auto_gptq-0.3.0/auto_gptq/modeling/baichuan.py
--rw-rw-rw-   0        0        0      490 2023-04-28 14:56:43.000000 auto_gptq-0.3.0/auto_gptq/modeling/bloom.py
--rw-rw-rw-   0        0        0      404 2023-05-28 08:23:38.000000 auto_gptq-0.3.0/auto_gptq/modeling/codegen.py
--rw-rw-rw-   0        0        0      409 2023-04-28 14:56:43.000000 auto_gptq-0.3.0/auto_gptq/modeling/gpt2.py
--rw-rw-rw-   0        0        0      469 2023-05-28 08:23:38.000000 auto_gptq-0.3.0/auto_gptq/modeling/gpt_bigcode.py
--rw-rw-rw-   0        0        0      478 2023-04-28 14:56:43.000000 auto_gptq-0.3.0/auto_gptq/modeling/gpt_neox.py
--rw-rw-rw-   0        0        0      569 2023-05-14 08:23:32.000000 auto_gptq-0.3.0/auto_gptq/modeling/gptj.py
--rw-rw-rw-   0        0        0      479 2023-07-16 06:23:10.000000 auto_gptq-0.3.0/auto_gptq/modeling/internlm.py
--rw-rw-rw-   0        0        0     1042 2023-05-20 07:21:20.000000 auto_gptq-0.3.0/auto_gptq/modeling/llama.py
--rw-rw-rw-   0        0        0      395 2023-04-29 02:36:14.000000 auto_gptq-0.3.0/auto_gptq/modeling/moss.py
--rw-rw-rw-   0        0        0      581 2023-04-28 15:06:27.000000 auto_gptq-0.3.0/auto_gptq/modeling/opt.py
--rw-rw-rw-   0        0        0      443 2023-05-28 08:23:38.000000 auto_gptq-0.3.0/auto_gptq/modeling/rw.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.597309 auto_gptq-0.3.0/auto_gptq/nn_modules/
--rw-rw-rw-   0        0        0        0 2023-04-26 13:22:55.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/__init__.py
--rw-rw-rw-   0        0        0      981 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/_fused_base.py
--rw-rw-rw-   0        0        0    11334 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/fused_gptj_attn.py
--rw-rw-rw-   0        0        0     7678 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/fused_llama_attn.py
--rw-rw-rw-   0        0        0    12200 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/fused_llama_mlp.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.597309 auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/
--rw-rw-rw-   0        0        0     2111 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/__init__.py
--rw-rw-rw-   0        0        0    11372 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/qlinear_cuda.py
--rw-rw-rw-   0        0        0    11762 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/qlinear_cuda_old.py
--rw-rw-rw-   0        0        0     6533 2023-06-19 02:37:40.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/qlinear_triton.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.597309 auto_gptq-0.3.0/auto_gptq/nn_modules/triton_utils/
--rw-rw-rw-   0        0        0        0 2023-05-20 09:01:53.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/triton_utils/__init__.py
--rw-rw-rw-   0        0        0     7099 2023-04-26 13:22:55.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/triton_utils/custom_autotune.py
--rw-rw-rw-   0        0        0    14285 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/triton_utils/kernels.py
--rw-rw-rw-   0        0        0      117 2023-05-20 09:01:53.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/triton_utils/mixin.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.597309 auto_gptq-0.3.0/auto_gptq/quantization/
--rw-rw-rw-   0        0        0       47 2023-04-26 13:22:55.000000 auto_gptq-0.3.0/auto_gptq/quantization/__init__.py
--rw-rw-rw-   0        0        0     6016 2023-05-14 05:13:14.000000 auto_gptq-0.3.0/auto_gptq/quantization/gptq.py
--rw-rw-rw-   0        0        0     4408 2023-04-26 13:22:55.000000 auto_gptq-0.3.0/auto_gptq/quantization/quantizer.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.597309 auto_gptq-0.3.0/auto_gptq/utils/
--rw-rw-rw-   0        0        0        0 2023-04-28 14:56:43.000000 auto_gptq-0.3.0/auto_gptq/utils/__init__.py
--rw-rw-rw-   0        0        0    11389 2023-04-28 14:56:43.000000 auto_gptq-0.3.0/auto_gptq/utils/data_utils.py
--rw-rw-rw-   0        0        0     1241 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/utils/import_utils.py
--rw-rw-rw-   0        0        0    18688 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/utils/peft_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.566062 auto_gptq-0.3.0/auto_gptq.egg-info/
--rw-rw-rw-   0        0        0    16857 2023-07-16 08:03:38.000000 auto_gptq-0.3.0/auto_gptq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1987 2023-07-16 08:03:38.000000 auto_gptq-0.3.0/auto_gptq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 08:03:38.000000 auto_gptq-0.3.0/auto_gptq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-07-16 08:03:38.000000 auto_gptq-0.3.0/auto_gptq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       45 2023-07-16 08:03:38.000000 auto_gptq-0.3.0/auto_gptq.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.628584 auto_gptq-0.3.0/autogptq_cuda/
--rw-rw-rw-   0        0        0     7212 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/autogptq_cuda/autogptq_cuda_256.cpp
--rw-rw-rw-   0        0        0     7212 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/autogptq_cuda/autogptq_cuda_64.cpp
--rw-rw-rw-   0        0        0    46659 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/autogptq_cuda/autogptq_cuda_kernel_256.cu
--rw-rw-rw-   0        0        0    46655 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/autogptq_cuda/autogptq_cuda_kernel_64.cu
--rw-rw-rw-   0        0        0       42 2023-07-16 08:03:38.628584 auto_gptq-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     3856 2023-07-16 08:02:59.000000 auto_gptq-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.710516 auto_gptq-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    16691 2023-07-26 10:22:07.710516 auto_gptq-0.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15813 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.690516 auto_gptq-0.3.1/auto_gptq/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.693516 auto_gptq-0.3.1/auto_gptq/eval_tasks/
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.693516 auto_gptq-0.3.1/auto_gptq/eval_tasks/_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/_utils/classification_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/_utils/generation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/language_modeling_task.py
+-rw-r--r--   0 root         (0) root         (0)     3653 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/sequence_classification_task.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/text_summarization_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.698516 auto_gptq-0.3.1/auto_gptq/modeling/
+-rw-r--r--   0 root         (0) root         (0)      340 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/modeling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41463 2023-07-26 10:21:12.000000 auto_gptq-0.3.1/auto_gptq/modeling/_base.py
+-rw-r--r--   0 root         (0) root         (0)      535 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/modeling/_const.py
+-rw-r--r--   0 root         (0) root         (0)     7181 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/modeling/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-07-26 10:21:12.000000 auto_gptq-0.3.1/auto_gptq/modeling/auto.py
+-rw-r--r--   0 root         (0) root         (0)      414 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/modeling/baichuan.py
+-rw-r--r--   0 root         (0) root         (0)      474 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/bloom.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/codegen.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/gpt2.py
+-rw-r--r--   0 root         (0) root         (0)      453 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/gpt_bigcode.py
+-rw-r--r--   0 root         (0) root         (0)      461 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/gpt_neox.py
+-rw-r--r--   0 root         (0) root         (0)      550 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/gptj.py
+-rw-r--r--   0 root         (0) root         (0)      463 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/modeling/internlm.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/llama.py
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/moss.py
+-rw-r--r--   0 root         (0) root         (0)      562 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/opt.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/rw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.700516 auto_gptq-0.3.1/auto_gptq/nn_modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/_fused_base.py
+-rw-r--r--   0 root         (0) root         (0)    11043 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/fused_gptj_attn.py
+-rw-r--r--   0 root         (0) root         (0)     7489 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/fused_llama_attn.py
+-rw-r--r--   0 root         (0) root         (0)    11870 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/fused_llama_mlp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.702516 auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11136 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/qlinear_cuda.py
+-rw-r--r--   0 root         (0) root         (0)    11551 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/qlinear_cuda_old.py
+-rw-r--r--   0 root         (0) root         (0)     6352 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/qlinear_triton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.703516 auto_gptq-0.3.1/auto_gptq/nn_modules/triton_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/triton_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6925 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/triton_utils/custom_autotune.py
+-rw-r--r--   0 root         (0) root         (0)    13883 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/triton_utils/kernels.py
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/triton_utils/mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.704516 auto_gptq-0.3.1/auto_gptq/quantization/
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/quantization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5835 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/quantization/gptq.py
+-rw-r--r--   0 root         (0) root         (0)     4271 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/quantization/quantizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.706516 auto_gptq-0.3.1/auto_gptq/utils/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11122 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/utils/data_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/utils/import_utils.py
+-rw-r--r--   0 root         (0) root         (0)    18265 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/utils/peft_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7098 2023-07-26 10:21:12.000000 auto_gptq-0.3.1/auto_gptq/utils/perplexity_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.691516 auto_gptq-0.3.1/auto_gptq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16691 2023-07-26 10:22:07.000000 auto_gptq-0.3.1/auto_gptq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2023 2023-07-26 10:22:07.000000 auto_gptq-0.3.1/auto_gptq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 10:22:07.000000 auto_gptq-0.3.1/auto_gptq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-26 10:22:07.000000 auto_gptq-0.3.1/auto_gptq.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-26 10:22:07.000000 auto_gptq-0.3.1/auto_gptq.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.708516 auto_gptq-0.3.1/autogptq_cuda/
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_256.cpp
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_64.cpp
+-rw-r--r--   0 root         (0) root         (0)    40941 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_kernel_256.cu
+-rw-r--r--   0 root         (0) root         (0)    40938 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_kernel_64.cu
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 10:22:07.710516 auto_gptq-0.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3695 2023-07-26 10:21:39.000000 auto_gptq-0.3.1/setup.py
```

### Comparing `auto_gptq-0.3.0/LICENSE` & `auto_gptq-0.3.1/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 潘其威(William)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 潘其威(William)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `auto_gptq-0.3.0/PKG-INFO` & `auto_gptq-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,345 +1,346 @@
-Metadata-Version: 2.1
-Name: auto_gptq
-Version: 0.3.0
-Summary: An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
-Home-page: https://github.com/PanQiWei/AutoGPTQ
-Author: PanQiWei
-Keywords: gptq,quantization,large-language-models,pytorch,transformers
-Platform: windows
-Platform: linux
-Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
-Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: C++
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Provides-Extra: triton
-License-File: LICENSE
-
-<h1 align="center">AutoGPTQ</h1>
-<p align="center">An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.</p>
-<p align="center">
-    <a href="https://github.com/PanQiWei/AutoGPTQ/releases">
-        <img alt="GitHub release" src="https://img.shields.io/github/release/PanQiWei/AutoGPTQ.svg">
-    </a>
-    <a href="https://pypi.org/project/auto-gptq/">
-        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/auto-gptq">
-    </a>
-</p>
-<h4 align="center">
-    <p>
-        <b>English</b> |
-        <a href="https://github.com/PanQiWei/AutoGPTQ/blob/main/README_zh.md">中文</a>
-    </p>
-</h4>
-
-*<center>📣 Long time no see! 👋 Architecture upgrade, performance optimization and more new features will come in July and August, stay tune! 🥂</center>*
-
-## News or Update
-
-- 2023-06-05 - (Update) - Integrate with 🤗 peft to use gptq quantized model to train adapters, support LoRA, AdaLoRA, AdaptionPrompt, etc.
-- 2023-05-30 - (Update) - Support download/upload quantized model from/to 🤗 Hub.
-- 2023-05-27 - (Update) - Support quantization and inference for `gpt_bigcode`, `codegen` and `RefineWeb/RefineWebModel`(falcon) model types.
-- 2023-05-04 - (Update) - Support using faster cuda kernel when `not desc_act or group_size == -1`.
-
-*For more histories please turn to [here](docs/NEWS_OR_UPDATE.md)*
-
-## Performance Comparison
-
-### Inference Speed
-> The result is generated using [this script](examples/benchmark/generation_speed.py), batch size of input is 1, decode strategy is beam search and enforce the model to generate 512 tokens, speed metric is tokens/s (the larger, the better).
-> 
-> The quantized model is loaded using the setup that can gain the fastest inference speed.
-
-| model         | GPU           | num_beams | fp16  | gptq-int4 |
-|---------------|---------------|-----------|-------|-----------|
-| llama-7b      | 1xA100-40G    | 1         | 18.87 | 25.53     |
-| llama-7b      | 1xA100-40G    | 4         | 68.79 | 91.30     |
-| moss-moon 16b | 1xA100-40G    | 1         | 12.48 | 15.25     |
-| moss-moon 16b | 1xA100-40G    | 4         | OOM   | 42.67     |
-| moss-moon 16b | 2xA100-40G    | 1         | 06.83 | 06.78     |
-| moss-moon 16b | 2xA100-40G    | 4         | 13.10 | 10.80     |
-| gpt-j 6b      | 1xRTX3060-12G | 1         | OOM   | 29.55     |
-| gpt-j 6b      | 1xRTX3060-12G | 4         | OOM   | 47.36     |
-
-
-### Perplexity
-For perplexity comparison, you can turn to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes)
-
-## Installation
-
-### Quick Installation
-You can install the latest stable release of AutoGPTQ from pip:
-```shell
-pip install auto-gptq
-```
-Start from v0.2.0, you can download pre-build wheel that satisfied your environment setup from each version's release assets and install it to skip building stage for the fastest installation speed. For example:
-```shell
-# firstly, cd the directory where the wheel saved, then execute command below
-pip install auto_gptq-0.2.0+cu118-cp310-cp310-linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for linux in an environment whose python=3.10 and cuda=11.8
-```
-#### disable cuda extensions
-By default, cuda extensions will be installed when `torch` and `cuda` is already installed in your machine, if you don't want to use them, using:
-```shell
-BUILD_CUDA_EXT=0 pip install auto-gptq
-```
-And to make sure `autogptq_cuda` is not ever in your virtual environment, run:
-```shell
-pip uninstall autogptq_cuda -y
-```
-
-#### to support triton speedup
-To integrate with `triton`, using:
-> warning: currently triton only supports linux; 3-bit quantization is not supported when using triton
-
-```shell
-pip install auto-gptq[triton]
-```
-
-### Install from source
-<details>
-<summary>click to see details</summary>
-
-Clone the source code:
-```shell
-git clone https://github.com/PanQiWei/AutoGPTQ.git && cd AutoGPTQ
-```
-Then, install from source:
-```shell
-pip install .
-```
-Like quick installation, you can also set `BUILD_CUDA_EXT=0` to disable pytorch extension building.
-
-Use `.[triton]` if you want to integrate with triton and it's available on your operating system.
-
-</details>
-
-## Quick Tour
-
-### Quantization and Inference
-> warning: this is just a showcase of the usage of basic apis in AutoGPTQ, which uses only one sample to quantize a much small model, quality of quantized model using such little samples may not good.
-
-Below is an example for the simplest use of `auto_gptq` to quantize a model and inference after quantization: 
-```python
-from transformers import AutoTokenizer, TextGenerationPipeline
-from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
-import logging
-
-logging.basicConfig(
-    format="%(asctime)s %(levelname)s [%(name)s] %(message)s", level=logging.INFO, datefmt="%Y-%m-%d %H:%M:%S"
-)
-
-pretrained_model_dir = "facebook/opt-125m"
-quantized_model_dir = "opt-125m-4bit"
-
-tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir, use_fast=True)
-examples = [
-    tokenizer(
-        "auto-gptq is an easy-to-use model quantization library with user-friendly apis, based on GPTQ algorithm."
-    )
-]
-
-quantize_config = BaseQuantizeConfig(
-    bits=4,  # quantize model to 4-bit
-    group_size=128,  # it is recommended to set the value to 128
-    desc_act=False,  # set to False can significantly speed up inference but the perplexity may slightly bad 
-)
-
-# load un-quantized model, by default, the model will always be loaded into CPU memory
-model = AutoGPTQForCausalLM.from_pretrained(pretrained_model_dir, quantize_config)
-
-# quantize model, the examples should be list of dict whose keys can only be "input_ids" and "attention_mask"
-model.quantize(examples)
-
-# save quantized model
-model.save_quantized(quantized_model_dir)
-
-# save quantized model using safetensors
-model.save_quantized(quantized_model_dir, use_safetensors=True)
-
-# push quantized model to Hugging Face Hub. 
-# to use use_auth_token=True, Login first via huggingface-cli login.
-# or pass explcit token with: use_auth_token="hf_xxxxxxx"
-# (uncomment the following three lines to enable this feature)
-# repo_id = f"YourUserName/{quantized_model_dir}"
-# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
-# model.push_to_hub(repo_id, commit_message=commit_message, use_auth_token=True)
-
-# alternatively you can save and push at the same time
-# (uncomment the following three lines to enable this feature)
-# repo_id = f"YourUserName/{quantized_model_dir}"
-# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
-# model.push_to_hub(repo_id, save_dir=quantized_model_dir, use_safetensors=True, commit_message=commit_message, use_auth_token=True)
-
-# load quantized model to the first GPU
-model = AutoGPTQForCausalLM.from_quantized(quantized_model_dir, device="cuda:0")
-
-# download quantized model from Hugging Face Hub and load to the first GPU
-# model = AutoGPTQForCausalLM.from_quantized(repo_id, device="cuda:0", use_safetensors=True, use_triton=False)
-
-# inference with model.generate
-print(tokenizer.decode(model.generate(**tokenizer("auto_gptq is", return_tensors="pt").to(model.device))[0]))
-
-# or you can also use pipeline
-pipeline = TextGenerationPipeline(model=model, tokenizer=tokenizer)
-print(pipeline("auto-gptq is")[0]["generated_text"])
-```
-
-For more advanced features of model quantization, please reference to [this script](examples/quantization/quant_with_alpaca.py)
-
-### Customize Model
-<details>
-
-<summary>Below is an example to extend `auto_gptq` to support `OPT` model, as you will see, it's very easy:</summary>
-
-```python
-from auto_gptq.modeling import BaseGPTQForCausalLM
-
-
-class OPTGPTQForCausalLM(BaseGPTQForCausalLM):
-    # chained attribute name of transformer layer block
-    layers_block_name = "model.decoder.layers"
-    # chained attribute names of other nn modules that in the same level as the transformer layer block
-    outside_layer_modules = [
-        "model.decoder.embed_tokens", "model.decoder.embed_positions", "model.decoder.project_out",
-        "model.decoder.project_in", "model.decoder.final_layer_norm"
-    ]
-    # chained attribute names of linear layers in transformer layer module
-    # normally, there are four sub lists, for each one the modules in it can be seen as one operation, 
-    # and the order should be the order when they are truly executed, in this case (and usually in most cases), 
-    # they are: attention q_k_v projection, attention output projection, MLP project input, MLP project output
-    inside_layer_modules = [
-        ["self_attn.k_proj", "self_attn.v_proj", "self_attn.q_proj"],
-        ["self_attn.out_proj"],
-        ["fc1"],
-        ["fc2"]
-    ]
-```
-After this, you can use `OPTGPTQForCausalLM.from_pretrained` and other methods as shown in Basic.
-
-</details>
-
-### Evaluation on Downstream Tasks
-You can use tasks defined in `auto_gptq.eval_tasks` to evaluate model's performance on specific down-stream task before and after quantization.
-
-The predefined tasks support all causal-language-models implemented in [🤗 transformers](https://github.com/huggingface/transformers) and in this project.
-
-<details>
-
-<summary>Below is an example to evaluate `EleutherAI/gpt-j-6b` on sequence-classification task using `cardiffnlp/tweet_sentiment_multilingual` dataset:</summary>
-
-```python
-from functools import partial
-
-import datasets
-from transformers import AutoTokenizer, AutoModelForCausalLM, GenerationConfig
-
-from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
-from auto_gptq.eval_tasks import SequenceClassificationTask
-
-
-MODEL = "EleutherAI/gpt-j-6b"
-DATASET = "cardiffnlp/tweet_sentiment_multilingual"
-TEMPLATE = "Question:What's the sentiment of the given text? Choices are {labels}.\nText: {text}\nAnswer:"
-ID2LABEL = {
-    0: "negative",
-    1: "neutral",
-    2: "positive"
-}
-LABELS = list(ID2LABEL.values())
-
-
-def ds_refactor_fn(samples):
-    text_data = samples["text"]
-    label_data = samples["label"]
-
-    new_samples = {"prompt": [], "label": []}
-    for text, label in zip(text_data, label_data):
-        prompt = TEMPLATE.format(labels=LABELS, text=text)
-        new_samples["prompt"].append(prompt)
-        new_samples["label"].append(ID2LABEL[label])
-
-    return new_samples
-
-
-#  model = AutoModelForCausalLM.from_pretrained(MODEL).eval().half().to("cuda:0")
-model = AutoGPTQForCausalLM.from_pretrained(MODEL, BaseQuantizeConfig())
-tokenizer = AutoTokenizer.from_pretrained(MODEL)
-
-task = SequenceClassificationTask(
-        model=model,
-        tokenizer=tokenizer,
-        classes=LABELS,
-        data_name_or_path=DATASET,
-        prompt_col_name="prompt",
-        label_col_name="label",
-        **{
-            "num_samples": 1000,  # how many samples will be sampled to evaluation
-            "sample_max_len": 1024,  # max tokens for each sample
-            "block_max_len": 2048,  # max tokens for each data block
-            # function to load dataset, one must only accept data_name_or_path as input 
-            # and return datasets.Dataset
-            "load_fn": partial(datasets.load_dataset, name="english"),  
-            # function to preprocess dataset, which is used for datasets.Dataset.map, 
-            # must return Dict[str, list] with only two keys: [prompt_col_name, label_col_name]
-            "preprocess_fn": ds_refactor_fn,  
-            # truncate label when sample's length exceed sample_max_len
-            "truncate_prompt": False  
-        }
-    )
-
-# note that max_new_tokens will be automatically specified internally based on given classes
-print(task.run())
-
-# self-consistency
-print(
-    task.run(
-        generation_config=GenerationConfig(
-            num_beams=3,
-            num_return_sequences=3,
-            do_sample=True
-        )
-    )
-)
-```
-
-</details>
-
-## Learn More
-[tutorials](docs/tutorial) provide step-by-step guidance to integrate `auto_gptq` with your own project and some best practice principles.
-
-[examples](examples/README.md) provide plenty of example scripts to use `auto_gptq` in different ways.
-
-## Supported Models
-
-> you can use `model.config.model_type` to compare with the table below to check whether the model you use is supported by `auto_gptq`.
-> 
-> for example, model_type of `WizardLM`, `vicuna` and `gpt4all` are all `llama`, hence they are all supported by `auto_gptq`.
-
-| model type                         | quantization | inference | peft-lora | peft-ada-lora | peft-adaption_prompt                                                                            |
-|------------------------------------|--------------|-----------|-----------|---------------|-------------------------------------------------------------------------------------------------|
-| bloom                              | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
-| gpt2                               | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
-| gpt_neox                           | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
-| gptj                               | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
-| llama                              | ✅            | ✅         | ✅         | ✅             | ✅                                                                                               |
-| moss                               | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
-| opt                                | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
-| gpt_bigcode                        | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
-| codegen                            | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
-| falcon(RefinedWebModel/RefinedWeb) | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
-
-## Supported Evaluation Tasks
-Currently, `auto_gptq` supports: `LanguageModelingTask`, `SequenceClassificationTask` and `TextSummarizationTask`; more Tasks will come soon!
-
-## Acknowledgement
-- Specially thanks **Elias Frantar**, **Saleh Ashkboos**, **Torsten Hoefler** and **Dan Alistarh** for proposing **GPTQ** algorithm and open source the [code](https://github.com/IST-DASLab/gptq).
-- Specially thanks **qwopqwop200**, for code in this project that relevant to quantization are mainly referenced from [GPTQ-for-LLaMa](https://github.com/qwopqwop200/GPTQ-for-LLaMa/tree/cuda).
-
-
-[![Star History Chart](https://api.star-history.com/svg?repos=PanQiwei/AutoGPTQ&type=Date)](https://star-history.com/#PanQiWei/AutoGPTQ&Date)
+Metadata-Version: 2.1
+Name: auto_gptq
+Version: 0.3.1
+Summary: An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
+Home-page: https://github.com/PanQiWei/AutoGPTQ
+Author: PanQiWei
+Keywords: gptq,quantization,large-language-models,pytorch,transformers
+Platform: windows
+Platform: linux
+Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
+Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: C++
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+Provides-Extra: triton
+License-File: LICENSE
+
+<h1 align="center">AutoGPTQ</h1>
+<p align="center">An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.</p>
+<p align="center">
+    <a href="https://github.com/PanQiWei/AutoGPTQ/releases">
+        <img alt="GitHub release" src="https://img.shields.io/github/release/PanQiWei/AutoGPTQ.svg">
+    </a>
+    <a href="https://pypi.org/project/auto-gptq/">
+        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/auto-gptq">
+    </a>
+</p>
+<h4 align="center">
+    <p>
+        <b>English</b> |
+        <a href="https://github.com/PanQiWei/AutoGPTQ/blob/main/README_zh.md">中文</a>
+    </p>
+</h4>
+
+*<center>📣 Long time no see! 👋 Architecture upgrade, performance optimization and more new features will come in July and August, stay tune! 🥂</center>*
+
+## News or Update
+
+- 2023-07-26 - (Update) - An elegant [PPL benchmark script](examples/benchmark/perplexity.py) to get results that can be fairly compared with other libraries such as `llama.cpp`.
+- 2023-06-05 - (Update) - Integrate with 🤗 peft to use gptq quantized model to train adapters, support LoRA, AdaLoRA, AdaptionPrompt, etc.
+- 2023-05-30 - (Update) - Support download/upload quantized model from/to 🤗 Hub.
+- 2023-05-27 - (Update) - Support quantization and inference for `gpt_bigcode`, `codegen` and `RefineWeb/RefineWebModel`(falcon) model types.
+- 2023-05-04 - (Update) - Support using faster cuda kernel when `not desc_act or group_size == -1`.
+
+*For more histories please turn to [here](docs/NEWS_OR_UPDATE.md)*
+
+## Performance Comparison
+
+### Inference Speed
+> The result is generated using [this script](examples/benchmark/generation_speed.py), batch size of input is 1, decode strategy is beam search and enforce the model to generate 512 tokens, speed metric is tokens/s (the larger, the better).
+> 
+> The quantized model is loaded using the setup that can gain the fastest inference speed.
+
+| model         | GPU           | num_beams | fp16  | gptq-int4 |
+|---------------|---------------|-----------|-------|-----------|
+| llama-7b      | 1xA100-40G    | 1         | 18.87 | 25.53     |
+| llama-7b      | 1xA100-40G    | 4         | 68.79 | 91.30     |
+| moss-moon 16b | 1xA100-40G    | 1         | 12.48 | 15.25     |
+| moss-moon 16b | 1xA100-40G    | 4         | OOM   | 42.67     |
+| moss-moon 16b | 2xA100-40G    | 1         | 06.83 | 06.78     |
+| moss-moon 16b | 2xA100-40G    | 4         | 13.10 | 10.80     |
+| gpt-j 6b      | 1xRTX3060-12G | 1         | OOM   | 29.55     |
+| gpt-j 6b      | 1xRTX3060-12G | 4         | OOM   | 47.36     |
+
+
+### Perplexity
+For perplexity comparison, you can turn to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes)
+
+## Installation
+
+### Quick Installation
+You can install the latest stable release of AutoGPTQ from pip:
+```shell
+pip install auto-gptq
+```
+Start from v0.2.0, you can download pre-build wheel that satisfied your environment setup from each version's release assets and install it to skip building stage for the fastest installation speed. For example:
+```shell
+# firstly, cd the directory where the wheel saved, then execute command below
+pip install auto_gptq-0.2.0+cu118-cp310-cp310-linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for linux in an environment whose python=3.10 and cuda=11.8
+```
+#### disable cuda extensions
+By default, cuda extensions will be installed when `torch` and `cuda` is already installed in your machine, if you don't want to use them, using:
+```shell
+BUILD_CUDA_EXT=0 pip install auto-gptq
+```
+And to make sure `autogptq_cuda` is not ever in your virtual environment, run:
+```shell
+pip uninstall autogptq_cuda -y
+```
+
+#### to support triton speedup
+To integrate with `triton`, using:
+> warning: currently triton only supports linux; 3-bit quantization is not supported when using triton
+
+```shell
+pip install auto-gptq[triton]
+```
+
+### Install from source
+<details>
+<summary>click to see details</summary>
+
+Clone the source code:
+```shell
+git clone https://github.com/PanQiWei/AutoGPTQ.git && cd AutoGPTQ
+```
+Then, install from source:
+```shell
+pip install .
+```
+Like quick installation, you can also set `BUILD_CUDA_EXT=0` to disable pytorch extension building.
+
+Use `.[triton]` if you want to integrate with triton and it's available on your operating system.
+
+</details>
+
+## Quick Tour
+
+### Quantization and Inference
+> warning: this is just a showcase of the usage of basic apis in AutoGPTQ, which uses only one sample to quantize a much small model, quality of quantized model using such little samples may not good.
+
+Below is an example for the simplest use of `auto_gptq` to quantize a model and inference after quantization: 
+```python
+from transformers import AutoTokenizer, TextGenerationPipeline
+from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
+import logging
+
+logging.basicConfig(
+    format="%(asctime)s %(levelname)s [%(name)s] %(message)s", level=logging.INFO, datefmt="%Y-%m-%d %H:%M:%S"
+)
+
+pretrained_model_dir = "facebook/opt-125m"
+quantized_model_dir = "opt-125m-4bit"
+
+tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir, use_fast=True)
+examples = [
+    tokenizer(
+        "auto-gptq is an easy-to-use model quantization library with user-friendly apis, based on GPTQ algorithm."
+    )
+]
+
+quantize_config = BaseQuantizeConfig(
+    bits=4,  # quantize model to 4-bit
+    group_size=128,  # it is recommended to set the value to 128
+    desc_act=False,  # set to False can significantly speed up inference but the perplexity may slightly bad 
+)
+
+# load un-quantized model, by default, the model will always be loaded into CPU memory
+model = AutoGPTQForCausalLM.from_pretrained(pretrained_model_dir, quantize_config)
+
+# quantize model, the examples should be list of dict whose keys can only be "input_ids" and "attention_mask"
+model.quantize(examples)
+
+# save quantized model
+model.save_quantized(quantized_model_dir)
+
+# save quantized model using safetensors
+model.save_quantized(quantized_model_dir, use_safetensors=True)
+
+# push quantized model to Hugging Face Hub. 
+# to use use_auth_token=True, Login first via huggingface-cli login.
+# or pass explcit token with: use_auth_token="hf_xxxxxxx"
+# (uncomment the following three lines to enable this feature)
+# repo_id = f"YourUserName/{quantized_model_dir}"
+# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
+# model.push_to_hub(repo_id, commit_message=commit_message, use_auth_token=True)
+
+# alternatively you can save and push at the same time
+# (uncomment the following three lines to enable this feature)
+# repo_id = f"YourUserName/{quantized_model_dir}"
+# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
+# model.push_to_hub(repo_id, save_dir=quantized_model_dir, use_safetensors=True, commit_message=commit_message, use_auth_token=True)
+
+# load quantized model to the first GPU
+model = AutoGPTQForCausalLM.from_quantized(quantized_model_dir, device="cuda:0")
+
+# download quantized model from Hugging Face Hub and load to the first GPU
+# model = AutoGPTQForCausalLM.from_quantized(repo_id, device="cuda:0", use_safetensors=True, use_triton=False)
+
+# inference with model.generate
+print(tokenizer.decode(model.generate(**tokenizer("auto_gptq is", return_tensors="pt").to(model.device))[0]))
+
+# or you can also use pipeline
+pipeline = TextGenerationPipeline(model=model, tokenizer=tokenizer)
+print(pipeline("auto-gptq is")[0]["generated_text"])
+```
+
+For more advanced features of model quantization, please reference to [this script](examples/quantization/quant_with_alpaca.py)
+
+### Customize Model
+<details>
+
+<summary>Below is an example to extend `auto_gptq` to support `OPT` model, as you will see, it's very easy:</summary>
+
+```python
+from auto_gptq.modeling import BaseGPTQForCausalLM
+
+
+class OPTGPTQForCausalLM(BaseGPTQForCausalLM):
+    # chained attribute name of transformer layer block
+    layers_block_name = "model.decoder.layers"
+    # chained attribute names of other nn modules that in the same level as the transformer layer block
+    outside_layer_modules = [
+        "model.decoder.embed_tokens", "model.decoder.embed_positions", "model.decoder.project_out",
+        "model.decoder.project_in", "model.decoder.final_layer_norm"
+    ]
+    # chained attribute names of linear layers in transformer layer module
+    # normally, there are four sub lists, for each one the modules in it can be seen as one operation, 
+    # and the order should be the order when they are truly executed, in this case (and usually in most cases), 
+    # they are: attention q_k_v projection, attention output projection, MLP project input, MLP project output
+    inside_layer_modules = [
+        ["self_attn.k_proj", "self_attn.v_proj", "self_attn.q_proj"],
+        ["self_attn.out_proj"],
+        ["fc1"],
+        ["fc2"]
+    ]
+```
+After this, you can use `OPTGPTQForCausalLM.from_pretrained` and other methods as shown in Basic.
+
+</details>
+
+### Evaluation on Downstream Tasks
+You can use tasks defined in `auto_gptq.eval_tasks` to evaluate model's performance on specific down-stream task before and after quantization.
+
+The predefined tasks support all causal-language-models implemented in [🤗 transformers](https://github.com/huggingface/transformers) and in this project.
+
+<details>
+
+<summary>Below is an example to evaluate `EleutherAI/gpt-j-6b` on sequence-classification task using `cardiffnlp/tweet_sentiment_multilingual` dataset:</summary>
+
+```python
+from functools import partial
+
+import datasets
+from transformers import AutoTokenizer, AutoModelForCausalLM, GenerationConfig
+
+from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
+from auto_gptq.eval_tasks import SequenceClassificationTask
+
+
+MODEL = "EleutherAI/gpt-j-6b"
+DATASET = "cardiffnlp/tweet_sentiment_multilingual"
+TEMPLATE = "Question:What's the sentiment of the given text? Choices are {labels}.\nText: {text}\nAnswer:"
+ID2LABEL = {
+    0: "negative",
+    1: "neutral",
+    2: "positive"
+}
+LABELS = list(ID2LABEL.values())
+
+
+def ds_refactor_fn(samples):
+    text_data = samples["text"]
+    label_data = samples["label"]
+
+    new_samples = {"prompt": [], "label": []}
+    for text, label in zip(text_data, label_data):
+        prompt = TEMPLATE.format(labels=LABELS, text=text)
+        new_samples["prompt"].append(prompt)
+        new_samples["label"].append(ID2LABEL[label])
+
+    return new_samples
+
+
+#  model = AutoModelForCausalLM.from_pretrained(MODEL).eval().half().to("cuda:0")
+model = AutoGPTQForCausalLM.from_pretrained(MODEL, BaseQuantizeConfig())
+tokenizer = AutoTokenizer.from_pretrained(MODEL)
+
+task = SequenceClassificationTask(
+        model=model,
+        tokenizer=tokenizer,
+        classes=LABELS,
+        data_name_or_path=DATASET,
+        prompt_col_name="prompt",
+        label_col_name="label",
+        **{
+            "num_samples": 1000,  # how many samples will be sampled to evaluation
+            "sample_max_len": 1024,  # max tokens for each sample
+            "block_max_len": 2048,  # max tokens for each data block
+            # function to load dataset, one must only accept data_name_or_path as input 
+            # and return datasets.Dataset
+            "load_fn": partial(datasets.load_dataset, name="english"),  
+            # function to preprocess dataset, which is used for datasets.Dataset.map, 
+            # must return Dict[str, list] with only two keys: [prompt_col_name, label_col_name]
+            "preprocess_fn": ds_refactor_fn,  
+            # truncate label when sample's length exceed sample_max_len
+            "truncate_prompt": False  
+        }
+    )
+
+# note that max_new_tokens will be automatically specified internally based on given classes
+print(task.run())
+
+# self-consistency
+print(
+    task.run(
+        generation_config=GenerationConfig(
+            num_beams=3,
+            num_return_sequences=3,
+            do_sample=True
+        )
+    )
+)
+```
+
+</details>
+
+## Learn More
+[tutorials](docs/tutorial) provide step-by-step guidance to integrate `auto_gptq` with your own project and some best practice principles.
+
+[examples](examples/README.md) provide plenty of example scripts to use `auto_gptq` in different ways.
+
+## Supported Models
+
+> you can use `model.config.model_type` to compare with the table below to check whether the model you use is supported by `auto_gptq`.
+> 
+> for example, model_type of `WizardLM`, `vicuna` and `gpt4all` are all `llama`, hence they are all supported by `auto_gptq`.
+
+| model type                         | quantization | inference | peft-lora | peft-ada-lora | peft-adaption_prompt                                                                            |
+|------------------------------------|--------------|-----------|-----------|---------------|-------------------------------------------------------------------------------------------------|
+| bloom                              | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| gpt2                               | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| gpt_neox                           | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
+| gptj                               | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
+| llama                              | ✅            | ✅         | ✅         | ✅             | ✅                                                                                               |
+| moss                               | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
+| opt                                | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| gpt_bigcode                        | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| codegen                            | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| falcon(RefinedWebModel/RefinedWeb) | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+
+## Supported Evaluation Tasks
+Currently, `auto_gptq` supports: `LanguageModelingTask`, `SequenceClassificationTask` and `TextSummarizationTask`; more Tasks will come soon!
+
+## Acknowledgement
+- Specially thanks **Elias Frantar**, **Saleh Ashkboos**, **Torsten Hoefler** and **Dan Alistarh** for proposing **GPTQ** algorithm and open source the [code](https://github.com/IST-DASLab/gptq).
+- Specially thanks **qwopqwop200**, for code in this project that relevant to quantization are mainly referenced from [GPTQ-for-LLaMa](https://github.com/qwopqwop200/GPTQ-for-LLaMa/tree/cuda).
+
+
+[![Star History Chart](https://api.star-history.com/svg?repos=PanQiwei/AutoGPTQ&type=Date)](https://star-history.com/#PanQiWei/AutoGPTQ&Date)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auto_gptq Version: 0.3.0 Summary: An easy-to-use
+Metadata-Version: 2.1 Name: auto_gptq Version: 0.3.1 Summary: An easy-to-use
 LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
 Home-page: https://github.com/PanQiWei/AutoGPTQ Author: PanQiWei Keywords:
 gptq,quantization,large-language-models,pytorch,transformers Platform: windows
 Platform: linux Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8 Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: Chinese
 (Simplified) Classifier: Natural Language :: English Classifier: Programming
@@ -14,82 +14,84 @@
 An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ
                                   algorithm.
                       [GitHub_release] [PyPI_-_Downloads]
                            *** English | ä¸­æ ***
 *
 ð£ Long time no see! ð Architecture upgrade, performance optimization and
         more new features will come in July and August, stay tune! ð¥
-* ## News or Update - 2023-06-05 - (Update) - Integrate with ð¤ peft to use
-gptq quantized model to train adapters, support LoRA, AdaLoRA, AdaptionPrompt,
-etc. - 2023-05-30 - (Update) - Support download/upload quantized model from/to
-ð¤ Hub. - 2023-05-27 - (Update) - Support quantization and inference for
-`gpt_bigcode`, `codegen` and `RefineWeb/RefineWebModel`(falcon) model types. -
-2023-05-04 - (Update) - Support using faster cuda kernel when `not desc_act or
-group_size == -1`. *For more histories please turn to [here](docs/
-NEWS_OR_UPDATE.md)* ## Performance Comparison ### Inference Speed > The result
-is generated using [this script](examples/benchmark/generation_speed.py), batch
-size of input is 1, decode strategy is beam search and enforce the model to
-generate 512 tokens, speed metric is tokens/s (the larger, the better). > > The
-quantized model is loaded using the setup that can gain the fastest inference
-speed. | model | GPU | num_beams | fp16 | gptq-int4 | |---------------|--------
--------|-----------|-------|-----------| | llama-7b | 1xA100-40G | 1 | 18.87 |
-25.53 | | llama-7b | 1xA100-40G | 4 | 68.79 | 91.30 | | moss-moon 16b | 1xA100-
-40G | 1 | 12.48 | 15.25 | | moss-moon 16b | 1xA100-40G | 4 | OOM | 42.67 | |
-moss-moon 16b | 2xA100-40G | 1 | 06.83 | 06.78 | | moss-moon 16b | 2xA100-40G |
-4 | 13.10 | 10.80 | | gpt-j 6b | 1xRTX3060-12G | 1 | OOM | 29.55 | | gpt-j 6b |
-1xRTX3060-12G | 4 | OOM | 47.36 | ### Perplexity For perplexity comparison, you
-can turn to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and
-[here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes) ##
-Installation ### Quick Installation You can install the latest stable release
-of AutoGPTQ from pip: ```shell pip install auto-gptq ``` Start from v0.2.0, you
-can download pre-build wheel that satisfied your environment setup from each
-version's release assets and install it to skip building stage for the fastest
-installation speed. For example: ```shell # firstly, cd the directory where the
-wheel saved, then execute command below pip install auto_gptq-0.2.0+cu118-
-cp310-cp310-linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for
-linux in an environment whose python=3.10 and cuda=11.8 ``` #### disable cuda
-extensions By default, cuda extensions will be installed when `torch` and
-`cuda` is already installed in your machine, if you don't want to use them,
-using: ```shell BUILD_CUDA_EXT=0 pip install auto-gptq ``` And to make sure
-`autogptq_cuda` is not ever in your virtual environment, run: ```shell pip
-uninstall autogptq_cuda -y ``` #### to support triton speedup To integrate with
-`triton`, using: > warning: currently triton only supports linux; 3-bit
-quantization is not supported when using triton ```shell pip install auto-gptq
-[triton] ``` ### Install from source  click to see details Clone the source
-code: ```shell git clone https://github.com/PanQiWei/AutoGPTQ.git && cd
-AutoGPTQ ``` Then, install from source: ```shell pip install . ``` Like quick
-installation, you can also set `BUILD_CUDA_EXT=0` to disable pytorch extension
-building. Use `.[triton]` if you want to integrate with triton and it's
-available on your operating system.  ## Quick Tour ### Quantization and
-Inference > warning: this is just a showcase of the usage of basic apis in
-AutoGPTQ, which uses only one sample to quantize a much small model, quality of
-quantized model using such little samples may not good. Below is an example for
-the simplest use of `auto_gptq` to quantize a model and inference after
-quantization: ```python from transformers import AutoTokenizer,
-TextGenerationPipeline from auto_gptq import AutoGPTQForCausalLM,
-BaseQuantizeConfig import logging logging.basicConfig( format="%(asctime)s %
-(levelname)s [%(name)s] %(message)s", level=logging.INFO, datefmt="%Y-%m-%d %H:
-%M:%S" ) pretrained_model_dir = "facebook/opt-125m" quantized_model_dir = "opt-
-125m-4bit" tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir,
-use_fast=True) examples = [ tokenizer( "auto-gptq is an easy-to-use model
-quantization library with user-friendly apis, based on GPTQ algorithm." ) ]
-quantize_config = BaseQuantizeConfig( bits=4, # quantize model to 4-bit
-group_size=128, # it is recommended to set the value to 128 desc_act=False, #
-set to False can significantly speed up inference but the perplexity may
-slightly bad ) # load un-quantized model, by default, the model will always be
-loaded into CPU memory model = AutoGPTQForCausalLM.from_pretrained
-(pretrained_model_dir, quantize_config) # quantize model, the examples should
-be list of dict whose keys can only be "input_ids" and "attention_mask"
-model.quantize(examples) # save quantized model model.save_quantized
-(quantized_model_dir) # save quantized model using safetensors
-model.save_quantized(quantized_model_dir, use_safetensors=True) # push
-quantized model to Hugging Face Hub. # to use use_auth_token=True, Login first
-via huggingface-cli login. # or pass explcit token with:
-use_auth_token="hf_xxxxxxx" # (uncomment the following three lines to enable
-this feature) # repo_id = f"YourUserName/{quantized_model_dir}" #
+* ## News or Update - 2023-07-26 - (Update) - An elegant [PPL benchmark script]
+(examples/benchmark/perplexity.py) to get results that can be fairly compared
+with other libraries such as `llama.cpp`. - 2023-06-05 - (Update) - Integrate
+with ð¤ peft to use gptq quantized model to train adapters, support LoRA,
+AdaLoRA, AdaptionPrompt, etc. - 2023-05-30 - (Update) - Support download/upload
+quantized model from/to ð¤ Hub. - 2023-05-27 - (Update) - Support
+quantization and inference for `gpt_bigcode`, `codegen` and `RefineWeb/
+RefineWebModel`(falcon) model types. - 2023-05-04 - (Update) - Support using
+faster cuda kernel when `not desc_act or group_size == -1`. *For more histories
+please turn to [here](docs/NEWS_OR_UPDATE.md)* ## Performance Comparison ###
+Inference Speed > The result is generated using [this script](examples/
+benchmark/generation_speed.py), batch size of input is 1, decode strategy is
+beam search and enforce the model to generate 512 tokens, speed metric is
+tokens/s (the larger, the better). > > The quantized model is loaded using the
+setup that can gain the fastest inference speed. | model | GPU | num_beams |
+fp16 | gptq-int4 | |---------------|---------------|-----------|-------|-------
+----| | llama-7b | 1xA100-40G | 1 | 18.87 | 25.53 | | llama-7b | 1xA100-40G | 4
+| 68.79 | 91.30 | | moss-moon 16b | 1xA100-40G | 1 | 12.48 | 15.25 | | moss-
+moon 16b | 1xA100-40G | 4 | OOM | 42.67 | | moss-moon 16b | 2xA100-40G | 1 |
+06.83 | 06.78 | | moss-moon 16b | 2xA100-40G | 4 | 13.10 | 10.80 | | gpt-j 6b |
+1xRTX3060-12G | 1 | OOM | 29.55 | | gpt-j 6b | 1xRTX3060-12G | 4 | OOM | 47.36
+| ### Perplexity For perplexity comparison, you can turn to [here](https://
+github.com/qwopqwop200/GPTQ-for-LLaMa#result) and [here](https://github.com/
+qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes) ## Installation ### Quick
+Installation You can install the latest stable release of AutoGPTQ from pip:
+```shell pip install auto-gptq ``` Start from v0.2.0, you can download pre-
+build wheel that satisfied your environment setup from each version's release
+assets and install it to skip building stage for the fastest installation
+speed. For example: ```shell # firstly, cd the directory where the wheel saved,
+then execute command below pip install auto_gptq-0.2.0+cu118-cp310-cp310-
+linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for linux in an
+environment whose python=3.10 and cuda=11.8 ``` #### disable cuda extensions By
+default, cuda extensions will be installed when `torch` and `cuda` is already
+installed in your machine, if you don't want to use them, using: ```shell
+BUILD_CUDA_EXT=0 pip install auto-gptq ``` And to make sure `autogptq_cuda` is
+not ever in your virtual environment, run: ```shell pip uninstall autogptq_cuda
+-y ``` #### to support triton speedup To integrate with `triton`, using: >
+warning: currently triton only supports linux; 3-bit quantization is not
+supported when using triton ```shell pip install auto-gptq[triton] ``` ###
+Install from source  click to see details Clone the source code: ```shell git
+clone https://github.com/PanQiWei/AutoGPTQ.git && cd AutoGPTQ ``` Then, install
+from source: ```shell pip install . ``` Like quick installation, you can also
+set `BUILD_CUDA_EXT=0` to disable pytorch extension building. Use `.[triton]`
+if you want to integrate with triton and it's available on your operating
+system.  ## Quick Tour ### Quantization and Inference > warning: this is just a
+showcase of the usage of basic apis in AutoGPTQ, which uses only one sample to
+quantize a much small model, quality of quantized model using such little
+samples may not good. Below is an example for the simplest use of `auto_gptq`
+to quantize a model and inference after quantization: ```python from
+transformers import AutoTokenizer, TextGenerationPipeline from auto_gptq import
+AutoGPTQForCausalLM, BaseQuantizeConfig import logging logging.basicConfig
+( format="%(asctime)s %(levelname)s [%(name)s] %(message)s",
+level=logging.INFO, datefmt="%Y-%m-%d %H:%M:%S" ) pretrained_model_dir =
+"facebook/opt-125m" quantized_model_dir = "opt-125m-4bit" tokenizer =
+AutoTokenizer.from_pretrained(pretrained_model_dir, use_fast=True) examples =
+[ tokenizer( "auto-gptq is an easy-to-use model quantization library with user-
+friendly apis, based on GPTQ algorithm." ) ] quantize_config =
+BaseQuantizeConfig( bits=4, # quantize model to 4-bit group_size=128, # it is
+recommended to set the value to 128 desc_act=False, # set to False can
+significantly speed up inference but the perplexity may slightly bad ) # load
+un-quantized model, by default, the model will always be loaded into CPU memory
+model = AutoGPTQForCausalLM.from_pretrained(pretrained_model_dir,
+quantize_config) # quantize model, the examples should be list of dict whose
+keys can only be "input_ids" and "attention_mask" model.quantize(examples) #
+save quantized model model.save_quantized(quantized_model_dir) # save quantized
+model using safetensors model.save_quantized(quantized_model_dir,
+use_safetensors=True) # push quantized model to Hugging Face Hub. # to use
+use_auth_token=True, Login first via huggingface-cli login. # or pass explcit
+token with: use_auth_token="hf_xxxxxxx" # (uncomment the following three lines
+to enable this feature) # repo_id = f"YourUserName/{quantized_model_dir}" #
 commit_message = f"AutoGPTQ model for {pretrained_model_dir}:
 {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act=
 {quantize_config.desc_act}" # model.push_to_hub(repo_id,
 commit_message=commit_message, use_auth_token=True) # alternatively you can
 save and push at the same time # (uncomment the following three lines to enable
 this feature) # repo_id = f"YourUserName/{quantized_model_dir}" #
 commit_message = f"AutoGPTQ model for {pretrained_model_dir}:
```

### Comparing `auto_gptq-0.3.0/README.md` & `auto_gptq-0.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,998 +1,989 @@
 00000000: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
 00000010: 7222 3e41 7574 6f47 5054 513c 2f68 313e  r">AutoGPTQ</h1>
-00000020: 0d0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
-00000030: 6572 223e 416e 2065 6173 792d 746f 2d75  er">An easy-to-u
-00000040: 7365 204c 4c4d 7320 7175 616e 7469 7a61  se LLMs quantiza
-00000050: 7469 6f6e 2070 6163 6b61 6765 2077 6974  tion package wit
-00000060: 6820 7573 6572 2d66 7269 656e 646c 7920  h user-friendly 
-00000070: 6170 6973 2c20 6261 7365 6420 6f6e 2047  apis, based on G
-00000080: 5054 5120 616c 676f 7269 7468 6d2e 3c2f  PTQ algorithm.</
-00000090: 703e 0d0a 3c70 2061 6c69 676e 3d22 6365  p>..<p align="ce
-000000a0: 6e74 6572 223e 0d0a 2020 2020 3c61 2068  nter">..    <a h
-000000b0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-000000c0: 6875 622e 636f 6d2f 5061 6e51 6957 6569  hub.com/PanQiWei
-000000d0: 2f41 7574 6f47 5054 512f 7265 6c65 6173  /AutoGPTQ/releas
-000000e0: 6573 223e 0d0a 2020 2020 2020 2020 3c69  es">..        <i
-000000f0: 6d67 2061 6c74 3d22 4769 7448 7562 2072  mg alt="GitHub r
-00000100: 656c 6561 7365 2220 7372 633d 2268 7474  elease" src="htt
-00000110: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000120: 2e69 6f2f 6769 7468 7562 2f72 656c 6561  .io/github/relea
-00000130: 7365 2f50 616e 5169 5765 692f 4175 746f  se/PanQiWei/Auto
-00000140: 4750 5451 2e73 7667 223e 0d0a 2020 2020  GPTQ.svg">..    
-00000150: 3c2f 613e 0d0a 2020 2020 3c61 2068 7265  </a>..    <a hre
-00000160: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
-00000170: 6f72 672f 7072 6f6a 6563 742f 6175 746f  org/project/auto
-00000180: 2d67 7074 712f 223e 0d0a 2020 2020 2020  -gptq/">..      
-00000190: 2020 3c69 6d67 2061 6c74 3d22 5079 5049    <img alt="PyPI
-000001a0: 202d 2044 6f77 6e6c 6f61 6473 2220 7372   - Downloads" sr
-000001b0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-000001c0: 6869 656c 6473 2e69 6f2f 7079 7069 2f64  hields.io/pypi/d
-000001d0: 642f 6175 746f 2d67 7074 7122 3e0d 0a20  d/auto-gptq">.. 
-000001e0: 2020 203c 2f61 3e0d 0a3c 2f70 3e0d 0a3c     </a>..</p>..<
-000001f0: 6834 2061 6c69 676e 3d22 6365 6e74 6572  h4 align="center
-00000200: 223e 0d0a 2020 2020 3c70 3e0d 0a20 2020  ">..    <p>..   
-00000210: 2020 2020 203c 623e 456e 676c 6973 683c       <b>English<
-00000220: 2f62 3e20 7c0d 0a20 2020 2020 2020 203c  /b> |..        <
-00000230: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000240: 6769 7468 7562 2e63 6f6d 2f50 616e 5169  github.com/PanQi
-00000250: 5765 692f 4175 746f 4750 5451 2f62 6c6f  Wei/AutoGPTQ/blo
-00000260: 622f 6d61 696e 2f52 4541 444d 455f 7a68  b/main/README_zh
-00000270: 2e6d 6422 3ee4 b8ad e696 873c 2f61 3e0d  .md">......</a>.
-00000280: 0a20 2020 203c 2f70 3e0d 0a3c 2f68 343e  .    </p>..</h4>
-00000290: 0d0a 0d0a 2a3c 6365 6e74 6572 3ef0 9f93  ....*<center>...
-000002a0: a320 4c6f 6e67 2074 696d 6520 6e6f 2073  . Long time no s
-000002b0: 6565 2120 f09f 918b 2041 7263 6869 7465  ee! .... Archite
-000002c0: 6374 7572 6520 7570 6772 6164 652c 2070  cture upgrade, p
-000002d0: 6572 666f 726d 616e 6365 206f 7074 696d  erformance optim
-000002e0: 697a 6174 696f 6e20 616e 6420 6d6f 7265  ization and more
-000002f0: 206e 6577 2066 6561 7475 7265 7320 7769   new features wi
-00000300: 6c6c 2063 6f6d 6520 696e 204a 756c 7920  ll come in July 
-00000310: 616e 6420 4175 6775 7374 2c20 7374 6179  and August, stay
-00000320: 2074 756e 6521 20f0 9fa5 823c 2f63 656e   tune! ....</cen
-00000330: 7465 723e 2a0d 0a0d 0a23 2320 4e65 7773  ter>*....## News
-00000340: 206f 7220 5570 6461 7465 0d0a 0d0a 2d20   or Update....- 
-00000350: 3230 3233 2d30 362d 3035 202d 2028 5570  2023-06-05 - (Up
-00000360: 6461 7465 2920 2d20 496e 7465 6772 6174  date) - Integrat
-00000370: 6520 7769 7468 20f0 9fa4 9720 7065 6674  e with .... peft
-00000380: 2074 6f20 7573 6520 6770 7471 2071 7561   to use gptq qua
-00000390: 6e74 697a 6564 206d 6f64 656c 2074 6f20  ntized model to 
-000003a0: 7472 6169 6e20 6164 6170 7465 7273 2c20  train adapters, 
-000003b0: 7375 7070 6f72 7420 4c6f 5241 2c20 4164  support LoRA, Ad
-000003c0: 614c 6f52 412c 2041 6461 7074 696f 6e50  aLoRA, AdaptionP
-000003d0: 726f 6d70 742c 2065 7463 2e0d 0a2d 2032  rompt, etc...- 2
-000003e0: 3032 332d 3035 2d33 3020 2d20 2855 7064  023-05-30 - (Upd
-000003f0: 6174 6529 202d 2053 7570 706f 7274 2064  ate) - Support d
-00000400: 6f77 6e6c 6f61 642f 7570 6c6f 6164 2071  ownload/upload q
-00000410: 7561 6e74 697a 6564 206d 6f64 656c 2066  uantized model f
-00000420: 726f 6d2f 746f 20f0 9fa4 9720 4875 622e  rom/to .... Hub.
-00000430: 0d0a 2d20 3230 3233 2d30 352d 3237 202d  ..- 2023-05-27 -
-00000440: 2028 5570 6461 7465 2920 2d20 5375 7070   (Update) - Supp
-00000450: 6f72 7420 7175 616e 7469 7a61 7469 6f6e  ort quantization
-00000460: 2061 6e64 2069 6e66 6572 656e 6365 2066   and inference f
-00000470: 6f72 2060 6770 745f 6269 6763 6f64 6560  or `gpt_bigcode`
-00000480: 2c20 6063 6f64 6567 656e 6020 616e 6420  , `codegen` and 
-00000490: 6052 6566 696e 6557 6562 2f52 6566 696e  `RefineWeb/Refin
-000004a0: 6557 6562 4d6f 6465 6c60 2866 616c 636f  eWebModel`(falco
-000004b0: 6e29 206d 6f64 656c 2074 7970 6573 2e0d  n) model types..
-000004c0: 0a2d 2032 3032 332d 3035 2d30 3420 2d20  .- 2023-05-04 - 
-000004d0: 2855 7064 6174 6529 202d 2053 7570 706f  (Update) - Suppo
-000004e0: 7274 2075 7369 6e67 2066 6173 7465 7220  rt using faster 
-000004f0: 6375 6461 206b 6572 6e65 6c20 7768 656e  cuda kernel when
-00000500: 2060 6e6f 7420 6465 7363 5f61 6374 206f   `not desc_act o
-00000510: 7220 6772 6f75 705f 7369 7a65 203d 3d20  r group_size == 
-00000520: 2d31 602e 0d0a 0d0a 2a46 6f72 206d 6f72  -1`.....*For mor
-00000530: 6520 6869 7374 6f72 6965 7320 706c 6561  e histories plea
-00000540: 7365 2074 7572 6e20 746f 205b 6865 7265  se turn to [here
-00000550: 5d28 646f 6373 2f4e 4557 535f 4f52 5f55  ](docs/NEWS_OR_U
-00000560: 5044 4154 452e 6d64 292a 0d0a 0d0a 2323  PDATE.md)*....##
-00000570: 2050 6572 666f 726d 616e 6365 2043 6f6d   Performance Com
-00000580: 7061 7269 736f 6e0d 0a0d 0a23 2323 2049  parison....### I
-00000590: 6e66 6572 656e 6365 2053 7065 6564 0d0a  nference Speed..
-000005a0: 3e20 5468 6520 7265 7375 6c74 2069 7320  > The result is 
-000005b0: 6765 6e65 7261 7465 6420 7573 696e 6720  generated using 
-000005c0: 5b74 6869 7320 7363 7269 7074 5d28 6578  [this script](ex
-000005d0: 616d 706c 6573 2f62 656e 6368 6d61 726b  amples/benchmark
-000005e0: 2f67 656e 6572 6174 696f 6e5f 7370 6565  /generation_spee
-000005f0: 642e 7079 292c 2062 6174 6368 2073 697a  d.py), batch siz
-00000600: 6520 6f66 2069 6e70 7574 2069 7320 312c  e of input is 1,
-00000610: 2064 6563 6f64 6520 7374 7261 7465 6779   decode strategy
-00000620: 2069 7320 6265 616d 2073 6561 7263 6820   is beam search 
-00000630: 616e 6420 656e 666f 7263 6520 7468 6520  and enforce the 
-00000640: 6d6f 6465 6c20 746f 2067 656e 6572 6174  model to generat
-00000650: 6520 3531 3220 746f 6b65 6e73 2c20 7370  e 512 tokens, sp
-00000660: 6565 6420 6d65 7472 6963 2069 7320 746f  eed metric is to
-00000670: 6b65 6e73 2f73 2028 7468 6520 6c61 7267  kens/s (the larg
-00000680: 6572 2c20 7468 6520 6265 7474 6572 292e  er, the better).
-00000690: 0d0a 3e20 0d0a 3e20 5468 6520 7175 616e  ..> ..> The quan
-000006a0: 7469 7a65 6420 6d6f 6465 6c20 6973 206c  tized model is l
-000006b0: 6f61 6465 6420 7573 696e 6720 7468 6520  oaded using the 
-000006c0: 7365 7475 7020 7468 6174 2063 616e 2067  setup that can g
-000006d0: 6169 6e20 7468 6520 6661 7374 6573 7420  ain the fastest 
-000006e0: 696e 6665 7265 6e63 6520 7370 6565 642e  inference speed.
-000006f0: 0d0a 0d0a 7c20 6d6f 6465 6c20 2020 2020  ....| model     
-00000700: 2020 2020 7c20 4750 5520 2020 2020 2020      | GPU       
-00000710: 2020 2020 7c20 6e75 6d5f 6265 616d 7320      | num_beams 
-00000720: 7c20 6670 3136 2020 7c20 6770 7471 2d69  | fp16  | gptq-i
-00000730: 6e74 3420 7c0d 0a7c 2d2d 2d2d 2d2d 2d2d  nt4 |..|--------
-00000740: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00000750: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00000760: 2d2d 2d7c 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d  ---|-------|----
-00000770: 2d2d 2d2d 2d2d 2d7c 0d0a 7c20 6c6c 616d  -------|..| llam
-00000780: 612d 3762 2020 2020 2020 7c20 3178 4131  a-7b      | 1xA1
-00000790: 3030 2d34 3047 2020 2020 7c20 3120 2020  00-40G    | 1   
-000007a0: 2020 2020 2020 7c20 3138 2e38 3720 7c20        | 18.87 | 
-000007b0: 3235 2e35 3320 2020 2020 7c0d 0a7c 206c  25.53     |..| l
-000007c0: 6c61 6d61 2d37 6220 2020 2020 207c 2031  lama-7b      | 1
-000007d0: 7841 3130 302d 3430 4720 2020 207c 2034  xA100-40G    | 4
-000007e0: 2020 2020 2020 2020 207c 2036 382e 3739           | 68.79
-000007f0: 207c 2039 312e 3330 2020 2020 207c 0d0a   | 91.30     |..
-00000800: 7c20 6d6f 7373 2d6d 6f6f 6e20 3136 6220  | moss-moon 16b 
-00000810: 7c20 3178 4131 3030 2d34 3047 2020 2020  | 1xA100-40G    
-00000820: 7c20 3120 2020 2020 2020 2020 7c20 3132  | 1         | 12
-00000830: 2e34 3820 7c20 3135 2e32 3520 2020 2020  .48 | 15.25     
-00000840: 7c0d 0a7c 206d 6f73 732d 6d6f 6f6e 2031  |..| moss-moon 1
-00000850: 3662 207c 2031 7841 3130 302d 3430 4720  6b | 1xA100-40G 
-00000860: 2020 207c 2034 2020 2020 2020 2020 207c     | 4         |
-00000870: 204f 4f4d 2020 207c 2034 322e 3637 2020   OOM   | 42.67  
-00000880: 2020 207c 0d0a 7c20 6d6f 7373 2d6d 6f6f     |..| moss-moo
-00000890: 6e20 3136 6220 7c20 3278 4131 3030 2d34  n 16b | 2xA100-4
-000008a0: 3047 2020 2020 7c20 3120 2020 2020 2020  0G    | 1       
-000008b0: 2020 7c20 3036 2e38 3320 7c20 3036 2e37    | 06.83 | 06.7
-000008c0: 3820 2020 2020 7c0d 0a7c 206d 6f73 732d  8     |..| moss-
-000008d0: 6d6f 6f6e 2031 3662 207c 2032 7841 3130  moon 16b | 2xA10
-000008e0: 302d 3430 4720 2020 207c 2034 2020 2020  0-40G    | 4    
-000008f0: 2020 2020 207c 2031 332e 3130 207c 2031       | 13.10 | 1
-00000900: 302e 3830 2020 2020 207c 0d0a 7c20 6770  0.80     |..| gp
-00000910: 742d 6a20 3662 2020 2020 2020 7c20 3178  t-j 6b      | 1x
-00000920: 5254 5833 3036 302d 3132 4720 7c20 3120  RTX3060-12G | 1 
-00000930: 2020 2020 2020 2020 7c20 4f4f 4d20 2020          | OOM   
-00000940: 7c20 3239 2e35 3520 2020 2020 7c0d 0a7c  | 29.55     |..|
-00000950: 2067 7074 2d6a 2036 6220 2020 2020 207c   gpt-j 6b      |
-00000960: 2031 7852 5458 3330 3630 2d31 3247 207c   1xRTX3060-12G |
-00000970: 2034 2020 2020 2020 2020 207c 204f 4f4d   4         | OOM
-00000980: 2020 207c 2034 372e 3336 2020 2020 207c     | 47.36     |
-00000990: 0d0a 0d0a 0d0a 2323 2320 5065 7270 6c65  ......### Perple
-000009a0: 7869 7479 0d0a 466f 7220 7065 7270 6c65  xity..For perple
-000009b0: 7869 7479 2063 6f6d 7061 7269 736f 6e2c  xity comparison,
-000009c0: 2079 6f75 2063 616e 2074 7572 6e20 746f   you can turn to
-000009d0: 205b 6865 7265 5d28 6874 7470 733a 2f2f   [here](https://
-000009e0: 6769 7468 7562 2e63 6f6d 2f71 776f 7071  github.com/qwopq
-000009f0: 776f 7032 3030 2f47 5054 512d 666f 722d  wop200/GPTQ-for-
-00000a00: 4c4c 614d 6123 7265 7375 6c74 2920 616e  LLaMa#result) an
-00000a10: 6420 5b68 6572 655d 2868 7474 7073 3a2f  d [here](https:/
-00000a20: 2f67 6974 6875 622e 636f 6d2f 7177 6f70  /github.com/qwop
-00000a30: 7177 6f70 3230 302f 4750 5451 2d66 6f72  qwop200/GPTQ-for
-00000a40: 2d4c 4c61 4d61 2367 7074 712d 7673 2d62  -LLaMa#gptq-vs-b
-00000a50: 6974 7361 6e64 6279 7465 7329 0d0a 0d0a  itsandbytes)....
-00000a60: 2323 2049 6e73 7461 6c6c 6174 696f 6e0d  ## Installation.
-00000a70: 0a0d 0a23 2323 2051 7569 636b 2049 6e73  ...### Quick Ins
-00000a80: 7461 6c6c 6174 696f 6e0d 0a59 6f75 2063  tallation..You c
-00000a90: 616e 2069 6e73 7461 6c6c 2074 6865 206c  an install the l
-00000aa0: 6174 6573 7420 7374 6162 6c65 2072 656c  atest stable rel
-00000ab0: 6561 7365 206f 6620 4175 746f 4750 5451  ease of AutoGPTQ
-00000ac0: 2066 726f 6d20 7069 703a 0d0a 6060 6073   from pip:..```s
-00000ad0: 6865 6c6c 0d0a 7069 7020 696e 7374 616c  hell..pip instal
-00000ae0: 6c20 6175 746f 2d67 7074 710d 0a60 6060  l auto-gptq..```
-00000af0: 0d0a 5374 6172 7420 6672 6f6d 2076 302e  ..Start from v0.
-00000b00: 322e 302c 2079 6f75 2063 616e 2064 6f77  2.0, you can dow
-00000b10: 6e6c 6f61 6420 7072 652d 6275 696c 6420  nload pre-build 
-00000b20: 7768 6565 6c20 7468 6174 2073 6174 6973  wheel that satis
-00000b30: 6669 6564 2079 6f75 7220 656e 7669 726f  fied your enviro
-00000b40: 6e6d 656e 7420 7365 7475 7020 6672 6f6d  nment setup from
-00000b50: 2065 6163 6820 7665 7273 696f 6e27 7320   each version's 
-00000b60: 7265 6c65 6173 6520 6173 7365 7473 2061  release assets a
-00000b70: 6e64 2069 6e73 7461 6c6c 2069 7420 746f  nd install it to
-00000b80: 2073 6b69 7020 6275 696c 6469 6e67 2073   skip building s
-00000b90: 7461 6765 2066 6f72 2074 6865 2066 6173  tage for the fas
-00000ba0: 7465 7374 2069 6e73 7461 6c6c 6174 696f  test installatio
-00000bb0: 6e20 7370 6565 642e 2046 6f72 2065 7861  n speed. For exa
-00000bc0: 6d70 6c65 3a0d 0a60 6060 7368 656c 6c0d  mple:..```shell.
-00000bd0: 0a23 2066 6972 7374 6c79 2c20 6364 2074  .# firstly, cd t
-00000be0: 6865 2064 6972 6563 746f 7279 2077 6865  he directory whe
-00000bf0: 7265 2074 6865 2077 6865 656c 2073 6176  re the wheel sav
-00000c00: 6564 2c20 7468 656e 2065 7865 6375 7465  ed, then execute
-00000c10: 2063 6f6d 6d61 6e64 2062 656c 6f77 0d0a   command below..
-00000c20: 7069 7020 696e 7374 616c 6c20 6175 746f  pip install auto
-00000c30: 5f67 7074 712d 302e 322e 302b 6375 3131  _gptq-0.2.0+cu11
-00000c40: 382d 6370 3331 302d 6370 3331 302d 6c69  8-cp310-cp310-li
-00000c50: 6e75 785f 7838 365f 3634 2e77 686c 2023  nux_x86_64.whl #
-00000c60: 2069 6e73 7461 6c6c 2076 302e 322e 3020   install v0.2.0 
-00000c70: 6175 746f 5f67 7074 7120 7072 652d 6275  auto_gptq pre-bu
-00000c80: 696c 6420 7768 6565 6c20 666f 7220 6c69  ild wheel for li
-00000c90: 6e75 7820 696e 2061 6e20 656e 7669 726f  nux in an enviro
-00000ca0: 6e6d 656e 7420 7768 6f73 6520 7079 7468  nment whose pyth
-00000cb0: 6f6e 3d33 2e31 3020 616e 6420 6375 6461  on=3.10 and cuda
-00000cc0: 3d31 312e 380d 0a60 6060 0d0a 2323 2323  =11.8..```..####
-00000cd0: 2064 6973 6162 6c65 2063 7564 6120 6578   disable cuda ex
-00000ce0: 7465 6e73 696f 6e73 0d0a 4279 2064 6566  tensions..By def
-00000cf0: 6175 6c74 2c20 6375 6461 2065 7874 656e  ault, cuda exten
-00000d00: 7369 6f6e 7320 7769 6c6c 2062 6520 696e  sions will be in
-00000d10: 7374 616c 6c65 6420 7768 656e 2060 746f  stalled when `to
-00000d20: 7263 6860 2061 6e64 2060 6375 6461 6020  rch` and `cuda` 
-00000d30: 6973 2061 6c72 6561 6479 2069 6e73 7461  is already insta
-00000d40: 6c6c 6564 2069 6e20 796f 7572 206d 6163  lled in your mac
-00000d50: 6869 6e65 2c20 6966 2079 6f75 2064 6f6e  hine, if you don
-00000d60: 2774 2077 616e 7420 746f 2075 7365 2074  't want to use t
-00000d70: 6865 6d2c 2075 7369 6e67 3a0d 0a60 6060  hem, using:..```
-00000d80: 7368 656c 6c0d 0a42 5549 4c44 5f43 5544  shell..BUILD_CUD
-00000d90: 415f 4558 543d 3020 7069 7020 696e 7374  A_EXT=0 pip inst
-00000da0: 616c 6c20 6175 746f 2d67 7074 710d 0a60  all auto-gptq..`
-00000db0: 6060 0d0a 416e 6420 746f 206d 616b 6520  ``..And to make 
-00000dc0: 7375 7265 2060 6175 746f 6770 7471 5f63  sure `autogptq_c
-00000dd0: 7564 6160 2069 7320 6e6f 7420 6576 6572  uda` is not ever
-00000de0: 2069 6e20 796f 7572 2076 6972 7475 616c   in your virtual
-00000df0: 2065 6e76 6972 6f6e 6d65 6e74 2c20 7275   environment, ru
-00000e00: 6e3a 0d0a 6060 6073 6865 6c6c 0d0a 7069  n:..```shell..pi
-00000e10: 7020 756e 696e 7374 616c 6c20 6175 746f  p uninstall auto
-00000e20: 6770 7471 5f63 7564 6120 2d79 0d0a 6060  gptq_cuda -y..``
-00000e30: 600d 0a0d 0a23 2323 2320 746f 2073 7570  `....#### to sup
-00000e40: 706f 7274 2074 7269 746f 6e20 7370 6565  port triton spee
-00000e50: 6475 700d 0a54 6f20 696e 7465 6772 6174  dup..To integrat
-00000e60: 6520 7769 7468 2060 7472 6974 6f6e 602c  e with `triton`,
-00000e70: 2075 7369 6e67 3a0d 0a3e 2077 6172 6e69   using:..> warni
-00000e80: 6e67 3a20 6375 7272 656e 746c 7920 7472  ng: currently tr
-00000e90: 6974 6f6e 206f 6e6c 7920 7375 7070 6f72  iton only suppor
-00000ea0: 7473 206c 696e 7578 3b20 332d 6269 7420  ts linux; 3-bit 
-00000eb0: 7175 616e 7469 7a61 7469 6f6e 2069 7320  quantization is 
-00000ec0: 6e6f 7420 7375 7070 6f72 7465 6420 7768  not supported wh
-00000ed0: 656e 2075 7369 6e67 2074 7269 746f 6e0d  en using triton.
-00000ee0: 0a0d 0a60 6060 7368 656c 6c0d 0a70 6970  ...```shell..pip
-00000ef0: 2069 6e73 7461 6c6c 2061 7574 6f2d 6770   install auto-gp
-00000f00: 7471 5b74 7269 746f 6e5d 0d0a 6060 600d  tq[triton]..```.
-00000f10: 0a0d 0a23 2323 2049 6e73 7461 6c6c 2066  ...### Install f
-00000f20: 726f 6d20 736f 7572 6365 0d0a 3c64 6574  rom source..<det
-00000f30: 6169 6c73 3e0d 0a3c 7375 6d6d 6172 793e  ails>..<summary>
-00000f40: 636c 6963 6b20 746f 2073 6565 2064 6574  click to see det
-00000f50: 6169 6c73 3c2f 7375 6d6d 6172 793e 0d0a  ails</summary>..
-00000f60: 0d0a 436c 6f6e 6520 7468 6520 736f 7572  ..Clone the sour
-00000f70: 6365 2063 6f64 653a 0d0a 6060 6073 6865  ce code:..```she
-00000f80: 6c6c 0d0a 6769 7420 636c 6f6e 6520 6874  ll..git clone ht
-00000f90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000fa0: 2f50 616e 5169 5765 692f 4175 746f 4750  /PanQiWei/AutoGP
-00000fb0: 5451 2e67 6974 2026 2620 6364 2041 7574  TQ.git && cd Aut
-00000fc0: 6f47 5054 510d 0a60 6060 0d0a 5468 656e  oGPTQ..```..Then
-00000fd0: 2c20 696e 7374 616c 6c20 6672 6f6d 2073  , install from s
-00000fe0: 6f75 7263 653a 0d0a 6060 6073 6865 6c6c  ource:..```shell
-00000ff0: 0d0a 7069 7020 696e 7374 616c 6c20 2e0d  ..pip install ..
-00001000: 0a60 6060 0d0a 4c69 6b65 2071 7569 636b  .```..Like quick
-00001010: 2069 6e73 7461 6c6c 6174 696f 6e2c 2079   installation, y
-00001020: 6f75 2063 616e 2061 6c73 6f20 7365 7420  ou can also set 
-00001030: 6042 5549 4c44 5f43 5544 415f 4558 543d  `BUILD_CUDA_EXT=
-00001040: 3060 2074 6f20 6469 7361 626c 6520 7079  0` to disable py
-00001050: 746f 7263 6820 6578 7465 6e73 696f 6e20  torch extension 
-00001060: 6275 696c 6469 6e67 2e0d 0a0d 0a55 7365  building.....Use
-00001070: 2060 2e5b 7472 6974 6f6e 5d60 2069 6620   `.[triton]` if 
-00001080: 796f 7520 7761 6e74 2074 6f20 696e 7465  you want to inte
-00001090: 6772 6174 6520 7769 7468 2074 7269 746f  grate with trito
-000010a0: 6e20 616e 6420 6974 2773 2061 7661 696c  n and it's avail
-000010b0: 6162 6c65 206f 6e20 796f 7572 206f 7065  able on your ope
-000010c0: 7261 7469 6e67 2073 7973 7465 6d2e 0d0a  rating system...
-000010d0: 0d0a 3c2f 6465 7461 696c 733e 0d0a 0d0a  ..</details>....
-000010e0: 2323 2051 7569 636b 2054 6f75 720d 0a0d  ## Quick Tour...
-000010f0: 0a23 2323 2051 7561 6e74 697a 6174 696f  .### Quantizatio
-00001100: 6e20 616e 6420 496e 6665 7265 6e63 650d  n and Inference.
-00001110: 0a3e 2077 6172 6e69 6e67 3a20 7468 6973  .> warning: this
-00001120: 2069 7320 6a75 7374 2061 2073 686f 7763   is just a showc
-00001130: 6173 6520 6f66 2074 6865 2075 7361 6765  ase of the usage
-00001140: 206f 6620 6261 7369 6320 6170 6973 2069   of basic apis i
-00001150: 6e20 4175 746f 4750 5451 2c20 7768 6963  n AutoGPTQ, whic
-00001160: 6820 7573 6573 206f 6e6c 7920 6f6e 6520  h uses only one 
-00001170: 7361 6d70 6c65 2074 6f20 7175 616e 7469  sample to quanti
-00001180: 7a65 2061 206d 7563 6820 736d 616c 6c20  ze a much small 
-00001190: 6d6f 6465 6c2c 2071 7561 6c69 7479 206f  model, quality o
-000011a0: 6620 7175 616e 7469 7a65 6420 6d6f 6465  f quantized mode
-000011b0: 6c20 7573 696e 6720 7375 6368 206c 6974  l using such lit
-000011c0: 746c 6520 7361 6d70 6c65 7320 6d61 7920  tle samples may 
-000011d0: 6e6f 7420 676f 6f64 2e0d 0a0d 0a42 656c  not good.....Bel
-000011e0: 6f77 2069 7320 616e 2065 7861 6d70 6c65  ow is an example
-000011f0: 2066 6f72 2074 6865 2073 696d 706c 6573   for the simples
-00001200: 7420 7573 6520 6f66 2060 6175 746f 5f67  t use of `auto_g
-00001210: 7074 7160 2074 6f20 7175 616e 7469 7a65  ptq` to quantize
-00001220: 2061 206d 6f64 656c 2061 6e64 2069 6e66   a model and inf
-00001230: 6572 656e 6365 2061 6674 6572 2071 7561  erence after qua
-00001240: 6e74 697a 6174 696f 6e3a 200d 0a60 6060  ntization: ..```
-00001250: 7079 7468 6f6e 0d0a 6672 6f6d 2074 7261  python..from tra
-00001260: 6e73 666f 726d 6572 7320 696d 706f 7274  nsformers import
-00001270: 2041 7574 6f54 6f6b 656e 697a 6572 2c20   AutoTokenizer, 
-00001280: 5465 7874 4765 6e65 7261 7469 6f6e 5069  TextGenerationPi
-00001290: 7065 6c69 6e65 0d0a 6672 6f6d 2061 7574  peline..from aut
-000012a0: 6f5f 6770 7471 2069 6d70 6f72 7420 4175  o_gptq import Au
-000012b0: 746f 4750 5451 466f 7243 6175 7361 6c4c  toGPTQForCausalL
-000012c0: 4d2c 2042 6173 6551 7561 6e74 697a 6543  M, BaseQuantizeC
-000012d0: 6f6e 6669 670d 0a69 6d70 6f72 7420 6c6f  onfig..import lo
-000012e0: 6767 696e 670d 0a0d 0a6c 6f67 6769 6e67  gging....logging
-000012f0: 2e62 6173 6963 436f 6e66 6967 280d 0a20  .basicConfig(.. 
-00001300: 2020 2066 6f72 6d61 743d 2225 2861 7363     format="%(asc
-00001310: 7469 6d65 2973 2025 286c 6576 656c 6e61  time)s %(levelna
-00001320: 6d65 2973 205b 2528 6e61 6d65 2973 5d20  me)s [%(name)s] 
-00001330: 2528 6d65 7373 6167 6529 7322 2c20 6c65  %(message)s", le
-00001340: 7665 6c3d 6c6f 6767 696e 672e 494e 464f  vel=logging.INFO
-00001350: 2c20 6461 7465 666d 743d 2225 592d 256d  , datefmt="%Y-%m
-00001360: 2d25 6420 2548 3a25 4d3a 2553 220d 0a29  -%d %H:%M:%S"..)
-00001370: 0d0a 0d0a 7072 6574 7261 696e 6564 5f6d  ....pretrained_m
-00001380: 6f64 656c 5f64 6972 203d 2022 6661 6365  odel_dir = "face
-00001390: 626f 6f6b 2f6f 7074 2d31 3235 6d22 0d0a  book/opt-125m"..
-000013a0: 7175 616e 7469 7a65 645f 6d6f 6465 6c5f  quantized_model_
-000013b0: 6469 7220 3d20 226f 7074 2d31 3235 6d2d  dir = "opt-125m-
-000013c0: 3462 6974 220d 0a0d 0a74 6f6b 656e 697a  4bit"....tokeniz
-000013d0: 6572 203d 2041 7574 6f54 6f6b 656e 697a  er = AutoTokeniz
-000013e0: 6572 2e66 726f 6d5f 7072 6574 7261 696e  er.from_pretrain
-000013f0: 6564 2870 7265 7472 6169 6e65 645f 6d6f  ed(pretrained_mo
-00001400: 6465 6c5f 6469 722c 2075 7365 5f66 6173  del_dir, use_fas
-00001410: 743d 5472 7565 290d 0a65 7861 6d70 6c65  t=True)..example
-00001420: 7320 3d20 5b0d 0a20 2020 2074 6f6b 656e  s = [..    token
-00001430: 697a 6572 280d 0a20 2020 2020 2020 2022  izer(..        "
-00001440: 6175 746f 2d67 7074 7120 6973 2061 6e20  auto-gptq is an 
-00001450: 6561 7379 2d74 6f2d 7573 6520 6d6f 6465  easy-to-use mode
-00001460: 6c20 7175 616e 7469 7a61 7469 6f6e 206c  l quantization l
-00001470: 6962 7261 7279 2077 6974 6820 7573 6572  ibrary with user
-00001480: 2d66 7269 656e 646c 7920 6170 6973 2c20  -friendly apis, 
-00001490: 6261 7365 6420 6f6e 2047 5054 5120 616c  based on GPTQ al
-000014a0: 676f 7269 7468 6d2e 220d 0a20 2020 2029  gorithm."..    )
-000014b0: 0d0a 5d0d 0a0d 0a71 7561 6e74 697a 655f  ..]....quantize_
-000014c0: 636f 6e66 6967 203d 2042 6173 6551 7561  config = BaseQua
-000014d0: 6e74 697a 6543 6f6e 6669 6728 0d0a 2020  ntizeConfig(..  
-000014e0: 2020 6269 7473 3d34 2c20 2023 2071 7561    bits=4,  # qua
-000014f0: 6e74 697a 6520 6d6f 6465 6c20 746f 2034  ntize model to 4
-00001500: 2d62 6974 0d0a 2020 2020 6772 6f75 705f  -bit..    group_
-00001510: 7369 7a65 3d31 3238 2c20 2023 2069 7420  size=128,  # it 
-00001520: 6973 2072 6563 6f6d 6d65 6e64 6564 2074  is recommended t
-00001530: 6f20 7365 7420 7468 6520 7661 6c75 6520  o set the value 
-00001540: 746f 2031 3238 0d0a 2020 2020 6465 7363  to 128..    desc
-00001550: 5f61 6374 3d46 616c 7365 2c20 2023 2073  _act=False,  # s
-00001560: 6574 2074 6f20 4661 6c73 6520 6361 6e20  et to False can 
-00001570: 7369 676e 6966 6963 616e 746c 7920 7370  significantly sp
-00001580: 6565 6420 7570 2069 6e66 6572 656e 6365  eed up inference
-00001590: 2062 7574 2074 6865 2070 6572 706c 6578   but the perplex
-000015a0: 6974 7920 6d61 7920 736c 6967 6874 6c79  ity may slightly
-000015b0: 2062 6164 200d 0a29 0d0a 0d0a 2320 6c6f   bad ..)....# lo
-000015c0: 6164 2075 6e2d 7175 616e 7469 7a65 6420  ad un-quantized 
-000015d0: 6d6f 6465 6c2c 2062 7920 6465 6661 756c  model, by defaul
-000015e0: 742c 2074 6865 206d 6f64 656c 2077 696c  t, the model wil
-000015f0: 6c20 616c 7761 7973 2062 6520 6c6f 6164  l always be load
-00001600: 6564 2069 6e74 6f20 4350 5520 6d65 6d6f  ed into CPU memo
-00001610: 7279 0d0a 6d6f 6465 6c20 3d20 4175 746f  ry..model = Auto
-00001620: 4750 5451 466f 7243 6175 7361 6c4c 4d2e  GPTQForCausalLM.
-00001630: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
-00001640: 7072 6574 7261 696e 6564 5f6d 6f64 656c  pretrained_model
-00001650: 5f64 6972 2c20 7175 616e 7469 7a65 5f63  _dir, quantize_c
-00001660: 6f6e 6669 6729 0d0a 0d0a 2320 7175 616e  onfig)....# quan
-00001670: 7469 7a65 206d 6f64 656c 2c20 7468 6520  tize model, the 
-00001680: 6578 616d 706c 6573 2073 686f 756c 6420  examples should 
-00001690: 6265 206c 6973 7420 6f66 2064 6963 7420  be list of dict 
-000016a0: 7768 6f73 6520 6b65 7973 2063 616e 206f  whose keys can o
-000016b0: 6e6c 7920 6265 2022 696e 7075 745f 6964  nly be "input_id
-000016c0: 7322 2061 6e64 2022 6174 7465 6e74 696f  s" and "attentio
-000016d0: 6e5f 6d61 736b 220d 0a6d 6f64 656c 2e71  n_mask"..model.q
-000016e0: 7561 6e74 697a 6528 6578 616d 706c 6573  uantize(examples
-000016f0: 290d 0a0d 0a23 2073 6176 6520 7175 616e  )....# save quan
-00001700: 7469 7a65 6420 6d6f 6465 6c0d 0a6d 6f64  tized model..mod
-00001710: 656c 2e73 6176 655f 7175 616e 7469 7a65  el.save_quantize
-00001720: 6428 7175 616e 7469 7a65 645f 6d6f 6465  d(quantized_mode
-00001730: 6c5f 6469 7229 0d0a 0d0a 2320 7361 7665  l_dir)....# save
-00001740: 2071 7561 6e74 697a 6564 206d 6f64 656c   quantized model
-00001750: 2075 7369 6e67 2073 6166 6574 656e 736f   using safetenso
-00001760: 7273 0d0a 6d6f 6465 6c2e 7361 7665 5f71  rs..model.save_q
-00001770: 7561 6e74 697a 6564 2871 7561 6e74 697a  uantized(quantiz
-00001780: 6564 5f6d 6f64 656c 5f64 6972 2c20 7573  ed_model_dir, us
-00001790: 655f 7361 6665 7465 6e73 6f72 733d 5472  e_safetensors=Tr
-000017a0: 7565 290d 0a0d 0a23 2070 7573 6820 7175  ue)....# push qu
-000017b0: 616e 7469 7a65 6420 6d6f 6465 6c20 746f  antized model to
-000017c0: 2048 7567 6769 6e67 2046 6163 6520 4875   Hugging Face Hu
-000017d0: 622e 200d 0a23 2074 6f20 7573 6520 7573  b. ..# to use us
-000017e0: 655f 6175 7468 5f74 6f6b 656e 3d54 7275  e_auth_token=Tru
-000017f0: 652c 204c 6f67 696e 2066 6972 7374 2076  e, Login first v
-00001800: 6961 2068 7567 6769 6e67 6661 6365 2d63  ia huggingface-c
-00001810: 6c69 206c 6f67 696e 2e0d 0a23 206f 7220  li login...# or 
-00001820: 7061 7373 2065 7870 6c63 6974 2074 6f6b  pass explcit tok
-00001830: 656e 2077 6974 683a 2075 7365 5f61 7574  en with: use_aut
-00001840: 685f 746f 6b65 6e3d 2268 665f 7878 7878  h_token="hf_xxxx
-00001850: 7878 7822 0d0a 2320 2875 6e63 6f6d 6d65  xxx"..# (uncomme
-00001860: 6e74 2074 6865 2066 6f6c 6c6f 7769 6e67  nt the following
-00001870: 2074 6872 6565 206c 696e 6573 2074 6f20   three lines to 
-00001880: 656e 6162 6c65 2074 6869 7320 6665 6174  enable this feat
-00001890: 7572 6529 0d0a 2320 7265 706f 5f69 6420  ure)..# repo_id 
-000018a0: 3d20 6622 596f 7572 5573 6572 4e61 6d65  = f"YourUserName
-000018b0: 2f7b 7175 616e 7469 7a65 645f 6d6f 6465  /{quantized_mode
-000018c0: 6c5f 6469 727d 220d 0a23 2063 6f6d 6d69  l_dir}"..# commi
-000018d0: 745f 6d65 7373 6167 6520 3d20 6622 4175  t_message = f"Au
-000018e0: 746f 4750 5451 206d 6f64 656c 2066 6f72  toGPTQ model for
-000018f0: 207b 7072 6574 7261 696e 6564 5f6d 6f64   {pretrained_mod
-00001900: 656c 5f64 6972 7d3a 207b 7175 616e 7469  el_dir}: {quanti
-00001910: 7a65 5f63 6f6e 6669 672e 6269 7473 7d62  ze_config.bits}b
-00001920: 6974 732c 2067 727b 7175 616e 7469 7a65  its, gr{quantize
-00001930: 5f63 6f6e 6669 672e 6772 6f75 705f 7369  _config.group_si
-00001940: 7a65 7d2c 2064 6573 635f 6163 743d 7b71  ze}, desc_act={q
-00001950: 7561 6e74 697a 655f 636f 6e66 6967 2e64  uantize_config.d
-00001960: 6573 635f 6163 747d 220d 0a23 206d 6f64  esc_act}"..# mod
-00001970: 656c 2e70 7573 685f 746f 5f68 7562 2872  el.push_to_hub(r
-00001980: 6570 6f5f 6964 2c20 636f 6d6d 6974 5f6d  epo_id, commit_m
-00001990: 6573 7361 6765 3d63 6f6d 6d69 745f 6d65  essage=commit_me
-000019a0: 7373 6167 652c 2075 7365 5f61 7574 685f  ssage, use_auth_
-000019b0: 746f 6b65 6e3d 5472 7565 290d 0a0d 0a23  token=True)....#
-000019c0: 2061 6c74 6572 6e61 7469 7665 6c79 2079   alternatively y
-000019d0: 6f75 2063 616e 2073 6176 6520 616e 6420  ou can save and 
-000019e0: 7075 7368 2061 7420 7468 6520 7361 6d65  push at the same
-000019f0: 2074 696d 650d 0a23 2028 756e 636f 6d6d   time..# (uncomm
-00001a00: 656e 7420 7468 6520 666f 6c6c 6f77 696e  ent the followin
-00001a10: 6720 7468 7265 6520 6c69 6e65 7320 746f  g three lines to
-00001a20: 2065 6e61 626c 6520 7468 6973 2066 6561   enable this fea
-00001a30: 7475 7265 290d 0a23 2072 6570 6f5f 6964  ture)..# repo_id
-00001a40: 203d 2066 2259 6f75 7255 7365 724e 616d   = f"YourUserNam
-00001a50: 652f 7b71 7561 6e74 697a 6564 5f6d 6f64  e/{quantized_mod
-00001a60: 656c 5f64 6972 7d22 0d0a 2320 636f 6d6d  el_dir}"..# comm
-00001a70: 6974 5f6d 6573 7361 6765 203d 2066 2241  it_message = f"A
-00001a80: 7574 6f47 5054 5120 6d6f 6465 6c20 666f  utoGPTQ model fo
-00001a90: 7220 7b70 7265 7472 6169 6e65 645f 6d6f  r {pretrained_mo
-00001aa0: 6465 6c5f 6469 727d 3a20 7b71 7561 6e74  del_dir}: {quant
-00001ab0: 697a 655f 636f 6e66 6967 2e62 6974 737d  ize_config.bits}
-00001ac0: 6269 7473 2c20 6772 7b71 7561 6e74 697a  bits, gr{quantiz
-00001ad0: 655f 636f 6e66 6967 2e67 726f 7570 5f73  e_config.group_s
-00001ae0: 697a 657d 2c20 6465 7363 5f61 6374 3d7b  ize}, desc_act={
-00001af0: 7175 616e 7469 7a65 5f63 6f6e 6669 672e  quantize_config.
-00001b00: 6465 7363 5f61 6374 7d22 0d0a 2320 6d6f  desc_act}"..# mo
-00001b10: 6465 6c2e 7075 7368 5f74 6f5f 6875 6228  del.push_to_hub(
-00001b20: 7265 706f 5f69 642c 2073 6176 655f 6469  repo_id, save_di
-00001b30: 723d 7175 616e 7469 7a65 645f 6d6f 6465  r=quantized_mode
-00001b40: 6c5f 6469 722c 2075 7365 5f73 6166 6574  l_dir, use_safet
-00001b50: 656e 736f 7273 3d54 7275 652c 2063 6f6d  ensors=True, com
-00001b60: 6d69 745f 6d65 7373 6167 653d 636f 6d6d  mit_message=comm
-00001b70: 6974 5f6d 6573 7361 6765 2c20 7573 655f  it_message, use_
-00001b80: 6175 7468 5f74 6f6b 656e 3d54 7275 6529  auth_token=True)
-00001b90: 0d0a 0d0a 2320 6c6f 6164 2071 7561 6e74  ....# load quant
-00001ba0: 697a 6564 206d 6f64 656c 2074 6f20 7468  ized model to th
-00001bb0: 6520 6669 7273 7420 4750 550d 0a6d 6f64  e first GPU..mod
-00001bc0: 656c 203d 2041 7574 6f47 5054 5146 6f72  el = AutoGPTQFor
-00001bd0: 4361 7573 616c 4c4d 2e66 726f 6d5f 7175  CausalLM.from_qu
-00001be0: 616e 7469 7a65 6428 7175 616e 7469 7a65  antized(quantize
-00001bf0: 645f 6d6f 6465 6c5f 6469 722c 2064 6576  d_model_dir, dev
-00001c00: 6963 653d 2263 7564 613a 3022 290d 0a0d  ice="cuda:0")...
-00001c10: 0a23 2064 6f77 6e6c 6f61 6420 7175 616e  .# download quan
-00001c20: 7469 7a65 6420 6d6f 6465 6c20 6672 6f6d  tized model from
-00001c30: 2048 7567 6769 6e67 2046 6163 6520 4875   Hugging Face Hu
-00001c40: 6220 616e 6420 6c6f 6164 2074 6f20 7468  b and load to th
-00001c50: 6520 6669 7273 7420 4750 550d 0a23 206d  e first GPU..# m
-00001c60: 6f64 656c 203d 2041 7574 6f47 5054 5146  odel = AutoGPTQF
-00001c70: 6f72 4361 7573 616c 4c4d 2e66 726f 6d5f  orCausalLM.from_
-00001c80: 7175 616e 7469 7a65 6428 7265 706f 5f69  quantized(repo_i
-00001c90: 642c 2064 6576 6963 653d 2263 7564 613a  d, device="cuda:
-00001ca0: 3022 2c20 7573 655f 7361 6665 7465 6e73  0", use_safetens
-00001cb0: 6f72 733d 5472 7565 2c20 7573 655f 7472  ors=True, use_tr
-00001cc0: 6974 6f6e 3d46 616c 7365 290d 0a0d 0a23  iton=False)....#
-00001cd0: 2069 6e66 6572 656e 6365 2077 6974 6820   inference with 
-00001ce0: 6d6f 6465 6c2e 6765 6e65 7261 7465 0d0a  model.generate..
-00001cf0: 7072 696e 7428 746f 6b65 6e69 7a65 722e  print(tokenizer.
-00001d00: 6465 636f 6465 286d 6f64 656c 2e67 656e  decode(model.gen
-00001d10: 6572 6174 6528 2a2a 746f 6b65 6e69 7a65  erate(**tokenize
-00001d20: 7228 2261 7574 6f5f 6770 7471 2069 7322  r("auto_gptq is"
-00001d30: 2c20 7265 7475 726e 5f74 656e 736f 7273  , return_tensors
-00001d40: 3d22 7074 2229 2e74 6f28 6d6f 6465 6c2e  ="pt").to(model.
-00001d50: 6465 7669 6365 2929 5b30 5d29 290d 0a0d  device))[0]))...
-00001d60: 0a23 206f 7220 796f 7520 6361 6e20 616c  .# or you can al
-00001d70: 736f 2075 7365 2070 6970 656c 696e 650d  so use pipeline.
-00001d80: 0a70 6970 656c 696e 6520 3d20 5465 7874  .pipeline = Text
-00001d90: 4765 6e65 7261 7469 6f6e 5069 7065 6c69  GenerationPipeli
-00001da0: 6e65 286d 6f64 656c 3d6d 6f64 656c 2c20  ne(model=model, 
-00001db0: 746f 6b65 6e69 7a65 723d 746f 6b65 6e69  tokenizer=tokeni
-00001dc0: 7a65 7229 0d0a 7072 696e 7428 7069 7065  zer)..print(pipe
-00001dd0: 6c69 6e65 2822 6175 746f 2d67 7074 7120  line("auto-gptq 
-00001de0: 6973 2229 5b30 5d5b 2267 656e 6572 6174  is")[0]["generat
-00001df0: 6564 5f74 6578 7422 5d29 0d0a 6060 600d  ed_text"])..```.
-00001e00: 0a0d 0a46 6f72 206d 6f72 6520 6164 7661  ...For more adva
-00001e10: 6e63 6564 2066 6561 7475 7265 7320 6f66  nced features of
-00001e20: 206d 6f64 656c 2071 7561 6e74 697a 6174   model quantizat
-00001e30: 696f 6e2c 2070 6c65 6173 6520 7265 6665  ion, please refe
-00001e40: 7265 6e63 6520 746f 205b 7468 6973 2073  rence to [this s
-00001e50: 6372 6970 745d 2865 7861 6d70 6c65 732f  cript](examples/
-00001e60: 7175 616e 7469 7a61 7469 6f6e 2f71 7561  quantization/qua
-00001e70: 6e74 5f77 6974 685f 616c 7061 6361 2e70  nt_with_alpaca.p
-00001e80: 7929 0d0a 0d0a 2323 2320 4375 7374 6f6d  y)....### Custom
-00001e90: 697a 6520 4d6f 6465 6c0d 0a3c 6465 7461  ize Model..<deta
-00001ea0: 696c 733e 0d0a 0d0a 3c73 756d 6d61 7279  ils>....<summary
-00001eb0: 3e42 656c 6f77 2069 7320 616e 2065 7861  >Below is an exa
-00001ec0: 6d70 6c65 2074 6f20 6578 7465 6e64 2060  mple to extend `
-00001ed0: 6175 746f 5f67 7074 7160 2074 6f20 7375  auto_gptq` to su
-00001ee0: 7070 6f72 7420 604f 5054 6020 6d6f 6465  pport `OPT` mode
-00001ef0: 6c2c 2061 7320 796f 7520 7769 6c6c 2073  l, as you will s
-00001f00: 6565 2c20 6974 2773 2076 6572 7920 6561  ee, it's very ea
-00001f10: 7379 3a3c 2f73 756d 6d61 7279 3e0d 0a0d  sy:</summary>...
-00001f20: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
-00001f30: 2061 7574 6f5f 6770 7471 2e6d 6f64 656c   auto_gptq.model
-00001f40: 696e 6720 696d 706f 7274 2042 6173 6547  ing import BaseG
-00001f50: 5054 5146 6f72 4361 7573 616c 4c4d 0d0a  PTQForCausalLM..
-00001f60: 0d0a 0d0a 636c 6173 7320 4f50 5447 5054  ....class OPTGPT
-00001f70: 5146 6f72 4361 7573 616c 4c4d 2842 6173  QForCausalLM(Bas
-00001f80: 6547 5054 5146 6f72 4361 7573 616c 4c4d  eGPTQForCausalLM
-00001f90: 293a 0d0a 2020 2020 2320 6368 6169 6e65  ):..    # chaine
-00001fa0: 6420 6174 7472 6962 7574 6520 6e61 6d65  d attribute name
-00001fb0: 206f 6620 7472 616e 7366 6f72 6d65 7220   of transformer 
-00001fc0: 6c61 7965 7220 626c 6f63 6b0d 0a20 2020  layer block..   
-00001fd0: 206c 6179 6572 735f 626c 6f63 6b5f 6e61   layers_block_na
-00001fe0: 6d65 203d 2022 6d6f 6465 6c2e 6465 636f  me = "model.deco
-00001ff0: 6465 722e 6c61 7965 7273 220d 0a20 2020  der.layers"..   
-00002000: 2023 2063 6861 696e 6564 2061 7474 7269   # chained attri
-00002010: 6275 7465 206e 616d 6573 206f 6620 6f74  bute names of ot
-00002020: 6865 7220 6e6e 206d 6f64 756c 6573 2074  her nn modules t
-00002030: 6861 7420 696e 2074 6865 2073 616d 6520  hat in the same 
-00002040: 6c65 7665 6c20 6173 2074 6865 2074 7261  level as the tra
-00002050: 6e73 666f 726d 6572 206c 6179 6572 2062  nsformer layer b
-00002060: 6c6f 636b 0d0a 2020 2020 6f75 7473 6964  lock..    outsid
-00002070: 655f 6c61 7965 725f 6d6f 6475 6c65 7320  e_layer_modules 
-00002080: 3d20 5b0d 0a20 2020 2020 2020 2022 6d6f  = [..        "mo
-00002090: 6465 6c2e 6465 636f 6465 722e 656d 6265  del.decoder.embe
-000020a0: 645f 746f 6b65 6e73 222c 2022 6d6f 6465  d_tokens", "mode
-000020b0: 6c2e 6465 636f 6465 722e 656d 6265 645f  l.decoder.embed_
-000020c0: 706f 7369 7469 6f6e 7322 2c20 226d 6f64  positions", "mod
-000020d0: 656c 2e64 6563 6f64 6572 2e70 726f 6a65  el.decoder.proje
-000020e0: 6374 5f6f 7574 222c 0d0a 2020 2020 2020  ct_out",..      
-000020f0: 2020 226d 6f64 656c 2e64 6563 6f64 6572    "model.decoder
-00002100: 2e70 726f 6a65 6374 5f69 6e22 2c20 226d  .project_in", "m
-00002110: 6f64 656c 2e64 6563 6f64 6572 2e66 696e  odel.decoder.fin
-00002120: 616c 5f6c 6179 6572 5f6e 6f72 6d22 0d0a  al_layer_norm"..
-00002130: 2020 2020 5d0d 0a20 2020 2023 2063 6861      ]..    # cha
-00002140: 696e 6564 2061 7474 7269 6275 7465 206e  ined attribute n
-00002150: 616d 6573 206f 6620 6c69 6e65 6172 206c  ames of linear l
-00002160: 6179 6572 7320 696e 2074 7261 6e73 666f  ayers in transfo
-00002170: 726d 6572 206c 6179 6572 206d 6f64 756c  rmer layer modul
-00002180: 650d 0a20 2020 2023 206e 6f72 6d61 6c6c  e..    # normall
-00002190: 792c 2074 6865 7265 2061 7265 2066 6f75  y, there are fou
-000021a0: 7220 7375 6220 6c69 7374 732c 2066 6f72  r sub lists, for
-000021b0: 2065 6163 6820 6f6e 6520 7468 6520 6d6f   each one the mo
-000021c0: 6475 6c65 7320 696e 2069 7420 6361 6e20  dules in it can 
-000021d0: 6265 2073 6565 6e20 6173 206f 6e65 206f  be seen as one o
-000021e0: 7065 7261 7469 6f6e 2c20 0d0a 2020 2020  peration, ..    
-000021f0: 2320 616e 6420 7468 6520 6f72 6465 7220  # and the order 
-00002200: 7368 6f75 6c64 2062 6520 7468 6520 6f72  should be the or
-00002210: 6465 7220 7768 656e 2074 6865 7920 6172  der when they ar
-00002220: 6520 7472 756c 7920 6578 6563 7574 6564  e truly executed
-00002230: 2c20 696e 2074 6869 7320 6361 7365 2028  , in this case (
-00002240: 616e 6420 7573 7561 6c6c 7920 696e 206d  and usually in m
-00002250: 6f73 7420 6361 7365 7329 2c20 0d0a 2020  ost cases), ..  
-00002260: 2020 2320 7468 6579 2061 7265 3a20 6174    # they are: at
-00002270: 7465 6e74 696f 6e20 715f 6b5f 7620 7072  tention q_k_v pr
-00002280: 6f6a 6563 7469 6f6e 2c20 6174 7465 6e74  ojection, attent
-00002290: 696f 6e20 6f75 7470 7574 2070 726f 6a65  ion output proje
-000022a0: 6374 696f 6e2c 204d 4c50 2070 726f 6a65  ction, MLP proje
-000022b0: 6374 2069 6e70 7574 2c20 4d4c 5020 7072  ct input, MLP pr
-000022c0: 6f6a 6563 7420 6f75 7470 7574 0d0a 2020  oject output..  
-000022d0: 2020 696e 7369 6465 5f6c 6179 6572 5f6d    inside_layer_m
-000022e0: 6f64 756c 6573 203d 205b 0d0a 2020 2020  odules = [..    
-000022f0: 2020 2020 5b22 7365 6c66 5f61 7474 6e2e      ["self_attn.
-00002300: 6b5f 7072 6f6a 222c 2022 7365 6c66 5f61  k_proj", "self_a
-00002310: 7474 6e2e 765f 7072 6f6a 222c 2022 7365  ttn.v_proj", "se
-00002320: 6c66 5f61 7474 6e2e 715f 7072 6f6a 225d  lf_attn.q_proj"]
-00002330: 2c0d 0a20 2020 2020 2020 205b 2273 656c  ,..        ["sel
-00002340: 665f 6174 746e 2e6f 7574 5f70 726f 6a22  f_attn.out_proj"
-00002350: 5d2c 0d0a 2020 2020 2020 2020 5b22 6663  ],..        ["fc
-00002360: 3122 5d2c 0d0a 2020 2020 2020 2020 5b22  1"],..        ["
-00002370: 6663 3222 5d0d 0a20 2020 205d 0d0a 6060  fc2"]..    ]..``
-00002380: 600d 0a41 6674 6572 2074 6869 732c 2079  `..After this, y
-00002390: 6f75 2063 616e 2075 7365 2060 4f50 5447  ou can use `OPTG
-000023a0: 5054 5146 6f72 4361 7573 616c 4c4d 2e66  PTQForCausalLM.f
-000023b0: 726f 6d5f 7072 6574 7261 696e 6564 6020  rom_pretrained` 
-000023c0: 616e 6420 6f74 6865 7220 6d65 7468 6f64  and other method
-000023d0: 7320 6173 2073 686f 776e 2069 6e20 4261  s as shown in Ba
-000023e0: 7369 632e 0d0a 0d0a 3c2f 6465 7461 696c  sic.....</detail
-000023f0: 733e 0d0a 0d0a 2323 2320 4576 616c 7561  s>....### Evalua
-00002400: 7469 6f6e 206f 6e20 446f 776e 7374 7265  tion on Downstre
-00002410: 616d 2054 6173 6b73 0d0a 596f 7520 6361  am Tasks..You ca
-00002420: 6e20 7573 6520 7461 736b 7320 6465 6669  n use tasks defi
-00002430: 6e65 6420 696e 2060 6175 746f 5f67 7074  ned in `auto_gpt
-00002440: 712e 6576 616c 5f74 6173 6b73 6020 746f  q.eval_tasks` to
-00002450: 2065 7661 6c75 6174 6520 6d6f 6465 6c27   evaluate model'
-00002460: 7320 7065 7266 6f72 6d61 6e63 6520 6f6e  s performance on
-00002470: 2073 7065 6369 6669 6320 646f 776e 2d73   specific down-s
-00002480: 7472 6561 6d20 7461 736b 2062 6566 6f72  tream task befor
-00002490: 6520 616e 6420 6166 7465 7220 7175 616e  e and after quan
-000024a0: 7469 7a61 7469 6f6e 2e0d 0a0d 0a54 6865  tization.....The
-000024b0: 2070 7265 6465 6669 6e65 6420 7461 736b   predefined task
-000024c0: 7320 7375 7070 6f72 7420 616c 6c20 6361  s support all ca
-000024d0: 7573 616c 2d6c 616e 6775 6167 652d 6d6f  usal-language-mo
-000024e0: 6465 6c73 2069 6d70 6c65 6d65 6e74 6564  dels implemented
-000024f0: 2069 6e20 5bf0 9fa4 9720 7472 616e 7366   in [.... transf
-00002500: 6f72 6d65 7273 5d28 6874 7470 733a 2f2f  ormers](https://
-00002510: 6769 7468 7562 2e63 6f6d 2f68 7567 6769  github.com/huggi
-00002520: 6e67 6661 6365 2f74 7261 6e73 666f 726d  ngface/transform
-00002530: 6572 7329 2061 6e64 2069 6e20 7468 6973  ers) and in this
-00002540: 2070 726f 6a65 6374 2e0d 0a0d 0a3c 6465   project.....<de
-00002550: 7461 696c 733e 0d0a 0d0a 3c73 756d 6d61  tails>....<summa
-00002560: 7279 3e42 656c 6f77 2069 7320 616e 2065  ry>Below is an e
-00002570: 7861 6d70 6c65 2074 6f20 6576 616c 7561  xample to evalua
-00002580: 7465 2060 456c 6575 7468 6572 4149 2f67  te `EleutherAI/g
-00002590: 7074 2d6a 2d36 6260 206f 6e20 7365 7175  pt-j-6b` on sequ
-000025a0: 656e 6365 2d63 6c61 7373 6966 6963 6174  ence-classificat
-000025b0: 696f 6e20 7461 736b 2075 7369 6e67 2060  ion task using `
-000025c0: 6361 7264 6966 666e 6c70 2f74 7765 6574  cardiffnlp/tweet
-000025d0: 5f73 656e 7469 6d65 6e74 5f6d 756c 7469  _sentiment_multi
-000025e0: 6c69 6e67 7561 6c60 2064 6174 6173 6574  lingual` dataset
-000025f0: 3a3c 2f73 756d 6d61 7279 3e0d 0a0d 0a60  :</summary>....`
-00002600: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2066  ``python..from f
-00002610: 756e 6374 6f6f 6c73 2069 6d70 6f72 7420  unctools import 
-00002620: 7061 7274 6961 6c0d 0a0d 0a69 6d70 6f72  partial....impor
-00002630: 7420 6461 7461 7365 7473 0d0a 6672 6f6d  t datasets..from
-00002640: 2074 7261 6e73 666f 726d 6572 7320 696d   transformers im
-00002650: 706f 7274 2041 7574 6f54 6f6b 656e 697a  port AutoTokeniz
-00002660: 6572 2c20 4175 746f 4d6f 6465 6c46 6f72  er, AutoModelFor
-00002670: 4361 7573 616c 4c4d 2c20 4765 6e65 7261  CausalLM, Genera
-00002680: 7469 6f6e 436f 6e66 6967 0d0a 0d0a 6672  tionConfig....fr
-00002690: 6f6d 2061 7574 6f5f 6770 7471 2069 6d70  om auto_gptq imp
-000026a0: 6f72 7420 4175 746f 4750 5451 466f 7243  ort AutoGPTQForC
-000026b0: 6175 7361 6c4c 4d2c 2042 6173 6551 7561  ausalLM, BaseQua
-000026c0: 6e74 697a 6543 6f6e 6669 670d 0a66 726f  ntizeConfig..fro
-000026d0: 6d20 6175 746f 5f67 7074 712e 6576 616c  m auto_gptq.eval
-000026e0: 5f74 6173 6b73 2069 6d70 6f72 7420 5365  _tasks import Se
-000026f0: 7175 656e 6365 436c 6173 7369 6669 6361  quenceClassifica
-00002700: 7469 6f6e 5461 736b 0d0a 0d0a 0d0a 4d4f  tionTask......MO
-00002710: 4445 4c20 3d20 2245 6c65 7574 6865 7241  DEL = "EleutherA
-00002720: 492f 6770 742d 6a2d 3662 220d 0a44 4154  I/gpt-j-6b"..DAT
-00002730: 4153 4554 203d 2022 6361 7264 6966 666e  ASET = "cardiffn
-00002740: 6c70 2f74 7765 6574 5f73 656e 7469 6d65  lp/tweet_sentime
-00002750: 6e74 5f6d 756c 7469 6c69 6e67 7561 6c22  nt_multilingual"
-00002760: 0d0a 5445 4d50 4c41 5445 203d 2022 5175  ..TEMPLATE = "Qu
-00002770: 6573 7469 6f6e 3a57 6861 7427 7320 7468  estion:What's th
-00002780: 6520 7365 6e74 696d 656e 7420 6f66 2074  e sentiment of t
-00002790: 6865 2067 6976 656e 2074 6578 743f 2043  he given text? C
-000027a0: 686f 6963 6573 2061 7265 207b 6c61 6265  hoices are {labe
-000027b0: 6c73 7d2e 5c6e 5465 7874 3a20 7b74 6578  ls}.\nText: {tex
-000027c0: 747d 5c6e 416e 7377 6572 3a22 0d0a 4944  t}\nAnswer:"..ID
-000027d0: 324c 4142 454c 203d 207b 0d0a 2020 2020  2LABEL = {..    
-000027e0: 303a 2022 6e65 6761 7469 7665 222c 0d0a  0: "negative",..
-000027f0: 2020 2020 313a 2022 6e65 7574 7261 6c22      1: "neutral"
-00002800: 2c0d 0a20 2020 2032 3a20 2270 6f73 6974  ,..    2: "posit
-00002810: 6976 6522 0d0a 7d0d 0a4c 4142 454c 5320  ive"..}..LABELS 
-00002820: 3d20 6c69 7374 2849 4432 4c41 4245 4c2e  = list(ID2LABEL.
-00002830: 7661 6c75 6573 2829 290d 0a0d 0a0d 0a64  values())......d
-00002840: 6566 2064 735f 7265 6661 6374 6f72 5f66  ef ds_refactor_f
-00002850: 6e28 7361 6d70 6c65 7329 3a0d 0a20 2020  n(samples):..   
-00002860: 2074 6578 745f 6461 7461 203d 2073 616d   text_data = sam
-00002870: 706c 6573 5b22 7465 7874 225d 0d0a 2020  ples["text"]..  
-00002880: 2020 6c61 6265 6c5f 6461 7461 203d 2073    label_data = s
-00002890: 616d 706c 6573 5b22 6c61 6265 6c22 5d0d  amples["label"].
-000028a0: 0a0d 0a20 2020 206e 6577 5f73 616d 706c  ...    new_sampl
-000028b0: 6573 203d 207b 2270 726f 6d70 7422 3a20  es = {"prompt": 
-000028c0: 5b5d 2c20 226c 6162 656c 223a 205b 5d7d  [], "label": []}
-000028d0: 0d0a 2020 2020 666f 7220 7465 7874 2c20  ..    for text, 
-000028e0: 6c61 6265 6c20 696e 207a 6970 2874 6578  label in zip(tex
-000028f0: 745f 6461 7461 2c20 6c61 6265 6c5f 6461  t_data, label_da
-00002900: 7461 293a 0d0a 2020 2020 2020 2020 7072  ta):..        pr
-00002910: 6f6d 7074 203d 2054 454d 504c 4154 452e  ompt = TEMPLATE.
-00002920: 666f 726d 6174 286c 6162 656c 733d 4c41  format(labels=LA
-00002930: 4245 4c53 2c20 7465 7874 3d74 6578 7429  BELS, text=text)
-00002940: 0d0a 2020 2020 2020 2020 6e65 775f 7361  ..        new_sa
-00002950: 6d70 6c65 735b 2270 726f 6d70 7422 5d2e  mples["prompt"].
-00002960: 6170 7065 6e64 2870 726f 6d70 7429 0d0a  append(prompt)..
-00002970: 2020 2020 2020 2020 6e65 775f 7361 6d70          new_samp
-00002980: 6c65 735b 226c 6162 656c 225d 2e61 7070  les["label"].app
-00002990: 656e 6428 4944 324c 4142 454c 5b6c 6162  end(ID2LABEL[lab
-000029a0: 656c 5d29 0d0a 0d0a 2020 2020 7265 7475  el])....    retu
-000029b0: 726e 206e 6577 5f73 616d 706c 6573 0d0a  rn new_samples..
-000029c0: 0d0a 0d0a 2320 206d 6f64 656c 203d 2041  ....#  model = A
-000029d0: 7574 6f4d 6f64 656c 466f 7243 6175 7361  utoModelForCausa
-000029e0: 6c4c 4d2e 6672 6f6d 5f70 7265 7472 6169  lLM.from_pretrai
-000029f0: 6e65 6428 4d4f 4445 4c29 2e65 7661 6c28  ned(MODEL).eval(
-00002a00: 292e 6861 6c66 2829 2e74 6f28 2263 7564  ).half().to("cud
-00002a10: 613a 3022 290d 0a6d 6f64 656c 203d 2041  a:0")..model = A
-00002a20: 7574 6f47 5054 5146 6f72 4361 7573 616c  utoGPTQForCausal
-00002a30: 4c4d 2e66 726f 6d5f 7072 6574 7261 696e  LM.from_pretrain
-00002a40: 6564 284d 4f44 454c 2c20 4261 7365 5175  ed(MODEL, BaseQu
-00002a50: 616e 7469 7a65 436f 6e66 6967 2829 290d  antizeConfig()).
-00002a60: 0a74 6f6b 656e 697a 6572 203d 2041 7574  .tokenizer = Aut
-00002a70: 6f54 6f6b 656e 697a 6572 2e66 726f 6d5f  oTokenizer.from_
-00002a80: 7072 6574 7261 696e 6564 284d 4f44 454c  pretrained(MODEL
-00002a90: 290d 0a0d 0a74 6173 6b20 3d20 5365 7175  )....task = Sequ
-00002aa0: 656e 6365 436c 6173 7369 6669 6361 7469  enceClassificati
-00002ab0: 6f6e 5461 736b 280d 0a20 2020 2020 2020  onTask(..       
-00002ac0: 206d 6f64 656c 3d6d 6f64 656c 2c0d 0a20   model=model,.. 
-00002ad0: 2020 2020 2020 2074 6f6b 656e 697a 6572         tokenizer
-00002ae0: 3d74 6f6b 656e 697a 6572 2c0d 0a20 2020  =tokenizer,..   
-00002af0: 2020 2020 2063 6c61 7373 6573 3d4c 4142       classes=LAB
-00002b00: 454c 532c 0d0a 2020 2020 2020 2020 6461  ELS,..        da
-00002b10: 7461 5f6e 616d 655f 6f72 5f70 6174 683d  ta_name_or_path=
-00002b20: 4441 5441 5345 542c 0d0a 2020 2020 2020  DATASET,..      
-00002b30: 2020 7072 6f6d 7074 5f63 6f6c 5f6e 616d    prompt_col_nam
-00002b40: 653d 2270 726f 6d70 7422 2c0d 0a20 2020  e="prompt",..   
-00002b50: 2020 2020 206c 6162 656c 5f63 6f6c 5f6e       label_col_n
-00002b60: 616d 653d 226c 6162 656c 222c 0d0a 2020  ame="label",..  
-00002b70: 2020 2020 2020 2a2a 7b0d 0a20 2020 2020        **{..     
-00002b80: 2020 2020 2020 2022 6e75 6d5f 7361 6d70         "num_samp
-00002b90: 6c65 7322 3a20 3130 3030 2c20 2023 2068  les": 1000,  # h
-00002ba0: 6f77 206d 616e 7920 7361 6d70 6c65 7320  ow many samples 
-00002bb0: 7769 6c6c 2062 6520 7361 6d70 6c65 6420  will be sampled 
-00002bc0: 746f 2065 7661 6c75 6174 696f 6e0d 0a20  to evaluation.. 
-00002bd0: 2020 2020 2020 2020 2020 2022 7361 6d70             "samp
-00002be0: 6c65 5f6d 6178 5f6c 656e 223a 2031 3032  le_max_len": 102
-00002bf0: 342c 2020 2320 6d61 7820 746f 6b65 6e73  4,  # max tokens
-00002c00: 2066 6f72 2065 6163 6820 7361 6d70 6c65   for each sample
-00002c10: 0d0a 2020 2020 2020 2020 2020 2020 2262  ..            "b
-00002c20: 6c6f 636b 5f6d 6178 5f6c 656e 223a 2032  lock_max_len": 2
-00002c30: 3034 382c 2020 2320 6d61 7820 746f 6b65  048,  # max toke
-00002c40: 6e73 2066 6f72 2065 6163 6820 6461 7461  ns for each data
-00002c50: 2062 6c6f 636b 0d0a 2020 2020 2020 2020   block..        
-00002c60: 2020 2020 2320 6675 6e63 7469 6f6e 2074      # function t
-00002c70: 6f20 6c6f 6164 2064 6174 6173 6574 2c20  o load dataset, 
-00002c80: 6f6e 6520 6d75 7374 206f 6e6c 7920 6163  one must only ac
-00002c90: 6365 7074 2064 6174 615f 6e61 6d65 5f6f  cept data_name_o
-00002ca0: 725f 7061 7468 2061 7320 696e 7075 7420  r_path as input 
-00002cb0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00002cc0: 616e 6420 7265 7475 726e 2064 6174 6173  and return datas
-00002cd0: 6574 732e 4461 7461 7365 740d 0a20 2020  ets.Dataset..   
-00002ce0: 2020 2020 2020 2020 2022 6c6f 6164 5f66           "load_f
-00002cf0: 6e22 3a20 7061 7274 6961 6c28 6461 7461  n": partial(data
-00002d00: 7365 7473 2e6c 6f61 645f 6461 7461 7365  sets.load_datase
-00002d10: 742c 206e 616d 653d 2265 6e67 6c69 7368  t, name="english
-00002d20: 2229 2c20 200d 0a20 2020 2020 2020 2020  "),  ..         
-00002d30: 2020 2023 2066 756e 6374 696f 6e20 746f     # function to
-00002d40: 2070 7265 7072 6f63 6573 7320 6461 7461   preprocess data
-00002d50: 7365 742c 2077 6869 6368 2069 7320 7573  set, which is us
-00002d60: 6564 2066 6f72 2064 6174 6173 6574 732e  ed for datasets.
-00002d70: 4461 7461 7365 742e 6d61 702c 200d 0a20  Dataset.map, .. 
-00002d80: 2020 2020 2020 2020 2020 2023 206d 7573             # mus
-00002d90: 7420 7265 7475 726e 2044 6963 745b 7374  t return Dict[st
-00002da0: 722c 206c 6973 745d 2077 6974 6820 6f6e  r, list] with on
-00002db0: 6c79 2074 776f 206b 6579 733a 205b 7072  ly two keys: [pr
-00002dc0: 6f6d 7074 5f63 6f6c 5f6e 616d 652c 206c  ompt_col_name, l
-00002dd0: 6162 656c 5f63 6f6c 5f6e 616d 655d 0d0a  abel_col_name]..
-00002de0: 2020 2020 2020 2020 2020 2020 2270 7265              "pre
-00002df0: 7072 6f63 6573 735f 666e 223a 2064 735f  process_fn": ds_
-00002e00: 7265 6661 6374 6f72 5f66 6e2c 2020 0d0a  refactor_fn,  ..
-00002e10: 2020 2020 2020 2020 2020 2020 2320 7472              # tr
-00002e20: 756e 6361 7465 206c 6162 656c 2077 6865  uncate label whe
-00002e30: 6e20 7361 6d70 6c65 2773 206c 656e 6774  n sample's lengt
-00002e40: 6820 6578 6365 6564 2073 616d 706c 655f  h exceed sample_
-00002e50: 6d61 785f 6c65 6e0d 0a20 2020 2020 2020  max_len..       
-00002e60: 2020 2020 2022 7472 756e 6361 7465 5f70       "truncate_p
-00002e70: 726f 6d70 7422 3a20 4661 6c73 6520 200d  rompt": False  .
-00002e80: 0a20 2020 2020 2020 207d 0d0a 2020 2020  .        }..    
-00002e90: 290d 0a0d 0a23 206e 6f74 6520 7468 6174  )....# note that
-00002ea0: 206d 6178 5f6e 6577 5f74 6f6b 656e 7320   max_new_tokens 
-00002eb0: 7769 6c6c 2062 6520 6175 746f 6d61 7469  will be automati
-00002ec0: 6361 6c6c 7920 7370 6563 6966 6965 6420  cally specified 
-00002ed0: 696e 7465 726e 616c 6c79 2062 6173 6564  internally based
-00002ee0: 206f 6e20 6769 7665 6e20 636c 6173 7365   on given classe
-00002ef0: 730d 0a70 7269 6e74 2874 6173 6b2e 7275  s..print(task.ru
-00002f00: 6e28 2929 0d0a 0d0a 2320 7365 6c66 2d63  n())....# self-c
-00002f10: 6f6e 7369 7374 656e 6379 0d0a 7072 696e  onsistency..prin
-00002f20: 7428 0d0a 2020 2020 7461 736b 2e72 756e  t(..    task.run
-00002f30: 280d 0a20 2020 2020 2020 2067 656e 6572  (..        gener
-00002f40: 6174 696f 6e5f 636f 6e66 6967 3d47 656e  ation_config=Gen
-00002f50: 6572 6174 696f 6e43 6f6e 6669 6728 0d0a  erationConfig(..
-00002f60: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
-00002f70: 6265 616d 733d 332c 0d0a 2020 2020 2020  beams=3,..      
-00002f80: 2020 2020 2020 6e75 6d5f 7265 7475 726e        num_return
-00002f90: 5f73 6571 7565 6e63 6573 3d33 2c0d 0a20  _sequences=3,.. 
-00002fa0: 2020 2020 2020 2020 2020 2064 6f5f 7361             do_sa
-00002fb0: 6d70 6c65 3d54 7275 650d 0a20 2020 2020  mple=True..     
-00002fc0: 2020 2029 0d0a 2020 2020 290d 0a29 0d0a     )..    )..)..
-00002fd0: 6060 600d 0a0d 0a3c 2f64 6574 6169 6c73  ```....</details
-00002fe0: 3e0d 0a0d 0a23 2320 4c65 6172 6e20 4d6f  >....## Learn Mo
-00002ff0: 7265 0d0a 5b74 7574 6f72 6961 6c73 5d28  re..[tutorials](
-00003000: 646f 6373 2f74 7574 6f72 6961 6c29 2070  docs/tutorial) p
-00003010: 726f 7669 6465 2073 7465 702d 6279 2d73  rovide step-by-s
-00003020: 7465 7020 6775 6964 616e 6365 2074 6f20  tep guidance to 
-00003030: 696e 7465 6772 6174 6520 6061 7574 6f5f  integrate `auto_
-00003040: 6770 7471 6020 7769 7468 2079 6f75 7220  gptq` with your 
-00003050: 6f77 6e20 7072 6f6a 6563 7420 616e 6420  own project and 
-00003060: 736f 6d65 2062 6573 7420 7072 6163 7469  some best practi
-00003070: 6365 2070 7269 6e63 6970 6c65 732e 0d0a  ce principles...
-00003080: 0d0a 5b65 7861 6d70 6c65 735d 2865 7861  ..[examples](exa
-00003090: 6d70 6c65 732f 5245 4144 4d45 2e6d 6429  mples/README.md)
-000030a0: 2070 726f 7669 6465 2070 6c65 6e74 7920   provide plenty 
-000030b0: 6f66 2065 7861 6d70 6c65 2073 6372 6970  of example scrip
-000030c0: 7473 2074 6f20 7573 6520 6061 7574 6f5f  ts to use `auto_
-000030d0: 6770 7471 6020 696e 2064 6966 6665 7265  gptq` in differe
-000030e0: 6e74 2077 6179 732e 0d0a 0d0a 2323 2053  nt ways.....## S
-000030f0: 7570 706f 7274 6564 204d 6f64 656c 730d  upported Models.
-00003100: 0a0d 0a3e 2079 6f75 2063 616e 2075 7365  ...> you can use
-00003110: 2060 6d6f 6465 6c2e 636f 6e66 6967 2e6d   `model.config.m
-00003120: 6f64 656c 5f74 7970 6560 2074 6f20 636f  odel_type` to co
-00003130: 6d70 6172 6520 7769 7468 2074 6865 2074  mpare with the t
-00003140: 6162 6c65 2062 656c 6f77 2074 6f20 6368  able below to ch
-00003150: 6563 6b20 7768 6574 6865 7220 7468 6520  eck whether the 
-00003160: 6d6f 6465 6c20 796f 7520 7573 6520 6973  model you use is
-00003170: 2073 7570 706f 7274 6564 2062 7920 6061   supported by `a
-00003180: 7574 6f5f 6770 7471 602e 0d0a 3e20 0d0a  uto_gptq`...> ..
-00003190: 3e20 666f 7220 6578 616d 706c 652c 206d  > for example, m
-000031a0: 6f64 656c 5f74 7970 6520 6f66 2060 5769  odel_type of `Wi
-000031b0: 7a61 7264 4c4d 602c 2060 7669 6375 6e61  zardLM`, `vicuna
-000031c0: 6020 616e 6420 6067 7074 3461 6c6c 6020  ` and `gpt4all` 
-000031d0: 6172 6520 616c 6c20 606c 6c61 6d61 602c  are all `llama`,
-000031e0: 2068 656e 6365 2074 6865 7920 6172 6520   hence they are 
-000031f0: 616c 6c20 7375 7070 6f72 7465 6420 6279  all supported by
-00003200: 2060 6175 746f 5f67 7074 7160 2e0d 0a0d   `auto_gptq`....
-00003210: 0a7c 206d 6f64 656c 2074 7970 6520 2020  .| model type   
+00000020: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000030: 7222 3e41 6e20 6561 7379 2d74 6f2d 7573  r">An easy-to-us
+00000040: 6520 4c4c 4d73 2071 7561 6e74 697a 6174  e LLMs quantizat
+00000050: 696f 6e20 7061 636b 6167 6520 7769 7468  ion package with
+00000060: 2075 7365 722d 6672 6965 6e64 6c79 2061   user-friendly a
+00000070: 7069 732c 2062 6173 6564 206f 6e20 4750  pis, based on GP
+00000080: 5451 2061 6c67 6f72 6974 686d 2e3c 2f70  TQ algorithm.</p
+00000090: 3e0a 3c70 2061 6c69 676e 3d22 6365 6e74  >.<p align="cent
+000000a0: 6572 223e 0a20 2020 203c 6120 6872 6566  er">.    <a href
+000000b0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+000000c0: 2e63 6f6d 2f50 616e 5169 5765 692f 4175  .com/PanQiWei/Au
+000000d0: 746f 4750 5451 2f72 656c 6561 7365 7322  toGPTQ/releases"
+000000e0: 3e0a 2020 2020 2020 2020 3c69 6d67 2061  >.        <img a
+000000f0: 6c74 3d22 4769 7448 7562 2072 656c 6561  lt="GitHub relea
+00000100: 7365 2220 7372 633d 2268 7474 7073 3a2f  se" src="https:/
+00000110: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000120: 6769 7468 7562 2f72 656c 6561 7365 2f50  github/release/P
+00000130: 616e 5169 5765 692f 4175 746f 4750 5451  anQiWei/AutoGPTQ
+00000140: 2e73 7667 223e 0a20 2020 203c 2f61 3e0a  .svg">.    </a>.
+00000150: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+00000160: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+00000170: 6f6a 6563 742f 6175 746f 2d67 7074 712f  oject/auto-gptq/
+00000180: 223e 0a20 2020 2020 2020 203c 696d 6720  ">.        <img 
+00000190: 616c 743d 2250 7950 4920 2d20 446f 776e  alt="PyPI - Down
+000001a0: 6c6f 6164 7322 2073 7263 3d22 6874 7470  loads" src="http
+000001b0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000001c0: 696f 2f70 7970 692f 6464 2f61 7574 6f2d  io/pypi/dd/auto-
+000001d0: 6770 7471 223e 0a20 2020 203c 2f61 3e0a  gptq">.    </a>.
+000001e0: 3c2f 703e 0a3c 6834 2061 6c69 676e 3d22  </p>.<h4 align="
+000001f0: 6365 6e74 6572 223e 0a20 2020 203c 703e  center">.    <p>
+00000200: 0a20 2020 2020 2020 203c 623e 456e 676c  .        <b>Engl
+00000210: 6973 683c 2f62 3e20 7c0a 2020 2020 2020  ish</b> |.      
+00000220: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000230: 3a2f 2f67 6974 6875 622e 636f 6d2f 5061  ://github.com/Pa
+00000240: 6e51 6957 6569 2f41 7574 6f47 5054 512f  nQiWei/AutoGPTQ/
+00000250: 626c 6f62 2f6d 6169 6e2f 5245 4144 4d45  blob/main/README
+00000260: 5f7a 682e 6d64 223e e4b8 ade6 9687 3c2f  _zh.md">......</
+00000270: 613e 0a20 2020 203c 2f70 3e0a 3c2f 6834  a>.    </p>.</h4
+00000280: 3e0a 0a2a 3c63 656e 7465 723e f09f 93a3  >..*<center>....
+00000290: 204c 6f6e 6720 7469 6d65 206e 6f20 7365   Long time no se
+000002a0: 6521 20f0 9f91 8b20 4172 6368 6974 6563  e! .... Architec
+000002b0: 7475 7265 2075 7067 7261 6465 2c20 7065  ture upgrade, pe
+000002c0: 7266 6f72 6d61 6e63 6520 6f70 7469 6d69  rformance optimi
+000002d0: 7a61 7469 6f6e 2061 6e64 206d 6f72 6520  zation and more 
+000002e0: 6e65 7720 6665 6174 7572 6573 2077 696c  new features wil
+000002f0: 6c20 636f 6d65 2069 6e20 4a75 6c79 2061  l come in July a
+00000300: 6e64 2041 7567 7573 742c 2073 7461 7920  nd August, stay 
+00000310: 7475 6e65 2120 f09f a582 3c2f 6365 6e74  tune! ....</cent
+00000320: 6572 3e2a 0a0a 2323 204e 6577 7320 6f72  er>*..## News or
+00000330: 2055 7064 6174 650a 0a2d 2032 3032 332d   Update..- 2023-
+00000340: 3037 2d32 3620 2d20 2855 7064 6174 6529  07-26 - (Update)
+00000350: 202d 2041 6e20 656c 6567 616e 7420 5b50   - An elegant [P
+00000360: 504c 2062 656e 6368 6d61 726b 2073 6372  PL benchmark scr
+00000370: 6970 745d 2865 7861 6d70 6c65 732f 6265  ipt](examples/be
+00000380: 6e63 686d 6172 6b2f 7065 7270 6c65 7869  nchmark/perplexi
+00000390: 7479 2e70 7929 2074 6f20 6765 7420 7265  ty.py) to get re
+000003a0: 7375 6c74 7320 7468 6174 2063 616e 2062  sults that can b
+000003b0: 6520 6661 6972 6c79 2063 6f6d 7061 7265  e fairly compare
+000003c0: 6420 7769 7468 206f 7468 6572 206c 6962  d with other lib
+000003d0: 7261 7269 6573 2073 7563 6820 6173 2060  raries such as `
+000003e0: 6c6c 616d 612e 6370 7060 2e0a 2d20 3230  llama.cpp`..- 20
+000003f0: 3233 2d30 362d 3035 202d 2028 5570 6461  23-06-05 - (Upda
+00000400: 7465 2920 2d20 496e 7465 6772 6174 6520  te) - Integrate 
+00000410: 7769 7468 20f0 9fa4 9720 7065 6674 2074  with .... peft t
+00000420: 6f20 7573 6520 6770 7471 2071 7561 6e74  o use gptq quant
+00000430: 697a 6564 206d 6f64 656c 2074 6f20 7472  ized model to tr
+00000440: 6169 6e20 6164 6170 7465 7273 2c20 7375  ain adapters, su
+00000450: 7070 6f72 7420 4c6f 5241 2c20 4164 614c  pport LoRA, AdaL
+00000460: 6f52 412c 2041 6461 7074 696f 6e50 726f  oRA, AdaptionPro
+00000470: 6d70 742c 2065 7463 2e0a 2d20 3230 3233  mpt, etc..- 2023
+00000480: 2d30 352d 3330 202d 2028 5570 6461 7465  -05-30 - (Update
+00000490: 2920 2d20 5375 7070 6f72 7420 646f 776e  ) - Support down
+000004a0: 6c6f 6164 2f75 706c 6f61 6420 7175 616e  load/upload quan
+000004b0: 7469 7a65 6420 6d6f 6465 6c20 6672 6f6d  tized model from
+000004c0: 2f74 6f20 f09f a497 2048 7562 2e0a 2d20  /to .... Hub..- 
+000004d0: 3230 3233 2d30 352d 3237 202d 2028 5570  2023-05-27 - (Up
+000004e0: 6461 7465 2920 2d20 5375 7070 6f72 7420  date) - Support 
+000004f0: 7175 616e 7469 7a61 7469 6f6e 2061 6e64  quantization and
+00000500: 2069 6e66 6572 656e 6365 2066 6f72 2060   inference for `
+00000510: 6770 745f 6269 6763 6f64 6560 2c20 6063  gpt_bigcode`, `c
+00000520: 6f64 6567 656e 6020 616e 6420 6052 6566  odegen` and `Ref
+00000530: 696e 6557 6562 2f52 6566 696e 6557 6562  ineWeb/RefineWeb
+00000540: 4d6f 6465 6c60 2866 616c 636f 6e29 206d  Model`(falcon) m
+00000550: 6f64 656c 2074 7970 6573 2e0a 2d20 3230  odel types..- 20
+00000560: 3233 2d30 352d 3034 202d 2028 5570 6461  23-05-04 - (Upda
+00000570: 7465 2920 2d20 5375 7070 6f72 7420 7573  te) - Support us
+00000580: 696e 6720 6661 7374 6572 2063 7564 6120  ing faster cuda 
+00000590: 6b65 726e 656c 2077 6865 6e20 606e 6f74  kernel when `not
+000005a0: 2064 6573 635f 6163 7420 6f72 2067 726f   desc_act or gro
+000005b0: 7570 5f73 697a 6520 3d3d 202d 3160 2e0a  up_size == -1`..
+000005c0: 0a2a 466f 7220 6d6f 7265 2068 6973 746f  .*For more histo
+000005d0: 7269 6573 2070 6c65 6173 6520 7475 726e  ries please turn
+000005e0: 2074 6f20 5b68 6572 655d 2864 6f63 732f   to [here](docs/
+000005f0: 4e45 5753 5f4f 525f 5550 4441 5445 2e6d  NEWS_OR_UPDATE.m
+00000600: 6429 2a0a 0a23 2320 5065 7266 6f72 6d61  d)*..## Performa
+00000610: 6e63 6520 436f 6d70 6172 6973 6f6e 0a0a  nce Comparison..
+00000620: 2323 2320 496e 6665 7265 6e63 6520 5370  ### Inference Sp
+00000630: 6565 640a 3e20 5468 6520 7265 7375 6c74  eed.> The result
+00000640: 2069 7320 6765 6e65 7261 7465 6420 7573   is generated us
+00000650: 696e 6720 5b74 6869 7320 7363 7269 7074  ing [this script
+00000660: 5d28 6578 616d 706c 6573 2f62 656e 6368  ](examples/bench
+00000670: 6d61 726b 2f67 656e 6572 6174 696f 6e5f  mark/generation_
+00000680: 7370 6565 642e 7079 292c 2062 6174 6368  speed.py), batch
+00000690: 2073 697a 6520 6f66 2069 6e70 7574 2069   size of input i
+000006a0: 7320 312c 2064 6563 6f64 6520 7374 7261  s 1, decode stra
+000006b0: 7465 6779 2069 7320 6265 616d 2073 6561  tegy is beam sea
+000006c0: 7263 6820 616e 6420 656e 666f 7263 6520  rch and enforce 
+000006d0: 7468 6520 6d6f 6465 6c20 746f 2067 656e  the model to gen
+000006e0: 6572 6174 6520 3531 3220 746f 6b65 6e73  erate 512 tokens
+000006f0: 2c20 7370 6565 6420 6d65 7472 6963 2069  , speed metric i
+00000700: 7320 746f 6b65 6e73 2f73 2028 7468 6520  s tokens/s (the 
+00000710: 6c61 7267 6572 2c20 7468 6520 6265 7474  larger, the bett
+00000720: 6572 292e 0a3e 200a 3e20 5468 6520 7175  er)..> .> The qu
+00000730: 616e 7469 7a65 6420 6d6f 6465 6c20 6973  antized model is
+00000740: 206c 6f61 6465 6420 7573 696e 6720 7468   loaded using th
+00000750: 6520 7365 7475 7020 7468 6174 2063 616e  e setup that can
+00000760: 2067 6169 6e20 7468 6520 6661 7374 6573   gain the fastes
+00000770: 7420 696e 6665 7265 6e63 6520 7370 6565  t inference spee
+00000780: 642e 0a0a 7c20 6d6f 6465 6c20 2020 2020  d...| model     
+00000790: 2020 2020 7c20 4750 5520 2020 2020 2020      | GPU       
+000007a0: 2020 2020 7c20 6e75 6d5f 6265 616d 7320      | num_beams 
+000007b0: 7c20 6670 3136 2020 7c20 6770 7471 2d69  | fp16  | gptq-i
+000007c0: 6e74 3420 7c0a 7c2d 2d2d 2d2d 2d2d 2d2d  nt4 |.|---------
+000007d0: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
+000007e0: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
+000007f0: 2d2d 7c2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  --|-------|-----
+00000800: 2d2d 2d2d 2d2d 7c0a 7c20 6c6c 616d 612d  ------|.| llama-
+00000810: 3762 2020 2020 2020 7c20 3178 4131 3030  7b      | 1xA100
+00000820: 2d34 3047 2020 2020 7c20 3120 2020 2020  -40G    | 1     
+00000830: 2020 2020 7c20 3138 2e38 3720 7c20 3235      | 18.87 | 25
+00000840: 2e35 3320 2020 2020 7c0a 7c20 6c6c 616d  .53     |.| llam
+00000850: 612d 3762 2020 2020 2020 7c20 3178 4131  a-7b      | 1xA1
+00000860: 3030 2d34 3047 2020 2020 7c20 3420 2020  00-40G    | 4   
+00000870: 2020 2020 2020 7c20 3638 2e37 3920 7c20        | 68.79 | 
+00000880: 3931 2e33 3020 2020 2020 7c0a 7c20 6d6f  91.30     |.| mo
+00000890: 7373 2d6d 6f6f 6e20 3136 6220 7c20 3178  ss-moon 16b | 1x
+000008a0: 4131 3030 2d34 3047 2020 2020 7c20 3120  A100-40G    | 1 
+000008b0: 2020 2020 2020 2020 7c20 3132 2e34 3820          | 12.48 
+000008c0: 7c20 3135 2e32 3520 2020 2020 7c0a 7c20  | 15.25     |.| 
+000008d0: 6d6f 7373 2d6d 6f6f 6e20 3136 6220 7c20  moss-moon 16b | 
+000008e0: 3178 4131 3030 2d34 3047 2020 2020 7c20  1xA100-40G    | 
+000008f0: 3420 2020 2020 2020 2020 7c20 4f4f 4d20  4         | OOM 
+00000900: 2020 7c20 3432 2e36 3720 2020 2020 7c0a    | 42.67     |.
+00000910: 7c20 6d6f 7373 2d6d 6f6f 6e20 3136 6220  | moss-moon 16b 
+00000920: 7c20 3278 4131 3030 2d34 3047 2020 2020  | 2xA100-40G    
+00000930: 7c20 3120 2020 2020 2020 2020 7c20 3036  | 1         | 06
+00000940: 2e38 3320 7c20 3036 2e37 3820 2020 2020  .83 | 06.78     
+00000950: 7c0a 7c20 6d6f 7373 2d6d 6f6f 6e20 3136  |.| moss-moon 16
+00000960: 6220 7c20 3278 4131 3030 2d34 3047 2020  b | 2xA100-40G  
+00000970: 2020 7c20 3420 2020 2020 2020 2020 7c20    | 4         | 
+00000980: 3133 2e31 3020 7c20 3130 2e38 3020 2020  13.10 | 10.80   
+00000990: 2020 7c0a 7c20 6770 742d 6a20 3662 2020    |.| gpt-j 6b  
+000009a0: 2020 2020 7c20 3178 5254 5833 3036 302d      | 1xRTX3060-
+000009b0: 3132 4720 7c20 3120 2020 2020 2020 2020  12G | 1         
+000009c0: 7c20 4f4f 4d20 2020 7c20 3239 2e35 3520  | OOM   | 29.55 
+000009d0: 2020 2020 7c0a 7c20 6770 742d 6a20 3662      |.| gpt-j 6b
+000009e0: 2020 2020 2020 7c20 3178 5254 5833 3036        | 1xRTX306
+000009f0: 302d 3132 4720 7c20 3420 2020 2020 2020  0-12G | 4       
+00000a00: 2020 7c20 4f4f 4d20 2020 7c20 3437 2e33    | OOM   | 47.3
+00000a10: 3620 2020 2020 7c0a 0a0a 2323 2320 5065  6     |...### Pe
+00000a20: 7270 6c65 7869 7479 0a46 6f72 2070 6572  rplexity.For per
+00000a30: 706c 6578 6974 7920 636f 6d70 6172 6973  plexity comparis
+00000a40: 6f6e 2c20 796f 7520 6361 6e20 7475 726e  on, you can turn
+00000a50: 2074 6f20 5b68 6572 655d 2868 7474 7073   to [here](https
+00000a60: 3a2f 2f67 6974 6875 622e 636f 6d2f 7177  ://github.com/qw
+00000a70: 6f70 7177 6f70 3230 302f 4750 5451 2d66  opqwop200/GPTQ-f
+00000a80: 6f72 2d4c 4c61 4d61 2372 6573 756c 7429  or-LLaMa#result)
+00000a90: 2061 6e64 205b 6865 7265 5d28 6874 7470   and [here](http
+00000aa0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f71  s://github.com/q
+00000ab0: 776f 7071 776f 7032 3030 2f47 5054 512d  wopqwop200/GPTQ-
+00000ac0: 666f 722d 4c4c 614d 6123 6770 7471 2d76  for-LLaMa#gptq-v
+00000ad0: 732d 6269 7473 616e 6462 7974 6573 290a  s-bitsandbytes).
+00000ae0: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+00000af0: 0a0a 2323 2320 5175 6963 6b20 496e 7374  ..### Quick Inst
+00000b00: 616c 6c61 7469 6f6e 0a59 6f75 2063 616e  allation.You can
+00000b10: 2069 6e73 7461 6c6c 2074 6865 206c 6174   install the lat
+00000b20: 6573 7420 7374 6162 6c65 2072 656c 6561  est stable relea
+00000b30: 7365 206f 6620 4175 746f 4750 5451 2066  se of AutoGPTQ f
+00000b40: 726f 6d20 7069 703a 0a60 6060 7368 656c  rom pip:.```shel
+00000b50: 6c0a 7069 7020 696e 7374 616c 6c20 6175  l.pip install au
+00000b60: 746f 2d67 7074 710a 6060 600a 5374 6172  to-gptq.```.Star
+00000b70: 7420 6672 6f6d 2076 302e 322e 302c 2079  t from v0.2.0, y
+00000b80: 6f75 2063 616e 2064 6f77 6e6c 6f61 6420  ou can download 
+00000b90: 7072 652d 6275 696c 6420 7768 6565 6c20  pre-build wheel 
+00000ba0: 7468 6174 2073 6174 6973 6669 6564 2079  that satisfied y
+00000bb0: 6f75 7220 656e 7669 726f 6e6d 656e 7420  our environment 
+00000bc0: 7365 7475 7020 6672 6f6d 2065 6163 6820  setup from each 
+00000bd0: 7665 7273 696f 6e27 7320 7265 6c65 6173  version's releas
+00000be0: 6520 6173 7365 7473 2061 6e64 2069 6e73  e assets and ins
+00000bf0: 7461 6c6c 2069 7420 746f 2073 6b69 7020  tall it to skip 
+00000c00: 6275 696c 6469 6e67 2073 7461 6765 2066  building stage f
+00000c10: 6f72 2074 6865 2066 6173 7465 7374 2069  or the fastest i
+00000c20: 6e73 7461 6c6c 6174 696f 6e20 7370 6565  nstallation spee
+00000c30: 642e 2046 6f72 2065 7861 6d70 6c65 3a0a  d. For example:.
+00000c40: 6060 6073 6865 6c6c 0a23 2066 6972 7374  ```shell.# first
+00000c50: 6c79 2c20 6364 2074 6865 2064 6972 6563  ly, cd the direc
+00000c60: 746f 7279 2077 6865 7265 2074 6865 2077  tory where the w
+00000c70: 6865 656c 2073 6176 6564 2c20 7468 656e  heel saved, then
+00000c80: 2065 7865 6375 7465 2063 6f6d 6d61 6e64   execute command
+00000c90: 2062 656c 6f77 0a70 6970 2069 6e73 7461   below.pip insta
+00000ca0: 6c6c 2061 7574 6f5f 6770 7471 2d30 2e32  ll auto_gptq-0.2
+00000cb0: 2e30 2b63 7531 3138 2d63 7033 3130 2d63  .0+cu118-cp310-c
+00000cc0: 7033 3130 2d6c 696e 7578 5f78 3836 5f36  p310-linux_x86_6
+00000cd0: 342e 7768 6c20 2320 696e 7374 616c 6c20  4.whl # install 
+00000ce0: 7630 2e32 2e30 2061 7574 6f5f 6770 7471  v0.2.0 auto_gptq
+00000cf0: 2070 7265 2d62 7569 6c64 2077 6865 656c   pre-build wheel
+00000d00: 2066 6f72 206c 696e 7578 2069 6e20 616e   for linux in an
+00000d10: 2065 6e76 6972 6f6e 6d65 6e74 2077 686f   environment who
+00000d20: 7365 2070 7974 686f 6e3d 332e 3130 2061  se python=3.10 a
+00000d30: 6e64 2063 7564 613d 3131 2e38 0a60 6060  nd cuda=11.8.```
+00000d40: 0a23 2323 2320 6469 7361 626c 6520 6375  .#### disable cu
+00000d50: 6461 2065 7874 656e 7369 6f6e 730a 4279  da extensions.By
+00000d60: 2064 6566 6175 6c74 2c20 6375 6461 2065   default, cuda e
+00000d70: 7874 656e 7369 6f6e 7320 7769 6c6c 2062  xtensions will b
+00000d80: 6520 696e 7374 616c 6c65 6420 7768 656e  e installed when
+00000d90: 2060 746f 7263 6860 2061 6e64 2060 6375   `torch` and `cu
+00000da0: 6461 6020 6973 2061 6c72 6561 6479 2069  da` is already i
+00000db0: 6e73 7461 6c6c 6564 2069 6e20 796f 7572  nstalled in your
+00000dc0: 206d 6163 6869 6e65 2c20 6966 2079 6f75   machine, if you
+00000dd0: 2064 6f6e 2774 2077 616e 7420 746f 2075   don't want to u
+00000de0: 7365 2074 6865 6d2c 2075 7369 6e67 3a0a  se them, using:.
+00000df0: 6060 6073 6865 6c6c 0a42 5549 4c44 5f43  ```shell.BUILD_C
+00000e00: 5544 415f 4558 543d 3020 7069 7020 696e  UDA_EXT=0 pip in
+00000e10: 7374 616c 6c20 6175 746f 2d67 7074 710a  stall auto-gptq.
+00000e20: 6060 600a 416e 6420 746f 206d 616b 6520  ```.And to make 
+00000e30: 7375 7265 2060 6175 746f 6770 7471 5f63  sure `autogptq_c
+00000e40: 7564 6160 2069 7320 6e6f 7420 6576 6572  uda` is not ever
+00000e50: 2069 6e20 796f 7572 2076 6972 7475 616c   in your virtual
+00000e60: 2065 6e76 6972 6f6e 6d65 6e74 2c20 7275   environment, ru
+00000e70: 6e3a 0a60 6060 7368 656c 6c0a 7069 7020  n:.```shell.pip 
+00000e80: 756e 696e 7374 616c 6c20 6175 746f 6770  uninstall autogp
+00000e90: 7471 5f63 7564 6120 2d79 0a60 6060 0a0a  tq_cuda -y.```..
+00000ea0: 2323 2323 2074 6f20 7375 7070 6f72 7420  #### to support 
+00000eb0: 7472 6974 6f6e 2073 7065 6564 7570 0a54  triton speedup.T
+00000ec0: 6f20 696e 7465 6772 6174 6520 7769 7468  o integrate with
+00000ed0: 2060 7472 6974 6f6e 602c 2075 7369 6e67   `triton`, using
+00000ee0: 3a0a 3e20 7761 726e 696e 673a 2063 7572  :.> warning: cur
+00000ef0: 7265 6e74 6c79 2074 7269 746f 6e20 6f6e  rently triton on
+00000f00: 6c79 2073 7570 706f 7274 7320 6c69 6e75  ly supports linu
+00000f10: 783b 2033 2d62 6974 2071 7561 6e74 697a  x; 3-bit quantiz
+00000f20: 6174 696f 6e20 6973 206e 6f74 2073 7570  ation is not sup
+00000f30: 706f 7274 6564 2077 6865 6e20 7573 696e  ported when usin
+00000f40: 6720 7472 6974 6f6e 0a0a 6060 6073 6865  g triton..```she
+00000f50: 6c6c 0a70 6970 2069 6e73 7461 6c6c 2061  ll.pip install a
+00000f60: 7574 6f2d 6770 7471 5b74 7269 746f 6e5d  uto-gptq[triton]
+00000f70: 0a60 6060 0a0a 2323 2320 496e 7374 616c  .```..### Instal
+00000f80: 6c20 6672 6f6d 2073 6f75 7263 650a 3c64  l from source.<d
+00000f90: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+00000fa0: 3e63 6c69 636b 2074 6f20 7365 6520 6465  >click to see de
+00000fb0: 7461 696c 733c 2f73 756d 6d61 7279 3e0a  tails</summary>.
+00000fc0: 0a43 6c6f 6e65 2074 6865 2073 6f75 7263  .Clone the sourc
+00000fd0: 6520 636f 6465 3a0a 6060 6073 6865 6c6c  e code:.```shell
+00000fe0: 0a67 6974 2063 6c6f 6e65 2068 7474 7073  .git clone https
+00000ff0: 3a2f 2f67 6974 6875 622e 636f 6d2f 5061  ://github.com/Pa
+00001000: 6e51 6957 6569 2f41 7574 6f47 5054 512e  nQiWei/AutoGPTQ.
+00001010: 6769 7420 2626 2063 6420 4175 746f 4750  git && cd AutoGP
+00001020: 5451 0a60 6060 0a54 6865 6e2c 2069 6e73  TQ.```.Then, ins
+00001030: 7461 6c6c 2066 726f 6d20 736f 7572 6365  tall from source
+00001040: 3a0a 6060 6073 6865 6c6c 0a70 6970 2069  :.```shell.pip i
+00001050: 6e73 7461 6c6c 202e 0a60 6060 0a4c 696b  nstall ..```.Lik
+00001060: 6520 7175 6963 6b20 696e 7374 616c 6c61  e quick installa
+00001070: 7469 6f6e 2c20 796f 7520 6361 6e20 616c  tion, you can al
+00001080: 736f 2073 6574 2060 4255 494c 445f 4355  so set `BUILD_CU
+00001090: 4441 5f45 5854 3d30 6020 746f 2064 6973  DA_EXT=0` to dis
+000010a0: 6162 6c65 2070 7974 6f72 6368 2065 7874  able pytorch ext
+000010b0: 656e 7369 6f6e 2062 7569 6c64 696e 672e  ension building.
+000010c0: 0a0a 5573 6520 602e 5b74 7269 746f 6e5d  ..Use `.[triton]
+000010d0: 6020 6966 2079 6f75 2077 616e 7420 746f  ` if you want to
+000010e0: 2069 6e74 6567 7261 7465 2077 6974 6820   integrate with 
+000010f0: 7472 6974 6f6e 2061 6e64 2069 7427 7320  triton and it's 
+00001100: 6176 6169 6c61 626c 6520 6f6e 2079 6f75  available on you
+00001110: 7220 6f70 6572 6174 696e 6720 7379 7374  r operating syst
+00001120: 656d 2e0a 0a3c 2f64 6574 6169 6c73 3e0a  em...</details>.
+00001130: 0a23 2320 5175 6963 6b20 546f 7572 0a0a  .## Quick Tour..
+00001140: 2323 2320 5175 616e 7469 7a61 7469 6f6e  ### Quantization
+00001150: 2061 6e64 2049 6e66 6572 656e 6365 0a3e   and Inference.>
+00001160: 2077 6172 6e69 6e67 3a20 7468 6973 2069   warning: this i
+00001170: 7320 6a75 7374 2061 2073 686f 7763 6173  s just a showcas
+00001180: 6520 6f66 2074 6865 2075 7361 6765 206f  e of the usage o
+00001190: 6620 6261 7369 6320 6170 6973 2069 6e20  f basic apis in 
+000011a0: 4175 746f 4750 5451 2c20 7768 6963 6820  AutoGPTQ, which 
+000011b0: 7573 6573 206f 6e6c 7920 6f6e 6520 7361  uses only one sa
+000011c0: 6d70 6c65 2074 6f20 7175 616e 7469 7a65  mple to quantize
+000011d0: 2061 206d 7563 6820 736d 616c 6c20 6d6f   a much small mo
+000011e0: 6465 6c2c 2071 7561 6c69 7479 206f 6620  del, quality of 
+000011f0: 7175 616e 7469 7a65 6420 6d6f 6465 6c20  quantized model 
+00001200: 7573 696e 6720 7375 6368 206c 6974 746c  using such littl
+00001210: 6520 7361 6d70 6c65 7320 6d61 7920 6e6f  e samples may no
+00001220: 7420 676f 6f64 2e0a 0a42 656c 6f77 2069  t good...Below i
+00001230: 7320 616e 2065 7861 6d70 6c65 2066 6f72  s an example for
+00001240: 2074 6865 2073 696d 706c 6573 7420 7573   the simplest us
+00001250: 6520 6f66 2060 6175 746f 5f67 7074 7160  e of `auto_gptq`
+00001260: 2074 6f20 7175 616e 7469 7a65 2061 206d   to quantize a m
+00001270: 6f64 656c 2061 6e64 2069 6e66 6572 656e  odel and inferen
+00001280: 6365 2061 6674 6572 2071 7561 6e74 697a  ce after quantiz
+00001290: 6174 696f 6e3a 200a 6060 6070 7974 686f  ation: .```pytho
+000012a0: 6e0a 6672 6f6d 2074 7261 6e73 666f 726d  n.from transform
+000012b0: 6572 7320 696d 706f 7274 2041 7574 6f54  ers import AutoT
+000012c0: 6f6b 656e 697a 6572 2c20 5465 7874 4765  okenizer, TextGe
+000012d0: 6e65 7261 7469 6f6e 5069 7065 6c69 6e65  nerationPipeline
+000012e0: 0a66 726f 6d20 6175 746f 5f67 7074 7120  .from auto_gptq 
+000012f0: 696d 706f 7274 2041 7574 6f47 5054 5146  import AutoGPTQF
+00001300: 6f72 4361 7573 616c 4c4d 2c20 4261 7365  orCausalLM, Base
+00001310: 5175 616e 7469 7a65 436f 6e66 6967 0a69  QuantizeConfig.i
+00001320: 6d70 6f72 7420 6c6f 6767 696e 670a 0a6c  mport logging..l
+00001330: 6f67 6769 6e67 2e62 6173 6963 436f 6e66  ogging.basicConf
+00001340: 6967 280a 2020 2020 666f 726d 6174 3d22  ig(.    format="
+00001350: 2528 6173 6374 696d 6529 7320 2528 6c65  %(asctime)s %(le
+00001360: 7665 6c6e 616d 6529 7320 5b25 286e 616d  velname)s [%(nam
+00001370: 6529 735d 2025 286d 6573 7361 6765 2973  e)s] %(message)s
+00001380: 222c 206c 6576 656c 3d6c 6f67 6769 6e67  ", level=logging
+00001390: 2e49 4e46 4f2c 2064 6174 6566 6d74 3d22  .INFO, datefmt="
+000013a0: 2559 2d25 6d2d 2564 2025 483a 254d 3a25  %Y-%m-%d %H:%M:%
+000013b0: 5322 0a29 0a0a 7072 6574 7261 696e 6564  S".)..pretrained
+000013c0: 5f6d 6f64 656c 5f64 6972 203d 2022 6661  _model_dir = "fa
+000013d0: 6365 626f 6f6b 2f6f 7074 2d31 3235 6d22  cebook/opt-125m"
+000013e0: 0a71 7561 6e74 697a 6564 5f6d 6f64 656c  .quantized_model
+000013f0: 5f64 6972 203d 2022 6f70 742d 3132 356d  _dir = "opt-125m
+00001400: 2d34 6269 7422 0a0a 746f 6b65 6e69 7a65  -4bit"..tokenize
+00001410: 7220 3d20 4175 746f 546f 6b65 6e69 7a65  r = AutoTokenize
+00001420: 722e 6672 6f6d 5f70 7265 7472 6169 6e65  r.from_pretraine
+00001430: 6428 7072 6574 7261 696e 6564 5f6d 6f64  d(pretrained_mod
+00001440: 656c 5f64 6972 2c20 7573 655f 6661 7374  el_dir, use_fast
+00001450: 3d54 7275 6529 0a65 7861 6d70 6c65 7320  =True).examples 
+00001460: 3d20 5b0a 2020 2020 746f 6b65 6e69 7a65  = [.    tokenize
+00001470: 7228 0a20 2020 2020 2020 2022 6175 746f  r(.        "auto
+00001480: 2d67 7074 7120 6973 2061 6e20 6561 7379  -gptq is an easy
+00001490: 2d74 6f2d 7573 6520 6d6f 6465 6c20 7175  -to-use model qu
+000014a0: 616e 7469 7a61 7469 6f6e 206c 6962 7261  antization libra
+000014b0: 7279 2077 6974 6820 7573 6572 2d66 7269  ry with user-fri
+000014c0: 656e 646c 7920 6170 6973 2c20 6261 7365  endly apis, base
+000014d0: 6420 6f6e 2047 5054 5120 616c 676f 7269  d on GPTQ algori
+000014e0: 7468 6d2e 220a 2020 2020 290a 5d0a 0a71  thm.".    ).]..q
+000014f0: 7561 6e74 697a 655f 636f 6e66 6967 203d  uantize_config =
+00001500: 2042 6173 6551 7561 6e74 697a 6543 6f6e   BaseQuantizeCon
+00001510: 6669 6728 0a20 2020 2062 6974 733d 342c  fig(.    bits=4,
+00001520: 2020 2320 7175 616e 7469 7a65 206d 6f64    # quantize mod
+00001530: 656c 2074 6f20 342d 6269 740a 2020 2020  el to 4-bit.    
+00001540: 6772 6f75 705f 7369 7a65 3d31 3238 2c20  group_size=128, 
+00001550: 2023 2069 7420 6973 2072 6563 6f6d 6d65   # it is recomme
+00001560: 6e64 6564 2074 6f20 7365 7420 7468 6520  nded to set the 
+00001570: 7661 6c75 6520 746f 2031 3238 0a20 2020  value to 128.   
+00001580: 2064 6573 635f 6163 743d 4661 6c73 652c   desc_act=False,
+00001590: 2020 2320 7365 7420 746f 2046 616c 7365    # set to False
+000015a0: 2063 616e 2073 6967 6e69 6669 6361 6e74   can significant
+000015b0: 6c79 2073 7065 6564 2075 7020 696e 6665  ly speed up infe
+000015c0: 7265 6e63 6520 6275 7420 7468 6520 7065  rence but the pe
+000015d0: 7270 6c65 7869 7479 206d 6179 2073 6c69  rplexity may sli
+000015e0: 6768 746c 7920 6261 6420 0a29 0a0a 2320  ghtly bad .)..# 
+000015f0: 6c6f 6164 2075 6e2d 7175 616e 7469 7a65  load un-quantize
+00001600: 6420 6d6f 6465 6c2c 2062 7920 6465 6661  d model, by defa
+00001610: 756c 742c 2074 6865 206d 6f64 656c 2077  ult, the model w
+00001620: 696c 6c20 616c 7761 7973 2062 6520 6c6f  ill always be lo
+00001630: 6164 6564 2069 6e74 6f20 4350 5520 6d65  aded into CPU me
+00001640: 6d6f 7279 0a6d 6f64 656c 203d 2041 7574  mory.model = Aut
+00001650: 6f47 5054 5146 6f72 4361 7573 616c 4c4d  oGPTQForCausalLM
+00001660: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
+00001670: 2870 7265 7472 6169 6e65 645f 6d6f 6465  (pretrained_mode
+00001680: 6c5f 6469 722c 2071 7561 6e74 697a 655f  l_dir, quantize_
+00001690: 636f 6e66 6967 290a 0a23 2071 7561 6e74  config)..# quant
+000016a0: 697a 6520 6d6f 6465 6c2c 2074 6865 2065  ize model, the e
+000016b0: 7861 6d70 6c65 7320 7368 6f75 6c64 2062  xamples should b
+000016c0: 6520 6c69 7374 206f 6620 6469 6374 2077  e list of dict w
+000016d0: 686f 7365 206b 6579 7320 6361 6e20 6f6e  hose keys can on
+000016e0: 6c79 2062 6520 2269 6e70 7574 5f69 6473  ly be "input_ids
+000016f0: 2220 616e 6420 2261 7474 656e 7469 6f6e  " and "attention
+00001700: 5f6d 6173 6b22 0a6d 6f64 656c 2e71 7561  _mask".model.qua
+00001710: 6e74 697a 6528 6578 616d 706c 6573 290a  ntize(examples).
+00001720: 0a23 2073 6176 6520 7175 616e 7469 7a65  .# save quantize
+00001730: 6420 6d6f 6465 6c0a 6d6f 6465 6c2e 7361  d model.model.sa
+00001740: 7665 5f71 7561 6e74 697a 6564 2871 7561  ve_quantized(qua
+00001750: 6e74 697a 6564 5f6d 6f64 656c 5f64 6972  ntized_model_dir
+00001760: 290a 0a23 2073 6176 6520 7175 616e 7469  )..# save quanti
+00001770: 7a65 6420 6d6f 6465 6c20 7573 696e 6720  zed model using 
+00001780: 7361 6665 7465 6e73 6f72 730a 6d6f 6465  safetensors.mode
+00001790: 6c2e 7361 7665 5f71 7561 6e74 697a 6564  l.save_quantized
+000017a0: 2871 7561 6e74 697a 6564 5f6d 6f64 656c  (quantized_model
+000017b0: 5f64 6972 2c20 7573 655f 7361 6665 7465  _dir, use_safete
+000017c0: 6e73 6f72 733d 5472 7565 290a 0a23 2070  nsors=True)..# p
+000017d0: 7573 6820 7175 616e 7469 7a65 6420 6d6f  ush quantized mo
+000017e0: 6465 6c20 746f 2048 7567 6769 6e67 2046  del to Hugging F
+000017f0: 6163 6520 4875 622e 200a 2320 746f 2075  ace Hub. .# to u
+00001800: 7365 2075 7365 5f61 7574 685f 746f 6b65  se use_auth_toke
+00001810: 6e3d 5472 7565 2c20 4c6f 6769 6e20 6669  n=True, Login fi
+00001820: 7273 7420 7669 6120 6875 6767 696e 6766  rst via huggingf
+00001830: 6163 652d 636c 6920 6c6f 6769 6e2e 0a23  ace-cli login..#
+00001840: 206f 7220 7061 7373 2065 7870 6c63 6974   or pass explcit
+00001850: 2074 6f6b 656e 2077 6974 683a 2075 7365   token with: use
+00001860: 5f61 7574 685f 746f 6b65 6e3d 2268 665f  _auth_token="hf_
+00001870: 7878 7878 7878 7822 0a23 2028 756e 636f  xxxxxxx".# (unco
+00001880: 6d6d 656e 7420 7468 6520 666f 6c6c 6f77  mment the follow
+00001890: 696e 6720 7468 7265 6520 6c69 6e65 7320  ing three lines 
+000018a0: 746f 2065 6e61 626c 6520 7468 6973 2066  to enable this f
+000018b0: 6561 7475 7265 290a 2320 7265 706f 5f69  eature).# repo_i
+000018c0: 6420 3d20 6622 596f 7572 5573 6572 4e61  d = f"YourUserNa
+000018d0: 6d65 2f7b 7175 616e 7469 7a65 645f 6d6f  me/{quantized_mo
+000018e0: 6465 6c5f 6469 727d 220a 2320 636f 6d6d  del_dir}".# comm
+000018f0: 6974 5f6d 6573 7361 6765 203d 2066 2241  it_message = f"A
+00001900: 7574 6f47 5054 5120 6d6f 6465 6c20 666f  utoGPTQ model fo
+00001910: 7220 7b70 7265 7472 6169 6e65 645f 6d6f  r {pretrained_mo
+00001920: 6465 6c5f 6469 727d 3a20 7b71 7561 6e74  del_dir}: {quant
+00001930: 697a 655f 636f 6e66 6967 2e62 6974 737d  ize_config.bits}
+00001940: 6269 7473 2c20 6772 7b71 7561 6e74 697a  bits, gr{quantiz
+00001950: 655f 636f 6e66 6967 2e67 726f 7570 5f73  e_config.group_s
+00001960: 697a 657d 2c20 6465 7363 5f61 6374 3d7b  ize}, desc_act={
+00001970: 7175 616e 7469 7a65 5f63 6f6e 6669 672e  quantize_config.
+00001980: 6465 7363 5f61 6374 7d22 0a23 206d 6f64  desc_act}".# mod
+00001990: 656c 2e70 7573 685f 746f 5f68 7562 2872  el.push_to_hub(r
+000019a0: 6570 6f5f 6964 2c20 636f 6d6d 6974 5f6d  epo_id, commit_m
+000019b0: 6573 7361 6765 3d63 6f6d 6d69 745f 6d65  essage=commit_me
+000019c0: 7373 6167 652c 2075 7365 5f61 7574 685f  ssage, use_auth_
+000019d0: 746f 6b65 6e3d 5472 7565 290a 0a23 2061  token=True)..# a
+000019e0: 6c74 6572 6e61 7469 7665 6c79 2079 6f75  lternatively you
+000019f0: 2063 616e 2073 6176 6520 616e 6420 7075   can save and pu
+00001a00: 7368 2061 7420 7468 6520 7361 6d65 2074  sh at the same t
+00001a10: 696d 650a 2320 2875 6e63 6f6d 6d65 6e74  ime.# (uncomment
+00001a20: 2074 6865 2066 6f6c 6c6f 7769 6e67 2074   the following t
+00001a30: 6872 6565 206c 696e 6573 2074 6f20 656e  hree lines to en
+00001a40: 6162 6c65 2074 6869 7320 6665 6174 7572  able this featur
+00001a50: 6529 0a23 2072 6570 6f5f 6964 203d 2066  e).# repo_id = f
+00001a60: 2259 6f75 7255 7365 724e 616d 652f 7b71  "YourUserName/{q
+00001a70: 7561 6e74 697a 6564 5f6d 6f64 656c 5f64  uantized_model_d
+00001a80: 6972 7d22 0a23 2063 6f6d 6d69 745f 6d65  ir}".# commit_me
+00001a90: 7373 6167 6520 3d20 6622 4175 746f 4750  ssage = f"AutoGP
+00001aa0: 5451 206d 6f64 656c 2066 6f72 207b 7072  TQ model for {pr
+00001ab0: 6574 7261 696e 6564 5f6d 6f64 656c 5f64  etrained_model_d
+00001ac0: 6972 7d3a 207b 7175 616e 7469 7a65 5f63  ir}: {quantize_c
+00001ad0: 6f6e 6669 672e 6269 7473 7d62 6974 732c  onfig.bits}bits,
+00001ae0: 2067 727b 7175 616e 7469 7a65 5f63 6f6e   gr{quantize_con
+00001af0: 6669 672e 6772 6f75 705f 7369 7a65 7d2c  fig.group_size},
+00001b00: 2064 6573 635f 6163 743d 7b71 7561 6e74   desc_act={quant
+00001b10: 697a 655f 636f 6e66 6967 2e64 6573 635f  ize_config.desc_
+00001b20: 6163 747d 220a 2320 6d6f 6465 6c2e 7075  act}".# model.pu
+00001b30: 7368 5f74 6f5f 6875 6228 7265 706f 5f69  sh_to_hub(repo_i
+00001b40: 642c 2073 6176 655f 6469 723d 7175 616e  d, save_dir=quan
+00001b50: 7469 7a65 645f 6d6f 6465 6c5f 6469 722c  tized_model_dir,
+00001b60: 2075 7365 5f73 6166 6574 656e 736f 7273   use_safetensors
+00001b70: 3d54 7275 652c 2063 6f6d 6d69 745f 6d65  =True, commit_me
+00001b80: 7373 6167 653d 636f 6d6d 6974 5f6d 6573  ssage=commit_mes
+00001b90: 7361 6765 2c20 7573 655f 6175 7468 5f74  sage, use_auth_t
+00001ba0: 6f6b 656e 3d54 7275 6529 0a0a 2320 6c6f  oken=True)..# lo
+00001bb0: 6164 2071 7561 6e74 697a 6564 206d 6f64  ad quantized mod
+00001bc0: 656c 2074 6f20 7468 6520 6669 7273 7420  el to the first 
+00001bd0: 4750 550a 6d6f 6465 6c20 3d20 4175 746f  GPU.model = Auto
+00001be0: 4750 5451 466f 7243 6175 7361 6c4c 4d2e  GPTQForCausalLM.
+00001bf0: 6672 6f6d 5f71 7561 6e74 697a 6564 2871  from_quantized(q
+00001c00: 7561 6e74 697a 6564 5f6d 6f64 656c 5f64  uantized_model_d
+00001c10: 6972 2c20 6465 7669 6365 3d22 6375 6461  ir, device="cuda
+00001c20: 3a30 2229 0a0a 2320 646f 776e 6c6f 6164  :0")..# download
+00001c30: 2071 7561 6e74 697a 6564 206d 6f64 656c   quantized model
+00001c40: 2066 726f 6d20 4875 6767 696e 6720 4661   from Hugging Fa
+00001c50: 6365 2048 7562 2061 6e64 206c 6f61 6420  ce Hub and load 
+00001c60: 746f 2074 6865 2066 6972 7374 2047 5055  to the first GPU
+00001c70: 0a23 206d 6f64 656c 203d 2041 7574 6f47  .# model = AutoG
+00001c80: 5054 5146 6f72 4361 7573 616c 4c4d 2e66  PTQForCausalLM.f
+00001c90: 726f 6d5f 7175 616e 7469 7a65 6428 7265  rom_quantized(re
+00001ca0: 706f 5f69 642c 2064 6576 6963 653d 2263  po_id, device="c
+00001cb0: 7564 613a 3022 2c20 7573 655f 7361 6665  uda:0", use_safe
+00001cc0: 7465 6e73 6f72 733d 5472 7565 2c20 7573  tensors=True, us
+00001cd0: 655f 7472 6974 6f6e 3d46 616c 7365 290a  e_triton=False).
+00001ce0: 0a23 2069 6e66 6572 656e 6365 2077 6974  .# inference wit
+00001cf0: 6820 6d6f 6465 6c2e 6765 6e65 7261 7465  h model.generate
+00001d00: 0a70 7269 6e74 2874 6f6b 656e 697a 6572  .print(tokenizer
+00001d10: 2e64 6563 6f64 6528 6d6f 6465 6c2e 6765  .decode(model.ge
+00001d20: 6e65 7261 7465 282a 2a74 6f6b 656e 697a  nerate(**tokeniz
+00001d30: 6572 2822 6175 746f 5f67 7074 7120 6973  er("auto_gptq is
+00001d40: 222c 2072 6574 7572 6e5f 7465 6e73 6f72  ", return_tensor
+00001d50: 733d 2270 7422 292e 746f 286d 6f64 656c  s="pt").to(model
+00001d60: 2e64 6576 6963 6529 295b 305d 2929 0a0a  .device))[0]))..
+00001d70: 2320 6f72 2079 6f75 2063 616e 2061 6c73  # or you can als
+00001d80: 6f20 7573 6520 7069 7065 6c69 6e65 0a70  o use pipeline.p
+00001d90: 6970 656c 696e 6520 3d20 5465 7874 4765  ipeline = TextGe
+00001da0: 6e65 7261 7469 6f6e 5069 7065 6c69 6e65  nerationPipeline
+00001db0: 286d 6f64 656c 3d6d 6f64 656c 2c20 746f  (model=model, to
+00001dc0: 6b65 6e69 7a65 723d 746f 6b65 6e69 7a65  kenizer=tokenize
+00001dd0: 7229 0a70 7269 6e74 2870 6970 656c 696e  r).print(pipelin
+00001de0: 6528 2261 7574 6f2d 6770 7471 2069 7322  e("auto-gptq is"
+00001df0: 295b 305d 5b22 6765 6e65 7261 7465 645f  )[0]["generated_
+00001e00: 7465 7874 225d 290a 6060 600a 0a46 6f72  text"]).```..For
+00001e10: 206d 6f72 6520 6164 7661 6e63 6564 2066   more advanced f
+00001e20: 6561 7475 7265 7320 6f66 206d 6f64 656c  eatures of model
+00001e30: 2071 7561 6e74 697a 6174 696f 6e2c 2070   quantization, p
+00001e40: 6c65 6173 6520 7265 6665 7265 6e63 6520  lease reference 
+00001e50: 746f 205b 7468 6973 2073 6372 6970 745d  to [this script]
+00001e60: 2865 7861 6d70 6c65 732f 7175 616e 7469  (examples/quanti
+00001e70: 7a61 7469 6f6e 2f71 7561 6e74 5f77 6974  zation/quant_wit
+00001e80: 685f 616c 7061 6361 2e70 7929 0a0a 2323  h_alpaca.py)..##
+00001e90: 2320 4375 7374 6f6d 697a 6520 4d6f 6465  # Customize Mode
+00001ea0: 6c0a 3c64 6574 6169 6c73 3e0a 0a3c 7375  l.<details>..<su
+00001eb0: 6d6d 6172 793e 4265 6c6f 7720 6973 2061  mmary>Below is a
+00001ec0: 6e20 6578 616d 706c 6520 746f 2065 7874  n example to ext
+00001ed0: 656e 6420 6061 7574 6f5f 6770 7471 6020  end `auto_gptq` 
+00001ee0: 746f 2073 7570 706f 7274 2060 4f50 5460  to support `OPT`
+00001ef0: 206d 6f64 656c 2c20 6173 2079 6f75 2077   model, as you w
+00001f00: 696c 6c20 7365 652c 2069 7427 7320 7665  ill see, it's ve
+00001f10: 7279 2065 6173 793a 3c2f 7375 6d6d 6172  ry easy:</summar
+00001f20: 793e 0a0a 6060 6070 7974 686f 6e0a 6672  y>..```python.fr
+00001f30: 6f6d 2061 7574 6f5f 6770 7471 2e6d 6f64  om auto_gptq.mod
+00001f40: 656c 696e 6720 696d 706f 7274 2042 6173  eling import Bas
+00001f50: 6547 5054 5146 6f72 4361 7573 616c 4c4d  eGPTQForCausalLM
+00001f60: 0a0a 0a63 6c61 7373 204f 5054 4750 5451  ...class OPTGPTQ
+00001f70: 466f 7243 6175 7361 6c4c 4d28 4261 7365  ForCausalLM(Base
+00001f80: 4750 5451 466f 7243 6175 7361 6c4c 4d29  GPTQForCausalLM)
+00001f90: 3a0a 2020 2020 2320 6368 6169 6e65 6420  :.    # chained 
+00001fa0: 6174 7472 6962 7574 6520 6e61 6d65 206f  attribute name o
+00001fb0: 6620 7472 616e 7366 6f72 6d65 7220 6c61  f transformer la
+00001fc0: 7965 7220 626c 6f63 6b0a 2020 2020 6c61  yer block.    la
+00001fd0: 7965 7273 5f62 6c6f 636b 5f6e 616d 6520  yers_block_name 
+00001fe0: 3d20 226d 6f64 656c 2e64 6563 6f64 6572  = "model.decoder
+00001ff0: 2e6c 6179 6572 7322 0a20 2020 2023 2063  .layers".    # c
+00002000: 6861 696e 6564 2061 7474 7269 6275 7465  hained attribute
+00002010: 206e 616d 6573 206f 6620 6f74 6865 7220   names of other 
+00002020: 6e6e 206d 6f64 756c 6573 2074 6861 7420  nn modules that 
+00002030: 696e 2074 6865 2073 616d 6520 6c65 7665  in the same leve
+00002040: 6c20 6173 2074 6865 2074 7261 6e73 666f  l as the transfo
+00002050: 726d 6572 206c 6179 6572 2062 6c6f 636b  rmer layer block
+00002060: 0a20 2020 206f 7574 7369 6465 5f6c 6179  .    outside_lay
+00002070: 6572 5f6d 6f64 756c 6573 203d 205b 0a20  er_modules = [. 
+00002080: 2020 2020 2020 2022 6d6f 6465 6c2e 6465         "model.de
+00002090: 636f 6465 722e 656d 6265 645f 746f 6b65  coder.embed_toke
+000020a0: 6e73 222c 2022 6d6f 6465 6c2e 6465 636f  ns", "model.deco
+000020b0: 6465 722e 656d 6265 645f 706f 7369 7469  der.embed_positi
+000020c0: 6f6e 7322 2c20 226d 6f64 656c 2e64 6563  ons", "model.dec
+000020d0: 6f64 6572 2e70 726f 6a65 6374 5f6f 7574  oder.project_out
+000020e0: 222c 0a20 2020 2020 2020 2022 6d6f 6465  ",.        "mode
+000020f0: 6c2e 6465 636f 6465 722e 7072 6f6a 6563  l.decoder.projec
+00002100: 745f 696e 222c 2022 6d6f 6465 6c2e 6465  t_in", "model.de
+00002110: 636f 6465 722e 6669 6e61 6c5f 6c61 7965  coder.final_laye
+00002120: 725f 6e6f 726d 220a 2020 2020 5d0a 2020  r_norm".    ].  
+00002130: 2020 2320 6368 6169 6e65 6420 6174 7472    # chained attr
+00002140: 6962 7574 6520 6e61 6d65 7320 6f66 206c  ibute names of l
+00002150: 696e 6561 7220 6c61 7965 7273 2069 6e20  inear layers in 
+00002160: 7472 616e 7366 6f72 6d65 7220 6c61 7965  transformer laye
+00002170: 7220 6d6f 6475 6c65 0a20 2020 2023 206e  r module.    # n
+00002180: 6f72 6d61 6c6c 792c 2074 6865 7265 2061  ormally, there a
+00002190: 7265 2066 6f75 7220 7375 6220 6c69 7374  re four sub list
+000021a0: 732c 2066 6f72 2065 6163 6820 6f6e 6520  s, for each one 
+000021b0: 7468 6520 6d6f 6475 6c65 7320 696e 2069  the modules in i
+000021c0: 7420 6361 6e20 6265 2073 6565 6e20 6173  t can be seen as
+000021d0: 206f 6e65 206f 7065 7261 7469 6f6e 2c20   one operation, 
+000021e0: 0a20 2020 2023 2061 6e64 2074 6865 206f  .    # and the o
+000021f0: 7264 6572 2073 686f 756c 6420 6265 2074  rder should be t
+00002200: 6865 206f 7264 6572 2077 6865 6e20 7468  he order when th
+00002210: 6579 2061 7265 2074 7275 6c79 2065 7865  ey are truly exe
+00002220: 6375 7465 642c 2069 6e20 7468 6973 2063  cuted, in this c
+00002230: 6173 6520 2861 6e64 2075 7375 616c 6c79  ase (and usually
+00002240: 2069 6e20 6d6f 7374 2063 6173 6573 292c   in most cases),
+00002250: 200a 2020 2020 2320 7468 6579 2061 7265   .    # they are
+00002260: 3a20 6174 7465 6e74 696f 6e20 715f 6b5f  : attention q_k_
+00002270: 7620 7072 6f6a 6563 7469 6f6e 2c20 6174  v projection, at
+00002280: 7465 6e74 696f 6e20 6f75 7470 7574 2070  tention output p
+00002290: 726f 6a65 6374 696f 6e2c 204d 4c50 2070  rojection, MLP p
+000022a0: 726f 6a65 6374 2069 6e70 7574 2c20 4d4c  roject input, ML
+000022b0: 5020 7072 6f6a 6563 7420 6f75 7470 7574  P project output
+000022c0: 0a20 2020 2069 6e73 6964 655f 6c61 7965  .    inside_laye
+000022d0: 725f 6d6f 6475 6c65 7320 3d20 5b0a 2020  r_modules = [.  
+000022e0: 2020 2020 2020 5b22 7365 6c66 5f61 7474        ["self_att
+000022f0: 6e2e 6b5f 7072 6f6a 222c 2022 7365 6c66  n.k_proj", "self
+00002300: 5f61 7474 6e2e 765f 7072 6f6a 222c 2022  _attn.v_proj", "
+00002310: 7365 6c66 5f61 7474 6e2e 715f 7072 6f6a  self_attn.q_proj
+00002320: 225d 2c0a 2020 2020 2020 2020 5b22 7365  "],.        ["se
+00002330: 6c66 5f61 7474 6e2e 6f75 745f 7072 6f6a  lf_attn.out_proj
+00002340: 225d 2c0a 2020 2020 2020 2020 5b22 6663  "],.        ["fc
+00002350: 3122 5d2c 0a20 2020 2020 2020 205b 2266  1"],.        ["f
+00002360: 6332 225d 0a20 2020 205d 0a60 6060 0a41  c2"].    ].```.A
+00002370: 6674 6572 2074 6869 732c 2079 6f75 2063  fter this, you c
+00002380: 616e 2075 7365 2060 4f50 5447 5054 5146  an use `OPTGPTQF
+00002390: 6f72 4361 7573 616c 4c4d 2e66 726f 6d5f  orCausalLM.from_
+000023a0: 7072 6574 7261 696e 6564 6020 616e 6420  pretrained` and 
+000023b0: 6f74 6865 7220 6d65 7468 6f64 7320 6173  other methods as
+000023c0: 2073 686f 776e 2069 6e20 4261 7369 632e   shown in Basic.
+000023d0: 0a0a 3c2f 6465 7461 696c 733e 0a0a 2323  ..</details>..##
+000023e0: 2320 4576 616c 7561 7469 6f6e 206f 6e20  # Evaluation on 
+000023f0: 446f 776e 7374 7265 616d 2054 6173 6b73  Downstream Tasks
+00002400: 0a59 6f75 2063 616e 2075 7365 2074 6173  .You can use tas
+00002410: 6b73 2064 6566 696e 6564 2069 6e20 6061  ks defined in `a
+00002420: 7574 6f5f 6770 7471 2e65 7661 6c5f 7461  uto_gptq.eval_ta
+00002430: 736b 7360 2074 6f20 6576 616c 7561 7465  sks` to evaluate
+00002440: 206d 6f64 656c 2773 2070 6572 666f 726d   model's perform
+00002450: 616e 6365 206f 6e20 7370 6563 6966 6963  ance on specific
+00002460: 2064 6f77 6e2d 7374 7265 616d 2074 6173   down-stream tas
+00002470: 6b20 6265 666f 7265 2061 6e64 2061 6674  k before and aft
+00002480: 6572 2071 7561 6e74 697a 6174 696f 6e2e  er quantization.
+00002490: 0a0a 5468 6520 7072 6564 6566 696e 6564  ..The predefined
+000024a0: 2074 6173 6b73 2073 7570 706f 7274 2061   tasks support a
+000024b0: 6c6c 2063 6175 7361 6c2d 6c61 6e67 7561  ll causal-langua
+000024c0: 6765 2d6d 6f64 656c 7320 696d 706c 656d  ge-models implem
+000024d0: 656e 7465 6420 696e 205b f09f a497 2074  ented in [.... t
+000024e0: 7261 6e73 666f 726d 6572 735d 2868 7474  ransformers](htt
+000024f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002500: 6875 6767 696e 6766 6163 652f 7472 616e  huggingface/tran
+00002510: 7366 6f72 6d65 7273 2920 616e 6420 696e  sformers) and in
+00002520: 2074 6869 7320 7072 6f6a 6563 742e 0a0a   this project...
+00002530: 3c64 6574 6169 6c73 3e0a 0a3c 7375 6d6d  <details>..<summ
+00002540: 6172 793e 4265 6c6f 7720 6973 2061 6e20  ary>Below is an 
+00002550: 6578 616d 706c 6520 746f 2065 7661 6c75  example to evalu
+00002560: 6174 6520 6045 6c65 7574 6865 7241 492f  ate `EleutherAI/
+00002570: 6770 742d 6a2d 3662 6020 6f6e 2073 6571  gpt-j-6b` on seq
+00002580: 7565 6e63 652d 636c 6173 7369 6669 6361  uence-classifica
+00002590: 7469 6f6e 2074 6173 6b20 7573 696e 6720  tion task using 
+000025a0: 6063 6172 6469 6666 6e6c 702f 7477 6565  `cardiffnlp/twee
+000025b0: 745f 7365 6e74 696d 656e 745f 6d75 6c74  t_sentiment_mult
+000025c0: 696c 696e 6775 616c 6020 6461 7461 7365  ilingual` datase
+000025d0: 743a 3c2f 7375 6d6d 6172 793e 0a0a 6060  t:</summary>..``
+000025e0: 6070 7974 686f 6e0a 6672 6f6d 2066 756e  `python.from fun
+000025f0: 6374 6f6f 6c73 2069 6d70 6f72 7420 7061  ctools import pa
+00002600: 7274 6961 6c0a 0a69 6d70 6f72 7420 6461  rtial..import da
+00002610: 7461 7365 7473 0a66 726f 6d20 7472 616e  tasets.from tran
+00002620: 7366 6f72 6d65 7273 2069 6d70 6f72 7420  sformers import 
+00002630: 4175 746f 546f 6b65 6e69 7a65 722c 2041  AutoTokenizer, A
+00002640: 7574 6f4d 6f64 656c 466f 7243 6175 7361  utoModelForCausa
+00002650: 6c4c 4d2c 2047 656e 6572 6174 696f 6e43  lLM, GenerationC
+00002660: 6f6e 6669 670a 0a66 726f 6d20 6175 746f  onfig..from auto
+00002670: 5f67 7074 7120 696d 706f 7274 2041 7574  _gptq import Aut
+00002680: 6f47 5054 5146 6f72 4361 7573 616c 4c4d  oGPTQForCausalLM
+00002690: 2c20 4261 7365 5175 616e 7469 7a65 436f  , BaseQuantizeCo
+000026a0: 6e66 6967 0a66 726f 6d20 6175 746f 5f67  nfig.from auto_g
+000026b0: 7074 712e 6576 616c 5f74 6173 6b73 2069  ptq.eval_tasks i
+000026c0: 6d70 6f72 7420 5365 7175 656e 6365 436c  mport SequenceCl
+000026d0: 6173 7369 6669 6361 7469 6f6e 5461 736b  assificationTask
+000026e0: 0a0a 0a4d 4f44 454c 203d 2022 456c 6575  ...MODEL = "Eleu
+000026f0: 7468 6572 4149 2f67 7074 2d6a 2d36 6222  therAI/gpt-j-6b"
+00002700: 0a44 4154 4153 4554 203d 2022 6361 7264  .DATASET = "card
+00002710: 6966 666e 6c70 2f74 7765 6574 5f73 656e  iffnlp/tweet_sen
+00002720: 7469 6d65 6e74 5f6d 756c 7469 6c69 6e67  timent_multiling
+00002730: 7561 6c22 0a54 454d 504c 4154 4520 3d20  ual".TEMPLATE = 
+00002740: 2251 7565 7374 696f 6e3a 5768 6174 2773  "Question:What's
+00002750: 2074 6865 2073 656e 7469 6d65 6e74 206f   the sentiment o
+00002760: 6620 7468 6520 6769 7665 6e20 7465 7874  f the given text
+00002770: 3f20 4368 6f69 6365 7320 6172 6520 7b6c  ? Choices are {l
+00002780: 6162 656c 737d 2e5c 6e54 6578 743a 207b  abels}.\nText: {
+00002790: 7465 7874 7d5c 6e41 6e73 7765 723a 220a  text}\nAnswer:".
+000027a0: 4944 324c 4142 454c 203d 207b 0a20 2020  ID2LABEL = {.   
+000027b0: 2030 3a20 226e 6567 6174 6976 6522 2c0a   0: "negative",.
+000027c0: 2020 2020 313a 2022 6e65 7574 7261 6c22      1: "neutral"
+000027d0: 2c0a 2020 2020 323a 2022 706f 7369 7469  ,.    2: "positi
+000027e0: 7665 220a 7d0a 4c41 4245 4c53 203d 206c  ve".}.LABELS = l
+000027f0: 6973 7428 4944 324c 4142 454c 2e76 616c  ist(ID2LABEL.val
+00002800: 7565 7328 2929 0a0a 0a64 6566 2064 735f  ues())...def ds_
+00002810: 7265 6661 6374 6f72 5f66 6e28 7361 6d70  refactor_fn(samp
+00002820: 6c65 7329 3a0a 2020 2020 7465 7874 5f64  les):.    text_d
+00002830: 6174 6120 3d20 7361 6d70 6c65 735b 2274  ata = samples["t
+00002840: 6578 7422 5d0a 2020 2020 6c61 6265 6c5f  ext"].    label_
+00002850: 6461 7461 203d 2073 616d 706c 6573 5b22  data = samples["
+00002860: 6c61 6265 6c22 5d0a 0a20 2020 206e 6577  label"]..    new
+00002870: 5f73 616d 706c 6573 203d 207b 2270 726f  _samples = {"pro
+00002880: 6d70 7422 3a20 5b5d 2c20 226c 6162 656c  mpt": [], "label
+00002890: 223a 205b 5d7d 0a20 2020 2066 6f72 2074  ": []}.    for t
+000028a0: 6578 742c 206c 6162 656c 2069 6e20 7a69  ext, label in zi
+000028b0: 7028 7465 7874 5f64 6174 612c 206c 6162  p(text_data, lab
+000028c0: 656c 5f64 6174 6129 3a0a 2020 2020 2020  el_data):.      
+000028d0: 2020 7072 6f6d 7074 203d 2054 454d 504c    prompt = TEMPL
+000028e0: 4154 452e 666f 726d 6174 286c 6162 656c  ATE.format(label
+000028f0: 733d 4c41 4245 4c53 2c20 7465 7874 3d74  s=LABELS, text=t
+00002900: 6578 7429 0a20 2020 2020 2020 206e 6577  ext).        new
+00002910: 5f73 616d 706c 6573 5b22 7072 6f6d 7074  _samples["prompt
+00002920: 225d 2e61 7070 656e 6428 7072 6f6d 7074  "].append(prompt
+00002930: 290a 2020 2020 2020 2020 6e65 775f 7361  ).        new_sa
+00002940: 6d70 6c65 735b 226c 6162 656c 225d 2e61  mples["label"].a
+00002950: 7070 656e 6428 4944 324c 4142 454c 5b6c  ppend(ID2LABEL[l
+00002960: 6162 656c 5d29 0a0a 2020 2020 7265 7475  abel])..    retu
+00002970: 726e 206e 6577 5f73 616d 706c 6573 0a0a  rn new_samples..
+00002980: 0a23 2020 6d6f 6465 6c20 3d20 4175 746f  .#  model = Auto
+00002990: 4d6f 6465 6c46 6f72 4361 7573 616c 4c4d  ModelForCausalLM
+000029a0: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
+000029b0: 284d 4f44 454c 292e 6576 616c 2829 2e68  (MODEL).eval().h
+000029c0: 616c 6628 292e 746f 2822 6375 6461 3a30  alf().to("cuda:0
+000029d0: 2229 0a6d 6f64 656c 203d 2041 7574 6f47  ").model = AutoG
+000029e0: 5054 5146 6f72 4361 7573 616c 4c4d 2e66  PTQForCausalLM.f
+000029f0: 726f 6d5f 7072 6574 7261 696e 6564 284d  rom_pretrained(M
+00002a00: 4f44 454c 2c20 4261 7365 5175 616e 7469  ODEL, BaseQuanti
+00002a10: 7a65 436f 6e66 6967 2829 290a 746f 6b65  zeConfig()).toke
+00002a20: 6e69 7a65 7220 3d20 4175 746f 546f 6b65  nizer = AutoToke
+00002a30: 6e69 7a65 722e 6672 6f6d 5f70 7265 7472  nizer.from_pretr
+00002a40: 6169 6e65 6428 4d4f 4445 4c29 0a0a 7461  ained(MODEL)..ta
+00002a50: 736b 203d 2053 6571 7565 6e63 6543 6c61  sk = SequenceCla
+00002a60: 7373 6966 6963 6174 696f 6e54 6173 6b28  ssificationTask(
+00002a70: 0a20 2020 2020 2020 206d 6f64 656c 3d6d  .        model=m
+00002a80: 6f64 656c 2c0a 2020 2020 2020 2020 746f  odel,.        to
+00002a90: 6b65 6e69 7a65 723d 746f 6b65 6e69 7a65  kenizer=tokenize
+00002aa0: 722c 0a20 2020 2020 2020 2063 6c61 7373  r,.        class
+00002ab0: 6573 3d4c 4142 454c 532c 0a20 2020 2020  es=LABELS,.     
+00002ac0: 2020 2064 6174 615f 6e61 6d65 5f6f 725f     data_name_or_
+00002ad0: 7061 7468 3d44 4154 4153 4554 2c0a 2020  path=DATASET,.  
+00002ae0: 2020 2020 2020 7072 6f6d 7074 5f63 6f6c        prompt_col
+00002af0: 5f6e 616d 653d 2270 726f 6d70 7422 2c0a  _name="prompt",.
+00002b00: 2020 2020 2020 2020 6c61 6265 6c5f 636f          label_co
+00002b10: 6c5f 6e61 6d65 3d22 6c61 6265 6c22 2c0a  l_name="label",.
+00002b20: 2020 2020 2020 2020 2a2a 7b0a 2020 2020          **{.    
+00002b30: 2020 2020 2020 2020 226e 756d 5f73 616d          "num_sam
+00002b40: 706c 6573 223a 2031 3030 302c 2020 2320  ples": 1000,  # 
+00002b50: 686f 7720 6d61 6e79 2073 616d 706c 6573  how many samples
+00002b60: 2077 696c 6c20 6265 2073 616d 706c 6564   will be sampled
+00002b70: 2074 6f20 6576 616c 7561 7469 6f6e 0a20   to evaluation. 
+00002b80: 2020 2020 2020 2020 2020 2022 7361 6d70             "samp
+00002b90: 6c65 5f6d 6178 5f6c 656e 223a 2031 3032  le_max_len": 102
+00002ba0: 342c 2020 2320 6d61 7820 746f 6b65 6e73  4,  # max tokens
+00002bb0: 2066 6f72 2065 6163 6820 7361 6d70 6c65   for each sample
+00002bc0: 0a20 2020 2020 2020 2020 2020 2022 626c  .            "bl
+00002bd0: 6f63 6b5f 6d61 785f 6c65 6e22 3a20 3230  ock_max_len": 20
+00002be0: 3438 2c20 2023 206d 6178 2074 6f6b 656e  48,  # max token
+00002bf0: 7320 666f 7220 6561 6368 2064 6174 6120  s for each data 
+00002c00: 626c 6f63 6b0a 2020 2020 2020 2020 2020  block.          
+00002c10: 2020 2320 6675 6e63 7469 6f6e 2074 6f20    # function to 
+00002c20: 6c6f 6164 2064 6174 6173 6574 2c20 6f6e  load dataset, on
+00002c30: 6520 6d75 7374 206f 6e6c 7920 6163 6365  e must only acce
+00002c40: 7074 2064 6174 615f 6e61 6d65 5f6f 725f  pt data_name_or_
+00002c50: 7061 7468 2061 7320 696e 7075 7420 0a20  path as input . 
+00002c60: 2020 2020 2020 2020 2020 2023 2061 6e64             # and
+00002c70: 2072 6574 7572 6e20 6461 7461 7365 7473   return datasets
+00002c80: 2e44 6174 6173 6574 0a20 2020 2020 2020  .Dataset.       
+00002c90: 2020 2020 2022 6c6f 6164 5f66 6e22 3a20       "load_fn": 
+00002ca0: 7061 7274 6961 6c28 6461 7461 7365 7473  partial(datasets
+00002cb0: 2e6c 6f61 645f 6461 7461 7365 742c 206e  .load_dataset, n
+00002cc0: 616d 653d 2265 6e67 6c69 7368 2229 2c20  ame="english"), 
+00002cd0: 200a 2020 2020 2020 2020 2020 2020 2320   .            # 
+00002ce0: 6675 6e63 7469 6f6e 2074 6f20 7072 6570  function to prep
+00002cf0: 726f 6365 7373 2064 6174 6173 6574 2c20  rocess dataset, 
+00002d00: 7768 6963 6820 6973 2075 7365 6420 666f  which is used fo
+00002d10: 7220 6461 7461 7365 7473 2e44 6174 6173  r datasets.Datas
+00002d20: 6574 2e6d 6170 2c20 0a20 2020 2020 2020  et.map, .       
+00002d30: 2020 2020 2023 206d 7573 7420 7265 7475       # must retu
+00002d40: 726e 2044 6963 745b 7374 722c 206c 6973  rn Dict[str, lis
+00002d50: 745d 2077 6974 6820 6f6e 6c79 2074 776f  t] with only two
+00002d60: 206b 6579 733a 205b 7072 6f6d 7074 5f63   keys: [prompt_c
+00002d70: 6f6c 5f6e 616d 652c 206c 6162 656c 5f63  ol_name, label_c
+00002d80: 6f6c 5f6e 616d 655d 0a20 2020 2020 2020  ol_name].       
+00002d90: 2020 2020 2022 7072 6570 726f 6365 7373       "preprocess
+00002da0: 5f66 6e22 3a20 6473 5f72 6566 6163 746f  _fn": ds_refacto
+00002db0: 725f 666e 2c20 200a 2020 2020 2020 2020  r_fn,  .        
+00002dc0: 2020 2020 2320 7472 756e 6361 7465 206c      # truncate l
+00002dd0: 6162 656c 2077 6865 6e20 7361 6d70 6c65  abel when sample
+00002de0: 2773 206c 656e 6774 6820 6578 6365 6564  's length exceed
+00002df0: 2073 616d 706c 655f 6d61 785f 6c65 6e0a   sample_max_len.
+00002e00: 2020 2020 2020 2020 2020 2020 2274 7275              "tru
+00002e10: 6e63 6174 655f 7072 6f6d 7074 223a 2046  ncate_prompt": F
+00002e20: 616c 7365 2020 0a20 2020 2020 2020 207d  alse  .        }
+00002e30: 0a20 2020 2029 0a0a 2320 6e6f 7465 2074  .    )..# note t
+00002e40: 6861 7420 6d61 785f 6e65 775f 746f 6b65  hat max_new_toke
+00002e50: 6e73 2077 696c 6c20 6265 2061 7574 6f6d  ns will be autom
+00002e60: 6174 6963 616c 6c79 2073 7065 6369 6669  atically specifi
+00002e70: 6564 2069 6e74 6572 6e61 6c6c 7920 6261  ed internally ba
+00002e80: 7365 6420 6f6e 2067 6976 656e 2063 6c61  sed on given cla
+00002e90: 7373 6573 0a70 7269 6e74 2874 6173 6b2e  sses.print(task.
+00002ea0: 7275 6e28 2929 0a0a 2320 7365 6c66 2d63  run())..# self-c
+00002eb0: 6f6e 7369 7374 656e 6379 0a70 7269 6e74  onsistency.print
+00002ec0: 280a 2020 2020 7461 736b 2e72 756e 280a  (.    task.run(.
+00002ed0: 2020 2020 2020 2020 6765 6e65 7261 7469          generati
+00002ee0: 6f6e 5f63 6f6e 6669 673d 4765 6e65 7261  on_config=Genera
+00002ef0: 7469 6f6e 436f 6e66 6967 280a 2020 2020  tionConfig(.    
+00002f00: 2020 2020 2020 2020 6e75 6d5f 6265 616d          num_beam
+00002f10: 733d 332c 0a20 2020 2020 2020 2020 2020  s=3,.           
+00002f20: 206e 756d 5f72 6574 7572 6e5f 7365 7175   num_return_sequ
+00002f30: 656e 6365 733d 332c 0a20 2020 2020 2020  ences=3,.       
+00002f40: 2020 2020 2064 6f5f 7361 6d70 6c65 3d54       do_sample=T
+00002f50: 7275 650a 2020 2020 2020 2020 290a 2020  rue.        ).  
+00002f60: 2020 290a 290a 6060 600a 0a3c 2f64 6574    ).).```..</det
+00002f70: 6169 6c73 3e0a 0a23 2320 4c65 6172 6e20  ails>..## Learn 
+00002f80: 4d6f 7265 0a5b 7475 746f 7269 616c 735d  More.[tutorials]
+00002f90: 2864 6f63 732f 7475 746f 7269 616c 2920  (docs/tutorial) 
+00002fa0: 7072 6f76 6964 6520 7374 6570 2d62 792d  provide step-by-
+00002fb0: 7374 6570 2067 7569 6461 6e63 6520 746f  step guidance to
+00002fc0: 2069 6e74 6567 7261 7465 2060 6175 746f   integrate `auto
+00002fd0: 5f67 7074 7160 2077 6974 6820 796f 7572  _gptq` with your
+00002fe0: 206f 776e 2070 726f 6a65 6374 2061 6e64   own project and
+00002ff0: 2073 6f6d 6520 6265 7374 2070 7261 6374   some best pract
+00003000: 6963 6520 7072 696e 6369 706c 6573 2e0a  ice principles..
+00003010: 0a5b 6578 616d 706c 6573 5d28 6578 616d  .[examples](exam
+00003020: 706c 6573 2f52 4541 444d 452e 6d64 2920  ples/README.md) 
+00003030: 7072 6f76 6964 6520 706c 656e 7479 206f  provide plenty o
+00003040: 6620 6578 616d 706c 6520 7363 7269 7074  f example script
+00003050: 7320 746f 2075 7365 2060 6175 746f 5f67  s to use `auto_g
+00003060: 7074 7160 2069 6e20 6469 6666 6572 656e  ptq` in differen
+00003070: 7420 7761 7973 2e0a 0a23 2320 5375 7070  t ways...## Supp
+00003080: 6f72 7465 6420 4d6f 6465 6c73 0a0a 3e20  orted Models..> 
+00003090: 796f 7520 6361 6e20 7573 6520 606d 6f64  you can use `mod
+000030a0: 656c 2e63 6f6e 6669 672e 6d6f 6465 6c5f  el.config.model_
+000030b0: 7479 7065 6020 746f 2063 6f6d 7061 7265  type` to compare
+000030c0: 2077 6974 6820 7468 6520 7461 626c 6520   with the table 
+000030d0: 6265 6c6f 7720 746f 2063 6865 636b 2077  below to check w
+000030e0: 6865 7468 6572 2074 6865 206d 6f64 656c  hether the model
+000030f0: 2079 6f75 2075 7365 2069 7320 7375 7070   you use is supp
+00003100: 6f72 7465 6420 6279 2060 6175 746f 5f67  orted by `auto_g
+00003110: 7074 7160 2e0a 3e20 0a3e 2066 6f72 2065  ptq`..> .> for e
+00003120: 7861 6d70 6c65 2c20 6d6f 6465 6c5f 7479  xample, model_ty
+00003130: 7065 206f 6620 6057 697a 6172 644c 4d60  pe of `WizardLM`
+00003140: 2c20 6076 6963 756e 6160 2061 6e64 2060  , `vicuna` and `
+00003150: 6770 7434 616c 6c60 2061 7265 2061 6c6c  gpt4all` are all
+00003160: 2060 6c6c 616d 6160 2c20 6865 6e63 6520   `llama`, hence 
+00003170: 7468 6579 2061 7265 2061 6c6c 2073 7570  they are all sup
+00003180: 706f 7274 6564 2062 7920 6061 7574 6f5f  ported by `auto_
+00003190: 6770 7471 602e 0a0a 7c20 6d6f 6465 6c20  gptq`...| model 
+000031a0: 7479 7065 2020 2020 2020 2020 2020 2020  type            
+000031b0: 2020 2020 2020 2020 2020 2020 207c 2071               | q
+000031c0: 7561 6e74 697a 6174 696f 6e20 7c20 696e  uantization | in
+000031d0: 6665 7265 6e63 6520 7c20 7065 6674 2d6c  ference | peft-l
+000031e0: 6f72 6120 7c20 7065 6674 2d61 6461 2d6c  ora | peft-ada-l
+000031f0: 6f72 6120 7c20 7065 6674 2d61 6461 7074  ora | peft-adapt
+00003200: 696f 6e5f 7072 6f6d 7074 2020 2020 2020  ion_prompt      
+00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003230: 2020 2020 2020 7c20 7175 616e 7469 7a61        | quantiza
-00003240: 7469 6f6e 207c 2069 6e66 6572 656e 6365  tion | inference
-00003250: 207c 2070 6566 742d 6c6f 7261 207c 2070   | peft-lora | p
-00003260: 6566 742d 6164 612d 6c6f 7261 207c 2070  eft-ada-lora | p
-00003270: 6566 742d 6164 6170 7469 6f6e 5f70 726f  eft-adaption_pro
-00003280: 6d70 7420 2020 2020 2020 2020 2020 2020  mpt             
-00003290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032c0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000032d0: 0d0a 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..|-------------
+00003230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003250: 2020 2020 2020 7c0a 7c2d 2d2d 2d2d 2d2d        |.|-------
+00003260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 2d2d  -------------|--
+00003280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d  ------------|---
+00003290: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
+000032a0: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
+000032b0: 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----|-----------
+000032c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000032d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 000032e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000032f0: 2d2d 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d  -------|--------
-00003300: 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d  ------|---------
-00003310: 2d2d 7c2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --|-----------|-
-00003320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d  --------------|-
-00003330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003390: 7c0d 0a7c 2062 6c6f 6f6d 2020 2020 2020  |..| bloom      
+000032f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003310: 2d2d 2d2d 2d2d 7c0a 7c20 626c 6f6f 6d20  ------|.| bloom 
+00003320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003330: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+00003340: 9c85 2020 2020 2020 2020 2020 2020 7c20  ..            | 
+00003350: e29c 8520 2020 2020 2020 2020 7c20 e29c  ...         | ..
+00003360: 8520 2020 2020 2020 2020 7c20 e29c 8520  .         | ... 
+00003370: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00003380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003390: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033b0: 2020 2020 2020 2020 7c20 e29c 8520 2020          | ...   
-000033c0: 2020 2020 2020 2020 207c 20e2 9c85 2020           | ...  
-000033d0: 2020 2020 2020 207c 20e2 9c85 2020 2020         | ...    
-000033e0: 2020 2020 207c 20e2 9c85 2020 2020 2020       | ...      
-000033f0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00003400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003450: 2020 2020 2020 2020 207c 0d0a 7c20 6770           |..| gp
-00003460: 7432 2020 2020 2020 2020 2020 2020 2020  t2              
+000033b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033d0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+000033e0: 7c20 6770 7432 2020 2020 2020 2020 2020  | gpt2          
+000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003400: 2020 2020 207c 20e2 9c85 2020 2020 2020       | ...      
+00003410: 2020 2020 2020 7c20 e29c 8520 2020 2020        | ...     
+00003420: 2020 2020 7c20 e29c 8520 2020 2020 2020      | ...       
+00003430: 2020 7c20 e29c 8520 2020 2020 2020 2020    | ...         
+00003440: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00003450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003480: 207c 20e2 9c85 2020 2020 2020 2020 2020   | ...          
-00003490: 2020 7c20 e29c 8520 2020 2020 2020 2020    | ...         
-000034a0: 7c20 e29c 8520 2020 2020 2020 2020 7c20  | ...         | 
-000034b0: e29c 8520 2020 2020 2020 2020 2020 2020  ...             
-000034c0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000034d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 2020 7c0d 0a7c 2067 7074 5f6e 656f 7820    |..| gpt_neox 
-00003530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003540: 2020 2020 2020 2020 2020 7c20 e29c 8520            | ... 
-00003550: 2020 2020 2020 2020 2020 207c 20e2 9c85             | ...
-00003560: 2020 2020 2020 2020 207c 20e2 9c85 2020           | ...  
-00003570: 2020 2020 2020 207c 20e2 9c85 2020 2020         | ...    
-00003580: 2020 2020 2020 2020 207c 20e2 9c85 5b72           | ...[r
-00003590: 6571 7569 7265 7320 7468 6973 2070 6566  equires this pef
-000035a0: 7420 6272 616e 6368 5d28 6874 7470 733a  t branch](https:
-000035b0: 2f2f 6769 7468 7562 2e63 6f6d 2f50 616e  //github.com/Pan
-000035c0: 5169 5765 692f 7065 6674 2f74 7265 652f  QiWei/peft/tree/
-000035d0: 6d75 6c74 695f 6d6f 6461 6c5f 6164 6170  multi_modal_adap
-000035e0: 7469 6f6e 5f70 726f 6d70 7429 207c 0d0a  tion_prompt) |..
-000035f0: 7c20 6770 746a 2020 2020 2020 2020 2020  | gptj          
-00003600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003610: 2020 2020 207c 20e2 9c85 2020 2020 2020       | ...      
-00003620: 2020 2020 2020 7c20 e29c 8520 2020 2020        | ...     
-00003630: 2020 2020 7c20 e29c 8520 2020 2020 2020      | ...       
-00003640: 2020 7c20 e29c 8520 2020 2020 2020 2020    | ...         
-00003650: 2020 2020 7c20 e29c 855b 7265 7175 6972      | ...[requir
-00003660: 6573 2074 6869 7320 7065 6674 2062 7261  es this peft bra
-00003670: 6e63 685d 2868 7474 7073 3a2f 2f67 6974  nch](https://git
-00003680: 6875 622e 636f 6d2f 5061 6e51 6957 6569  hub.com/PanQiWei
-00003690: 2f70 6566 742f 7472 6565 2f6d 756c 7469  /peft/tree/multi
-000036a0: 5f6d 6f64 616c 5f61 6461 7074 696f 6e5f  _modal_adaption_
-000036b0: 7072 6f6d 7074 2920 7c0d 0a7c 206c 6c61  prompt) |..| lla
-000036c0: 6d61 2020 2020 2020 2020 2020 2020 2020  ma              
+00003480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034a0: 2020 2020 2020 7c0a 7c20 6770 745f 6e65        |.| gpt_ne
+000034b0: 6f78 2020 2020 2020 2020 2020 2020 2020  ox              
+000034c0: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+000034d0: 9c85 2020 2020 2020 2020 2020 2020 7c20  ..            | 
+000034e0: e29c 8520 2020 2020 2020 2020 7c20 e29c  ...         | ..
+000034f0: 8520 2020 2020 2020 2020 7c20 e29c 8520  .         | ... 
+00003500: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
+00003510: 855b 7265 7175 6972 6573 2074 6869 7320  .[requires this 
+00003520: 7065 6674 2062 7261 6e63 685d 2868 7474  peft branch](htt
+00003530: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00003540: 5061 6e51 6957 6569 2f70 6566 742f 7472  PanQiWei/peft/tr
+00003550: 6565 2f6d 756c 7469 5f6d 6f64 616c 5f61  ee/multi_modal_a
+00003560: 6461 7074 696f 6e5f 7072 6f6d 7074 2920  daption_prompt) 
+00003570: 7c0a 7c20 6770 746a 2020 2020 2020 2020  |.| gptj        
+00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003590: 2020 2020 2020 207c 20e2 9c85 2020 2020         | ...    
+000035a0: 2020 2020 2020 2020 7c20 e29c 8520 2020          | ...   
+000035b0: 2020 2020 2020 7c20 e29c 8520 2020 2020        | ...     
+000035c0: 2020 2020 7c20 e29c 8520 2020 2020 2020      | ...       
+000035d0: 2020 2020 2020 7c20 e29c 855b 7265 7175        | ...[requ
+000035e0: 6972 6573 2074 6869 7320 7065 6674 2062  ires this peft b
+000035f0: 7261 6e63 685d 2868 7474 7073 3a2f 2f67  ranch](https://g
+00003600: 6974 6875 622e 636f 6d2f 5061 6e51 6957  ithub.com/PanQiW
+00003610: 6569 2f70 6566 742f 7472 6565 2f6d 756c  ei/peft/tree/mul
+00003620: 7469 5f6d 6f64 616c 5f61 6461 7074 696f  ti_modal_adaptio
+00003630: 6e5f 7072 6f6d 7074 2920 7c0a 7c20 6c6c  n_prompt) |.| ll
+00003640: 616d 6120 2020 2020 2020 2020 2020 2020  ama             
+00003650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003660: 207c 20e2 9c85 2020 2020 2020 2020 2020   | ...          
+00003670: 2020 7c20 e29c 8520 2020 2020 2020 2020    | ...         
+00003680: 7c20 e29c 8520 2020 2020 2020 2020 7c20  | ...         | 
+00003690: e29c 8520 2020 2020 2020 2020 2020 2020  ...             
+000036a0: 7c20 e29c 8520 2020 2020 2020 2020 2020  | ...           
+000036b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000036d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036e0: 7c20 e29c 8520 2020 2020 2020 2020 2020  | ...           
-000036f0: 207c 20e2 9c85 2020 2020 2020 2020 207c   | ...         |
-00003700: 20e2 9c85 2020 2020 2020 2020 207c 20e2   ...         | .
-00003710: 9c85 2020 2020 2020 2020 2020 2020 207c  ..             |
-00003720: 20e2 9c85 2020 2020 2020 2020 2020 2020   ...            
-00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003780: 2020 207c 0d0a 7c20 6d6f 7373 2020 2020     |..| moss    
-00003790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037a0: 2020 2020 2020 2020 2020 207c 20e2 9c85             | ...
-000037b0: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
-000037c0: 8520 2020 2020 2020 2020 7c20 e29c 8520  .         | ... 
-000037d0: 2020 2020 2020 2020 7c20 e29c 8520 2020          | ...   
-000037e0: 2020 2020 2020 2020 2020 7c20 e29c 855b            | ...[
-000037f0: 7265 7175 6972 6573 2074 6869 7320 7065  requires this pe
-00003800: 6674 2062 7261 6e63 685d 2868 7474 7073  ft branch](https
-00003810: 3a2f 2f67 6974 6875 622e 636f 6d2f 5061  ://github.com/Pa
-00003820: 6e51 6957 6569 2f70 6566 742f 7472 6565  nQiWei/peft/tree
-00003830: 2f6d 756c 7469 5f6d 6f64 616c 5f61 6461  /multi_modal_ada
-00003840: 7074 696f 6e5f 7072 6f6d 7074 2920 7c0d  ption_prompt) |.
-00003850: 0a7c 206f 7074 2020 2020 2020 2020 2020  .| opt          
+000036e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003700: 2020 2020 7c0a 7c20 6d6f 7373 2020 2020      |.| moss    
+00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003720: 2020 2020 2020 2020 2020 207c 20e2 9c85             | ...
+00003730: 2020 2020 2020 2020 2020 2020 7c20 e29c              | ..
+00003740: 8520 2020 2020 2020 2020 7c20 e29c 8520  .         | ... 
+00003750: 2020 2020 2020 2020 7c20 e29c 8520 2020          | ...   
+00003760: 2020 2020 2020 2020 2020 7c20 e29c 855b            | ...[
+00003770: 7265 7175 6972 6573 2074 6869 7320 7065  requires this pe
+00003780: 6674 2062 7261 6e63 685d 2868 7474 7073  ft branch](https
+00003790: 3a2f 2f67 6974 6875 622e 636f 6d2f 5061  ://github.com/Pa
+000037a0: 6e51 6957 6569 2f70 6566 742f 7472 6565  nQiWei/peft/tree
+000037b0: 2f6d 756c 7469 5f6d 6f64 616c 5f61 6461  /multi_modal_ada
+000037c0: 7074 696f 6e5f 7072 6f6d 7074 2920 7c0a  ption_prompt) |.
+000037d0: 7c20 6f70 7420 2020 2020 2020 2020 2020  | opt           
+000037e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037f0: 2020 2020 207c 20e2 9c85 2020 2020 2020       | ...      
+00003800: 2020 2020 2020 7c20 e29c 8520 2020 2020        | ...     
+00003810: 2020 2020 7c20 e29c 8520 2020 2020 2020      | ...       
+00003820: 2020 7c20 e29c 8520 2020 2020 2020 2020    | ...         
+00003830: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003870: 2020 2020 2020 7c20 e29c 8520 2020 2020        | ...     
-00003880: 2020 2020 2020 207c 20e2 9c85 2020 2020         | ...    
-00003890: 2020 2020 207c 20e2 9c85 2020 2020 2020       | ...      
-000038a0: 2020 207c 20e2 9c85 2020 2020 2020 2020     | ...        
-000038b0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003890: 2020 2020 2020 7c0a 7c20 6770 745f 6269        |.| gpt_bi
+000038a0: 6763 6f64 6520 2020 2020 2020 2020 2020  gcode           
+000038b0: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+000038c0: 9c85 2020 2020 2020 2020 2020 2020 7c20  ..            | 
+000038d0: e29c 8520 2020 2020 2020 2020 7c20 e29c  ...         | ..
+000038e0: 8520 2020 2020 2020 2020 7c20 e29c 8520  .         | ... 
+000038f0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 00003900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003910: 2020 2020 2020 207c 0d0a 7c20 6770 745f         |..| gpt_
-00003920: 6269 6763 6f64 6520 2020 2020 2020 2020  bigcode         
-00003930: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00003940: 20e2 9c85 2020 2020 2020 2020 2020 2020   ...            
-00003950: 7c20 e29c 8520 2020 2020 2020 2020 7c20  | ...         | 
-00003960: e29c 8520 2020 2020 2020 2020 7c20 e29c  ...         | ..
-00003970: 8520 2020 2020 2020 2020 2020 2020 7c20  .             | 
-00003980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003950: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00003960: 7c20 636f 6465 6765 6e20 2020 2020 2020  | codegen       
+00003970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003980: 2020 2020 207c 20e2 9c85 2020 2020 2020       | ...      
+00003990: 2020 2020 2020 7c20 e29c 8520 2020 2020        | ...     
+000039a0: 2020 2020 7c20 e29c 8520 2020 2020 2020      | ...       
+000039b0: 2020 7c20 e29c 8520 2020 2020 2020 2020    | ...         
+000039c0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
 000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039e0: 7c0d 0a7c 2063 6f64 6567 656e 2020 2020  |..| codegen    
+000039e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000039f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a00: 2020 2020 2020 2020 7c20 e29c 8520 2020          | ...   
-00003a10: 2020 2020 2020 2020 207c 20e2 9c85 2020           | ...  
-00003a20: 2020 2020 2020 207c 20e2 9c85 2020 2020         | ...    
-00003a30: 2020 2020 207c 20e2 9c85 2020 2020 2020       | ...      
-00003a40: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a20: 2020 2020 2020 7c0a 7c20 6661 6c63 6f6e        |.| falcon
+00003a30: 2852 6566 696e 6564 5765 624d 6f64 656c  (RefinedWebModel
+00003a40: 2f52 6566 696e 6564 5765 6229 207c 20e2  /RefinedWeb) | .
+00003a50: 9c85 2020 2020 2020 2020 2020 2020 7c20  ..            | 
+00003a60: e29c 8520 2020 2020 2020 2020 7c20 e29c  ...         | ..
+00003a70: 8520 2020 2020 2020 2020 7c20 e29c 8520  .         | ... 
+00003a80: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 00003a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003aa0: 2020 2020 2020 2020 207c 0d0a 7c20 6661           |..| fa
-00003ab0: 6c63 6f6e 2852 6566 696e 6564 5765 624d  lcon(RefinedWebM
-00003ac0: 6f64 656c 2f52 6566 696e 6564 5765 6229  odel/RefinedWeb)
-00003ad0: 207c 20e2 9c85 2020 2020 2020 2020 2020   | ...          
-00003ae0: 2020 7c20 e29c 8520 2020 2020 2020 2020    | ...         
-00003af0: 7c20 e29c 8520 2020 2020 2020 2020 7c20  | ...         | 
-00003b00: e29c 8520 2020 2020 2020 2020 2020 2020  ...             
-00003b10: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00003b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b70: 2020 7c0d 0a0d 0a23 2320 5375 7070 6f72    |....## Suppor
-00003b80: 7465 6420 4576 616c 7561 7469 6f6e 2054  ted Evaluation T
-00003b90: 6173 6b73 0d0a 4375 7272 656e 746c 792c  asks..Currently,
-00003ba0: 2060 6175 746f 5f67 7074 7160 2073 7570   `auto_gptq` sup
-00003bb0: 706f 7274 733a 2060 4c61 6e67 7561 6765  ports: `Language
-00003bc0: 4d6f 6465 6c69 6e67 5461 736b 602c 2060  ModelingTask`, `
-00003bd0: 5365 7175 656e 6365 436c 6173 7369 6669  SequenceClassifi
-00003be0: 6361 7469 6f6e 5461 736b 6020 616e 6420  cationTask` and 
-00003bf0: 6054 6578 7453 756d 6d61 7269 7a61 7469  `TextSummarizati
-00003c00: 6f6e 5461 736b 603b 206d 6f72 6520 5461  onTask`; more Ta
-00003c10: 736b 7320 7769 6c6c 2063 6f6d 6520 736f  sks will come so
-00003c20: 6f6e 210d 0a0d 0a23 2320 4163 6b6e 6f77  on!....## Acknow
-00003c30: 6c65 6467 656d 656e 740d 0a2d 2053 7065  ledgement..- Spe
-00003c40: 6369 616c 6c79 2074 6861 6e6b 7320 2a2a  cially thanks **
-00003c50: 456c 6961 7320 4672 616e 7461 722a 2a2c  Elias Frantar**,
-00003c60: 202a 2a53 616c 6568 2041 7368 6b62 6f6f   **Saleh Ashkboo
-00003c70: 732a 2a2c 202a 2a54 6f72 7374 656e 2048  s**, **Torsten H
-00003c80: 6f65 666c 6572 2a2a 2061 6e64 202a 2a44  oefler** and **D
-00003c90: 616e 2041 6c69 7374 6172 682a 2a20 666f  an Alistarh** fo
-00003ca0: 7220 7072 6f70 6f73 696e 6720 2a2a 4750  r proposing **GP
-00003cb0: 5451 2a2a 2061 6c67 6f72 6974 686d 2061  TQ** algorithm a
-00003cc0: 6e64 206f 7065 6e20 736f 7572 6365 2074  nd open source t
-00003cd0: 6865 205b 636f 6465 5d28 6874 7470 733a  he [code](https:
-00003ce0: 2f2f 6769 7468 7562 2e63 6f6d 2f49 5354  //github.com/IST
-00003cf0: 2d44 4153 4c61 622f 6770 7471 292e 0d0a  -DASLab/gptq)...
-00003d00: 2d20 5370 6563 6961 6c6c 7920 7468 616e  - Specially than
-00003d10: 6b73 202a 2a71 776f 7071 776f 7032 3030  ks **qwopqwop200
-00003d20: 2a2a 2c20 666f 7220 636f 6465 2069 6e20  **, for code in 
-00003d30: 7468 6973 2070 726f 6a65 6374 2074 6861  this project tha
-00003d40: 7420 7265 6c65 7661 6e74 2074 6f20 7175  t relevant to qu
-00003d50: 616e 7469 7a61 7469 6f6e 2061 7265 206d  antization are m
-00003d60: 6169 6e6c 7920 7265 6665 7265 6e63 6564  ainly referenced
-00003d70: 2066 726f 6d20 5b47 5054 512d 666f 722d   from [GPTQ-for-
-00003d80: 4c4c 614d 615d 2868 7474 7073 3a2f 2f67  LLaMa](https://g
-00003d90: 6974 6875 622e 636f 6d2f 7177 6f70 7177  ithub.com/qwopqw
-00003da0: 6f70 3230 302f 4750 5451 2d66 6f72 2d4c  op200/GPTQ-for-L
-00003db0: 4c61 4d61 2f74 7265 652f 6375 6461 292e  LaMa/tree/cuda).
-00003dc0: 0d0a 0d0a 0d0a 5b21 5b53 7461 7220 4869  ......[![Star Hi
-00003dd0: 7374 6f72 7920 4368 6172 745d 2868 7474  story Chart](htt
-00003de0: 7073 3a2f 2f61 7069 2e73 7461 722d 6869  ps://api.star-hi
-00003df0: 7374 6f72 792e 636f 6d2f 7376 673f 7265  story.com/svg?re
-00003e00: 706f 733d 5061 6e51 6977 6569 2f41 7574  pos=PanQiwei/Aut
-00003e10: 6f47 5054 5126 7479 7065 3d44 6174 6529  oGPTQ&type=Date)
-00003e20: 5d28 6874 7470 733a 2f2f 7374 6172 2d68  ](https://star-h
-00003e30: 6973 746f 7279 2e63 6f6d 2f23 5061 6e51  istory.com/#PanQ
-00003e40: 6957 6569 2f41 7574 6f47 5054 5126 4461  iWei/AutoGPTQ&Da
-00003e50: 7465 29                                  te)
+00003aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00003af0: 0a23 2320 5375 7070 6f72 7465 6420 4576  .## Supported Ev
+00003b00: 616c 7561 7469 6f6e 2054 6173 6b73 0a43  aluation Tasks.C
+00003b10: 7572 7265 6e74 6c79 2c20 6061 7574 6f5f  urrently, `auto_
+00003b20: 6770 7471 6020 7375 7070 6f72 7473 3a20  gptq` supports: 
+00003b30: 604c 616e 6775 6167 654d 6f64 656c 696e  `LanguageModelin
+00003b40: 6754 6173 6b60 2c20 6053 6571 7565 6e63  gTask`, `Sequenc
+00003b50: 6543 6c61 7373 6966 6963 6174 696f 6e54  eClassificationT
+00003b60: 6173 6b60 2061 6e64 2060 5465 7874 5375  ask` and `TextSu
+00003b70: 6d6d 6172 697a 6174 696f 6e54 6173 6b60  mmarizationTask`
+00003b80: 3b20 6d6f 7265 2054 6173 6b73 2077 696c  ; more Tasks wil
+00003b90: 6c20 636f 6d65 2073 6f6f 6e21 0a0a 2323  l come soon!..##
+00003ba0: 2041 636b 6e6f 776c 6564 6765 6d65 6e74   Acknowledgement
+00003bb0: 0a2d 2053 7065 6369 616c 6c79 2074 6861  .- Specially tha
+00003bc0: 6e6b 7320 2a2a 456c 6961 7320 4672 616e  nks **Elias Fran
+00003bd0: 7461 722a 2a2c 202a 2a53 616c 6568 2041  tar**, **Saleh A
+00003be0: 7368 6b62 6f6f 732a 2a2c 202a 2a54 6f72  shkboos**, **Tor
+00003bf0: 7374 656e 2048 6f65 666c 6572 2a2a 2061  sten Hoefler** a
+00003c00: 6e64 202a 2a44 616e 2041 6c69 7374 6172  nd **Dan Alistar
+00003c10: 682a 2a20 666f 7220 7072 6f70 6f73 696e  h** for proposin
+00003c20: 6720 2a2a 4750 5451 2a2a 2061 6c67 6f72  g **GPTQ** algor
+00003c30: 6974 686d 2061 6e64 206f 7065 6e20 736f  ithm and open so
+00003c40: 7572 6365 2074 6865 205b 636f 6465 5d28  urce the [code](
+00003c50: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003c60: 6f6d 2f49 5354 2d44 4153 4c61 622f 6770  om/IST-DASLab/gp
+00003c70: 7471 292e 0a2d 2053 7065 6369 616c 6c79  tq)..- Specially
+00003c80: 2074 6861 6e6b 7320 2a2a 7177 6f70 7177   thanks **qwopqw
+00003c90: 6f70 3230 302a 2a2c 2066 6f72 2063 6f64  op200**, for cod
+00003ca0: 6520 696e 2074 6869 7320 7072 6f6a 6563  e in this projec
+00003cb0: 7420 7468 6174 2072 656c 6576 616e 7420  t that relevant 
+00003cc0: 746f 2071 7561 6e74 697a 6174 696f 6e20  to quantization 
+00003cd0: 6172 6520 6d61 696e 6c79 2072 6566 6572  are mainly refer
+00003ce0: 656e 6365 6420 6672 6f6d 205b 4750 5451  enced from [GPTQ
+00003cf0: 2d66 6f72 2d4c 4c61 4d61 5d28 6874 7470  -for-LLaMa](http
+00003d00: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f71  s://github.com/q
+00003d10: 776f 7071 776f 7032 3030 2f47 5054 512d  wopqwop200/GPTQ-
+00003d20: 666f 722d 4c4c 614d 612f 7472 6565 2f63  for-LLaMa/tree/c
+00003d30: 7564 6129 2e0a 0a0a 5b21 5b53 7461 7220  uda)....[![Star 
+00003d40: 4869 7374 6f72 7920 4368 6172 745d 2868  History Chart](h
+00003d50: 7474 7073 3a2f 2f61 7069 2e73 7461 722d  ttps://api.star-
+00003d60: 6869 7374 6f72 792e 636f 6d2f 7376 673f  history.com/svg?
+00003d70: 7265 706f 733d 5061 6e51 6977 6569 2f41  repos=PanQiwei/A
+00003d80: 7574 6f47 5054 5126 7479 7065 3d44 6174  utoGPTQ&type=Dat
+00003d90: 6529 5d28 6874 7470 733a 2f2f 7374 6172  e)](https://star
+00003da0: 2d68 6973 746f 7279 2e63 6f6d 2f23 5061  -history.com/#Pa
+00003db0: 6e51 6957 6569 2f41 7574 6f47 5054 5126  nQiWei/AutoGPTQ&
+00003dc0: 4461 7465 29                             Date)
```

### Comparing `auto_gptq-0.3.0/auto_gptq/eval_tasks/_base.py` & `auto_gptq-0.3.1/auto_gptq/eval_tasks/_base.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from abc import abstractmethod
-from typing import Any, Dict, List, Optional, Union
-
-import torch
-from transformers import PreTrainedTokenizer, PreTrainedModel
-
-from ..modeling import BaseGPTQForCausalLM
-from ..utils.data_utils import get_dataloader
-
-
-class BaseTask:
-    def __init__(
-        self,
-        model: Union[BaseGPTQForCausalLM, PreTrainedModel],
-        tokenizer: PreTrainedTokenizer,
-        data_name_or_path: str,
-        prompt_col_name: str,
-        label_col_name: str,
-        device: Optional[str] = None,
-        **kwargs
-    ):
-        self.model = model
-        self.tokenizer = tokenizer
-        if self.tokenizer.pad_token_id is None:
-            self.tokenizer.pad_token = self.tokenizer.eos_token
-            self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
-            self.model.config.pad_token_id = self.tokenizer.eos_token_id
-        self.dl = get_dataloader(
-            data_name_or_path,
-            prompt_col_name=prompt_col_name,
-            label_col_name=label_col_name,
-            tokenizer=tokenizer,
-            **kwargs
-        )
-
-        self.device = device
-        if not self.device:
-            self.device = self.model.device
-        if isinstance(self.device, str):
-            self.device = torch.device(self.device)
-
-    @abstractmethod
-    def _predict(self, batch_data: Dict[str, Any], **kwargs) -> List[Any]:
-        pass
-
-    @abstractmethod
-    def _parse_labels(self, label_ids: torch.LongTensor) -> List[Any]:
-        pass
-
-    @abstractmethod
-    def _metric(self, pred: List[Any], label: List[Any]) -> Dict[str, float]:
-        pass
-
-    def run(self, **predict_kwargs) -> Dict[str, float]:
-        with torch.inference_mode(), torch.amp.autocast(device_type=self.device.type):
-            predictions = []
-            labels = []
-            for batch_data in self.dl:
-                for k, v in batch_data.items():
-                    if isinstance(v, torch.Tensor):
-                        batch_data[k] = v.to(self.device)
-                labels += self._parse_labels(batch_data["labels"])
-                predictions += self._predict(batch_data, **predict_kwargs)
-
-        return self._metric(predictions, labels)
+from abc import abstractmethod
+from typing import Any, Dict, List, Optional, Union
+
+import torch
+from transformers import PreTrainedTokenizer, PreTrainedModel
+
+from ..modeling import BaseGPTQForCausalLM
+from ..utils.data_utils import get_dataloader
+
+
+class BaseTask:
+    def __init__(
+        self,
+        model: Union[BaseGPTQForCausalLM, PreTrainedModel],
+        tokenizer: PreTrainedTokenizer,
+        data_name_or_path: str,
+        prompt_col_name: str,
+        label_col_name: str,
+        device: Optional[str] = None,
+        **kwargs
+    ):
+        self.model = model
+        self.tokenizer = tokenizer
+        if self.tokenizer.pad_token_id is None:
+            self.tokenizer.pad_token = self.tokenizer.eos_token
+            self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
+            self.model.config.pad_token_id = self.tokenizer.eos_token_id
+        self.dl = get_dataloader(
+            data_name_or_path,
+            prompt_col_name=prompt_col_name,
+            label_col_name=label_col_name,
+            tokenizer=tokenizer,
+            **kwargs
+        )
+
+        self.device = device
+        if not self.device:
+            self.device = self.model.device
+        if isinstance(self.device, str):
+            self.device = torch.device(self.device)
+
+    @abstractmethod
+    def _predict(self, batch_data: Dict[str, Any], **kwargs) -> List[Any]:
+        pass
+
+    @abstractmethod
+    def _parse_labels(self, label_ids: torch.LongTensor) -> List[Any]:
+        pass
+
+    @abstractmethod
+    def _metric(self, pred: List[Any], label: List[Any]) -> Dict[str, float]:
+        pass
+
+    def run(self, **predict_kwargs) -> Dict[str, float]:
+        with torch.inference_mode(), torch.amp.autocast(device_type=self.device.type):
+            predictions = []
+            labels = []
+            for batch_data in self.dl:
+                for k, v in batch_data.items():
+                    if isinstance(v, torch.Tensor):
+                        batch_data[k] = v.to(self.device)
+                labels += self._parse_labels(batch_data["labels"])
+                predictions += self._predict(batch_data, **predict_kwargs)
+
+        return self._metric(predictions, labels)
```

### Comparing `auto_gptq-0.3.0/auto_gptq/eval_tasks/_utils/classification_utils.py` & `auto_gptq-0.3.1/auto_gptq/eval_tasks/_utils/classification_utils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import sys
-from typing import List, Sequence
-
-import numpy as np
-
-
-def levenshtein_distance(seq1: Sequence, seq2: Sequence):
-    if seq1 == seq2:
-        return 0
-    num_rows = len(seq1) + 1
-    num_cols = len(seq2) + 1
-    dp_matrix = np.empty((num_rows, num_cols))
-    dp_matrix[0, :] = range(num_cols)
-    dp_matrix[:, 0] = range(num_rows)
-
-    for i in range(1, num_rows):
-        for j in range(1, num_cols):
-            if seq1[i - 1] == seq2[j - 1]:
-                dp_matrix[i, j] = dp_matrix[i - 1, j - 1]
-            else:
-                dp_matrix[i, j] = min(dp_matrix[i - 1, j - 1], dp_matrix[i - 1, j], dp_matrix[i, j - 1]) + 1
-
-    return dp_matrix[num_rows - 1, num_cols - 1]
-
-
-def get_closest_label(pred: Sequence, classes: List[Sequence]) -> int:
-    min_id = sys.maxsize
-    min_edit_distance = sys.maxsize
-    for i, class_label in enumerate(classes):
-        edit_distance = levenshtein_distance(pred, class_label)
-        if edit_distance < min_edit_distance:
-            min_id = i
-            min_edit_distance = edit_distance
-    return min_id
-
-
-__all__ = ["levenshtein_distance", "get_closest_label"]
+import sys
+from typing import List, Sequence
+
+import numpy as np
+
+
+def levenshtein_distance(seq1: Sequence, seq2: Sequence):
+    if seq1 == seq2:
+        return 0
+    num_rows = len(seq1) + 1
+    num_cols = len(seq2) + 1
+    dp_matrix = np.empty((num_rows, num_cols))
+    dp_matrix[0, :] = range(num_cols)
+    dp_matrix[:, 0] = range(num_rows)
+
+    for i in range(1, num_rows):
+        for j in range(1, num_cols):
+            if seq1[i - 1] == seq2[j - 1]:
+                dp_matrix[i, j] = dp_matrix[i - 1, j - 1]
+            else:
+                dp_matrix[i, j] = min(dp_matrix[i - 1, j - 1], dp_matrix[i - 1, j], dp_matrix[i, j - 1]) + 1
+
+    return dp_matrix[num_rows - 1, num_cols - 1]
+
+
+def get_closest_label(pred: Sequence, classes: List[Sequence]) -> int:
+    min_id = sys.maxsize
+    min_edit_distance = sys.maxsize
+    for i, class_label in enumerate(classes):
+        edit_distance = levenshtein_distance(pred, class_label)
+        if edit_distance < min_edit_distance:
+            min_id = i
+            min_edit_distance = edit_distance
+    return min_id
+
+
+__all__ = ["levenshtein_distance", "get_closest_label"]
```

### Comparing `auto_gptq-0.3.0/auto_gptq/eval_tasks/_utils/generation_utils.py` & `auto_gptq-0.3.1/auto_gptq/eval_tasks/_utils/generation_utils.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import List, Optional, Union
-
-from torch import LongTensor
-from transformers import PreTrainedTokenizer
-
-
-def postprocess_generation_ids(
-    input_ids: LongTensor,
-    output_ids: LongTensor,
-    num_return_sequences: int,
-    tokenizer: Optional[PreTrainedTokenizer] = None,
-    pad_token_ids: Optional[int] = None,
-) -> List[List[Union[str, List[int]]]]:
-    outputs = []
-    for idx, start in enumerate(range(0, len(output_ids), num_return_sequences)):
-        sub_output_ids = output_ids[start: start + num_return_sequences]
-        sub_generated_ids = sub_output_ids[..., input_ids[idx].size(0):]
-        if tokenizer:
-            outputs.append(
-                [
-                    generated_text for generated_text in tokenizer.batch_decode(
-                        sub_generated_ids,
-                        clean_up_tokenization_spaces=True
-                    )
-                ]
-            )
-        else:
-            sub_generated_ids = sub_output_ids.cpu().numpy().tolist()
-            for i, one_sub_generated_ids in enumerate(sub_generated_ids):
-                if pad_token_ids is not None and pad_token_ids in one_sub_generated_ids:
-                    one_sub_generated_ids = one_sub_generated_ids[: one_sub_generated_ids.index(pad_token_ids)]
-                sub_generated_ids[i] = one_sub_generated_ids
-            outputs.append(sub_generated_ids)
-
-    return outputs
-
-
-__all__ = ["postprocess_generation_ids"]
+from typing import List, Optional, Union
+
+from torch import LongTensor
+from transformers import PreTrainedTokenizer
+
+
+def postprocess_generation_ids(
+    input_ids: LongTensor,
+    output_ids: LongTensor,
+    num_return_sequences: int,
+    tokenizer: Optional[PreTrainedTokenizer] = None,
+    pad_token_ids: Optional[int] = None,
+) -> List[List[Union[str, List[int]]]]:
+    outputs = []
+    for idx, start in enumerate(range(0, len(output_ids), num_return_sequences)):
+        sub_output_ids = output_ids[start: start + num_return_sequences]
+        sub_generated_ids = sub_output_ids[..., input_ids[idx].size(0):]
+        if tokenizer:
+            outputs.append(
+                [
+                    generated_text for generated_text in tokenizer.batch_decode(
+                        sub_generated_ids,
+                        clean_up_tokenization_spaces=True
+                    )
+                ]
+            )
+        else:
+            sub_generated_ids = sub_output_ids.cpu().numpy().tolist()
+            for i, one_sub_generated_ids in enumerate(sub_generated_ids):
+                if pad_token_ids is not None and pad_token_ids in one_sub_generated_ids:
+                    one_sub_generated_ids = one_sub_generated_ids[: one_sub_generated_ids.index(pad_token_ids)]
+                sub_generated_ids[i] = one_sub_generated_ids
+            outputs.append(sub_generated_ids)
+
+    return outputs
+
+
+__all__ = ["postprocess_generation_ids"]
```

### Comparing `auto_gptq-0.3.0/auto_gptq/eval_tasks/language_modeling_task.py` & `auto_gptq-0.3.1/auto_gptq/eval_tasks/language_modeling_task.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import math
-from typing import Any, Dict, List, Optional
-
-from torch import LongTensor
-
-from ._base import BaseTask
-
-
-class LanguageModelingTask(BaseTask):
-    def __init__(
-        self,
-        model,
-        tokenizer,
-        data_name_or_path: str,
-        prompt_col_name: str,
-        label_col_name: str,
-        device: Optional[str] = None,
-        **kwargs
-    ):
-        kwargs["merge_prompt_label"] = True
-        super().__init__(
-            model=model,
-            tokenizer=tokenizer,
-            data_name_or_path=data_name_or_path,
-            prompt_col_name=prompt_col_name,
-            label_col_name=label_col_name,
-            device=device,
-            **kwargs
-        )
-
-    def _predict(self, batch_data: Dict[str, Any], *args, **kwargs) -> List[float]:
-        outputs = self.model(**batch_data)
-        loss = outputs.loss.cpu().item()
-
-        return [loss]
-
-    def _parse_labels(self, label_ids: LongTensor) -> List[Any]:
-        return []
-
-    def _metric(self, pred: List[Any], label: List[Any]) -> Dict[str, float]:
-        return {"ppl": math.exp(sum(pred) / len(pred))}
-
-    def run(self) -> Dict[str, float]:
-        return super().run()
-
-
-__all__ = ["LanguageModelingTask"]
+import math
+from typing import Any, Dict, List, Optional
+
+from torch import LongTensor
+
+from ._base import BaseTask
+
+
+class LanguageModelingTask(BaseTask):
+    def __init__(
+        self,
+        model,
+        tokenizer,
+        data_name_or_path: str,
+        prompt_col_name: str,
+        label_col_name: str,
+        device: Optional[str] = None,
+        **kwargs
+    ):
+        kwargs["merge_prompt_label"] = True
+        super().__init__(
+            model=model,
+            tokenizer=tokenizer,
+            data_name_or_path=data_name_or_path,
+            prompt_col_name=prompt_col_name,
+            label_col_name=label_col_name,
+            device=device,
+            **kwargs
+        )
+
+    def _predict(self, batch_data: Dict[str, Any], *args, **kwargs) -> List[float]:
+        outputs = self.model(**batch_data)
+        loss = outputs.loss.cpu().item()
+
+        return [loss]
+
+    def _parse_labels(self, label_ids: LongTensor) -> List[Any]:
+        return []
+
+    def _metric(self, pred: List[Any], label: List[Any]) -> Dict[str, float]:
+        return {"ppl": math.exp(sum(pred) / len(pred))}
+
+    def run(self) -> Dict[str, float]:
+        return super().run()
+
+
+__all__ = ["LanguageModelingTask"]
```

### Comparing `auto_gptq-0.3.0/auto_gptq/modeling/_base.py` & `auto_gptq-0.3.1/auto_gptq/modeling/_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,899 +1,953 @@
-import copy
-import json
-import warnings
-import os
-from dataclasses import dataclass, field, fields
-from logging import getLogger
-from os.path import join, isfile, isdir
-from typing import Dict, List, Optional, Union
-
-import accelerate
-import torch
-import torch.nn as nn
-import transformers
-from accelerate.hooks import remove_hook_from_module
-from safetensors.torch import save_file as safe_save
-from transformers import AutoConfig, AutoModelForCausalLM, PreTrainedModel
-from transformers.utils.hub import PushToHubMixin, cached_file, create_repo, create_commit, CommitOperationAdd
-from transformers.utils.generic import ContextManagers
-from transformers.modeling_utils import no_init_weights
-
-from ._const import *
-from ._utils import *
-from ..nn_modules.qlinear import GeneralQuantLinear
-from ..nn_modules._fused_base import FusedBaseAttentionModule, FusedBaseMLPModule
-from ..quantization import GPTQ
-from ..utils.data_utils import collate_data
-from ..utils.import_utils import dynamically_import_QuantLinear, TRITON_AVAILABLE, AUTOGPTQ_CUDA_AVAILABLE
-
-logger = getLogger(__name__)
-
-
-@dataclass
-class BaseQuantizeConfig(PushToHubMixin):
-    bits: int = field(default=4, metadata={"choices": [2, 3, 4, 8]})
-    group_size: int = field(default=-1)
-    damp_percent: float = field(default=0.01)
-    desc_act: bool = field(default=True)
-    sym: bool = field(default=True)
-    true_sequential: bool = field(default=True)
-    model_name_or_path: Optional[str] = field(default=None)
-    model_file_base_name: Optional[str] = field(default=None)
-
-    def __post_init__(self):
-        fields_info = fields(self)
-
-        if self.bits not in fields_info[0].metadata["choices"]:
-            raise ValueError(f"only support quantize to {fields_info[0].metadata['choices']} bits.")
-        if self.group_size != -1 and self.group_size <= 0:
-            raise ValueError("unless equal to -1, group_size must greater then 0.")
-        if not (0 < self.damp_percent < 1):
-            raise ValueError("damp_percent must between 0 and 1.")
-
-    def save_pretrained(self, save_dir: str, **kwargs):
-        with open(join(save_dir, "quantize_config.json"), "w", encoding="utf-8") as f:
-            json.dump(self.to_dict(), f, indent=2)
-
-    @classmethod
-    def from_pretrained(cls, save_dir: str, **kwargs):
-        # Parameters related to loading from Hugging Face Hub
-        cache_dir = kwargs.pop("cache_dir", None)
-        force_download = kwargs.pop("force_download", False)
-        resume_download = kwargs.pop("resume_download", False)
-        proxies = kwargs.pop("proxies", None)
-        local_files_only = kwargs.pop("local_files_only", False)
-        use_auth_token = kwargs.pop("use_auth_token", None)
-        revision = kwargs.pop("revision", None)
-        subfolder = kwargs.pop("subfolder", None)
-        commit_hash = kwargs.pop("_commit_hash", None)
-
-        quantize_config_filename = "quantize_config.json"
-        if os.path.isdir(save_dir):  # Local
-            resolved_config_file = join(save_dir, quantize_config_filename)
-        else: # Remote
-               resolved_config_file = cached_file(
-                    save_dir,
-                    quantize_config_filename,
-                    cache_dir=cache_dir,
-                    force_download=force_download,
-                    resume_download=resume_download,
-                    proxies=proxies,
-                    use_auth_token=use_auth_token,
-                    revision=revision,
-                    local_files_only=local_files_only,
-                    subfolder=subfolder,
-                    _raise_exceptions_for_missing_entries=False,
-                    _raise_exceptions_for_connection_errors=False,
-                    _commit_hash=commit_hash,
-               )
-
-        with open(resolved_config_file, "r", encoding="utf-8") as f:
-            return cls(**json.load(f))
-                
-    def to_dict(self):
-        return {
-            "bits": self.bits,
-            "group_size": self.group_size,
-            "damp_percent": self.damp_percent,
-            "desc_act": self.desc_act,
-            "sym": self.sym,
-            "true_sequential": self.true_sequential,
-            "model_name_or_path": self.model_name_or_path,
-            "model_file_base_name": self.model_file_base_name,
-        }
-
-
-class BaseGPTQForCausalLM(nn.Module, PushToHubMixin):
-    layer_type: str = None
-    layers_block_name: str = None
-    outside_layer_modules: List[str] = None
-    inside_layer_modules: List[List[str]] = None
-    lm_head_name: str = "lm_head"
-
-    fused_attn_module_type: Optional[FusedBaseAttentionModule] = None
-    fused_mlp_module_type: Optional[FusedBaseMLPModule] = None
-
-    def __init__(
-        self,
-        model: PreTrainedModel,
-        quantized: bool,
-        quantize_config: BaseQuantizeConfig,
-        is_triton_backend: bool = False,
-        injected_fused_attention: bool = False,
-        injected_fused_mlp: bool = False,
-        trainable: bool = False
-    ):
-        super().__init__()
-
-        self.model = model
-        self.model_type = self.model.config.model_type
-        self._quantized = quantized
-        self.quantize_config = quantize_config
-        self.config = self.model.config
-
-        self.is_triton_backend = is_triton_backend
-        self.injected_fused_attention = injected_fused_attention
-        self.injected_fused_mlp = injected_fused_mlp
-        self.trainable = trainable
-
-    @property
-    def quantized(self):
-        return self._quantized
-
-    @property
-    def hf_device_map(self):
-        return getattr(self.model, "hf_device_map", None)
-
-    @staticmethod
-    def _resize_attention_mask(attention_mask: List[torch.LongTensor]):
-        return attention_mask
-
-    @staticmethod
-    def _resize_position_ids(position_ids: List[torch.LongTensor]):
-        return position_ids
-
-    def _prepare_examples_for_quantization(
-        self,
-        examples: List[Dict[str, Union[List[int], torch.LongTensor]]],
-        batch_size: int = 1,
-    ):
-        def _convert_tensor_to_list(tensor):
-            if isinstance(tensor, torch.Tensor):
-                if len(tensor.shape) == 1:
-                    tensor = tensor.unsqueeze(0)
-                tensor = tensor.long()
-                return tensor.cpu().numpy().tolist()
-            return [tensor]
-
-        new_examples = []
-        for example in examples:
-            input_ids = _convert_tensor_to_list(example["input_ids"])
-            attention_mask = _convert_tensor_to_list(example["attention_mask"])
-            if "labels" in example:
-                labels = _convert_tensor_to_list(example["labels"])
-            elif "label" in example:
-                labels = _convert_tensor_to_list(example["label"])
-            elif "label_ids" in example:
-                labels = _convert_tensor_to_list(example["label_ids"])
-            else:
-                labels = copy.deepcopy(input_ids)
-            new_examples.append(
-                {"input_ids": input_ids, "attention_mask": attention_mask, "labels": labels}
-            )
-        pad_token_id = self.config.pad_token_id
-        if not pad_token_id:
-            pad_token_id = self.config.eos_token_id
-
-        new_examples = [
-            collate_data(new_examples[start: start + batch_size], pad_token_id)
-            for start in range(0, len(new_examples), batch_size)
-        ]
-        for new_example in new_examples:
-            del new_example["labels"]
-
-        return new_examples
-
-    @torch.inference_mode()
-    def quantize(
-        self,
-        examples: List[Dict[str, Union[List[int], torch.LongTensor]]],
-        batch_size: int = 1,
-        use_triton: bool = False,
-        use_cuda_fp16: bool = True,
-        autotune_warmup_after_quantized: bool = False,
-        cache_examples_on_gpu: bool = True
-    ):
-        if self.quantized:
-            raise EnvironmentError("can't execute quantize because the model is quantized.")
-        if use_triton and not TRITON_AVAILABLE:
-            logger.warning("triton is not installed, reset use_triton to False")
-            use_triton = False
-
-        device_map = self.hf_device_map
-        if device_map:
-            for name, device in device_map.items():
-                if device == "cpu":
-                    logger.info(f"truly offloading {name} to cpu with hook.")
-                    module = get_module_by_name_suffix(self.model, name)
-                    remove_hook_from_module(module, recurse=True)
-                    accelerate.cpu_offload_with_hook(module, CUDA_0)
-
-        layer_inputs = []
-        attention_masks = []
-        position_ids = []
-        layer_input_kwargs = []
-        layer_outputs = []
-
-        examples = self._prepare_examples_for_quantization(examples, batch_size)
-
-        class LayerHijacker(nn.Module):
-            """hijack layer's forward pass to cache data"""
-
-            def __init__(self, m, device):
-                super().__init__()
-                self.module = m
-                self.data_device = device if cache_examples_on_gpu else CPU
-
-            def forward(self, inp=None, **kwargs):
-                if inp is None:  # some models use all key-value arguments in forward pass call
-                    for kwarg_name in ["hidden_states"]:
-                        if kwarg_name in kwargs:
-                            inp = kwargs[kwarg_name]
-                            break
-                layer_inputs.append(move_to_device(inp, self.data_device))
-                attention_masks.append(kwargs["attention_mask"].to(self.data_device))
-                pos_ids = kwargs.get("position_ids", None)
-                if pos_ids is not None:
-                    position_ids.append(move_to_device(pos_ids, self.data_device))
-                one_kwargs = dict()
-                for k, v in kwargs.items():  # make sure other arguments also be captured
-                    if k not in ["hidden_states", "attention_mask", "position_ids"]:
-                        if isinstance(v, torch.Tensor):
-                            one_kwargs[k] = move_to_device(v, self.data_device)
-                        else:
-                            one_kwargs[k] = v
-                layer_input_kwargs.append(one_kwargs)
-                raise ValueError
-
-        forward_pass_use_cache = self.model.config.use_cache
-        self.model.config.use_cache = False
-
-        num_batches = len(examples)
-        layers = get_module_by_name_prefix(self.model, self.layers_block_name)
-
-        force_layer_back_to_cpu = False
-        if get_device(layers[0]) == CPU:
-            layers[0] = layers[0].to(CUDA_0)
-            force_layer_back_to_cpu = True
-
-        cur_layer_device = get_device(layers[0])
-        ori_outside_layer_module_devices = {}
-        for module_name in self.outside_layer_modules:
-            module = get_module_by_name_prefix(self.model, module_name)
-
-            if module is None:
-                continue
-
-            ori_outside_layer_module_devices[module_name] = get_device(module)
-            if module is not None:
-                move_to_device(module, cur_layer_device)
-
-        # get inputs for first layer
-        layers[0] = LayerHijacker(layers[0], cur_layer_device)
-        for example in examples:
-            for k, v in example.items():
-                if len(v.shape) == 1:
-                    v = v.unsqueeze(0)
-                example[k] = move_to_device(v, cur_layer_device)
-            try:
-                self.model(**example)
-            except ValueError:
-                pass
-        layers[0] = layers[0].module
-
-        move_to_device(layers[0], CPU if force_layer_back_to_cpu else cur_layer_device)
-        for module_name in self.outside_layer_modules:
-            module = get_module_by_name_prefix(self.model, module_name)
-            if module is not None:
-                move_to_device(module, ori_outside_layer_module_devices[module_name])
-
-        torch.cuda.empty_cache()
-
-        # resize attention mask and position ids for some special models
-        attention_masks = self._resize_attention_mask(attention_masks)
-        position_ids = self._resize_position_ids(position_ids)
-
-        inside_layer_modules = self.inside_layer_modules
-        if not self.quantize_config.true_sequential:
-            inside_layer_modules = [sum(inside_layer_modules, [])]
-        quantizers = {}
-        for i in range(len(layers)):
-            logger.info(f"Start quantizing layer {i + 1}/{len(layers)}")
-            layer = layers[i]
-            force_layer_back_to_cpu = False
-            if get_device(layer) == CPU:
-                move_to_device(layer, CUDA_0)
-                force_layer_back_to_cpu = True
-            cur_layer_device = get_device(layer)
-
-            full = find_layers(layer)
-            for names in inside_layer_modules:
-                subset = {n: full[n] for n in names}
-                gptq = {}
-                for name in subset:
-                    gptq[name] = GPTQ(subset[name])
-                    gptq[name].quantizer.configure(
-                        self.quantize_config.bits,
-                        perchannel=True,
-                        sym=self.quantize_config.sym,
-                        mse=False,
-                    )
-
-                def add_batch(name):
-                    def tmp(_, inp, out):
-                        gptq[name].add_batch(inp[0].data, out.data)
-
-                    return tmp
-
-                handles = []
-                for name in subset:
-                    handles.append(subset[name].register_forward_hook(add_batch(name)))
-                for j in range(num_batches):
-                    layer_input = move_to_device(layer_inputs[j], cur_layer_device)
-                    layer_attention_mask = move_to_device(attention_masks[j], cur_layer_device)
-                    additional_layer_inputs = {
-                        "attention_mask": layer_attention_mask
-                    }
-                    layer_position_ids = None if not position_ids else move_to_device(position_ids[j], cur_layer_device)
-                    if layer_position_ids is not None:
-                        additional_layer_inputs["position_ids"] = layer_position_ids
-                    for k, v in layer_input_kwargs[j].items():
-                        if isinstance(v, torch.Tensor):
-                            additional_layer_inputs[k] = move_to_device(v, cur_layer_device)
-                        else:
-                            additional_layer_inputs[k] = v
-                    layer(layer_input, **additional_layer_inputs)
-                for h in handles:
-                    h.remove()
-
-                for name in subset:
-                    logger.info(f'Quantizing {name} in layer {i + 1}/{len(layers)}...')
-                    scale, zero, g_idx = gptq[name].fasterquant(
-                        percdamp=self.quantize_config.damp_percent,
-                        group_size=self.quantize_config.group_size,
-                        actorder=self.quantize_config.desc_act
-                    )
-                    quantizers[f'{self.layers_block_name}.{i}.{name}'] = (
-                        gptq[name].quantizer.to(CPU if force_layer_back_to_cpu else cur_layer_device),
-                        move_to_device(scale, CPU if force_layer_back_to_cpu else cur_layer_device),
-                        move_to_device(zero, CPU if force_layer_back_to_cpu else cur_layer_device),
-                        move_to_device(g_idx, CPU if force_layer_back_to_cpu else cur_layer_device)
-                    )
-                    gptq[name].free()
-
-            for j in range(num_batches):
-                layer_input = move_to_device(layer_inputs[j], cur_layer_device)
-                layer_attention_mask = move_to_device(attention_masks[j], cur_layer_device)
-                additional_layer_inputs = {
-                    "attention_mask": layer_attention_mask
-                }
-                layer_position_ids = None if not position_ids else move_to_device(position_ids[j], cur_layer_device)
-                if layer_position_ids is not None:
-                    additional_layer_inputs["position_ids"] = layer_position_ids
-                for k, v in layer_input_kwargs[j].items():
-                    if isinstance(v, torch.Tensor):
-                        additional_layer_inputs[k] = move_to_device(v, cur_layer_device)
-                    else:
-                        additional_layer_inputs[k] = v
-                layer_output = move_to_device(
-                    layer(layer_input, **additional_layer_inputs)[0],
-                    cur_layer_device if cache_examples_on_gpu else CPU
-                )
-                layer_outputs.append(layer_output)
-
-            layers[i] = move_to_device(layer, CPU if force_layer_back_to_cpu else cur_layer_device)
-            del layer
-            del gptq
-            del layer_inputs
-            layer_inputs, layer_outputs = layer_outputs, []
-            torch.cuda.empty_cache()
-
-        pack_model(
-            model=self.model,
-            quantizers=quantizers,
-            bits=self.quantize_config.bits,
-            group_size=self.quantize_config.group_size,
-            use_triton=use_triton,
-            use_cuda_fp16=use_cuda_fp16,
-            desc_act=self.quantize_config.desc_act,
-            warmup_triton=autotune_warmup_after_quantized,
-            force_layer_back_to_cpu=force_layer_back_to_cpu
-        )
-        if device_map:
-            self.model = remove_hook_from_module(self.model, recurse=True)
-            self.model = simple_dispatch_model(self.model, device_map)
-        self.model.config.use_cache = forward_pass_use_cache
-
-        self._quantized = True
-
-        torch.cuda.empty_cache()
-
-    @property
-    def device(self):
-        if not self.hf_device_map:
-            return self.model.device
-        else:
-            device = [d for d in self.hf_device_map.values() if d not in {'cpu', 'disk'}][0]
-            return torch.device(device)
-
-    def to(self, device: Union[str, torch.device]):
-        return self.model.to(device)
-
-    def forward(self, *args, **kwargs):
-        return self.model(*args, **kwargs)
-
-    def generate(self, **kwargs):
-        """shortcut for model.generate"""
-        with torch.inference_mode(), torch.amp.autocast(device_type=self.device.type):
-            return self.model.generate(**kwargs)
-
-    def prepare_inputs_for_generation(self, *args, **kwargs):
-        """shortcut for model.prepare_inputs_for_generation"""
-        return self.model.prepare_inputs_for_generation(*args, **kwargs)
-
-    def push_to_hub(
-        self,
-        repo_id: str,
-        save_dir: Optional[str] = None,
-        use_safetensors: Optional[bool] = True,
-        commit_message: Optional[str] = "Upload of AutoGPTQ quantized model",
-        use_auth_token: Optional[Union[bool, str]] = None,
-        private: Optional[bool] = None,
-        token: Optional[Union[bool, str]] = None,
-        create_pr: Optional[bool] = False,
-    ) -> str:
-        """
-        Upload the model to the Hugging Face Hub.
-
-        Parameters:
-            repo_id (`str`):
-                The name of the repository you want to push your tool to. It should contain your organization name when
-                pushing to a given organization.
-            save_dir (`str`, *optional*):
-                The name of the local folder to save the model to.
-                If the model has already been saved, this parameter can be omitted.
-            use_safetensors (`bool`, *optional*):
-                Save the model using `safetensors`.
-                If the model has already been saved, this parameter can be omitted.
-            commit_message (`str`, *optional*, defaults to `"Upload tool"`):
-                Message to commit while pushing.
-            use_auth_token (`bool` or `str`, *optional*):
-                The token to use as HTTP bearer authorization for remote files. If `True`, will use the token generated
-                when running `huggingface-cli login` (stored in `~/.huggingface`). Will default to `True` if `repo_url`
-                is not specified.
-            private (`bool`, *optional*):
-                Whether or not the repository created should be private.
-            token (`bool` or `str`, *optional*):
-                The token to use as HTTP bearer authorization for remote files. If unset, will use the token generated
-                when running `huggingface-cli login` (stored in `~/.huggingface`).
-            create_pr (`bool`, *optional*, defaults to `False`):
-                Whether or not to create a PR with the uploaded files or directly commit.
-        """
-        if (self.quantize_config.model_name_or_path is None or not isdir(self.quantize_config.model_name_or_path)) and save_dir is None:
-            raise ValueError("Quantized model should be saved first, or you can provide save_dir to make sure model is saved to local disk before uploading.")
-        
-        if save_dir is not None:
-            logger.info(f"Saving model to {save_dir}")
-            self.save_quantized(save_dir, use_safetensors)
-
-        repo_url = create_repo(
-            repo_id=repo_id, token=token, private=private, exist_ok=True, repo_type="model"
-        )
-        repo_id = repo_url.repo_id
-
-        if self.quantize_config.model_name_or_path is not None:
-            work_dir = self.quantize_config.model_name_or_path
-            operations = [
-                CommitOperationAdd(path_or_fileobj=join(work_dir, f), path_in_repo=f)
-                for f in os.listdir(work_dir)
-            ]
-            logger.info(f"Uploading the following files to {repo_id}: {','.join(os.listdir(work_dir))}")
-            return create_commit(
-                repo_id=repo_id,
-                operations=operations,
-                commit_message=commit_message,
-                token=use_auth_token,
-                create_pr=create_pr,
-                repo_type="model",
-            )
-
-    def save_quantized(self, save_dir: str, use_safetensors: bool = False):
-        """save quantized model and configs to local disk"""
-        os.makedirs(save_dir, exist_ok=True)
-
-        if not self.quantized:
-            raise EnvironmentError("can only save quantized model, please execute .quantize first.")
-
-        self.model.to(CPU)
-
-        model_base_name = self.quantize_config.model_file_base_name or f"gptq_model-{self.quantize_config.bits}bit-{self.quantize_config.group_size}g"
-        if use_safetensors:
-            model_save_name = model_base_name + ".safetensors"
-            state_dict = self.model.state_dict()
-            state_dict = {k: v.clone().contiguous() for k, v in state_dict.items()}
-            safe_save(state_dict, join(save_dir, model_save_name))
-        else:
-            model_save_name = model_base_name + ".bin"
-            torch.save(self.model.state_dict(), join(save_dir, model_save_name))
-
-        self.model.config.save_pretrained(save_dir)
-        self.quantize_config.save_pretrained(save_dir)
-        self.quantize_config.model_name_or_path = save_dir
-        self.quantize_config.model_file_base_name = model_base_name
-
-    def save_pretrained(self, save_dir: str, use_safetensors: bool = False, **kwargs):
-        """alias of save_quantized"""
-        logger.warning("you are using save_pretrained, which will re-direct to save_quantized.")
-        self.save_quantized(save_dir, use_safetensors)
-
-    @classmethod
-    def from_pretrained(
-        cls,
-        pretrained_model_name_or_path: str,
-        quantize_config: BaseQuantizeConfig,
-        max_memory: Optional[dict] = None,
-        trust_remote_code: bool = False,
-        torch_dtype: torch.dtype = torch.float16,
-        **model_init_kwargs
-    ):
-        """load un-quantized pretrained model to cpu"""
-
-        if not torch.cuda.is_available():
-            raise EnvironmentError("Load pretrained model to do quantization requires CUDA available.")
-
-        def skip(*args, **kwargs):
-            pass
-
-        torch.nn.init.kaiming_uniform_ = skip
-        torch.nn.init.uniform_ = skip
-        torch.nn.init.normal_ = skip
-
-        config = AutoConfig.from_pretrained(pretrained_model_name_or_path, trust_remote_code=True)
-        if config.model_type not in SUPPORTED_MODELS:
-            raise TypeError(f"{config.model_type} isn't supported yet.")
-
-        # enforce some values despite user specified
-        model_init_kwargs["torch_dtype"] = torch_dtype
-        model_init_kwargs["trust_remote_code"] = trust_remote_code
-        if max_memory:
-            if "disk" in max_memory:
-                raise NotImplementedError("disk offload not support yet.")
-            with accelerate.init_empty_weights():
-                model = AutoModelForCausalLM.from_config(config, trust_remote_code=True)
-            model.tie_weights()
-
-            max_memory = accelerate.utils.get_balanced_memory(
-                model,
-                max_memory=max_memory,
-                no_split_module_classes=[cls.layer_type],
-                dtype=model_init_kwargs["torch_dtype"],
-                low_zero=False
-            )
-            model_init_kwargs["device_map"] = accelerate.infer_auto_device_map(
-                model,
-                max_memory=max_memory,
-                no_split_module_classes=[cls.layer_type],
-                dtype=model_init_kwargs["torch_dtype"]
-            )
-            model_init_kwargs["low_cpu_mem_usage"] = True
-
-            del model
-        else:
-            model_init_kwargs["device_map"] = None
-            model_init_kwargs["low_cpu_mem_usage"] = False
-
-        torch.cuda.empty_cache()
-
-        model = AutoModelForCausalLM.from_pretrained(pretrained_model_name_or_path, **model_init_kwargs)
-        model_config = model.config.to_dict()
-        seq_len_keys = ["max_position_embeddings", "seq_length", "n_positions"]
-        if any([k in model_config for k in seq_len_keys]):
-            for key in seq_len_keys:
-                if key in model_config:
-                    model.seqlen = model_config[key]
-                    break
-        else:
-            logger.warning("can't get model's sequence length from model config, will set to 4096.")
-            model.seqlen = 4096
-        model.eval()
-
-        return cls(model, False, quantize_config)
-
-    @classmethod
-    def from_quantized(
-        cls,
-        model_name_or_path: Optional[str] = None,
-        save_dir: Optional[str] = None,
-        device_map: Optional[Union[str, Dict[str, Union[int, str]]]] = None,
-        max_memory: Optional[dict] = None,
-        device: Optional[Union[str, int]] = None,
-        low_cpu_mem_usage: bool = False,
-        use_triton: bool = False,
-        torch_dtype: torch.dtype = torch.float16,
-        inject_fused_attention: bool = True,
-        inject_fused_mlp: bool = True,
-        use_cuda_fp16: bool = True,
-        quantize_config: Optional[BaseQuantizeConfig] = None,
-        model_basename: Optional[str] = None,
-        use_safetensors: bool = False,
-        trust_remote_code: bool = False,
-        warmup_triton: bool = False,
-        trainable: bool = False,
-        **kwargs
-    ):
-        """load quantized model from local disk"""
-       
-        # Parameters related to loading from Hugging Face Hub
-        cache_dir = kwargs.pop("cache_dir", None)
-        force_download = kwargs.pop("force_download", False)
-        resume_download = kwargs.pop("resume_download", False)
-        proxies = kwargs.pop("proxies", None)
-        local_files_only = kwargs.pop("local_files_only", False)
-        use_auth_token = kwargs.pop("use_auth_token", None)
-        revision = kwargs.pop("revision", None)
-        subfolder = kwargs.pop("subfolder", "")
-        commit_hash = kwargs.pop("_commit_hash", None)
-
-        if use_triton and not TRITON_AVAILABLE:
-            logger.warning("triton is not installed, reset use_triton to False")
-            use_triton = False
-
-        # == step1: prepare configs and file names == #
-        if model_name_or_path and save_dir:
-            logger.warning("save_dir will be ignored because model_name_or_path is explicit specified.")
-        if not model_name_or_path and save_dir:
-            model_name_or_path = save_dir
-            warnings.warn("save_dir is deprecated and will be removed in version 0.3.0", PendingDeprecationWarning, stacklevel=2)
-        if not model_name_or_path and not save_dir:
-            raise ValueError("at least one of model_name_or_path or save_dir should be specified.")
-        
-        config = AutoConfig.from_pretrained(model_name_or_path, trust_remote_code=trust_remote_code)
-
-        if config.model_type not in SUPPORTED_MODELS:
-            raise TypeError(f"{config.model_type} isn't supported yet.")
-
-        if quantize_config is None:
-            quantize_config = BaseQuantizeConfig.from_pretrained(model_name_or_path, **kwargs)
-        
-        if model_basename is None:
-            if quantize_config.model_file_base_name:
-                model_basename = quantize_config.model_file_base_name
-            else:
-                model_basename = f"gptq_model-{quantize_config.bits}bit-{quantize_config.group_size}g"
-        
-        quantize_config.model_name_or_path = model_name_or_path
-        quantize_config.model_file_base_name = model_basename
-
-        extensions = []
-        if use_safetensors:
-            extensions.append(".safetensors")
-        else:
-            extensions += [".bin", ".pt"]
-
-        model_name_or_path = str(model_name_or_path)
-        is_local = isdir(model_name_or_path)
-
-        resolved_archive_file = None
-        if is_local:
-            model_save_name = join(model_name_or_path, model_basename)
-
-            for ext in extensions:
-                if isfile(model_save_name + ext):
-                    resolved_archive_file = model_save_name + ext
-                    break
-        else: # remote
-            cached_file_kwargs = {
-                "cache_dir": cache_dir,
-                "force_download": force_download,
-                "proxies": proxies,
-                "resume_download": resume_download,
-                "local_files_only": local_files_only,
-                "use_auth_token": use_auth_token,
-                "revision": revision,
-                "subfolder": subfolder,
-                "_raise_exceptions_for_missing_entries": False,
-                "_commit_hash": commit_hash,
-            }
-            
-            for ext in extensions:
-                resolved_archive_file = cached_file(model_name_or_path, model_basename + ext, **cached_file_kwargs)
-                if resolved_archive_file is not None:
-                    break
-        
-        if resolved_archive_file is None: # Could not find a model file to use
-            raise FileNotFoundError(f"Could not find model in {model_name_or_path}")
-                
-        model_save_name = resolved_archive_file
-
-        if not use_triton and trainable:
-            logger.warning("QuantLinear with cuda backend not support trainable mode yet, Switch to the pytorch backend.")
-
-        # == step2: convert model to gptq-model (replace Linear with QuantLinear) == #
-        def skip(*args, **kwargs):
-            pass
-
-        torch.nn.init.kaiming_uniform_ = skip
-        torch.nn.init.uniform_ = skip
-        torch.nn.init.normal_ = skip
-
-        transformers.modeling_utils._init_weights = False
-
-        init_contexts = [no_init_weights()]
-        if low_cpu_mem_usage:
-            init_contexts.append(accelerate.init_empty_weights(include_buffers=False))
-
-        with ContextManagers(init_contexts):
-            model = AutoModelForCausalLM.from_config(
-                config,
-                trust_remote_code=trust_remote_code,
-                torch_dtype=torch_dtype
-            )
-
-            layers = find_layers(model)
-            ignore_layers = [cls.lm_head_name] + cls.outside_layer_modules
-            for name in list(layers.keys()):
-                if any([name.startswith(ignore_layer) for ignore_layer in ignore_layers]):
-                    logger.info(f"{name} not been quantized, will be ignored when make_quant.")
-                    del layers[name]
-
-            make_quant(
-                model,
-                layers,
-                quantize_config.bits,
-                quantize_config.group_size,
-                use_triton=use_triton,
-                use_cuda_fp16=use_cuda_fp16,
-                desc_act=quantize_config.desc_act,
-                trainable=trainable
-            )
-            model.tie_weights()
-
-        # == step3: load checkpoint and dispatch == #
-        if isinstance(device_map, str) and device_map not in ["auto", "balanced", "balanced_low_0", "sequential"]:
-            raise ValueError(
-                "If passing a string for `device_map`, please choose 'auto', 'balanced', 'balanced_low_0' or "
-                "'sequential'."
-            )
-        if isinstance(device_map, dict):
-            max_memory = None
-        else:
-            if device is None and not device_map and not max_memory:
-                device_map = "auto"
-            if device is not None:
-                device = torch.device(device)
-                if not max_memory and not device_map:
-                    device_map = {"": device.index if device.type == "cuda" else device.type}
-            if not isinstance(device_map, dict) and device_map != "sequential":
-                max_memory = accelerate.utils.get_balanced_memory(
-                    model=model,
-                    max_memory=max_memory,
-                    no_split_module_classes=[cls.layer_type],
-                    low_zero=(device_map == "balanced_low_0")
-                )
-        if not isinstance(device_map, dict):
-            device_map = accelerate.infer_auto_device_map(
-                model,
-                max_memory=max_memory,
-                no_split_module_classes=[cls.layer_type]
-            )
-
-        if low_cpu_mem_usage:
-            make_sure_no_tensor_in_meta_device(model, use_triton, quantize_config.desc_act, quantize_config.group_size)
-
-        accelerate.utils.modeling.load_checkpoint_in_model(
-            model,
-            checkpoint=model_save_name,
-            device_map=device_map,
-            offload_state_dict=True,
-            offload_buffers=True
-        )
-        model = simple_dispatch_model(model, device_map)
-
-        # == step4: set seqlen == #
-        model_config = model.config.to_dict()
-        seq_len_keys = ["max_position_embeddings", "seq_length", "n_positions"]
-        if any([k in model_config for k in seq_len_keys]):
-            for key in seq_len_keys:
-                if key in model_config:
-                    model.seqlen = model_config[key]
-                    break
-        else:
-            logger.warning("can't get model's sequence length from model config, will set to 4096.")
-            model.seqlen = 4096
-
-        # == step5: (optional) inject optimized module == #
-        if inject_fused_attention:
-            if cls.fused_attn_module_type is None:
-                inject_fused_attention = False
-                logger.warning(f"{cls.__name__} hasn't fused attention module yet, will skip inject fused attention.")
-            else:
-                cls.fused_attn_module_type.inject_to_model(
-                    model,
-                    use_triton=use_triton,
-                    group_size=quantize_config.group_size,
-                    use_cuda_fp16=use_cuda_fp16,
-                    desc_act=quantize_config.desc_act,
-                    trainable=trainable
-                )
-        if inject_fused_mlp:
-            if cls.fused_mlp_module_type is None:
-                inject_fused_mlp = False
-                logger.warning(f"{cls.__name__} hasn't fused mlp module yet, will skip inject fused mlp.")
-            else:
-                cls.fused_mlp_module_type.inject_to_model(
-                    model,
-                    use_triton=use_triton
-                )
-
-        model.eval()
-        # == step6: (optional) warmup triton == #
-        if use_triton and warmup_triton:
-            from ..nn_modules.qlinear.qlinear_triton import QuantLinear
-            QuantLinear.warmup(model, seqlen=model.seqlen)
-
-            if inject_fused_mlp and cls.fused_mlp_module_type is not None:
-                cls.fused_mlp_module_type.warmup(model, seqlen=model.seqlen)
-
-        # == step7: make model compatible with peft
-        cls.make_sure_compatible_with_peft(
-            model, use_triton, quantize_config.desc_act, quantize_config.group_size
-        )
-
-        return cls(
-            model,
-            True,
-            quantize_config,
-            is_triton_backend=use_triton,
-            injected_fused_attention=inject_fused_attention,
-            injected_fused_mlp=inject_fused_mlp and use_triton,
-            trainable=trainable
-        )
-
-    def warmup_triton(self, enabled: bool = True):
-        if not enabled:
-            return
-        if not TRITON_AVAILABLE:
-            logger.warning(f"triton is not available, skip warmup stage directly.")
-            return
-
-        from ..nn_modules.qlinear.qlinear_triton import QuantLinear
-        QuantLinear.warmup(self.model, seqlen=self.model.seqlen)
-
-        if self.fused_mlp_module_type is not None:
-            self.fused_mlp_module_type.warmup(self.model, seqlen=self.model.seqlen)
-
-    def enable_trainable_mode(self, enabled: bool = True):
-        if not self.is_triton_backend and enabled:
-            raise NotImplementedError("For now, trainable mode only supports triton backend.")
-        for n, m in self.model.named_modules():
-            if hasattr(m, "trainable"):
-                setattr(m, "trainable", enabled)
-
-    def disable_trainable_mode(self):
-        self.enable_trainable_mode(enabled=False)
-
-    @staticmethod
-    def make_sure_compatible_with_peft(model: PreTrainedModel, use_triton: bool, desc_act: bool, group_size: int):
-        GeneralQuantLinear.inject_to_model(
-            model,
-            dynamically_import_QuantLinear(use_triton, desc_act, group_size)
-        )
-
-    def __getattr__(self, item):
-        try:
-            return super().__getattr__(item)
-        except:
-            return getattr(self.model, item)
-
-
-__all__ = ["BaseGPTQForCausalLM", "BaseQuantizeConfig"]
+import copy
+import json
+import warnings
+import os
+from dataclasses import dataclass, field, fields
+from logging import getLogger
+from os.path import join, isfile, isdir
+from typing import Dict, List, Optional, Union
+
+import accelerate
+import torch
+import torch.nn as nn
+import transformers
+from accelerate.hooks import remove_hook_from_module
+from safetensors.torch import save_file as safe_save
+from transformers import AutoConfig, AutoModelForCausalLM, PreTrainedModel
+from transformers.utils.hub import PushToHubMixin, cached_file, create_repo, create_commit, CommitOperationAdd
+from transformers.utils.generic import ContextManagers
+from transformers.modeling_utils import no_init_weights
+
+from ._const import *
+from ._utils import *
+from ..nn_modules.qlinear import GeneralQuantLinear
+from ..nn_modules._fused_base import FusedBaseAttentionModule, FusedBaseMLPModule
+from ..quantization import GPTQ
+from ..utils.data_utils import collate_data
+from ..utils.import_utils import dynamically_import_QuantLinear, TRITON_AVAILABLE, AUTOGPTQ_CUDA_AVAILABLE
+
+logger = getLogger(__name__)
+
+
+@dataclass
+class BaseQuantizeConfig(PushToHubMixin):
+    bits: int = field(default=4, metadata={"choices": [2, 3, 4, 8]})
+    group_size: int = field(default=-1)
+    damp_percent: float = field(default=0.01)
+    desc_act: bool = field(default=True)
+    sym: bool = field(default=True)
+    true_sequential: bool = field(default=True)
+    model_name_or_path: Optional[str] = field(default=None)
+    model_file_base_name: Optional[str] = field(default=None)
+
+    def __post_init__(self):
+        fields_info = fields(self)
+
+        if self.bits not in fields_info[0].metadata["choices"]:
+            raise ValueError(f"only support quantize to {fields_info[0].metadata['choices']} bits.")
+        if self.group_size != -1 and self.group_size <= 0:
+            raise ValueError("unless equal to -1, group_size must greater then 0.")
+        if not (0 < self.damp_percent < 1):
+            raise ValueError("damp_percent must between 0 and 1.")
+
+    def save_pretrained(self, save_dir: str, **kwargs):
+        with open(join(save_dir, "quantize_config.json"), "w", encoding="utf-8") as f:
+            json.dump(self.to_dict(), f, indent=2)
+
+    @classmethod
+    def from_pretrained(cls, save_dir: str, **kwargs):
+        # Parameters related to loading from Hugging Face Hub
+        cache_dir = kwargs.pop("cache_dir", None)
+        force_download = kwargs.pop("force_download", False)
+        resume_download = kwargs.pop("resume_download", False)
+        proxies = kwargs.pop("proxies", None)
+        local_files_only = kwargs.pop("local_files_only", False)
+        use_auth_token = kwargs.pop("use_auth_token", None)
+        revision = kwargs.pop("revision", None)
+        subfolder = kwargs.pop("subfolder", None)
+        commit_hash = kwargs.pop("_commit_hash", None)
+
+        quantize_config_filename = "quantize_config.json"
+        if os.path.isdir(save_dir):  # Local
+            resolved_config_file = join(save_dir, quantize_config_filename)
+        else: # Remote
+               resolved_config_file = cached_file(
+                    save_dir,
+                    quantize_config_filename,
+                    cache_dir=cache_dir,
+                    force_download=force_download,
+                    resume_download=resume_download,
+                    proxies=proxies,
+                    use_auth_token=use_auth_token,
+                    revision=revision,
+                    local_files_only=local_files_only,
+                    subfolder=subfolder,
+                    _raise_exceptions_for_missing_entries=False,
+                    _raise_exceptions_for_connection_errors=False,
+                    _commit_hash=commit_hash,
+               )
+
+        with open(resolved_config_file, "r", encoding="utf-8") as f:
+            return cls(**json.load(f))
+                
+    def to_dict(self):
+        return {
+            "bits": self.bits,
+            "group_size": self.group_size,
+            "damp_percent": self.damp_percent,
+            "desc_act": self.desc_act,
+            "sym": self.sym,
+            "true_sequential": self.true_sequential,
+            "model_name_or_path": self.model_name_or_path,
+            "model_file_base_name": self.model_file_base_name,
+        }
+
+
+class BaseGPTQForCausalLM(nn.Module, PushToHubMixin):
+    layer_type: str = None
+    layers_block_name: str = None
+    outside_layer_modules: List[str] = None
+    inside_layer_modules: List[List[str]] = None
+    lm_head_name: str = "lm_head"
+
+    fused_attn_module_type: Optional[FusedBaseAttentionModule] = None
+    fused_mlp_module_type: Optional[FusedBaseMLPModule] = None
+
+    def __init__(
+        self,
+        model: PreTrainedModel,
+        quantized: bool,
+        quantize_config: BaseQuantizeConfig,
+        is_triton_backend: bool = False,
+        injected_fused_attention: bool = False,
+        injected_fused_mlp: bool = False,
+        trainable: bool = False
+    ):
+        super().__init__()
+
+        self.model = model
+        self.model_type = self.model.config.model_type
+        self._quantized = quantized
+        self.quantize_config = quantize_config
+        self.config = self.model.config
+
+        self.is_triton_backend = is_triton_backend
+        self.injected_fused_attention = injected_fused_attention
+        self.injected_fused_mlp = injected_fused_mlp
+        self.trainable = trainable
+
+    @property
+    def quantized(self):
+        return self._quantized
+
+    @property
+    def hf_device_map(self):
+        return getattr(self.model, "hf_device_map", None)
+
+    @staticmethod
+    def _resize_attention_mask(attention_mask: List[torch.LongTensor]):
+        return attention_mask
+
+    @staticmethod
+    def _resize_position_ids(position_ids: List[torch.LongTensor]):
+        return position_ids
+
+    def _prepare_examples_for_quantization(
+        self,
+        examples: List[Dict[str, Union[List[int], torch.LongTensor]]],
+        batch_size: int = 1,
+    ):
+        def _convert_tensor_to_list(tensor):
+            if isinstance(tensor, torch.Tensor):
+                if len(tensor.shape) == 1:
+                    tensor = tensor.unsqueeze(0)
+                tensor = tensor.long()
+                return tensor.cpu().numpy().tolist()
+            return [tensor]
+
+        new_examples = []
+        for example in examples:
+            input_ids = _convert_tensor_to_list(example["input_ids"])
+            attention_mask = _convert_tensor_to_list(example["attention_mask"])
+            if "labels" in example:
+                labels = _convert_tensor_to_list(example["labels"])
+            elif "label" in example:
+                labels = _convert_tensor_to_list(example["label"])
+            elif "label_ids" in example:
+                labels = _convert_tensor_to_list(example["label_ids"])
+            else:
+                labels = copy.deepcopy(input_ids)
+            new_examples.append(
+                {"input_ids": input_ids, "attention_mask": attention_mask, "labels": labels}
+            )
+        pad_token_id = self.config.pad_token_id
+        if not pad_token_id:
+            pad_token_id = self.config.eos_token_id
+
+        new_examples = [
+            collate_data(new_examples[start: start + batch_size], pad_token_id)
+            for start in range(0, len(new_examples), batch_size)
+        ]
+        for new_example in new_examples:
+            del new_example["labels"]
+
+        return new_examples
+
+    @torch.inference_mode()
+    def quantize(
+        self,
+        examples: List[Dict[str, Union[List[int], torch.LongTensor]]],
+        batch_size: int = 1,
+        use_triton: bool = False,
+        use_cuda_fp16: bool = True,
+        autotune_warmup_after_quantized: bool = False,
+        cache_examples_on_gpu: bool = True
+    ):
+        if self.quantized:
+            raise EnvironmentError("can't execute quantize because the model is quantized.")
+        if use_triton and not TRITON_AVAILABLE:
+            logger.warning("triton is not installed, reset use_triton to False")
+            use_triton = False
+
+        device_map = self.hf_device_map
+        if device_map:
+            for name, device in device_map.items():
+                if device == "cpu":
+                    logger.info(f"truly offloading {name} to cpu with hook.")
+                    module = get_module_by_name_suffix(self.model, name)
+                    remove_hook_from_module(module, recurse=True)
+                    accelerate.cpu_offload_with_hook(module, CUDA_0)
+
+        layer_inputs = []
+        attention_masks = []
+        position_ids = []
+        layer_input_kwargs = []
+        layer_outputs = []
+
+        examples = self._prepare_examples_for_quantization(examples, batch_size)
+
+        class LayerHijacker(nn.Module):
+            """hijack layer's forward pass to cache data"""
+
+            def __init__(self, m, device):
+                super().__init__()
+                self.module = m
+                self.data_device = device if cache_examples_on_gpu else CPU
+
+            def forward(self, inp=None, **kwargs):
+                if inp is None:  # some models use all key-value arguments in forward pass call
+                    for kwarg_name in ["hidden_states"]:
+                        if kwarg_name in kwargs:
+                            inp = kwargs[kwarg_name]
+                            break
+                layer_inputs.append(move_to_device(inp, self.data_device))
+                attention_masks.append(kwargs["attention_mask"].to(self.data_device))
+                pos_ids = kwargs.get("position_ids", None)
+                if pos_ids is not None:
+                    position_ids.append(move_to_device(pos_ids, self.data_device))
+                one_kwargs = dict()
+                for k, v in kwargs.items():  # make sure other arguments also be captured
+                    if k not in ["hidden_states", "attention_mask", "position_ids"]:
+                        if isinstance(v, torch.Tensor):
+                            one_kwargs[k] = move_to_device(v, self.data_device)
+                        else:
+                            one_kwargs[k] = v
+                layer_input_kwargs.append(one_kwargs)
+                raise ValueError
+
+        forward_pass_use_cache = self.model.config.use_cache
+        self.model.config.use_cache = False
+
+        num_batches = len(examples)
+        layers = get_module_by_name_prefix(self.model, self.layers_block_name)
+
+        force_layer_back_to_cpu = False
+        if get_device(layers[0]) == CPU:
+            layers[0] = layers[0].to(CUDA_0)
+            force_layer_back_to_cpu = True
+
+        cur_layer_device = get_device(layers[0])
+        ori_outside_layer_module_devices = {}
+        for module_name in self.outside_layer_modules:
+            module = get_module_by_name_prefix(self.model, module_name)
+
+            if module is None:
+                continue
+
+            ori_outside_layer_module_devices[module_name] = get_device(module)
+            if module is not None:
+                move_to_device(module, cur_layer_device)
+
+        # get inputs for first layer
+        layers[0] = LayerHijacker(layers[0], cur_layer_device)
+        for example in examples:
+            for k, v in example.items():
+                if len(v.shape) == 1:
+                    v = v.unsqueeze(0)
+                example[k] = move_to_device(v, cur_layer_device)
+            try:
+                self.model(**example)
+            except ValueError:
+                pass
+        layers[0] = layers[0].module
+
+        move_to_device(layers[0], CPU if force_layer_back_to_cpu else cur_layer_device)
+        for module_name in self.outside_layer_modules:
+            module = get_module_by_name_prefix(self.model, module_name)
+            if module is not None:
+                move_to_device(module, ori_outside_layer_module_devices[module_name])
+
+        torch.cuda.empty_cache()
+
+        # resize attention mask and position ids for some special models
+        attention_masks = self._resize_attention_mask(attention_masks)
+        position_ids = self._resize_position_ids(position_ids)
+
+        inside_layer_modules = self.inside_layer_modules
+        if not self.quantize_config.true_sequential:
+            inside_layer_modules = [sum(inside_layer_modules, [])]
+        quantizers = {}
+        for i in range(len(layers)):
+            logger.info(f"Start quantizing layer {i + 1}/{len(layers)}")
+            layer = layers[i]
+            force_layer_back_to_cpu = False
+            if get_device(layer) == CPU:
+                move_to_device(layer, CUDA_0)
+                force_layer_back_to_cpu = True
+            cur_layer_device = get_device(layer)
+
+            full = find_layers(layer)
+            for names in inside_layer_modules:
+                subset = {n: full[n] for n in names}
+                gptq = {}
+                for name in subset:
+                    gptq[name] = GPTQ(subset[name])
+                    gptq[name].quantizer.configure(
+                        self.quantize_config.bits,
+                        perchannel=True,
+                        sym=self.quantize_config.sym,
+                        mse=False,
+                    )
+
+                def add_batch(name):
+                    def tmp(_, inp, out):
+                        gptq[name].add_batch(inp[0].data, out.data)
+
+                    return tmp
+
+                handles = []
+                for name in subset:
+                    handles.append(subset[name].register_forward_hook(add_batch(name)))
+                for j in range(num_batches):
+                    layer_input = move_to_device(layer_inputs[j], cur_layer_device)
+                    layer_attention_mask = move_to_device(attention_masks[j], cur_layer_device)
+                    additional_layer_inputs = {
+                        "attention_mask": layer_attention_mask
+                    }
+                    layer_position_ids = None if not position_ids else move_to_device(position_ids[j], cur_layer_device)
+                    if layer_position_ids is not None:
+                        additional_layer_inputs["position_ids"] = layer_position_ids
+                    for k, v in layer_input_kwargs[j].items():
+                        if isinstance(v, torch.Tensor):
+                            additional_layer_inputs[k] = move_to_device(v, cur_layer_device)
+                        else:
+                            additional_layer_inputs[k] = v
+                    layer(layer_input, **additional_layer_inputs)
+                for h in handles:
+                    h.remove()
+
+                for name in subset:
+                    logger.info(f'Quantizing {name} in layer {i + 1}/{len(layers)}...')
+                    scale, zero, g_idx = gptq[name].fasterquant(
+                        percdamp=self.quantize_config.damp_percent,
+                        group_size=self.quantize_config.group_size,
+                        actorder=self.quantize_config.desc_act
+                    )
+                    quantizers[f'{self.layers_block_name}.{i}.{name}'] = (
+                        gptq[name].quantizer.to(CPU if force_layer_back_to_cpu else cur_layer_device),
+                        move_to_device(scale, CPU if force_layer_back_to_cpu else cur_layer_device),
+                        move_to_device(zero, CPU if force_layer_back_to_cpu else cur_layer_device),
+                        move_to_device(g_idx, CPU if force_layer_back_to_cpu else cur_layer_device)
+                    )
+                    gptq[name].free()
+
+            for j in range(num_batches):
+                layer_input = move_to_device(layer_inputs[j], cur_layer_device)
+                layer_attention_mask = move_to_device(attention_masks[j], cur_layer_device)
+                additional_layer_inputs = {
+                    "attention_mask": layer_attention_mask
+                }
+                layer_position_ids = None if not position_ids else move_to_device(position_ids[j], cur_layer_device)
+                if layer_position_ids is not None:
+                    additional_layer_inputs["position_ids"] = layer_position_ids
+                for k, v in layer_input_kwargs[j].items():
+                    if isinstance(v, torch.Tensor):
+                        additional_layer_inputs[k] = move_to_device(v, cur_layer_device)
+                    else:
+                        additional_layer_inputs[k] = v
+                layer_output = move_to_device(
+                    layer(layer_input, **additional_layer_inputs)[0],
+                    cur_layer_device if cache_examples_on_gpu else CPU
+                )
+                layer_outputs.append(layer_output)
+
+            layers[i] = move_to_device(layer, CPU if force_layer_back_to_cpu else cur_layer_device)
+            del layer
+            del gptq
+            del layer_inputs
+            layer_inputs, layer_outputs = layer_outputs, []
+            torch.cuda.empty_cache()
+
+        pack_model(
+            model=self.model,
+            quantizers=quantizers,
+            bits=self.quantize_config.bits,
+            group_size=self.quantize_config.group_size,
+            use_triton=use_triton,
+            use_cuda_fp16=use_cuda_fp16,
+            desc_act=self.quantize_config.desc_act,
+            warmup_triton=autotune_warmup_after_quantized,
+            force_layer_back_to_cpu=force_layer_back_to_cpu
+        )
+        if device_map:
+            self.model = remove_hook_from_module(self.model, recurse=True)
+            self.model = simple_dispatch_model(self.model, device_map)
+        self.model.config.use_cache = forward_pass_use_cache
+
+        self._quantized = True
+
+        torch.cuda.empty_cache()
+
+    @property
+    def device(self):
+        if not self.hf_device_map:
+            return self.model.device
+        else:
+            device = [d for d in self.hf_device_map.values() if d not in {'cpu', 'disk'}][0]
+            return torch.device(device)
+
+    def to(self, device: Union[str, torch.device]):
+        return self.model.to(device)
+
+    def forward(self, *args, **kwargs):
+        return self.model(*args, **kwargs)
+
+    def generate(self, **kwargs):
+        """shortcut for model.generate"""
+        with torch.inference_mode(), torch.amp.autocast(device_type=self.device.type):
+            return self.model.generate(**kwargs)
+
+    def prepare_inputs_for_generation(self, *args, **kwargs):
+        """shortcut for model.prepare_inputs_for_generation"""
+        return self.model.prepare_inputs_for_generation(*args, **kwargs)
+
+    def push_to_hub(
+        self,
+        repo_id: str,
+        save_dir: Optional[str] = None,
+        use_safetensors: Optional[bool] = True,
+        safetensors_metadata: Optional[Dict[str, str]] = None,
+        commit_message: Optional[str] = "Upload of AutoGPTQ quantized model",
+        use_auth_token: Optional[Union[bool, str]] = None,
+        private: Optional[bool] = None,
+        token: Optional[Union[bool, str]] = None,
+        create_pr: Optional[bool] = False,
+    ) -> str:
+        """
+        Upload the model to the Hugging Face Hub.
+
+        Parameters:
+            repo_id (`str`):
+                The name of the repository you want to push your tool to. It should contain your organization name when
+                pushing to a given organization.
+            save_dir (`str`, *optional*):
+                The name of the local folder to save the model to.
+                If the model has already been saved, this parameter can be omitted.
+            use_safetensors (`bool`, *optional*):
+                Save the model using `safetensors`.
+                If the model has already been saved, this parameter can be omitted.
+            safetensors_metadata: (`dict`, *optional*, defaults to `None`):
+                Pass optional metadata dictionary to be saved in the `safetensors` model file(s).
+                Metadata is optional and is purely for informational purposes. It does not affect inference.
+                If `None`, no metadata will be saved.
+            commit_message (`str`, *optional*, defaults to `"Upload tool"`):
+                Message to commit while pushing.
+            use_auth_token (`bool` or `str`, *optional*):
+                The token to use as HTTP bearer authorization for remote files. If `True`, will use the token generated
+                when running `huggingface-cli login` (stored in `~/.huggingface`). Will default to `True` if `repo_url`
+                is not specified.
+            private (`bool`, *optional*):
+                Whether or not the repository created should be private.
+            token (`bool` or `str`, *optional*):
+                The token to use as HTTP bearer authorization for remote files. If unset, will use the token generated
+                when running `huggingface-cli login` (stored in `~/.huggingface`).
+            create_pr (`bool`, *optional*, defaults to `False`):
+                Whether or not to create a PR with the uploaded files or directly commit.
+        """
+        if (self.quantize_config.model_name_or_path is None or not isdir(self.quantize_config.model_name_or_path)) and save_dir is None:
+            raise ValueError("Quantized model should be saved first, or you can provide save_dir to make sure model is saved to local disk before uploading.")
+        
+        if save_dir is not None:
+            logger.info(f"Saving model to {save_dir}")
+            self.save_quantized(save_dir, use_safetensors, safetensors_metadata)
+
+        repo_url = create_repo(
+            repo_id=repo_id, token=token, private=private, exist_ok=True, repo_type="model"
+        )
+        repo_id = repo_url.repo_id
+
+        if self.quantize_config.model_name_or_path is not None:
+            work_dir = self.quantize_config.model_name_or_path
+            operations = [
+                CommitOperationAdd(path_or_fileobj=join(work_dir, f), path_in_repo=f)
+                for f in os.listdir(work_dir)
+            ]
+            logger.info(f"Uploading the following files to {repo_id}: {','.join(os.listdir(work_dir))}")
+            return create_commit(
+                repo_id=repo_id,
+                operations=operations,
+                commit_message=commit_message,
+                token=use_auth_token,
+                create_pr=create_pr,
+                repo_type="model",
+            )
+
+    def save_quantized(self, save_dir: str, use_safetensors: bool = False, safetensors_metadata: Optional[Dict[str, str]] = None):
+        """save quantized model and configs to local disk"""
+        os.makedirs(save_dir, exist_ok=True)
+
+        if not self.quantized:
+            raise EnvironmentError("can only save quantized model, please execute .quantize first.")
+
+        self.model.to(CPU)
+
+        model_base_name = self.quantize_config.model_file_base_name or f"gptq_model-{self.quantize_config.bits}bit-{self.quantize_config.group_size}g"
+        if use_safetensors:
+            model_save_name = model_base_name + ".safetensors"
+            state_dict = self.model.state_dict()
+            state_dict = {k: v.clone().contiguous() for k, v in state_dict.items()}
+            if safetensors_metadata is None:
+                safetensors_metadata = {}
+            elif not isinstance(safetensors_metadata, dict):
+                raise TypeError("safetensors_metadata must be a dictionary.")
+            else:
+                logger.debug(f"Received safetensors_metadata: {safetensors_metadata}")
+                new_safetensors_metadata = {}
+                converted_keys = False
+                for key, value in safetensors_metadata.items():
+                    if not isinstance(key, str) or not isinstance(value, str):
+                        converted_keys = True
+                        try:
+                            new_key = str(key)
+                            new_value = str(value)
+                        except Exception as e:
+                            raise TypeError(f"safetensors_metadata: both keys and values must be strings and an error occured when trying to convert them: {e}")
+                        if new_key in new_safetensors_metadata:
+                            logger.warning(f"After converting safetensors_metadata keys to strings, the key '{new_key}' is duplicated. Ensure that all your metadata keys are strings to avoid overwriting.")
+                        new_safetensors_metadata[new_key] = new_value
+                safetensors_metadata = new_safetensors_metadata
+                if converted_keys:
+                    logger.debug(f"One or more safetensors_metadata keys or values had to be converted to str(). Final safetensors_metadata: {safetensors_metadata}")
+
+            # Format is required to enable Accelerate to load the metadata
+            # otherwise it raises an OSError
+            safetensors_metadata['format'] = "pt"
+
+            # Store the quantization configuration as safetensors metadata
+            from auto_gptq import __version__
+            safetensors_metadata['auto_gptq_version'] = str(__version__)
+            safetensors_metadata['gptq_bits'] = str(self.quantize_config.bits)
+            safetensors_metadata['gptq_group_size'] = str(self.quantize_config.group_size)
+            safetensors_metadata['gptq_desc_act'] = str(self.quantize_config.desc_act)
+            safetensors_metadata['gptq_damp_percent'] = str(self.quantize_config.damp_percent)
+
+            safe_save(state_dict, join(save_dir, model_save_name), safetensors_metadata)
+        else:
+            model_save_name = model_base_name + ".bin"
+            torch.save(self.model.state_dict(), join(save_dir, model_save_name))
+
+        self.model.config.save_pretrained(save_dir)
+        self.quantize_config.save_pretrained(save_dir)
+        self.quantize_config.model_name_or_path = save_dir
+        self.quantize_config.model_file_base_name = model_base_name
+
+    def save_pretrained(self, save_dir: str, use_safetensors: bool = False, safetensors_metadata: Optional[Dict[str, str]] = None, **kwargs):
+        """alias of save_quantized"""
+        logger.warning("you are using save_pretrained, which will re-direct to save_quantized.")
+        self.save_quantized(save_dir, use_safetensors, safetensors_metadata)
+
+    @classmethod
+    def from_pretrained(
+        cls,
+        pretrained_model_name_or_path: str,
+        quantize_config: BaseQuantizeConfig,
+        max_memory: Optional[dict] = None,
+        trust_remote_code: bool = False,
+        torch_dtype: torch.dtype = torch.float16,
+        **model_init_kwargs
+    ):
+        """load un-quantized pretrained model to cpu"""
+
+        if not torch.cuda.is_available():
+            raise EnvironmentError("Load pretrained model to do quantization requires CUDA available.")
+
+        def skip(*args, **kwargs):
+            pass
+
+        torch.nn.init.kaiming_uniform_ = skip
+        torch.nn.init.uniform_ = skip
+        torch.nn.init.normal_ = skip
+
+        # Parameters related to loading from Hugging Face Hub
+        cache_dir = model_init_kwargs.pop("cache_dir", None)
+        force_download = model_init_kwargs.pop("force_download", False)
+        resume_download = model_init_kwargs.pop("resume_download", False)
+        proxies = model_init_kwargs.pop("proxies", None)
+        local_files_only = model_init_kwargs.pop("local_files_only", False)
+        use_auth_token = model_init_kwargs.pop("use_auth_token", None)
+        revision = model_init_kwargs.pop("revision", None)
+        subfolder = model_init_kwargs.pop("subfolder", "")
+        commit_hash = model_init_kwargs.pop("_commit_hash", None)
+
+        cached_file_kwargs = {
+            "cache_dir": cache_dir,
+            "force_download": force_download,
+            "proxies": proxies,
+            "resume_download": resume_download,
+            "local_files_only": local_files_only,
+            "use_auth_token": use_auth_token,
+            "revision": revision,
+            "subfolder": subfolder,
+        }
+
+        config = AutoConfig.from_pretrained(pretrained_model_name_or_path, trust_remote_code=True, **cached_file_kwargs)
+        if config.model_type not in SUPPORTED_MODELS:
+            raise TypeError(f"{config.model_type} isn't supported yet.")
+
+        # enforce some values despite user specified
+        model_init_kwargs["torch_dtype"] = torch_dtype
+        model_init_kwargs["trust_remote_code"] = trust_remote_code
+        if max_memory:
+            if "disk" in max_memory:
+                raise NotImplementedError("disk offload not support yet.")
+            with accelerate.init_empty_weights():
+                model = AutoModelForCausalLM.from_config(config, trust_remote_code=True)
+            model.tie_weights()
+
+            max_memory = accelerate.utils.get_balanced_memory(
+                model,
+                max_memory=max_memory,
+                no_split_module_classes=[cls.layer_type],
+                dtype=model_init_kwargs["torch_dtype"],
+                low_zero=False
+            )
+            model_init_kwargs["device_map"] = accelerate.infer_auto_device_map(
+                model,
+                max_memory=max_memory,
+                no_split_module_classes=[cls.layer_type],
+                dtype=model_init_kwargs["torch_dtype"]
+            )
+            model_init_kwargs["low_cpu_mem_usage"] = True
+
+            del model
+        else:
+            model_init_kwargs["device_map"] = None
+            model_init_kwargs["low_cpu_mem_usage"] = False
+
+        torch.cuda.empty_cache()
+
+        merged_kwargs = {**model_init_kwargs, **cached_file_kwargs}
+        model = AutoModelForCausalLM.from_pretrained(pretrained_model_name_or_path, **merged_kwargs)
+
+        model_config = model.config.to_dict()
+        seq_len_keys = ["max_position_embeddings", "seq_length", "n_positions"]
+        if any([k in model_config for k in seq_len_keys]):
+            for key in seq_len_keys:
+                if key in model_config:
+                    model.seqlen = model_config[key]
+                    break
+        else:
+            logger.warning("can't get model's sequence length from model config, will set to 4096.")
+            model.seqlen = 4096
+        model.eval()
+
+        return cls(model, False, quantize_config)
+
+    @classmethod
+    def from_quantized(
+        cls,
+        model_name_or_path: Optional[str],
+        device_map: Optional[Union[str, Dict[str, Union[int, str]]]] = None,
+        max_memory: Optional[dict] = None,
+        device: Optional[Union[str, int]] = None,
+        low_cpu_mem_usage: bool = False,
+        use_triton: bool = False,
+        torch_dtype: torch.dtype = torch.float16,
+        inject_fused_attention: bool = True,
+        inject_fused_mlp: bool = True,
+        use_cuda_fp16: bool = True,
+        quantize_config: Optional[BaseQuantizeConfig] = None,
+        model_basename: Optional[str] = None,
+        use_safetensors: bool = False,
+        trust_remote_code: bool = False,
+        warmup_triton: bool = False,
+        trainable: bool = False,
+        **kwargs
+    ):
+        """load quantized model from local disk"""
+       
+        # Parameters related to loading from Hugging Face Hub
+        cache_dir = kwargs.pop("cache_dir", None)
+        force_download = kwargs.pop("force_download", False)
+        resume_download = kwargs.pop("resume_download", False)
+        proxies = kwargs.pop("proxies", None)
+        local_files_only = kwargs.pop("local_files_only", False)
+        use_auth_token = kwargs.pop("use_auth_token", None)
+        revision = kwargs.pop("revision", None)
+        subfolder = kwargs.pop("subfolder", "")
+        commit_hash = kwargs.pop("_commit_hash", None)
+
+        cached_file_kwargs = {
+            "cache_dir": cache_dir,
+            "force_download": force_download,
+            "proxies": proxies,
+            "resume_download": resume_download,
+            "local_files_only": local_files_only,
+            "use_auth_token": use_auth_token,
+            "revision": revision,
+            "subfolder": subfolder,
+            "_raise_exceptions_for_missing_entries": False,
+            "_commit_hash": commit_hash,
+        }
+            
+        if use_triton and not TRITON_AVAILABLE:
+            logger.warning("triton is not installed, reset use_triton to False")
+            use_triton = False
+
+        # == step1: prepare configs and file names == #
+        config = AutoConfig.from_pretrained(model_name_or_path, trust_remote_code=trust_remote_code, **cached_file_kwargs)
+
+        if config.model_type not in SUPPORTED_MODELS:
+            raise TypeError(f"{config.model_type} isn't supported yet.")
+
+        if quantize_config is None:
+            quantize_config = BaseQuantizeConfig.from_pretrained(model_name_or_path, **kwargs)
+        
+        if model_basename is None:
+            if quantize_config.model_file_base_name:
+                model_basename = quantize_config.model_file_base_name
+            else:
+                model_basename = f"gptq_model-{quantize_config.bits}bit-{quantize_config.group_size}g"
+        
+        quantize_config.model_name_or_path = model_name_or_path
+        quantize_config.model_file_base_name = model_basename
+
+        extensions = []
+        if use_safetensors:
+            extensions.append(".safetensors")
+        else:
+            extensions += [".bin", ".pt"]
+
+        model_name_or_path = str(model_name_or_path)
+        is_local = isdir(model_name_or_path)
+
+        resolved_archive_file = None
+        if is_local:
+            model_save_name = join(model_name_or_path, model_basename)
+            for ext in extensions:
+                if isfile(model_save_name + ext):
+                    resolved_archive_file = model_save_name + ext
+                    break
+        else: # remote
+            for ext in extensions:
+                resolved_archive_file = cached_file(model_name_or_path, model_basename + ext, **cached_file_kwargs)
+                if resolved_archive_file is not None:
+                    break
+        
+        if resolved_archive_file is None: # Could not find a model file to use
+            raise FileNotFoundError(f"Could not find model in {model_name_or_path}")
+                
+        model_save_name = resolved_archive_file
+
+        if not use_triton and trainable:
+            logger.warning("QuantLinear with cuda backend not support trainable mode yet, Switch to the pytorch backend.")
+
+        # == step2: convert model to gptq-model (replace Linear with QuantLinear) == #
+        def skip(*args, **kwargs):
+            pass
+
+        torch.nn.init.kaiming_uniform_ = skip
+        torch.nn.init.uniform_ = skip
+        torch.nn.init.normal_ = skip
+
+        transformers.modeling_utils._init_weights = False
+
+        init_contexts = [no_init_weights()]
+        if low_cpu_mem_usage:
+            init_contexts.append(accelerate.init_empty_weights(include_buffers=False))
+
+        with ContextManagers(init_contexts):
+            model = AutoModelForCausalLM.from_config(
+                config,
+                trust_remote_code=trust_remote_code,
+                torch_dtype=torch_dtype
+            )
+
+            layers = find_layers(model)
+            ignore_layers = [cls.lm_head_name] + cls.outside_layer_modules
+            for name in list(layers.keys()):
+                if any([name.startswith(ignore_layer) for ignore_layer in ignore_layers]):
+                    logger.info(f"{name} not been quantized, will be ignored when make_quant.")
+                    del layers[name]
+
+            make_quant(
+                model,
+                layers,
+                quantize_config.bits,
+                quantize_config.group_size,
+                use_triton=use_triton,
+                use_cuda_fp16=use_cuda_fp16,
+                desc_act=quantize_config.desc_act,
+                trainable=trainable
+            )
+            model.tie_weights()
+
+        # == step3: load checkpoint and dispatch == #
+        if isinstance(device_map, str) and device_map not in ["auto", "balanced", "balanced_low_0", "sequential"]:
+            raise ValueError(
+                "If passing a string for `device_map`, please choose 'auto', 'balanced', 'balanced_low_0' or "
+                "'sequential'."
+            )
+        if isinstance(device_map, dict):
+            max_memory = None
+        else:
+            if device is None and not device_map and not max_memory:
+                device_map = "auto"
+            if device is not None:
+                device = torch.device(device)
+                if not max_memory and not device_map:
+                    device_map = {"": device.index if device.type == "cuda" else device.type}
+            if not isinstance(device_map, dict) and device_map != "sequential":
+                max_memory = accelerate.utils.get_balanced_memory(
+                    model=model,
+                    max_memory=max_memory,
+                    no_split_module_classes=[cls.layer_type],
+                    low_zero=(device_map == "balanced_low_0")
+                )
+        if not isinstance(device_map, dict):
+            device_map = accelerate.infer_auto_device_map(
+                model,
+                max_memory=max_memory,
+                no_split_module_classes=[cls.layer_type]
+            )
+
+        if low_cpu_mem_usage:
+            make_sure_no_tensor_in_meta_device(model, use_triton, quantize_config.desc_act, quantize_config.group_size)
+
+        accelerate.utils.modeling.load_checkpoint_in_model(
+            model,
+            checkpoint=model_save_name,
+            device_map=device_map,
+            offload_state_dict=True,
+            offload_buffers=True
+        )
+        model = simple_dispatch_model(model, device_map)
+
+        # == step4: set seqlen == #
+        model_config = model.config.to_dict()
+        seq_len_keys = ["max_position_embeddings", "seq_length", "n_positions"]
+        if any([k in model_config for k in seq_len_keys]):
+            for key in seq_len_keys:
+                if key in model_config:
+                    model.seqlen = model_config[key]
+                    break
+        else:
+            logger.warning("can't get model's sequence length from model config, will set to 4096.")
+            model.seqlen = 4096
+
+        # == step5: (optional) inject optimized module == #
+        if inject_fused_attention:
+            if cls.fused_attn_module_type is None:
+                inject_fused_attention = False
+                logger.warning(f"{cls.__name__} hasn't fused attention module yet, will skip inject fused attention.")
+            else:
+                cls.fused_attn_module_type.inject_to_model(
+                    model,
+                    use_triton=use_triton,
+                    group_size=quantize_config.group_size,
+                    use_cuda_fp16=use_cuda_fp16,
+                    desc_act=quantize_config.desc_act,
+                    trainable=trainable
+                )
+        if inject_fused_mlp:
+            if cls.fused_mlp_module_type is None:
+                inject_fused_mlp = False
+                logger.warning(f"{cls.__name__} hasn't fused mlp module yet, will skip inject fused mlp.")
+            else:
+                cls.fused_mlp_module_type.inject_to_model(
+                    model,
+                    use_triton=use_triton
+                )
+
+        model.eval()
+        # == step6: (optional) warmup triton == #
+        if use_triton and warmup_triton:
+            from ..nn_modules.qlinear.qlinear_triton import QuantLinear
+            QuantLinear.warmup(model, seqlen=model.seqlen)
+
+            if inject_fused_mlp and cls.fused_mlp_module_type is not None:
+                cls.fused_mlp_module_type.warmup(model, seqlen=model.seqlen)
+
+        # == step7: make model compatible with peft
+        cls.make_sure_compatible_with_peft(
+            model, use_triton, quantize_config.desc_act, quantize_config.group_size
+        )
+
+        return cls(
+            model,
+            True,
+            quantize_config,
+            is_triton_backend=use_triton,
+            injected_fused_attention=inject_fused_attention,
+            injected_fused_mlp=inject_fused_mlp and use_triton,
+            trainable=trainable
+        )
+
+    def warmup_triton(self, enabled: bool = True):
+        if not enabled:
+            return
+        if not TRITON_AVAILABLE:
+            logger.warning(f"triton is not available, skip warmup stage directly.")
+            return
+
+        from ..nn_modules.qlinear.qlinear_triton import QuantLinear
+        QuantLinear.warmup(self.model, seqlen=self.model.seqlen)
+
+        if self.fused_mlp_module_type is not None:
+            self.fused_mlp_module_type.warmup(self.model, seqlen=self.model.seqlen)
+
+    def enable_trainable_mode(self, enabled: bool = True):
+        if not self.is_triton_backend and enabled:
+            raise NotImplementedError("For now, trainable mode only supports triton backend.")
+        for n, m in self.model.named_modules():
+            if hasattr(m, "trainable"):
+                setattr(m, "trainable", enabled)
+
+    def disable_trainable_mode(self):
+        self.enable_trainable_mode(enabled=False)
+
+    @staticmethod
+    def make_sure_compatible_with_peft(model: PreTrainedModel, use_triton: bool, desc_act: bool, group_size: int):
+        GeneralQuantLinear.inject_to_model(
+            model,
+            dynamically_import_QuantLinear(use_triton, desc_act, group_size)
+        )
+
+    def __getattr__(self, item):
+        try:
+            return super().__getattr__(item)
+        except:
+            return getattr(self.model, item)
+
+
+__all__ = ["BaseGPTQForCausalLM", "BaseQuantizeConfig"]
```

### Comparing `auto_gptq-0.3.0/auto_gptq/modeling/_utils.py` & `auto_gptq-0.3.1/auto_gptq/modeling/_utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-from logging import getLogger
-from typing import Union
-
-import accelerate
-import torch
-import torch.nn as nn
-from transformers import AutoConfig
-import transformers
-
-from ._const import SUPPORTED_MODELS, CPU, CUDA_0
-from ..utils.import_utils import dynamically_import_QuantLinear
-
-
-logger = getLogger(__name__)
-
-
-def get_device(obj: Union[torch.Tensor, nn.Module]):
-    if isinstance(obj, torch.Tensor):
-        return obj.device
-    return next(obj.parameters()).device
-
-
-def move_to_device(obj: Union[torch.Tensor, nn.Module], device: torch.device):
-    if get_device(obj) != device:
-        obj = obj.to(device)
-    return obj
-
-
-def find_layers(module, layers=None, name=''):
-    if not layers:
-        layers = [transformers.pytorch_utils.Conv1D, nn.Conv2d, nn.Linear]
-    for layer in layers:
-        if isinstance(module,layer):
-            return {name: module}
-    res = {}
-    for name1, child in module.named_children():
-        res.update(find_layers(child, layers=layers, name=name + '.' + name1 if name != '' else name1))
-    return res
-
-
-def get_module_by_name_prefix(model, module_name: str):
-    for name, module in model.named_modules():
-        if name.startswith(module_name):
-            return module
-
-
-def get_module_by_name_suffix(model, module_name: str):
-    for name, module in model.named_modules():
-        if name.endswith(module_name):
-            return module
-
-
-def make_quant(
-    module,
-    names,
-    bits,
-    group_size,
-    name='',
-    use_triton=False,
-    use_cuda_fp16=True,
-    desc_act=False,
-    trainable=False
-):
-    QuantLinear = dynamically_import_QuantLinear(use_triton=use_triton, desc_act=desc_act, group_size=group_size)
-
-    if isinstance(module, QuantLinear):
-        return
-    for attr in dir(module):
-        tmp = getattr(module, attr)
-        name1 = name + '.' + attr if name != '' else attr
-        if name1 in names:
-            ori_layer_device = get_device(getattr(module, attr))
-            delattr(module, attr)
-            if isinstance(tmp,nn.Linear):
-                in_features = tmp.in_features
-                out_features = tmp.out_features
-            elif isinstance(tmp,nn.Conv2d):
-                in_features = tmp.in_channels
-                out_features = tmp.out_channels
-            elif isinstance(tmp,transformers.pytorch_utils.Conv1D):            
-                in_features = tmp.weight.shape[0]
-                out_features = tmp.weight.shape[1]
-            if (not(desc_act) or group_size == -1) and not use_triton:
-                new_layer = QuantLinear(
-                    bits, group_size, in_features, out_features, True, use_cuda_fp16=use_cuda_fp16, trainable=trainable
-                )
-            else:
-                new_layer = QuantLinear(bits, group_size, in_features, out_features, True, trainable=trainable)
-            new_layer.device = ori_layer_device
-            setattr(module, attr, new_layer.to(ori_layer_device))
-    for name1, child in module.named_children():
-        make_quant(
-            child,
-            names,
-            bits,
-            group_size,
-            name + '.' + name1 if name != '' else name1,
-            use_triton=use_triton,
-            use_cuda_fp16=use_cuda_fp16,
-            desc_act=desc_act,
-            trainable=trainable
-        )
-
-
-def pack_model(
-    model,
-    quantizers,
-    bits,
-    group_size,
-    use_triton=False,
-    use_cuda_fp16=True,
-    desc_act=False,
-    warmup_triton: bool = False,
-    force_layer_back_to_cpu: bool = False
-):
-    QuantLinear = dynamically_import_QuantLinear(use_triton=use_triton, desc_act=desc_act, group_size=group_size)
-
-    if force_layer_back_to_cpu:
-        model.to(CPU)
-
-    logger.info('Packing model...')
-    layers = find_layers(model)
-    layers = {n: layers[n] for n in quantizers}
-    make_quant(model, quantizers, bits, group_size, use_triton=use_triton, use_cuda_fp16=use_cuda_fp16, desc_act=desc_act)
-    qlayers = find_layers(model, [QuantLinear])
-    for name in qlayers:
-        logger.info(name)
-        quantizers[name], scale, zero, g_idx = quantizers[name]
-        # so far can only pack layer on CPU
-        layer_device = qlayers[name].device
-        qlayers[name].to(CPU)
-        layers[name], scale, zero, g_idx = layers[name].to(CPU), scale.to(CPU), zero.to(CPU), g_idx.to(CPU)
-        qlayers[name].pack(layers[name], scale, zero, g_idx)
-        qlayers[name].to(layer_device)
-    logger.info('Model packed.')
-
-    if use_triton and warmup_triton:
-        logger.warning(
-            "using autotune_warmup will move model to GPU, make sure you have enough VRAM to load the whole model."
-        )
-        QuantLinear.warmup(model.to(CUDA_0), seqlen=model.seqlen)
-
-
-def check_and_get_model_type(model_dir, trust_remote_code=False):
-    config = AutoConfig.from_pretrained(model_dir, trust_remote_code=trust_remote_code)
-    if config.model_type not in SUPPORTED_MODELS:
-        raise TypeError(f"{config.model_type} isn't supported yet.")
-    model_type = config.model_type
-    return model_type
-
-
-def simple_dispatch_model(model, device_map):
-    from accelerate.hooks import add_hook_to_module, AlignDevicesHook
-
-    if "" in device_map:
-        d = device_map[""]
-        model = model.to(torch.device(d))
-        model.hf_device_map = device_map
-        return model
-
-    tied_params = accelerate.utils.modeling.find_tied_parameters(model)
-    if set(device_map.values()) == {"cpu"} or set(device_map.values()) == {"cpu", "disk"}:
-        main_device = "cpu"
-    else:
-        main_device = [d for d in device_map.values() if d not in ["cpu", "disk"]][0]
-
-    cpu_offload_group = [(n, d) for n, d in device_map.items() if d == "cpu"]
-    prev_hook = None
-    for idx, (n, d) in enumerate(cpu_offload_group):
-        m = get_module_by_name_suffix(model, n)
-        _, prev_hook = accelerate.cpu_offload_with_hook(m, execution_device=main_device, prev_module_hook=prev_hook)
-    # set first cpu offload module's prev_module_hook to the last cpu offload module's hook
-    if len(cpu_offload_group) > 1:
-        get_module_by_name_suffix(model, cpu_offload_group[0][0])._hf_hook.prev_module_hook = prev_hook
-
-    for n, d in device_map.items():
-        m = get_module_by_name_suffix(model, n)
-        if d != "cpu":
-            d = torch.device(d)
-            hook = AlignDevicesHook(d, io_same_device=True, place_submodules=True)
-            add_hook_to_module(m, hook)
-    accelerate.utils.modeling.retie_parameters(model, tied_params)
-    model.hf_device_map = device_map
-
-    return model
-
-
-def make_sure_no_tensor_in_meta_device(model, use_triton, desc_act, group_size):
-    QuantLinear = dynamically_import_QuantLinear(use_triton, desc_act, group_size)
-    for n, m in model.named_modules():
-        if isinstance(m, QuantLinear) and m.bias.device == torch.device("meta"):
-            m.register_buffer('bias', torch.zeros((m.outfeatures), dtype=torch.float16, device="cpu"))
-
-
-__all__ = [
-    "get_device",
-    "move_to_device",
-    "find_layers",
-    "get_module_by_name_prefix",
-    "get_module_by_name_suffix",
-    "make_quant",
-    "pack_model",
-    "check_and_get_model_type",
-    "simple_dispatch_model",
-    "make_sure_no_tensor_in_meta_device"
-]
+from logging import getLogger
+from typing import Union
+
+import accelerate
+import torch
+import torch.nn as nn
+from transformers import AutoConfig
+import transformers
+
+from ._const import SUPPORTED_MODELS, CPU, CUDA_0
+from ..utils.import_utils import dynamically_import_QuantLinear
+
+
+logger = getLogger(__name__)
+
+
+def get_device(obj: Union[torch.Tensor, nn.Module]):
+    if isinstance(obj, torch.Tensor):
+        return obj.device
+    return next(obj.parameters()).device
+
+
+def move_to_device(obj: Union[torch.Tensor, nn.Module], device: torch.device):
+    if get_device(obj) != device:
+        obj = obj.to(device)
+    return obj
+
+
+def find_layers(module, layers=None, name=''):
+    if not layers:
+        layers = [transformers.pytorch_utils.Conv1D, nn.Conv2d, nn.Linear]
+    for layer in layers:
+        if isinstance(module,layer):
+            return {name: module}
+    res = {}
+    for name1, child in module.named_children():
+        res.update(find_layers(child, layers=layers, name=name + '.' + name1 if name != '' else name1))
+    return res
+
+
+def get_module_by_name_prefix(model, module_name: str):
+    for name, module in model.named_modules():
+        if name.startswith(module_name):
+            return module
+
+
+def get_module_by_name_suffix(model, module_name: str):
+    for name, module in model.named_modules():
+        if name.endswith(module_name):
+            return module
+
+
+def make_quant(
+    module,
+    names,
+    bits,
+    group_size,
+    name='',
+    use_triton=False,
+    use_cuda_fp16=True,
+    desc_act=False,
+    trainable=False
+):
+    QuantLinear = dynamically_import_QuantLinear(use_triton=use_triton, desc_act=desc_act, group_size=group_size)
+
+    if isinstance(module, QuantLinear):
+        return
+    for attr in dir(module):
+        tmp = getattr(module, attr)
+        name1 = name + '.' + attr if name != '' else attr
+        if name1 in names:
+            ori_layer_device = get_device(getattr(module, attr))
+            delattr(module, attr)
+            if isinstance(tmp,nn.Linear):
+                in_features = tmp.in_features
+                out_features = tmp.out_features
+            elif isinstance(tmp,nn.Conv2d):
+                in_features = tmp.in_channels
+                out_features = tmp.out_channels
+            elif isinstance(tmp,transformers.pytorch_utils.Conv1D):            
+                in_features = tmp.weight.shape[0]
+                out_features = tmp.weight.shape[1]
+            if (not(desc_act) or group_size == -1) and not use_triton:
+                new_layer = QuantLinear(
+                    bits, group_size, in_features, out_features, True, use_cuda_fp16=use_cuda_fp16, trainable=trainable
+                )
+            else:
+                new_layer = QuantLinear(bits, group_size, in_features, out_features, True, trainable=trainable)
+            new_layer.device = ori_layer_device
+            setattr(module, attr, new_layer.to(ori_layer_device))
+    for name1, child in module.named_children():
+        make_quant(
+            child,
+            names,
+            bits,
+            group_size,
+            name + '.' + name1 if name != '' else name1,
+            use_triton=use_triton,
+            use_cuda_fp16=use_cuda_fp16,
+            desc_act=desc_act,
+            trainable=trainable
+        )
+
+
+def pack_model(
+    model,
+    quantizers,
+    bits,
+    group_size,
+    use_triton=False,
+    use_cuda_fp16=True,
+    desc_act=False,
+    warmup_triton: bool = False,
+    force_layer_back_to_cpu: bool = False
+):
+    QuantLinear = dynamically_import_QuantLinear(use_triton=use_triton, desc_act=desc_act, group_size=group_size)
+
+    if force_layer_back_to_cpu:
+        model.to(CPU)
+
+    logger.info('Packing model...')
+    layers = find_layers(model)
+    layers = {n: layers[n] for n in quantizers}
+    make_quant(model, quantizers, bits, group_size, use_triton=use_triton, use_cuda_fp16=use_cuda_fp16, desc_act=desc_act)
+    qlayers = find_layers(model, [QuantLinear])
+    for name in qlayers:
+        logger.info(name)
+        quantizers[name], scale, zero, g_idx = quantizers[name]
+        # so far can only pack layer on CPU
+        layer_device = qlayers[name].device
+        qlayers[name].to(CPU)
+        layers[name], scale, zero, g_idx = layers[name].to(CPU), scale.to(CPU), zero.to(CPU), g_idx.to(CPU)
+        qlayers[name].pack(layers[name], scale, zero, g_idx)
+        qlayers[name].to(layer_device)
+    logger.info('Model packed.')
+
+    if use_triton and warmup_triton:
+        logger.warning(
+            "using autotune_warmup will move model to GPU, make sure you have enough VRAM to load the whole model."
+        )
+        QuantLinear.warmup(model.to(CUDA_0), seqlen=model.seqlen)
+
+
+def check_and_get_model_type(model_dir, trust_remote_code=False):
+    config = AutoConfig.from_pretrained(model_dir, trust_remote_code=trust_remote_code)
+    if config.model_type not in SUPPORTED_MODELS:
+        raise TypeError(f"{config.model_type} isn't supported yet.")
+    model_type = config.model_type
+    return model_type
+
+
+def simple_dispatch_model(model, device_map):
+    from accelerate.hooks import add_hook_to_module, AlignDevicesHook
+
+    if "" in device_map:
+        d = device_map[""]
+        model = model.to(torch.device(d))
+        model.hf_device_map = device_map
+        return model
+
+    tied_params = accelerate.utils.modeling.find_tied_parameters(model)
+    if set(device_map.values()) == {"cpu"} or set(device_map.values()) == {"cpu", "disk"}:
+        main_device = "cpu"
+    else:
+        main_device = [d for d in device_map.values() if d not in ["cpu", "disk"]][0]
+
+    cpu_offload_group = [(n, d) for n, d in device_map.items() if d == "cpu"]
+    prev_hook = None
+    for idx, (n, d) in enumerate(cpu_offload_group):
+        m = get_module_by_name_suffix(model, n)
+        _, prev_hook = accelerate.cpu_offload_with_hook(m, execution_device=main_device, prev_module_hook=prev_hook)
+    # set first cpu offload module's prev_module_hook to the last cpu offload module's hook
+    if len(cpu_offload_group) > 1:
+        get_module_by_name_suffix(model, cpu_offload_group[0][0])._hf_hook.prev_module_hook = prev_hook
+
+    for n, d in device_map.items():
+        m = get_module_by_name_suffix(model, n)
+        if d != "cpu":
+            d = torch.device(d)
+            hook = AlignDevicesHook(d, io_same_device=True, place_submodules=True)
+            add_hook_to_module(m, hook)
+    accelerate.utils.modeling.retie_parameters(model, tied_params)
+    model.hf_device_map = device_map
+
+    return model
+
+
+def make_sure_no_tensor_in_meta_device(model, use_triton, desc_act, group_size):
+    QuantLinear = dynamically_import_QuantLinear(use_triton, desc_act, group_size)
+    for n, m in model.named_modules():
+        if isinstance(m, QuantLinear) and m.bias.device == torch.device("meta"):
+            m.register_buffer('bias', torch.zeros((m.outfeatures), dtype=torch.float16, device="cpu"))
+
+
+__all__ = [
+    "get_device",
+    "move_to_device",
+    "find_layers",
+    "get_module_by_name_prefix",
+    "get_module_by_name_suffix",
+    "make_quant",
+    "pack_model",
+    "check_and_get_model_type",
+    "simple_dispatch_model",
+    "make_sure_no_tensor_in_meta_device"
+]
```

### Comparing `auto_gptq-0.3.0/auto_gptq/modeling/gptj.py` & `auto_gptq-0.3.1/auto_gptq/modeling/gptj.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from ._base import *
-from ..nn_modules.fused_gptj_attn import FusedGPTJAttentionForQuantizedModel
-
-
-class GPTJGPTQForCausalLM(BaseGPTQForCausalLM):
-    layer_type = "GPTJBlock"
-    layers_block_name = "transformer.h"
-    outside_layer_modules = ["transformer.wte", "transformer.ln_f"]
-    inside_layer_modules = [
-        ["attn.k_proj", "attn.v_proj", "attn.q_proj"],
-        ["attn.out_proj"],
-        ["mlp.fc_in"],
-        ["mlp.fc_out"]
-    ]
-
-    fused_attn_module_type = FusedGPTJAttentionForQuantizedModel
-
-
-__all__ = ["GPTJGPTQForCausalLM"]
+from ._base import *
+from ..nn_modules.fused_gptj_attn import FusedGPTJAttentionForQuantizedModel
+
+
+class GPTJGPTQForCausalLM(BaseGPTQForCausalLM):
+    layer_type = "GPTJBlock"
+    layers_block_name = "transformer.h"
+    outside_layer_modules = ["transformer.wte", "transformer.ln_f"]
+    inside_layer_modules = [
+        ["attn.k_proj", "attn.v_proj", "attn.q_proj"],
+        ["attn.out_proj"],
+        ["mlp.fc_in"],
+        ["mlp.fc_out"]
+    ]
+
+    fused_attn_module_type = FusedGPTJAttentionForQuantizedModel
+
+
+__all__ = ["GPTJGPTQForCausalLM"]
```

### Comparing `auto_gptq-0.3.0/auto_gptq/nn_modules/fused_llama_attn.py` & `auto_gptq-0.3.1/auto_gptq/nn_modules/fused_llama_attn.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,189 +1,189 @@
-import math
-import torch
-import torch.nn as nn
-from torch.nn import functional as F
-from transformers.models.llama.modeling_llama import LlamaAttention, apply_rotary_pos_emb
-
-from ._fused_base import FusedBaseAttentionModule
-from ..utils.import_utils import compare_pytorch_version, dynamically_import_QuantLinear
-
-
-class FusedLlamaAttentionForQuantizedModel(FusedBaseAttentionModule):
-    """Multi-headed attention from 'Attention Is All You Need' paper"""
-
-    def __init__(
-        self,
-        hidden_size,
-        num_heads,
-        qkv_proj,
-        o_proj,
-        rotary_emb,
-    ):
-        super().__init__()
-        self.hidden_size = hidden_size
-        self.num_heads = num_heads
-        self.head_dim = hidden_size // num_heads
-
-        if self.head_dim * num_heads != self.hidden_size:
-            raise ValueError(
-                f"hidden_size must be divisible by num_heads (got `hidden_size`: {self.hidden_size}"
-                f" and `num_heads`: {num_heads})."
-            )
-        self.qkv_proj = qkv_proj
-        self.o_proj = o_proj
-        self.rotary_emb = rotary_emb
-
-    def _shape(self, tensor, seq_len, bsz):
-        return tensor.view(bsz, seq_len, self.num_heads, self.head_dim).transpose(1, 2).contiguous()
-
-    def forward(
-        self,
-        hidden_states,
-        past_key_value=None,
-        attention_mask=None,
-        position_ids=None,
-        output_attentions=False,
-        use_cache=False,
-        **kwargs
-    ):
-        """Input shape: Batch x Time x Channel"""
-
-        bsz, q_len, _ = hidden_states.size()
-
-        qkv_states = self.qkv_proj(hidden_states)
-        query_states, key_states, value_states = torch.split(qkv_states, self.hidden_size, dim=2)
-
-        query_states = query_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
-        key_states = key_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
-        value_states = value_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
-
-        kv_seq_len = key_states.shape[-2]
-        if past_key_value is not None:
-            kv_seq_len += past_key_value[0].shape[-2]
-        cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
-        query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin, position_ids)
-        # [bsz, nh, t, hd]
-
-        is_causal = past_key_value is None
-        if past_key_value is not None:
-            # reuse k, v, self_attention
-            key_states = torch.cat([past_key_value[0], key_states], dim=2)
-            value_states = torch.cat([past_key_value[1], value_states], dim=2)
-
-        if use_cache:
-            # Since qkv_proj is fused, query_states etc will hold a reference to the original qkv_states tensor
-            # which can cause excessive memory usage by the cache. `contiguous` is a convenient way to workaround this.
-            query_states = query_states.contiguous()
-            key_states = key_states.contiguous()
-            value_states = value_states.contiguous()
-
-        past_key_value = (key_states, value_states) if use_cache else None
-
-        if compare_pytorch_version("v2.0.0", op="eq"):
-            attn_output = F.scaled_dot_product_attention(
-                query_states,
-                key_states,
-                value_states,
-                attn_mask=None if is_causal else attention_mask,
-                is_causal=is_causal
-            )
-            attn_weights = None
-        else:
-            attn_weights = torch.matmul(query_states, key_states.transpose(2, 3)) / math.sqrt(self.head_dim)
-
-            if attn_weights.size() != (bsz, self.num_heads, q_len, kv_seq_len):
-                raise ValueError(
-                    f"Attention weights should be of size {(bsz * self.num_heads, q_len, kv_seq_len)}, but is"
-                    f" {attn_weights.size()}"
-                )
-
-            if attention_mask is not None:
-                if attention_mask.size() != (bsz, 1, q_len, kv_seq_len):
-                    raise ValueError(
-                        f"Attention mask should be of size {(bsz, 1, q_len, kv_seq_len)}, but is {attention_mask.size()}"
-                    )
-                attn_weights = attn_weights + attention_mask
-                attn_weights = torch.max(attn_weights, torch.tensor(torch.finfo(attn_weights.dtype).min))
-
-            # upcast attention to fp32
-            attn_weights = nn.functional.softmax(attn_weights, dim=-1, dtype=torch.float32).to(query_states.dtype)
-            attn_output = torch.matmul(attn_weights, value_states)
-
-        if attn_output.size() != (bsz, self.num_heads, q_len, self.head_dim):
-            raise ValueError(
-                f"`attn_output` should be of size {(bsz, self.num_heads, q_len, self.head_dim)}, but is"
-                f" {attn_output.size()}"
-            )
-
-        attn_output = attn_output.transpose(1, 2)
-        attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
-
-        attn_output = self.o_proj(attn_output)
-
-        if not output_attentions:
-            attn_weights = None
-
-        return attn_output, attn_weights, past_key_value
-
-    @classmethod
-    def inject_to_model(
-        cls,
-        model,
-        use_triton=False,
-        group_size=-1,
-        use_cuda_fp16=True,
-        desc_act=False,
-        trainable=False,
-        **kwargs
-    ):
-        """
-        Replace all LlamaAttention modules with QuantLlamaAttention modules, fusing the q, k, v projections.
-        """
-        QuantLinear = dynamically_import_QuantLinear(use_triton=use_triton, desc_act=desc_act, group_size=group_size)
-
-        for name, m in model.named_modules():
-            if not isinstance(m, LlamaAttention):
-                continue
-
-            q_proj = m.q_proj
-            k_proj = m.k_proj
-            v_proj = m.v_proj
-
-            qweights = torch.cat([q_proj.qweight, k_proj.qweight, v_proj.qweight], dim=1)
-            qzeros = torch.cat([q_proj.qzeros, k_proj.qzeros, v_proj.qzeros], dim=1)
-            scales = torch.cat([q_proj.scales, k_proj.scales, v_proj.scales], dim=1)
-            g_idx = torch.cat([q_proj.g_idx, k_proj.g_idx, v_proj.g_idx], dim=0)
-            bias = torch.cat([q_proj.bias, k_proj.bias, v_proj.bias], dim=0) if q_proj.bias is not None else None
-
-            qlinear_args = (
-                q_proj.bits,
-                q_proj.group_size,
-                q_proj.infeatures,
-                q_proj.outfeatures + k_proj.outfeatures + v_proj.outfeatures,
-                True if q_proj.bias is not None else False,
-            )
-            qlinear_kwargs = {"trainable": trainable}
-            if (not desc_act or group_size == -1) and not use_triton:
-                qlinear_kwargs["use_cuda_fp16"] = use_cuda_fp16
-            qkv_layer = QuantLinear(*qlinear_args, **qlinear_kwargs)
-            qkv_layer.qweight = qweights
-            qkv_layer.qzeros = qzeros
-            qkv_layer.scales = scales
-            qkv_layer.g_idx = g_idx
-            qkv_layer.bias = bias
-
-            attn = cls(m.hidden_size, m.num_heads, qkv_layer, m.o_proj, m.rotary_emb)
-
-            if '.' in name:
-                parent_name = name.rsplit('.', 1)[0]
-                child_name = name[len(parent_name) + 1:]
-                parent = model.get_submodule(parent_name)
-            else:
-                parent_name = ''
-                parent = model
-                child_name = name
-
-            setattr(parent, child_name, attn)
-
-
-__all__ = ["FusedLlamaAttentionForQuantizedModel"]
+import math
+import torch
+import torch.nn as nn
+from torch.nn import functional as F
+from transformers.models.llama.modeling_llama import LlamaAttention, apply_rotary_pos_emb
+
+from ._fused_base import FusedBaseAttentionModule
+from ..utils.import_utils import compare_pytorch_version, dynamically_import_QuantLinear
+
+
+class FusedLlamaAttentionForQuantizedModel(FusedBaseAttentionModule):
+    """Multi-headed attention from 'Attention Is All You Need' paper"""
+
+    def __init__(
+        self,
+        hidden_size,
+        num_heads,
+        qkv_proj,
+        o_proj,
+        rotary_emb,
+    ):
+        super().__init__()
+        self.hidden_size = hidden_size
+        self.num_heads = num_heads
+        self.head_dim = hidden_size // num_heads
+
+        if self.head_dim * num_heads != self.hidden_size:
+            raise ValueError(
+                f"hidden_size must be divisible by num_heads (got `hidden_size`: {self.hidden_size}"
+                f" and `num_heads`: {num_heads})."
+            )
+        self.qkv_proj = qkv_proj
+        self.o_proj = o_proj
+        self.rotary_emb = rotary_emb
+
+    def _shape(self, tensor, seq_len, bsz):
+        return tensor.view(bsz, seq_len, self.num_heads, self.head_dim).transpose(1, 2).contiguous()
+
+    def forward(
+        self,
+        hidden_states,
+        past_key_value=None,
+        attention_mask=None,
+        position_ids=None,
+        output_attentions=False,
+        use_cache=False,
+        **kwargs
+    ):
+        """Input shape: Batch x Time x Channel"""
+
+        bsz, q_len, _ = hidden_states.size()
+
+        qkv_states = self.qkv_proj(hidden_states)
+        query_states, key_states, value_states = torch.split(qkv_states, self.hidden_size, dim=2)
+
+        query_states = query_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
+        key_states = key_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
+        value_states = value_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
+
+        kv_seq_len = key_states.shape[-2]
+        if past_key_value is not None:
+            kv_seq_len += past_key_value[0].shape[-2]
+        cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
+        query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin, position_ids)
+        # [bsz, nh, t, hd]
+
+        is_causal = past_key_value is None
+        if past_key_value is not None:
+            # reuse k, v, self_attention
+            key_states = torch.cat([past_key_value[0], key_states], dim=2)
+            value_states = torch.cat([past_key_value[1], value_states], dim=2)
+
+        if use_cache:
+            # Since qkv_proj is fused, query_states etc will hold a reference to the original qkv_states tensor
+            # which can cause excessive memory usage by the cache. `contiguous` is a convenient way to workaround this.
+            query_states = query_states.contiguous()
+            key_states = key_states.contiguous()
+            value_states = value_states.contiguous()
+
+        past_key_value = (key_states, value_states) if use_cache else None
+
+        if compare_pytorch_version("v2.0.0", op="eq"):
+            attn_output = F.scaled_dot_product_attention(
+                query_states,
+                key_states,
+                value_states,
+                attn_mask=None if is_causal else attention_mask,
+                is_causal=is_causal
+            )
+            attn_weights = None
+        else:
+            attn_weights = torch.matmul(query_states, key_states.transpose(2, 3)) / math.sqrt(self.head_dim)
+
+            if attn_weights.size() != (bsz, self.num_heads, q_len, kv_seq_len):
+                raise ValueError(
+                    f"Attention weights should be of size {(bsz * self.num_heads, q_len, kv_seq_len)}, but is"
+                    f" {attn_weights.size()}"
+                )
+
+            if attention_mask is not None:
+                if attention_mask.size() != (bsz, 1, q_len, kv_seq_len):
+                    raise ValueError(
+                        f"Attention mask should be of size {(bsz, 1, q_len, kv_seq_len)}, but is {attention_mask.size()}"
+                    )
+                attn_weights = attn_weights + attention_mask
+                attn_weights = torch.max(attn_weights, torch.tensor(torch.finfo(attn_weights.dtype).min))
+
+            # upcast attention to fp32
+            attn_weights = nn.functional.softmax(attn_weights, dim=-1, dtype=torch.float32).to(query_states.dtype)
+            attn_output = torch.matmul(attn_weights, value_states)
+
+        if attn_output.size() != (bsz, self.num_heads, q_len, self.head_dim):
+            raise ValueError(
+                f"`attn_output` should be of size {(bsz, self.num_heads, q_len, self.head_dim)}, but is"
+                f" {attn_output.size()}"
+            )
+
+        attn_output = attn_output.transpose(1, 2)
+        attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
+
+        attn_output = self.o_proj(attn_output)
+
+        if not output_attentions:
+            attn_weights = None
+
+        return attn_output, attn_weights, past_key_value
+
+    @classmethod
+    def inject_to_model(
+        cls,
+        model,
+        use_triton=False,
+        group_size=-1,
+        use_cuda_fp16=True,
+        desc_act=False,
+        trainable=False,
+        **kwargs
+    ):
+        """
+        Replace all LlamaAttention modules with QuantLlamaAttention modules, fusing the q, k, v projections.
+        """
+        QuantLinear = dynamically_import_QuantLinear(use_triton=use_triton, desc_act=desc_act, group_size=group_size)
+
+        for name, m in model.named_modules():
+            if not isinstance(m, LlamaAttention):
+                continue
+
+            q_proj = m.q_proj
+            k_proj = m.k_proj
+            v_proj = m.v_proj
+
+            qweights = torch.cat([q_proj.qweight, k_proj.qweight, v_proj.qweight], dim=1)
+            qzeros = torch.cat([q_proj.qzeros, k_proj.qzeros, v_proj.qzeros], dim=1)
+            scales = torch.cat([q_proj.scales, k_proj.scales, v_proj.scales], dim=1)
+            g_idx = torch.cat([q_proj.g_idx, k_proj.g_idx, v_proj.g_idx], dim=0)
+            bias = torch.cat([q_proj.bias, k_proj.bias, v_proj.bias], dim=0) if q_proj.bias is not None else None
+
+            qlinear_args = (
+                q_proj.bits,
+                q_proj.group_size,
+                q_proj.infeatures,
+                q_proj.outfeatures + k_proj.outfeatures + v_proj.outfeatures,
+                True if q_proj.bias is not None else False,
+            )
+            qlinear_kwargs = {"trainable": trainable}
+            if (not desc_act or group_size == -1) and not use_triton:
+                qlinear_kwargs["use_cuda_fp16"] = use_cuda_fp16
+            qkv_layer = QuantLinear(*qlinear_args, **qlinear_kwargs)
+            qkv_layer.qweight = qweights
+            qkv_layer.qzeros = qzeros
+            qkv_layer.scales = scales
+            qkv_layer.g_idx = g_idx
+            qkv_layer.bias = bias
+
+            attn = cls(m.hidden_size, m.num_heads, qkv_layer, m.o_proj, m.rotary_emb)
+
+            if '.' in name:
+                parent_name = name.rsplit('.', 1)[0]
+                child_name = name[len(parent_name) + 1:]
+                parent = model.get_submodule(parent_name)
+            else:
+                parent_name = ''
+                parent = model
+                child_name = name
+
+            setattr(parent, child_name, attn)
+
+
+__all__ = ["FusedLlamaAttentionForQuantizedModel"]
```

### Comparing `auto_gptq-0.3.0/auto_gptq/nn_modules/fused_llama_mlp.py` & `auto_gptq-0.3.1/auto_gptq/nn_modules/fused_llama_mlp.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,330 +1,330 @@
-import math
-from logging import getLogger
-
-import torch
-from transformers.models.llama.modeling_llama import LlamaMLP
-
-from ._fused_base import FusedBaseMLPModule
-from ..utils.import_utils import TRITON_AVAILABLE
-
-logger = getLogger(__name__)
-
-if TRITON_AVAILABLE:
-    import triton
-    import triton.language as tl
-    from .triton_utils import custom_autotune
-    from .triton_utils.kernels import silu
-
-
-    @custom_autotune.autotune(
-        configs=[
-            triton.Config(
-                {
-                    'BLOCK_SIZE_M': 256,
-                    'BLOCK_SIZE_N': 64,
-                    'BLOCK_SIZE_K': 32,
-                    'GROUP_SIZE_M': 8
-                },
-                num_stages=4,
-                num_warps=4
-            ),
-            triton.Config(
-                {
-                    'BLOCK_SIZE_M': 64,
-                    'BLOCK_SIZE_N': 256,
-                    'BLOCK_SIZE_K': 32,
-                    'GROUP_SIZE_M': 8
-                },
-                num_stages=4,
-                num_warps=4
-            ),
-            triton.Config(
-                {
-                    'BLOCK_SIZE_M': 128,
-                    'BLOCK_SIZE_N': 128,
-                    'BLOCK_SIZE_K': 32,
-                    'GROUP_SIZE_M': 8
-                },
-                num_stages=4,
-                num_warps=4
-            ),
-            triton.Config(
-                {
-                    'BLOCK_SIZE_M': 128,
-                    'BLOCK_SIZE_N': 64,
-                    'BLOCK_SIZE_K': 32,
-                    'GROUP_SIZE_M': 8
-                },
-                num_stages=4,
-                num_warps=4
-            ),
-            triton.Config(
-                {
-                    'BLOCK_SIZE_M': 64,
-                    'BLOCK_SIZE_N': 128,
-                    'BLOCK_SIZE_K': 32,
-                    'GROUP_SIZE_M': 8
-                },
-                num_stages=4,
-                num_warps=4
-            ),
-            triton.Config(
-                {
-                    'BLOCK_SIZE_M': 128,
-                    'BLOCK_SIZE_N': 32,
-                    'BLOCK_SIZE_K': 32,
-                    'GROUP_SIZE_M': 8
-                },
-                num_stages=4,
-                num_warps=4
-            ),  # 3090
-            triton.Config(
-                {
-                    'BLOCK_SIZE_M': 128,
-                    'BLOCK_SIZE_N': 16,
-                    'BLOCK_SIZE_K': 32,
-                    'GROUP_SIZE_M': 8
-                },
-                num_stages=4,
-                num_warps=4
-            ),  # 3090
-            triton.Config(
-                {
-                    'BLOCK_SIZE_M': 32,
-                    'BLOCK_SIZE_N': 32,
-                    'BLOCK_SIZE_K': 128,
-                    'GROUP_SIZE_M': 8
-                },
-                num_stages=2,
-                num_warps=4
-            ),  # 3090
-            triton.Config(
-                {
-                    'BLOCK_SIZE_M': 64,
-                    'BLOCK_SIZE_N': 16,
-                    'BLOCK_SIZE_K': 64,
-                    'GROUP_SIZE_M': 8
-                },
-                num_stages=4,
-                num_warps=4
-            ),  # 3090
-            triton.Config(
-                {
-                    'BLOCK_SIZE_M': 64,
-                    'BLOCK_SIZE_N': 32,
-                    'BLOCK_SIZE_K': 64,
-                    'GROUP_SIZE_M': 8
-                },
-                num_stages=4,
-                num_warps=4
-            ),  # 3090
-        ],
-        key=['M', 'N', 'K'],
-        nearest_power_of_two=True,
-        prune_configs_by={
-            'early_config_prune': custom_autotune.matmul248_kernel_config_pruner,
-            'perf_model': None,
-            'top_k': None,
-        },
-    )
-    @triton.jit
-    def quant_fused_matmul_248_kernel(
-        a_ptr, c_ptr, b1_ptr,
-        scales1_ptr, zeros1_ptr,
-        g1_ptr, b2_ptr,
-        scales2_ptr, zeros2_ptr,
-        g2_ptr,
-        M, N, K,
-        bits, maxq,
-        stride_am, stride_ak,
-        stride_bk, stride_bn,
-        stride_cm, stride_cn,
-        stride_scales, stride_zeros,
-        BLOCK_SIZE_M: tl.constexpr, BLOCK_SIZE_N: tl.constexpr, BLOCK_SIZE_K: tl.constexpr,
-        GROUP_SIZE_M: tl.constexpr
-    ):
-        """
-        Computes: C = silu(A * B1) * (A * B2)
-        A is of shape (M, K) float16
-        B is of shape (K//8, N) int32
-        C is of shape (M, N) float16
-        scales is of shape (1, N) float16
-        zeros is of shape (1, N//8) int32
-        """
-        infearure_per_bits = 32 // bits
-
-        pid = tl.program_id(axis=0)
-        num_pid_m = tl.cdiv(M, BLOCK_SIZE_M)
-        num_pid_n = tl.cdiv(N, BLOCK_SIZE_N)
-        num_pid_k = tl.cdiv(K, BLOCK_SIZE_K)
-        num_pid_in_group = GROUP_SIZE_M * num_pid_n
-        group_id = pid // num_pid_in_group
-        first_pid_m = group_id * GROUP_SIZE_M
-        group_size_m = min(num_pid_m - first_pid_m, GROUP_SIZE_M)
-        pid_m = first_pid_m + (pid % group_size_m)
-        pid_n = (pid % num_pid_in_group) // group_size_m
-
-        offs_am = pid_m * BLOCK_SIZE_M + tl.arange(0, BLOCK_SIZE_M)
-        offs_bn = pid_n * BLOCK_SIZE_N + tl.arange(0, BLOCK_SIZE_N)
-        offs_k = tl.arange(0, BLOCK_SIZE_K)
-        a_ptrs = a_ptr + (offs_am[:, None] * stride_am + offs_k[None, :] * stride_ak)  # (BLOCK_SIZE_M, BLOCK_SIZE_K)
-        a_mask = (offs_am[:, None] < M)
-        # b_ptrs is set up such that it repeats elements along the K axis 8 times
-        b1_ptrs = b1_ptr + ((offs_k[:, None] // infearure_per_bits) * stride_bk + offs_bn[None, :] * stride_bn)
-        b2_ptrs = b2_ptr + ((offs_k[:, None] // infearure_per_bits) * stride_bk + offs_bn[None, :] * stride_bn)
-        g1_ptrs = g1_ptr + offs_k
-        g2_ptrs = g2_ptr + offs_k
-        # shifter is used to extract the N bits of each element in the 32-bit word from B
-        scales1_ptrs = scales1_ptr + offs_bn[None, :]
-        scales2_ptrs = scales2_ptr + offs_bn[None, :]
-        zeros1_ptrs = zeros1_ptr + (offs_bn[None, :] // infearure_per_bits)
-        zeros2_ptrs = zeros2_ptr + (offs_bn[None, :] // infearure_per_bits)
-
-        shifter = (offs_k % infearure_per_bits) * bits
-        zeros_shifter = (offs_bn % infearure_per_bits) * bits
-        accumulator1 = tl.zeros((BLOCK_SIZE_M, BLOCK_SIZE_N), dtype=tl.float32)
-        accumulator2 = tl.zeros((BLOCK_SIZE_M, BLOCK_SIZE_N), dtype=tl.float32)
-        for k in range(0, num_pid_k):
-            g1_idx = tl.load(g1_ptrs)
-            g2_idx = tl.load(g2_ptrs)
-
-            # Fetch scales and zeros; these are per-outfeature and thus reused in the inner loop
-            scales1 = tl.load(scales1_ptrs + g1_idx[:, None] * stride_scales)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
-            scales2 = tl.load(scales2_ptrs + g2_idx[:, None] * stride_scales)
-
-            zeros1 = tl.load(zeros1_ptrs + g1_idx[:, None] * stride_zeros)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
-            zeros1 = (zeros1 >> zeros_shifter[None, :]) & maxq
-            zeros1 = (zeros1 + 1)
-
-            zeros2 = tl.load(zeros2_ptrs + g2_idx[:, None] * stride_zeros)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
-            zeros2 = (zeros2 >> zeros_shifter[None, :]) & maxq
-            zeros2 = (zeros2 + 1)
-
-            a = tl.load(a_ptrs, mask=a_mask, other=0.)  # (BLOCK_SIZE_M, BLOCK_SIZE_K)
-            b1 = tl.load(b1_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N), but repeated
-            b2 = tl.load(b2_ptrs)
-
-            # Now we need to unpack b (which is N-bit values) into 32-bit values
-            b1 = (b1 >> shifter[:, None]) & maxq  # Extract the N-bit values
-            b1 = (b1 - zeros1) * scales1  # Scale and shift
-            accumulator1 += tl.dot(a, b1)
-
-            b2 = (b2 >> shifter[:, None]) & maxq
-            b2 = (b2 - zeros2) * scales2
-            accumulator2 += tl.dot(a, b2)
-
-            a_ptrs += BLOCK_SIZE_K
-            b1_ptrs += (BLOCK_SIZE_K // infearure_per_bits) * stride_bk
-            b2_ptrs += (BLOCK_SIZE_K // infearure_per_bits) * stride_bk
-            g1_ptrs += BLOCK_SIZE_K
-            g2_ptrs += BLOCK_SIZE_K
-
-        accumulator1 = silu(accumulator1)
-        c = accumulator1 * accumulator2
-        c = c.to(tl.float16)
-        c_ptrs = c_ptr + stride_cm * offs_am[:, None] + stride_cn * offs_bn[None, :]
-        c_mask = (offs_am[:, None] < M) & (offs_bn[None, :] < N)
-        tl.store(c_ptrs, c, mask=c_mask)
-else:
-    quant_fused_matmul_248_kernel = None
-
-
-class FusedLlamaMLPForQuantizedModel(FusedBaseMLPModule):
-    def __init__(
-        self,
-        gate_proj,
-        down_proj,
-        up_proj,
-    ):
-        super().__init__()
-
-        self.infeatures = gate_proj.infeatures
-        self.intermediate_size = gate_proj.outfeatures
-        self.outfeatures = down_proj.outfeatures
-        self.bits = gate_proj.bits
-        self.maxq = gate_proj.maxq
-
-        self.gate_proj = gate_proj
-        self.up_proj = up_proj
-        self.down_proj = down_proj
-
-    def forward(self, x):
-        return self.down_proj(self.triton_llama_mlp(x))
-
-    def triton_llama_mlp(self, x):
-        with torch.cuda.device(x.device):
-            out_shape = x.shape[:-1] + (self.intermediate_size, )
-            x = x.reshape(-1, x.shape[-1])
-            M, K = x.shape
-            N = self.intermediate_size
-            c = torch.empty((M, N), device=x.device, dtype=torch.float16)
-            grid = lambda META: (triton.cdiv(M, META['BLOCK_SIZE_M']) * triton.cdiv(N, META['BLOCK_SIZE_N']), )
-            quant_fused_matmul_248_kernel[grid](
-                x, c, self.gate_proj.qweight,
-                self.gate_proj.scales, self.gate_proj.qzeros, self.gate_proj.g_idx,
-                self.up_proj.qweight,
-                self.up_proj.scales, self.up_proj.qzeros, self.up_proj.g_idx,
-                M, N, K,
-                self.bits, self.maxq,
-                x.stride(0), x.stride(1),
-                self.gate_proj.qweight.stride(0), self.gate_proj.qweight.stride(1),
-                c.stride(0), c.stride(1),
-                self.gate_proj.scales.stride(0), self.gate_proj.qzeros.stride(0)
-            )
-            c = c.reshape(out_shape)
-            return c
-
-    @classmethod
-    def inject_to_model(cls, model, use_triton=False, **kwargs):
-        if not use_triton:
-            logger.warning(f"skip module injection for {cls.__name__} not support integrate without triton yet.")
-            return
-        elif not TRITON_AVAILABLE:
-            logger.warning(f"skip module injection for triton is not installed.")
-            return
-
-        for name, m in model.named_modules():
-            if not isinstance(m, LlamaMLP):
-                continue
-
-            mlp = cls(m.gate_proj, m.down_proj, m.up_proj)
-
-            if '.' in name:
-                parent_name = name.rsplit('.', 1)[0]
-                child_name = name[len(parent_name) + 1:]
-                parent = model.get_submodule(parent_name)
-            else:
-                parent_name = ''
-                parent = model
-                child_name = name
-
-            setattr(parent, child_name, mlp)
-
-    @classmethod
-    def warmup(cls, model, transpose=False, seqlen=2048):
-        from tqdm import tqdm
-
-        kn_values = {}
-
-        for _, m in model.named_modules():
-            if not isinstance(m, cls):
-                continue
-
-            k = m.infeatures
-            n = m.intermediate_size
-
-            if (k, n) not in kn_values:
-                kn_values[(k, n)] = m
-
-        logger.info(f'Found {len(kn_values)} unique fused mlp KN values.')
-        logger.info('Warming up autotune cache ...')
-        with torch.no_grad():
-            for m in tqdm(range(0, math.ceil(math.log2(seqlen)) + 1)):
-                m = 2 ** m
-                for (k, n), (modules) in kn_values.items():
-                    a = torch.randn(m, k, dtype=torch.float16, device=model.device)
-                    modules.triton_llama_mlp(a)
-        del kn_values
-
-
-__all__ = ["FusedLlamaMLPForQuantizedModel"]
+import math
+from logging import getLogger
+
+import torch
+from transformers.models.llama.modeling_llama import LlamaMLP
+
+from ._fused_base import FusedBaseMLPModule
+from ..utils.import_utils import TRITON_AVAILABLE
+
+logger = getLogger(__name__)
+
+if TRITON_AVAILABLE:
+    import triton
+    import triton.language as tl
+    from .triton_utils import custom_autotune
+    from .triton_utils.kernels import silu
+
+
+    @custom_autotune.autotune(
+        configs=[
+            triton.Config(
+                {
+                    'BLOCK_SIZE_M': 256,
+                    'BLOCK_SIZE_N': 64,
+                    'BLOCK_SIZE_K': 32,
+                    'GROUP_SIZE_M': 8
+                },
+                num_stages=4,
+                num_warps=4
+            ),
+            triton.Config(
+                {
+                    'BLOCK_SIZE_M': 64,
+                    'BLOCK_SIZE_N': 256,
+                    'BLOCK_SIZE_K': 32,
+                    'GROUP_SIZE_M': 8
+                },
+                num_stages=4,
+                num_warps=4
+            ),
+            triton.Config(
+                {
+                    'BLOCK_SIZE_M': 128,
+                    'BLOCK_SIZE_N': 128,
+                    'BLOCK_SIZE_K': 32,
+                    'GROUP_SIZE_M': 8
+                },
+                num_stages=4,
+                num_warps=4
+            ),
+            triton.Config(
+                {
+                    'BLOCK_SIZE_M': 128,
+                    'BLOCK_SIZE_N': 64,
+                    'BLOCK_SIZE_K': 32,
+                    'GROUP_SIZE_M': 8
+                },
+                num_stages=4,
+                num_warps=4
+            ),
+            triton.Config(
+                {
+                    'BLOCK_SIZE_M': 64,
+                    'BLOCK_SIZE_N': 128,
+                    'BLOCK_SIZE_K': 32,
+                    'GROUP_SIZE_M': 8
+                },
+                num_stages=4,
+                num_warps=4
+            ),
+            triton.Config(
+                {
+                    'BLOCK_SIZE_M': 128,
+                    'BLOCK_SIZE_N': 32,
+                    'BLOCK_SIZE_K': 32,
+                    'GROUP_SIZE_M': 8
+                },
+                num_stages=4,
+                num_warps=4
+            ),  # 3090
+            triton.Config(
+                {
+                    'BLOCK_SIZE_M': 128,
+                    'BLOCK_SIZE_N': 16,
+                    'BLOCK_SIZE_K': 32,
+                    'GROUP_SIZE_M': 8
+                },
+                num_stages=4,
+                num_warps=4
+            ),  # 3090
+            triton.Config(
+                {
+                    'BLOCK_SIZE_M': 32,
+                    'BLOCK_SIZE_N': 32,
+                    'BLOCK_SIZE_K': 128,
+                    'GROUP_SIZE_M': 8
+                },
+                num_stages=2,
+                num_warps=4
+            ),  # 3090
+            triton.Config(
+                {
+                    'BLOCK_SIZE_M': 64,
+                    'BLOCK_SIZE_N': 16,
+                    'BLOCK_SIZE_K': 64,
+                    'GROUP_SIZE_M': 8
+                },
+                num_stages=4,
+                num_warps=4
+            ),  # 3090
+            triton.Config(
+                {
+                    'BLOCK_SIZE_M': 64,
+                    'BLOCK_SIZE_N': 32,
+                    'BLOCK_SIZE_K': 64,
+                    'GROUP_SIZE_M': 8
+                },
+                num_stages=4,
+                num_warps=4
+            ),  # 3090
+        ],
+        key=['M', 'N', 'K'],
+        nearest_power_of_two=True,
+        prune_configs_by={
+            'early_config_prune': custom_autotune.matmul248_kernel_config_pruner,
+            'perf_model': None,
+            'top_k': None,
+        },
+    )
+    @triton.jit
+    def quant_fused_matmul_248_kernel(
+        a_ptr, c_ptr, b1_ptr,
+        scales1_ptr, zeros1_ptr,
+        g1_ptr, b2_ptr,
+        scales2_ptr, zeros2_ptr,
+        g2_ptr,
+        M, N, K,
+        bits, maxq,
+        stride_am, stride_ak,
+        stride_bk, stride_bn,
+        stride_cm, stride_cn,
+        stride_scales, stride_zeros,
+        BLOCK_SIZE_M: tl.constexpr, BLOCK_SIZE_N: tl.constexpr, BLOCK_SIZE_K: tl.constexpr,
+        GROUP_SIZE_M: tl.constexpr
+    ):
+        """
+        Computes: C = silu(A * B1) * (A * B2)
+        A is of shape (M, K) float16
+        B is of shape (K//8, N) int32
+        C is of shape (M, N) float16
+        scales is of shape (1, N) float16
+        zeros is of shape (1, N//8) int32
+        """
+        infearure_per_bits = 32 // bits
+
+        pid = tl.program_id(axis=0)
+        num_pid_m = tl.cdiv(M, BLOCK_SIZE_M)
+        num_pid_n = tl.cdiv(N, BLOCK_SIZE_N)
+        num_pid_k = tl.cdiv(K, BLOCK_SIZE_K)
+        num_pid_in_group = GROUP_SIZE_M * num_pid_n
+        group_id = pid // num_pid_in_group
+        first_pid_m = group_id * GROUP_SIZE_M
+        group_size_m = min(num_pid_m - first_pid_m, GROUP_SIZE_M)
+        pid_m = first_pid_m + (pid % group_size_m)
+        pid_n = (pid % num_pid_in_group) // group_size_m
+
+        offs_am = pid_m * BLOCK_SIZE_M + tl.arange(0, BLOCK_SIZE_M)
+        offs_bn = pid_n * BLOCK_SIZE_N + tl.arange(0, BLOCK_SIZE_N)
+        offs_k = tl.arange(0, BLOCK_SIZE_K)
+        a_ptrs = a_ptr + (offs_am[:, None] * stride_am + offs_k[None, :] * stride_ak)  # (BLOCK_SIZE_M, BLOCK_SIZE_K)
+        a_mask = (offs_am[:, None] < M)
+        # b_ptrs is set up such that it repeats elements along the K axis 8 times
+        b1_ptrs = b1_ptr + ((offs_k[:, None] // infearure_per_bits) * stride_bk + offs_bn[None, :] * stride_bn)
+        b2_ptrs = b2_ptr + ((offs_k[:, None] // infearure_per_bits) * stride_bk + offs_bn[None, :] * stride_bn)
+        g1_ptrs = g1_ptr + offs_k
+        g2_ptrs = g2_ptr + offs_k
+        # shifter is used to extract the N bits of each element in the 32-bit word from B
+        scales1_ptrs = scales1_ptr + offs_bn[None, :]
+        scales2_ptrs = scales2_ptr + offs_bn[None, :]
+        zeros1_ptrs = zeros1_ptr + (offs_bn[None, :] // infearure_per_bits)
+        zeros2_ptrs = zeros2_ptr + (offs_bn[None, :] // infearure_per_bits)
+
+        shifter = (offs_k % infearure_per_bits) * bits
+        zeros_shifter = (offs_bn % infearure_per_bits) * bits
+        accumulator1 = tl.zeros((BLOCK_SIZE_M, BLOCK_SIZE_N), dtype=tl.float32)
+        accumulator2 = tl.zeros((BLOCK_SIZE_M, BLOCK_SIZE_N), dtype=tl.float32)
+        for k in range(0, num_pid_k):
+            g1_idx = tl.load(g1_ptrs)
+            g2_idx = tl.load(g2_ptrs)
+
+            # Fetch scales and zeros; these are per-outfeature and thus reused in the inner loop
+            scales1 = tl.load(scales1_ptrs + g1_idx[:, None] * stride_scales)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
+            scales2 = tl.load(scales2_ptrs + g2_idx[:, None] * stride_scales)
+
+            zeros1 = tl.load(zeros1_ptrs + g1_idx[:, None] * stride_zeros)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
+            zeros1 = (zeros1 >> zeros_shifter[None, :]) & maxq
+            zeros1 = (zeros1 + 1)
+
+            zeros2 = tl.load(zeros2_ptrs + g2_idx[:, None] * stride_zeros)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
+            zeros2 = (zeros2 >> zeros_shifter[None, :]) & maxq
+            zeros2 = (zeros2 + 1)
+
+            a = tl.load(a_ptrs, mask=a_mask, other=0.)  # (BLOCK_SIZE_M, BLOCK_SIZE_K)
+            b1 = tl.load(b1_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N), but repeated
+            b2 = tl.load(b2_ptrs)
+
+            # Now we need to unpack b (which is N-bit values) into 32-bit values
+            b1 = (b1 >> shifter[:, None]) & maxq  # Extract the N-bit values
+            b1 = (b1 - zeros1) * scales1  # Scale and shift
+            accumulator1 += tl.dot(a, b1)
+
+            b2 = (b2 >> shifter[:, None]) & maxq
+            b2 = (b2 - zeros2) * scales2
+            accumulator2 += tl.dot(a, b2)
+
+            a_ptrs += BLOCK_SIZE_K
+            b1_ptrs += (BLOCK_SIZE_K // infearure_per_bits) * stride_bk
+            b2_ptrs += (BLOCK_SIZE_K // infearure_per_bits) * stride_bk
+            g1_ptrs += BLOCK_SIZE_K
+            g2_ptrs += BLOCK_SIZE_K
+
+        accumulator1 = silu(accumulator1)
+        c = accumulator1 * accumulator2
+        c = c.to(tl.float16)
+        c_ptrs = c_ptr + stride_cm * offs_am[:, None] + stride_cn * offs_bn[None, :]
+        c_mask = (offs_am[:, None] < M) & (offs_bn[None, :] < N)
+        tl.store(c_ptrs, c, mask=c_mask)
+else:
+    quant_fused_matmul_248_kernel = None
+
+
+class FusedLlamaMLPForQuantizedModel(FusedBaseMLPModule):
+    def __init__(
+        self,
+        gate_proj,
+        down_proj,
+        up_proj,
+    ):
+        super().__init__()
+
+        self.infeatures = gate_proj.infeatures
+        self.intermediate_size = gate_proj.outfeatures
+        self.outfeatures = down_proj.outfeatures
+        self.bits = gate_proj.bits
+        self.maxq = gate_proj.maxq
+
+        self.gate_proj = gate_proj
+        self.up_proj = up_proj
+        self.down_proj = down_proj
+
+    def forward(self, x):
+        return self.down_proj(self.triton_llama_mlp(x))
+
+    def triton_llama_mlp(self, x):
+        with torch.cuda.device(x.device):
+            out_shape = x.shape[:-1] + (self.intermediate_size, )
+            x = x.reshape(-1, x.shape[-1])
+            M, K = x.shape
+            N = self.intermediate_size
+            c = torch.empty((M, N), device=x.device, dtype=torch.float16)
+            grid = lambda META: (triton.cdiv(M, META['BLOCK_SIZE_M']) * triton.cdiv(N, META['BLOCK_SIZE_N']), )
+            quant_fused_matmul_248_kernel[grid](
+                x, c, self.gate_proj.qweight,
+                self.gate_proj.scales, self.gate_proj.qzeros, self.gate_proj.g_idx,
+                self.up_proj.qweight,
+                self.up_proj.scales, self.up_proj.qzeros, self.up_proj.g_idx,
+                M, N, K,
+                self.bits, self.maxq,
+                x.stride(0), x.stride(1),
+                self.gate_proj.qweight.stride(0), self.gate_proj.qweight.stride(1),
+                c.stride(0), c.stride(1),
+                self.gate_proj.scales.stride(0), self.gate_proj.qzeros.stride(0)
+            )
+            c = c.reshape(out_shape)
+            return c
+
+    @classmethod
+    def inject_to_model(cls, model, use_triton=False, **kwargs):
+        if not use_triton:
+            logger.warning(f"skip module injection for {cls.__name__} not support integrate without triton yet.")
+            return
+        elif not TRITON_AVAILABLE:
+            logger.warning(f"skip module injection for triton is not installed.")
+            return
+
+        for name, m in model.named_modules():
+            if not isinstance(m, LlamaMLP):
+                continue
+
+            mlp = cls(m.gate_proj, m.down_proj, m.up_proj)
+
+            if '.' in name:
+                parent_name = name.rsplit('.', 1)[0]
+                child_name = name[len(parent_name) + 1:]
+                parent = model.get_submodule(parent_name)
+            else:
+                parent_name = ''
+                parent = model
+                child_name = name
+
+            setattr(parent, child_name, mlp)
+
+    @classmethod
+    def warmup(cls, model, transpose=False, seqlen=2048):
+        from tqdm import tqdm
+
+        kn_values = {}
+
+        for _, m in model.named_modules():
+            if not isinstance(m, cls):
+                continue
+
+            k = m.infeatures
+            n = m.intermediate_size
+
+            if (k, n) not in kn_values:
+                kn_values[(k, n)] = m
+
+        logger.info(f'Found {len(kn_values)} unique fused mlp KN values.')
+        logger.info('Warming up autotune cache ...')
+        with torch.no_grad():
+            for m in tqdm(range(0, math.ceil(math.log2(seqlen)) + 1)):
+                m = 2 ** m
+                for (k, n), (modules) in kn_values.items():
+                    a = torch.randn(m, k, dtype=torch.float16, device=model.device)
+                    modules.triton_llama_mlp(a)
+        del kn_values
+
+
+__all__ = ["FusedLlamaMLPForQuantizedModel"]
```

### Comparing `auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/__init__.py` & `auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import torch.nn as nn
-
-
-class GeneralQuantLinear(nn.Linear):
-    def __init__(self, quant_linear_module):
-        super().__init__(
-            in_features=quant_linear_module.infeatures,
-            out_features=quant_linear_module.outfeatures,
-            bias=True
-        )
-
-        self.infeatures = quant_linear_module.infeatures
-        self.outfeatures = quant_linear_module.outfeatures
-        self.bits = quant_linear_module.bits
-        self.group_size = quant_linear_module.group_size
-        self.maxq = quant_linear_module.maxq
-
-        self.weight.requires_grad = False
-
-        self.weight.data = quant_linear_module.qweight
-        self.qweight = self.weight
-        self.bias.data = quant_linear_module.bias
-
-        self.qweight.requires_grad = False
-        self.bias.requires_grad = False
-
-        self.qzeros = quant_linear_module.qzeros
-        self.scales = quant_linear_module.scales
-        self.g_idx = quant_linear_module.g_idx
-
-        if hasattr(quant_linear_module, "wf"):
-            self.wf = quant_linear_module.wf
-        if hasattr(quant_linear_module, "kernel_switch_threshold"):
-            self.kernel_switch_threshold = quant_linear_module.kernel_switch_threshold
-        if hasattr(quant_linear_module, "autogptq_cuda_available"):
-            self.autogptq_cuda_available = quant_linear_module.autogptq_cuda_available
-
-        self.trainable = quant_linear_module.trainable
-
-        self.forward = quant_linear_module.forward
-
-    @classmethod
-    def inject_to_model(cls, model, target_module_type):
-        for name, m in model.named_modules():
-            if not isinstance(m, target_module_type):
-                continue
-            new_m = cls(m)
-            if '.' in name:
-                parent_name = name.rsplit('.', 1)[0]
-                child_name = name[len(parent_name) + 1:]
-                parent = model.get_submodule(parent_name)
-            else:
-                parent_name = ''
-                parent = model
-                child_name = name
-
-            setattr(parent, child_name, new_m)
+import torch.nn as nn
+
+
+class GeneralQuantLinear(nn.Linear):
+    def __init__(self, quant_linear_module):
+        super().__init__(
+            in_features=quant_linear_module.infeatures,
+            out_features=quant_linear_module.outfeatures,
+            bias=True
+        )
+
+        self.infeatures = quant_linear_module.infeatures
+        self.outfeatures = quant_linear_module.outfeatures
+        self.bits = quant_linear_module.bits
+        self.group_size = quant_linear_module.group_size
+        self.maxq = quant_linear_module.maxq
+
+        self.weight.requires_grad = False
+
+        self.weight.data = quant_linear_module.qweight
+        self.qweight = self.weight
+        self.bias.data = quant_linear_module.bias
+
+        self.qweight.requires_grad = False
+        self.bias.requires_grad = False
+
+        self.qzeros = quant_linear_module.qzeros
+        self.scales = quant_linear_module.scales
+        self.g_idx = quant_linear_module.g_idx
+
+        if hasattr(quant_linear_module, "wf"):
+            self.wf = quant_linear_module.wf
+        if hasattr(quant_linear_module, "kernel_switch_threshold"):
+            self.kernel_switch_threshold = quant_linear_module.kernel_switch_threshold
+        if hasattr(quant_linear_module, "autogptq_cuda_available"):
+            self.autogptq_cuda_available = quant_linear_module.autogptq_cuda_available
+
+        self.trainable = quant_linear_module.trainable
+
+        self.forward = quant_linear_module.forward
+
+    @classmethod
+    def inject_to_model(cls, model, target_module_type):
+        for name, m in model.named_modules():
+            if not isinstance(m, target_module_type):
+                continue
+            new_m = cls(m)
+            if '.' in name:
+                parent_name = name.rsplit('.', 1)[0]
+                child_name = name[len(parent_name) + 1:]
+                parent = model.get_submodule(parent_name)
+            else:
+                parent_name = ''
+                parent = model
+                child_name = name
+
+            setattr(parent, child_name, new_m)
```

### Comparing `auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/qlinear_cuda.py` & `auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/qlinear_cuda.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,271 +1,271 @@
-import math
-from logging import getLogger
-
-import numpy as np
-import torch
-import torch.nn as nn
-import transformers
-
-logger = getLogger(__name__)
-
-try:
-    import autogptq_cuda_256
-    import autogptq_cuda_64
-    _autogptq_cuda_available = True
-except ImportError:
-    logger.warning('CUDA extension not installed.')
-    _autogptq_cuda_available = False
-
-
-
-class QuantLinear(nn.Module):
-    def __init__(
-        self,
-        bits,
-        group_size,
-        infeatures,
-        outfeatures,
-        bias,
-        kernel_switch_threshold=128,
-        trainable=False
-    ):
-        super().__init__()
-        global _autogptq_cuda_available
-
-        if bits not in [2, 3, 4, 8]:
-            raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-        if trainable:
-            _autogptq_cuda_available = False
-
-        self.infeatures = infeatures
-        self.outfeatures = outfeatures
-        self.bits = bits
-        self.group_size = group_size if group_size != -1 else infeatures
-        self.maxq = 2 ** self.bits - 1
-
-        self.register_buffer(
-            'qweight',
-            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'qzeros',
-            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures // 32 * self.bits), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'scales',
-            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures), dtype=torch.float16)
-        )
-        self.register_buffer(
-            'g_idx',
-            torch.tensor([i // self.group_size for i in range(infeatures)], dtype=torch.int32)
-        )
-        if bias:
-            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
-        else:
-            self.bias = None
-
-        # is performed by unpacking the weights and using torch.matmul
-        if self.bits in [2, 4, 8]:
-            self.wf = torch.tensor(list(range(0, 32, self.bits)), dtype=torch.int32).unsqueeze(0)
-        elif self.bits == 3:
-            self.wf = torch.tensor(
-                [
-                    [0, 3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 0],
-                    [0, 1, 4, 7, 10, 13, 16, 19, 22, 25, 28, 31],
-                    [0, 2, 5, 8, 11, 14, 17, 20, 23, 26, 29, 0],
-                ],
-                dtype=torch.int32
-            ).reshape(1, 3, 12)
-
-        self.kernel_switch_threshold = kernel_switch_threshold
-        self.autogptq_cuda_available = _autogptq_cuda_available
-        
-        self.autogptq_cuda = autogptq_cuda_256
-        if infeatures % 256 != 0 or outfeatures % 256 != 0:
-            self.autogptq_cuda = autogptq_cuda_64
-        if infeatures % 64 != 0 or outfeatures % 64 != 0:
-            self.autogptq_cuda_available = False
-
-        self.trainable = trainable
-
-    def pack(self, linear, scales, zeros, g_idx=None):
-        W = linear.weight.data.clone()
-        if isinstance(linear, nn.Conv2d):
-            W = W.flatten(1)
-        if isinstance(linear, transformers.pytorch_utils.Conv1D):
-            W = W.t()
-
-        self.g_idx = g_idx.clone() if g_idx is not None else self.g_idx
-
-        scales = scales.t().contiguous()
-        zeros = zeros.t().contiguous()
-        scale_zeros = zeros * scales
-        self.scales = scales.clone().half()
-        if linear.bias is not None:
-            self.bias = linear.bias.clone().half()
-
-        intweight = []
-        for idx in range(self.infeatures):
-            intweight.append(
-                torch.round(
-                    (
-                        W[:, idx] + scale_zeros[self.g_idx[idx]]) / self.scales[self.g_idx[idx]]
-                ).to(torch.int)[:, None]
-            )
-        intweight = torch.cat(intweight, dim=1)
-        intweight = intweight.t().contiguous()
-        intweight = intweight.numpy().astype(np.uint32)
-
-        i = 0
-        row = 0
-        qweight = np.zeros(
-            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
-        )
-        while row < qweight.shape[0]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qweight[row] |= intweight[j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                row += 1
-            elif self.bits == 3:
-                for j in range(i, i + 10):
-                    qweight[row] |= intweight[j] << (3 * (j - i))
-                i += 10
-                qweight[row] |= intweight[i] << 30
-                row += 1
-                qweight[row] |= (intweight[i] >> 2) & 1
-                i += 1
-                for j in range(i, i + 10):
-                    qweight[row] |= intweight[j] << (3 * (j - i) + 1)
-                i += 10
-                qweight[row] |= intweight[i] << 31
-                row += 1
-                qweight[row] |= (intweight[i] >> 1) & 0x3
-                i += 1
-                for j in range(i, i + 10):
-                    qweight[row] |= intweight[j] << (3 * (j - i) + 2)
-                i += 10
-                row += 1
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
-        qweight = qweight.astype(np.int32)
-        self.qweight = torch.from_numpy(qweight)
-
-        zeros -= 1
-        zeros = zeros.numpy().astype(np.uint32)
-        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
-        i = 0
-        col = 0
-        while col < qzeros.shape[1]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                col += 1
-            elif self.bits == 3:
-                for j in range(i, i + 10):
-                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i))
-                i += 10
-                qzeros[:, col] |= zeros[:, i] << 30
-                col += 1
-                qzeros[:, col] |= (zeros[:, i] >> 2) & 1
-                i += 1
-                for j in range(i, i + 10):
-                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 1)
-                i += 10
-                qzeros[:, col] |= zeros[:, i] << 31
-                col += 1
-                qzeros[:, col] |= (zeros[:, i] >> 1) & 0x3
-                i += 1
-                for j in range(i, i + 10):
-                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 2)
-                i += 10
-                col += 1
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
-        qzeros = qzeros.astype(np.int32)
-        self.qzeros = torch.from_numpy(qzeros)
-
-    def forward(self, x: torch.Tensor):
-        out_shape = x.shape[:-1] + (self.outfeatures,)
-        x = x.reshape(-1, x.shape[-1])
-        if self.autogptq_cuda_available and (
-            self.kernel_switch_threshold == 0 or x.shape[0] < self.kernel_switch_threshold
-        ):
-            out = torch.zeros((x.shape[0], self.outfeatures), device=x.device, dtype=torch.float32)
-            if self.bits == 2:
-                self.autogptq_cuda.vecquant2matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
-            elif self.bits == 3:
-                self.autogptq_cuda.vecquant3matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
-            elif self.bits == 4:
-                self.autogptq_cuda.vecquant4matmul(x.half(), self.qweight, out.half(), self.scales, self.qzeros, self.g_idx, self.infeatures // 2)
-            elif self.bits == 8:
-                self.autogptq_cuda.vecquant8matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-        else:
-            if self.wf.device != self.qzeros.device:
-                self.wf = self.wf.to(self.qzeros.device)
-
-            if self.bits in [2, 4, 8]:
-                zeros = torch.bitwise_right_shift(
-                    torch.unsqueeze(self.qzeros, 2).expand(-1, -1, 32 // self.bits),
-                    self.wf.unsqueeze(0)
-                ).to(torch.int16 if self.bits == 8 else torch.int8)
-                torch.bitwise_and(zeros, (2 ** self.bits) - 1, out=zeros)
-
-                zeros = zeros + 1
-                zeros = zeros.reshape(self.scales.shape)
-
-                weight = torch.bitwise_right_shift(
-                    torch.unsqueeze(self.qweight, 1).expand(-1, 32 // self.bits, -1),
-                    self.wf.unsqueeze(-1)
-                ).to(torch.int16 if self.bits == 8 else torch.int8)
-                torch.bitwise_and(weight, (2 ** self.bits) - 1, out=weight)
-            elif self.bits == 3:
-                zeros = self.qzeros.reshape(
-                    self.qzeros.shape[0], self.qzeros.shape[1] // 3, 3, 1
-                ).expand(-1, -1, -1, 12)
-                zeros = (zeros >> self.wf.unsqueeze(0))
-                zeros[:, :, 0, 10] = (zeros[:, :, 0, 10] & 0x3) | ((zeros[:, :, 1, 0] << 2) & 0x4)
-                zeros[:, :, 1, 11] = (zeros[:, :, 1, 11] & 0x1) | ((zeros[:, :, 2, 0] << 1) & 0x6)
-                zeros = zeros & 0x7
-                zeros = torch.cat([zeros[:, :, 0, :11], zeros[:, :, 1, 1:12], zeros[:, :, 2, 1:11]], dim=2)
-
-                zeros = zeros + 1
-                zeros = zeros.reshape(self.scales.shape)
-
-                weight = self.qweight.reshape(
-                    self.qweight.shape[0] // 3, 3, 1, self.qweight.shape[1]
-                ).expand(-1, -1, 12, -1)
-                weight = (weight >> self.wf.unsqueeze(-1)) & 0x7
-                weight[:, 0, 10] = (weight[:, 0, 10] & 0x3) | ((weight[:, 1, 0] << 2) & 0x4)
-                weight[:, 1, 11] = (weight[:, 1, 11] & 0x1) | ((weight[:, 2, 0] << 1) & 0x6)
-                weight = weight & 0x7
-                weight = torch.cat([weight[:, 0, :11], weight[:, 1, 1:12], weight[:, 2, 1:11]], dim=1)
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
-            weight = weight.reshape(weight.shape[0] * weight.shape[1], weight.shape[2])
-            num_itr = self.g_idx.shape[0]//x.shape[-1]
-            if num_itr == 1:
-                weights = (self.scales[self.g_idx.long()] * (weight - zeros[self.g_idx.long()]))
-            else:
-                num_dim = self.g_idx.shape[0]//num_itr
-                weights = []
-                for i in range(num_itr):
-                    scale_i = self.scales[:,i*num_dim:(i+1)*num_dim]
-                    weight_i = weight[:,i*num_dim:(i+1)*num_dim]
-                    zeros_i = zeros[:,i*num_dim:(i+1)*num_dim]
-                    g_idx_i = self.g_idx[i*num_dim:(i+1)*num_dim]
-                    weights.append(scale_i[g_idx_i.long()] * (weight_i - zeros_i[g_idx_i.long()]))
-                weights = torch.cat(weights,dim=1)
-            out = torch.matmul(x.half(), weights)
-        out = out.half().reshape(out_shape)
-        out = out + self.bias if self.bias is not None else out
-        return out
-
-
-__all__ = ["QuantLinear"]
+import math
+from logging import getLogger
+
+import numpy as np
+import torch
+import torch.nn as nn
+import transformers
+
+logger = getLogger(__name__)
+
+try:
+    import autogptq_cuda_256
+    import autogptq_cuda_64
+    _autogptq_cuda_available = True
+except ImportError:
+    logger.warning('CUDA extension not installed.')
+    autogptq_cuda_256 = None
+    autogptq_cuda_64 = None
+    _autogptq_cuda_available = False
+
+
+class QuantLinear(nn.Module):
+    def __init__(
+        self,
+        bits,
+        group_size,
+        infeatures,
+        outfeatures,
+        bias,
+        kernel_switch_threshold=128,
+        trainable=False
+    ):
+        super().__init__()
+        global _autogptq_cuda_available
+        if bits not in [2, 3, 4, 8]:
+            raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+        if trainable:
+            _autogptq_cuda_available = False
+
+        self.infeatures = infeatures
+        self.outfeatures = outfeatures
+        self.bits = bits
+        self.group_size = group_size if group_size != -1 else infeatures
+        self.maxq = 2 ** self.bits - 1
+
+        self.register_buffer(
+            'qweight',
+            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'qzeros',
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures // 32 * self.bits), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'scales',
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures), dtype=torch.float16)
+        )
+        self.register_buffer(
+            'g_idx',
+            torch.tensor([i // self.group_size for i in range(infeatures)], dtype=torch.int32)
+        )
+        if bias:
+            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
+        else:
+            self.bias = None
+
+        # is performed by unpacking the weights and using torch.matmul
+        if self.bits in [2, 4, 8]:
+            self.wf = torch.tensor(list(range(0, 32, self.bits)), dtype=torch.int32).unsqueeze(0)
+        elif self.bits == 3:
+            self.wf = torch.tensor(
+                [
+                    [0, 3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 0],
+                    [0, 1, 4, 7, 10, 13, 16, 19, 22, 25, 28, 31],
+                    [0, 2, 5, 8, 11, 14, 17, 20, 23, 26, 29, 0],
+                ],
+                dtype=torch.int32
+            ).reshape(1, 3, 12)
+
+        self.kernel_switch_threshold = kernel_switch_threshold
+        self.autogptq_cuda_available = _autogptq_cuda_available
+        
+        self.autogptq_cuda = autogptq_cuda_256
+        if infeatures % 256 != 0 or outfeatures % 256 != 0:
+            self.autogptq_cuda = autogptq_cuda_64
+        if infeatures % 64 != 0 or outfeatures % 64 != 0:
+            self.autogptq_cuda_available = False
+
+        self.trainable = trainable
+
+    def pack(self, linear, scales, zeros, g_idx=None):
+        W = linear.weight.data.clone()
+        if isinstance(linear, nn.Conv2d):
+            W = W.flatten(1)
+        if isinstance(linear, transformers.pytorch_utils.Conv1D):
+            W = W.t()
+
+        self.g_idx = g_idx.clone() if g_idx is not None else self.g_idx
+
+        scales = scales.t().contiguous()
+        zeros = zeros.t().contiguous()
+        scale_zeros = zeros * scales
+        self.scales = scales.clone().half()
+        if linear.bias is not None:
+            self.bias = linear.bias.clone().half()
+
+        intweight = []
+        for idx in range(self.infeatures):
+            intweight.append(
+                torch.round(
+                    (
+                        W[:, idx] + scale_zeros[self.g_idx[idx]]) / self.scales[self.g_idx[idx]]
+                ).to(torch.int)[:, None]
+            )
+        intweight = torch.cat(intweight, dim=1)
+        intweight = intweight.t().contiguous()
+        intweight = intweight.numpy().astype(np.uint32)
+
+        i = 0
+        row = 0
+        qweight = np.zeros(
+            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
+        )
+        while row < qweight.shape[0]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qweight[row] |= intweight[j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                row += 1
+            elif self.bits == 3:
+                for j in range(i, i + 10):
+                    qweight[row] |= intweight[j] << (3 * (j - i))
+                i += 10
+                qweight[row] |= intweight[i] << 30
+                row += 1
+                qweight[row] |= (intweight[i] >> 2) & 1
+                i += 1
+                for j in range(i, i + 10):
+                    qweight[row] |= intweight[j] << (3 * (j - i) + 1)
+                i += 10
+                qweight[row] |= intweight[i] << 31
+                row += 1
+                qweight[row] |= (intweight[i] >> 1) & 0x3
+                i += 1
+                for j in range(i, i + 10):
+                    qweight[row] |= intweight[j] << (3 * (j - i) + 2)
+                i += 10
+                row += 1
+            else:
+                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+
+        qweight = qweight.astype(np.int32)
+        self.qweight = torch.from_numpy(qweight)
+
+        zeros -= 1
+        zeros = zeros.numpy().astype(np.uint32)
+        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
+        i = 0
+        col = 0
+        while col < qzeros.shape[1]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                col += 1
+            elif self.bits == 3:
+                for j in range(i, i + 10):
+                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i))
+                i += 10
+                qzeros[:, col] |= zeros[:, i] << 30
+                col += 1
+                qzeros[:, col] |= (zeros[:, i] >> 2) & 1
+                i += 1
+                for j in range(i, i + 10):
+                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 1)
+                i += 10
+                qzeros[:, col] |= zeros[:, i] << 31
+                col += 1
+                qzeros[:, col] |= (zeros[:, i] >> 1) & 0x3
+                i += 1
+                for j in range(i, i + 10):
+                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 2)
+                i += 10
+                col += 1
+            else:
+                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+
+        qzeros = qzeros.astype(np.int32)
+        self.qzeros = torch.from_numpy(qzeros)
+
+    def forward(self, x: torch.Tensor):
+        out_shape = x.shape[:-1] + (self.outfeatures,)
+        x = x.reshape(-1, x.shape[-1])
+        if self.autogptq_cuda_available and (
+            self.kernel_switch_threshold == 0 or x.shape[0] < self.kernel_switch_threshold
+        ):
+            out = torch.zeros((x.shape[0], self.outfeatures), device=x.device, dtype=torch.float32)
+            if self.bits == 2:
+                self.autogptq_cuda.vecquant2matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
+            elif self.bits == 3:
+                self.autogptq_cuda.vecquant3matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
+            elif self.bits == 4:
+                self.autogptq_cuda.vecquant4matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
+            elif self.bits == 8:
+                self.autogptq_cuda.vecquant8matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
+            else:
+                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+        else:
+            if self.wf.device != self.qzeros.device:
+                self.wf = self.wf.to(self.qzeros.device)
+
+            if self.bits in [2, 4, 8]:
+                zeros = torch.bitwise_right_shift(
+                    torch.unsqueeze(self.qzeros, 2).expand(-1, -1, 32 // self.bits),
+                    self.wf.unsqueeze(0)
+                ).to(torch.int16 if self.bits == 8 else torch.int8)
+                torch.bitwise_and(zeros, (2 ** self.bits) - 1, out=zeros)
+
+                zeros = zeros + 1
+                zeros = zeros.reshape(self.scales.shape)
+
+                weight = torch.bitwise_right_shift(
+                    torch.unsqueeze(self.qweight, 1).expand(-1, 32 // self.bits, -1),
+                    self.wf.unsqueeze(-1)
+                ).to(torch.int16 if self.bits == 8 else torch.int8)
+                torch.bitwise_and(weight, (2 ** self.bits) - 1, out=weight)
+            elif self.bits == 3:
+                zeros = self.qzeros.reshape(
+                    self.qzeros.shape[0], self.qzeros.shape[1] // 3, 3, 1
+                ).expand(-1, -1, -1, 12)
+                zeros = (zeros >> self.wf.unsqueeze(0))
+                zeros[:, :, 0, 10] = (zeros[:, :, 0, 10] & 0x3) | ((zeros[:, :, 1, 0] << 2) & 0x4)
+                zeros[:, :, 1, 11] = (zeros[:, :, 1, 11] & 0x1) | ((zeros[:, :, 2, 0] << 1) & 0x6)
+                zeros = zeros & 0x7
+                zeros = torch.cat([zeros[:, :, 0, :11], zeros[:, :, 1, 1:12], zeros[:, :, 2, 1:11]], dim=2)
+
+                zeros = zeros + 1
+                zeros = zeros.reshape(self.scales.shape)
+
+                weight = self.qweight.reshape(
+                    self.qweight.shape[0] // 3, 3, 1, self.qweight.shape[1]
+                ).expand(-1, -1, 12, -1)
+                weight = (weight >> self.wf.unsqueeze(-1)) & 0x7
+                weight[:, 0, 10] = (weight[:, 0, 10] & 0x3) | ((weight[:, 1, 0] << 2) & 0x4)
+                weight[:, 1, 11] = (weight[:, 1, 11] & 0x1) | ((weight[:, 2, 0] << 1) & 0x6)
+                weight = weight & 0x7
+                weight = torch.cat([weight[:, 0, :11], weight[:, 1, 1:12], weight[:, 2, 1:11]], dim=1)
+            else:
+                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+
+            weight = weight.reshape(weight.shape[0] * weight.shape[1], weight.shape[2])
+            num_itr = self.g_idx.shape[0]//x.shape[-1]
+            if num_itr == 1:
+                weights = (self.scales[self.g_idx.long()] * (weight - zeros[self.g_idx.long()]))
+            else:
+                num_dim = self.g_idx.shape[0]//num_itr
+                weights = []
+                for i in range(num_itr):
+                    scale_i = self.scales[:,i*num_dim:(i+1)*num_dim]
+                    weight_i = weight[:,i*num_dim:(i+1)*num_dim]
+                    zeros_i = zeros[:,i*num_dim:(i+1)*num_dim]
+                    g_idx_i = self.g_idx[i*num_dim:(i+1)*num_dim]
+                    weights.append(scale_i[g_idx_i.long()] * (weight_i - zeros_i[g_idx_i.long()]))
+                weights = torch.cat(weights,dim=1)
+            out = torch.matmul(x.half(), weights)
+        out = out.half().reshape(out_shape)
+        out = out + self.bias if self.bias is not None else out
+        return out
+
+
+__all__ = ["QuantLinear"]
```

### Comparing `auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/qlinear_cuda_old.py` & `auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/qlinear_cuda_old.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,268 +1,270 @@
-import math
-from logging import getLogger
-
-import numpy as np
-import torch
-import torch.nn as nn
-import transformers
-
-logger = getLogger(__name__)
-try:
-    import autogptq_cuda_256
-    import autogptq_cuda_64
-    _autogptq_cuda_available = True
-except ImportError:
-    logger.warning('CUDA extension not installed.')
-    _autogptq_cuda_available = False
-
-
-class QuantLinear(nn.Module):
-    def __init__(
-        self,
-        bits,
-        group_size,
-        infeatures,
-        outfeatures,
-        bias,
-        use_cuda_fp16=True,
-        kernel_switch_threshold=128,
-        trainable=False
-    ):
-        super().__init__()
-        global _autogptq_cuda_available
-        if bits not in [2, 3, 4, 8]:
-            raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-        if trainable:
-            _autogptq_cuda_available = False
-        self.infeatures = infeatures
-        self.outfeatures = outfeatures
-        self.bits = bits
-        self.group_size = group_size if group_size != -1 else infeatures
-        self.maxq = 2 ** self.bits - 1
-
-        self.register_buffer(
-            'qweight',
-            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'qzeros',
-            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures // 32 * self.bits), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'scales',
-            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures), dtype=torch.float16)
-        )
-        self.register_buffer(
-            'g_idx',
-            torch.tensor([i // self.group_size for i in range(infeatures)], dtype=torch.int32)
-        )
-
-        if bias:
-            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
-        else:
-            self.bias = None
-        self.half_indim = self.infeatures // 2
-
-        self.use_cuda_fp16 = use_cuda_fp16 if bits != 8 else False
-        
-        # is performed by unpacking the weights and using torch.matmul
-        if self.bits in [2, 4, 8]:
-            self.wf = torch.tensor(list(range(0, 32, self.bits)), dtype=torch.int32).unsqueeze(0)
-        elif self.bits == 3:
-            self.wf = torch.tensor(
-                [
-                    [0, 3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 0],
-                    [0, 1, 4, 7, 10, 13, 16, 19, 22, 25, 28, 31],
-                    [0, 2, 5, 8, 11, 14, 17, 20, 23, 26, 29, 0],
-                ],
-                dtype=torch.int32
-            ).reshape(1, 3, 12)
-
-        self.kernel_switch_threshold = kernel_switch_threshold
-        self.autogptq_cuda_available = _autogptq_cuda_available
-        self.autogptq_cuda = autogptq_cuda_256
-        if infeatures % 256 != 0 or outfeatures % 256 != 0:
-            self.autogptq_cuda = autogptq_cuda_64
-        if infeatures % 64 != 0 or outfeatures % 64 != 0:
-            self.autogptq_cuda_available = False
-
-        self.trainable = trainable
-
-    def pack(self, linear, scales, zeros, g_idx):
-        W = linear.weight.data.clone()
-        if isinstance(linear, nn.Conv2d):
-            W = W.flatten(1)
-        if isinstance(linear, transformers.pytorch_utils.Conv1D):
-            W = W.t()
-
-        scales = scales.t().contiguous()
-        zeros = zeros.t().contiguous()
-        scale_zeros = zeros * scales
-        self.scales = scales.clone().half()
-        if linear.bias is not None:
-            self.bias = linear.bias.clone().half()
-
-        intweight = []
-        for idx in range(self.infeatures):
-            g_idx = idx // self.group_size
-            intweight.append(
-                torch.round(
-                    (W[:, idx] + scale_zeros[g_idx]) / self.scales[g_idx]
-                ).to(torch.int)[:, None]
-            )
-        intweight = torch.cat(intweight, dim=1)
-        intweight = intweight.t().contiguous()
-        intweight = intweight.numpy().astype(np.uint32)
-
-        i = 0
-        row = 0
-        qweight = np.zeros(
-            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
-        )
-        while row < qweight.shape[0]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qweight[row] |= intweight[j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                row += 1
-            elif self.bits == 3:
-                for j in range(i, i + 10):
-                    qweight[row] |= intweight[j] << (3 * (j - i))
-                i += 10
-                qweight[row] |= intweight[i] << 30
-                row += 1
-                qweight[row] |= (intweight[i] >> 2) & 1
-                i += 1
-                for j in range(i, i + 10):
-                    qweight[row] |= intweight[j] << (3 * (j - i) + 1)
-                i += 10
-                qweight[row] |= intweight[i] << 31
-                row += 1
-                qweight[row] |= (intweight[i] >> 1) & 0x3
-                i += 1
-                for j in range(i, i + 10):
-                    qweight[row] |= intweight[j] << (3 * (j - i) + 2)
-                i += 10
-                row += 1
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
-        qweight = qweight.astype(np.int32)
-        self.qweight = torch.from_numpy(qweight)
-
-        zeros -= 1
-        zeros = zeros.numpy().astype(np.uint32)
-        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
-        i = 0
-        col = 0
-        while col < qzeros.shape[1]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                col += 1
-            elif self.bits == 3:
-                for j in range(i, i + 10):
-                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i))
-                i += 10
-                qzeros[:, col] |= zeros[:, i] << 30
-                col += 1
-                qzeros[:, col] |= (zeros[:, i] >> 2) & 1
-                i += 1
-                for j in range(i, i + 10):
-                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 1)
-                i += 10
-                qzeros[:, col] |= zeros[:, i] << 31
-                col += 1
-                qzeros[:, col] |= (zeros[:, i] >> 1) & 0x3
-                i += 1
-                for j in range(i, i + 10):
-                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 2)
-                i += 10
-                col += 1
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
-        qzeros = qzeros.astype(np.int32)
-        self.qzeros = torch.from_numpy(qzeros)
-
-    def forward(self, x):
-        out_shape = x.shape[:-1] + (self.outfeatures,)
-        x = x.reshape(-1, x.shape[-1])
-        if self.autogptq_cuda_available is True and (
-            self.kernel_switch_threshold is False or x.shape[0] < self.kernel_switch_threshold
-        ):
-            out = torch.zeros(x.shape[0], out_shape[-1], dtype=torch.float, device=x.device)
-            if self.use_cuda_fp16:
-                x = x.half()
-                if self.bits == 2:
-                    self.autogptq_cuda.vecquant2matmul_faster_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size, self.half_indim)
-                elif self.bits == 3:
-                    self.autogptq_cuda.vecquant3matmul_faster_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size, self.half_indim)
-                elif self.bits == 4:
-                    self.autogptq_cuda.vecquant4matmul_faster_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size, self.half_indim)
-
-                else:
-                    raise NotImplementedError("Only 2,3,4 bits are supported.")
-            else:
-                x = x.float()
-                if self.bits == 2:
-                    self.autogptq_cuda.vecquant2matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
-                elif self.bits == 3:
-                    self.autogptq_cuda.vecquant3matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
-                elif self.bits == 4:
-                    self.autogptq_cuda.vecquant4matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
-                elif self.bits == 8:
-                    self.autogptq_cuda.vecquant8matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
-                else:
-                    raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-        else:
-            if self.wf.device != self.qzeros.device:
-               self.wf = self.wf.to(self.qzeros.device)
-                
-            if self.bits in [2,4,8]:
-               zeros = torch.bitwise_right_shift(torch.unsqueeze(self.qzeros, 2).expand(-1, -1, 32 // self.bits), self.wf.unsqueeze(0)).to(torch.int16 if self.bits == 8 else torch.int8)
-               torch.bitwise_and(zeros, (2 ** self.bits) - 1, out=zeros)
-                   
-               zeros = zeros + 1
-               zeros = zeros.reshape(-1, 1, zeros.shape[1] * zeros.shape[2])
-   
-               scales = self.scales
-               scales = scales.reshape(-1, 1, scales.shape[-1])
-                
-               weight = torch.bitwise_right_shift(torch.unsqueeze(self.qweight, 1).expand(-1, 32 // self.bits, -1), self.wf.unsqueeze(-1)).to(torch.int16 if self.bits == 8 else torch.int8)
-               torch.bitwise_and(weight,(2 ** self.bits) - 1, out=weight)
-               weight = weight.reshape(-1, self.group_size, weight.shape[2])
-            elif self.bits == 3:
-               zeros = self.qzeros.reshape(self.qzeros.shape[0], self.qzeros.shape[1]//3, 3, 1).expand(-1, -1, -1, 12)
-               zeros = (zeros >> self.wf.unsqueeze(0))
-               zeros[:,:,0,10] = (zeros[:,:,0,10]&0x3) | ((zeros[:,:,1,0] << 2)&0x4)
-               zeros[:,:,1,11] = (zeros[:,:,1,11]&0x1) | ((zeros[:,:,2,0] << 1)&0x6)
-               zeros = zeros & 0x7
-               zeros = torch.cat([zeros[:,:,0,:11], zeros[:,:,1,1:12], zeros[:,:,2,1:11]], dim=2)
-                
-               zeros = zeros + 1
-               zeros = zeros.reshape(-1, 1, zeros.shape[1] * zeros.shape[2]) 
-               
-               scales = self.scales
-               scales = scales.reshape(-1, 1, scales.shape[-1])
-                
-               weight = self.qweight.reshape(self.qweight.shape[0]//3, 3, 1, self.qweight.shape[1]).expand(-1, -1, 12, -1)
-               weight = (weight >> self.wf.unsqueeze(-1))&0x7
-               weight[:,0,10] = (weight[:,0,10]&0x3) | ((weight[:,1,0] << 2)&0x4)
-               weight[:,1,11] = (weight[:,1,11]&0x1) | ((weight[:,2,0] << 1)&0x6)
-               weight = weight & 0x7
-               weight = torch.cat([weight[:,0,:11], weight[:,1,1:12], weight[:,2,1:11]], dim=1)
-               weight = weight.reshape(-1, self.group_size, weight.shape[2])
-            else:
-               raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-            weight = (scales * (weight - zeros))
-            weight = weight.reshape(weight.shape[0] * weight.shape[1], weight.shape[2])
-
-            out = torch.matmul(x.half(), weight)
-        out = out.half().reshape(out_shape)
-        out = out + self.bias if self.bias is not None else out
-        return out
-
-
-__all__ = ["QuantLinear"]
+import math
+from logging import getLogger
+
+import numpy as np
+import torch
+import torch.nn as nn
+import transformers
+
+logger = getLogger(__name__)
+try:
+    import autogptq_cuda_256
+    import autogptq_cuda_64
+    _autogptq_cuda_available = True
+except ImportError:
+    logger.warning('CUDA extension not installed.')
+    autogptq_cuda_256 = None
+    autogptq_cuda_64 = None
+    _autogptq_cuda_available = False
+
+
+class QuantLinear(nn.Module):
+    def __init__(
+        self,
+        bits,
+        group_size,
+        infeatures,
+        outfeatures,
+        bias,
+        use_cuda_fp16=True,
+        kernel_switch_threshold=128,
+        trainable=False
+    ):
+        super().__init__()
+        global _autogptq_cuda_available
+        if bits not in [2, 3, 4, 8]:
+            raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+        if trainable:
+            _autogptq_cuda_available = False
+        self.infeatures = infeatures
+        self.outfeatures = outfeatures
+        self.bits = bits
+        self.group_size = group_size if group_size != -1 else infeatures
+        self.maxq = 2 ** self.bits - 1
+
+        self.register_buffer(
+            'qweight',
+            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'qzeros',
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures // 32 * self.bits), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'scales',
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures), dtype=torch.float16)
+        )
+        self.register_buffer(
+            'g_idx',
+            torch.tensor([i // self.group_size for i in range(infeatures)], dtype=torch.int32)
+        )
+
+        if bias:
+            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
+        else:
+            self.bias = None
+        self.half_indim = self.infeatures // 2
+
+        self.use_cuda_fp16 = use_cuda_fp16 if bits != 8 else False
+        
+        # is performed by unpacking the weights and using torch.matmul
+        if self.bits in [2, 4, 8]:
+            self.wf = torch.tensor(list(range(0, 32, self.bits)), dtype=torch.int32).unsqueeze(0)
+        elif self.bits == 3:
+            self.wf = torch.tensor(
+                [
+                    [0, 3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 0],
+                    [0, 1, 4, 7, 10, 13, 16, 19, 22, 25, 28, 31],
+                    [0, 2, 5, 8, 11, 14, 17, 20, 23, 26, 29, 0],
+                ],
+                dtype=torch.int32
+            ).reshape(1, 3, 12)
+
+        self.kernel_switch_threshold = kernel_switch_threshold
+        self.autogptq_cuda_available = _autogptq_cuda_available
+        self.autogptq_cuda = autogptq_cuda_256
+        if infeatures % 256 != 0 or outfeatures % 256 != 0:
+            self.autogptq_cuda = autogptq_cuda_64
+        if infeatures % 64 != 0 or outfeatures % 64 != 0:
+            self.autogptq_cuda_available = False
+
+        self.trainable = trainable
+
+    def pack(self, linear, scales, zeros, g_idx):
+        W = linear.weight.data.clone()
+        if isinstance(linear, nn.Conv2d):
+            W = W.flatten(1)
+        if isinstance(linear, transformers.pytorch_utils.Conv1D):
+            W = W.t()
+
+        scales = scales.t().contiguous()
+        zeros = zeros.t().contiguous()
+        scale_zeros = zeros * scales
+        self.scales = scales.clone().half()
+        if linear.bias is not None:
+            self.bias = linear.bias.clone().half()
+
+        intweight = []
+        for idx in range(self.infeatures):
+            g_idx = idx // self.group_size
+            intweight.append(
+                torch.round(
+                    (W[:, idx] + scale_zeros[g_idx]) / self.scales[g_idx]
+                ).to(torch.int)[:, None]
+            )
+        intweight = torch.cat(intweight, dim=1)
+        intweight = intweight.t().contiguous()
+        intweight = intweight.numpy().astype(np.uint32)
+
+        i = 0
+        row = 0
+        qweight = np.zeros(
+            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
+        )
+        while row < qweight.shape[0]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qweight[row] |= intweight[j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                row += 1
+            elif self.bits == 3:
+                for j in range(i, i + 10):
+                    qweight[row] |= intweight[j] << (3 * (j - i))
+                i += 10
+                qweight[row] |= intweight[i] << 30
+                row += 1
+                qweight[row] |= (intweight[i] >> 2) & 1
+                i += 1
+                for j in range(i, i + 10):
+                    qweight[row] |= intweight[j] << (3 * (j - i) + 1)
+                i += 10
+                qweight[row] |= intweight[i] << 31
+                row += 1
+                qweight[row] |= (intweight[i] >> 1) & 0x3
+                i += 1
+                for j in range(i, i + 10):
+                    qweight[row] |= intweight[j] << (3 * (j - i) + 2)
+                i += 10
+                row += 1
+            else:
+                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+
+        qweight = qweight.astype(np.int32)
+        self.qweight = torch.from_numpy(qweight)
+
+        zeros -= 1
+        zeros = zeros.numpy().astype(np.uint32)
+        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
+        i = 0
+        col = 0
+        while col < qzeros.shape[1]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                col += 1
+            elif self.bits == 3:
+                for j in range(i, i + 10):
+                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i))
+                i += 10
+                qzeros[:, col] |= zeros[:, i] << 30
+                col += 1
+                qzeros[:, col] |= (zeros[:, i] >> 2) & 1
+                i += 1
+                for j in range(i, i + 10):
+                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 1)
+                i += 10
+                qzeros[:, col] |= zeros[:, i] << 31
+                col += 1
+                qzeros[:, col] |= (zeros[:, i] >> 1) & 0x3
+                i += 1
+                for j in range(i, i + 10):
+                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 2)
+                i += 10
+                col += 1
+            else:
+                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+
+        qzeros = qzeros.astype(np.int32)
+        self.qzeros = torch.from_numpy(qzeros)
+
+    def forward(self, x):
+        out_shape = x.shape[:-1] + (self.outfeatures,)
+        x = x.reshape(-1, x.shape[-1])
+        if self.autogptq_cuda_available is True and (
+            self.kernel_switch_threshold is False or x.shape[0] < self.kernel_switch_threshold
+        ):
+            out = torch.zeros(x.shape[0], out_shape[-1], dtype=torch.float, device=x.device)
+            if self.use_cuda_fp16:
+                x = x.half()
+                if self.bits == 2:
+                    self.autogptq_cuda.vecquant2matmul_faster_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size, self.half_indim)
+                elif self.bits == 3:
+                    self.autogptq_cuda.vecquant3matmul_faster_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size, self.half_indim)
+                elif self.bits == 4:
+                    self.autogptq_cuda.vecquant4matmul_faster_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size, self.half_indim)
+
+                else:
+                    raise NotImplementedError("Only 2,3,4 bits are supported.")
+            else:
+                x = x.float()
+                if self.bits == 2:
+                    self.autogptq_cuda.vecquant2matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
+                elif self.bits == 3:
+                    self.autogptq_cuda.vecquant3matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
+                elif self.bits == 4:
+                    self.autogptq_cuda.vecquant4matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
+                elif self.bits == 8:
+                    self.autogptq_cuda.vecquant8matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
+                else:
+                    raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+        else:
+            if self.wf.device != self.qzeros.device:
+               self.wf = self.wf.to(self.qzeros.device)
+                
+            if self.bits in [2,4,8]:
+               zeros = torch.bitwise_right_shift(torch.unsqueeze(self.qzeros, 2).expand(-1, -1, 32 // self.bits), self.wf.unsqueeze(0)).to(torch.int16 if self.bits == 8 else torch.int8)
+               torch.bitwise_and(zeros, (2 ** self.bits) - 1, out=zeros)
+                   
+               zeros = zeros + 1
+               zeros = zeros.reshape(-1, 1, zeros.shape[1] * zeros.shape[2])
+   
+               scales = self.scales
+               scales = scales.reshape(-1, 1, scales.shape[-1])
+                
+               weight = torch.bitwise_right_shift(torch.unsqueeze(self.qweight, 1).expand(-1, 32 // self.bits, -1), self.wf.unsqueeze(-1)).to(torch.int16 if self.bits == 8 else torch.int8)
+               torch.bitwise_and(weight,(2 ** self.bits) - 1, out=weight)
+               weight = weight.reshape(-1, self.group_size, weight.shape[2])
+            elif self.bits == 3:
+               zeros = self.qzeros.reshape(self.qzeros.shape[0], self.qzeros.shape[1]//3, 3, 1).expand(-1, -1, -1, 12)
+               zeros = (zeros >> self.wf.unsqueeze(0))
+               zeros[:,:,0,10] = (zeros[:,:,0,10]&0x3) | ((zeros[:,:,1,0] << 2)&0x4)
+               zeros[:,:,1,11] = (zeros[:,:,1,11]&0x1) | ((zeros[:,:,2,0] << 1)&0x6)
+               zeros = zeros & 0x7
+               zeros = torch.cat([zeros[:,:,0,:11], zeros[:,:,1,1:12], zeros[:,:,2,1:11]], dim=2)
+                
+               zeros = zeros + 1
+               zeros = zeros.reshape(-1, 1, zeros.shape[1] * zeros.shape[2]) 
+               
+               scales = self.scales
+               scales = scales.reshape(-1, 1, scales.shape[-1])
+                
+               weight = self.qweight.reshape(self.qweight.shape[0]//3, 3, 1, self.qweight.shape[1]).expand(-1, -1, 12, -1)
+               weight = (weight >> self.wf.unsqueeze(-1))&0x7
+               weight[:,0,10] = (weight[:,0,10]&0x3) | ((weight[:,1,0] << 2)&0x4)
+               weight[:,1,11] = (weight[:,1,11]&0x1) | ((weight[:,2,0] << 1)&0x6)
+               weight = weight & 0x7
+               weight = torch.cat([weight[:,0,:11], weight[:,1,1:12], weight[:,2,1:11]], dim=1)
+               weight = weight.reshape(-1, self.group_size, weight.shape[2])
+            else:
+               raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+            weight = (scales * (weight - zeros))
+            weight = weight.reshape(weight.shape[0] * weight.shape[1], weight.shape[2])
+
+            out = torch.matmul(x.half(), weight)
+        out = out.half().reshape(out_shape)
+        out = out + self.bias if self.bias is not None else out
+        return out
+
+
+__all__ = ["QuantLinear"]
```

### Comparing `auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/qlinear_triton.py` & `auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/qlinear_triton.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-import math
-from logging import getLogger
-
-import numpy as np
-import torch
-import torch.nn as nn
-import transformers
-
-from ..triton_utils.mixin import TritonModuleMixin
-
-logger = getLogger(__name__)
-
-try:
-    from ..triton_utils.kernels import (
-        quant_matmul_248, transpose_quant_matmul_248, quant_matmul_inference_only_248,
-        QuantLinearFunction, QuantLinearInferenceOnlyFunction
-    )
-except ImportError:
-    logger.error('triton not installed.')
-    raise
-
-
-class QuantLinear(nn.Module, TritonModuleMixin):
-    def __init__(
-        self,
-        bits,
-        group_size,
-        infeatures,
-        outfeatures,
-        bias,
-        trainable=False
-    ):
-        super().__init__()
-        if bits not in [2, 4, 8]:
-            raise NotImplementedError("Only 2,4,8 bits are supported.")
-        if infeatures % 32 != 0 or outfeatures % 32 != 0:
-            raise NotImplementedError("in_feature and out_feature must be divisible by 32.")
-        self.infeatures = infeatures
-        self.outfeatures = outfeatures
-        self.bits = bits
-        self.group_size = group_size if group_size != -1 else infeatures
-        self.maxq = 2 ** self.bits - 1
-
-        self.register_buffer(
-            'qweight',
-            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'qzeros',
-            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures // 32 * self.bits), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'scales',
-            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures), dtype=torch.float16)
-        )
-        self.register_buffer(
-            'g_idx',
-            torch.tensor([i // self.group_size for i in range(infeatures)], dtype=torch.int32)
-        )
-        if bias:
-            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
-        else:
-            self.bias = None
-
-        self.trainable = trainable
-
-    def pack(self, linear, scales, zeros, g_idx=None):
-        W = linear.weight.data.clone()
-        if isinstance(linear, nn.Conv2d):
-            W = W.flatten(1)
-        if isinstance(linear, transformers.pytorch_utils.Conv1D):
-            W = W.t()
-    
-        self.g_idx = g_idx.clone() if g_idx is not None else self.g_idx
-
-        scales = scales.t().contiguous()
-        zeros = zeros.t().contiguous()
-        scale_zeros = zeros * scales
-        self.scales = scales.clone().half()
-        if linear.bias is not None:
-            self.bias = linear.bias.clone().half()
-
-        intweight = []
-        for idx in range(self.infeatures):
-            intweight.append(
-                torch.round(
-                    (
-                        W[:, idx] + scale_zeros[self.g_idx[idx]]) / self.scales[self.g_idx[idx]]
-                ).to(torch.int)[:, None]
-            )
-        intweight = torch.cat(intweight, dim=1)
-        intweight = intweight.t().contiguous()
-        intweight = intweight.numpy().astype(np.uint32)
-
-        i = 0
-        row = 0
-        qweight = np.zeros(
-            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
-        )
-        while row < qweight.shape[0]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qweight[row] |= intweight[j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                row += 1
-            else:
-                raise NotImplementedError("Only 2,4,8 bits are supported.")
-
-        qweight = qweight.astype(np.int32)
-        self.qweight = torch.from_numpy(qweight)
-
-        zeros -= 1
-        zeros = zeros.numpy().astype(np.uint32)
-        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
-        i = 0
-        col = 0
-        while col < qzeros.shape[1]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                col += 1
-            else:
-                raise NotImplementedError("Only 2,4,8 bits are supported.")
-
-        qzeros = qzeros.astype(np.int32)
-        self.qzeros = torch.from_numpy(qzeros)
-
-    def forward(self, x):
-        out_shape = x.shape[:-1] + (self.outfeatures,)
-        quant_linear_fn = QuantLinearFunction if self.trainable else QuantLinearInferenceOnlyFunction
-        out = quant_linear_fn.apply(
-            x.reshape(-1, x.shape[-1]),
-            self.qweight,
-            self.scales,
-            self.qzeros,
-            self.g_idx,
-            self.bits,
-            self.maxq
-        )
-        out = out.half().reshape(out_shape)
-        out = out + self.bias if self.bias is not None else out
-        return out
-
-    @classmethod
-    def warmup(cls, model, transpose=False, seqlen=2048):
-        """
-        Pre-tunes the quantized kernel
-        """
-        from tqdm import tqdm
-
-        kn_values = {}
-
-        for _, m in model.named_modules():
-            if not isinstance(m, cls):
-                continue
-
-            k = m.infeatures
-            n = m.outfeatures
-
-            if (k, n) not in kn_values:
-                kn_values[(k, n)] = (m.qweight, m.scales, m.qzeros, m.g_idx, m.bits, m.maxq)
-
-        logger.info(f'Found {len(kn_values)} unique KN Linear values.')
-        logger.info('Warming up autotune cache ...')
-        with torch.no_grad():
-            for m in tqdm(range(0, math.ceil(math.log2(seqlen)) + 1)):
-                m = 2 ** m
-                for (k, n), (qweight, scales, qzeros, g_idx, bits, maxq) in kn_values.items():
-                    if transpose:
-                        a = torch.randn(m, k, dtype=torch.float16, device=model.device)
-                        quant_matmul_248(a, qweight, scales, qzeros, g_idx, bits, maxq)
-                        a = torch.randn(m, n, dtype=torch.float16, device=model.device)
-                        transpose_quant_matmul_248(a, qweight, scales, qzeros, g_idx, bits, maxq)
-                    else:
-                        a = torch.randn(m, k, dtype=torch.float16, device=model.device)
-                        quant_matmul_inference_only_248(a, qweight, scales, qzeros, g_idx, bits, maxq)
-        del kn_values
-
-
-__all__ = ["QuantLinear"]
+import math
+from logging import getLogger
+
+import numpy as np
+import torch
+import torch.nn as nn
+import transformers
+
+from ..triton_utils.mixin import TritonModuleMixin
+
+logger = getLogger(__name__)
+
+try:
+    from ..triton_utils.kernels import (
+        quant_matmul_248, transpose_quant_matmul_248, quant_matmul_inference_only_248,
+        QuantLinearFunction, QuantLinearInferenceOnlyFunction
+    )
+except ImportError:
+    logger.error('triton not installed.')
+    raise
+
+
+class QuantLinear(nn.Module, TritonModuleMixin):
+    def __init__(
+        self,
+        bits,
+        group_size,
+        infeatures,
+        outfeatures,
+        bias,
+        trainable=False
+    ):
+        super().__init__()
+        if bits not in [2, 4, 8]:
+            raise NotImplementedError("Only 2,4,8 bits are supported.")
+        if infeatures % 32 != 0 or outfeatures % 32 != 0:
+            raise NotImplementedError("in_feature and out_feature must be divisible by 32.")
+        self.infeatures = infeatures
+        self.outfeatures = outfeatures
+        self.bits = bits
+        self.group_size = group_size if group_size != -1 else infeatures
+        self.maxq = 2 ** self.bits - 1
+
+        self.register_buffer(
+            'qweight',
+            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'qzeros',
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures // 32 * self.bits), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'scales',
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures), dtype=torch.float16)
+        )
+        self.register_buffer(
+            'g_idx',
+            torch.tensor([i // self.group_size for i in range(infeatures)], dtype=torch.int32)
+        )
+        if bias:
+            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
+        else:
+            self.bias = None
+
+        self.trainable = trainable
+
+    def pack(self, linear, scales, zeros, g_idx=None):
+        W = linear.weight.data.clone()
+        if isinstance(linear, nn.Conv2d):
+            W = W.flatten(1)
+        if isinstance(linear, transformers.pytorch_utils.Conv1D):
+            W = W.t()
+    
+        self.g_idx = g_idx.clone() if g_idx is not None else self.g_idx
+
+        scales = scales.t().contiguous()
+        zeros = zeros.t().contiguous()
+        scale_zeros = zeros * scales
+        self.scales = scales.clone().half()
+        if linear.bias is not None:
+            self.bias = linear.bias.clone().half()
+
+        intweight = []
+        for idx in range(self.infeatures):
+            intweight.append(
+                torch.round(
+                    (
+                        W[:, idx] + scale_zeros[self.g_idx[idx]]) / self.scales[self.g_idx[idx]]
+                ).to(torch.int)[:, None]
+            )
+        intweight = torch.cat(intweight, dim=1)
+        intweight = intweight.t().contiguous()
+        intweight = intweight.numpy().astype(np.uint32)
+
+        i = 0
+        row = 0
+        qweight = np.zeros(
+            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
+        )
+        while row < qweight.shape[0]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qweight[row] |= intweight[j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                row += 1
+            else:
+                raise NotImplementedError("Only 2,4,8 bits are supported.")
+
+        qweight = qweight.astype(np.int32)
+        self.qweight = torch.from_numpy(qweight)
+
+        zeros -= 1
+        zeros = zeros.numpy().astype(np.uint32)
+        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
+        i = 0
+        col = 0
+        while col < qzeros.shape[1]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                col += 1
+            else:
+                raise NotImplementedError("Only 2,4,8 bits are supported.")
+
+        qzeros = qzeros.astype(np.int32)
+        self.qzeros = torch.from_numpy(qzeros)
+
+    def forward(self, x):
+        out_shape = x.shape[:-1] + (self.outfeatures,)
+        quant_linear_fn = QuantLinearFunction if self.trainable else QuantLinearInferenceOnlyFunction
+        out = quant_linear_fn.apply(
+            x.reshape(-1, x.shape[-1]),
+            self.qweight,
+            self.scales,
+            self.qzeros,
+            self.g_idx,
+            self.bits,
+            self.maxq
+        )
+        out = out.half().reshape(out_shape)
+        out = out + self.bias if self.bias is not None else out
+        return out
+
+    @classmethod
+    def warmup(cls, model, transpose=False, seqlen=2048):
+        """
+        Pre-tunes the quantized kernel
+        """
+        from tqdm import tqdm
+
+        kn_values = {}
+
+        for _, m in model.named_modules():
+            if not isinstance(m, cls):
+                continue
+
+            k = m.infeatures
+            n = m.outfeatures
+
+            if (k, n) not in kn_values:
+                kn_values[(k, n)] = (m.qweight, m.scales, m.qzeros, m.g_idx, m.bits, m.maxq)
+
+        logger.info(f'Found {len(kn_values)} unique KN Linear values.')
+        logger.info('Warming up autotune cache ...')
+        with torch.no_grad():
+            for m in tqdm(range(0, math.ceil(math.log2(seqlen)) + 1)):
+                m = 2 ** m
+                for (k, n), (qweight, scales, qzeros, g_idx, bits, maxq) in kn_values.items():
+                    if transpose:
+                        a = torch.randn(m, k, dtype=torch.float16, device=model.device)
+                        quant_matmul_248(a, qweight, scales, qzeros, g_idx, bits, maxq)
+                        a = torch.randn(m, n, dtype=torch.float16, device=model.device)
+                        transpose_quant_matmul_248(a, qweight, scales, qzeros, g_idx, bits, maxq)
+                    else:
+                        a = torch.randn(m, k, dtype=torch.float16, device=model.device)
+                        quant_matmul_inference_only_248(a, qweight, scales, qzeros, g_idx, bits, maxq)
+        del kn_values
+
+
+__all__ = ["QuantLinear"]
```

### Comparing `auto_gptq-0.3.0/auto_gptq/nn_modules/triton_utils/custom_autotune.py` & `auto_gptq-0.3.1/auto_gptq/nn_modules/triton_utils/custom_autotune.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-import builtins
-import math
-import time
-from typing import Dict
-
-import triton
-
-
-#  code based https://github.com/fpgaminer/GPTQ-triton
-"""
-Mostly the same as the autotuner in Triton, but with a few changes like using 40 runs instead of 100.
-"""
-
-
-class CustomizedTritonAutoTuner(triton.KernelInterface):
-    def __init__(
-        self,
-        fn,
-        arg_names,
-        configs,
-        key,
-        reset_to_zero,
-        prune_configs_by: Dict = None,
-        nearest_power_of_two: bool = False
-    ):
-        if not configs:
-            self.configs = [triton.Config({}, num_warps=4, num_stages=2)]
-        else:
-            self.configs = configs
-        self.key_idx = [arg_names.index(k) for k in key]
-        self.nearest_power_of_two = nearest_power_of_two
-        self.cache = {}
-        # hook to reset all required tensor to zeros before relaunching a kernel
-        self.hook = lambda args: 0
-        if reset_to_zero is not None:
-            self.reset_idx = [arg_names.index(k) for k in reset_to_zero]
-
-            def _hook(args):
-                for i in self.reset_idx:
-                    args[i].zero_()
-
-            self.hook = _hook
-        self.arg_names = arg_names
-        # prune configs
-        if prune_configs_by:
-            perf_model, top_k = prune_configs_by['perf_model'], prune_configs_by['top_k']
-            if 'early_config_prune' in prune_configs_by:
-                early_config_prune = prune_configs_by['early_config_prune']
-        else:
-            perf_model, top_k, early_config_prune = None, None, None
-        self.perf_model, self.configs_top_k = perf_model, top_k
-        self.early_config_prune = early_config_prune
-        self.fn = fn
-
-    def _bench(self, *args, config, **meta):
-        # check for conflicts, i.e. meta-parameters both provided
-        # as kwargs and by the autotuner
-        conflicts = meta.keys() & config.kwargs.keys()
-        if conflicts:
-            raise ValueError(f"Conflicting meta-parameters: {', '.join(conflicts)}."
-                             " Make sure that you don't re-define auto-tuned symbols.")
-        # augment meta-parameters with tunable ones
-        current = dict(meta, **config.kwargs)
-
-        def kernel_call():
-            if config.pre_hook:
-                config.pre_hook(self.nargs)
-            self.hook(args)
-            self.fn.run(*args, num_warps=config.num_warps, num_stages=config.num_stages, **current)
-
-        try:
-            # In testings using only 40 reps seems to be close enough and it appears to be what PyTorch uses
-            # PyTorch also sets fast_flush to True, but I didn't see any speedup so I'll leave the default
-            return triton.testing.do_bench(kernel_call, percentiles=(0.5, 0.2, 0.8), rep=40)
-        except triton.compiler.OutOfResources:
-            return (float('inf'), float('inf'), float('inf'))
-
-    def run(self, *args, **kwargs):
-        self.nargs = dict(zip(self.arg_names, args))
-        if len(self.configs) > 1:
-            key = tuple(args[i] for i in self.key_idx)
-
-            # This reduces the amount of autotuning by rounding the keys to the nearest power of two
-            # In my testing this gives decent results, and greatly reduces the amount of tuning required
-            if self.nearest_power_of_two:
-                key = tuple([2 ** int(math.log2(x) + 0.5) for x in key])
-
-            if key not in self.cache:
-                # prune configs
-                pruned_configs = self.prune_configs(kwargs)
-                bench_start = time.time()
-                timings = {config: self._bench(*args, config=config, **kwargs) for config in pruned_configs}
-                bench_end = time.time()
-                self.bench_time = bench_end - bench_start
-                self.cache[key] = builtins.min(timings, key=timings.get)
-                self.hook(args)
-                self.configs_timings = timings
-            config = self.cache[key]
-        else:
-            config = self.configs[0]
-        self.best_config = config
-        if config.pre_hook is not None:
-            config.pre_hook(self.nargs)
-        return self.fn.run(*args, num_warps=config.num_warps, num_stages=config.num_stages, **kwargs, **config.kwargs)
-
-    def prune_configs(self, kwargs):
-        pruned_configs = self.configs
-        if self.early_config_prune:
-            pruned_configs = self.early_config_prune(self.configs, self.nargs)
-        if self.perf_model:
-            top_k = self.configs_top_k
-            if isinstance(top_k, float) and top_k <= 1.0:
-                top_k = int(len(self.configs) * top_k)
-            if len(pruned_configs) > top_k:
-                est_timing = {
-                    config: self.perf_model(**self.nargs, **kwargs, **config.kwargs, num_stages=config.num_stages,
-                                            num_warps=config.num_warps) for config in pruned_configs}
-                pruned_configs = sorted(est_timing.keys(), key=lambda x: est_timing[x])[:top_k]
-        return pruned_configs
-
-    def warmup(self, *args, **kwargs):
-        self.nargs = dict(zip(self.arg_names, args))
-        for config in self.prune_configs(kwargs):
-            self.fn.warmup(
-                *args,
-                num_warps=config.num_warps,
-                num_stages=config.num_stages,
-                **kwargs,
-                **config.kwargs,
-            )
-        self.nargs = None
-
-
-def autotune(configs, key, prune_configs_by=None, reset_to_zero=None, nearest_power_of_two=False):
-    def decorator(fn):
-        return CustomizedTritonAutoTuner(
-            fn, fn.arg_names, configs, key, reset_to_zero, prune_configs_by, nearest_power_of_two
-        )
-
-    return decorator
-
-
-def matmul248_kernel_config_pruner(configs, nargs):
-    """
-    The main purpose of this function is to shrink BLOCK_SIZE_* when the corresponding dimension is smaller.
-    """
-    m = max(2 ** int(math.ceil(math.log2(nargs['M']))), 16)
-    n = max(2 ** int(math.ceil(math.log2(nargs['N']))), 16)
-    k = max(2 ** int(math.ceil(math.log2(nargs['K']))), 16)
-
-    used = set()
-    for config in configs:
-        block_size_m = min(m, config.kwargs['BLOCK_SIZE_M'])
-        block_size_n = min(n, config.kwargs['BLOCK_SIZE_N'])
-        block_size_k = min(k, config.kwargs['BLOCK_SIZE_K'])
-        group_size_m = config.kwargs['GROUP_SIZE_M']
-
-        if (block_size_m, block_size_n, block_size_k, group_size_m, config.num_stages, config.num_warps) in used:
-            continue
-
-        used.add((block_size_m, block_size_n, block_size_k, group_size_m, config.num_stages, config.num_warps))
-        yield triton.Config(
-            {
-                'BLOCK_SIZE_M': block_size_m,
-                'BLOCK_SIZE_N': block_size_n,
-                'BLOCK_SIZE_K': block_size_k,
-                'GROUP_SIZE_M': group_size_m
-            },
-            num_stages=config.num_stages,
-            num_warps=config.num_warps
-        )
-
-
-__all__ = ["autotune"]
+import builtins
+import math
+import time
+from typing import Dict
+
+import triton
+
+
+#  code based https://github.com/fpgaminer/GPTQ-triton
+"""
+Mostly the same as the autotuner in Triton, but with a few changes like using 40 runs instead of 100.
+"""
+
+
+class CustomizedTritonAutoTuner(triton.KernelInterface):
+    def __init__(
+        self,
+        fn,
+        arg_names,
+        configs,
+        key,
+        reset_to_zero,
+        prune_configs_by: Dict = None,
+        nearest_power_of_two: bool = False
+    ):
+        if not configs:
+            self.configs = [triton.Config({}, num_warps=4, num_stages=2)]
+        else:
+            self.configs = configs
+        self.key_idx = [arg_names.index(k) for k in key]
+        self.nearest_power_of_two = nearest_power_of_two
+        self.cache = {}
+        # hook to reset all required tensor to zeros before relaunching a kernel
+        self.hook = lambda args: 0
+        if reset_to_zero is not None:
+            self.reset_idx = [arg_names.index(k) for k in reset_to_zero]
+
+            def _hook(args):
+                for i in self.reset_idx:
+                    args[i].zero_()
+
+            self.hook = _hook
+        self.arg_names = arg_names
+        # prune configs
+        if prune_configs_by:
+            perf_model, top_k = prune_configs_by['perf_model'], prune_configs_by['top_k']
+            if 'early_config_prune' in prune_configs_by:
+                early_config_prune = prune_configs_by['early_config_prune']
+        else:
+            perf_model, top_k, early_config_prune = None, None, None
+        self.perf_model, self.configs_top_k = perf_model, top_k
+        self.early_config_prune = early_config_prune
+        self.fn = fn
+
+    def _bench(self, *args, config, **meta):
+        # check for conflicts, i.e. meta-parameters both provided
+        # as kwargs and by the autotuner
+        conflicts = meta.keys() & config.kwargs.keys()
+        if conflicts:
+            raise ValueError(f"Conflicting meta-parameters: {', '.join(conflicts)}."
+                             " Make sure that you don't re-define auto-tuned symbols.")
+        # augment meta-parameters with tunable ones
+        current = dict(meta, **config.kwargs)
+
+        def kernel_call():
+            if config.pre_hook:
+                config.pre_hook(self.nargs)
+            self.hook(args)
+            self.fn.run(*args, num_warps=config.num_warps, num_stages=config.num_stages, **current)
+
+        try:
+            # In testings using only 40 reps seems to be close enough and it appears to be what PyTorch uses
+            # PyTorch also sets fast_flush to True, but I didn't see any speedup so I'll leave the default
+            return triton.testing.do_bench(kernel_call, percentiles=(0.5, 0.2, 0.8), rep=40)
+        except triton.compiler.OutOfResources:
+            return (float('inf'), float('inf'), float('inf'))
+
+    def run(self, *args, **kwargs):
+        self.nargs = dict(zip(self.arg_names, args))
+        if len(self.configs) > 1:
+            key = tuple(args[i] for i in self.key_idx)
+
+            # This reduces the amount of autotuning by rounding the keys to the nearest power of two
+            # In my testing this gives decent results, and greatly reduces the amount of tuning required
+            if self.nearest_power_of_two:
+                key = tuple([2 ** int(math.log2(x) + 0.5) for x in key])
+
+            if key not in self.cache:
+                # prune configs
+                pruned_configs = self.prune_configs(kwargs)
+                bench_start = time.time()
+                timings = {config: self._bench(*args, config=config, **kwargs) for config in pruned_configs}
+                bench_end = time.time()
+                self.bench_time = bench_end - bench_start
+                self.cache[key] = builtins.min(timings, key=timings.get)
+                self.hook(args)
+                self.configs_timings = timings
+            config = self.cache[key]
+        else:
+            config = self.configs[0]
+        self.best_config = config
+        if config.pre_hook is not None:
+            config.pre_hook(self.nargs)
+        return self.fn.run(*args, num_warps=config.num_warps, num_stages=config.num_stages, **kwargs, **config.kwargs)
+
+    def prune_configs(self, kwargs):
+        pruned_configs = self.configs
+        if self.early_config_prune:
+            pruned_configs = self.early_config_prune(self.configs, self.nargs)
+        if self.perf_model:
+            top_k = self.configs_top_k
+            if isinstance(top_k, float) and top_k <= 1.0:
+                top_k = int(len(self.configs) * top_k)
+            if len(pruned_configs) > top_k:
+                est_timing = {
+                    config: self.perf_model(**self.nargs, **kwargs, **config.kwargs, num_stages=config.num_stages,
+                                            num_warps=config.num_warps) for config in pruned_configs}
+                pruned_configs = sorted(est_timing.keys(), key=lambda x: est_timing[x])[:top_k]
+        return pruned_configs
+
+    def warmup(self, *args, **kwargs):
+        self.nargs = dict(zip(self.arg_names, args))
+        for config in self.prune_configs(kwargs):
+            self.fn.warmup(
+                *args,
+                num_warps=config.num_warps,
+                num_stages=config.num_stages,
+                **kwargs,
+                **config.kwargs,
+            )
+        self.nargs = None
+
+
+def autotune(configs, key, prune_configs_by=None, reset_to_zero=None, nearest_power_of_two=False):
+    def decorator(fn):
+        return CustomizedTritonAutoTuner(
+            fn, fn.arg_names, configs, key, reset_to_zero, prune_configs_by, nearest_power_of_two
+        )
+
+    return decorator
+
+
+def matmul248_kernel_config_pruner(configs, nargs):
+    """
+    The main purpose of this function is to shrink BLOCK_SIZE_* when the corresponding dimension is smaller.
+    """
+    m = max(2 ** int(math.ceil(math.log2(nargs['M']))), 16)
+    n = max(2 ** int(math.ceil(math.log2(nargs['N']))), 16)
+    k = max(2 ** int(math.ceil(math.log2(nargs['K']))), 16)
+
+    used = set()
+    for config in configs:
+        block_size_m = min(m, config.kwargs['BLOCK_SIZE_M'])
+        block_size_n = min(n, config.kwargs['BLOCK_SIZE_N'])
+        block_size_k = min(k, config.kwargs['BLOCK_SIZE_K'])
+        group_size_m = config.kwargs['GROUP_SIZE_M']
+
+        if (block_size_m, block_size_n, block_size_k, group_size_m, config.num_stages, config.num_warps) in used:
+            continue
+
+        used.add((block_size_m, block_size_n, block_size_k, group_size_m, config.num_stages, config.num_warps))
+        yield triton.Config(
+            {
+                'BLOCK_SIZE_M': block_size_m,
+                'BLOCK_SIZE_N': block_size_n,
+                'BLOCK_SIZE_K': block_size_k,
+                'GROUP_SIZE_M': group_size_m
+            },
+            num_stages=config.num_stages,
+            num_warps=config.num_warps
+        )
+
+
+__all__ = ["autotune"]
```

### Comparing `auto_gptq-0.3.0/auto_gptq/quantization/gptq.py` & `auto_gptq-0.3.1/auto_gptq/quantization/gptq.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-import math
-import os
-import time
-from logging import getLogger
-
-import torch
-import torch.nn as nn
-import transformers
-
-from .quantizer import Quantizer
-
-
-logger = getLogger(__name__)
-
-torch.backends.cuda.matmul.allow_tf32 = False
-torch.backends.cudnn.allow_tf32 = False
-
-
-class GPTQ:
-    def __init__(self, layer):
-        self.layer = layer
-        self.dev = self.layer.weight.device
-        W = layer.weight.data.clone()
-        if isinstance(self.layer, nn.Conv2d):
-            W = W.flatten(1)
-        if isinstance(self.layer, transformers.pytorch_utils.Conv1D):
-            W = W.t()
-        self.rows = W.shape[0]
-        self.columns = W.shape[1]
-        self.H = torch.zeros((self.columns, self.columns), device=self.dev)
-        self.nsamples = 0
-        self.quantizer = Quantizer()
-
-    def add_batch(self, inp, out):
-        if os.environ.get("DEBUG"):
-            self.inp1 = inp
-            self.out1 = out
-        if len(inp.shape) == 2:
-            inp = inp.unsqueeze(0)
-        tmp = inp.shape[0]
-        if isinstance(self.layer, nn.Linear) or isinstance(self.layer, transformers.Conv1D):
-            if len(inp.shape) == 3:
-                inp = inp.reshape((-1, inp.shape[-1]))
-            inp = inp.t()
-        if isinstance(self.layer, nn.Conv2d):
-            unfold = nn.Unfold(
-                self.layer.kernel_size,
-                dilation=self.layer.dilation,
-                padding=self.layer.padding,
-                stride=self.layer.stride
-            )
-            inp = unfold(inp)
-            inp = inp.permute([1, 0, 2])
-            inp = inp.flatten(1)
-        self.H *= self.nsamples / (self.nsamples + tmp)
-        self.nsamples += tmp
-        # inp = inp.float()
-        inp = math.sqrt(2 / self.nsamples) * inp.float()
-        # self.H += 2 / self.nsamples * inp.matmul(inp.t())
-        self.H += inp.matmul(inp.t())
-
-    def fasterquant(
-        self, blocksize=128, percdamp=.01, group_size=-1, actorder=False
-    ):
-        W = self.layer.weight.data.clone()
-        if isinstance(self.layer, nn.Conv2d):
-            W = W.flatten(1)
-        if isinstance(self.layer, transformers.Conv1D):
-            W = W.t()
-        W = W.float()
-
-        tick = time.time()
-
-        if not self.quantizer.ready():
-            self.quantizer.find_params(W, weight=True)
-
-        H = self.H
-        del self.H
-        dead = torch.diag(H) == 0
-        H[dead, dead] = 1
-        W[:, dead] = 0
-
-        if actorder:
-            perm = torch.argsort(torch.diag(H), descending=True)
-            W = W[:, perm]
-            H = H[perm][:, perm]
-
-        Losses = torch.zeros_like(W)
-        Q = torch.zeros_like(W)
-
-        damp = percdamp * torch.mean(torch.diag(H))
-        diag = torch.arange(self.columns, device=self.dev)
-        H[diag, diag] += damp
-        H = torch.linalg.cholesky(H)
-        H = torch.cholesky_inverse(H)
-        H = torch.linalg.cholesky(H, upper=True)
-        Hinv = H
-
-        g_idx = []
-        scale = []
-        zero = []
-        now_idx = 1
-
-        for i1 in range(0, self.columns, blocksize):
-            i2 = min(i1 + blocksize, self.columns)
-            count = i2 - i1
-
-            W1 = W[:, i1:i2].clone()
-            Q1 = torch.zeros_like(W1)
-            Err1 = torch.zeros_like(W1)
-            Losses1 = torch.zeros_like(W1)
-            Hinv1 = Hinv[i1:i2, i1:i2]
-
-            for i in range(count):
-                w = W1[:, i]
-                d = Hinv1[i, i]
-
-                if group_size != -1:
-                    if (i1 + i) % group_size == 0:
-                        self.quantizer.find_params(W[:, (i1 + i):(i1 + i + group_size)], weight=True)
-
-                    if ((i1 + i) // group_size) - now_idx == -1:
-                        scale.append(self.quantizer.scale)
-                        zero.append(self.quantizer.zero)
-                        now_idx += 1
-
-                q = self.quantizer.quantize(w.unsqueeze(1)).flatten()
-                Q1[:, i] = q
-                Losses1[:, i] = (w - q) ** 2 / d ** 2
-
-                err1 = (w - q) / d
-                W1[:, i:] -= err1.unsqueeze(1).matmul(Hinv1[i, i:].unsqueeze(0))
-                Err1[:, i] = err1
-
-            Q[:, i1:i2] = Q1
-            Losses[:, i1:i2] = Losses1 / 2
-
-            W[:, i2:] -= Err1.matmul(Hinv[i1:i2, i2:])
-
-            if os.environ.get("DEBUG"):
-                self.layer.weight.data[:, :i2] = Q[:, :i2]
-                self.layer.weight.data[:, i2:] = W[:, i2:]
-                logger.debug(torch.sum((self.layer(self.inp1) - self.out1) ** 2))
-                logger.debug(torch.sum(Losses))
-
-        torch.cuda.synchronize()
-        logger.info(f'duration: {(time.time() - tick)}')
-        logger.info(f'avg loss: {torch.sum(Losses).item() / self.nsamples}')
-
-        group_size = group_size if group_size != -1 else self.columns
-        g_idx = [i // group_size for i in range(self.columns)]
-        g_idx = torch.tensor(g_idx, dtype=torch.int32, device=Q.device)
-        if actorder:
-            invperm = torch.argsort(perm)
-            Q = Q[:, invperm]
-            g_idx = g_idx[invperm]
-
-        if isinstance(self.layer, transformers.Conv1D):
-            Q = Q.t()
-        self.layer.weight.data = Q.reshape(self.layer.weight.shape).type_as(self.layer.weight.data)
-        if os.environ.get("DEBUG"):
-            logger.debug(torch.sum((self.layer(self.inp1) - self.out1) ** 2))
-
-        if scale == []:
-            scale.append(self.quantizer.scale)
-            zero.append(self.quantizer.zero)
-        scale = torch.cat(scale, dim=1)
-        zero = torch.cat(zero, dim=1)
-        return scale, zero, g_idx
-
-    def free(self):
-        if os.environ.get("DEBUG"):
-            self.inp1 = None
-            self.out1 = None
-        self.H = None
-        self.Losses = None
-        self.Trace = None
-        torch.cuda.empty_cache()
-
-
-__all__ = ["GPTQ"]
+import math
+import os
+import time
+from logging import getLogger
+
+import torch
+import torch.nn as nn
+import transformers
+
+from .quantizer import Quantizer
+
+
+logger = getLogger(__name__)
+
+torch.backends.cuda.matmul.allow_tf32 = False
+torch.backends.cudnn.allow_tf32 = False
+
+
+class GPTQ:
+    def __init__(self, layer):
+        self.layer = layer
+        self.dev = self.layer.weight.device
+        W = layer.weight.data.clone()
+        if isinstance(self.layer, nn.Conv2d):
+            W = W.flatten(1)
+        if isinstance(self.layer, transformers.pytorch_utils.Conv1D):
+            W = W.t()
+        self.rows = W.shape[0]
+        self.columns = W.shape[1]
+        self.H = torch.zeros((self.columns, self.columns), device=self.dev)
+        self.nsamples = 0
+        self.quantizer = Quantizer()
+
+    def add_batch(self, inp, out):
+        if os.environ.get("DEBUG"):
+            self.inp1 = inp
+            self.out1 = out
+        if len(inp.shape) == 2:
+            inp = inp.unsqueeze(0)
+        tmp = inp.shape[0]
+        if isinstance(self.layer, nn.Linear) or isinstance(self.layer, transformers.Conv1D):
+            if len(inp.shape) == 3:
+                inp = inp.reshape((-1, inp.shape[-1]))
+            inp = inp.t()
+        if isinstance(self.layer, nn.Conv2d):
+            unfold = nn.Unfold(
+                self.layer.kernel_size,
+                dilation=self.layer.dilation,
+                padding=self.layer.padding,
+                stride=self.layer.stride
+            )
+            inp = unfold(inp)
+            inp = inp.permute([1, 0, 2])
+            inp = inp.flatten(1)
+        self.H *= self.nsamples / (self.nsamples + tmp)
+        self.nsamples += tmp
+        # inp = inp.float()
+        inp = math.sqrt(2 / self.nsamples) * inp.float()
+        # self.H += 2 / self.nsamples * inp.matmul(inp.t())
+        self.H += inp.matmul(inp.t())
+
+    def fasterquant(
+        self, blocksize=128, percdamp=.01, group_size=-1, actorder=False
+    ):
+        W = self.layer.weight.data.clone()
+        if isinstance(self.layer, nn.Conv2d):
+            W = W.flatten(1)
+        if isinstance(self.layer, transformers.Conv1D):
+            W = W.t()
+        W = W.float()
+
+        tick = time.time()
+
+        if not self.quantizer.ready():
+            self.quantizer.find_params(W, weight=True)
+
+        H = self.H
+        del self.H
+        dead = torch.diag(H) == 0
+        H[dead, dead] = 1
+        W[:, dead] = 0
+
+        if actorder:
+            perm = torch.argsort(torch.diag(H), descending=True)
+            W = W[:, perm]
+            H = H[perm][:, perm]
+
+        Losses = torch.zeros_like(W)
+        Q = torch.zeros_like(W)
+
+        damp = percdamp * torch.mean(torch.diag(H))
+        diag = torch.arange(self.columns, device=self.dev)
+        H[diag, diag] += damp
+        H = torch.linalg.cholesky(H)
+        H = torch.cholesky_inverse(H)
+        H = torch.linalg.cholesky(H, upper=True)
+        Hinv = H
+
+        g_idx = []
+        scale = []
+        zero = []
+        now_idx = 1
+
+        for i1 in range(0, self.columns, blocksize):
+            i2 = min(i1 + blocksize, self.columns)
+            count = i2 - i1
+
+            W1 = W[:, i1:i2].clone()
+            Q1 = torch.zeros_like(W1)
+            Err1 = torch.zeros_like(W1)
+            Losses1 = torch.zeros_like(W1)
+            Hinv1 = Hinv[i1:i2, i1:i2]
+
+            for i in range(count):
+                w = W1[:, i]
+                d = Hinv1[i, i]
+
+                if group_size != -1:
+                    if (i1 + i) % group_size == 0:
+                        self.quantizer.find_params(W[:, (i1 + i):(i1 + i + group_size)], weight=True)
+
+                    if ((i1 + i) // group_size) - now_idx == -1:
+                        scale.append(self.quantizer.scale)
+                        zero.append(self.quantizer.zero)
+                        now_idx += 1
+
+                q = self.quantizer.quantize(w.unsqueeze(1)).flatten()
+                Q1[:, i] = q
+                Losses1[:, i] = (w - q) ** 2 / d ** 2
+
+                err1 = (w - q) / d
+                W1[:, i:] -= err1.unsqueeze(1).matmul(Hinv1[i, i:].unsqueeze(0))
+                Err1[:, i] = err1
+
+            Q[:, i1:i2] = Q1
+            Losses[:, i1:i2] = Losses1 / 2
+
+            W[:, i2:] -= Err1.matmul(Hinv[i1:i2, i2:])
+
+            if os.environ.get("DEBUG"):
+                self.layer.weight.data[:, :i2] = Q[:, :i2]
+                self.layer.weight.data[:, i2:] = W[:, i2:]
+                logger.debug(torch.sum((self.layer(self.inp1) - self.out1) ** 2))
+                logger.debug(torch.sum(Losses))
+
+        torch.cuda.synchronize()
+        logger.info(f'duration: {(time.time() - tick)}')
+        logger.info(f'avg loss: {torch.sum(Losses).item() / self.nsamples}')
+
+        group_size = group_size if group_size != -1 else self.columns
+        g_idx = [i // group_size for i in range(self.columns)]
+        g_idx = torch.tensor(g_idx, dtype=torch.int32, device=Q.device)
+        if actorder:
+            invperm = torch.argsort(perm)
+            Q = Q[:, invperm]
+            g_idx = g_idx[invperm]
+
+        if isinstance(self.layer, transformers.Conv1D):
+            Q = Q.t()
+        self.layer.weight.data = Q.reshape(self.layer.weight.shape).type_as(self.layer.weight.data)
+        if os.environ.get("DEBUG"):
+            logger.debug(torch.sum((self.layer(self.inp1) - self.out1) ** 2))
+
+        if scale == []:
+            scale.append(self.quantizer.scale)
+            zero.append(self.quantizer.zero)
+        scale = torch.cat(scale, dim=1)
+        zero = torch.cat(zero, dim=1)
+        return scale, zero, g_idx
+
+    def free(self):
+        if os.environ.get("DEBUG"):
+            self.inp1 = None
+            self.out1 = None
+        self.H = None
+        self.Losses = None
+        self.Trace = None
+        torch.cuda.empty_cache()
+
+
+__all__ = ["GPTQ"]
```

### Comparing `auto_gptq-0.3.0/auto_gptq/quantization/quantizer.py` & `auto_gptq-0.3.1/auto_gptq/quantization/quantizer.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-from logging import getLogger
-
-import torch
-import torch.nn as nn
-
-
-logger = getLogger(__name__)
-
-
-def quantize(x, scale, zero, maxq):
-    if maxq < 0:
-        return (x > scale / 2).float() * scale + (x < zero / 2).float() * zero
-    q = torch.clamp(torch.round(x / scale) + zero, 0, maxq)
-    return scale * (q - zero)
-
-
-class Quantizer(nn.Module):
-
-    def __init__(self, shape=1):
-        super(Quantizer, self).__init__()
-        self.register_buffer('maxq', torch.tensor(0))
-        self.register_buffer('scale', torch.zeros(shape))
-        self.register_buffer('zero', torch.zeros(shape))
-
-    def configure(
-        self,
-        bits, perchannel=False, sym=True,
-        mse=False, norm=2.4, grid=100, maxshrink=.8,
-        trits=False
-    ):
-
-        self.maxq = torch.tensor(2 ** bits - 1)
-        self.perchannel = perchannel
-        self.sym = sym
-        self.mse = mse
-        self.norm = norm
-        self.grid = grid
-        self.maxshrink = maxshrink
-        if trits:
-            self.maxq = torch.tensor(-1)
-
-    def find_params(self, x, weight=False):
-        dev = x.device
-        self.maxq = self.maxq.to(dev)
-
-        shape = x.shape
-        if self.perchannel:
-            if weight:
-                x = x.flatten(1)
-            else:
-                if len(shape) == 4:
-                    x = x.permute([1, 0, 2, 3])
-                    x = x.flatten(1)
-                if len(shape) == 3:
-                    x = x.reshape((-1, shape[-1])).t()
-                if len(shape) == 2:
-                    x = x.t()
-        else:
-            x = x.flatten().unsqueeze(0)
-
-        tmp = torch.zeros(x.shape[0], device=dev)
-        xmin = torch.minimum(x.min(1)[0], tmp)
-        xmax = torch.maximum(x.max(1)[0], tmp)
-
-        if self.sym:
-            xmax = torch.maximum(torch.abs(xmin), xmax)
-            tmp = xmin < 0
-            if torch.any(tmp):
-                xmin[tmp] = -xmax[tmp]
-        tmp = (xmin == 0) & (xmax == 0)
-        xmin[tmp] = -1
-        xmax[tmp] = +1
-
-        if self.maxq < 0:
-            self.scale = xmax
-            self.zero = xmin
-        else:
-            self.scale = (xmax - xmin) / self.maxq
-            if self.sym:
-                self.zero = torch.full_like(self.scale, (self.maxq + 1) / 2)
-            else:
-                self.zero = torch.round(-xmin / self.scale)
-
-        if self.mse:
-            best = torch.full([x.shape[0]], float('inf'), device=dev)
-            for i in range(int(self.maxshrink * self.grid)):
-                p = 1 - i / self.grid
-                xmin1 = p * xmin
-                xmax1 = p * xmax
-                scale1 = (xmax1 - xmin1) / self.maxq
-                zero1 = torch.round(-xmin1 / scale1) if not self.sym else self.zero
-                q = quantize(x, scale1.unsqueeze(1), zero1.unsqueeze(1), self.maxq)
-                q -= x
-                q.abs_()
-                q.pow_(self.norm)
-                err = torch.sum(q, 1)
-                tmp = err < best
-                if torch.any(tmp):
-                    best[tmp] = err[tmp]
-                    self.scale[tmp] = scale1[tmp]
-                    self.zero[tmp] = zero1[tmp]
-        if not self.perchannel:
-            if weight:
-                tmp = shape[0]
-            else:
-                tmp = shape[1] if len(shape) != 3 else shape[2]
-            self.scale = self.scale.repeat(tmp)
-            self.zero = self.zero.repeat(tmp)
-
-        if weight:
-            shape = [-1] + [1] * (len(shape) - 1)
-            self.scale = self.scale.reshape(shape)
-            self.zero = self.zero.reshape(shape)
-            return
-        if len(shape) == 4:
-            self.scale = self.scale.reshape((1, -1, 1, 1))
-            self.zero = self.zero.reshape((1, -1, 1, 1))
-        if len(shape) == 3:
-            self.scale = self.scale.reshape((1, 1, -1))
-            self.zero = self.zero.reshape((1, 1, -1))
-        if len(shape) == 2:
-            self.scale = self.scale.unsqueeze(0)
-            self.zero = self.zero.unsqueeze(0)
-
-    def quantize(self, x):
-        if self.ready():
-            return quantize(x, self.scale, self.zero, self.maxq)
-        return x
-
-    def enabled(self):
-        return self.maxq > 0
-
-    def ready(self):
-        return torch.all(self.scale != 0)
-
-
-__all__ = ["Quantizer"]
+from logging import getLogger
+
+import torch
+import torch.nn as nn
+
+
+logger = getLogger(__name__)
+
+
+def quantize(x, scale, zero, maxq):
+    if maxq < 0:
+        return (x > scale / 2).float() * scale + (x < zero / 2).float() * zero
+    q = torch.clamp(torch.round(x / scale) + zero, 0, maxq)
+    return scale * (q - zero)
+
+
+class Quantizer(nn.Module):
+
+    def __init__(self, shape=1):
+        super(Quantizer, self).__init__()
+        self.register_buffer('maxq', torch.tensor(0))
+        self.register_buffer('scale', torch.zeros(shape))
+        self.register_buffer('zero', torch.zeros(shape))
+
+    def configure(
+        self,
+        bits, perchannel=False, sym=True,
+        mse=False, norm=2.4, grid=100, maxshrink=.8,
+        trits=False
+    ):
+
+        self.maxq = torch.tensor(2 ** bits - 1)
+        self.perchannel = perchannel
+        self.sym = sym
+        self.mse = mse
+        self.norm = norm
+        self.grid = grid
+        self.maxshrink = maxshrink
+        if trits:
+            self.maxq = torch.tensor(-1)
+
+    def find_params(self, x, weight=False):
+        dev = x.device
+        self.maxq = self.maxq.to(dev)
+
+        shape = x.shape
+        if self.perchannel:
+            if weight:
+                x = x.flatten(1)
+            else:
+                if len(shape) == 4:
+                    x = x.permute([1, 0, 2, 3])
+                    x = x.flatten(1)
+                if len(shape) == 3:
+                    x = x.reshape((-1, shape[-1])).t()
+                if len(shape) == 2:
+                    x = x.t()
+        else:
+            x = x.flatten().unsqueeze(0)
+
+        tmp = torch.zeros(x.shape[0], device=dev)
+        xmin = torch.minimum(x.min(1)[0], tmp)
+        xmax = torch.maximum(x.max(1)[0], tmp)
+
+        if self.sym:
+            xmax = torch.maximum(torch.abs(xmin), xmax)
+            tmp = xmin < 0
+            if torch.any(tmp):
+                xmin[tmp] = -xmax[tmp]
+        tmp = (xmin == 0) & (xmax == 0)
+        xmin[tmp] = -1
+        xmax[tmp] = +1
+
+        if self.maxq < 0:
+            self.scale = xmax
+            self.zero = xmin
+        else:
+            self.scale = (xmax - xmin) / self.maxq
+            if self.sym:
+                self.zero = torch.full_like(self.scale, (self.maxq + 1) / 2)
+            else:
+                self.zero = torch.round(-xmin / self.scale)
+
+        if self.mse:
+            best = torch.full([x.shape[0]], float('inf'), device=dev)
+            for i in range(int(self.maxshrink * self.grid)):
+                p = 1 - i / self.grid
+                xmin1 = p * xmin
+                xmax1 = p * xmax
+                scale1 = (xmax1 - xmin1) / self.maxq
+                zero1 = torch.round(-xmin1 / scale1) if not self.sym else self.zero
+                q = quantize(x, scale1.unsqueeze(1), zero1.unsqueeze(1), self.maxq)
+                q -= x
+                q.abs_()
+                q.pow_(self.norm)
+                err = torch.sum(q, 1)
+                tmp = err < best
+                if torch.any(tmp):
+                    best[tmp] = err[tmp]
+                    self.scale[tmp] = scale1[tmp]
+                    self.zero[tmp] = zero1[tmp]
+        if not self.perchannel:
+            if weight:
+                tmp = shape[0]
+            else:
+                tmp = shape[1] if len(shape) != 3 else shape[2]
+            self.scale = self.scale.repeat(tmp)
+            self.zero = self.zero.repeat(tmp)
+
+        if weight:
+            shape = [-1] + [1] * (len(shape) - 1)
+            self.scale = self.scale.reshape(shape)
+            self.zero = self.zero.reshape(shape)
+            return
+        if len(shape) == 4:
+            self.scale = self.scale.reshape((1, -1, 1, 1))
+            self.zero = self.zero.reshape((1, -1, 1, 1))
+        if len(shape) == 3:
+            self.scale = self.scale.reshape((1, 1, -1))
+            self.zero = self.zero.reshape((1, 1, -1))
+        if len(shape) == 2:
+            self.scale = self.scale.unsqueeze(0)
+            self.zero = self.zero.unsqueeze(0)
+
+    def quantize(self, x):
+        if self.ready():
+            return quantize(x, self.scale, self.zero, self.maxq)
+        return x
+
+    def enabled(self):
+        return self.maxq > 0
+
+    def ready(self):
+        return torch.all(self.scale != 0)
+
+
+__all__ = ["Quantizer"]
```

### Comparing `auto_gptq-0.3.0/auto_gptq/utils/data_utils.py` & `auto_gptq-0.3.1/auto_gptq/utils/data_utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,267 +1,267 @@
-import copy
-import random
-from functools import partial
-from typing import Callable, Dict, List, Optional
-
-import torch
-from datasets import load_dataset, DatasetDict, IterableDatasetDict
-from torch import LongTensor
-from torch.utils.data import DataLoader
-from transformers import PreTrainedTokenizer
-
-
-def make_data_block(
-    samples: Dict[str, List[str]],
-    prompt_col_name: str,
-    label_col_name: str,
-    tokenizer: PreTrainedTokenizer,
-    preprocess_fn: Optional[Callable] = None,
-    sample_max_len: int = 1024,
-    block_max_len: int = 2048,
-    add_eos_token: bool = False,
-    truncate_prompt: bool = True,
-    merge_prompt_label: bool = False
-) -> Dict[str, List[LongTensor]]:
-    """A simple implementation of text generation oriented smart batching to maximize VRAM usage when evaluation
-
-    :param samples: Dict[str, List[str]], samples that used to make data blocks
-    :param prompt_col_name: str, name of the key in samples whose value stores prompt
-    :param label_col_name: str, name of the key in samples whose value stores label
-    :param tokenizer: transformers.PretrainedTokenizer, tokenizer that used to tokenize samples
-    :param preprocess_fn: Optional[Callable], optional function that used to preprocess samples such as
-        refactor the data structure of samples, note the output of this function must be a dict whose keys
-        at least contains `prompt_col_name` and `label_col_name`
-    :param sample_max_len: int, defaults to 1024, max tokens number of each sample (before padding)
-    :param block_max_len: int, defaults to 2048, max tokens number of each data block (after padding)
-    :param add_eos_token: bool, defaults to False, whether add eos_token or not to the label
-    :param truncate_prompt: bool, defaults to True, whether to truncate prompt if the sample's total tokens
-        number exceeds `sample_max_len`, if not, will truncate label and drop this sample when all tokens
-        in label are truncated
-    :param merge_prompt_label: bool, defaults to False, will merge label into prompt if set to True, usually
-        this only required when doing language modeling task
-    :return: Dict[str, List[torch.LongTensor]], a dict whose keys are `input_ids`, `attention_mask` and
-        `label` and values are a list of torch.LongTensor
-    """
-    if preprocess_fn:
-        samples = preprocess_fn(samples)
-
-    prompts = samples[prompt_col_name]
-    labels = samples[label_col_name]
-
-    # tokenize samples
-    tokenized_prompts = tokenizer(prompts, truncation=False)["input_ids"]
-    tokenized_labels = tokenizer(labels, truncation=False)["input_ids"]
-
-    # filter tokenized samples by length
-    dropped_indices = []
-    for idx, (tokenized_prompt, tokenized_label) in enumerate(zip(tokenized_prompts, tokenized_labels)):
-        if add_eos_token:
-            tokenized_label += [tokenizer.eos_token_id]
-        len_prompt = len(tokenized_prompt)
-        len_label = len(tokenized_label)
-        exceed_len = len_prompt + len_label - sample_max_len
-        if exceed_len > 0:
-            if truncate_prompt:
-                tokenized_prompt = tokenized_prompt[exceed_len:]
-            else:
-                tokenized_label = tokenized_label[: -exceed_len]
-        tokenized_prompts[idx] = tokenized_prompt
-        tokenized_labels[idx] = tokenized_label
-        if not tokenized_label:
-            dropped_indices.append(idx)
-
-    # make data blocks of samples
-    tokenized_samples = sorted(
-        [
-            (p, l) for idx, (p, l) in enumerate(zip(tokenized_prompts, tokenized_labels))
-            if idx not in dropped_indices
-        ],
-        key=lambda x: (len(x[0]) + len(x[1])) if merge_prompt_label else len(x[0])
-    )
-    sample_blocks = []
-    sample_block = []
-    blk_max_len = 0
-    blk_total_len = 0
-    for tokenized_sample in tokenized_samples:
-        prompt_ids, label_ids = tokenized_sample
-        ori_sample_len = len(prompt_ids)
-        if merge_prompt_label:
-            ori_sample_len += len(label_ids)
-        if ori_sample_len <= blk_max_len:
-            additional_len = blk_max_len
-            sample_len = blk_max_len
-        else:
-            additional_len = len(sample_block) * (ori_sample_len - blk_max_len) + ori_sample_len
-            sample_len = ori_sample_len
-
-        if blk_total_len + additional_len > block_max_len:
-            sample_blocks.append((copy.copy(sample_block), blk_max_len))
-            sample_block = []
-            blk_max_len = 0
-            blk_total_len = 0
-            sample_len = ori_sample_len
-            additional_len = ori_sample_len
-
-        sample_block.append(tokenized_sample)
-        blk_max_len = max(blk_max_len, sample_len)
-        blk_total_len += additional_len
-
-    if sample_block:
-        sample_blocks.append((copy.copy(sample_block), blk_max_len))
-    del sample_block
-    del blk_max_len
-    del blk_total_len
-
-    new_samples = {
-        "input_ids": [],
-        "attention_mask": [],
-        "labels": []
-    }
-    # padding each data block internally
-    for block, blk_max_len in sample_blocks:
-        input_ids = []
-        attention_mask = []
-        label_ids = []
-        label_max_len = max([len(sample[1]) for sample in block])
-
-        for sample in block:
-            tokenized_prompt, tokenized_label = sample
-            sample_len = len(tokenized_prompt)
-            if merge_prompt_label:
-                sample_len += len(tokenized_label)
-            pad_num = blk_max_len - sample_len
-            if merge_prompt_label:
-                input_ids.append([tokenizer.pad_token_id] * pad_num + tokenized_prompt + tokenized_label)
-                label_ids.append([-100] * (pad_num + len(tokenized_prompt)) + tokenized_label)
-            else:
-                input_ids.append([tokenizer.pad_token_id] * pad_num + tokenized_prompt)
-                label_ids.append([-100] * (label_max_len - len(tokenized_label)) + tokenized_label)
-            attention_mask.append([0] * pad_num + [1] * sample_len)
-
-        new_samples["input_ids"].append(input_ids)
-        new_samples["attention_mask"].append(attention_mask)
-        new_samples["labels"].append(label_ids)
-
-    return new_samples
-
-
-def collate_data(blocks: List[Dict[str, List[List[int]]]], pad_token_id: int) -> Dict[str, LongTensor]:
-    def pad_block(block, pads):
-        return torch.cat((pads.to(block.device), block), dim=-1)
-
-    input_ids_blocks = [LongTensor(block["input_ids"]) for block in blocks]
-    attention_mask_blocks = [LongTensor(block["attention_mask"]) for block in blocks]
-    label_blocks = [LongTensor(block["labels"]) for block in blocks]
-
-    bsz = len(blocks)
-    inp_max_len = max([block.size(-1) for block in input_ids_blocks])
-    label_max_len = max([block.size(-1) for block in label_blocks])
-
-    for i in range(bsz):
-        block_bsz, block_inp_len = input_ids_blocks[i].shape
-        block_label_len = label_blocks[i].shape[-1]
-        pad_num = inp_max_len - block_inp_len
-        if pad_num > 0:
-            input_ids_blocks[i] = pad_block(input_ids_blocks[i], torch.ones((block_bsz, pad_num)) * pad_token_id)
-            attention_mask_blocks[i] = pad_block(attention_mask_blocks[i], torch.zeros((block_bsz, pad_num)))
-        label_pad_num = label_max_len - block_label_len
-        if label_pad_num > 0:
-            label_blocks[i] = pad_block(label_blocks[i], torch.ones((block_bsz, label_pad_num)) * -100)
-
-    return {
-        "input_ids": torch.cat(input_ids_blocks, dim=0).long(),
-        "attention_mask": torch.cat(attention_mask_blocks, dim=0).long(),
-        "labels": torch.cat(label_blocks, dim=0).long()
-    }
-
-
-def get_dataloader(
-    data_path_or_name: str,
-    prompt_col_name: str,
-    label_col_name: str,
-    tokenizer: PreTrainedTokenizer,
-    load_fn: Optional[Callable] = None,
-    preprocess_fn: Optional[Callable] = None,
-    num_samples: int = 128,
-    sample_max_len: int = 1024,
-    block_max_len: int = 2048,
-    add_eos_token: bool = False,
-    truncate_prompt: bool = True,
-    merge_prompt_label: bool = False,
-    load_fn_kwargs: Optional[dict] = None,
-    preprocess_fn_kwargs: Optional[dict] = None,
-    **kwargs
-) -> DataLoader:
-    """load dataset and build dataloader
-
-    :param data_path_or_name: str, dataset name in hf-hub or local file path
-    :param prompt_col_name: str, see `make_data_block`
-    :param label_col_name: str, see `make_data_block`
-    :param tokenizer: str, see `make_data_block`
-    :param load_fn: Optional[Callable], defaults to None, function used to load dataset, if not specified,
-        use `datasets.load_dataset`
-    :param preprocess_fn: Optional[Callable], see `make_data_block`
-    :param num_samples: int, defaults to 128, total samples used to evaluation
-    :param sample_max_len: int, see `make_data_block`
-    :param block_max_len: int, see `make_data_block`
-    :param add_eos_token: bool, see `make_data_block`
-    :param truncate_prompt: bool, see `make_data_block`
-    :param merge_prompt_label: bool, see `make_data_block`
-    :param load_fn_kwargs: Optional[dict], defaults to None, keyword arguments used
-        for `load_fn` or `datasets.load_dataset`
-    :param preprocess_fn_kwargs: Optional[dict], defaults to None, keyword arguments used
-        for `preprocess_fn`
-    :param kwargs: additional keyword arguments will be passed to torch's `DataLoader` initialization,
-        note values of `batch_size`, `shuffle` and `collate_fn` will always be overridden to fixed value
-    :return: torch.utils.data.DataLoader
-    """
-
-    if not load_fn_kwargs:
-        load_fn_kwargs = dict()
-    if not preprocess_fn_kwargs:
-        preprocess_fn_kwargs = dict()
-
-    if load_fn:
-        ds = load_fn(data_path_or_name, **load_fn_kwargs)
-    else:
-        ds = load_dataset(data_path_or_name, **load_fn_kwargs)
-    if isinstance(ds, (DatasetDict, IterableDatasetDict)):
-        if "evaluation" in ds:
-            ds = ds["evaluation"]
-        elif "test" in ds:
-            ds = ds["test"]
-        else:
-            ds = ds["train"]
-
-    ds = ds.select(indices=random.sample(range(len(ds)), min(len(ds), num_samples)), keep_in_memory=True)
-    ds = ds.map(
-        make_data_block,
-        batched=True,
-        batch_size=len(ds),
-        num_proc=1,
-        remove_columns=ds.column_names,
-        keep_in_memory=True,
-        load_from_cache_file=False,
-        fn_kwargs={
-            "prompt_col_name": prompt_col_name,
-            "label_col_name": label_col_name,
-            "tokenizer": tokenizer,
-            "preprocess_fn": partial(preprocess_fn, **preprocess_fn_kwargs),
-            "sample_max_len": sample_max_len,
-            "block_max_len": block_max_len,
-            "add_eos_token": add_eos_token,
-            "truncate_prompt": truncate_prompt,
-            "merge_prompt_label": merge_prompt_label
-        }
-    )
-
-    # override some arguments' values in kwargs despite user specified
-    kwargs["batch_size"] = 1
-    kwargs["shuffle"] = False
-    kwargs["collate_fn"] = partial(collate_data, pad_token_id=tokenizer.pad_token_id)
-    dl = DataLoader(ds, **kwargs)
-
-    return dl
-
-
-__all__ = ["make_data_block", "collate_data", "get_dataloader"]
+import copy
+import random
+from functools import partial
+from typing import Callable, Dict, List, Optional
+
+import torch
+from datasets import load_dataset, DatasetDict, IterableDatasetDict
+from torch import LongTensor
+from torch.utils.data import DataLoader
+from transformers import PreTrainedTokenizer
+
+
+def make_data_block(
+    samples: Dict[str, List[str]],
+    prompt_col_name: str,
+    label_col_name: str,
+    tokenizer: PreTrainedTokenizer,
+    preprocess_fn: Optional[Callable] = None,
+    sample_max_len: int = 1024,
+    block_max_len: int = 2048,
+    add_eos_token: bool = False,
+    truncate_prompt: bool = True,
+    merge_prompt_label: bool = False
+) -> Dict[str, List[LongTensor]]:
+    """A simple implementation of text generation oriented smart batching to maximize VRAM usage when evaluation
+
+    :param samples: Dict[str, List[str]], samples that used to make data blocks
+    :param prompt_col_name: str, name of the key in samples whose value stores prompt
+    :param label_col_name: str, name of the key in samples whose value stores label
+    :param tokenizer: transformers.PretrainedTokenizer, tokenizer that used to tokenize samples
+    :param preprocess_fn: Optional[Callable], optional function that used to preprocess samples such as
+        refactor the data structure of samples, note the output of this function must be a dict whose keys
+        at least contains `prompt_col_name` and `label_col_name`
+    :param sample_max_len: int, defaults to 1024, max tokens number of each sample (before padding)
+    :param block_max_len: int, defaults to 2048, max tokens number of each data block (after padding)
+    :param add_eos_token: bool, defaults to False, whether add eos_token or not to the label
+    :param truncate_prompt: bool, defaults to True, whether to truncate prompt if the sample's total tokens
+        number exceeds `sample_max_len`, if not, will truncate label and drop this sample when all tokens
+        in label are truncated
+    :param merge_prompt_label: bool, defaults to False, will merge label into prompt if set to True, usually
+        this only required when doing language modeling task
+    :return: Dict[str, List[torch.LongTensor]], a dict whose keys are `input_ids`, `attention_mask` and
+        `label` and values are a list of torch.LongTensor
+    """
+    if preprocess_fn:
+        samples = preprocess_fn(samples)
+
+    prompts = samples[prompt_col_name]
+    labels = samples[label_col_name]
+
+    # tokenize samples
+    tokenized_prompts = tokenizer(prompts, truncation=False)["input_ids"]
+    tokenized_labels = tokenizer(labels, truncation=False)["input_ids"]
+
+    # filter tokenized samples by length
+    dropped_indices = []
+    for idx, (tokenized_prompt, tokenized_label) in enumerate(zip(tokenized_prompts, tokenized_labels)):
+        if add_eos_token:
+            tokenized_label += [tokenizer.eos_token_id]
+        len_prompt = len(tokenized_prompt)
+        len_label = len(tokenized_label)
+        exceed_len = len_prompt + len_label - sample_max_len
+        if exceed_len > 0:
+            if truncate_prompt:
+                tokenized_prompt = tokenized_prompt[exceed_len:]
+            else:
+                tokenized_label = tokenized_label[: -exceed_len]
+        tokenized_prompts[idx] = tokenized_prompt
+        tokenized_labels[idx] = tokenized_label
+        if not tokenized_label:
+            dropped_indices.append(idx)
+
+    # make data blocks of samples
+    tokenized_samples = sorted(
+        [
+            (p, l) for idx, (p, l) in enumerate(zip(tokenized_prompts, tokenized_labels))
+            if idx not in dropped_indices
+        ],
+        key=lambda x: (len(x[0]) + len(x[1])) if merge_prompt_label else len(x[0])
+    )
+    sample_blocks = []
+    sample_block = []
+    blk_max_len = 0
+    blk_total_len = 0
+    for tokenized_sample in tokenized_samples:
+        prompt_ids, label_ids = tokenized_sample
+        ori_sample_len = len(prompt_ids)
+        if merge_prompt_label:
+            ori_sample_len += len(label_ids)
+        if ori_sample_len <= blk_max_len:
+            additional_len = blk_max_len
+            sample_len = blk_max_len
+        else:
+            additional_len = len(sample_block) * (ori_sample_len - blk_max_len) + ori_sample_len
+            sample_len = ori_sample_len
+
+        if blk_total_len + additional_len > block_max_len:
+            sample_blocks.append((copy.copy(sample_block), blk_max_len))
+            sample_block = []
+            blk_max_len = 0
+            blk_total_len = 0
+            sample_len = ori_sample_len
+            additional_len = ori_sample_len
+
+        sample_block.append(tokenized_sample)
+        blk_max_len = max(blk_max_len, sample_len)
+        blk_total_len += additional_len
+
+    if sample_block:
+        sample_blocks.append((copy.copy(sample_block), blk_max_len))
+    del sample_block
+    del blk_max_len
+    del blk_total_len
+
+    new_samples = {
+        "input_ids": [],
+        "attention_mask": [],
+        "labels": []
+    }
+    # padding each data block internally
+    for block, blk_max_len in sample_blocks:
+        input_ids = []
+        attention_mask = []
+        label_ids = []
+        label_max_len = max([len(sample[1]) for sample in block])
+
+        for sample in block:
+            tokenized_prompt, tokenized_label = sample
+            sample_len = len(tokenized_prompt)
+            if merge_prompt_label:
+                sample_len += len(tokenized_label)
+            pad_num = blk_max_len - sample_len
+            if merge_prompt_label:
+                input_ids.append([tokenizer.pad_token_id] * pad_num + tokenized_prompt + tokenized_label)
+                label_ids.append([-100] * (pad_num + len(tokenized_prompt)) + tokenized_label)
+            else:
+                input_ids.append([tokenizer.pad_token_id] * pad_num + tokenized_prompt)
+                label_ids.append([-100] * (label_max_len - len(tokenized_label)) + tokenized_label)
+            attention_mask.append([0] * pad_num + [1] * sample_len)
+
+        new_samples["input_ids"].append(input_ids)
+        new_samples["attention_mask"].append(attention_mask)
+        new_samples["labels"].append(label_ids)
+
+    return new_samples
+
+
+def collate_data(blocks: List[Dict[str, List[List[int]]]], pad_token_id: int) -> Dict[str, LongTensor]:
+    def pad_block(block, pads):
+        return torch.cat((pads.to(block.device), block), dim=-1)
+
+    input_ids_blocks = [LongTensor(block["input_ids"]) for block in blocks]
+    attention_mask_blocks = [LongTensor(block["attention_mask"]) for block in blocks]
+    label_blocks = [LongTensor(block["labels"]) for block in blocks]
+
+    bsz = len(blocks)
+    inp_max_len = max([block.size(-1) for block in input_ids_blocks])
+    label_max_len = max([block.size(-1) for block in label_blocks])
+
+    for i in range(bsz):
+        block_bsz, block_inp_len = input_ids_blocks[i].shape
+        block_label_len = label_blocks[i].shape[-1]
+        pad_num = inp_max_len - block_inp_len
+        if pad_num > 0:
+            input_ids_blocks[i] = pad_block(input_ids_blocks[i], torch.ones((block_bsz, pad_num)) * pad_token_id)
+            attention_mask_blocks[i] = pad_block(attention_mask_blocks[i], torch.zeros((block_bsz, pad_num)))
+        label_pad_num = label_max_len - block_label_len
+        if label_pad_num > 0:
+            label_blocks[i] = pad_block(label_blocks[i], torch.ones((block_bsz, label_pad_num)) * -100)
+
+    return {
+        "input_ids": torch.cat(input_ids_blocks, dim=0).long(),
+        "attention_mask": torch.cat(attention_mask_blocks, dim=0).long(),
+        "labels": torch.cat(label_blocks, dim=0).long()
+    }
+
+
+def get_dataloader(
+    data_path_or_name: str,
+    prompt_col_name: str,
+    label_col_name: str,
+    tokenizer: PreTrainedTokenizer,
+    load_fn: Optional[Callable] = None,
+    preprocess_fn: Optional[Callable] = None,
+    num_samples: int = 128,
+    sample_max_len: int = 1024,
+    block_max_len: int = 2048,
+    add_eos_token: bool = False,
+    truncate_prompt: bool = True,
+    merge_prompt_label: bool = False,
+    load_fn_kwargs: Optional[dict] = None,
+    preprocess_fn_kwargs: Optional[dict] = None,
+    **kwargs
+) -> DataLoader:
+    """load dataset and build dataloader
+
+    :param data_path_or_name: str, dataset name in hf-hub or local file path
+    :param prompt_col_name: str, see `make_data_block`
+    :param label_col_name: str, see `make_data_block`
+    :param tokenizer: str, see `make_data_block`
+    :param load_fn: Optional[Callable], defaults to None, function used to load dataset, if not specified,
+        use `datasets.load_dataset`
+    :param preprocess_fn: Optional[Callable], see `make_data_block`
+    :param num_samples: int, defaults to 128, total samples used to evaluation
+    :param sample_max_len: int, see `make_data_block`
+    :param block_max_len: int, see `make_data_block`
+    :param add_eos_token: bool, see `make_data_block`
+    :param truncate_prompt: bool, see `make_data_block`
+    :param merge_prompt_label: bool, see `make_data_block`
+    :param load_fn_kwargs: Optional[dict], defaults to None, keyword arguments used
+        for `load_fn` or `datasets.load_dataset`
+    :param preprocess_fn_kwargs: Optional[dict], defaults to None, keyword arguments used
+        for `preprocess_fn`
+    :param kwargs: additional keyword arguments will be passed to torch's `DataLoader` initialization,
+        note values of `batch_size`, `shuffle` and `collate_fn` will always be overridden to fixed value
+    :return: torch.utils.data.DataLoader
+    """
+
+    if not load_fn_kwargs:
+        load_fn_kwargs = dict()
+    if not preprocess_fn_kwargs:
+        preprocess_fn_kwargs = dict()
+
+    if load_fn:
+        ds = load_fn(data_path_or_name, **load_fn_kwargs)
+    else:
+        ds = load_dataset(data_path_or_name, **load_fn_kwargs)
+    if isinstance(ds, (DatasetDict, IterableDatasetDict)):
+        if "evaluation" in ds:
+            ds = ds["evaluation"]
+        elif "test" in ds:
+            ds = ds["test"]
+        else:
+            ds = ds["train"]
+
+    ds = ds.select(indices=random.sample(range(len(ds)), min(len(ds), num_samples)), keep_in_memory=True)
+    ds = ds.map(
+        make_data_block,
+        batched=True,
+        batch_size=len(ds),
+        num_proc=1,
+        remove_columns=ds.column_names,
+        keep_in_memory=True,
+        load_from_cache_file=False,
+        fn_kwargs={
+            "prompt_col_name": prompt_col_name,
+            "label_col_name": label_col_name,
+            "tokenizer": tokenizer,
+            "preprocess_fn": partial(preprocess_fn, **preprocess_fn_kwargs),
+            "sample_max_len": sample_max_len,
+            "block_max_len": block_max_len,
+            "add_eos_token": add_eos_token,
+            "truncate_prompt": truncate_prompt,
+            "merge_prompt_label": merge_prompt_label
+        }
+    )
+
+    # override some arguments' values in kwargs despite user specified
+    kwargs["batch_size"] = 1
+    kwargs["shuffle"] = False
+    kwargs["collate_fn"] = partial(collate_data, pad_token_id=tokenizer.pad_token_id)
+    dl = DataLoader(ds, **kwargs)
+
+    return dl
+
+
+__all__ = ["make_data_block", "collate_data", "get_dataloader"]
```

### Comparing `auto_gptq-0.3.0/auto_gptq/utils/import_utils.py` & `auto_gptq-0.3.1/auto_gptq/utils/import_utils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from packaging.version import parse as parse_version
-
-try:
-    import triton
-
-    TRITON_AVAILABLE = True
-except ImportError:
-    TRITON_AVAILABLE = False
-
-try:
-    import autogptq_cuda
-
-    AUTOGPTQ_CUDA_AVAILABLE = True
-except:
-    AUTOGPTQ_CUDA_AVAILABLE = False
-
-
-def dynamically_import_QuantLinear(use_triton: bool, desc_act: bool, group_size: int):
-    if use_triton:
-        from ..nn_modules.qlinear.qlinear_triton import QuantLinear
-    else:
-        if not desc_act or group_size == -1:
-            from ..nn_modules.qlinear.qlinear_cuda_old import QuantLinear
-        else:
-            from ..nn_modules.qlinear.qlinear_cuda import QuantLinear
-
-    return QuantLinear
-
-
-def compare_transformers_version(
-    version: str = "v4.28.0",
-    op: str = "eq"
-):
-    assert op in ["eq", "lt", "le", "gt", "ge"]
-
-    from transformers import __version__
-
-    return getattr(parse_version(__version__), f"__{op}__")(parse_version(version))
-
-
-def compare_pytorch_version(
-    version: str = "v2.0.0",
-    op: str = "eq"
-):
-    assert op in ["eq", "lt", "le", "gt", "ge"]
-
-    from torch import __version__
-
-    return getattr(parse_version(__version__), f"__{op}__")(parse_version(version))
+from packaging.version import parse as parse_version
+
+try:
+    import triton
+
+    TRITON_AVAILABLE = True
+except ImportError:
+    TRITON_AVAILABLE = False
+
+try:
+    import autogptq_cuda
+
+    AUTOGPTQ_CUDA_AVAILABLE = True
+except:
+    AUTOGPTQ_CUDA_AVAILABLE = False
+
+
+def dynamically_import_QuantLinear(use_triton: bool, desc_act: bool, group_size: int):
+    if use_triton:
+        from ..nn_modules.qlinear.qlinear_triton import QuantLinear
+    else:
+        if not desc_act or group_size == -1:
+            from ..nn_modules.qlinear.qlinear_cuda_old import QuantLinear
+        else:
+            from ..nn_modules.qlinear.qlinear_cuda import QuantLinear
+
+    return QuantLinear
+
+
+def compare_transformers_version(
+    version: str = "v4.28.0",
+    op: str = "eq"
+):
+    assert op in ["eq", "lt", "le", "gt", "ge"]
+
+    from transformers import __version__
+
+    return getattr(parse_version(__version__), f"__{op}__")(parse_version(version))
+
+
+def compare_pytorch_version(
+    version: str = "v2.0.0",
+    op: str = "eq"
+):
+    assert op in ["eq", "lt", "le", "gt", "ge"]
+
+    from torch import __version__
+
+    return getattr(parse_version(__version__), f"__{op}__")(parse_version(version))
```

### Comparing `auto_gptq-0.3.0/auto_gptq.egg-info/PKG-INFO` & `auto_gptq-0.3.1/auto_gptq.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,345 +1,346 @@
-Metadata-Version: 2.1
-Name: auto-gptq
-Version: 0.3.0
-Summary: An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
-Home-page: https://github.com/PanQiWei/AutoGPTQ
-Author: PanQiWei
-Keywords: gptq,quantization,large-language-models,pytorch,transformers
-Platform: windows
-Platform: linux
-Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
-Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: C++
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Provides-Extra: triton
-License-File: LICENSE
-
-<h1 align="center">AutoGPTQ</h1>
-<p align="center">An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.</p>
-<p align="center">
-    <a href="https://github.com/PanQiWei/AutoGPTQ/releases">
-        <img alt="GitHub release" src="https://img.shields.io/github/release/PanQiWei/AutoGPTQ.svg">
-    </a>
-    <a href="https://pypi.org/project/auto-gptq/">
-        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/auto-gptq">
-    </a>
-</p>
-<h4 align="center">
-    <p>
-        <b>English</b> |
-        <a href="https://github.com/PanQiWei/AutoGPTQ/blob/main/README_zh.md">中文</a>
-    </p>
-</h4>
-
-*<center>📣 Long time no see! 👋 Architecture upgrade, performance optimization and more new features will come in July and August, stay tune! 🥂</center>*
-
-## News or Update
-
-- 2023-06-05 - (Update) - Integrate with 🤗 peft to use gptq quantized model to train adapters, support LoRA, AdaLoRA, AdaptionPrompt, etc.
-- 2023-05-30 - (Update) - Support download/upload quantized model from/to 🤗 Hub.
-- 2023-05-27 - (Update) - Support quantization and inference for `gpt_bigcode`, `codegen` and `RefineWeb/RefineWebModel`(falcon) model types.
-- 2023-05-04 - (Update) - Support using faster cuda kernel when `not desc_act or group_size == -1`.
-
-*For more histories please turn to [here](docs/NEWS_OR_UPDATE.md)*
-
-## Performance Comparison
-
-### Inference Speed
-> The result is generated using [this script](examples/benchmark/generation_speed.py), batch size of input is 1, decode strategy is beam search and enforce the model to generate 512 tokens, speed metric is tokens/s (the larger, the better).
-> 
-> The quantized model is loaded using the setup that can gain the fastest inference speed.
-
-| model         | GPU           | num_beams | fp16  | gptq-int4 |
-|---------------|---------------|-----------|-------|-----------|
-| llama-7b      | 1xA100-40G    | 1         | 18.87 | 25.53     |
-| llama-7b      | 1xA100-40G    | 4         | 68.79 | 91.30     |
-| moss-moon 16b | 1xA100-40G    | 1         | 12.48 | 15.25     |
-| moss-moon 16b | 1xA100-40G    | 4         | OOM   | 42.67     |
-| moss-moon 16b | 2xA100-40G    | 1         | 06.83 | 06.78     |
-| moss-moon 16b | 2xA100-40G    | 4         | 13.10 | 10.80     |
-| gpt-j 6b      | 1xRTX3060-12G | 1         | OOM   | 29.55     |
-| gpt-j 6b      | 1xRTX3060-12G | 4         | OOM   | 47.36     |
-
-
-### Perplexity
-For perplexity comparison, you can turn to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes)
-
-## Installation
-
-### Quick Installation
-You can install the latest stable release of AutoGPTQ from pip:
-```shell
-pip install auto-gptq
-```
-Start from v0.2.0, you can download pre-build wheel that satisfied your environment setup from each version's release assets and install it to skip building stage for the fastest installation speed. For example:
-```shell
-# firstly, cd the directory where the wheel saved, then execute command below
-pip install auto_gptq-0.2.0+cu118-cp310-cp310-linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for linux in an environment whose python=3.10 and cuda=11.8
-```
-#### disable cuda extensions
-By default, cuda extensions will be installed when `torch` and `cuda` is already installed in your machine, if you don't want to use them, using:
-```shell
-BUILD_CUDA_EXT=0 pip install auto-gptq
-```
-And to make sure `autogptq_cuda` is not ever in your virtual environment, run:
-```shell
-pip uninstall autogptq_cuda -y
-```
-
-#### to support triton speedup
-To integrate with `triton`, using:
-> warning: currently triton only supports linux; 3-bit quantization is not supported when using triton
-
-```shell
-pip install auto-gptq[triton]
-```
-
-### Install from source
-<details>
-<summary>click to see details</summary>
-
-Clone the source code:
-```shell
-git clone https://github.com/PanQiWei/AutoGPTQ.git && cd AutoGPTQ
-```
-Then, install from source:
-```shell
-pip install .
-```
-Like quick installation, you can also set `BUILD_CUDA_EXT=0` to disable pytorch extension building.
-
-Use `.[triton]` if you want to integrate with triton and it's available on your operating system.
-
-</details>
-
-## Quick Tour
-
-### Quantization and Inference
-> warning: this is just a showcase of the usage of basic apis in AutoGPTQ, which uses only one sample to quantize a much small model, quality of quantized model using such little samples may not good.
-
-Below is an example for the simplest use of `auto_gptq` to quantize a model and inference after quantization: 
-```python
-from transformers import AutoTokenizer, TextGenerationPipeline
-from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
-import logging
-
-logging.basicConfig(
-    format="%(asctime)s %(levelname)s [%(name)s] %(message)s", level=logging.INFO, datefmt="%Y-%m-%d %H:%M:%S"
-)
-
-pretrained_model_dir = "facebook/opt-125m"
-quantized_model_dir = "opt-125m-4bit"
-
-tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir, use_fast=True)
-examples = [
-    tokenizer(
-        "auto-gptq is an easy-to-use model quantization library with user-friendly apis, based on GPTQ algorithm."
-    )
-]
-
-quantize_config = BaseQuantizeConfig(
-    bits=4,  # quantize model to 4-bit
-    group_size=128,  # it is recommended to set the value to 128
-    desc_act=False,  # set to False can significantly speed up inference but the perplexity may slightly bad 
-)
-
-# load un-quantized model, by default, the model will always be loaded into CPU memory
-model = AutoGPTQForCausalLM.from_pretrained(pretrained_model_dir, quantize_config)
-
-# quantize model, the examples should be list of dict whose keys can only be "input_ids" and "attention_mask"
-model.quantize(examples)
-
-# save quantized model
-model.save_quantized(quantized_model_dir)
-
-# save quantized model using safetensors
-model.save_quantized(quantized_model_dir, use_safetensors=True)
-
-# push quantized model to Hugging Face Hub. 
-# to use use_auth_token=True, Login first via huggingface-cli login.
-# or pass explcit token with: use_auth_token="hf_xxxxxxx"
-# (uncomment the following three lines to enable this feature)
-# repo_id = f"YourUserName/{quantized_model_dir}"
-# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
-# model.push_to_hub(repo_id, commit_message=commit_message, use_auth_token=True)
-
-# alternatively you can save and push at the same time
-# (uncomment the following three lines to enable this feature)
-# repo_id = f"YourUserName/{quantized_model_dir}"
-# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
-# model.push_to_hub(repo_id, save_dir=quantized_model_dir, use_safetensors=True, commit_message=commit_message, use_auth_token=True)
-
-# load quantized model to the first GPU
-model = AutoGPTQForCausalLM.from_quantized(quantized_model_dir, device="cuda:0")
-
-# download quantized model from Hugging Face Hub and load to the first GPU
-# model = AutoGPTQForCausalLM.from_quantized(repo_id, device="cuda:0", use_safetensors=True, use_triton=False)
-
-# inference with model.generate
-print(tokenizer.decode(model.generate(**tokenizer("auto_gptq is", return_tensors="pt").to(model.device))[0]))
-
-# or you can also use pipeline
-pipeline = TextGenerationPipeline(model=model, tokenizer=tokenizer)
-print(pipeline("auto-gptq is")[0]["generated_text"])
-```
-
-For more advanced features of model quantization, please reference to [this script](examples/quantization/quant_with_alpaca.py)
-
-### Customize Model
-<details>
-
-<summary>Below is an example to extend `auto_gptq` to support `OPT` model, as you will see, it's very easy:</summary>
-
-```python
-from auto_gptq.modeling import BaseGPTQForCausalLM
-
-
-class OPTGPTQForCausalLM(BaseGPTQForCausalLM):
-    # chained attribute name of transformer layer block
-    layers_block_name = "model.decoder.layers"
-    # chained attribute names of other nn modules that in the same level as the transformer layer block
-    outside_layer_modules = [
-        "model.decoder.embed_tokens", "model.decoder.embed_positions", "model.decoder.project_out",
-        "model.decoder.project_in", "model.decoder.final_layer_norm"
-    ]
-    # chained attribute names of linear layers in transformer layer module
-    # normally, there are four sub lists, for each one the modules in it can be seen as one operation, 
-    # and the order should be the order when they are truly executed, in this case (and usually in most cases), 
-    # they are: attention q_k_v projection, attention output projection, MLP project input, MLP project output
-    inside_layer_modules = [
-        ["self_attn.k_proj", "self_attn.v_proj", "self_attn.q_proj"],
-        ["self_attn.out_proj"],
-        ["fc1"],
-        ["fc2"]
-    ]
-```
-After this, you can use `OPTGPTQForCausalLM.from_pretrained` and other methods as shown in Basic.
-
-</details>
-
-### Evaluation on Downstream Tasks
-You can use tasks defined in `auto_gptq.eval_tasks` to evaluate model's performance on specific down-stream task before and after quantization.
-
-The predefined tasks support all causal-language-models implemented in [🤗 transformers](https://github.com/huggingface/transformers) and in this project.
-
-<details>
-
-<summary>Below is an example to evaluate `EleutherAI/gpt-j-6b` on sequence-classification task using `cardiffnlp/tweet_sentiment_multilingual` dataset:</summary>
-
-```python
-from functools import partial
-
-import datasets
-from transformers import AutoTokenizer, AutoModelForCausalLM, GenerationConfig
-
-from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
-from auto_gptq.eval_tasks import SequenceClassificationTask
-
-
-MODEL = "EleutherAI/gpt-j-6b"
-DATASET = "cardiffnlp/tweet_sentiment_multilingual"
-TEMPLATE = "Question:What's the sentiment of the given text? Choices are {labels}.\nText: {text}\nAnswer:"
-ID2LABEL = {
-    0: "negative",
-    1: "neutral",
-    2: "positive"
-}
-LABELS = list(ID2LABEL.values())
-
-
-def ds_refactor_fn(samples):
-    text_data = samples["text"]
-    label_data = samples["label"]
-
-    new_samples = {"prompt": [], "label": []}
-    for text, label in zip(text_data, label_data):
-        prompt = TEMPLATE.format(labels=LABELS, text=text)
-        new_samples["prompt"].append(prompt)
-        new_samples["label"].append(ID2LABEL[label])
-
-    return new_samples
-
-
-#  model = AutoModelForCausalLM.from_pretrained(MODEL).eval().half().to("cuda:0")
-model = AutoGPTQForCausalLM.from_pretrained(MODEL, BaseQuantizeConfig())
-tokenizer = AutoTokenizer.from_pretrained(MODEL)
-
-task = SequenceClassificationTask(
-        model=model,
-        tokenizer=tokenizer,
-        classes=LABELS,
-        data_name_or_path=DATASET,
-        prompt_col_name="prompt",
-        label_col_name="label",
-        **{
-            "num_samples": 1000,  # how many samples will be sampled to evaluation
-            "sample_max_len": 1024,  # max tokens for each sample
-            "block_max_len": 2048,  # max tokens for each data block
-            # function to load dataset, one must only accept data_name_or_path as input 
-            # and return datasets.Dataset
-            "load_fn": partial(datasets.load_dataset, name="english"),  
-            # function to preprocess dataset, which is used for datasets.Dataset.map, 
-            # must return Dict[str, list] with only two keys: [prompt_col_name, label_col_name]
-            "preprocess_fn": ds_refactor_fn,  
-            # truncate label when sample's length exceed sample_max_len
-            "truncate_prompt": False  
-        }
-    )
-
-# note that max_new_tokens will be automatically specified internally based on given classes
-print(task.run())
-
-# self-consistency
-print(
-    task.run(
-        generation_config=GenerationConfig(
-            num_beams=3,
-            num_return_sequences=3,
-            do_sample=True
-        )
-    )
-)
-```
-
-</details>
-
-## Learn More
-[tutorials](docs/tutorial) provide step-by-step guidance to integrate `auto_gptq` with your own project and some best practice principles.
-
-[examples](examples/README.md) provide plenty of example scripts to use `auto_gptq` in different ways.
-
-## Supported Models
-
-> you can use `model.config.model_type` to compare with the table below to check whether the model you use is supported by `auto_gptq`.
-> 
-> for example, model_type of `WizardLM`, `vicuna` and `gpt4all` are all `llama`, hence they are all supported by `auto_gptq`.
-
-| model type                         | quantization | inference | peft-lora | peft-ada-lora | peft-adaption_prompt                                                                            |
-|------------------------------------|--------------|-----------|-----------|---------------|-------------------------------------------------------------------------------------------------|
-| bloom                              | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
-| gpt2                               | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
-| gpt_neox                           | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
-| gptj                               | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
-| llama                              | ✅            | ✅         | ✅         | ✅             | ✅                                                                                               |
-| moss                               | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
-| opt                                | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
-| gpt_bigcode                        | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
-| codegen                            | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
-| falcon(RefinedWebModel/RefinedWeb) | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
-
-## Supported Evaluation Tasks
-Currently, `auto_gptq` supports: `LanguageModelingTask`, `SequenceClassificationTask` and `TextSummarizationTask`; more Tasks will come soon!
-
-## Acknowledgement
-- Specially thanks **Elias Frantar**, **Saleh Ashkboos**, **Torsten Hoefler** and **Dan Alistarh** for proposing **GPTQ** algorithm and open source the [code](https://github.com/IST-DASLab/gptq).
-- Specially thanks **qwopqwop200**, for code in this project that relevant to quantization are mainly referenced from [GPTQ-for-LLaMa](https://github.com/qwopqwop200/GPTQ-for-LLaMa/tree/cuda).
-
-
-[![Star History Chart](https://api.star-history.com/svg?repos=PanQiwei/AutoGPTQ&type=Date)](https://star-history.com/#PanQiWei/AutoGPTQ&Date)
+Metadata-Version: 2.1
+Name: auto-gptq
+Version: 0.3.1
+Summary: An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
+Home-page: https://github.com/PanQiWei/AutoGPTQ
+Author: PanQiWei
+Keywords: gptq,quantization,large-language-models,pytorch,transformers
+Platform: windows
+Platform: linux
+Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
+Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: C++
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+Provides-Extra: triton
+License-File: LICENSE
+
+<h1 align="center">AutoGPTQ</h1>
+<p align="center">An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.</p>
+<p align="center">
+    <a href="https://github.com/PanQiWei/AutoGPTQ/releases">
+        <img alt="GitHub release" src="https://img.shields.io/github/release/PanQiWei/AutoGPTQ.svg">
+    </a>
+    <a href="https://pypi.org/project/auto-gptq/">
+        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/auto-gptq">
+    </a>
+</p>
+<h4 align="center">
+    <p>
+        <b>English</b> |
+        <a href="https://github.com/PanQiWei/AutoGPTQ/blob/main/README_zh.md">中文</a>
+    </p>
+</h4>
+
+*<center>📣 Long time no see! 👋 Architecture upgrade, performance optimization and more new features will come in July and August, stay tune! 🥂</center>*
+
+## News or Update
+
+- 2023-07-26 - (Update) - An elegant [PPL benchmark script](examples/benchmark/perplexity.py) to get results that can be fairly compared with other libraries such as `llama.cpp`.
+- 2023-06-05 - (Update) - Integrate with 🤗 peft to use gptq quantized model to train adapters, support LoRA, AdaLoRA, AdaptionPrompt, etc.
+- 2023-05-30 - (Update) - Support download/upload quantized model from/to 🤗 Hub.
+- 2023-05-27 - (Update) - Support quantization and inference for `gpt_bigcode`, `codegen` and `RefineWeb/RefineWebModel`(falcon) model types.
+- 2023-05-04 - (Update) - Support using faster cuda kernel when `not desc_act or group_size == -1`.
+
+*For more histories please turn to [here](docs/NEWS_OR_UPDATE.md)*
+
+## Performance Comparison
+
+### Inference Speed
+> The result is generated using [this script](examples/benchmark/generation_speed.py), batch size of input is 1, decode strategy is beam search and enforce the model to generate 512 tokens, speed metric is tokens/s (the larger, the better).
+> 
+> The quantized model is loaded using the setup that can gain the fastest inference speed.
+
+| model         | GPU           | num_beams | fp16  | gptq-int4 |
+|---------------|---------------|-----------|-------|-----------|
+| llama-7b      | 1xA100-40G    | 1         | 18.87 | 25.53     |
+| llama-7b      | 1xA100-40G    | 4         | 68.79 | 91.30     |
+| moss-moon 16b | 1xA100-40G    | 1         | 12.48 | 15.25     |
+| moss-moon 16b | 1xA100-40G    | 4         | OOM   | 42.67     |
+| moss-moon 16b | 2xA100-40G    | 1         | 06.83 | 06.78     |
+| moss-moon 16b | 2xA100-40G    | 4         | 13.10 | 10.80     |
+| gpt-j 6b      | 1xRTX3060-12G | 1         | OOM   | 29.55     |
+| gpt-j 6b      | 1xRTX3060-12G | 4         | OOM   | 47.36     |
+
+
+### Perplexity
+For perplexity comparison, you can turn to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes)
+
+## Installation
+
+### Quick Installation
+You can install the latest stable release of AutoGPTQ from pip:
+```shell
+pip install auto-gptq
+```
+Start from v0.2.0, you can download pre-build wheel that satisfied your environment setup from each version's release assets and install it to skip building stage for the fastest installation speed. For example:
+```shell
+# firstly, cd the directory where the wheel saved, then execute command below
+pip install auto_gptq-0.2.0+cu118-cp310-cp310-linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for linux in an environment whose python=3.10 and cuda=11.8
+```
+#### disable cuda extensions
+By default, cuda extensions will be installed when `torch` and `cuda` is already installed in your machine, if you don't want to use them, using:
+```shell
+BUILD_CUDA_EXT=0 pip install auto-gptq
+```
+And to make sure `autogptq_cuda` is not ever in your virtual environment, run:
+```shell
+pip uninstall autogptq_cuda -y
+```
+
+#### to support triton speedup
+To integrate with `triton`, using:
+> warning: currently triton only supports linux; 3-bit quantization is not supported when using triton
+
+```shell
+pip install auto-gptq[triton]
+```
+
+### Install from source
+<details>
+<summary>click to see details</summary>
+
+Clone the source code:
+```shell
+git clone https://github.com/PanQiWei/AutoGPTQ.git && cd AutoGPTQ
+```
+Then, install from source:
+```shell
+pip install .
+```
+Like quick installation, you can also set `BUILD_CUDA_EXT=0` to disable pytorch extension building.
+
+Use `.[triton]` if you want to integrate with triton and it's available on your operating system.
+
+</details>
+
+## Quick Tour
+
+### Quantization and Inference
+> warning: this is just a showcase of the usage of basic apis in AutoGPTQ, which uses only one sample to quantize a much small model, quality of quantized model using such little samples may not good.
+
+Below is an example for the simplest use of `auto_gptq` to quantize a model and inference after quantization: 
+```python
+from transformers import AutoTokenizer, TextGenerationPipeline
+from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
+import logging
+
+logging.basicConfig(
+    format="%(asctime)s %(levelname)s [%(name)s] %(message)s", level=logging.INFO, datefmt="%Y-%m-%d %H:%M:%S"
+)
+
+pretrained_model_dir = "facebook/opt-125m"
+quantized_model_dir = "opt-125m-4bit"
+
+tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir, use_fast=True)
+examples = [
+    tokenizer(
+        "auto-gptq is an easy-to-use model quantization library with user-friendly apis, based on GPTQ algorithm."
+    )
+]
+
+quantize_config = BaseQuantizeConfig(
+    bits=4,  # quantize model to 4-bit
+    group_size=128,  # it is recommended to set the value to 128
+    desc_act=False,  # set to False can significantly speed up inference but the perplexity may slightly bad 
+)
+
+# load un-quantized model, by default, the model will always be loaded into CPU memory
+model = AutoGPTQForCausalLM.from_pretrained(pretrained_model_dir, quantize_config)
+
+# quantize model, the examples should be list of dict whose keys can only be "input_ids" and "attention_mask"
+model.quantize(examples)
+
+# save quantized model
+model.save_quantized(quantized_model_dir)
+
+# save quantized model using safetensors
+model.save_quantized(quantized_model_dir, use_safetensors=True)
+
+# push quantized model to Hugging Face Hub. 
+# to use use_auth_token=True, Login first via huggingface-cli login.
+# or pass explcit token with: use_auth_token="hf_xxxxxxx"
+# (uncomment the following three lines to enable this feature)
+# repo_id = f"YourUserName/{quantized_model_dir}"
+# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
+# model.push_to_hub(repo_id, commit_message=commit_message, use_auth_token=True)
+
+# alternatively you can save and push at the same time
+# (uncomment the following three lines to enable this feature)
+# repo_id = f"YourUserName/{quantized_model_dir}"
+# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
+# model.push_to_hub(repo_id, save_dir=quantized_model_dir, use_safetensors=True, commit_message=commit_message, use_auth_token=True)
+
+# load quantized model to the first GPU
+model = AutoGPTQForCausalLM.from_quantized(quantized_model_dir, device="cuda:0")
+
+# download quantized model from Hugging Face Hub and load to the first GPU
+# model = AutoGPTQForCausalLM.from_quantized(repo_id, device="cuda:0", use_safetensors=True, use_triton=False)
+
+# inference with model.generate
+print(tokenizer.decode(model.generate(**tokenizer("auto_gptq is", return_tensors="pt").to(model.device))[0]))
+
+# or you can also use pipeline
+pipeline = TextGenerationPipeline(model=model, tokenizer=tokenizer)
+print(pipeline("auto-gptq is")[0]["generated_text"])
+```
+
+For more advanced features of model quantization, please reference to [this script](examples/quantization/quant_with_alpaca.py)
+
+### Customize Model
+<details>
+
+<summary>Below is an example to extend `auto_gptq` to support `OPT` model, as you will see, it's very easy:</summary>
+
+```python
+from auto_gptq.modeling import BaseGPTQForCausalLM
+
+
+class OPTGPTQForCausalLM(BaseGPTQForCausalLM):
+    # chained attribute name of transformer layer block
+    layers_block_name = "model.decoder.layers"
+    # chained attribute names of other nn modules that in the same level as the transformer layer block
+    outside_layer_modules = [
+        "model.decoder.embed_tokens", "model.decoder.embed_positions", "model.decoder.project_out",
+        "model.decoder.project_in", "model.decoder.final_layer_norm"
+    ]
+    # chained attribute names of linear layers in transformer layer module
+    # normally, there are four sub lists, for each one the modules in it can be seen as one operation, 
+    # and the order should be the order when they are truly executed, in this case (and usually in most cases), 
+    # they are: attention q_k_v projection, attention output projection, MLP project input, MLP project output
+    inside_layer_modules = [
+        ["self_attn.k_proj", "self_attn.v_proj", "self_attn.q_proj"],
+        ["self_attn.out_proj"],
+        ["fc1"],
+        ["fc2"]
+    ]
+```
+After this, you can use `OPTGPTQForCausalLM.from_pretrained` and other methods as shown in Basic.
+
+</details>
+
+### Evaluation on Downstream Tasks
+You can use tasks defined in `auto_gptq.eval_tasks` to evaluate model's performance on specific down-stream task before and after quantization.
+
+The predefined tasks support all causal-language-models implemented in [🤗 transformers](https://github.com/huggingface/transformers) and in this project.
+
+<details>
+
+<summary>Below is an example to evaluate `EleutherAI/gpt-j-6b` on sequence-classification task using `cardiffnlp/tweet_sentiment_multilingual` dataset:</summary>
+
+```python
+from functools import partial
+
+import datasets
+from transformers import AutoTokenizer, AutoModelForCausalLM, GenerationConfig
+
+from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
+from auto_gptq.eval_tasks import SequenceClassificationTask
+
+
+MODEL = "EleutherAI/gpt-j-6b"
+DATASET = "cardiffnlp/tweet_sentiment_multilingual"
+TEMPLATE = "Question:What's the sentiment of the given text? Choices are {labels}.\nText: {text}\nAnswer:"
+ID2LABEL = {
+    0: "negative",
+    1: "neutral",
+    2: "positive"
+}
+LABELS = list(ID2LABEL.values())
+
+
+def ds_refactor_fn(samples):
+    text_data = samples["text"]
+    label_data = samples["label"]
+
+    new_samples = {"prompt": [], "label": []}
+    for text, label in zip(text_data, label_data):
+        prompt = TEMPLATE.format(labels=LABELS, text=text)
+        new_samples["prompt"].append(prompt)
+        new_samples["label"].append(ID2LABEL[label])
+
+    return new_samples
+
+
+#  model = AutoModelForCausalLM.from_pretrained(MODEL).eval().half().to("cuda:0")
+model = AutoGPTQForCausalLM.from_pretrained(MODEL, BaseQuantizeConfig())
+tokenizer = AutoTokenizer.from_pretrained(MODEL)
+
+task = SequenceClassificationTask(
+        model=model,
+        tokenizer=tokenizer,
+        classes=LABELS,
+        data_name_or_path=DATASET,
+        prompt_col_name="prompt",
+        label_col_name="label",
+        **{
+            "num_samples": 1000,  # how many samples will be sampled to evaluation
+            "sample_max_len": 1024,  # max tokens for each sample
+            "block_max_len": 2048,  # max tokens for each data block
+            # function to load dataset, one must only accept data_name_or_path as input 
+            # and return datasets.Dataset
+            "load_fn": partial(datasets.load_dataset, name="english"),  
+            # function to preprocess dataset, which is used for datasets.Dataset.map, 
+            # must return Dict[str, list] with only two keys: [prompt_col_name, label_col_name]
+            "preprocess_fn": ds_refactor_fn,  
+            # truncate label when sample's length exceed sample_max_len
+            "truncate_prompt": False  
+        }
+    )
+
+# note that max_new_tokens will be automatically specified internally based on given classes
+print(task.run())
+
+# self-consistency
+print(
+    task.run(
+        generation_config=GenerationConfig(
+            num_beams=3,
+            num_return_sequences=3,
+            do_sample=True
+        )
+    )
+)
+```
+
+</details>
+
+## Learn More
+[tutorials](docs/tutorial) provide step-by-step guidance to integrate `auto_gptq` with your own project and some best practice principles.
+
+[examples](examples/README.md) provide plenty of example scripts to use `auto_gptq` in different ways.
+
+## Supported Models
+
+> you can use `model.config.model_type` to compare with the table below to check whether the model you use is supported by `auto_gptq`.
+> 
+> for example, model_type of `WizardLM`, `vicuna` and `gpt4all` are all `llama`, hence they are all supported by `auto_gptq`.
+
+| model type                         | quantization | inference | peft-lora | peft-ada-lora | peft-adaption_prompt                                                                            |
+|------------------------------------|--------------|-----------|-----------|---------------|-------------------------------------------------------------------------------------------------|
+| bloom                              | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| gpt2                               | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| gpt_neox                           | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
+| gptj                               | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
+| llama                              | ✅            | ✅         | ✅         | ✅             | ✅                                                                                               |
+| moss                               | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
+| opt                                | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| gpt_bigcode                        | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| codegen                            | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| falcon(RefinedWebModel/RefinedWeb) | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+
+## Supported Evaluation Tasks
+Currently, `auto_gptq` supports: `LanguageModelingTask`, `SequenceClassificationTask` and `TextSummarizationTask`; more Tasks will come soon!
+
+## Acknowledgement
+- Specially thanks **Elias Frantar**, **Saleh Ashkboos**, **Torsten Hoefler** and **Dan Alistarh** for proposing **GPTQ** algorithm and open source the [code](https://github.com/IST-DASLab/gptq).
+- Specially thanks **qwopqwop200**, for code in this project that relevant to quantization are mainly referenced from [GPTQ-for-LLaMa](https://github.com/qwopqwop200/GPTQ-for-LLaMa/tree/cuda).
+
+
+[![Star History Chart](https://api.star-history.com/svg?repos=PanQiwei/AutoGPTQ&type=Date)](https://star-history.com/#PanQiWei/AutoGPTQ&Date)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auto-gptq Version: 0.3.0 Summary: An easy-to-use
+Metadata-Version: 2.1 Name: auto-gptq Version: 0.3.1 Summary: An easy-to-use
 LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
 Home-page: https://github.com/PanQiWei/AutoGPTQ Author: PanQiWei Keywords:
 gptq,quantization,large-language-models,pytorch,transformers Platform: windows
 Platform: linux Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8 Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: Chinese
 (Simplified) Classifier: Natural Language :: English Classifier: Programming
@@ -14,82 +14,84 @@
 An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ
                                   algorithm.
                       [GitHub_release] [PyPI_-_Downloads]
                            *** English | ä¸­æ ***
 *
 ð£ Long time no see! ð Architecture upgrade, performance optimization and
         more new features will come in July and August, stay tune! ð¥
-* ## News or Update - 2023-06-05 - (Update) - Integrate with ð¤ peft to use
-gptq quantized model to train adapters, support LoRA, AdaLoRA, AdaptionPrompt,
-etc. - 2023-05-30 - (Update) - Support download/upload quantized model from/to
-ð¤ Hub. - 2023-05-27 - (Update) - Support quantization and inference for
-`gpt_bigcode`, `codegen` and `RefineWeb/RefineWebModel`(falcon) model types. -
-2023-05-04 - (Update) - Support using faster cuda kernel when `not desc_act or
-group_size == -1`. *For more histories please turn to [here](docs/
-NEWS_OR_UPDATE.md)* ## Performance Comparison ### Inference Speed > The result
-is generated using [this script](examples/benchmark/generation_speed.py), batch
-size of input is 1, decode strategy is beam search and enforce the model to
-generate 512 tokens, speed metric is tokens/s (the larger, the better). > > The
-quantized model is loaded using the setup that can gain the fastest inference
-speed. | model | GPU | num_beams | fp16 | gptq-int4 | |---------------|--------
--------|-----------|-------|-----------| | llama-7b | 1xA100-40G | 1 | 18.87 |
-25.53 | | llama-7b | 1xA100-40G | 4 | 68.79 | 91.30 | | moss-moon 16b | 1xA100-
-40G | 1 | 12.48 | 15.25 | | moss-moon 16b | 1xA100-40G | 4 | OOM | 42.67 | |
-moss-moon 16b | 2xA100-40G | 1 | 06.83 | 06.78 | | moss-moon 16b | 2xA100-40G |
-4 | 13.10 | 10.80 | | gpt-j 6b | 1xRTX3060-12G | 1 | OOM | 29.55 | | gpt-j 6b |
-1xRTX3060-12G | 4 | OOM | 47.36 | ### Perplexity For perplexity comparison, you
-can turn to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and
-[here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes) ##
-Installation ### Quick Installation You can install the latest stable release
-of AutoGPTQ from pip: ```shell pip install auto-gptq ``` Start from v0.2.0, you
-can download pre-build wheel that satisfied your environment setup from each
-version's release assets and install it to skip building stage for the fastest
-installation speed. For example: ```shell # firstly, cd the directory where the
-wheel saved, then execute command below pip install auto_gptq-0.2.0+cu118-
-cp310-cp310-linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for
-linux in an environment whose python=3.10 and cuda=11.8 ``` #### disable cuda
-extensions By default, cuda extensions will be installed when `torch` and
-`cuda` is already installed in your machine, if you don't want to use them,
-using: ```shell BUILD_CUDA_EXT=0 pip install auto-gptq ``` And to make sure
-`autogptq_cuda` is not ever in your virtual environment, run: ```shell pip
-uninstall autogptq_cuda -y ``` #### to support triton speedup To integrate with
-`triton`, using: > warning: currently triton only supports linux; 3-bit
-quantization is not supported when using triton ```shell pip install auto-gptq
-[triton] ``` ### Install from source  click to see details Clone the source
-code: ```shell git clone https://github.com/PanQiWei/AutoGPTQ.git && cd
-AutoGPTQ ``` Then, install from source: ```shell pip install . ``` Like quick
-installation, you can also set `BUILD_CUDA_EXT=0` to disable pytorch extension
-building. Use `.[triton]` if you want to integrate with triton and it's
-available on your operating system.  ## Quick Tour ### Quantization and
-Inference > warning: this is just a showcase of the usage of basic apis in
-AutoGPTQ, which uses only one sample to quantize a much small model, quality of
-quantized model using such little samples may not good. Below is an example for
-the simplest use of `auto_gptq` to quantize a model and inference after
-quantization: ```python from transformers import AutoTokenizer,
-TextGenerationPipeline from auto_gptq import AutoGPTQForCausalLM,
-BaseQuantizeConfig import logging logging.basicConfig( format="%(asctime)s %
-(levelname)s [%(name)s] %(message)s", level=logging.INFO, datefmt="%Y-%m-%d %H:
-%M:%S" ) pretrained_model_dir = "facebook/opt-125m" quantized_model_dir = "opt-
-125m-4bit" tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir,
-use_fast=True) examples = [ tokenizer( "auto-gptq is an easy-to-use model
-quantization library with user-friendly apis, based on GPTQ algorithm." ) ]
-quantize_config = BaseQuantizeConfig( bits=4, # quantize model to 4-bit
-group_size=128, # it is recommended to set the value to 128 desc_act=False, #
-set to False can significantly speed up inference but the perplexity may
-slightly bad ) # load un-quantized model, by default, the model will always be
-loaded into CPU memory model = AutoGPTQForCausalLM.from_pretrained
-(pretrained_model_dir, quantize_config) # quantize model, the examples should
-be list of dict whose keys can only be "input_ids" and "attention_mask"
-model.quantize(examples) # save quantized model model.save_quantized
-(quantized_model_dir) # save quantized model using safetensors
-model.save_quantized(quantized_model_dir, use_safetensors=True) # push
-quantized model to Hugging Face Hub. # to use use_auth_token=True, Login first
-via huggingface-cli login. # or pass explcit token with:
-use_auth_token="hf_xxxxxxx" # (uncomment the following three lines to enable
-this feature) # repo_id = f"YourUserName/{quantized_model_dir}" #
+* ## News or Update - 2023-07-26 - (Update) - An elegant [PPL benchmark script]
+(examples/benchmark/perplexity.py) to get results that can be fairly compared
+with other libraries such as `llama.cpp`. - 2023-06-05 - (Update) - Integrate
+with ð¤ peft to use gptq quantized model to train adapters, support LoRA,
+AdaLoRA, AdaptionPrompt, etc. - 2023-05-30 - (Update) - Support download/upload
+quantized model from/to ð¤ Hub. - 2023-05-27 - (Update) - Support
+quantization and inference for `gpt_bigcode`, `codegen` and `RefineWeb/
+RefineWebModel`(falcon) model types. - 2023-05-04 - (Update) - Support using
+faster cuda kernel when `not desc_act or group_size == -1`. *For more histories
+please turn to [here](docs/NEWS_OR_UPDATE.md)* ## Performance Comparison ###
+Inference Speed > The result is generated using [this script](examples/
+benchmark/generation_speed.py), batch size of input is 1, decode strategy is
+beam search and enforce the model to generate 512 tokens, speed metric is
+tokens/s (the larger, the better). > > The quantized model is loaded using the
+setup that can gain the fastest inference speed. | model | GPU | num_beams |
+fp16 | gptq-int4 | |---------------|---------------|-----------|-------|-------
+----| | llama-7b | 1xA100-40G | 1 | 18.87 | 25.53 | | llama-7b | 1xA100-40G | 4
+| 68.79 | 91.30 | | moss-moon 16b | 1xA100-40G | 1 | 12.48 | 15.25 | | moss-
+moon 16b | 1xA100-40G | 4 | OOM | 42.67 | | moss-moon 16b | 2xA100-40G | 1 |
+06.83 | 06.78 | | moss-moon 16b | 2xA100-40G | 4 | 13.10 | 10.80 | | gpt-j 6b |
+1xRTX3060-12G | 1 | OOM | 29.55 | | gpt-j 6b | 1xRTX3060-12G | 4 | OOM | 47.36
+| ### Perplexity For perplexity comparison, you can turn to [here](https://
+github.com/qwopqwop200/GPTQ-for-LLaMa#result) and [here](https://github.com/
+qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes) ## Installation ### Quick
+Installation You can install the latest stable release of AutoGPTQ from pip:
+```shell pip install auto-gptq ``` Start from v0.2.0, you can download pre-
+build wheel that satisfied your environment setup from each version's release
+assets and install it to skip building stage for the fastest installation
+speed. For example: ```shell # firstly, cd the directory where the wheel saved,
+then execute command below pip install auto_gptq-0.2.0+cu118-cp310-cp310-
+linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for linux in an
+environment whose python=3.10 and cuda=11.8 ``` #### disable cuda extensions By
+default, cuda extensions will be installed when `torch` and `cuda` is already
+installed in your machine, if you don't want to use them, using: ```shell
+BUILD_CUDA_EXT=0 pip install auto-gptq ``` And to make sure `autogptq_cuda` is
+not ever in your virtual environment, run: ```shell pip uninstall autogptq_cuda
+-y ``` #### to support triton speedup To integrate with `triton`, using: >
+warning: currently triton only supports linux; 3-bit quantization is not
+supported when using triton ```shell pip install auto-gptq[triton] ``` ###
+Install from source  click to see details Clone the source code: ```shell git
+clone https://github.com/PanQiWei/AutoGPTQ.git && cd AutoGPTQ ``` Then, install
+from source: ```shell pip install . ``` Like quick installation, you can also
+set `BUILD_CUDA_EXT=0` to disable pytorch extension building. Use `.[triton]`
+if you want to integrate with triton and it's available on your operating
+system.  ## Quick Tour ### Quantization and Inference > warning: this is just a
+showcase of the usage of basic apis in AutoGPTQ, which uses only one sample to
+quantize a much small model, quality of quantized model using such little
+samples may not good. Below is an example for the simplest use of `auto_gptq`
+to quantize a model and inference after quantization: ```python from
+transformers import AutoTokenizer, TextGenerationPipeline from auto_gptq import
+AutoGPTQForCausalLM, BaseQuantizeConfig import logging logging.basicConfig
+( format="%(asctime)s %(levelname)s [%(name)s] %(message)s",
+level=logging.INFO, datefmt="%Y-%m-%d %H:%M:%S" ) pretrained_model_dir =
+"facebook/opt-125m" quantized_model_dir = "opt-125m-4bit" tokenizer =
+AutoTokenizer.from_pretrained(pretrained_model_dir, use_fast=True) examples =
+[ tokenizer( "auto-gptq is an easy-to-use model quantization library with user-
+friendly apis, based on GPTQ algorithm." ) ] quantize_config =
+BaseQuantizeConfig( bits=4, # quantize model to 4-bit group_size=128, # it is
+recommended to set the value to 128 desc_act=False, # set to False can
+significantly speed up inference but the perplexity may slightly bad ) # load
+un-quantized model, by default, the model will always be loaded into CPU memory
+model = AutoGPTQForCausalLM.from_pretrained(pretrained_model_dir,
+quantize_config) # quantize model, the examples should be list of dict whose
+keys can only be "input_ids" and "attention_mask" model.quantize(examples) #
+save quantized model model.save_quantized(quantized_model_dir) # save quantized
+model using safetensors model.save_quantized(quantized_model_dir,
+use_safetensors=True) # push quantized model to Hugging Face Hub. # to use
+use_auth_token=True, Login first via huggingface-cli login. # or pass explcit
+token with: use_auth_token="hf_xxxxxxx" # (uncomment the following three lines
+to enable this feature) # repo_id = f"YourUserName/{quantized_model_dir}" #
 commit_message = f"AutoGPTQ model for {pretrained_model_dir}:
 {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act=
 {quantize_config.desc_act}" # model.push_to_hub(repo_id,
 commit_message=commit_message, use_auth_token=True) # alternatively you can
 save and push at the same time # (uncomment the following three lines to enable
 this feature) # repo_id = f"YourUserName/{quantized_model_dir}" #
 commit_message = f"AutoGPTQ model for {pretrained_model_dir}:
```

### Comparing `auto_gptq-0.3.0/auto_gptq.egg-info/SOURCES.txt` & `auto_gptq-0.3.1/auto_gptq.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,11 +48,12 @@
 auto_gptq/quantization/__init__.py
 auto_gptq/quantization/gptq.py
 auto_gptq/quantization/quantizer.py
 auto_gptq/utils/__init__.py
 auto_gptq/utils/data_utils.py
 auto_gptq/utils/import_utils.py
 auto_gptq/utils/peft_utils.py
+auto_gptq/utils/perplexity_utils.py
 autogptq_cuda/autogptq_cuda_256.cpp
 autogptq_cuda/autogptq_cuda_64.cpp
 autogptq_cuda/autogptq_cuda_kernel_256.cu
 autogptq_cuda/autogptq_cuda_kernel_64.cu
```

### Comparing `auto_gptq-0.3.0/autogptq_cuda/autogptq_cuda_256.cpp` & `auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_256.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,202 +1,187 @@
-#include <torch/all.h>
-#include <torch/python.h>
-#include <c10/cuda/CUDAGuard.h>
-
-void vecquant2matmul_cuda(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-);
-
-void vecquant2matmul(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant2matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
-}
-
-void vecquant3matmul_cuda(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-);
-
-void vecquant3matmul(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant3matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
-}
-
-void vecquant4matmul_cuda(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx, int vec_height
-);
-
-void vecquant4matmul(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx, int vec_height
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant4matmul_cuda(vec, mat, mul, scales, zeros, g_idx, vec_height);
-}
-
-//void vecquant4matmul_cuda(
-//  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-//  torch::Tensor scales, torch::Tensor zeros,
-//  torch::Tensor g_idx
-//);
-//
-//void vecquant4matmul(
-//  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-//  torch::Tensor scales, torch::Tensor zeros,
-//  torch::Tensor g_idx
-//) {
-//  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-//  vecquant4matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
-//}
-
-void vecquant8matmul_cuda(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-);
-
-void vecquant8matmul(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant8matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
-}
-
-
-// old
-
-void vecquant2matmul_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-); 
-
-void vecquant2matmul_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant2matmul_cuda_old(vec, mat, mul, scales, zeros,groupsize);
-}
-
-void vecquant3matmul_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-); 
-
-void vecquant3matmul_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant3matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
-}
-
-void vecquant4matmul_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-); 
-
-void vecquant4matmul_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant4matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
-}
-
-void vecquant8matmul_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-); 
-
-void vecquant8matmul_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant8matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
-}
-
-void vecquant2matmul_faster_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-); 
-
-void vecquant2matmul_faster_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant2matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
-}
-
-void vecquant3matmul_faster_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-); 
-
-void vecquant3matmul_faster_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant3matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
-}
-
-void vecquant4matmul_faster_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-); 
-
-void vecquant4matmul_faster_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant4matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
-}
-
-
-PYBIND11_MODULE(TORCH_EXTENSION_NAME, m) {
-  m.def("vecquant2matmul", &vecquant2matmul, "Vector 2-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
-  m.def("vecquant3matmul", &vecquant3matmul, "Vector 3-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
-  m.def("vecquant4matmul", &vecquant4matmul, "Vector 4-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
-  m.def("vecquant8matmul", &vecquant8matmul, "Vector 8-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
-  
-  m.def("vecquant2matmul_old", &vecquant2matmul_old, "Vector 2-bit Quantized Matrix Multiplication (CUDA)");
-  m.def("vecquant3matmul_old", &vecquant3matmul_old, "Vector 3-bit Quantized Matrix Multiplication (CUDA)");
-  m.def("vecquant4matmul_old", &vecquant4matmul_old, "Vector 4-bit Quantized Matrix Multiplication (CUDA)");
-  m.def("vecquant8matmul_old", &vecquant8matmul_old, "Vector 8-bit Quantized Matrix Multiplication (CUDA)");
-  m.def("vecquant2matmul_faster_old", &vecquant2matmul_faster_old, "Vector 2-bit Quantized Matrix Multiplication (CUDA), faster version");
-  m.def("vecquant3matmul_faster_old", &vecquant3matmul_faster_old, "Vector 3-bit Quantized Matrix Multiplication (CUDA), faster version");
-  m.def("vecquant4matmul_faster_old", &vecquant4matmul_faster_old, "Vector 4-bit Quantized Matrix Multiplication (CUDA), faster version");
-}
+#include <torch/all.h>
+#include <torch/python.h>
+#include <c10/cuda/CUDAGuard.h>
+
+void vecquant2matmul_cuda(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+);
+
+void vecquant2matmul(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant2matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
+}
+
+void vecquant3matmul_cuda(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+);
+
+void vecquant3matmul(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant3matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
+}
+
+void vecquant4matmul_cuda(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+);
+
+void vecquant4matmul(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant4matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
+}
+
+void vecquant8matmul_cuda(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+);
+
+void vecquant8matmul(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant8matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
+}
+
+
+// old
+
+void vecquant2matmul_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+); 
+
+void vecquant2matmul_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant2matmul_cuda_old(vec, mat, mul, scales, zeros,groupsize);
+}
+
+void vecquant3matmul_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+); 
+
+void vecquant3matmul_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant3matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
+}
+
+void vecquant4matmul_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+); 
+
+void vecquant4matmul_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant4matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
+}
+
+void vecquant8matmul_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+); 
+
+void vecquant8matmul_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant8matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
+}
+
+void vecquant2matmul_faster_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+); 
+
+void vecquant2matmul_faster_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant2matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
+}
+
+void vecquant3matmul_faster_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+); 
+
+void vecquant3matmul_faster_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant3matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
+}
+
+void vecquant4matmul_faster_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+); 
+
+void vecquant4matmul_faster_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant4matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
+}
+
+
+PYBIND11_MODULE(TORCH_EXTENSION_NAME, m) {
+  m.def("vecquant2matmul", &vecquant2matmul, "Vector 2-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
+  m.def("vecquant3matmul", &vecquant3matmul, "Vector 3-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
+  m.def("vecquant4matmul", &vecquant4matmul, "Vector 4-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
+  m.def("vecquant8matmul", &vecquant8matmul, "Vector 8-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
+  
+  m.def("vecquant2matmul_old", &vecquant2matmul_old, "Vector 2-bit Quantized Matrix Multiplication (CUDA)");
+  m.def("vecquant3matmul_old", &vecquant3matmul_old, "Vector 3-bit Quantized Matrix Multiplication (CUDA)");
+  m.def("vecquant4matmul_old", &vecquant4matmul_old, "Vector 4-bit Quantized Matrix Multiplication (CUDA)");
+  m.def("vecquant8matmul_old", &vecquant8matmul_old, "Vector 8-bit Quantized Matrix Multiplication (CUDA)");
+  m.def("vecquant2matmul_faster_old", &vecquant2matmul_faster_old, "Vector 2-bit Quantized Matrix Multiplication (CUDA), faster version");
+  m.def("vecquant3matmul_faster_old", &vecquant3matmul_faster_old, "Vector 3-bit Quantized Matrix Multiplication (CUDA), faster version");
+  m.def("vecquant4matmul_faster_old", &vecquant4matmul_faster_old, "Vector 4-bit Quantized Matrix Multiplication (CUDA), faster version");
+}
```

### Comparing `auto_gptq-0.3.0/autogptq_cuda/autogptq_cuda_64.cpp` & `auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_64.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,202 +1,187 @@
-#include <torch/all.h>
-#include <torch/python.h>
-#include <c10/cuda/CUDAGuard.h>
-
-void vecquant2matmul_cuda(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-);
-
-void vecquant2matmul(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant2matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
-}
-
-void vecquant3matmul_cuda(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-);
-
-void vecquant3matmul(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant3matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
-}
-
-void vecquant4matmul_cuda(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx, int vec_height
-);
-
-void vecquant4matmul(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx, int vec_height
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant4matmul_cuda(vec, mat, mul, scales, zeros, g_idx, vec_height);
-}
-
-//void vecquant4matmul_cuda(
-//  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-//  torch::Tensor scales, torch::Tensor zeros,
-//  torch::Tensor g_idx
-//);
-//
-//void vecquant4matmul(
-//  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-//  torch::Tensor scales, torch::Tensor zeros,
-//  torch::Tensor g_idx
-//) {
-//  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-//  vecquant4matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
-//}
-
-void vecquant8matmul_cuda(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-);
-
-void vecquant8matmul(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant8matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
-}
-
-
-// old
-
-void vecquant2matmul_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-); 
-
-void vecquant2matmul_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant2matmul_cuda_old(vec, mat, mul, scales, zeros,groupsize);
-}
-
-void vecquant3matmul_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-); 
-
-void vecquant3matmul_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant3matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
-}
-
-void vecquant4matmul_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-); 
-
-void vecquant4matmul_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant4matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
-}
-
-void vecquant8matmul_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-); 
-
-void vecquant8matmul_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant8matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
-}
-
-void vecquant2matmul_faster_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-); 
-
-void vecquant2matmul_faster_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant2matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
-}
-
-void vecquant3matmul_faster_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-); 
-
-void vecquant3matmul_faster_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant3matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
-}
-
-void vecquant4matmul_faster_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-); 
-
-void vecquant4matmul_faster_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant4matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
-}
-
-
-PYBIND11_MODULE(TORCH_EXTENSION_NAME, m) {
-  m.def("vecquant2matmul", &vecquant2matmul, "Vector 2-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
-  m.def("vecquant3matmul", &vecquant3matmul, "Vector 3-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
-  m.def("vecquant4matmul", &vecquant4matmul, "Vector 4-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
-  m.def("vecquant8matmul", &vecquant8matmul, "Vector 8-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
-  
-  m.def("vecquant2matmul_old", &vecquant2matmul_old, "Vector 2-bit Quantized Matrix Multiplication (CUDA)");
-  m.def("vecquant3matmul_old", &vecquant3matmul_old, "Vector 3-bit Quantized Matrix Multiplication (CUDA)");
-  m.def("vecquant4matmul_old", &vecquant4matmul_old, "Vector 4-bit Quantized Matrix Multiplication (CUDA)");
-  m.def("vecquant8matmul_old", &vecquant8matmul_old, "Vector 8-bit Quantized Matrix Multiplication (CUDA)");
-  m.def("vecquant2matmul_faster_old", &vecquant2matmul_faster_old, "Vector 2-bit Quantized Matrix Multiplication (CUDA), faster version");
-  m.def("vecquant3matmul_faster_old", &vecquant3matmul_faster_old, "Vector 3-bit Quantized Matrix Multiplication (CUDA), faster version");
-  m.def("vecquant4matmul_faster_old", &vecquant4matmul_faster_old, "Vector 4-bit Quantized Matrix Multiplication (CUDA), faster version");
-}
+#include <torch/all.h>
+#include <torch/python.h>
+#include <c10/cuda/CUDAGuard.h>
+
+void vecquant2matmul_cuda(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+);
+
+void vecquant2matmul(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant2matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
+}
+
+void vecquant3matmul_cuda(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+);
+
+void vecquant3matmul(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant3matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
+}
+
+void vecquant4matmul_cuda(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+);
+
+void vecquant4matmul(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant4matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
+}
+
+void vecquant8matmul_cuda(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+);
+
+void vecquant8matmul(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant8matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
+}
+
+
+// old
+
+void vecquant2matmul_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+); 
+
+void vecquant2matmul_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant2matmul_cuda_old(vec, mat, mul, scales, zeros,groupsize);
+}
+
+void vecquant3matmul_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+); 
+
+void vecquant3matmul_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant3matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
+}
+
+void vecquant4matmul_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+); 
+
+void vecquant4matmul_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant4matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
+}
+
+void vecquant8matmul_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+); 
+
+void vecquant8matmul_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant8matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
+}
+
+void vecquant2matmul_faster_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+); 
+
+void vecquant2matmul_faster_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant2matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
+}
+
+void vecquant3matmul_faster_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+); 
+
+void vecquant3matmul_faster_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant3matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
+}
+
+void vecquant4matmul_faster_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+); 
+
+void vecquant4matmul_faster_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant4matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
+}
+
+
+PYBIND11_MODULE(TORCH_EXTENSION_NAME, m) {
+  m.def("vecquant2matmul", &vecquant2matmul, "Vector 2-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
+  m.def("vecquant3matmul", &vecquant3matmul, "Vector 3-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
+  m.def("vecquant4matmul", &vecquant4matmul, "Vector 4-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
+  m.def("vecquant8matmul", &vecquant8matmul, "Vector 8-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
+  
+  m.def("vecquant2matmul_old", &vecquant2matmul_old, "Vector 2-bit Quantized Matrix Multiplication (CUDA)");
+  m.def("vecquant3matmul_old", &vecquant3matmul_old, "Vector 3-bit Quantized Matrix Multiplication (CUDA)");
+  m.def("vecquant4matmul_old", &vecquant4matmul_old, "Vector 4-bit Quantized Matrix Multiplication (CUDA)");
+  m.def("vecquant8matmul_old", &vecquant8matmul_old, "Vector 8-bit Quantized Matrix Multiplication (CUDA)");
+  m.def("vecquant2matmul_faster_old", &vecquant2matmul_faster_old, "Vector 2-bit Quantized Matrix Multiplication (CUDA), faster version");
+  m.def("vecquant3matmul_faster_old", &vecquant3matmul_faster_old, "Vector 3-bit Quantized Matrix Multiplication (CUDA), faster version");
+  m.def("vecquant4matmul_faster_old", &vecquant4matmul_faster_old, "Vector 4-bit Quantized Matrix Multiplication (CUDA), faster version");
+}
```

### Comparing `auto_gptq-0.3.0/autogptq_cuda/autogptq_cuda_kernel_256.cu` & `auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_kernel_256.cu`

 * *Files 22% similar despite different names*

```diff
@@ -1,1560 +1,1427 @@
-#include <torch/all.h>
-#include <torch/python.h>
-#include <cuda.h>
-#include <cuda_runtime.h>
-#include <cuda_fp16.h>
-
-// atomicAdd for double-precision floating-point numbers on hardware with
-// compute capability < 6.0 from:
-// https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#atomic-functions
-// #if defined(__CUDA_ARCH__) && __CUDA_ARCH__ < 600
-// __device__ double atomicAdd(
-//     double* address,
-//     double val
-// ) {
-//   unsigned long long int* address_as_ull = (unsigned long long int*)address;
-//   unsigned long long int old = *address_as_ull, assumed;
-//
-//   do {
-//     assumed = old;
-//     old = atomicCAS(
-//       address_as_ull,
-//       assumed,
-//       __double_as_longlong(val + __longlong_as_double(assumed))
-//     );
-//
-//   // Note: uses integer comparison to avoid hang in case of NaN (since NaN != NaN)
-//   } while (assumed != old);
-//
-//   return __longlong_as_double(old);
-// }
-// #endif
-
-#if defined(__CUDA_ARCH__) && __CUDA_ARCH__ < 700
-// adapted from https://github.com/torch/cutorch/blob/master/lib/THC/THCAtomics.cuh
-__device__ __forceinline__ void atomicAdd(c10::Half* address, c10::Half val) {
-    unsigned int *address_as_ui = reinterpret_cast<unsigned int *>(reinterpret_cast<char *>(address) - (reinterpret_cast<size_t>(address) & 2));
-    unsigned int old = *address_as_ui;
-    unsigned int assumed;
-
-    do {
-        assumed = old;
-        unsigned short hsum = reinterpret_cast<size_t>(address) & 2 ? (old >> 16) : (old & 0xffff);
-        hsum += val;
-        old = reinterpret_cast<size_t>(address) & 2
-                 ? (old & 0xffff) | (hsum << 16)
-                 : (old & 0xffff0000) | hsum;
-        old = atomicCAS(address_as_ui, assumed, old);
-
-    // Note: uses integer comparison to avoid hang in case of NaN (since NaN != NaN)
-    } while (assumed != old);
-}
-__device__ __forceinline__ void atomicAdd(__half* address, c10::Half val) {
-    unsigned int * address_as_ui = (unsigned int *) ((char *)address - ((size_t)address & 2));
-    unsigned int old = *address_as_ui;
-    unsigned int assumed;
-
-    do {
-        assumed = old;
-        __half_raw hsum;
-        hsum.x = (size_t)address & 2 ? (old >> 16) : (old & 0xffff);
-        half tmpres = __hadd(hsum, val);
-        hsum = __half_raw(tmpres);
-        old = (size_t)address & 2 ? (old & 0xffff) | (hsum.x << 16) : (old & 0xffff0000) | hsum.x;
-        old = atomicCAS(address_as_ui, assumed, old);
-    } while (assumed != old);
-}
-#endif
-
-
-template <typename scalar_t>
-__global__ void VecQuant2MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-	const  	    int* __restrict__ g_idx,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-	int zero_width
-);
-
-template <typename scalar_t>
-__global__ void VecQuant3MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-	const  	    int* __restrict__ g_idx,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-	int zero_width
-);
-
-// template <typename scalar_t>
-// __global__ void VecQuant4MatMulKernel(
-//     const  scalar_t* __restrict__ vec,
-//     const       int* __restrict__ mat,
-//            scalar_t* __restrict__ mul,
-//     const  scalar_t* __restrict__ scales,
-//     const  		int* __restrict__ zeros,
-// 	const  	    int* __restrict__ g_idx,
-//     int batch,
-//     int vec_height,
-//     int height,
-//     int width,
-// 	int zero_width
-// );
-
-// referenced from https://github.com/iwalton3/GPTQ-for-LLaMa/commit/209d16b0187f149bf13318360925cc4f679cb2ea
-template <typename scalar_t>
-__global__ void VecQuant4MatMulKernel(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const    int* __restrict__ zeros,
-    const    int* __restrict__ g_idx,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width
-);
-
-template <typename scalar_t>
-__global__ void VecQuant8MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-	const  	    int* __restrict__ g_idx,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-	int zero_width
-);
-
-template <typename scalar_t>
-__global__ void VecQuant2MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-template <typename scalar_t>
-__global__ void VecQuant3MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-template <typename scalar_t>
-__global__ void VecQuant4MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-template <typename scalar_t>
-__global__ void VecQuant8MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-__global__ void VecQuant2MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const    int* __restrict__ zeros,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-__global__ void VecQuant3MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const    int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-__global__ void VecQuant4MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const    int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-
-const int BLOCKWIDTH  = 256;
-const int BLOCKHEIGHT2 =  16;
-const int BLOCKHEIGHT3 =  24;
-const int BLOCKHEIGHT4 =  32;
-const int BLOCKHEIGHT8 =  64;
-
-__device__ inline unsigned int as_unsigned(int i) {
-  return *reinterpret_cast<unsigned int*>(&i);
-}
-
-__device__ inline int as_int(int i) {
-  return *reinterpret_cast<int*>(&i);
-}
-
-
-void vecquant2matmul_cuda(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant2matmul_cuda", ([&] {
-      VecQuant2MatMulKernel<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
-        batch, vec_height, height, width, zero_width
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant2MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-    const   	int* __restrict__ g_idx,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-	int zero_width
-) {
-  int h = BLOCKHEIGHT2 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-  
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  int i = width * h + w;
-  int g_h = h * 16;
-  int k;
-  unsigned int g;
-  scalar_t w_tmp;
-  
-  int z_w = w / 16; 
-  int z_mod = (w % 16) * 2;
-  
-  float weight[BLOCKWIDTH];
-  
-  for (k = 0; k <  BLOCKWIDTH; ++k){	
-	int k_w = (k / 16); 
-	int k_bit = (k % 16) * 2;
-	
-    g = as_int(g_idx[g_h + k]);
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scalar_t((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod & 0x3) + 1);
-	
-    w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0x3);
-    
-	weight[k] = scale * (w_tmp - zero);
-  }
-
-  scalar_t res;
-  for (int b = 0; b < batch; ++b){	
-	res = 0;
-	
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-    __syncthreads();
-	for (k = 0; k <  BLOCKWIDTH; ++k){	
-	  res += weight[k] * blockvec[k];
-    }
-    atomicAdd(&mul[b * width + w], res);
-    __syncthreads();
-  }
-}
-
-void vecquant3matmul_cuda(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant3matmul_cuda", ([&] {
-      VecQuant3MatMulKernel<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
-        batch, vec_height, height, width, zero_width
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant3MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const       int* __restrict__ zeros,
-    const   	int* __restrict__ g_idx,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-	int zero_width
-) {
-  int h = BLOCKHEIGHT3 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-  
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  int i = width * h + w;
-  int g_h = (h / 3) * 32;
-  int k;
-  unsigned int g;
-  scalar_t w_tmp;
-  
-  int z_w = (w / 32) * 3; 
-  int z_mod = w % 32;
-  int z_bit;
-  unsigned int z_tmp;
-  if (z_mod != 10){
-    if (z_mod != 21){
-      z_bit = z_mod;
-      if (z_bit > 21){
-        z_bit -= 22;
-        z_bit *= 3;
-        z_bit += 2;
-        z_w += 2;
-      } else if (z_bit > 10){
-        z_bit -= 11;
-        z_bit *= 3;
-        z_bit += 1;
-        z_w += 1;
-      } else {
-        z_bit *= 3;
-      }
-    } else {
-      z_w += 1;
-    }
-  }
-  
-  float weight[BLOCKWIDTH];
-  
-  for (k = 0; k <  BLOCKWIDTH; ++k){	
-	int k_w = (k / 32) * 3; 
-	int k_mod = k % 32;
-	int k_bit;
-	  
-	if (k_mod != 10){
-	  if (k_mod != 21){
-        k_bit = k_mod;
-        if (k_bit > 21){
-		  k_bit -= 22;
-		  k_bit *= 3;
-		  k_bit += 2;
-		  k_w += 2;
-        } else if (k_bit > 10){
-		  k_bit -= 11;
-		  k_bit *= 3;
-		  k_bit += 1;
-		  k_w += 1;
-        } else {
-		  k_bit *= 3;
-        }
-	  } else {
-        k_w += 1;
-	  }
-	}
-	
-    g = as_int(g_idx[g_h + k]);
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero;
-    if (z_mod == 10) {
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
-      zero = scalar_t((z_tmp) + 1);
-    } else if (z_mod == 21){
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
-      zero = scalar_t((z_tmp) + 1);
-    } else {
-      zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1);
-    }
-	
-    if (k_mod == 10) {
-      w_tmp = (as_unsigned(mat[i + (k_w * width)]) >> 30) | ((as_unsigned(mat[i + ((k_w + 1)* width)]) << 2) & 0x4);
-    } else if (k_mod == 21){
-      w_tmp = (as_unsigned(mat[i + (k_w * width)]) >> 31) | ((as_unsigned(mat[i + ((k_w + 1)* width)]) << 1) & 0x6);
-    } else {
-      w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0x7);
-    }
-	weight[k] = scale * (w_tmp - zero);
-  }
-
-  scalar_t res;
-  for (int b = 0; b < batch; ++b){	
-	res = 0;
-	
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-    __syncthreads();
-	for (k = 0; k <  BLOCKWIDTH; ++k){	
-	  res += weight[k] * blockvec[k];
-    }
-    atomicAdd(&mul[b * width + w], res);
-    __syncthreads();
-  }
-}
-
-void vecquant4matmul_cuda(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  torch::Tensor g_idx,
-  int vec_height
-) {
-  int batch = vec.size(0);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_SWITCH(vec.type(), "vecquant4matmul_cuda",
-    AT_DISPATCH_CASE(at::ScalarType::Half, ([&] {
-      VecQuant4MatMulKernel<<<blocks, threads>>>(
-        (half2*) vec.data_ptr<scalar_t>(),
-        mat.data_ptr<int>(),
-        mul.data_ptr<scalar_t>(),
-        scales.data_ptr<scalar_t>(),
-        zeros.data_ptr<int>(),
-        g_idx.data_ptr<int>(),
-        batch, vec_height, height, width, zero_width
-      );
-    })
-  ));
-}
-
-// void vecquant4matmul_cuda(
-//   torch::Tensor vec,
-//   torch::Tensor mat,
-//   torch::Tensor mul,
-//   torch::Tensor scales,
-//   torch::Tensor zeros,
-//   torch::Tensor g_idx
-// ) {
-//   int batch = vec.size(0);
-//   int vec_height = vec.size(1);
-//   int height = mat.size(0);
-//   int width = mat.size(1);
-//   int zero_width = zeros.size(1);
-//
-//   dim3 blocks(
-//     (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
-//     (width + BLOCKWIDTH - 1) / BLOCKWIDTH
-//   );
-//   dim3 threads(BLOCKWIDTH);
-//
-//   AT_DISPATCH_FLOATING_TYPES(
-//     vec.type(), "vecquant4matmul_cuda", ([&] {
-//       VecQuant4MatMulKernel<<<blocks, threads>>>(
-//         vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-//         scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(),
-//         batch, vec_height, height, width, zero_width
-//       );
-//     })
-//   );
-// }
-
-template <typename scalar_t>
-__global__ void VecQuant4MatMulKernel(
-    const     half2* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	    int* __restrict__ zeros,
-    const       int* __restrict__ g_idx,
-	int batch,
-	int vec_height,
-    int height,
-    int width,
-    int zero_width
-) {
-  const int blockwidth2 = BLOCKWIDTH / 2;
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT4 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ half2 blockvec[blockwidth2];
-  if (threadIdx.x < blockwidth2)
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
-
-  __shared__ half2 deq2[256][8];
-  int val = threadIdx.x / 8;
-  int off = threadIdx.x % 8;
-  for (; val < 256; val += BLOCKWIDTH / 8) {
-    deq2[val][off] = __halves2half2(
-       __int2half_rn(val & 0xF), __int2half_rn(val >> 4)
-    );
-  }
-
-  int i = width * h + w;
-  int g_h = h * 8;
-  int k = 0;
-
-  int z_w = w / 8;
-  int z_mod = (w % 8) * 4;
-
-  scalar_t res = 0;
-  half2 res2;
-
-  unsigned int tmp;
-
-  __syncthreads();
-
-  while (k < blockwidth2) {
-    res2 = {};
-    tmp = as_unsigned(mat[i]);
-
-    int tmp_k = 0;
-    half2 scales_tmp[4];
-    half2 zeros_tmp[4];
-    while (tmp_k < 4) {
-      int g = as_int(g_idx[g_h + (k + tmp_k) * 2]);
-      int g2 = as_int(g_idx[g_h + (k + tmp_k) * 2 + 1]);
-      scalar_t scale_f = scales[g * width + w];
-      scalar_t scale_f2 = scales[g2 * width + w];
-      half2 scale = __halves2half2(scale_f, scale_f2);
-      half2 zero = __halves2half2(
-        __hmul(-scale_f, __int2half_rn(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1)),
-        __hmul(-scale_f2, __int2half_rn(((as_unsigned(zeros[g2 * zero_width + z_w]) >> z_mod) & 0xF) + 1))
-      );
-      scales_tmp[tmp_k] = scale;
-      zeros_tmp[tmp_k] = zero;
-      tmp_k += 1;
-    }
-
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  0) & 0xff][off], scales_tmp[0], zeros_tmp[0]), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  8) & 0xff][off], scales_tmp[1], zeros_tmp[1]), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 16) & 0xff][off], scales_tmp[2], zeros_tmp[2]), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 24) & 0xff][off], scales_tmp[3], zeros_tmp[3]), blockvec[k + 3], res2);
-	i += width;
-    k += 4;
-    res = __hadd(res, __hadd(res2.x, res2.y));;
-  }
-
-  __half* mul2 = (__half*)mul;
-  atomicAdd(&mul2[b * width + w], res);
-}
-
-// template <typename scalar_t>
-// __global__ void VecQuant4MatMulKernel(
-//     const  scalar_t* __restrict__ vec,
-//     const       int* __restrict__ mat,
-//            scalar_t* __restrict__ mul,
-//     const  scalar_t* __restrict__ scales,
-//     const       int* __restrict__ zeros,
-//     const   	int* __restrict__ g_idx,
-//     int batch,
-//     int vec_height,
-//     int height,
-//     int width,
-// 	int zero_width
-// ) {
-//   int h = BLOCKHEIGHT4 * blockIdx.x;
-//   int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-//
-//   __shared__ scalar_t blockvec[BLOCKWIDTH];
-//   int i = width * h + w;
-//   int g_h = h * 8;
-//   int k;
-//   unsigned int g;
-//   scalar_t w_tmp;
-//
-//
-//   int z_w = w / 8;
-//   int z_mod = (w % 8) * 4;
-//
-//   float weight[BLOCKWIDTH];
-//
-//   for (k = 0; k <  BLOCKWIDTH; ++k){
-// 	int k_w = (k / 8);
-// 	int k_bit = (k % 8) * 4;
-//
-//     g = as_int(g_idx[g_h + k]);
-//     scalar_t scale = scales[g * width + w];
-//     scalar_t zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1);
-//
-//     w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0xF);
-//
-// 	weight[k] = scale * (w_tmp - zero);
-//   }
-//
-//   scalar_t res;
-//   for (int b = 0; b < batch; ++b){
-// 	res = 0;
-//
-//     blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-//     __syncthreads();
-// 	for (k = 0; k <  BLOCKWIDTH; ++k){
-// 	  res += weight[k] * blockvec[k];
-//     }
-//     atomicAdd(&mul[b * width + w], res);
-//     __syncthreads();
-//   }
-// }
-
-void vecquant8matmul_cuda(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT8 - 1) / BLOCKHEIGHT8,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant8matmul_cuda", ([&] {
-      VecQuant8MatMulKernel<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
-        batch, vec_height, height, width, zero_width
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant8MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const       int* __restrict__ zeros,
-    const   	int* __restrict__ g_idx,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-	int zero_width
-) {
-  int h = BLOCKHEIGHT8 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-  
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  int i = width * h + w;
-  int g_h = h * 4;
-  int k;
-  unsigned int g;
-  scalar_t w_tmp;
-  
-  int z_w = w / 4; 
-  int z_mod = (w % 4) * 8;
-  
-  float weight[BLOCKWIDTH];
-  
-  for (k = 0; k <  BLOCKWIDTH; ++k){	
-	int k_w = (k / 4); 
-	int k_bit = (k % 4) * 8;
-	
-    g = as_int(g_idx[g_h + k]);
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xFF) + 1);
-	
-    w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0xFF);
-    
-	weight[k] = scale * (w_tmp - zero);
-  }
-
-  scalar_t res;
-  for (int b = 0; b < batch; ++b){	
-	res = 0;
-	
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-    __syncthreads();
-	for (k = 0; k <  BLOCKWIDTH; ++k){	
-	  res += weight[k] * blockvec[k];
-    }
-    atomicAdd(&mul[b * width + w], res);
-    __syncthreads();
-  }
-}
-
-
-void vecquant2matmul_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant2matmul_cuda_old", ([&] {
-      VecQuant2MatMulKernel_old<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(),
-        batch, vec_height, height, width, zero_width, groupsize
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant2MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT2 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-  __syncthreads();
-
-  scalar_t res = 0;
-  int i = width * h + w;
-  int g_h = h * 16;
-  int k = 0;
-  
-  int z_w = w / 16; 
-  int z_mod = (w % 16) * 2;
-
-  unsigned int tmp;
-
-  while (k < BLOCKWIDTH) {
-    tmp = as_unsigned(mat[i]);
-	
-    int g = (g_h + k) / groupsize;
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scale * scalar_t((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod & 0x3) + 1);
-	
-    res += (scale * scalar_t((tmp >> 0) & 0x3) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp >> 2) & 0x3) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp >> 4) & 0x3) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp >> 6) & 0x3) - zero) * blockvec[k + 3];
-    res += (scale * scalar_t((tmp >> 8) & 0x3) - zero) * blockvec[k + 4];
-    res += (scale * scalar_t((tmp >> 10) & 0x3) - zero) * blockvec[k + 5];
-    res += (scale * scalar_t((tmp >> 12) & 0x3) - zero) * blockvec[k + 6];
-    res += (scale * scalar_t((tmp >> 14) & 0x3) - zero) * blockvec[k + 7];
-    res += (scale * scalar_t((tmp >> 16) & 0x3) - zero) * blockvec[k + 8];
-    res += (scale * scalar_t((tmp >> 18) & 0x3) - zero) * blockvec[k + 9];
-    res += (scale * scalar_t((tmp >> 20) & 0x3) - zero) * blockvec[k + 10];
-    res += (scale * scalar_t((tmp >> 22) & 0x3) - zero) * blockvec[k + 11];
-    res += (scale * scalar_t((tmp >> 24) & 0x3) - zero) * blockvec[k + 12];
-    res += (scale * scalar_t((tmp >> 26) & 0x3) - zero) * blockvec[k + 13];
-    res += (scale * scalar_t((tmp >> 28) & 0x3) - zero) * blockvec[k + 14];
-    res += (scale * scalar_t((tmp >> 30) & 0x3) - zero) * blockvec[k + 15];
-	
-    i += width;
-    k += 16;
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-void vecquant3matmul_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant3matmul_cuda_old", ([&] {
-      VecQuant3MatMulKernel_old<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(),
-        batch, vec_height, height, width, zero_width, groupsize
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant3MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT3 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-  __syncthreads();
-
-  scalar_t res = 0;
-  int i = width * h + w;
-  int g_h = (h / 3) * 32;
-  int k = 0;
-  
-  int z_w = (w / 32) * 3; 
-  int z_mod = w % 32;
-  int z_bit;
-  
-  if (z_mod != 10){
-    if (z_mod != 21){
-      z_bit = z_mod;
-      if (z_bit > 21){
-        z_bit -= 22;
-        z_bit *= 3;
-        z_bit += 2;
-        z_w += 2;
-      } else if (z_bit > 10){
-        z_bit -= 11;
-        z_bit *= 3;
-        z_bit += 1;
-        z_w += 1;
-      } else {
-        z_bit *= 3;
-      }
-    } else {
-      z_w += 1;
-    }
-  }
- 
-  unsigned int tmp1;
-  unsigned int tmp2;
-  unsigned int tmp;
-  unsigned int z_tmp;
-
-  while (k < BLOCKWIDTH) {
-    tmp1 = as_unsigned(mat[i]);
-	
-    int g = (g_h + k) / groupsize;
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero;
-    if (z_mod == 10) {
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
-      zero = scale * scalar_t((z_tmp) + 1);
-    } else if (z_mod == 21){
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
-      zero = scale * scalar_t((z_tmp) + 1);
-    } else {
-      zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1);
-    }
-	
-    res += (scale * scalar_t((tmp1 >>  0) & 0x7) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp1 >>  3) & 0x7) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp1 >>  6) & 0x7) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp1 >>  9) & 0x7) - zero) * blockvec[k + 3];
-    res += (scale * scalar_t((tmp1 >> 12) & 0x7) - zero) * blockvec[k + 4];
-    res += (scale * scalar_t((tmp1 >> 15) & 0x7) - zero) * blockvec[k + 5];
-    res += (scale * scalar_t((tmp1 >> 18) & 0x7) - zero) * blockvec[k + 6];
-    res += (scale * scalar_t((tmp1 >> 21) & 0x7) - zero) * blockvec[k + 7];
-    res += (scale * scalar_t((tmp1 >> 24) & 0x7) - zero) * blockvec[k + 8];
-    res += (scale * scalar_t((tmp1 >> 27) & 0x7) - zero) * blockvec[k + 9];
-	
-    i += width;
-    tmp2 = as_unsigned(mat[i]);
-    tmp = (tmp1 >> 30) | ((tmp2 << 2) & 0x4);
-    tmp2 >>= 1;
-    res += (scale * scalar_t(tmp) - zero) * blockvec[k + 10];
-    k += 11;
-	
-    res += (scale * scalar_t((tmp2 >>  0) & 0x7) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp2 >>  3) & 0x7) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp2 >>  6) & 0x7) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp2 >>  9) & 0x7) - zero) * blockvec[k + 3];
-    res += (scale * scalar_t((tmp2 >> 12) & 0x7) - zero) * blockvec[k + 4];
-    res += (scale * scalar_t((tmp2 >> 15) & 0x7) - zero) * blockvec[k + 5];
-    res += (scale * scalar_t((tmp2 >> 18) & 0x7) - zero) * blockvec[k + 6];
-    res += (scale * scalar_t((tmp2 >> 21) & 0x7) - zero) * blockvec[k + 7];
-    res += (scale * scalar_t((tmp2 >> 24) & 0x7) - zero) * blockvec[k + 8];
-    res += (scale * scalar_t((tmp2 >> 27) & 0x7) - zero) * blockvec[k + 9];
-	
-    i += width;
-    tmp1 = as_unsigned(mat[i]);
-    tmp = (tmp2 >> 30) | ((tmp1 << 1) & 0x6);
-    tmp1 >>= 2;
-    res += (scale * scalar_t(tmp) - zero) * blockvec[k + 10];
-    k += 11;
-	
-    res += (scale * scalar_t((tmp1 >>  0) & 0x7) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp1 >>  3) & 0x7) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp1 >>  6) & 0x7) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp1 >>  9) & 0x7) - zero) * blockvec[k + 3];
-    res += (scale * scalar_t((tmp1 >> 12) & 0x7) - zero) * blockvec[k + 4];
-    res += (scale * scalar_t((tmp1 >> 15) & 0x7) - zero) * blockvec[k + 5];
-    res += (scale * scalar_t((tmp1 >> 18) & 0x7) - zero) * blockvec[k + 6];
-    res += (scale * scalar_t((tmp1 >> 21) & 0x7) - zero) * blockvec[k + 7];
-    res += (scale * scalar_t((tmp1 >> 24) & 0x7) - zero) * blockvec[k + 8];
-    res += (scale * scalar_t((tmp1 >> 27) & 0x7) - zero) * blockvec[k + 9];
-	
-    i += width;
-    k += 10;
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-void vecquant4matmul_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant4matmul_cuda_old", ([&] {
-      VecQuant4MatMulKernel_old<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(),
-        batch, vec_height, height, width, zero_width, groupsize
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant4MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const       int* __restrict__ zeros,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT4 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-  __syncthreads();
-
-  scalar_t res = 0;
-  int i = width * h + w;
-  int g_h = h * 8;
-  int k = 0;
-
-  int z_w = w / 8; 
-  int z_mod = (w % 8) * 4;
-
-  unsigned int tmp;
-
-  while (k < BLOCKWIDTH) {
-    tmp = as_unsigned(mat[i]);
-	
-    int g = (g_h + k) / groupsize;
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1);
-	
-    res += (scale * scalar_t((tmp >> 0) & 0xF) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp >> 4) & 0xF) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp >> 8) & 0xF) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp >> 12) & 0xF) - zero) * blockvec[k + 3];
-    res += (scale * scalar_t((tmp >> 16) & 0xF) - zero) * blockvec[k + 4];
-    res += (scale * scalar_t((tmp >> 20) & 0xF) - zero) * blockvec[k + 5];
-    res += (scale * scalar_t((tmp >> 24) & 0xF) - zero) * blockvec[k + 6];
-    res += (scale * scalar_t((tmp >> 28) & 0xF) - zero) * blockvec[k + 7];
-	
-    i += width;
-    k += 8;
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-void vecquant8matmul_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT8 - 1) / BLOCKHEIGHT8,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant8matmul_cuda_old", ([&] {
-      VecQuant8MatMulKernel_old<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(),
-        batch, vec_height, height, width, zero_width, groupsize
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant8MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT8 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-  __syncthreads();
-
-  scalar_t res = 0;
-  int i = width * h + w;
-  int g_h = h * 4;
-  int k = 0;
-  
-  int z_w = w / 4; 
-  int z_mod = (w % 4) * 8;
-
-  unsigned int tmp;
-
-  while (k < BLOCKWIDTH) { 
-    tmp = as_unsigned(mat[i]);
-	
-    int g = (g_h + k) / groupsize;
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xFF) + 1);
-	
-    res += (scale * scalar_t((tmp >> 0) & 0xFF) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp >> 8) & 0xFF) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp >> 16) & 0xFF) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp >> 24) & 0xFF) - zero) * blockvec[k + 3];
-	
-    i += width;
-    k += 4;
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-
-void vecquant2matmul_faster_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize,
-  int vec_height
-) {
-  int batch = vec.size(0);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-  
-  dim3 blocks(
-    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  VecQuant2MatMulKernelFaster_old<<<blocks, threads>>>(
-    (half2*) vec.data_ptr(),
-    mat.data_ptr<int>(),
-    mul.data_ptr<float>(),
-    scales.data_ptr<float>(),
-    zeros.data_ptr<int>(),
-    batch, vec_height, height, width, zero_width, groupsize
-  );
-}
-
-__global__ void VecQuant2MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const  	 int* __restrict__ zeros,
-	int batch,
-	int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  const int blockwidth2 = BLOCKWIDTH / 2;
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT2 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ half2 blockvec[blockwidth2];
-  if (threadIdx.x < blockwidth2)
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
-
-  __shared__ half2 deq2[16][16];
-  int val = threadIdx.x / 16;
-  int off = threadIdx.x % 16;
-  for (; val < 16; val += BLOCKWIDTH / 16) {
-    deq2[val][off] = __halves2half2(
-       __int2half_rn(val & 0x3), __int2half_rn(val >> 2)
-    );
-  }
-
-  int i = width * h + w;
-  int g_h = h * 16;
-  int k = 0;
-  
-  int z_w = w / 16; 
-  int z_mod = (w % 16) * 2;
-
-  float res = 0;
-  half2 res2;
-
-  unsigned int tmp;
-
-  __syncthreads();
-
-  while (k < blockwidth2) {
-    int g = (g_h + (k * 2)) / groupsize;
-	float scale_f = scales[g * width + w];
-    half2 scale = __float2half2_rn(scale_f);
-    half2 zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0x3) + 1)));
-	
-    res2 = {};
-    tmp = as_unsigned(mat[i]);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  0) & 0xf][off], scale, zero), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  4) & 0xf][off], scale, zero), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  8) & 0xf][off], scale, zero), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 12) & 0xf][off], scale, zero), blockvec[k + 3], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 16) & 0xf][off], scale, zero), blockvec[k + 4], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 20) & 0xf][off], scale, zero), blockvec[k + 5], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 24) & 0xf][off], scale, zero), blockvec[k + 6], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 28) & 0xf][off], scale, zero), blockvec[k + 7], res2);
-	i += width;
-    k += 8;
-    res += __half2float(res2.x) + __half2float(res2.y);
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-void vecquant3matmul_faster_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize,
-  int vec_height
-) {
-  int batch = vec.size(0);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-  
-  dim3 blocks(
-    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  VecQuant3MatMulKernelFaster_old<<<blocks, threads>>>(
-    (half2*) vec.data_ptr(),
-    mat.data_ptr<int>(),
-    mul.data_ptr<float>(),
-    scales.data_ptr<float>(),
-    zeros.data_ptr<int>(),
-    batch, vec_height, height, width, zero_width, groupsize
-  );
-}
-
-__global__ void VecQuant3MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const  	 int* __restrict__ zeros,
-	int batch,
-	int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  const int blockwidth2 = BLOCKWIDTH / 2;
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT3 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ half2 blockvec[blockwidth2];
-  if (threadIdx.x < blockwidth2)
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
-
-  __shared__ half2 deq2[64][32];
-  int val = threadIdx.x / 32;
-  int off = threadIdx.x % 32;
-  for (; val < 64; val += BLOCKWIDTH / 32) {
-    deq2[val][off] = __halves2half2(
-       __int2half_rn(val & 0x7), __int2half_rn(val >> 3)
-    );
-  }
-
-  int i = width * h + w;
-  int g_h = (h / 3) * 32;
-  int k = 0;
-  
-  int z_w = (w / 32) * 3;
-  int z_mod = w % 32;
-  int z_bit;
-  
-  if (z_mod != 10){
-    if (z_mod != 21){
-      z_bit = z_mod;
-      if (z_bit > 21){
-        z_bit -= 22;
-        z_bit *= 3;
-        z_bit += 2;
-        z_w += 2;
-      } else if (z_bit > 10){
-        z_bit -= 11;
-        z_bit *= 3;
-        z_bit += 1;
-        z_w += 1;
-      } else {
-        z_bit *= 3;
-      }
-    } else {
-      z_w += 1;
-    }
-  }
-
-  float res = 0;
-  half2 res2;
-
-  unsigned int tmp1;
-  unsigned int tmp2;
-  unsigned int tmp;
-  unsigned int z_tmp;
-
-  __syncthreads();
-
-  while (k < blockwidth2) {
-    int g = (g_h + (k * 2)) / groupsize;
-	float scale_f = scales[g * width + w];
-    half2 scale = __float2half2_rn(scale_f);
-    half2 zero;
-    if (z_mod == 10) {
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
-      zero = __float2half2_rn(-(scale_f * ((z_tmp) + 1)));
-    } else if (z_mod == 21){
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
-      zero = __float2half2_rn(-(scale_f * ((z_tmp) + 1)));
-    } else {
-      zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1)));
-    }
-	
-    res2 = {};
-    tmp1 = as_unsigned(mat[i]);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 24) & 0x3f][off], scale, zero), blockvec[k + 4], res2);
-    i += width;
-    tmp2 = as_unsigned(mat[i]);
-    tmp = (tmp1 >> 30) | ((tmp2 << 2) & 0x3c);
-    res2 = __hfma2(__hfma2(deq2[tmp][off], scale, zero), blockvec[k + 5], res2);
-    tmp2 >>= 4;
-    k += 6;
-    res2 = __hfma2(__hfma2(deq2[(tmp2 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp2 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp2 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp2 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
-    i += width;
-    tmp1 = as_unsigned(mat[i]);
-    tmp = (tmp2 >> 24) | ((tmp1 << 4) & 0x30);
-    res2 = __hfma2(__hfma2(deq2[tmp][off], scale, zero), blockvec[k + 4], res2);
-    tmp1 >>= 2;
-    k += 5;
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 24) & 0x3f][off], scale, zero), blockvec[k + 4], res2);
-    i += width;
-    k += 5;
-    res += __half2float(res2.x) + __half2float(res2.y);
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-void vecquant4matmul_faster_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize,
-  int vec_height
-) {
-  int batch = vec.size(0);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-  
-  dim3 blocks(
-    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  VecQuant4MatMulKernelFaster_old<<<blocks, threads>>>(
-    (half2*) vec.data_ptr(),
-    mat.data_ptr<int>(),
-    mul.data_ptr<float>(),
-    scales.data_ptr<float>(),
-    zeros.data_ptr<int>(),
-    batch, vec_height, height, width, zero_width, groupsize
-  );
-}
-
-__global__ void VecQuant4MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const  	 int* __restrict__ zeros,
-	int batch,
-	int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  const int blockwidth2 = BLOCKWIDTH / 2;
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT4 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ half2 blockvec[blockwidth2];
-  if (threadIdx.x < blockwidth2)
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
-
-  __shared__ half2 deq2[256][8];
-  int val = threadIdx.x / 8;
-  int off = threadIdx.x % 8;
-  for (; val < 256; val += BLOCKWIDTH / 8) {
-    deq2[val][off] = __halves2half2(
-       __int2half_rn(val & 0xF), __int2half_rn(val >> 4)
-    );
-  }
-
-  int i = width * h + w;
-  int g_h = h * 8;
-  int k = 0;
-
-  int z_w = w / 8; 
-  int z_mod = (w % 8) * 4;
-
-  float res = 0;
-  half2 res2;
-
-  unsigned int tmp;
-
-  __syncthreads();
-
-  while (k < blockwidth2) {
-    int g = (g_h + (k * 2)) / groupsize;
-	float scale_f = scales[g * width + w];
-    half2 scale = __float2half2_rn(scale_f);
-    half2 zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1)));
-	
-    res2 = {};
-    tmp = as_unsigned(mat[i]);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  0) & 0xff][off], scale, zero), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  8) & 0xff][off], scale, zero), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 16) & 0xff][off], scale, zero), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 24) & 0xff][off], scale, zero), blockvec[k + 3], res2);
-	i += width;
-    k += 4;
-    res += __half2float(res2.x) + __half2float(res2.y);
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
+#include <torch/all.h>
+#include <torch/python.h>
+#include <cuda.h>
+#include <cuda_runtime.h>
+#include <cuda_fp16.h>
+
+// atomicAdd for double-precision floating-point numbers on hardware with
+// compute capability < 6.0 from:
+// https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#atomic-functions
+// #if defined(__CUDA_ARCH__) && __CUDA_ARCH__ < 600
+// __device__ double atomicAdd(
+//     double* address,
+//     double val
+// ) {
+//   unsigned long long int* address_as_ull = (unsigned long long int*)address;
+//   unsigned long long int old = *address_as_ull, assumed;
+//
+//   do {
+//     assumed = old;
+//     old = atomicCAS(
+//       address_as_ull,
+//       assumed,
+//       __double_as_longlong(val + __longlong_as_double(assumed))
+//     );
+//
+//   // Note: uses integer comparison to avoid hang in case of NaN (since NaN != NaN)
+//   } while (assumed != old);
+//
+//   return __longlong_as_double(old);
+// }
+// #endif
+
+#if defined(__CUDA_ARCH__) && __CUDA_ARCH__ < 700
+// adapted from https://github.com/torch/cutorch/blob/master/lib/THC/THCAtomics.cuh
+__device__ __forceinline__ void atomicAdd(c10::Half* address, c10::Half val) {
+    unsigned int *address_as_ui = reinterpret_cast<unsigned int *>(reinterpret_cast<char *>(address) - (reinterpret_cast<size_t>(address) & 2));
+    unsigned int old = *address_as_ui;
+    unsigned int assumed;
+
+    do {
+        assumed = old;
+        unsigned short hsum = reinterpret_cast<size_t>(address) & 2 ? (old >> 16) : (old & 0xffff);
+        hsum += val;
+        old = reinterpret_cast<size_t>(address) & 2
+                 ? (old & 0xffff) | (hsum << 16)
+                 : (old & 0xffff0000) | hsum;
+        old = atomicCAS(address_as_ui, assumed, old);
+
+    // Note: uses integer comparison to avoid hang in case of NaN (since NaN != NaN)
+    } while (assumed != old);
+}
+__device__ __forceinline__ void atomicAdd(__half* address, c10::Half val) {
+    unsigned int * address_as_ui = (unsigned int *) ((char *)address - ((size_t)address & 2));
+    unsigned int old = *address_as_ui;
+    unsigned int assumed;
+
+    do {
+        assumed = old;
+        __half_raw hsum;
+        hsum.x = (size_t)address & 2 ? (old >> 16) : (old & 0xffff);
+        half tmpres = __hadd(hsum, val);
+        hsum = __half_raw(tmpres);
+        old = (size_t)address & 2 ? (old & 0xffff) | (hsum.x << 16) : (old & 0xffff0000) | hsum.x;
+        old = atomicCAS(address_as_ui, assumed, old);
+    } while (assumed != old);
+}
+#endif
+
+
+template <typename scalar_t>
+__global__ void VecQuant2MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+	const  	    int* __restrict__ g_idx,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+	int zero_width
+);
+
+template <typename scalar_t>
+__global__ void VecQuant3MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+	const  	    int* __restrict__ g_idx,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+	int zero_width
+);
+
+template <typename scalar_t>
+__global__ void VecQuant4MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+	const  	    int* __restrict__ g_idx,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+	int zero_width
+);
+
+template <typename scalar_t>
+__global__ void VecQuant8MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+	const  	    int* __restrict__ g_idx,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+	int zero_width
+);
+
+template <typename scalar_t>
+__global__ void VecQuant2MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+template <typename scalar_t>
+__global__ void VecQuant3MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+template <typename scalar_t>
+__global__ void VecQuant4MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+template <typename scalar_t>
+__global__ void VecQuant8MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+__global__ void VecQuant2MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const    int* __restrict__ zeros,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+__global__ void VecQuant3MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const    int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+__global__ void VecQuant4MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const    int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+
+const int BLOCKWIDTH  = 256;
+const int BLOCKHEIGHT2 =  16;
+const int BLOCKHEIGHT3 =  24;
+const int BLOCKHEIGHT4 =  32;
+const int BLOCKHEIGHT8 =  64;
+
+__device__ inline unsigned int as_unsigned(int i) {
+  return *reinterpret_cast<unsigned int*>(&i);
+}
+
+__device__ inline int as_int(int i) {
+  return *reinterpret_cast<int*>(&i);
+}
+
+
+void vecquant2matmul_cuda(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant2matmul_cuda", ([&] {
+      VecQuant2MatMulKernel<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
+        batch, vec_height, height, width, zero_width
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant2MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+    const   	int* __restrict__ g_idx,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+	int zero_width
+) {
+  int h = BLOCKHEIGHT2 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+  
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  int i = width * h + w;
+  int g_h = h * 16;
+  int k;
+  unsigned int g;
+  scalar_t w_tmp;
+  
+  int z_w = w / 16; 
+  int z_mod = (w % 16) * 2;
+  
+  float weight[BLOCKWIDTH];
+  
+  for (k = 0; k <  BLOCKWIDTH; ++k){	
+	int k_w = (k / 16); 
+	int k_bit = (k % 16) * 2;
+	
+    g = as_int(g_idx[g_h + k]);
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scalar_t((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod & 0x3) + 1);
+	
+    w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0x3);
+    
+	weight[k] = scale * (w_tmp - zero);
+  }
+
+  scalar_t res;
+  for (int b = 0; b < batch; ++b){	
+	res = 0;
+	
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+    __syncthreads();
+	for (k = 0; k <  BLOCKWIDTH; ++k){	
+	  res += weight[k] * blockvec[k];
+    }
+    atomicAdd(&mul[b * width + w], res);
+    __syncthreads();
+  }
+}
+
+void vecquant3matmul_cuda(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant3matmul_cuda", ([&] {
+      VecQuant3MatMulKernel<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
+        batch, vec_height, height, width, zero_width
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant3MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const       int* __restrict__ zeros,
+    const   	int* __restrict__ g_idx,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+	int zero_width
+) {
+  int h = BLOCKHEIGHT3 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+  
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  int i = width * h + w;
+  int g_h = (h / 3) * 32;
+  int k;
+  unsigned int g;
+  scalar_t w_tmp;
+  
+  int z_w = (w / 32) * 3; 
+  int z_mod = w % 32;
+  int z_bit;
+  unsigned int z_tmp;
+  if (z_mod != 10){
+    if (z_mod != 21){
+      z_bit = z_mod;
+      if (z_bit > 21){
+        z_bit -= 22;
+        z_bit *= 3;
+        z_bit += 2;
+        z_w += 2;
+      } else if (z_bit > 10){
+        z_bit -= 11;
+        z_bit *= 3;
+        z_bit += 1;
+        z_w += 1;
+      } else {
+        z_bit *= 3;
+      }
+    } else {
+      z_w += 1;
+    }
+  }
+  
+  float weight[BLOCKWIDTH];
+  
+  for (k = 0; k <  BLOCKWIDTH; ++k){	
+	int k_w = (k / 32) * 3; 
+	int k_mod = k % 32;
+	int k_bit;
+	  
+	if (k_mod != 10){
+	  if (k_mod != 21){
+        k_bit = k_mod;
+        if (k_bit > 21){
+		  k_bit -= 22;
+		  k_bit *= 3;
+		  k_bit += 2;
+		  k_w += 2;
+        } else if (k_bit > 10){
+		  k_bit -= 11;
+		  k_bit *= 3;
+		  k_bit += 1;
+		  k_w += 1;
+        } else {
+		  k_bit *= 3;
+        }
+	  } else {
+        k_w += 1;
+	  }
+	}
+	
+    g = as_int(g_idx[g_h + k]);
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero;
+    if (z_mod == 10) {
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
+      zero = scalar_t((z_tmp) + 1);
+    } else if (z_mod == 21){
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
+      zero = scalar_t((z_tmp) + 1);
+    } else {
+      zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1);
+    }
+	
+    if (k_mod == 10) {
+      w_tmp = (as_unsigned(mat[i + (k_w * width)]) >> 30) | ((as_unsigned(mat[i + ((k_w + 1)* width)]) << 2) & 0x4);
+    } else if (k_mod == 21){
+      w_tmp = (as_unsigned(mat[i + (k_w * width)]) >> 31) | ((as_unsigned(mat[i + ((k_w + 1)* width)]) << 1) & 0x6);
+    } else {
+      w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0x7);
+    }
+	weight[k] = scale * (w_tmp - zero);
+  }
+
+  scalar_t res;
+  for (int b = 0; b < batch; ++b){	
+	res = 0;
+	
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+    __syncthreads();
+	for (k = 0; k <  BLOCKWIDTH; ++k){	
+	  res += weight[k] * blockvec[k];
+    }
+    atomicAdd(&mul[b * width + w], res);
+    __syncthreads();
+  }
+}
+
+void vecquant4matmul_cuda(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant4matmul_cuda", ([&] {
+      VecQuant4MatMulKernel<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
+        batch, vec_height, height, width, zero_width
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant4MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const       int* __restrict__ zeros,
+    const   	int* __restrict__ g_idx,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+	int zero_width
+) {
+  int h = BLOCKHEIGHT4 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+  
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  int i = width * h + w;
+  int g_h = h * 8;
+  int k;
+  unsigned int g;
+  scalar_t w_tmp;
+  
+
+  int z_w = w / 8; 
+  int z_mod = (w % 8) * 4;
+  
+  float weight[BLOCKWIDTH];
+  
+  for (k = 0; k <  BLOCKWIDTH; ++k){	
+	int k_w = (k / 8); 
+	int k_bit = (k % 8) * 4;
+	
+    g = as_int(g_idx[g_h + k]);
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1);
+	
+    w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0xF);
+    
+	weight[k] = scale * (w_tmp - zero);
+  }
+
+  scalar_t res;
+  for (int b = 0; b < batch; ++b){	
+	res = 0;
+	
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+    __syncthreads();
+	for (k = 0; k <  BLOCKWIDTH; ++k){	
+	  res += weight[k] * blockvec[k];
+    }
+    atomicAdd(&mul[b * width + w], res);
+    __syncthreads();
+  }
+}
+
+void vecquant8matmul_cuda(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT8 - 1) / BLOCKHEIGHT8,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant8matmul_cuda", ([&] {
+      VecQuant8MatMulKernel<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
+        batch, vec_height, height, width, zero_width
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant8MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const       int* __restrict__ zeros,
+    const   	int* __restrict__ g_idx,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+	int zero_width
+) {
+  int h = BLOCKHEIGHT8 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+  
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  int i = width * h + w;
+  int g_h = h * 4;
+  int k;
+  unsigned int g;
+  scalar_t w_tmp;
+  
+  int z_w = w / 4; 
+  int z_mod = (w % 4) * 8;
+  
+  float weight[BLOCKWIDTH];
+  
+  for (k = 0; k <  BLOCKWIDTH; ++k){	
+	int k_w = (k / 4); 
+	int k_bit = (k % 4) * 8;
+	
+    g = as_int(g_idx[g_h + k]);
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xFF) + 1);
+	
+    w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0xFF);
+    
+	weight[k] = scale * (w_tmp - zero);
+  }
+
+  scalar_t res;
+  for (int b = 0; b < batch; ++b){	
+	res = 0;
+	
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+    __syncthreads();
+	for (k = 0; k <  BLOCKWIDTH; ++k){	
+	  res += weight[k] * blockvec[k];
+    }
+    atomicAdd(&mul[b * width + w], res);
+    __syncthreads();
+  }
+}
+
+
+void vecquant2matmul_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant2matmul_cuda_old", ([&] {
+      VecQuant2MatMulKernel_old<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(),
+        batch, vec_height, height, width, zero_width, groupsize
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant2MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT2 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+  __syncthreads();
+
+  scalar_t res = 0;
+  int i = width * h + w;
+  int g_h = h * 16;
+  int k = 0;
+  
+  int z_w = w / 16; 
+  int z_mod = (w % 16) * 2;
+
+  unsigned int tmp;
+
+  while (k < BLOCKWIDTH) {
+    tmp = as_unsigned(mat[i]);
+	
+    int g = (g_h + k) / groupsize;
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scale * scalar_t((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod & 0x3) + 1);
+	
+    res += (scale * scalar_t((tmp >> 0) & 0x3) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp >> 2) & 0x3) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp >> 4) & 0x3) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp >> 6) & 0x3) - zero) * blockvec[k + 3];
+    res += (scale * scalar_t((tmp >> 8) & 0x3) - zero) * blockvec[k + 4];
+    res += (scale * scalar_t((tmp >> 10) & 0x3) - zero) * blockvec[k + 5];
+    res += (scale * scalar_t((tmp >> 12) & 0x3) - zero) * blockvec[k + 6];
+    res += (scale * scalar_t((tmp >> 14) & 0x3) - zero) * blockvec[k + 7];
+    res += (scale * scalar_t((tmp >> 16) & 0x3) - zero) * blockvec[k + 8];
+    res += (scale * scalar_t((tmp >> 18) & 0x3) - zero) * blockvec[k + 9];
+    res += (scale * scalar_t((tmp >> 20) & 0x3) - zero) * blockvec[k + 10];
+    res += (scale * scalar_t((tmp >> 22) & 0x3) - zero) * blockvec[k + 11];
+    res += (scale * scalar_t((tmp >> 24) & 0x3) - zero) * blockvec[k + 12];
+    res += (scale * scalar_t((tmp >> 26) & 0x3) - zero) * blockvec[k + 13];
+    res += (scale * scalar_t((tmp >> 28) & 0x3) - zero) * blockvec[k + 14];
+    res += (scale * scalar_t((tmp >> 30) & 0x3) - zero) * blockvec[k + 15];
+	
+    i += width;
+    k += 16;
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+void vecquant3matmul_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant3matmul_cuda_old", ([&] {
+      VecQuant3MatMulKernel_old<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(),
+        batch, vec_height, height, width, zero_width, groupsize
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant3MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT3 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+  __syncthreads();
+
+  scalar_t res = 0;
+  int i = width * h + w;
+  int g_h = (h / 3) * 32;
+  int k = 0;
+  
+  int z_w = (w / 32) * 3; 
+  int z_mod = w % 32;
+  int z_bit;
+  
+  if (z_mod != 10){
+    if (z_mod != 21){
+      z_bit = z_mod;
+      if (z_bit > 21){
+        z_bit -= 22;
+        z_bit *= 3;
+        z_bit += 2;
+        z_w += 2;
+      } else if (z_bit > 10){
+        z_bit -= 11;
+        z_bit *= 3;
+        z_bit += 1;
+        z_w += 1;
+      } else {
+        z_bit *= 3;
+      }
+    } else {
+      z_w += 1;
+    }
+  }
+ 
+  unsigned int tmp1;
+  unsigned int tmp2;
+  unsigned int tmp;
+  unsigned int z_tmp;
+
+  while (k < BLOCKWIDTH) {
+    tmp1 = as_unsigned(mat[i]);
+	
+    int g = (g_h + k) / groupsize;
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero;
+    if (z_mod == 10) {
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
+      zero = scale * scalar_t((z_tmp) + 1);
+    } else if (z_mod == 21){
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
+      zero = scale * scalar_t((z_tmp) + 1);
+    } else {
+      zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1);
+    }
+	
+    res += (scale * scalar_t((tmp1 >>  0) & 0x7) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp1 >>  3) & 0x7) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp1 >>  6) & 0x7) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp1 >>  9) & 0x7) - zero) * blockvec[k + 3];
+    res += (scale * scalar_t((tmp1 >> 12) & 0x7) - zero) * blockvec[k + 4];
+    res += (scale * scalar_t((tmp1 >> 15) & 0x7) - zero) * blockvec[k + 5];
+    res += (scale * scalar_t((tmp1 >> 18) & 0x7) - zero) * blockvec[k + 6];
+    res += (scale * scalar_t((tmp1 >> 21) & 0x7) - zero) * blockvec[k + 7];
+    res += (scale * scalar_t((tmp1 >> 24) & 0x7) - zero) * blockvec[k + 8];
+    res += (scale * scalar_t((tmp1 >> 27) & 0x7) - zero) * blockvec[k + 9];
+	
+    i += width;
+    tmp2 = as_unsigned(mat[i]);
+    tmp = (tmp1 >> 30) | ((tmp2 << 2) & 0x4);
+    tmp2 >>= 1;
+    res += (scale * scalar_t(tmp) - zero) * blockvec[k + 10];
+    k += 11;
+	
+    res += (scale * scalar_t((tmp2 >>  0) & 0x7) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp2 >>  3) & 0x7) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp2 >>  6) & 0x7) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp2 >>  9) & 0x7) - zero) * blockvec[k + 3];
+    res += (scale * scalar_t((tmp2 >> 12) & 0x7) - zero) * blockvec[k + 4];
+    res += (scale * scalar_t((tmp2 >> 15) & 0x7) - zero) * blockvec[k + 5];
+    res += (scale * scalar_t((tmp2 >> 18) & 0x7) - zero) * blockvec[k + 6];
+    res += (scale * scalar_t((tmp2 >> 21) & 0x7) - zero) * blockvec[k + 7];
+    res += (scale * scalar_t((tmp2 >> 24) & 0x7) - zero) * blockvec[k + 8];
+    res += (scale * scalar_t((tmp2 >> 27) & 0x7) - zero) * blockvec[k + 9];
+	
+    i += width;
+    tmp1 = as_unsigned(mat[i]);
+    tmp = (tmp2 >> 30) | ((tmp1 << 1) & 0x6);
+    tmp1 >>= 2;
+    res += (scale * scalar_t(tmp) - zero) * blockvec[k + 10];
+    k += 11;
+	
+    res += (scale * scalar_t((tmp1 >>  0) & 0x7) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp1 >>  3) & 0x7) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp1 >>  6) & 0x7) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp1 >>  9) & 0x7) - zero) * blockvec[k + 3];
+    res += (scale * scalar_t((tmp1 >> 12) & 0x7) - zero) * blockvec[k + 4];
+    res += (scale * scalar_t((tmp1 >> 15) & 0x7) - zero) * blockvec[k + 5];
+    res += (scale * scalar_t((tmp1 >> 18) & 0x7) - zero) * blockvec[k + 6];
+    res += (scale * scalar_t((tmp1 >> 21) & 0x7) - zero) * blockvec[k + 7];
+    res += (scale * scalar_t((tmp1 >> 24) & 0x7) - zero) * blockvec[k + 8];
+    res += (scale * scalar_t((tmp1 >> 27) & 0x7) - zero) * blockvec[k + 9];
+	
+    i += width;
+    k += 10;
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+void vecquant4matmul_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant4matmul_cuda_old", ([&] {
+      VecQuant4MatMulKernel_old<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(),
+        batch, vec_height, height, width, zero_width, groupsize
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant4MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const       int* __restrict__ zeros,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT4 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+  __syncthreads();
+
+  scalar_t res = 0;
+  int i = width * h + w;
+  int g_h = h * 8;
+  int k = 0;
+
+  int z_w = w / 8; 
+  int z_mod = (w % 8) * 4;
+
+  unsigned int tmp;
+
+  while (k < BLOCKWIDTH) {
+    tmp = as_unsigned(mat[i]);
+	
+    int g = (g_h + k) / groupsize;
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1);
+	
+    res += (scale * scalar_t((tmp >> 0) & 0xF) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp >> 4) & 0xF) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp >> 8) & 0xF) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp >> 12) & 0xF) - zero) * blockvec[k + 3];
+    res += (scale * scalar_t((tmp >> 16) & 0xF) - zero) * blockvec[k + 4];
+    res += (scale * scalar_t((tmp >> 20) & 0xF) - zero) * blockvec[k + 5];
+    res += (scale * scalar_t((tmp >> 24) & 0xF) - zero) * blockvec[k + 6];
+    res += (scale * scalar_t((tmp >> 28) & 0xF) - zero) * blockvec[k + 7];
+	
+    i += width;
+    k += 8;
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+void vecquant8matmul_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT8 - 1) / BLOCKHEIGHT8,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant8matmul_cuda_old", ([&] {
+      VecQuant8MatMulKernel_old<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(),
+        batch, vec_height, height, width, zero_width, groupsize
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant8MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT8 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+  __syncthreads();
+
+  scalar_t res = 0;
+  int i = width * h + w;
+  int g_h = h * 4;
+  int k = 0;
+  
+  int z_w = w / 4; 
+  int z_mod = (w % 4) * 8;
+
+  unsigned int tmp;
+
+  while (k < BLOCKWIDTH) { 
+    tmp = as_unsigned(mat[i]);
+	
+    int g = (g_h + k) / groupsize;
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xFF) + 1);
+	
+    res += (scale * scalar_t((tmp >> 0) & 0xFF) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp >> 8) & 0xFF) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp >> 16) & 0xFF) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp >> 24) & 0xFF) - zero) * blockvec[k + 3];
+	
+    i += width;
+    k += 4;
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+
+void vecquant2matmul_faster_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize,
+  int vec_height
+) {
+  int batch = vec.size(0);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+  
+  dim3 blocks(
+    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  VecQuant2MatMulKernelFaster_old<<<blocks, threads>>>(
+    (half2*) vec.data_ptr(),
+    mat.data_ptr<int>(),
+    mul.data_ptr<float>(),
+    scales.data_ptr<float>(),
+    zeros.data_ptr<int>(),
+    batch, vec_height, height, width, zero_width, groupsize
+  );
+}
+
+__global__ void VecQuant2MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const  	 int* __restrict__ zeros,
+	int batch,
+	int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  const int blockwidth2 = BLOCKWIDTH / 2;
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT2 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ half2 blockvec[blockwidth2];
+  if (threadIdx.x < blockwidth2)
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
+
+  __shared__ half2 deq2[16][16];
+  int val = threadIdx.x / 16;
+  int off = threadIdx.x % 16;
+  for (; val < 16; val += BLOCKWIDTH / 16) {
+    deq2[val][off] = __halves2half2(
+       __int2half_rn(val & 0x3), __int2half_rn(val >> 2)
+    );
+  }
+
+  int i = width * h + w;
+  int g_h = h * 16;
+  int k = 0;
+  
+  int z_w = w / 16; 
+  int z_mod = (w % 16) * 2;
+
+  float res = 0;
+  half2 res2;
+
+  unsigned int tmp;
+
+  __syncthreads();
+
+  while (k < blockwidth2) {
+    int g = (g_h + (k * 2)) / groupsize;
+	float scale_f = scales[g * width + w];
+    half2 scale = __float2half2_rn(scale_f);
+    half2 zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0x3) + 1)));
+	
+    res2 = {};
+    tmp = as_unsigned(mat[i]);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  0) & 0xf][off], scale, zero), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  4) & 0xf][off], scale, zero), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  8) & 0xf][off], scale, zero), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 12) & 0xf][off], scale, zero), blockvec[k + 3], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 16) & 0xf][off], scale, zero), blockvec[k + 4], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 20) & 0xf][off], scale, zero), blockvec[k + 5], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 24) & 0xf][off], scale, zero), blockvec[k + 6], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 28) & 0xf][off], scale, zero), blockvec[k + 7], res2);
+	i += width;
+    k += 8;
+    res += __half2float(res2.x) + __half2float(res2.y);
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+void vecquant3matmul_faster_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize,
+  int vec_height
+) {
+  int batch = vec.size(0);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+  
+  dim3 blocks(
+    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  VecQuant3MatMulKernelFaster_old<<<blocks, threads>>>(
+    (half2*) vec.data_ptr(),
+    mat.data_ptr<int>(),
+    mul.data_ptr<float>(),
+    scales.data_ptr<float>(),
+    zeros.data_ptr<int>(),
+    batch, vec_height, height, width, zero_width, groupsize
+  );
+}
+
+__global__ void VecQuant3MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const  	 int* __restrict__ zeros,
+	int batch,
+	int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  const int blockwidth2 = BLOCKWIDTH / 2;
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT3 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ half2 blockvec[blockwidth2];
+  if (threadIdx.x < blockwidth2)
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
+
+  __shared__ half2 deq2[64][32];
+  int val = threadIdx.x / 32;
+  int off = threadIdx.x % 32;
+  for (; val < 64; val += BLOCKWIDTH / 32) {
+    deq2[val][off] = __halves2half2(
+       __int2half_rn(val & 0x7), __int2half_rn(val >> 3)
+    );
+  }
+
+  int i = width * h + w;
+  int g_h = (h / 3) * 32;
+  int k = 0;
+  
+  int z_w = (w / 32) * 3;
+  int z_mod = w % 32;
+  int z_bit;
+  
+  if (z_mod != 10){
+    if (z_mod != 21){
+      z_bit = z_mod;
+      if (z_bit > 21){
+        z_bit -= 22;
+        z_bit *= 3;
+        z_bit += 2;
+        z_w += 2;
+      } else if (z_bit > 10){
+        z_bit -= 11;
+        z_bit *= 3;
+        z_bit += 1;
+        z_w += 1;
+      } else {
+        z_bit *= 3;
+      }
+    } else {
+      z_w += 1;
+    }
+  }
+
+  float res = 0;
+  half2 res2;
+
+  unsigned int tmp1;
+  unsigned int tmp2;
+  unsigned int tmp;
+  unsigned int z_tmp;
+
+  __syncthreads();
+
+  while (k < blockwidth2) {
+    int g = (g_h + (k * 2)) / groupsize;
+	float scale_f = scales[g * width + w];
+    half2 scale = __float2half2_rn(scale_f);
+    half2 zero;
+    if (z_mod == 10) {
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
+      zero = __float2half2_rn(-(scale_f * ((z_tmp) + 1)));
+    } else if (z_mod == 21){
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
+      zero = __float2half2_rn(-(scale_f * ((z_tmp) + 1)));
+    } else {
+      zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1)));
+    }
+	
+    res2 = {};
+    tmp1 = as_unsigned(mat[i]);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 24) & 0x3f][off], scale, zero), blockvec[k + 4], res2);
+    i += width;
+    tmp2 = as_unsigned(mat[i]);
+    tmp = (tmp1 >> 30) | ((tmp2 << 2) & 0x3c);
+    res2 = __hfma2(__hfma2(deq2[tmp][off], scale, zero), blockvec[k + 5], res2);
+    tmp2 >>= 4;
+    k += 6;
+    res2 = __hfma2(__hfma2(deq2[(tmp2 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp2 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp2 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp2 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
+    i += width;
+    tmp1 = as_unsigned(mat[i]);
+    tmp = (tmp2 >> 24) | ((tmp1 << 4) & 0x30);
+    res2 = __hfma2(__hfma2(deq2[tmp][off], scale, zero), blockvec[k + 4], res2);
+    tmp1 >>= 2;
+    k += 5;
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 24) & 0x3f][off], scale, zero), blockvec[k + 4], res2);
+    i += width;
+    k += 5;
+    res += __half2float(res2.x) + __half2float(res2.y);
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+void vecquant4matmul_faster_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize,
+  int vec_height
+) {
+  int batch = vec.size(0);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+  
+  dim3 blocks(
+    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  VecQuant4MatMulKernelFaster_old<<<blocks, threads>>>(
+    (half2*) vec.data_ptr(),
+    mat.data_ptr<int>(),
+    mul.data_ptr<float>(),
+    scales.data_ptr<float>(),
+    zeros.data_ptr<int>(),
+    batch, vec_height, height, width, zero_width, groupsize
+  );
+}
+
+__global__ void VecQuant4MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const  	 int* __restrict__ zeros,
+	int batch,
+	int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  const int blockwidth2 = BLOCKWIDTH / 2;
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT4 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ half2 blockvec[blockwidth2];
+  if (threadIdx.x < blockwidth2)
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
+
+  __shared__ half2 deq2[256][8];
+  int val = threadIdx.x / 8;
+  int off = threadIdx.x % 8;
+  for (; val < 256; val += BLOCKWIDTH / 8) {
+    deq2[val][off] = __halves2half2(
+       __int2half_rn(val & 0xF), __int2half_rn(val >> 4)
+    );
+  }
+
+  int i = width * h + w;
+  int g_h = h * 8;
+  int k = 0;
+
+  int z_w = w / 8; 
+  int z_mod = (w % 8) * 4;
+
+  float res = 0;
+  half2 res2;
+
+  unsigned int tmp;
+
+  __syncthreads();
+
+  while (k < blockwidth2) {
+    int g = (g_h + (k * 2)) / groupsize;
+	float scale_f = scales[g * width + w];
+    half2 scale = __float2half2_rn(scale_f);
+    half2 zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1)));
+	
+    res2 = {};
+    tmp = as_unsigned(mat[i]);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  0) & 0xff][off], scale, zero), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  8) & 0xff][off], scale, zero), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 16) & 0xff][off], scale, zero), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 24) & 0xff][off], scale, zero), blockvec[k + 3], res2);
+	i += width;
+    k += 4;
+    res += __half2float(res2.x) + __half2float(res2.y);
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
```

### Comparing `auto_gptq-0.3.0/autogptq_cuda/autogptq_cuda_kernel_64.cu` & `auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_kernel_64.cu`

 * *Files 22% similar despite different names*

```diff
@@ -1,1560 +1,1428 @@
-#include <torch/all.h>
-#include <torch/python.h>
-#include <cuda.h>
-#include <cuda_runtime.h>
-#include <cuda_fp16.h>
-
-// atomicAdd for double-precision floating-point numbers on hardware with
-// compute capability < 6.0 from:
-// https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#atomic-functions
-// #if defined(__CUDA_ARCH__) && __CUDA_ARCH__ < 600
-// __device__ double atomicAdd(
-//     double* address,
-//     double val
-// ) {
-//   unsigned long long int* address_as_ull = (unsigned long long int*)address;
-//   unsigned long long int old = *address_as_ull, assumed;
-//
-//   do {
-//     assumed = old;
-//     old = atomicCAS(
-//       address_as_ull,
-//       assumed,
-//       __double_as_longlong(val + __longlong_as_double(assumed))
-//     );
-//
-//   // Note: uses integer comparison to avoid hang in case of NaN (since NaN != NaN)
-//   } while (assumed != old);
-//
-//   return __longlong_as_double(old);
-// }
-// #endif
-
-#if defined(__CUDA_ARCH__) && __CUDA_ARCH__ < 700
-// adapted from https://github.com/torch/cutorch/blob/master/lib/THC/THCAtomics.cuh
-__device__ __forceinline__ void atomicAdd(c10::Half* address, c10::Half val) {
-    unsigned int *address_as_ui = reinterpret_cast<unsigned int *>(reinterpret_cast<char *>(address) - (reinterpret_cast<size_t>(address) & 2));
-    unsigned int old = *address_as_ui;
-    unsigned int assumed;
-
-    do {
-        assumed = old;
-        unsigned short hsum = reinterpret_cast<size_t>(address) & 2 ? (old >> 16) : (old & 0xffff);
-        hsum += val;
-        old = reinterpret_cast<size_t>(address) & 2
-                 ? (old & 0xffff) | (hsum << 16)
-                 : (old & 0xffff0000) | hsum;
-        old = atomicCAS(address_as_ui, assumed, old);
-
-    // Note: uses integer comparison to avoid hang in case of NaN (since NaN != NaN)
-    } while (assumed != old);
-}
-__device__ __forceinline__ void atomicAdd(__half* address, c10::Half val) {
-    unsigned int * address_as_ui = (unsigned int *) ((char *)address - ((size_t)address & 2));
-    unsigned int old = *address_as_ui;
-    unsigned int assumed;
-
-    do {
-        assumed = old;
-        __half_raw hsum;
-        hsum.x = (size_t)address & 2 ? (old >> 16) : (old & 0xffff);
-        half tmpres = __hadd(hsum, val);
-        hsum = __half_raw(tmpres);
-        old = (size_t)address & 2 ? (old & 0xffff) | (hsum.x << 16) : (old & 0xffff0000) | hsum.x;
-        old = atomicCAS(address_as_ui, assumed, old);
-    } while (assumed != old);
-}
-#endif
-
-
-template <typename scalar_t>
-__global__ void VecQuant2MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-	const  	    int* __restrict__ g_idx,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-	int zero_width
-);
-
-template <typename scalar_t>
-__global__ void VecQuant3MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-	const  	    int* __restrict__ g_idx,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-	int zero_width
-);
-
-// template <typename scalar_t>
-// __global__ void VecQuant4MatMulKernel(
-//     const  scalar_t* __restrict__ vec,
-//     const       int* __restrict__ mat,
-//            scalar_t* __restrict__ mul,
-//     const  scalar_t* __restrict__ scales,
-//     const  		int* __restrict__ zeros,
-// 	const  	    int* __restrict__ g_idx,
-//     int batch,
-//     int vec_height,
-//     int height,
-//     int width,
-// 	int zero_width
-// );
-
-// referenced from https://github.com/iwalton3/GPTQ-for-LLaMa/commit/209d16b0187f149bf13318360925cc4f679cb2ea
-template <typename scalar_t>
-__global__ void VecQuant4MatMulKernel(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const    int* __restrict__ zeros,
-    const    int* __restrict__ g_idx,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width
-);
-
-template <typename scalar_t>
-__global__ void VecQuant8MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-	const  	    int* __restrict__ g_idx,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-	int zero_width
-);
-
-template <typename scalar_t>
-__global__ void VecQuant2MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-template <typename scalar_t>
-__global__ void VecQuant3MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-template <typename scalar_t>
-__global__ void VecQuant4MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-template <typename scalar_t>
-__global__ void VecQuant8MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-__global__ void VecQuant2MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const    int* __restrict__ zeros,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-__global__ void VecQuant3MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const    int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-__global__ void VecQuant4MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const    int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-
-const int BLOCKWIDTH  = 64;
-const int BLOCKHEIGHT2 =  4;
-const int BLOCKHEIGHT3 =  6;
-const int BLOCKHEIGHT4 =  8;
-const int BLOCKHEIGHT8 =  16;
-
-__device__ inline unsigned int as_unsigned(int i) {
-  return *reinterpret_cast<unsigned int*>(&i);
-}
-
-__device__ inline int as_int(int i) {
-  return *reinterpret_cast<int*>(&i);
-}
-
-
-void vecquant2matmul_cuda(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant2matmul_cuda", ([&] {
-      VecQuant2MatMulKernel<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
-        batch, vec_height, height, width, zero_width
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant2MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-    const   	int* __restrict__ g_idx,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-	int zero_width
-) {
-  int h = BLOCKHEIGHT2 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-  
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  int i = width * h + w;
-  int g_h = h * 16;
-  int k;
-  unsigned int g;
-  scalar_t w_tmp;
-  
-  int z_w = w / 16; 
-  int z_mod = (w % 16) * 2;
-  
-  float weight[BLOCKWIDTH];
-  
-  for (k = 0; k <  BLOCKWIDTH; ++k){	
-	int k_w = (k / 16); 
-	int k_bit = (k % 16) * 2;
-	
-    g = as_int(g_idx[g_h + k]);
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scalar_t((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod & 0x3) + 1);
-	
-    w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0x3);
-    
-	weight[k] = scale * (w_tmp - zero);
-  }
-
-  scalar_t res;
-  for (int b = 0; b < batch; ++b){	
-	res = 0;
-	
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-    __syncthreads();
-	for (k = 0; k <  BLOCKWIDTH; ++k){	
-	  res += weight[k] * blockvec[k];
-    }
-    atomicAdd(&mul[b * width + w], res);
-    __syncthreads();
-  }
-}
-
-void vecquant3matmul_cuda(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant3matmul_cuda", ([&] {
-      VecQuant3MatMulKernel<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
-        batch, vec_height, height, width, zero_width
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant3MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const       int* __restrict__ zeros,
-    const   	int* __restrict__ g_idx,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-	int zero_width
-) {
-  int h = BLOCKHEIGHT3 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-  
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  int i = width * h + w;
-  int g_h = (h / 3) * 32;
-  int k;
-  unsigned int g;
-  scalar_t w_tmp;
-  
-  int z_w = (w / 32) * 3; 
-  int z_mod = w % 32;
-  int z_bit;
-  unsigned int z_tmp;
-  if (z_mod != 10){
-    if (z_mod != 21){
-      z_bit = z_mod;
-      if (z_bit > 21){
-        z_bit -= 22;
-        z_bit *= 3;
-        z_bit += 2;
-        z_w += 2;
-      } else if (z_bit > 10){
-        z_bit -= 11;
-        z_bit *= 3;
-        z_bit += 1;
-        z_w += 1;
-      } else {
-        z_bit *= 3;
-      }
-    } else {
-      z_w += 1;
-    }
-  }
-  
-  float weight[BLOCKWIDTH];
-  
-  for (k = 0; k <  BLOCKWIDTH; ++k){	
-	int k_w = (k / 32) * 3; 
-	int k_mod = k % 32;
-	int k_bit;
-	  
-	if (k_mod != 10){
-	  if (k_mod != 21){
-        k_bit = k_mod;
-        if (k_bit > 21){
-		  k_bit -= 22;
-		  k_bit *= 3;
-		  k_bit += 2;
-		  k_w += 2;
-        } else if (k_bit > 10){
-		  k_bit -= 11;
-		  k_bit *= 3;
-		  k_bit += 1;
-		  k_w += 1;
-        } else {
-		  k_bit *= 3;
-        }
-	  } else {
-        k_w += 1;
-	  }
-	}
-	
-    g = as_int(g_idx[g_h + k]);
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero;
-    if (z_mod == 10) {
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
-      zero = scalar_t((z_tmp) + 1);
-    } else if (z_mod == 21){
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
-      zero = scalar_t((z_tmp) + 1);
-    } else {
-      zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1);
-    }
-	
-    if (k_mod == 10) {
-      w_tmp = (as_unsigned(mat[i + (k_w * width)]) >> 30) | ((as_unsigned(mat[i + ((k_w + 1)* width)]) << 2) & 0x4);
-    } else if (k_mod == 21){
-      w_tmp = (as_unsigned(mat[i + (k_w * width)]) >> 31) | ((as_unsigned(mat[i + ((k_w + 1)* width)]) << 1) & 0x6);
-    } else {
-      w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0x7);
-    }
-	weight[k] = scale * (w_tmp - zero);
-  }
-
-  scalar_t res;
-  for (int b = 0; b < batch; ++b){	
-	res = 0;
-	
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-    __syncthreads();
-	for (k = 0; k <  BLOCKWIDTH; ++k){	
-	  res += weight[k] * blockvec[k];
-    }
-    atomicAdd(&mul[b * width + w], res);
-    __syncthreads();
-  }
-}
-
-void vecquant4matmul_cuda(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  torch::Tensor g_idx,
-  int vec_height
-) {
-  int batch = vec.size(0);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_SWITCH(vec.type(), "vecquant4matmul_cuda",
-    AT_DISPATCH_CASE(at::ScalarType::Half, ([&] {
-      VecQuant4MatMulKernel<<<blocks, threads>>>(
-        (half2*) vec.data_ptr<scalar_t>(),
-        mat.data_ptr<int>(),
-        mul.data_ptr<scalar_t>(),
-        scales.data_ptr<scalar_t>(),
-        zeros.data_ptr<int>(),
-        g_idx.data_ptr<int>(),
-        batch, vec_height, height, width, zero_width
-      );
-    })
-  ));
-}
-
-// void vecquant4matmul_cuda(
-//   torch::Tensor vec,
-//   torch::Tensor mat,
-//   torch::Tensor mul,
-//   torch::Tensor scales,
-//   torch::Tensor zeros,
-//   torch::Tensor g_idx
-// ) {
-//   int batch = vec.size(0);
-//   int vec_height = vec.size(1);
-//   int height = mat.size(0);
-//   int width = mat.size(1);
-//   int zero_width = zeros.size(1);
-//
-//   dim3 blocks(
-//     (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
-//     (width + BLOCKWIDTH - 1) / BLOCKWIDTH
-//   );
-//   dim3 threads(BLOCKWIDTH);
-//
-//   AT_DISPATCH_FLOATING_TYPES(
-//     vec.type(), "vecquant4matmul_cuda", ([&] {
-//       VecQuant4MatMulKernel<<<blocks, threads>>>(
-//         vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-//         scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(),
-//         batch, vec_height, height, width, zero_width
-//       );
-//     })
-//   );
-// }
-
-template <typename scalar_t>
-__global__ void VecQuant4MatMulKernel(
-    const     half2* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	    int* __restrict__ zeros,
-    const       int* __restrict__ g_idx,
-	int batch,
-	int vec_height,
-    int height,
-    int width,
-    int zero_width
-) {
-  const int blockwidth2 = BLOCKWIDTH / 2;
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT4 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ half2 blockvec[blockwidth2];
-  if (threadIdx.x < blockwidth2)
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
-
-  __shared__ half2 deq2[256][8];
-  int val = threadIdx.x / 8;
-  int off = threadIdx.x % 8;
-  for (; val < 256; val += BLOCKWIDTH / 8) {
-    deq2[val][off] = __halves2half2(
-       __int2half_rn(val & 0xF), __int2half_rn(val >> 4)
-    );
-  }
-
-  int i = width * h + w;
-  int g_h = h * 8;
-  int k = 0;
-
-  int z_w = w / 8;
-  int z_mod = (w % 8) * 4;
-
-  scalar_t res = 0;
-  half2 res2;
-
-  unsigned int tmp;
-
-  __syncthreads();
-
-  while (k < blockwidth2) {
-    res2 = {};
-    tmp = as_unsigned(mat[i]);
-
-    int tmp_k = 0;
-    half2 scales_tmp[4];
-    half2 zeros_tmp[4];
-    while (tmp_k < 4) {
-      int g = as_int(g_idx[g_h + (k + tmp_k) * 2]);
-      int g2 = as_int(g_idx[g_h + (k + tmp_k) * 2 + 1]);
-      scalar_t scale_f = scales[g * width + w];
-      scalar_t scale_f2 = scales[g2 * width + w];
-      half2 scale = __halves2half2(scale_f, scale_f2);
-      half2 zero = __halves2half2(
-        __hmul(-scale_f, __int2half_rn(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1)),
-        __hmul(-scale_f2, __int2half_rn(((as_unsigned(zeros[g2 * zero_width + z_w]) >> z_mod) & 0xF) + 1))
-      );
-      scales_tmp[tmp_k] = scale;
-      zeros_tmp[tmp_k] = zero;
-      tmp_k += 1;
-    }
-
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  0) & 0xff][off], scales_tmp[0], zeros_tmp[0]), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  8) & 0xff][off], scales_tmp[1], zeros_tmp[1]), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 16) & 0xff][off], scales_tmp[2], zeros_tmp[2]), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 24) & 0xff][off], scales_tmp[3], zeros_tmp[3]), blockvec[k + 3], res2);
-	i += width;
-    k += 4;
-    res = __hadd(res, __hadd(res2.x, res2.y));;
-  }
-
-  __half* mul2 = (__half*)mul;
-  atomicAdd(&mul2[b * width + w], res);
-}
-
-// template <typename scalar_t>
-// __global__ void VecQuant4MatMulKernel(
-//     const  scalar_t* __restrict__ vec,
-//     const       int* __restrict__ mat,
-//            scalar_t* __restrict__ mul,
-//     const  scalar_t* __restrict__ scales,
-//     const       int* __restrict__ zeros,
-//     const   	int* __restrict__ g_idx,
-//     int batch,
-//     int vec_height,
-//     int height,
-//     int width,
-// 	int zero_width
-// ) {
-//   int h = BLOCKHEIGHT4 * blockIdx.x;
-//   int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-//
-//   __shared__ scalar_t blockvec[BLOCKWIDTH];
-//   int i = width * h + w;
-//   int g_h = h * 8;
-//   int k;
-//   unsigned int g;
-//   scalar_t w_tmp;
-//
-//
-//   int z_w = w / 8;
-//   int z_mod = (w % 8) * 4;
-//
-//   float weight[BLOCKWIDTH];
-//
-//   for (k = 0; k <  BLOCKWIDTH; ++k){
-// 	int k_w = (k / 8);
-// 	int k_bit = (k % 8) * 4;
-//
-//     g = as_int(g_idx[g_h + k]);
-//     scalar_t scale = scales[g * width + w];
-//     scalar_t zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1);
-//
-//     w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0xF);
-//
-// 	weight[k] = scale * (w_tmp - zero);
-//   }
-//
-//   scalar_t res;
-//   for (int b = 0; b < batch; ++b){
-// 	res = 0;
-//
-//     blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-//     __syncthreads();
-// 	for (k = 0; k <  BLOCKWIDTH; ++k){
-// 	  res += weight[k] * blockvec[k];
-//     }
-//     atomicAdd(&mul[b * width + w], res);
-//     __syncthreads();
-//   }
-// }
-
-void vecquant8matmul_cuda(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT8 - 1) / BLOCKHEIGHT8,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant8matmul_cuda", ([&] {
-      VecQuant8MatMulKernel<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
-        batch, vec_height, height, width, zero_width
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant8MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const       int* __restrict__ zeros,
-    const   	int* __restrict__ g_idx,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-	int zero_width
-) {
-  int h = BLOCKHEIGHT8 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-  
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  int i = width * h + w;
-  int g_h = h * 4;
-  int k;
-  unsigned int g;
-  scalar_t w_tmp;
-  
-  int z_w = w / 4; 
-  int z_mod = (w % 4) * 8;
-  
-  float weight[BLOCKWIDTH];
-  
-  for (k = 0; k <  BLOCKWIDTH; ++k){	
-	int k_w = (k / 4); 
-	int k_bit = (k % 4) * 8;
-	
-    g = as_int(g_idx[g_h + k]);
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xFF) + 1);
-	
-    w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0xFF);
-    
-	weight[k] = scale * (w_tmp - zero);
-  }
-
-  scalar_t res;
-  for (int b = 0; b < batch; ++b){	
-	res = 0;
-	
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-    __syncthreads();
-	for (k = 0; k <  BLOCKWIDTH; ++k){	
-	  res += weight[k] * blockvec[k];
-    }
-    atomicAdd(&mul[b * width + w], res);
-    __syncthreads();
-  }
-}
-
-
-void vecquant2matmul_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant2matmul_cuda_old", ([&] {
-      VecQuant2MatMulKernel_old<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(),
-        batch, vec_height, height, width, zero_width, groupsize
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant2MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT2 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-  __syncthreads();
-
-  scalar_t res = 0;
-  int i = width * h + w;
-  int g_h = h * 16;
-  int k = 0;
-  
-  int z_w = w / 16; 
-  int z_mod = (w % 16) * 2;
-
-  unsigned int tmp;
-
-  while (k < BLOCKWIDTH) {
-    tmp = as_unsigned(mat[i]);
-	
-    int g = (g_h + k) / groupsize;
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scale * scalar_t((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod & 0x3) + 1);
-	
-    res += (scale * scalar_t((tmp >> 0) & 0x3) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp >> 2) & 0x3) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp >> 4) & 0x3) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp >> 6) & 0x3) - zero) * blockvec[k + 3];
-    res += (scale * scalar_t((tmp >> 8) & 0x3) - zero) * blockvec[k + 4];
-    res += (scale * scalar_t((tmp >> 10) & 0x3) - zero) * blockvec[k + 5];
-    res += (scale * scalar_t((tmp >> 12) & 0x3) - zero) * blockvec[k + 6];
-    res += (scale * scalar_t((tmp >> 14) & 0x3) - zero) * blockvec[k + 7];
-    res += (scale * scalar_t((tmp >> 16) & 0x3) - zero) * blockvec[k + 8];
-    res += (scale * scalar_t((tmp >> 18) & 0x3) - zero) * blockvec[k + 9];
-    res += (scale * scalar_t((tmp >> 20) & 0x3) - zero) * blockvec[k + 10];
-    res += (scale * scalar_t((tmp >> 22) & 0x3) - zero) * blockvec[k + 11];
-    res += (scale * scalar_t((tmp >> 24) & 0x3) - zero) * blockvec[k + 12];
-    res += (scale * scalar_t((tmp >> 26) & 0x3) - zero) * blockvec[k + 13];
-    res += (scale * scalar_t((tmp >> 28) & 0x3) - zero) * blockvec[k + 14];
-    res += (scale * scalar_t((tmp >> 30) & 0x3) - zero) * blockvec[k + 15];
-	
-    i += width;
-    k += 16;
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-void vecquant3matmul_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant3matmul_cuda_old", ([&] {
-      VecQuant3MatMulKernel_old<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(),
-        batch, vec_height, height, width, zero_width, groupsize
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant3MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT3 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-  __syncthreads();
-
-  scalar_t res = 0;
-  int i = width * h + w;
-  int g_h = (h / 3) * 32;
-  int k = 0;
-  
-  int z_w = (w / 32) * 3; 
-  int z_mod = w % 32;
-  int z_bit;
-  
-  if (z_mod != 10){
-    if (z_mod != 21){
-      z_bit = z_mod;
-      if (z_bit > 21){
-        z_bit -= 22;
-        z_bit *= 3;
-        z_bit += 2;
-        z_w += 2;
-      } else if (z_bit > 10){
-        z_bit -= 11;
-        z_bit *= 3;
-        z_bit += 1;
-        z_w += 1;
-      } else {
-        z_bit *= 3;
-      }
-    } else {
-      z_w += 1;
-    }
-  }
- 
-  unsigned int tmp1;
-  unsigned int tmp2;
-  unsigned int tmp;
-  unsigned int z_tmp;
-
-  while (k < BLOCKWIDTH) {
-    tmp1 = as_unsigned(mat[i]);
-	
-    int g = (g_h + k) / groupsize;
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero;
-    if (z_mod == 10) {
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
-      zero = scale * scalar_t((z_tmp) + 1);
-    } else if (z_mod == 21){
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
-      zero = scale * scalar_t((z_tmp) + 1);
-    } else {
-      zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1);
-    }
-	
-    res += (scale * scalar_t((tmp1 >>  0) & 0x7) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp1 >>  3) & 0x7) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp1 >>  6) & 0x7) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp1 >>  9) & 0x7) - zero) * blockvec[k + 3];
-    res += (scale * scalar_t((tmp1 >> 12) & 0x7) - zero) * blockvec[k + 4];
-    res += (scale * scalar_t((tmp1 >> 15) & 0x7) - zero) * blockvec[k + 5];
-    res += (scale * scalar_t((tmp1 >> 18) & 0x7) - zero) * blockvec[k + 6];
-    res += (scale * scalar_t((tmp1 >> 21) & 0x7) - zero) * blockvec[k + 7];
-    res += (scale * scalar_t((tmp1 >> 24) & 0x7) - zero) * blockvec[k + 8];
-    res += (scale * scalar_t((tmp1 >> 27) & 0x7) - zero) * blockvec[k + 9];
-	
-    i += width;
-    tmp2 = as_unsigned(mat[i]);
-    tmp = (tmp1 >> 30) | ((tmp2 << 2) & 0x4);
-    tmp2 >>= 1;
-    res += (scale * scalar_t(tmp) - zero) * blockvec[k + 10];
-    k += 11;
-	
-    res += (scale * scalar_t((tmp2 >>  0) & 0x7) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp2 >>  3) & 0x7) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp2 >>  6) & 0x7) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp2 >>  9) & 0x7) - zero) * blockvec[k + 3];
-    res += (scale * scalar_t((tmp2 >> 12) & 0x7) - zero) * blockvec[k + 4];
-    res += (scale * scalar_t((tmp2 >> 15) & 0x7) - zero) * blockvec[k + 5];
-    res += (scale * scalar_t((tmp2 >> 18) & 0x7) - zero) * blockvec[k + 6];
-    res += (scale * scalar_t((tmp2 >> 21) & 0x7) - zero) * blockvec[k + 7];
-    res += (scale * scalar_t((tmp2 >> 24) & 0x7) - zero) * blockvec[k + 8];
-    res += (scale * scalar_t((tmp2 >> 27) & 0x7) - zero) * blockvec[k + 9];
-	
-    i += width;
-    tmp1 = as_unsigned(mat[i]);
-    tmp = (tmp2 >> 30) | ((tmp1 << 1) & 0x6);
-    tmp1 >>= 2;
-    res += (scale * scalar_t(tmp) - zero) * blockvec[k + 10];
-    k += 11;
-	
-    res += (scale * scalar_t((tmp1 >>  0) & 0x7) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp1 >>  3) & 0x7) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp1 >>  6) & 0x7) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp1 >>  9) & 0x7) - zero) * blockvec[k + 3];
-    res += (scale * scalar_t((tmp1 >> 12) & 0x7) - zero) * blockvec[k + 4];
-    res += (scale * scalar_t((tmp1 >> 15) & 0x7) - zero) * blockvec[k + 5];
-    res += (scale * scalar_t((tmp1 >> 18) & 0x7) - zero) * blockvec[k + 6];
-    res += (scale * scalar_t((tmp1 >> 21) & 0x7) - zero) * blockvec[k + 7];
-    res += (scale * scalar_t((tmp1 >> 24) & 0x7) - zero) * blockvec[k + 8];
-    res += (scale * scalar_t((tmp1 >> 27) & 0x7) - zero) * blockvec[k + 9];
-	
-    i += width;
-    k += 10;
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-void vecquant4matmul_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant4matmul_cuda_old", ([&] {
-      VecQuant4MatMulKernel_old<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(),
-        batch, vec_height, height, width, zero_width, groupsize
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant4MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const       int* __restrict__ zeros,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT4 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-  __syncthreads();
-
-  scalar_t res = 0;
-  int i = width * h + w;
-  int g_h = h * 8;
-  int k = 0;
-
-  int z_w = w / 8; 
-  int z_mod = (w % 8) * 4;
-
-  unsigned int tmp;
-
-  while (k < BLOCKWIDTH) {
-    tmp = as_unsigned(mat[i]);
-	
-    int g = (g_h + k) / groupsize;
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1);
-	
-    res += (scale * scalar_t((tmp >> 0) & 0xF) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp >> 4) & 0xF) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp >> 8) & 0xF) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp >> 12) & 0xF) - zero) * blockvec[k + 3];
-    res += (scale * scalar_t((tmp >> 16) & 0xF) - zero) * blockvec[k + 4];
-    res += (scale * scalar_t((tmp >> 20) & 0xF) - zero) * blockvec[k + 5];
-    res += (scale * scalar_t((tmp >> 24) & 0xF) - zero) * blockvec[k + 6];
-    res += (scale * scalar_t((tmp >> 28) & 0xF) - zero) * blockvec[k + 7];
-	
-    i += width;
-    k += 8;
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-void vecquant8matmul_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT8 - 1) / BLOCKHEIGHT8,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant8matmul_cuda_old", ([&] {
-      VecQuant8MatMulKernel_old<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(),
-        batch, vec_height, height, width, zero_width, groupsize
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant8MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT8 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-  __syncthreads();
-
-  scalar_t res = 0;
-  int i = width * h + w;
-  int g_h = h * 4;
-  int k = 0;
-  
-  int z_w = w / 4; 
-  int z_mod = (w % 4) * 8;
-
-  unsigned int tmp;
-
-  while (k < BLOCKWIDTH) { 
-    tmp = as_unsigned(mat[i]);
-	
-    int g = (g_h + k) / groupsize;
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xFF) + 1);
-	
-    res += (scale * scalar_t((tmp >> 0) & 0xFF) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp >> 8) & 0xFF) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp >> 16) & 0xFF) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp >> 24) & 0xFF) - zero) * blockvec[k + 3];
-	
-    i += width;
-    k += 4;
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-
-void vecquant2matmul_faster_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize,
-  int vec_height
-) {
-  int batch = vec.size(0);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-  
-  dim3 blocks(
-    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  VecQuant2MatMulKernelFaster_old<<<blocks, threads>>>(
-    (half2*) vec.data_ptr(),
-    mat.data_ptr<int>(),
-    mul.data_ptr<float>(),
-    scales.data_ptr<float>(),
-    zeros.data_ptr<int>(),
-    batch, vec_height, height, width, zero_width, groupsize
-  );
-}
-
-__global__ void VecQuant2MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const  	 int* __restrict__ zeros,
-	int batch,
-	int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  const int blockwidth2 = BLOCKWIDTH / 2;
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT2 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ half2 blockvec[blockwidth2];
-  if (threadIdx.x < blockwidth2)
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
-
-  __shared__ half2 deq2[16][16];
-  int val = threadIdx.x / 16;
-  int off = threadIdx.x % 16;
-  for (; val < 16; val += BLOCKWIDTH / 16) {
-    deq2[val][off] = __halves2half2(
-       __int2half_rn(val & 0x3), __int2half_rn(val >> 2)
-    );
-  }
-
-  int i = width * h + w;
-  int g_h = h * 16;
-  int k = 0;
-  
-  int z_w = w / 16; 
-  int z_mod = (w % 16) * 2;
-
-  float res = 0;
-  half2 res2;
-
-  unsigned int tmp;
-
-  __syncthreads();
-
-  while (k < blockwidth2) {
-    int g = (g_h + (k * 2)) / groupsize;
-	float scale_f = scales[g * width + w];
-    half2 scale = __float2half2_rn(scale_f);
-    half2 zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0x3) + 1)));
-	
-    res2 = {};
-    tmp = as_unsigned(mat[i]);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  0) & 0xf][off], scale, zero), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  4) & 0xf][off], scale, zero), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  8) & 0xf][off], scale, zero), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 12) & 0xf][off], scale, zero), blockvec[k + 3], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 16) & 0xf][off], scale, zero), blockvec[k + 4], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 20) & 0xf][off], scale, zero), blockvec[k + 5], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 24) & 0xf][off], scale, zero), blockvec[k + 6], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 28) & 0xf][off], scale, zero), blockvec[k + 7], res2);
-	i += width;
-    k += 8;
-    res += __half2float(res2.x) + __half2float(res2.y);
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-void vecquant3matmul_faster_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize,
-  int vec_height
-) {
-  int batch = vec.size(0);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-  
-  dim3 blocks(
-    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  VecQuant3MatMulKernelFaster_old<<<blocks, threads>>>(
-    (half2*) vec.data_ptr(),
-    mat.data_ptr<int>(),
-    mul.data_ptr<float>(),
-    scales.data_ptr<float>(),
-    zeros.data_ptr<int>(),
-    batch, vec_height, height, width, zero_width, groupsize
-  );
-}
-
-__global__ void VecQuant3MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const  	 int* __restrict__ zeros,
-	int batch,
-	int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  const int blockwidth2 = BLOCKWIDTH / 2;
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT3 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ half2 blockvec[blockwidth2];
-  if (threadIdx.x < blockwidth2)
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
-
-  __shared__ half2 deq2[64][32];
-  int val = threadIdx.x / 32;
-  int off = threadIdx.x % 32;
-  for (; val < 64; val += BLOCKWIDTH / 32) {
-    deq2[val][off] = __halves2half2(
-       __int2half_rn(val & 0x7), __int2half_rn(val >> 3)
-    );
-  }
-
-  int i = width * h + w;
-  int g_h = (h / 3) * 32;
-  int k = 0;
-  
-  int z_w = (w / 32) * 3;
-  int z_mod = w % 32;
-  int z_bit;
-  
-  if (z_mod != 10){
-    if (z_mod != 21){
-      z_bit = z_mod;
-      if (z_bit > 21){
-        z_bit -= 22;
-        z_bit *= 3;
-        z_bit += 2;
-        z_w += 2;
-      } else if (z_bit > 10){
-        z_bit -= 11;
-        z_bit *= 3;
-        z_bit += 1;
-        z_w += 1;
-      } else {
-        z_bit *= 3;
-      }
-    } else {
-      z_w += 1;
-    }
-  }
-
-  float res = 0;
-  half2 res2;
-
-  unsigned int tmp1;
-  unsigned int tmp2;
-  unsigned int tmp;
-  unsigned int z_tmp;
-
-  __syncthreads();
-
-  while (k < blockwidth2) {
-    int g = (g_h + (k * 2)) / groupsize;
-	float scale_f = scales[g * width + w];
-    half2 scale = __float2half2_rn(scale_f);
-    half2 zero;
-    if (z_mod == 10) {
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
-      zero = __float2half2_rn(-(scale_f * ((z_tmp) + 1)));
-    } else if (z_mod == 21){
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
-      zero = __float2half2_rn(-(scale_f * ((z_tmp) + 1)));
-    } else {
-      zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1)));
-    }
-	
-    res2 = {};
-    tmp1 = as_unsigned(mat[i]);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 24) & 0x3f][off], scale, zero), blockvec[k + 4], res2);
-    i += width;
-    tmp2 = as_unsigned(mat[i]);
-    tmp = (tmp1 >> 30) | ((tmp2 << 2) & 0x3c);
-    res2 = __hfma2(__hfma2(deq2[tmp][off], scale, zero), blockvec[k + 5], res2);
-    tmp2 >>= 4;
-    k += 6;
-    res2 = __hfma2(__hfma2(deq2[(tmp2 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp2 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp2 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp2 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
-    i += width;
-    tmp1 = as_unsigned(mat[i]);
-    tmp = (tmp2 >> 24) | ((tmp1 << 4) & 0x30);
-    res2 = __hfma2(__hfma2(deq2[tmp][off], scale, zero), blockvec[k + 4], res2);
-    tmp1 >>= 2;
-    k += 5;
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 24) & 0x3f][off], scale, zero), blockvec[k + 4], res2);
-    i += width;
-    k += 5;
-    res += __half2float(res2.x) + __half2float(res2.y);
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-void vecquant4matmul_faster_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize,
-  int vec_height
-) {
-  int batch = vec.size(0);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-  
-  dim3 blocks(
-    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  VecQuant4MatMulKernelFaster_old<<<blocks, threads>>>(
-    (half2*) vec.data_ptr(),
-    mat.data_ptr<int>(),
-    mul.data_ptr<float>(),
-    scales.data_ptr<float>(),
-    zeros.data_ptr<int>(),
-    batch, vec_height, height, width, zero_width, groupsize
-  );
-}
-
-__global__ void VecQuant4MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const  	 int* __restrict__ zeros,
-	int batch,
-	int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  const int blockwidth2 = BLOCKWIDTH / 2;
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT4 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ half2 blockvec[blockwidth2];
-  if (threadIdx.x < blockwidth2)
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
-
-  __shared__ half2 deq2[256][8];
-  int val = threadIdx.x / 8;
-  int off = threadIdx.x % 8;
-  for (; val < 256; val += BLOCKWIDTH / 8) {
-    deq2[val][off] = __halves2half2(
-       __int2half_rn(val & 0xF), __int2half_rn(val >> 4)
-    );
-  }
-
-  int i = width * h + w;
-  int g_h = h * 8;
-  int k = 0;
-
-  int z_w = w / 8; 
-  int z_mod = (w % 8) * 4;
-
-  float res = 0;
-  half2 res2;
-
-  unsigned int tmp;
-
-  __syncthreads();
-
-  while (k < blockwidth2) {
-    int g = (g_h + (k * 2)) / groupsize;
-	float scale_f = scales[g * width + w];
-    half2 scale = __float2half2_rn(scale_f);
-    half2 zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1)));
-	
-    res2 = {};
-    tmp = as_unsigned(mat[i]);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  0) & 0xff][off], scale, zero), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  8) & 0xff][off], scale, zero), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 16) & 0xff][off], scale, zero), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 24) & 0xff][off], scale, zero), blockvec[k + 3], res2);
-	i += width;
-    k += 4;
-    res += __half2float(res2.x) + __half2float(res2.y);
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
+#include <torch/all.h>
+#include <torch/python.h>
+#include <cuda.h>
+#include <cuda_runtime.h>
+#include <cuda_fp16.h>
+
+// atomicAdd for double-precision floating-point numbers on hardware with
+// compute capability < 6.0 from:
+// https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#atomic-functions
+// #if defined(__CUDA_ARCH__) && __CUDA_ARCH__ < 600
+// __device__ double atomicAdd(
+//     double* address,
+//     double val
+// ) {
+//   unsigned long long int* address_as_ull = (unsigned long long int*)address;
+//   unsigned long long int old = *address_as_ull, assumed;
+//
+//   do {
+//     assumed = old;
+//     old = atomicCAS(
+//       address_as_ull,
+//       assumed,
+//       __double_as_longlong(val + __longlong_as_double(assumed))
+//     );
+//
+//   // Note: uses integer comparison to avoid hang in case of NaN (since NaN != NaN)
+//   } while (assumed != old);
+//
+//   return __longlong_as_double(old);
+// }
+// #endif
+
+#if defined(__CUDA_ARCH__) && __CUDA_ARCH__ < 700
+// adapted from https://github.com/torch/cutorch/blob/master/lib/THC/THCAtomics.cuh
+__device__ __forceinline__ void atomicAdd(c10::Half* address, c10::Half val) {
+    unsigned int *address_as_ui = reinterpret_cast<unsigned int *>(reinterpret_cast<char *>(address) - (reinterpret_cast<size_t>(address) & 2));
+    unsigned int old = *address_as_ui;
+    unsigned int assumed;
+
+    do {
+        assumed = old;
+        unsigned short hsum = reinterpret_cast<size_t>(address) & 2 ? (old >> 16) : (old & 0xffff);
+        hsum += val;
+        old = reinterpret_cast<size_t>(address) & 2
+                 ? (old & 0xffff) | (hsum << 16)
+                 : (old & 0xffff0000) | hsum;
+        old = atomicCAS(address_as_ui, assumed, old);
+
+    // Note: uses integer comparison to avoid hang in case of NaN (since NaN != NaN)
+    } while (assumed != old);
+}
+__device__ __forceinline__ void atomicAdd(__half* address, c10::Half val) {
+    unsigned int * address_as_ui = (unsigned int *) ((char *)address - ((size_t)address & 2));
+    unsigned int old = *address_as_ui;
+    unsigned int assumed;
+
+    do {
+        assumed = old;
+        __half_raw hsum;
+        hsum.x = (size_t)address & 2 ? (old >> 16) : (old & 0xffff);
+        half tmpres = __hadd(hsum, val);
+        hsum = __half_raw(tmpres);
+        old = (size_t)address & 2 ? (old & 0xffff) | (hsum.x << 16) : (old & 0xffff0000) | hsum.x;
+        old = atomicCAS(address_as_ui, assumed, old);
+    } while (assumed != old);
+}
+#endif
+
+
+template <typename scalar_t>
+__global__ void VecQuant2MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+	const  	    int* __restrict__ g_idx,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+	int zero_width
+);
+
+template <typename scalar_t>
+__global__ void VecQuant3MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+	const  	    int* __restrict__ g_idx,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+	int zero_width
+);
+
+template <typename scalar_t>
+__global__ void VecQuant4MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+	const  	    int* __restrict__ g_idx,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+	int zero_width
+);
+
+
+template <typename scalar_t>
+__global__ void VecQuant8MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+	const  	    int* __restrict__ g_idx,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+	int zero_width
+);
+
+template <typename scalar_t>
+__global__ void VecQuant2MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+template <typename scalar_t>
+__global__ void VecQuant3MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+template <typename scalar_t>
+__global__ void VecQuant4MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+template <typename scalar_t>
+__global__ void VecQuant8MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+__global__ void VecQuant2MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const    int* __restrict__ zeros,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+__global__ void VecQuant3MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const    int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+__global__ void VecQuant4MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const    int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+
+const int BLOCKWIDTH  = 64;
+const int BLOCKHEIGHT2 =  4;
+const int BLOCKHEIGHT3 =  6;
+const int BLOCKHEIGHT4 =  8;
+const int BLOCKHEIGHT8 =  16;
+
+__device__ inline unsigned int as_unsigned(int i) {
+  return *reinterpret_cast<unsigned int*>(&i);
+}
+
+__device__ inline int as_int(int i) {
+  return *reinterpret_cast<int*>(&i);
+}
+
+
+void vecquant2matmul_cuda(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant2matmul_cuda", ([&] {
+      VecQuant2MatMulKernel<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
+        batch, vec_height, height, width, zero_width
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant2MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+    const   	int* __restrict__ g_idx,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+	int zero_width
+) {
+  int h = BLOCKHEIGHT2 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+  
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  int i = width * h + w;
+  int g_h = h * 16;
+  int k;
+  unsigned int g;
+  scalar_t w_tmp;
+  
+  int z_w = w / 16; 
+  int z_mod = (w % 16) * 2;
+  
+  float weight[BLOCKWIDTH];
+  
+  for (k = 0; k <  BLOCKWIDTH; ++k){	
+	int k_w = (k / 16); 
+	int k_bit = (k % 16) * 2;
+	
+    g = as_int(g_idx[g_h + k]);
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scalar_t((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod & 0x3) + 1);
+	
+    w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0x3);
+    
+	weight[k] = scale * (w_tmp - zero);
+  }
+
+  scalar_t res;
+  for (int b = 0; b < batch; ++b){	
+	res = 0;
+	
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+    __syncthreads();
+	for (k = 0; k <  BLOCKWIDTH; ++k){	
+	  res += weight[k] * blockvec[k];
+    }
+    atomicAdd(&mul[b * width + w], res);
+    __syncthreads();
+  }
+}
+
+void vecquant3matmul_cuda(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant3matmul_cuda", ([&] {
+      VecQuant3MatMulKernel<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
+        batch, vec_height, height, width, zero_width
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant3MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const       int* __restrict__ zeros,
+    const   	int* __restrict__ g_idx,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+	int zero_width
+) {
+  int h = BLOCKHEIGHT3 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+  
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  int i = width * h + w;
+  int g_h = (h / 3) * 32;
+  int k;
+  unsigned int g;
+  scalar_t w_tmp;
+  
+  int z_w = (w / 32) * 3; 
+  int z_mod = w % 32;
+  int z_bit;
+  unsigned int z_tmp;
+  if (z_mod != 10){
+    if (z_mod != 21){
+      z_bit = z_mod;
+      if (z_bit > 21){
+        z_bit -= 22;
+        z_bit *= 3;
+        z_bit += 2;
+        z_w += 2;
+      } else if (z_bit > 10){
+        z_bit -= 11;
+        z_bit *= 3;
+        z_bit += 1;
+        z_w += 1;
+      } else {
+        z_bit *= 3;
+      }
+    } else {
+      z_w += 1;
+    }
+  }
+  
+  float weight[BLOCKWIDTH];
+  
+  for (k = 0; k <  BLOCKWIDTH; ++k){	
+	int k_w = (k / 32) * 3; 
+	int k_mod = k % 32;
+	int k_bit;
+	  
+	if (k_mod != 10){
+	  if (k_mod != 21){
+        k_bit = k_mod;
+        if (k_bit > 21){
+		  k_bit -= 22;
+		  k_bit *= 3;
+		  k_bit += 2;
+		  k_w += 2;
+        } else if (k_bit > 10){
+		  k_bit -= 11;
+		  k_bit *= 3;
+		  k_bit += 1;
+		  k_w += 1;
+        } else {
+		  k_bit *= 3;
+        }
+	  } else {
+        k_w += 1;
+	  }
+	}
+	
+    g = as_int(g_idx[g_h + k]);
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero;
+    if (z_mod == 10) {
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
+      zero = scalar_t((z_tmp) + 1);
+    } else if (z_mod == 21){
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
+      zero = scalar_t((z_tmp) + 1);
+    } else {
+      zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1);
+    }
+	
+    if (k_mod == 10) {
+      w_tmp = (as_unsigned(mat[i + (k_w * width)]) >> 30) | ((as_unsigned(mat[i + ((k_w + 1)* width)]) << 2) & 0x4);
+    } else if (k_mod == 21){
+      w_tmp = (as_unsigned(mat[i + (k_w * width)]) >> 31) | ((as_unsigned(mat[i + ((k_w + 1)* width)]) << 1) & 0x6);
+    } else {
+      w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0x7);
+    }
+	weight[k] = scale * (w_tmp - zero);
+  }
+
+  scalar_t res;
+  for (int b = 0; b < batch; ++b){	
+	res = 0;
+	
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+    __syncthreads();
+	for (k = 0; k <  BLOCKWIDTH; ++k){	
+	  res += weight[k] * blockvec[k];
+    }
+    atomicAdd(&mul[b * width + w], res);
+    __syncthreads();
+  }
+}
+
+void vecquant4matmul_cuda(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant4matmul_cuda", ([&] {
+      VecQuant4MatMulKernel<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
+        batch, vec_height, height, width, zero_width
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant4MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const       int* __restrict__ zeros,
+    const   	int* __restrict__ g_idx,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+	int zero_width
+) {
+  int h = BLOCKHEIGHT4 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+  
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  int i = width * h + w;
+  int g_h = h * 8;
+  int k;
+  unsigned int g;
+  scalar_t w_tmp;
+  
+
+  int z_w = w / 8; 
+  int z_mod = (w % 8) * 4;
+  
+  float weight[BLOCKWIDTH];
+  
+  for (k = 0; k <  BLOCKWIDTH; ++k){	
+	int k_w = (k / 8); 
+	int k_bit = (k % 8) * 4;
+	
+    g = as_int(g_idx[g_h + k]);
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1);
+	
+    w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0xF);
+    
+	weight[k] = scale * (w_tmp - zero);
+  }
+
+  scalar_t res;
+  for (int b = 0; b < batch; ++b){	
+	res = 0;
+	
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+    __syncthreads();
+	for (k = 0; k <  BLOCKWIDTH; ++k){	
+	  res += weight[k] * blockvec[k];
+    }
+    atomicAdd(&mul[b * width + w], res);
+    __syncthreads();
+  }
+}
+
+void vecquant8matmul_cuda(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT8 - 1) / BLOCKHEIGHT8,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant8matmul_cuda", ([&] {
+      VecQuant8MatMulKernel<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
+        batch, vec_height, height, width, zero_width
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant8MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const       int* __restrict__ zeros,
+    const   	int* __restrict__ g_idx,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+	int zero_width
+) {
+  int h = BLOCKHEIGHT8 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+  
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  int i = width * h + w;
+  int g_h = h * 4;
+  int k;
+  unsigned int g;
+  scalar_t w_tmp;
+  
+  int z_w = w / 4; 
+  int z_mod = (w % 4) * 8;
+  
+  float weight[BLOCKWIDTH];
+  
+  for (k = 0; k <  BLOCKWIDTH; ++k){	
+	int k_w = (k / 4); 
+	int k_bit = (k % 4) * 8;
+	
+    g = as_int(g_idx[g_h + k]);
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xFF) + 1);
+	
+    w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0xFF);
+    
+	weight[k] = scale * (w_tmp - zero);
+  }
+
+  scalar_t res;
+  for (int b = 0; b < batch; ++b){	
+	res = 0;
+	
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+    __syncthreads();
+	for (k = 0; k <  BLOCKWIDTH; ++k){	
+	  res += weight[k] * blockvec[k];
+    }
+    atomicAdd(&mul[b * width + w], res);
+    __syncthreads();
+  }
+}
+
+
+void vecquant2matmul_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant2matmul_cuda_old", ([&] {
+      VecQuant2MatMulKernel_old<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(),
+        batch, vec_height, height, width, zero_width, groupsize
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant2MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT2 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+  __syncthreads();
+
+  scalar_t res = 0;
+  int i = width * h + w;
+  int g_h = h * 16;
+  int k = 0;
+  
+  int z_w = w / 16; 
+  int z_mod = (w % 16) * 2;
+
+  unsigned int tmp;
+
+  while (k < BLOCKWIDTH) {
+    tmp = as_unsigned(mat[i]);
+	
+    int g = (g_h + k) / groupsize;
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scale * scalar_t((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod & 0x3) + 1);
+	
+    res += (scale * scalar_t((tmp >> 0) & 0x3) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp >> 2) & 0x3) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp >> 4) & 0x3) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp >> 6) & 0x3) - zero) * blockvec[k + 3];
+    res += (scale * scalar_t((tmp >> 8) & 0x3) - zero) * blockvec[k + 4];
+    res += (scale * scalar_t((tmp >> 10) & 0x3) - zero) * blockvec[k + 5];
+    res += (scale * scalar_t((tmp >> 12) & 0x3) - zero) * blockvec[k + 6];
+    res += (scale * scalar_t((tmp >> 14) & 0x3) - zero) * blockvec[k + 7];
+    res += (scale * scalar_t((tmp >> 16) & 0x3) - zero) * blockvec[k + 8];
+    res += (scale * scalar_t((tmp >> 18) & 0x3) - zero) * blockvec[k + 9];
+    res += (scale * scalar_t((tmp >> 20) & 0x3) - zero) * blockvec[k + 10];
+    res += (scale * scalar_t((tmp >> 22) & 0x3) - zero) * blockvec[k + 11];
+    res += (scale * scalar_t((tmp >> 24) & 0x3) - zero) * blockvec[k + 12];
+    res += (scale * scalar_t((tmp >> 26) & 0x3) - zero) * blockvec[k + 13];
+    res += (scale * scalar_t((tmp >> 28) & 0x3) - zero) * blockvec[k + 14];
+    res += (scale * scalar_t((tmp >> 30) & 0x3) - zero) * blockvec[k + 15];
+	
+    i += width;
+    k += 16;
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+void vecquant3matmul_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant3matmul_cuda_old", ([&] {
+      VecQuant3MatMulKernel_old<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(),
+        batch, vec_height, height, width, zero_width, groupsize
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant3MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT3 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+  __syncthreads();
+
+  scalar_t res = 0;
+  int i = width * h + w;
+  int g_h = (h / 3) * 32;
+  int k = 0;
+  
+  int z_w = (w / 32) * 3; 
+  int z_mod = w % 32;
+  int z_bit;
+  
+  if (z_mod != 10){
+    if (z_mod != 21){
+      z_bit = z_mod;
+      if (z_bit > 21){
+        z_bit -= 22;
+        z_bit *= 3;
+        z_bit += 2;
+        z_w += 2;
+      } else if (z_bit > 10){
+        z_bit -= 11;
+        z_bit *= 3;
+        z_bit += 1;
+        z_w += 1;
+      } else {
+        z_bit *= 3;
+      }
+    } else {
+      z_w += 1;
+    }
+  }
+ 
+  unsigned int tmp1;
+  unsigned int tmp2;
+  unsigned int tmp;
+  unsigned int z_tmp;
+
+  while (k < BLOCKWIDTH) {
+    tmp1 = as_unsigned(mat[i]);
+	
+    int g = (g_h + k) / groupsize;
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero;
+    if (z_mod == 10) {
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
+      zero = scale * scalar_t((z_tmp) + 1);
+    } else if (z_mod == 21){
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
+      zero = scale * scalar_t((z_tmp) + 1);
+    } else {
+      zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1);
+    }
+	
+    res += (scale * scalar_t((tmp1 >>  0) & 0x7) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp1 >>  3) & 0x7) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp1 >>  6) & 0x7) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp1 >>  9) & 0x7) - zero) * blockvec[k + 3];
+    res += (scale * scalar_t((tmp1 >> 12) & 0x7) - zero) * blockvec[k + 4];
+    res += (scale * scalar_t((tmp1 >> 15) & 0x7) - zero) * blockvec[k + 5];
+    res += (scale * scalar_t((tmp1 >> 18) & 0x7) - zero) * blockvec[k + 6];
+    res += (scale * scalar_t((tmp1 >> 21) & 0x7) - zero) * blockvec[k + 7];
+    res += (scale * scalar_t((tmp1 >> 24) & 0x7) - zero) * blockvec[k + 8];
+    res += (scale * scalar_t((tmp1 >> 27) & 0x7) - zero) * blockvec[k + 9];
+	
+    i += width;
+    tmp2 = as_unsigned(mat[i]);
+    tmp = (tmp1 >> 30) | ((tmp2 << 2) & 0x4);
+    tmp2 >>= 1;
+    res += (scale * scalar_t(tmp) - zero) * blockvec[k + 10];
+    k += 11;
+	
+    res += (scale * scalar_t((tmp2 >>  0) & 0x7) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp2 >>  3) & 0x7) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp2 >>  6) & 0x7) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp2 >>  9) & 0x7) - zero) * blockvec[k + 3];
+    res += (scale * scalar_t((tmp2 >> 12) & 0x7) - zero) * blockvec[k + 4];
+    res += (scale * scalar_t((tmp2 >> 15) & 0x7) - zero) * blockvec[k + 5];
+    res += (scale * scalar_t((tmp2 >> 18) & 0x7) - zero) * blockvec[k + 6];
+    res += (scale * scalar_t((tmp2 >> 21) & 0x7) - zero) * blockvec[k + 7];
+    res += (scale * scalar_t((tmp2 >> 24) & 0x7) - zero) * blockvec[k + 8];
+    res += (scale * scalar_t((tmp2 >> 27) & 0x7) - zero) * blockvec[k + 9];
+	
+    i += width;
+    tmp1 = as_unsigned(mat[i]);
+    tmp = (tmp2 >> 30) | ((tmp1 << 1) & 0x6);
+    tmp1 >>= 2;
+    res += (scale * scalar_t(tmp) - zero) * blockvec[k + 10];
+    k += 11;
+	
+    res += (scale * scalar_t((tmp1 >>  0) & 0x7) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp1 >>  3) & 0x7) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp1 >>  6) & 0x7) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp1 >>  9) & 0x7) - zero) * blockvec[k + 3];
+    res += (scale * scalar_t((tmp1 >> 12) & 0x7) - zero) * blockvec[k + 4];
+    res += (scale * scalar_t((tmp1 >> 15) & 0x7) - zero) * blockvec[k + 5];
+    res += (scale * scalar_t((tmp1 >> 18) & 0x7) - zero) * blockvec[k + 6];
+    res += (scale * scalar_t((tmp1 >> 21) & 0x7) - zero) * blockvec[k + 7];
+    res += (scale * scalar_t((tmp1 >> 24) & 0x7) - zero) * blockvec[k + 8];
+    res += (scale * scalar_t((tmp1 >> 27) & 0x7) - zero) * blockvec[k + 9];
+	
+    i += width;
+    k += 10;
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+void vecquant4matmul_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant4matmul_cuda_old", ([&] {
+      VecQuant4MatMulKernel_old<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(),
+        batch, vec_height, height, width, zero_width, groupsize
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant4MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const       int* __restrict__ zeros,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT4 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+  __syncthreads();
+
+  scalar_t res = 0;
+  int i = width * h + w;
+  int g_h = h * 8;
+  int k = 0;
+
+  int z_w = w / 8; 
+  int z_mod = (w % 8) * 4;
+
+  unsigned int tmp;
+
+  while (k < BLOCKWIDTH) {
+    tmp = as_unsigned(mat[i]);
+	
+    int g = (g_h + k) / groupsize;
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1);
+	
+    res += (scale * scalar_t((tmp >> 0) & 0xF) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp >> 4) & 0xF) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp >> 8) & 0xF) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp >> 12) & 0xF) - zero) * blockvec[k + 3];
+    res += (scale * scalar_t((tmp >> 16) & 0xF) - zero) * blockvec[k + 4];
+    res += (scale * scalar_t((tmp >> 20) & 0xF) - zero) * blockvec[k + 5];
+    res += (scale * scalar_t((tmp >> 24) & 0xF) - zero) * blockvec[k + 6];
+    res += (scale * scalar_t((tmp >> 28) & 0xF) - zero) * blockvec[k + 7];
+	
+    i += width;
+    k += 8;
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+void vecquant8matmul_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT8 - 1) / BLOCKHEIGHT8,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant8matmul_cuda_old", ([&] {
+      VecQuant8MatMulKernel_old<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(),
+        batch, vec_height, height, width, zero_width, groupsize
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant8MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT8 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+  __syncthreads();
+
+  scalar_t res = 0;
+  int i = width * h + w;
+  int g_h = h * 4;
+  int k = 0;
+  
+  int z_w = w / 4; 
+  int z_mod = (w % 4) * 8;
+
+  unsigned int tmp;
+
+  while (k < BLOCKWIDTH) { 
+    tmp = as_unsigned(mat[i]);
+	
+    int g = (g_h + k) / groupsize;
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xFF) + 1);
+	
+    res += (scale * scalar_t((tmp >> 0) & 0xFF) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp >> 8) & 0xFF) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp >> 16) & 0xFF) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp >> 24) & 0xFF) - zero) * blockvec[k + 3];
+	
+    i += width;
+    k += 4;
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+
+void vecquant2matmul_faster_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize,
+  int vec_height
+) {
+  int batch = vec.size(0);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+  
+  dim3 blocks(
+    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  VecQuant2MatMulKernelFaster_old<<<blocks, threads>>>(
+    (half2*) vec.data_ptr(),
+    mat.data_ptr<int>(),
+    mul.data_ptr<float>(),
+    scales.data_ptr<float>(),
+    zeros.data_ptr<int>(),
+    batch, vec_height, height, width, zero_width, groupsize
+  );
+}
+
+__global__ void VecQuant2MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const  	 int* __restrict__ zeros,
+	int batch,
+	int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  const int blockwidth2 = BLOCKWIDTH / 2;
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT2 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ half2 blockvec[blockwidth2];
+  if (threadIdx.x < blockwidth2)
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
+
+  __shared__ half2 deq2[16][16];
+  int val = threadIdx.x / 16;
+  int off = threadIdx.x % 16;
+  for (; val < 16; val += BLOCKWIDTH / 16) {
+    deq2[val][off] = __halves2half2(
+       __int2half_rn(val & 0x3), __int2half_rn(val >> 2)
+    );
+  }
+
+  int i = width * h + w;
+  int g_h = h * 16;
+  int k = 0;
+  
+  int z_w = w / 16; 
+  int z_mod = (w % 16) * 2;
+
+  float res = 0;
+  half2 res2;
+
+  unsigned int tmp;
+
+  __syncthreads();
+
+  while (k < blockwidth2) {
+    int g = (g_h + (k * 2)) / groupsize;
+	float scale_f = scales[g * width + w];
+    half2 scale = __float2half2_rn(scale_f);
+    half2 zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0x3) + 1)));
+	
+    res2 = {};
+    tmp = as_unsigned(mat[i]);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  0) & 0xf][off], scale, zero), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  4) & 0xf][off], scale, zero), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  8) & 0xf][off], scale, zero), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 12) & 0xf][off], scale, zero), blockvec[k + 3], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 16) & 0xf][off], scale, zero), blockvec[k + 4], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 20) & 0xf][off], scale, zero), blockvec[k + 5], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 24) & 0xf][off], scale, zero), blockvec[k + 6], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 28) & 0xf][off], scale, zero), blockvec[k + 7], res2);
+	i += width;
+    k += 8;
+    res += __half2float(res2.x) + __half2float(res2.y);
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+void vecquant3matmul_faster_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize,
+  int vec_height
+) {
+  int batch = vec.size(0);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+  
+  dim3 blocks(
+    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  VecQuant3MatMulKernelFaster_old<<<blocks, threads>>>(
+    (half2*) vec.data_ptr(),
+    mat.data_ptr<int>(),
+    mul.data_ptr<float>(),
+    scales.data_ptr<float>(),
+    zeros.data_ptr<int>(),
+    batch, vec_height, height, width, zero_width, groupsize
+  );
+}
+
+__global__ void VecQuant3MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const  	 int* __restrict__ zeros,
+	int batch,
+	int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  const int blockwidth2 = BLOCKWIDTH / 2;
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT3 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ half2 blockvec[blockwidth2];
+  if (threadIdx.x < blockwidth2)
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
+
+  __shared__ half2 deq2[64][32];
+  int val = threadIdx.x / 32;
+  int off = threadIdx.x % 32;
+  for (; val < 64; val += BLOCKWIDTH / 32) {
+    deq2[val][off] = __halves2half2(
+       __int2half_rn(val & 0x7), __int2half_rn(val >> 3)
+    );
+  }
+
+  int i = width * h + w;
+  int g_h = (h / 3) * 32;
+  int k = 0;
+  
+  int z_w = (w / 32) * 3;
+  int z_mod = w % 32;
+  int z_bit;
+  
+  if (z_mod != 10){
+    if (z_mod != 21){
+      z_bit = z_mod;
+      if (z_bit > 21){
+        z_bit -= 22;
+        z_bit *= 3;
+        z_bit += 2;
+        z_w += 2;
+      } else if (z_bit > 10){
+        z_bit -= 11;
+        z_bit *= 3;
+        z_bit += 1;
+        z_w += 1;
+      } else {
+        z_bit *= 3;
+      }
+    } else {
+      z_w += 1;
+    }
+  }
+
+  float res = 0;
+  half2 res2;
+
+  unsigned int tmp1;
+  unsigned int tmp2;
+  unsigned int tmp;
+  unsigned int z_tmp;
+
+  __syncthreads();
+
+  while (k < blockwidth2) {
+    int g = (g_h + (k * 2)) / groupsize;
+	float scale_f = scales[g * width + w];
+    half2 scale = __float2half2_rn(scale_f);
+    half2 zero;
+    if (z_mod == 10) {
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
+      zero = __float2half2_rn(-(scale_f * ((z_tmp) + 1)));
+    } else if (z_mod == 21){
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
+      zero = __float2half2_rn(-(scale_f * ((z_tmp) + 1)));
+    } else {
+      zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1)));
+    }
+	
+    res2 = {};
+    tmp1 = as_unsigned(mat[i]);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 24) & 0x3f][off], scale, zero), blockvec[k + 4], res2);
+    i += width;
+    tmp2 = as_unsigned(mat[i]);
+    tmp = (tmp1 >> 30) | ((tmp2 << 2) & 0x3c);
+    res2 = __hfma2(__hfma2(deq2[tmp][off], scale, zero), blockvec[k + 5], res2);
+    tmp2 >>= 4;
+    k += 6;
+    res2 = __hfma2(__hfma2(deq2[(tmp2 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp2 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp2 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp2 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
+    i += width;
+    tmp1 = as_unsigned(mat[i]);
+    tmp = (tmp2 >> 24) | ((tmp1 << 4) & 0x30);
+    res2 = __hfma2(__hfma2(deq2[tmp][off], scale, zero), blockvec[k + 4], res2);
+    tmp1 >>= 2;
+    k += 5;
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 24) & 0x3f][off], scale, zero), blockvec[k + 4], res2);
+    i += width;
+    k += 5;
+    res += __half2float(res2.x) + __half2float(res2.y);
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+void vecquant4matmul_faster_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize,
+  int vec_height
+) {
+  int batch = vec.size(0);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+  
+  dim3 blocks(
+    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  VecQuant4MatMulKernelFaster_old<<<blocks, threads>>>(
+    (half2*) vec.data_ptr(),
+    mat.data_ptr<int>(),
+    mul.data_ptr<float>(),
+    scales.data_ptr<float>(),
+    zeros.data_ptr<int>(),
+    batch, vec_height, height, width, zero_width, groupsize
+  );
+}
+
+__global__ void VecQuant4MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const  	 int* __restrict__ zeros,
+	int batch,
+	int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  const int blockwidth2 = BLOCKWIDTH / 2;
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT4 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ half2 blockvec[blockwidth2];
+  if (threadIdx.x < blockwidth2)
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
+
+  __shared__ half2 deq2[256][8];
+  int val = threadIdx.x / 8;
+  int off = threadIdx.x % 8;
+  for (; val < 256; val += BLOCKWIDTH / 8) {
+    deq2[val][off] = __halves2half2(
+       __int2half_rn(val & 0xF), __int2half_rn(val >> 4)
+    );
+  }
+
+  int i = width * h + w;
+  int g_h = h * 8;
+  int k = 0;
+
+  int z_w = w / 8; 
+  int z_mod = (w % 8) * 4;
+
+  float res = 0;
+  half2 res2;
+
+  unsigned int tmp;
+
+  __syncthreads();
+
+  while (k < blockwidth2) {
+    int g = (g_h + (k * 2)) / groupsize;
+	float scale_f = scales[g * width + w];
+    half2 scale = __float2half2_rn(scale_f);
+    half2 zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1)));
+	
+    res2 = {};
+    tmp = as_unsigned(mat[i]);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  0) & 0xff][off], scale, zero), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  8) & 0xff][off], scale, zero), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 16) & 0xff][off], scale, zero), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 24) & 0xff][off], scale, zero), blockvec[k + 3], res2);
+	i += width;
+    k += 4;
+    res += __half2float(res2.x) + __half2float(res2.y);
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
```

### Comparing `auto_gptq-0.3.0/setup.py` & `auto_gptq-0.3.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,112 +1,115 @@
-import os
-import platform
-import sys
-from pathlib import Path
-from setuptools import setup, find_packages
-
-try:
-    import torch
-    TORCH_AVAILABLE = True
-except ImportError:
-    TORCH_AVAILABLE = False
-
-IN_GITHUB_ACTIONS = os.environ.get("GITHUB_ACTIONS", "false") == "true"
-
-python_min_version = (3, 8, 0)
-python_min_version_str = '.'.join(map(str, python_min_version))
-if sys.version_info < python_min_version:
-    print(f"You are using Python {platform.python_version()}. Python >={python_min_version_str} is required.")
-    sys.exit(-1)
-
-CUDA_VERSION = "".join(os.environ.get("CUDA_VERSION", "").split("."))
-
-version = "0.3.0" + (f"+cu{CUDA_VERSION}" if CUDA_VERSION and IN_GITHUB_ACTIONS else "")
-common_setup_kwargs = {
-    "version": version,
-    "name": "auto_gptq",
-    "author": "PanQiWei",
-    "description": "An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.",
-    "long_description": (Path(__file__).parent / "README.md").read_text(encoding="UTF-8"),
-    "long_description_content_type": "text/markdown",
-    "url": "https://github.com/PanQiWei/AutoGPTQ",
-    "keywords": ["gptq", "quantization", "large-language-models", "pytorch", "transformers"],
-    "platforms": ["windows", "linux"],
-    "classifiers": [
-        "Environment :: GPU :: NVIDIA CUDA :: 11.7",
-        "Environment :: GPU :: NVIDIA CUDA :: 11.8",
-        "License :: OSI Approved :: MIT License",
-        "Natural Language :: Chinese (Simplified)",
-        "Natural Language :: English",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: C++",
-    ],
-    "python_requires": f">={python_min_version_str}"
-}
-
-requirements = [
-    "accelerate>=0.19.0",
-    "datasets",
-    "numpy",
-    "rouge",
-    "torch>=1.13.0",
-    "safetensors",
-    "transformers>=4.29.0",
-    "peft"
-]
-
-extras_require = {
-    "triton": ["triton>=2.0.0"]
-}
-
-include_dirs = ["autogptq_cuda"]
-
-if TORCH_AVAILABLE:
-    BUILD_CUDA_EXT = int(os.environ.get('BUILD_CUDA_EXT', '1')) == 1
-    
-    additional_setup_kwargs = dict()
-    if BUILD_CUDA_EXT and (torch.cuda.is_available() or IN_GITHUB_ACTIONS):
-        from torch.utils import cpp_extension
-        from distutils.sysconfig import get_python_lib
-        conda_cuda_include_dir = os.path.join(get_python_lib(), "nvidia/cuda_runtime/include")
-        if os.path.isdir(conda_cuda_include_dir):
-            include_dirs.append(conda_cuda_include_dir)
-            print(f"appending conda cuda include dir {conda_cuda_include_dir}")
-        extensions = [
-            cpp_extension.CUDAExtension(
-                "autogptq_cuda_64",
-                [
-                    "autogptq_cuda/autogptq_cuda_64.cpp",
-                    "autogptq_cuda/autogptq_cuda_kernel_64.cu"
-                ]
-            ),
-            cpp_extension.CUDAExtension(
-                "autogptq_cuda_256",
-                [
-                    "autogptq_cuda/autogptq_cuda_256.cpp",
-                    "autogptq_cuda/autogptq_cuda_kernel_256.cu"
-                ]
-            )
-        ]
-
-        additional_setup_kwargs = {
-            "ext_modules": extensions,
-            "cmdclass": {'build_ext': cpp_extension.BuildExtension}
-        }
-    common_setup_kwargs.update(additional_setup_kwargs)
-    setup(
-        packages=find_packages(),
-        install_requires=requirements,
-        extras_require=extras_require,
-        include_dirs=include_dirs,
-        **common_setup_kwargs
-    )
-else:
-    setup(
-        packages=find_packages(),
-        install_requires=requirements,
-        extras_require=extras_require,
-        include_dirs=include_dirs,
-        **common_setup_kwargs
-    )
+import os
+import platform
+import sys
+from pathlib import Path
+from setuptools import setup, find_packages
+
+try:
+    import torch
+    TORCH_AVAILABLE = False
+except ImportError:
+    TORCH_AVAILABLE = False
+
+python_min_version = (3, 8, 0)
+python_min_version_str = '.'.join(map(str, python_min_version))
+if sys.version_info < python_min_version:
+    print(f"You are using Python {platform.python_version()}. Python >={python_min_version_str} is required.")
+    sys.exit(-1)
+
+if TORCH_AVAILABLE:
+    CUDA_VERSION = "".join(torch.version.cuda.split("."))
+else:
+    CUDA_VERSION = "".join(os.environ.get("CUDA_VERSION", "").split("."))
+
+common_setup_kwargs = {
+    "version": "0.3.1",
+    "name": "auto_gptq",
+    "author": "PanQiWei",
+    "description": "An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.",
+    "long_description": (Path(__file__).parent / "README.md").read_text(encoding="UTF-8"),
+    "long_description_content_type": "text/markdown",
+    "url": "https://github.com/PanQiWei/AutoGPTQ",
+    "keywords": ["gptq", "quantization", "large-language-models", "pytorch", "transformers"],
+    "platforms": ["windows", "linux"],
+    "classifiers": [
+        "Environment :: GPU :: NVIDIA CUDA :: 11.7",
+        "Environment :: GPU :: NVIDIA CUDA :: 11.8",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: Chinese (Simplified)",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: C++",
+    ],
+    "python_requires": f">={python_min_version_str}"
+}
+
+if CUDA_VERSION:
+    common_setup_kwargs['version'] += f"+cu{CUDA_VERSION}"
+
+requirements = [
+    "accelerate>=0.19.0",
+    "datasets",
+    "numpy",
+    "rouge",
+    "torch>=1.13.0",
+    "safetensors",
+    "transformers>=4.31.0",
+    "peft"
+]
+
+extras_require = {
+    "triton": ["triton>=2.0.0"]
+}
+
+include_dirs = ["autogptq_cuda"]
+
+if TORCH_AVAILABLE:
+    BUILD_CUDA_EXT = int(os.environ.get('BUILD_CUDA_EXT', '1')) == 1
+    
+    additional_setup_kwargs = dict()
+    if BUILD_CUDA_EXT:
+        from torch.utils import cpp_extension
+        from distutils.sysconfig import get_python_lib
+        conda_cuda_include_dir = os.path.join(get_python_lib(), "nvidia/cuda_runtime/include")
+        if os.path.isdir(conda_cuda_include_dir):
+            include_dirs.append(conda_cuda_include_dir)
+            print(f"appending conda cuda include dir {conda_cuda_include_dir}")
+        extensions = [
+            cpp_extension.CUDAExtension(
+                "autogptq_cuda_64",
+                [
+                    "autogptq_cuda/autogptq_cuda_64.cpp",
+                    "autogptq_cuda/autogptq_cuda_kernel_64.cu"
+                ]
+            ),
+            cpp_extension.CUDAExtension(
+                "autogptq_cuda_256",
+                [
+                    "autogptq_cuda/autogptq_cuda_256.cpp",
+                    "autogptq_cuda/autogptq_cuda_kernel_256.cu"
+                ]
+            )
+        ]
+
+        additional_setup_kwargs = {
+            "ext_modules": extensions,
+            "cmdclass": {'build_ext': cpp_extension.BuildExtension}
+        }
+    common_setup_kwargs.update(additional_setup_kwargs)
+    setup(
+        packages=find_packages(),
+        install_requires=requirements,
+        extras_require=extras_require,
+        include_dirs=include_dirs,
+        **common_setup_kwargs
+    )
+else:
+    setup(
+        packages=find_packages(),
+        install_requires=requirements,
+        extras_require=extras_require,
+        include_dirs=include_dirs,
+        **common_setup_kwargs
+    )
```

