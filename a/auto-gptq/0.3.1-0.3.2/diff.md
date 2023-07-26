# Comparing `tmp/auto_gptq-0.3.1.tar.gz` & `tmp/auto_gptq-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_gptq-0.3.1.tar", last modified: Wed Jul 26 10:22:07 2023, max compression
+gzip compressed data, was "auto_gptq-0.3.2.tar", last modified: Wed Jul 26 11:18:40 2023, max compression
```

## Comparing `auto_gptq-0.3.1.tar` & `auto_gptq-0.3.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.710516 auto_gptq-0.3.1/
--rw-r--r--   0 root         (0) root         (0)     1075 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    16691 2023-07-26 10:22:07.710516 auto_gptq-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15813 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.690516 auto_gptq-0.3.1/auto_gptq/
--rw-r--r--   0 root         (0) root         (0)      155 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.693516 auto_gptq-0.3.1/auto_gptq/eval_tasks/
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2194 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.693516 auto_gptq-0.3.1/auto_gptq/eval_tasks/_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/_utils/classification_utils.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/_utils/generation_utils.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/language_modeling_task.py
--rw-r--r--   0 root         (0) root         (0)     3653 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/sequence_classification_task.py
--rw-r--r--   0 root         (0) root         (0)     2571 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/eval_tasks/text_summarization_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.698516 auto_gptq-0.3.1/auto_gptq/modeling/
--rw-r--r--   0 root         (0) root         (0)      340 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/modeling/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41463 2023-07-26 10:21:12.000000 auto_gptq-0.3.1/auto_gptq/modeling/_base.py
--rw-r--r--   0 root         (0) root         (0)      535 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/modeling/_const.py
--rw-r--r--   0 root         (0) root         (0)     7181 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/modeling/_utils.py
--rw-r--r--   0 root         (0) root         (0)     4635 2023-07-26 10:21:12.000000 auto_gptq-0.3.1/auto_gptq/modeling/auto.py
--rw-r--r--   0 root         (0) root         (0)      414 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/modeling/baichuan.py
--rw-r--r--   0 root         (0) root         (0)      474 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/bloom.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/codegen.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/gpt2.py
--rw-r--r--   0 root         (0) root         (0)      453 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/gpt_bigcode.py
--rw-r--r--   0 root         (0) root         (0)      461 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/gpt_neox.py
--rw-r--r--   0 root         (0) root         (0)      550 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/gptj.py
--rw-r--r--   0 root         (0) root         (0)      463 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/modeling/internlm.py
--rw-r--r--   0 root         (0) root         (0)     1011 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/llama.py
--rw-r--r--   0 root         (0) root         (0)      379 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/moss.py
--rw-r--r--   0 root         (0) root         (0)      562 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/opt.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/modeling/rw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.700516 auto_gptq-0.3.1/auto_gptq/nn_modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/_fused_base.py
--rw-r--r--   0 root         (0) root         (0)    11043 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/fused_gptj_attn.py
--rw-r--r--   0 root         (0) root         (0)     7489 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/fused_llama_attn.py
--rw-r--r--   0 root         (0) root         (0)    11870 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/fused_llama_mlp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.702516 auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/
--rw-r--r--   0 root         (0) root         (0)     2054 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11136 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/qlinear_cuda.py
--rw-r--r--   0 root         (0) root         (0)    11551 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/qlinear_cuda_old.py
--rw-r--r--   0 root         (0) root         (0)     6352 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/qlinear_triton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.703516 auto_gptq-0.3.1/auto_gptq/nn_modules/triton_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/triton_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6925 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/triton_utils/custom_autotune.py
--rw-r--r--   0 root         (0) root         (0)    13883 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/triton_utils/kernels.py
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/nn_modules/triton_utils/mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.704516 auto_gptq-0.3.1/auto_gptq/quantization/
--rw-r--r--   0 root         (0) root         (0)       45 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/quantization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5835 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/quantization/gptq.py
--rw-r--r--   0 root         (0) root         (0)     4271 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/quantization/quantizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.706516 auto_gptq-0.3.1/auto_gptq/utils/
--rw-r--r--   0 root         (0) root         (0)       40 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/auto_gptq/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11122 2023-06-07 03:56:07.000000 auto_gptq-0.3.1/auto_gptq/utils/data_utils.py
--rw-r--r--   0 root         (0) root         (0)     1192 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/utils/import_utils.py
--rw-r--r--   0 root         (0) root         (0)    18265 2023-06-08 06:11:00.000000 auto_gptq-0.3.1/auto_gptq/utils/peft_utils.py
--rw-r--r--   0 root         (0) root         (0)     7098 2023-07-26 10:21:12.000000 auto_gptq-0.3.1/auto_gptq/utils/perplexity_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.691516 auto_gptq-0.3.1/auto_gptq.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16691 2023-07-26 10:22:07.000000 auto_gptq-0.3.1/auto_gptq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2023 2023-07-26 10:22:07.000000 auto_gptq-0.3.1/auto_gptq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 10:22:07.000000 auto_gptq-0.3.1/auto_gptq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-07-26 10:22:07.000000 auto_gptq-0.3.1/auto_gptq.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-26 10:22:07.000000 auto_gptq-0.3.1/auto_gptq.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:22:07.708516 auto_gptq-0.3.1/autogptq_cuda/
--rw-r--r--   0 root         (0) root         (0)     6499 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_256.cpp
--rw-r--r--   0 root         (0) root         (0)     6499 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_64.cpp
--rw-r--r--   0 root         (0) root         (0)    40941 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_kernel_256.cu
--rw-r--r--   0 root         (0) root         (0)    40938 2023-07-26 07:26:39.000000 auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_kernel_64.cu
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 10:22:07.710516 auto_gptq-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3695 2023-07-26 10:21:39.000000 auto_gptq-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:18:40.371329 auto_gptq-0.3.2/
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    16691 2023-07-26 11:18:40.371329 auto_gptq-0.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15813 2023-07-26 07:26:39.000000 auto_gptq-0.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:18:40.363330 auto_gptq-0.3.2/auto_gptq/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-26 10:40:53.000000 auto_gptq-0.3.2/auto_gptq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:18:40.365329 auto_gptq-0.3.2/auto_gptq/eval_tasks/
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/eval_tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/eval_tasks/_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:18:40.365329 auto_gptq-0.3.2/auto_gptq/eval_tasks/_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/eval_tasks/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/eval_tasks/_utils/classification_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/eval_tasks/_utils/generation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/eval_tasks/language_modeling_task.py
+-rw-r--r--   0 root         (0) root         (0)     3653 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/eval_tasks/sequence_classification_task.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/eval_tasks/text_summarization_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:18:40.367329 auto_gptq-0.3.2/auto_gptq/modeling/
+-rw-r--r--   0 root         (0) root         (0)      340 2023-07-26 07:26:39.000000 auto_gptq-0.3.2/auto_gptq/modeling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41463 2023-07-26 10:21:12.000000 auto_gptq-0.3.2/auto_gptq/modeling/_base.py
+-rw-r--r--   0 root         (0) root         (0)      535 2023-07-26 07:26:39.000000 auto_gptq-0.3.2/auto_gptq/modeling/_const.py
+-rw-r--r--   0 root         (0) root         (0)     7181 2023-06-08 06:11:00.000000 auto_gptq-0.3.2/auto_gptq/modeling/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-07-26 10:21:12.000000 auto_gptq-0.3.2/auto_gptq/modeling/auto.py
+-rw-r--r--   0 root         (0) root         (0)      414 2023-07-26 07:26:39.000000 auto_gptq-0.3.2/auto_gptq/modeling/baichuan.py
+-rw-r--r--   0 root         (0) root         (0)      474 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/modeling/bloom.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/modeling/codegen.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/modeling/gpt2.py
+-rw-r--r--   0 root         (0) root         (0)      453 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/modeling/gpt_bigcode.py
+-rw-r--r--   0 root         (0) root         (0)      461 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/modeling/gpt_neox.py
+-rw-r--r--   0 root         (0) root         (0)      550 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/modeling/gptj.py
+-rw-r--r--   0 root         (0) root         (0)      463 2023-07-26 07:26:39.000000 auto_gptq-0.3.2/auto_gptq/modeling/internlm.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/modeling/llama.py
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/modeling/moss.py
+-rw-r--r--   0 root         (0) root         (0)      562 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/modeling/opt.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/modeling/rw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:18:40.368329 auto_gptq-0.3.2/auto_gptq/nn_modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/nn_modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-06-08 06:11:00.000000 auto_gptq-0.3.2/auto_gptq/nn_modules/_fused_base.py
+-rw-r--r--   0 root         (0) root         (0)    11043 2023-06-08 06:11:00.000000 auto_gptq-0.3.2/auto_gptq/nn_modules/fused_gptj_attn.py
+-rw-r--r--   0 root         (0) root         (0)     7489 2023-06-08 06:11:00.000000 auto_gptq-0.3.2/auto_gptq/nn_modules/fused_llama_attn.py
+-rw-r--r--   0 root         (0) root         (0)    11870 2023-06-08 06:11:00.000000 auto_gptq-0.3.2/auto_gptq/nn_modules/fused_llama_mlp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:18:40.369329 auto_gptq-0.3.2/auto_gptq/nn_modules/qlinear/
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-06-08 06:11:00.000000 auto_gptq-0.3.2/auto_gptq/nn_modules/qlinear/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11136 2023-07-26 07:26:39.000000 auto_gptq-0.3.2/auto_gptq/nn_modules/qlinear/qlinear_cuda.py
+-rw-r--r--   0 root         (0) root         (0)    11551 2023-07-26 07:26:39.000000 auto_gptq-0.3.2/auto_gptq/nn_modules/qlinear/qlinear_cuda_old.py
+-rw-r--r--   0 root         (0) root         (0)     6352 2023-07-26 07:26:39.000000 auto_gptq-0.3.2/auto_gptq/nn_modules/qlinear/qlinear_triton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:18:40.369329 auto_gptq-0.3.2/auto_gptq/nn_modules/triton_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/nn_modules/triton_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6925 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/nn_modules/triton_utils/custom_autotune.py
+-rw-r--r--   0 root         (0) root         (0)    13883 2023-06-08 06:11:00.000000 auto_gptq-0.3.2/auto_gptq/nn_modules/triton_utils/kernels.py
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/nn_modules/triton_utils/mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:18:40.370329 auto_gptq-0.3.2/auto_gptq/quantization/
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/quantization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5835 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/quantization/gptq.py
+-rw-r--r--   0 root         (0) root         (0)     4271 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/quantization/quantizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:18:40.370329 auto_gptq-0.3.2/auto_gptq/utils/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-26 07:26:39.000000 auto_gptq-0.3.2/auto_gptq/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11122 2023-06-07 03:56:07.000000 auto_gptq-0.3.2/auto_gptq/utils/data_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-06-08 06:11:00.000000 auto_gptq-0.3.2/auto_gptq/utils/import_utils.py
+-rw-r--r--   0 root         (0) root         (0)    18265 2023-06-08 06:11:00.000000 auto_gptq-0.3.2/auto_gptq/utils/peft_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7098 2023-07-26 10:21:12.000000 auto_gptq-0.3.2/auto_gptq/utils/perplexity_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:18:40.364329 auto_gptq-0.3.2/auto_gptq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16691 2023-07-26 11:18:40.000000 auto_gptq-0.3.2/auto_gptq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2023 2023-07-26 11:18:40.000000 auto_gptq-0.3.2/auto_gptq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 11:18:40.000000 auto_gptq-0.3.2/auto_gptq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-26 11:18:40.000000 auto_gptq-0.3.2/auto_gptq.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-26 11:18:40.000000 auto_gptq-0.3.2/auto_gptq.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:18:40.371329 auto_gptq-0.3.2/autogptq_cuda/
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-07-26 07:26:39.000000 auto_gptq-0.3.2/autogptq_cuda/autogptq_cuda_256.cpp
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-07-26 07:26:39.000000 auto_gptq-0.3.2/autogptq_cuda/autogptq_cuda_64.cpp
+-rw-r--r--   0 root         (0) root         (0)    40941 2023-07-26 07:26:39.000000 auto_gptq-0.3.2/autogptq_cuda/autogptq_cuda_kernel_256.cu
+-rw-r--r--   0 root         (0) root         (0)    40938 2023-07-26 07:26:39.000000 auto_gptq-0.3.2/autogptq_cuda/autogptq_cuda_kernel_64.cu
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 11:18:40.371329 auto_gptq-0.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3355 2023-07-26 11:18:23.000000 auto_gptq-0.3.2/setup.py
```

### Comparing `auto_gptq-0.3.1/LICENSE` & `auto_gptq-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/PKG-INFO` & `auto_gptq-0.3.2/auto_gptq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: auto_gptq
-Version: 0.3.1
+Name: auto-gptq
+Version: 0.3.2
 Summary: An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
 Home-page: https://github.com/PanQiWei/AutoGPTQ
 Author: PanQiWei
 Keywords: gptq,quantization,large-language-models,pytorch,transformers
 Platform: windows
 Platform: linux
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auto_gptq Version: 0.3.1 Summary: An easy-to-use
+Metadata-Version: 2.1 Name: auto-gptq Version: 0.3.2 Summary: An easy-to-use
 LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
 Home-page: https://github.com/PanQiWei/AutoGPTQ Author: PanQiWei Keywords:
 gptq,quantization,large-language-models,pytorch,transformers Platform: windows
 Platform: linux Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8 Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: Chinese
 (Simplified) Classifier: Natural Language :: English Classifier: Programming
```

### Comparing `auto_gptq-0.3.1/README.md` & `auto_gptq-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/eval_tasks/_base.py` & `auto_gptq-0.3.2/auto_gptq/eval_tasks/_base.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/eval_tasks/_utils/classification_utils.py` & `auto_gptq-0.3.2/auto_gptq/eval_tasks/_utils/classification_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/eval_tasks/_utils/generation_utils.py` & `auto_gptq-0.3.2/auto_gptq/eval_tasks/_utils/generation_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/eval_tasks/language_modeling_task.py` & `auto_gptq-0.3.2/auto_gptq/eval_tasks/language_modeling_task.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/eval_tasks/sequence_classification_task.py` & `auto_gptq-0.3.2/auto_gptq/eval_tasks/sequence_classification_task.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/eval_tasks/text_summarization_task.py` & `auto_gptq-0.3.2/auto_gptq/eval_tasks/text_summarization_task.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/modeling/_base.py` & `auto_gptq-0.3.2/auto_gptq/modeling/_base.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/modeling/_const.py` & `auto_gptq-0.3.2/auto_gptq/modeling/_const.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/modeling/_utils.py` & `auto_gptq-0.3.2/auto_gptq/modeling/_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/modeling/auto.py` & `auto_gptq-0.3.2/auto_gptq/modeling/auto.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/modeling/gptj.py` & `auto_gptq-0.3.2/auto_gptq/modeling/gptj.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/modeling/llama.py` & `auto_gptq-0.3.2/auto_gptq/modeling/llama.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/modeling/opt.py` & `auto_gptq-0.3.2/auto_gptq/modeling/opt.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/nn_modules/_fused_base.py` & `auto_gptq-0.3.2/auto_gptq/nn_modules/_fused_base.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/nn_modules/fused_gptj_attn.py` & `auto_gptq-0.3.2/auto_gptq/nn_modules/fused_gptj_attn.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/nn_modules/fused_llama_attn.py` & `auto_gptq-0.3.2/auto_gptq/nn_modules/fused_llama_attn.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/nn_modules/fused_llama_mlp.py` & `auto_gptq-0.3.2/auto_gptq/nn_modules/fused_llama_mlp.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/__init__.py` & `auto_gptq-0.3.2/auto_gptq/nn_modules/qlinear/__init__.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/qlinear_cuda.py` & `auto_gptq-0.3.2/auto_gptq/nn_modules/qlinear/qlinear_cuda.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/qlinear_cuda_old.py` & `auto_gptq-0.3.2/auto_gptq/nn_modules/qlinear/qlinear_cuda_old.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/nn_modules/qlinear/qlinear_triton.py` & `auto_gptq-0.3.2/auto_gptq/nn_modules/qlinear/qlinear_triton.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/nn_modules/triton_utils/custom_autotune.py` & `auto_gptq-0.3.2/auto_gptq/nn_modules/triton_utils/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/nn_modules/triton_utils/kernels.py` & `auto_gptq-0.3.2/auto_gptq/nn_modules/triton_utils/kernels.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/quantization/gptq.py` & `auto_gptq-0.3.2/auto_gptq/quantization/gptq.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/quantization/quantizer.py` & `auto_gptq-0.3.2/auto_gptq/quantization/quantizer.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/utils/data_utils.py` & `auto_gptq-0.3.2/auto_gptq/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/utils/import_utils.py` & `auto_gptq-0.3.2/auto_gptq/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/utils/peft_utils.py` & `auto_gptq-0.3.2/auto_gptq/utils/peft_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq/utils/perplexity_utils.py` & `auto_gptq-0.3.2/auto_gptq/utils/perplexity_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/auto_gptq.egg-info/PKG-INFO` & `auto_gptq-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: auto-gptq
-Version: 0.3.1
+Name: auto_gptq
+Version: 0.3.2
 Summary: An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
 Home-page: https://github.com/PanQiWei/AutoGPTQ
 Author: PanQiWei
 Keywords: gptq,quantization,large-language-models,pytorch,transformers
 Platform: windows
 Platform: linux
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auto-gptq Version: 0.3.1 Summary: An easy-to-use
+Metadata-Version: 2.1 Name: auto_gptq Version: 0.3.2 Summary: An easy-to-use
 LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
 Home-page: https://github.com/PanQiWei/AutoGPTQ Author: PanQiWei Keywords:
 gptq,quantization,large-language-models,pytorch,transformers Platform: windows
 Platform: linux Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8 Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: Chinese
 (Simplified) Classifier: Natural Language :: English Classifier: Programming
```

### Comparing `auto_gptq-0.3.1/auto_gptq.egg-info/SOURCES.txt` & `auto_gptq-0.3.2/auto_gptq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_256.cpp` & `auto_gptq-0.3.2/autogptq_cuda/autogptq_cuda_256.cpp`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_64.cpp` & `auto_gptq-0.3.2/autogptq_cuda/autogptq_cuda_64.cpp`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_kernel_256.cu` & `auto_gptq-0.3.2/autogptq_cuda/autogptq_cuda_kernel_256.cu`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/autogptq_cuda/autogptq_cuda_kernel_64.cu` & `auto_gptq-0.3.2/autogptq_cuda/autogptq_cuda_kernel_64.cu`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.3.1/setup.py` & `auto_gptq-0.3.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import os
 import platform
 import sys
 from pathlib import Path
 from setuptools import setup, find_packages
 
-try:
-    import torch
-    TORCH_AVAILABLE = False
-except ImportError:
-    TORCH_AVAILABLE = False
-
 python_min_version = (3, 8, 0)
 python_min_version_str = '.'.join(map(str, python_min_version))
 if sys.version_info < python_min_version:
     print(f"You are using Python {platform.python_version()}. Python >={python_min_version_str} is required.")
     sys.exit(-1)
 
-if TORCH_AVAILABLE:
+BUILD_CUDA_EXT = int(os.environ.get('BUILD_CUDA_EXT', '1')) == 1
+
+if BUILD_CUDA_EXT:
+    try:
+        import torch
+    except:
+        print("torch is not installed, please install torch first!")
+        sys.exit(-1)
     CUDA_VERSION = "".join(torch.version.cuda.split("."))
 else:
     CUDA_VERSION = "".join(os.environ.get("CUDA_VERSION", "").split("."))
 
 common_setup_kwargs = {
-    "version": "0.3.1",
+    "version": "0.3.2",
     "name": "auto_gptq",
     "author": "PanQiWei",
     "description": "An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.",
     "long_description": (Path(__file__).parent / "README.md").read_text(encoding="UTF-8"),
     "long_description_content_type": "text/markdown",
     "url": "https://github.com/PanQiWei/AutoGPTQ",
     "keywords": ["gptq", "quantization", "large-language-models", "pytorch", "transformers"],
@@ -61,55 +62,44 @@
 
 extras_require = {
     "triton": ["triton>=2.0.0"]
 }
 
 include_dirs = ["autogptq_cuda"]
 
-if TORCH_AVAILABLE:
-    BUILD_CUDA_EXT = int(os.environ.get('BUILD_CUDA_EXT', '1')) == 1
-    
-    additional_setup_kwargs = dict()
-    if BUILD_CUDA_EXT:
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
+additional_setup_kwargs = dict()
+if BUILD_CUDA_EXT:
+    from torch.utils import cpp_extension
+    from distutils.sysconfig import get_python_lib
+    conda_cuda_include_dir = os.path.join(get_python_lib(), "nvidia/cuda_runtime/include")
+    if os.path.isdir(conda_cuda_include_dir):
+        include_dirs.append(conda_cuda_include_dir)
+        print(f"appending conda cuda include dir {conda_cuda_include_dir}")
+    extensions = [
+        cpp_extension.CUDAExtension(
+            "autogptq_cuda_64",
+            [
+                "autogptq_cuda/autogptq_cuda_64.cpp",
+                "autogptq_cuda/autogptq_cuda_kernel_64.cu"
+            ]
+        ),
+        cpp_extension.CUDAExtension(
+            "autogptq_cuda_256",
+            [
+                "autogptq_cuda/autogptq_cuda_256.cpp",
+                "autogptq_cuda/autogptq_cuda_kernel_256.cu"
+            ]
+        )
+    ]
+
+    additional_setup_kwargs = {
+        "ext_modules": extensions,
+        "cmdclass": {'build_ext': cpp_extension.BuildExtension}
+    }
+common_setup_kwargs.update(additional_setup_kwargs)
+setup(
+    packages=find_packages(),
+    install_requires=requirements,
+    extras_require=extras_require,
+    include_dirs=include_dirs,
+    **common_setup_kwargs
+)
```

