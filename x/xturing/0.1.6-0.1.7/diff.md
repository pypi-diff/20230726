# Comparing `tmp/xturing-0.1.6.tar.gz` & `tmp/xturing-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xturing-0.1.6.tar", last modified: Wed Jul 12 11:45:19 2023, max compression
+gzip compressed data, was "xturing-0.1.7.tar", last modified: Wed Jul 26 17:34:50 2023, max compression
```

## Comparing `xturing-0.1.6.tar` & `xturing-0.1.7.tar`

### file list

```diff
@@ -1,122 +1,126 @@
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.369494 xturing-0.1.6/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    11357 2023-06-13 13:40:44.000000 xturing-0.1.6/LICENSE
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       34 2023-06-13 13:40:44.000000 xturing-0.1.6/MANIFEST.in
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    22233 2023-07-12 11:45:19.369494 xturing-0.1.6/PKG-INFO
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     7771 2023-07-12 11:43:55.000000 xturing-0.1.6/README.md
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2216 2023-07-12 11:43:55.000000 xturing-0.1.6/pyproject.toml
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       38 2023-07-12 11:45:19.369494 xturing-0.1.6/setup.cfg
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.337494 xturing-0.1.6/src/
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.341494 xturing-0.1.6/src/xturing/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       22 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/__about__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      438 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/__init__.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.345494 xturing-0.1.6/src/xturing/cli/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      561 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/cli/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2042 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/cli/api.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      989 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/cli/chat.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      131 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/cli/ui.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.345494 xturing-0.1.6/src/xturing/config/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      569 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/config/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      972 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/config/config_data_classes.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4091 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/config/finetuning_config.yaml
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3205 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/config/generation_config.yaml
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1892 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/config/read_config.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.349494 xturing-0.1.6/src/xturing/datasets/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      436 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/datasets/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      199 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/datasets/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8197 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/datasets/instruction_dataset.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      222 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/datasets/text2image_dataset.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/datasets/text_dataset.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.349494 xturing-0.1.6/src/xturing/engines/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4254 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      272 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1871 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/bloom_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     9748 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/causal.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1923 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/cerebras_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      804 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/distilgpt2_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2986 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/falcon_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1755 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/galactica_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2310 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/generic_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1446 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/gpt2_engine.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2885 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/gptj_engine.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.353494 xturing-0.1.6/src/xturing/engines/gptj_utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/gptj_utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8053 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/gptj_utils/gptj.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6227 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/llama_engine.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.353494 xturing-0.1.6/src/xturing/engines/llama_utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       65 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/llama_utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    44506 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/llama_utils/llama.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.353494 xturing-0.1.6/src/xturing/engines/lora_engine/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       73 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/lora_engine/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    47142 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/lora_engine/lora.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3556 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/lora_engine/save_and_load.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/lora_engine/test.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/opt_engine.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.357494 xturing-0.1.6/src/xturing/engines/quant_utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       59 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/quant_utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2768 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/quant_utils/cachedistillationoutputs.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8651 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/quant_utils/custom_autotune.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    15980 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/quant_utils/lrec.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    12996 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/quant_utils/peft_utils.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2862 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/engines/quant_utils/qerdataloading.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    28505 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/engines/quant_utils/quant.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.357494 xturing-0.1.6/src/xturing/model_apis/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      864 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/model_apis/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1827 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/model_apis/ai21.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      573 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/model_apis/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1847 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/model_apis/cohere.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4600 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/model_apis/openai.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.361494 xturing-0.1.6/src/xturing/models/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3484 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/models/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2248 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/models/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1084 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/bloom.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     8858 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/models/causal.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1135 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/cerebras.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      579 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/distilgpt2.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1373 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/models/falcon.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1152 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/galactica.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2851 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/models/generic.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1033 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/gpt2.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1067 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/gptj.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2331 2023-07-12 11:43:55.000000 xturing-0.1.6/src/xturing/models/llama.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1050 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/opt.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      808 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/models/stable_diffusion.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.361494 xturing-0.1.6/src/xturing/preprocessors/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      137 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/preprocessors/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      484 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/preprocessors/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4582 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/preprocessors/instruction_collator.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2252 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/preprocessors/text_collator.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      642 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/registry.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.365494 xturing-0.1.6/src/xturing/self_instruct/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     9891 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/bootstrap_instructions.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     5490 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/generate_instances.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3737 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/identify_if_classification.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    14280 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/prepare_for_finetuning.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2198 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/prepare_seed_tasks.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.365494 xturing-0.1.6/src/xturing/self_instruct/templates/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3580 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/templates/clf_task_template.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    12674 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/self_instruct/templates/instance_gen_template.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.365494 xturing-0.1.6/src/xturing/trainers/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       78 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/trainers/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      233 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/trainers/base.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6265 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/trainers/lightning_trainer.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.365494 xturing-0.1.6/src/xturing/ui/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/ui/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    13685 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/ui/playground.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.369494 xturing-0.1.6/src/xturing/utils/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/__init__.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      215 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/external_loggers.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3117 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/hub.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      304 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/interactive.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     2147 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/logging.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      621 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/loss_fns.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     1366 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/notebooks.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     6886 2023-06-13 13:40:45.000000 xturing-0.1.6/src/xturing/utils/text_splitter.py
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     4034 2023-06-14 11:34:56.000000 xturing-0.1.6/src/xturing/utils/utils.py
-drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-12 11:45:19.341494 xturing-0.1.6/src/xturing.egg-info/
--rw-rw-r--   0 marcos    (1000) marcos    (1000)    22233 2023-07-12 11:45:19.000000 xturing-0.1.6/src/xturing.egg-info/PKG-INFO
--rw-rw-r--   0 marcos    (1000) marcos    (1000)     3531 2023-07-12 11:45:19.000000 xturing-0.1.6/src/xturing.egg-info/SOURCES.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        1 2023-07-12 11:45:19.000000 xturing-0.1.6/src/xturing.egg-info/dependency_links.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)       48 2023-07-12 11:45:19.000000 xturing-0.1.6/src/xturing.egg-info/entry_points.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)      243 2023-07-12 11:45:19.000000 xturing-0.1.6/src/xturing.egg-info/requires.txt
--rw-rw-r--   0 marcos    (1000) marcos    (1000)        8 2023-07-12 11:45:19.000000 xturing-0.1.6/src/xturing.egg-info/top_level.txt
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.744199 xturing-0.1.7/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    11357 2023-06-13 13:40:44.000000 xturing-0.1.7/LICENSE
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       34 2023-06-13 13:40:44.000000 xturing-0.1.7/MANIFEST.in
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    24340 2023-07-26 17:34:50.744199 xturing-0.1.7/PKG-INFO
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     9878 2023-07-26 16:08:06.000000 xturing-0.1.7/README.md
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2216 2023-07-26 17:29:58.000000 xturing-0.1.7/pyproject.toml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       38 2023-07-26 17:34:50.744199 xturing-0.1.7/setup.cfg
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.708199 xturing-0.1.7/src/
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.728199 xturing-0.1.7/src/xturing/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       22 2023-07-26 17:29:58.000000 xturing-0.1.7/src/xturing/__about__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      438 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/__init__.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.728199 xturing-0.1.7/src/xturing/cli/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      561 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/cli/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2042 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/cli/api.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      977 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/cli/chat.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      131 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/cli/ui.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.732199 xturing-0.1.7/src/xturing/config/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      569 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/config/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      972 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/config/config_data_classes.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4627 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/config/finetuning_config.yaml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3639 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/config/generation_config.yaml
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1926 2023-07-26 17:31:38.000000 xturing-0.1.7/src/xturing/config/read_config.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.732199 xturing-0.1.7/src/xturing/datasets/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      513 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/datasets/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      199 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/datasets/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8187 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/datasets/instruction_dataset.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      222 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/datasets/text2image_dataset.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1830 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/datasets/text_dataset.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.732199 xturing-0.1.7/src/xturing/engines/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4604 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/engines/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      272 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/engines/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1871 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/engines/bloom_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     9747 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/engines/causal.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1923 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/engines/cerebras_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      804 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/engines/distilgpt2_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2986 2023-07-12 11:43:55.000000 xturing-0.1.7/src/xturing/engines/falcon_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1755 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/engines/galactica_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2300 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/engines/generic_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1446 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/engines/gpt2_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2885 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/engines/gptj_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.736199 xturing-0.1.7/src/xturing/engines/gptj_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/engines/gptj_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8053 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/engines/gptj_utils/gptj.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2772 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/engines/llama2_engine.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4673 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/engines/llama_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.736199 xturing-0.1.7/src/xturing/engines/llama_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      109 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/engines/llama_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    44414 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/engines/llama_utils/llama.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.736199 xturing-0.1.7/src/xturing/engines/lora_engine/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      117 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/engines/lora_engine/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    47142 2023-07-12 11:43:55.000000 xturing-0.1.7/src/xturing/engines/lora_engine/lora.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3556 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/engines/lora_engine/save_and_load.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/engines/lora_engine/test.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1820 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/engines/opt_engine.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.736199 xturing-0.1.7/src/xturing/engines/quant_utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       87 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/engines/quant_utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2768 2023-07-12 11:43:55.000000 xturing-0.1.7/src/xturing/engines/quant_utils/cachedistillationoutputs.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     8651 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/engines/quant_utils/custom_autotune.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    15980 2023-07-12 11:43:55.000000 xturing-0.1.7/src/xturing/engines/quant_utils/lrec.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    12996 2023-07-12 11:43:55.000000 xturing-0.1.7/src/xturing/engines/quant_utils/peft_utils.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2862 2023-07-12 11:43:55.000000 xturing-0.1.7/src/xturing/engines/quant_utils/qerdataloading.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    28505 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/engines/quant_utils/quant.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.736199 xturing-0.1.7/src/xturing/model_apis/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1008 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/model_apis/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1827 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/model_apis/ai21.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      573 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/model_apis/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1847 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/model_apis/cohere.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4600 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/model_apis/openai.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.740199 xturing-0.1.7/src/xturing/models/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3839 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/models/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2248 2023-07-12 11:43:55.000000 xturing-0.1.7/src/xturing/models/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1084 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/models/bloom.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    12794 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/models/causal.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1135 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/models/cerebras.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      592 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/models/distilgpt2.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1373 2023-07-12 11:43:55.000000 xturing-0.1.7/src/xturing/models/falcon.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1152 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/models/galactica.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2851 2023-07-12 11:43:55.000000 xturing-0.1.7/src/xturing/models/generic.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1067 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/models/gpt2.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1067 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/models/gptj.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2030 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/models/llama.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1373 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/models/llama2.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1050 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/models/opt.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      808 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/models/stable_diffusion.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.740199 xturing-0.1.7/src/xturing/preprocessors/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      200 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/preprocessors/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      424 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/preprocessors/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4582 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/preprocessors/instruction_collator.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2252 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/preprocessors/text_collator.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      636 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/registry.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.740199 xturing-0.1.7/src/xturing/self_instruct/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/self_instruct/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     9881 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/self_instruct/bootstrap_instructions.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     5480 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/self_instruct/generate_instances.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3727 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/self_instruct/identify_if_classification.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    14270 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/self_instruct/prepare_for_finetuning.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2163 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/self_instruct/prepare_seed_tasks.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.740199 xturing-0.1.7/src/xturing/self_instruct/templates/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3580 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/self_instruct/templates/clf_task_template.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    12674 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/self_instruct/templates/instance_gen_template.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.740199 xturing-0.1.7/src/xturing/trainers/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      110 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/trainers/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      233 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/trainers/base.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6221 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/trainers/lightning_trainer.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.740199 xturing-0.1.7/src/xturing/ui/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/ui/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    13685 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/ui/playground.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.744199 xturing-0.1.7/src/xturing/utils/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        0 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/utils/__init__.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      215 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/utils/external_loggers.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3117 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/utils/hub.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      304 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/utils/interactive.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2147 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/utils/logging.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      621 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/utils/loss_fns.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1721 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/utils/metrics.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     1366 2023-06-13 13:40:45.000000 xturing-0.1.7/src/xturing/utils/notebooks.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     2247 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/utils/prompt.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     6801 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/utils/text_splitter.py
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     4540 2023-07-26 16:08:06.000000 xturing-0.1.7/src/xturing/utils/utils.py
+drwxrwxr-x   0 marcos    (1000) marcos    (1000)        0 2023-07-26 17:34:50.728199 xturing-0.1.7/src/xturing.egg-info/
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)    24340 2023-07-26 17:34:50.000000 xturing-0.1.7/src/xturing.egg-info/PKG-INFO
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)     3654 2023-07-26 17:34:50.000000 xturing-0.1.7/src/xturing.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        1 2023-07-26 17:34:50.000000 xturing-0.1.7/src/xturing.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)       48 2023-07-26 17:34:50.000000 xturing-0.1.7/src/xturing.egg-info/entry_points.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)      243 2023-07-26 17:34:50.000000 xturing-0.1.7/src/xturing.egg-info/requires.txt
+-rw-rw-r--   0 marcos    (1000) marcos    (1000)        8 2023-07-26 17:34:50.000000 xturing-0.1.7/src/xturing.egg-info/top_level.txt
```

### Comparing `xturing-0.1.6/LICENSE` & `xturing-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/PKG-INFO` & `xturing-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.1.6
+Version: 0.1.7
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -259,19 +259,79 @@
 - Explore different fine-tuning methods and benchmark them to find the best performing model
 - Evaluate fine-tuned models on well-defined metrics for in-depth analysis
 
 <br>
 
 ## 🌟 What's new?
 We are excited to announce the latest enhancements to our `xTuring` library:
-1. __`Falcon LLM` integration__ - You can use and fine-tune the _`Falcon-7B`_ model in different configurations: _off-the-shelf_, _off-the-shelf with INT8 precision_, _LoRA fine-tuning_, and _LoRA fine-tuning with INT8 precision_.
-2. __`GenericModel` wrapper__ - This new integration allows you to test and fine-tune any new model on `xTuring` without waiting for it to be integrated using class _`GenericModel`_.
+1. __`LLaMA 2` integration__ - You can use and fine-tune the _`LLaMA 2`_ model in different configurations: _off-the-shelf_, _off-the-shelf with INT8 precision_, _LoRA fine-tuning_, _LoRA fine-tuning with INT8 precision_ and _LoRA fine-tuning with INT4 precision_ using the `GenericModel` wrapper and/or you can use the `Llama2` class from `xturing.models` to test and finetune the model.
+```python
+from xturing.models import Llama2
+model = Llama2()
+
+## or
+from xturing.models import BaseModel
+model = BaseModel.create('llama2')
+
+```
+2. __`Evaluation`__ - Now you can evaluate any `Causal Language Model` on any dataset. The metrics currently supported is [`perplexity`](https://towardsdatascience.com/perplexity-in-language-models-87a196019a94).
+```python
+# Make the necessary imports
+from xturing.datasets import InstructionDataset
+from xturing.models import BaseModel
+
+# Load the desired dataset
+dataset = InstructionDataset('../llama/alpaca_data')
+
+# Load the desired model
+model = BaseModel.create('gpt2')
+
+# Run the Evaluation of the model on the dataset
+result = model.evaluate(dataset)
+
+# Print the result
+print(f"Perplexity of the evalution: {result}")
+
+```
+3. __`INT4` Precision__ - You can now use and fine-tune any LLM with `INT4 Precision` using `GenericKbitModel`.
+```python
+# Make the necessary imports
+from xturing.datasets import InstructionDataset
+from xturing.models import GenericKbitModel
+
+# Load the desired dataset
+dataset = InstructionDataset('../llama/alpaca_data')
+
+# Load the desired model for INT4 bit fine-tuning
+model = GenericKbitModel('tiiuae/falcon-7b')
+
+# Run the fine-tuning
+model.finetune(dataset)
+```
+4. __CPU inference__ - Now you can use just your CPU for inference of any LLM. _CAUTION : The inference process may be sluggish because CPUs lack the required computational capacity for efficient inference_.
+5. __Batch integration__ - By tweaking the 'batch_size' in the .generate() and .evaluate() functions, you can expedite results. Using a 'batch_size' greater than 1 typically enhances processing efficiency.
+```python
+# Make the necessary imports
+from xturing.datasets import InstructionDataset
+from xturing.models import GenericKbitModel
+
+# Load the desired dataset
+dataset = InstructionDataset('../llama/alpaca_data')
+
+# Load the desired model for INT4 bit fine-tuning
+model = GenericKbitModel('tiiuae/falcon-7b')
+
+# Generate outputs on desired prompts
+outputs = model.generate(dataset = dataset, batch_size=10)
+
+```
+
+An exploration of the [Llama LoRA INT4 working example](examples/int4_finetuning/LLaMA_lora_int4.ipynb) is recommended for an understanding of its application.
 
-You can check the  [Falcon LoRA INT8 working example](examples/falcon/falcon_lora_int8.py) repository to see how it works.
-Also, you can check the  [GenericModel working example](examples/generic/generic_model.py) repository to see how it works.
+For an extended insight, consider examining the [GenericModel working example](examples/generic/generic_model.py) available in the repository.
 
 <br>
 
 ## ⚙️ Installation
 ```bash
 pip install xturing
 ```
@@ -394,16 +454,16 @@
 - [x] INT8 low-precision fine-tuning support
 - [x] OpenAI, Cohere and AI21 Studio model APIs for dataset generation
 - [x] Added fine-tuned checkpoints for some models to the hub
 - [x] INT4 LLaMA LoRA fine-tuning demo
 - [x] INT4 LLaMA LoRA fine-tuning with INT4 generation
 - [x] Support for a `Generic model` wrapper
 - [x] Support for `Falcon-7B` model
-- [X] INT4 low-precision fine-tuning support
-- [ ] Evaluation of LLM models
+- [x] INT4 low-precision fine-tuning support
+- [x] Evaluation of LLM models
 - [ ] INT3, INT2, INT1 low-precision fine-tuning support
 - [ ] Support for Stable Diffusion
 
 <br>
 
 ## 🤝 Help and Support
 If you have any questions, you can create an issue on this repository.
```

### Comparing `xturing-0.1.6/README.md` & `xturing-0.1.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -31,19 +31,79 @@
 - Explore different fine-tuning methods and benchmark them to find the best performing model
 - Evaluate fine-tuned models on well-defined metrics for in-depth analysis
 
 <br>
 
 ## 🌟 What's new?
 We are excited to announce the latest enhancements to our `xTuring` library:
-1. __`Falcon LLM` integration__ - You can use and fine-tune the _`Falcon-7B`_ model in different configurations: _off-the-shelf_, _off-the-shelf with INT8 precision_, _LoRA fine-tuning_, and _LoRA fine-tuning with INT8 precision_.
-2. __`GenericModel` wrapper__ - This new integration allows you to test and fine-tune any new model on `xTuring` without waiting for it to be integrated using class _`GenericModel`_.
+1. __`LLaMA 2` integration__ - You can use and fine-tune the _`LLaMA 2`_ model in different configurations: _off-the-shelf_, _off-the-shelf with INT8 precision_, _LoRA fine-tuning_, _LoRA fine-tuning with INT8 precision_ and _LoRA fine-tuning with INT4 precision_ using the `GenericModel` wrapper and/or you can use the `Llama2` class from `xturing.models` to test and finetune the model.
+```python
+from xturing.models import Llama2
+model = Llama2()
+
+## or
+from xturing.models import BaseModel
+model = BaseModel.create('llama2')
+
+```
+2. __`Evaluation`__ - Now you can evaluate any `Causal Language Model` on any dataset. The metrics currently supported is [`perplexity`](https://towardsdatascience.com/perplexity-in-language-models-87a196019a94).
+```python
+# Make the necessary imports
+from xturing.datasets import InstructionDataset
+from xturing.models import BaseModel
+
+# Load the desired dataset
+dataset = InstructionDataset('../llama/alpaca_data')
+
+# Load the desired model
+model = BaseModel.create('gpt2')
+
+# Run the Evaluation of the model on the dataset
+result = model.evaluate(dataset)
+
+# Print the result
+print(f"Perplexity of the evalution: {result}")
+
+```
+3. __`INT4` Precision__ - You can now use and fine-tune any LLM with `INT4 Precision` using `GenericKbitModel`.
+```python
+# Make the necessary imports
+from xturing.datasets import InstructionDataset
+from xturing.models import GenericKbitModel
+
+# Load the desired dataset
+dataset = InstructionDataset('../llama/alpaca_data')
+
+# Load the desired model for INT4 bit fine-tuning
+model = GenericKbitModel('tiiuae/falcon-7b')
+
+# Run the fine-tuning
+model.finetune(dataset)
+```
+4. __CPU inference__ - Now you can use just your CPU for inference of any LLM. _CAUTION : The inference process may be sluggish because CPUs lack the required computational capacity for efficient inference_.
+5. __Batch integration__ - By tweaking the 'batch_size' in the .generate() and .evaluate() functions, you can expedite results. Using a 'batch_size' greater than 1 typically enhances processing efficiency.
+```python
+# Make the necessary imports
+from xturing.datasets import InstructionDataset
+from xturing.models import GenericKbitModel
+
+# Load the desired dataset
+dataset = InstructionDataset('../llama/alpaca_data')
+
+# Load the desired model for INT4 bit fine-tuning
+model = GenericKbitModel('tiiuae/falcon-7b')
+
+# Generate outputs on desired prompts
+outputs = model.generate(dataset = dataset, batch_size=10)
+
+```
+
+An exploration of the [Llama LoRA INT4 working example](examples/int4_finetuning/LLaMA_lora_int4.ipynb) is recommended for an understanding of its application.
 
-You can check the  [Falcon LoRA INT8 working example](examples/falcon/falcon_lora_int8.py) repository to see how it works.
-Also, you can check the  [GenericModel working example](examples/generic/generic_model.py) repository to see how it works.
+For an extended insight, consider examining the [GenericModel working example](examples/generic/generic_model.py) available in the repository.
 
 <br>
 
 ## ⚙️ Installation
 ```bash
 pip install xturing
 ```
@@ -166,16 +226,16 @@
 - [x] INT8 low-precision fine-tuning support
 - [x] OpenAI, Cohere and AI21 Studio model APIs for dataset generation
 - [x] Added fine-tuned checkpoints for some models to the hub
 - [x] INT4 LLaMA LoRA fine-tuning demo
 - [x] INT4 LLaMA LoRA fine-tuning with INT4 generation
 - [x] Support for a `Generic model` wrapper
 - [x] Support for `Falcon-7B` model
-- [X] INT4 low-precision fine-tuning support
-- [ ] Evaluation of LLM models
+- [x] INT4 low-precision fine-tuning support
+- [x] Evaluation of LLM models
 - [ ] INT3, INT2, INT1 low-precision fine-tuning support
 - [ ] Support for Stable Diffusion
 
 <br>
 
 ## 🤝 Help and Support
 If you have any questions, you can create an issue on this repository.
```

#### html2text {}

```diff
@@ -13,23 +13,51 @@
 `xTuring` you can, - Ingest data from different sources and preprocess them to
 a format LLMs can understand - Scale from single to multiple GPUs for faster
 fine-tuning - Leverage memory-efficient methods (i.e. INT4, LoRA fine-tuning)
 to reduce hardware costs by up to 90% - Explore different fine-tuning methods
 and benchmark them to find the best performing model - Evaluate fine-tuned
 models on well-defined metrics for in-depth analysis
 ## ð What's new? We are excited to announce the latest enhancements to our
-`xTuring` library: 1. __`Falcon LLM` integration__ - You can use and fine-tune
-the _`Falcon-7B`_ model in different configurations: _off-the-shelf_, _off-the-
-shelf with INT8 precision_, _LoRA fine-tuning_, and _LoRA fine-tuning with INT8
-precision_. 2. __`GenericModel` wrapper__ - This new integration allows you to
-test and fine-tune any new model on `xTuring` without waiting for it to be
-integrated using class _`GenericModel`_. You can check the [Falcon LoRA INT8
-working example](examples/falcon/falcon_lora_int8.py) repository to see how it
-works. Also, you can check the [GenericModel working example](examples/generic/
-generic_model.py) repository to see how it works.
+`xTuring` library: 1. __`LLaMA 2` integration__ - You can use and fine-tune the
+_`LLaMA 2`_ model in different configurations: _off-the-shelf_, _off-the-shelf
+with INT8 precision_, _LoRA fine-tuning_, _LoRA fine-tuning with INT8
+precision_ and _LoRA fine-tuning with INT4 precision_ using the `GenericModel`
+wrapper and/or you can use the `Llama2` class from `xturing.models` to test and
+finetune the model. ```python from xturing.models import Llama2 model = Llama2
+() ## or from xturing.models import BaseModel model = BaseModel.create
+('llama2') ``` 2. __`Evaluation`__ - Now you can evaluate any `Causal Language
+Model` on any dataset. The metrics currently supported is [`perplexity`](https:
+//towardsdatascience.com/perplexity-in-language-models-87a196019a94). ```python
+# Make the necessary imports from xturing.datasets import InstructionDataset
+from xturing.models import BaseModel # Load the desired dataset dataset =
+InstructionDataset('../llama/alpaca_data') # Load the desired model model =
+BaseModel.create('gpt2') # Run the Evaluation of the model on the dataset
+result = model.evaluate(dataset) # Print the result print(f"Perplexity of the
+evalution: {result}") ``` 3. __`INT4` Precision__ - You can now use and fine-
+tune any LLM with `INT4 Precision` using `GenericKbitModel`. ```python # Make
+the necessary imports from xturing.datasets import InstructionDataset from
+xturing.models import GenericKbitModel # Load the desired dataset dataset =
+InstructionDataset('../llama/alpaca_data') # Load the desired model for INT4
+bit fine-tuning model = GenericKbitModel('tiiuae/falcon-7b') # Run the fine-
+tuning model.finetune(dataset) ``` 4. __CPU inference__ - Now you can use just
+your CPU for inference of any LLM. _CAUTION : The inference process may be
+sluggish because CPUs lack the required computational capacity for efficient
+inference_. 5. __Batch integration__ - By tweaking the 'batch_size' in the
+.generate() and .evaluate() functions, you can expedite results. Using a
+'batch_size' greater than 1 typically enhances processing efficiency. ```python
+# Make the necessary imports from xturing.datasets import InstructionDataset
+from xturing.models import GenericKbitModel # Load the desired dataset dataset
+= InstructionDataset('../llama/alpaca_data') # Load the desired model for INT4
+bit fine-tuning model = GenericKbitModel('tiiuae/falcon-7b') # Generate outputs
+on desired prompts outputs = model.generate(dataset = dataset, batch_size=10)
+``` An exploration of the [Llama LoRA INT4 working example](examples/
+int4_finetuning/LLaMA_lora_int4.ipynb) is recommended for an understanding of
+its application. For an extended insight, consider examining the [GenericModel
+working example](examples/generic/generic_model.py) available in the
+repository.
 ## âï¸ Installation ```bash pip install xturing ```
 ## ð Quickstart ```python from xturing.datasets import InstructionDataset
 from xturing.models import BaseModel # Load the dataset instruction_dataset =
 InstructionDataset("./alpaca_data") # Initialize the model model =
 BaseModel.create("llama_lora") # Finetune the model model.finetune
 (dataset=instruction_dataset) # Perform inference output = model.generate
 (texts=["Why LLM models are becoming so important?"]) print("Generated output
@@ -83,16 +111,16 @@
 ## ð Roadmap - [x] Support for `LLaMA`, `GPT-J`, `GPT-2`, `OPT`, `Cerebras-
 GPT`, `Galactica` and `Bloom` models - [x] Dataset generation using self-
 instruction - [x] Low-precision LoRA fine-tuning and unsupervised fine-tuning -
 [x] INT8 low-precision fine-tuning support - [x] OpenAI, Cohere and AI21 Studio
 model APIs for dataset generation - [x] Added fine-tuned checkpoints for some
 models to the hub - [x] INT4 LLaMA LoRA fine-tuning demo - [x] INT4 LLaMA LoRA
 fine-tuning with INT4 generation - [x] Support for a `Generic model` wrapper -
-[x] Support for `Falcon-7B` model - [X] INT4 low-precision fine-tuning support
-- [ ] Evaluation of LLM models - [ ] INT3, INT2, INT1 low-precision fine-tuning
+[x] Support for `Falcon-7B` model - [x] INT4 low-precision fine-tuning support
+- [x] Evaluation of LLM models - [ ] INT3, INT2, INT1 low-precision fine-tuning
 support - [ ] Support for Stable Diffusion
 ## ð¤ Help and Support If you have any questions, you can create an issue on
 this repository. You can also join our [Discord server](https://discord.gg/
 TgHXuSJEk6) and start a discussion in the `#xturing` channel.
 ## ð License This project is licensed under the Apache License 2.0 - see the
 [LICENSE](LICENSE) file for details.
 ## ð Contributing As an open source project in a rapidly evolving field, we
```

### Comparing `xturing-0.1.6/pyproject.toml` & `xturing-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xturing"
-version = "0.1.6"
+version = "0.1.7"
 description = "Fine-tuning, evaluation and data generation for LLMs"
 
 authors = [
     { name = "Glenn Ko", email = "glenn@stochastic.ai" },
     { name = "Yuji Chai", email = "yuji.chai@stochastic.ai" },
     { name = "Roman Ageev", email = "roman.ageev@stochastic.ai" },
     { name = "Toan Do", email = "toan.do@stochastic.ai" },
```

### Comparing `xturing-0.1.6/src/xturing/cli/__init__.py` & `xturing-0.1.7/src/xturing/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/cli/api.py` & `xturing-0.1.7/src/xturing/cli/api.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/cli/chat.py` & `xturing-0.1.7/src/xturing/cli/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import time
 from pathlib import Path
 
 import click
 
 from xturing import BaseModel
```

### Comparing `xturing-0.1.6/src/xturing/config/__init__.py` & `xturing-0.1.7/src/xturing/config/__init__.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/config/config_data_classes.py` & `xturing-0.1.7/src/xturing/config/config_data_classes.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/config/finetuning_config.yaml` & `xturing-0.1.7/src/xturing/config/finetuning_config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -189,14 +189,15 @@
 
 llama:
   learning_rate: 5e-5
   weight_decay: 0.01
   num_train_epochs: 3
   optimizer_name: cpu_adam
 
+
 llama_lora:
   learning_rate: 1e-4
   weight_decay: 0.01
   num_train_epochs: 3
   batch_size: 1
 
 llama_lora_int8:
@@ -223,14 +224,44 @@
   save_freq: 1
   trainable_kl_weight: False
   trainable_ce_weight: False
   weight_decay: 1e-5
   intra_save_freq: 200
   groupsize: 128
 
+llama2:
+  learning_rate: 5e-5
+  weight_decay: 0.01
+  num_train_epochs: 3
+  optimizer_name: cpu_adam
+
+llama2_lora:
+  learning_rate: 5e-5
+  weight_decay: 0.01
+  num_train_epochs: 3
+  optimizer_name: cpu_adam
+
+llama2_lora_int8:
+  learning_rate: 5e-5
+  weight_decay: 0.01
+  num_train_epochs: 3
+  optimizer_name: cpu_adam
+
+llama2_int8:
+  learning_rate: 5e-5
+  weight_decay: 0.01
+  num_train_epochs: 3
+  optimizer_name: cpu_adam
+
+llama2_lora_kbit:
+  learning_rate: 5e-5
+  weight_decay: 0.01
+  num_train_epochs: 3
+  optimizer_name: cpu_adam
+
 opt:
   learning_rate: 5e-5
   weight_decay: 0.01
   num_train_epochs: 3
 
 opt_lora:
   learning_rate: 1e-4
```

### Comparing `xturing-0.1.6/src/xturing/config/generation_config.yaml` & `xturing-0.1.7/src/xturing/config/generation_config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,43 @@
 
 # Greedy search
 llama_lora_kbit:
   max_new_tokens: 256
   do_sample: false
 
 # Contrastive search
+llama2:
+  penalty_alpha: 0.6
+  top_k: 4
+  max_new_tokens: 256
+  do_sample: false
+
+# Contrastive search
+llama2_lora:
+  penalty_alpha: 0.6
+  top_k: 4
+  max_new_tokens: 256
+  do_sample: false
+
+# Greedy search
+llama2_int8:
+  max_new_tokens: 256
+  do_sample: false
+
+# Greedy search
+llama2_lora_int8:
+  max_new_tokens: 256
+  do_sample: false
+
+# Greedy search
+llama2_lora_kbit:
+  max_new_tokens: 256
+  do_sample: false
+
+# Contrastive search
 opt:
   penalty_alpha: 0.6
   top_k: 4
   max_new_tokens: 256
   do_sample: false
 
 # Contrastive search
```

### Comparing `xturing-0.1.6/src/xturing/config/read_config.py` & `xturing-0.1.7/src/xturing/config/read_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
     xturing_config_file_path = dir_path / "xturing.json"
 
     return xturing_config_file_path.is_file()
 
 
 def exists_lora_config_file(dir_path: Optional[Union[Path, str]] = None):
+    # Check if lora config exists
     if dir_path is None:
         return False
     dir_path = Path(dir_path)
     assert dir_path.is_dir(), "The following path {} should be a directory".format(
         str(dir_path)
     )
```

### Comparing `xturing-0.1.6/src/xturing/datasets/instruction_dataset.py` & `xturing-0.1.7/src/xturing/datasets/instruction_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import os
 from dataclasses import dataclass
 from pathlib import Path
 from typing import List, Optional, Union
 
 from datasets import Dataset
 from datasets import Dataset as HFDataset
 from datasets import DatasetDict, load_from_disk
```

### Comparing `xturing-0.1.6/src/xturing/datasets/text_dataset.py` & `xturing-0.1.7/src/xturing/datasets/text_dataset.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/__init__.py` & `xturing-0.1.7/src/xturing/engines/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,67 @@
-from .base import BaseEngine
-from .bloom_engine import (
+from xturing.engines.base import BaseEngine
+from xturing.engines.bloom_engine import (
     BloomEngine,
     BloomInt8Engine,
     BloomLoraEngine,
     BloomLoraInt8Engine,
 )
-from .cerebras_engine import (
+from xturing.engines.cerebras_engine import (
     CerebrasEngine,
     CerebrasInt8Engine,
     CerebrasLoraEngine,
     CerebrasLoraInt8Engine,
 )
-from .distilgpt2_engine import DistilGPT2Engine, DistilGPT2LoraEngine
-from .falcon_engine import (
+from xturing.engines.distilgpt2_engine import DistilGPT2Engine, DistilGPT2LoraEngine
+from xturing.engines.falcon_engine import (
     FalconEngine,
     FalconInt8Engine,
     FalconLoraEngine,
     FalconLoraInt8Engine,
     FalconLoraKbitEngine,
 )
-from .galactica_engine import (
+from xturing.engines.galactica_engine import (
     GalacticaEngine,
     GalacticaInt8Engine,
     GalacticaLoraEngine,
     GalacticaLoraInt8Engine,
 )
-from .generic_engine import (
+from xturing.engines.generic_engine import (
     GenericEngine,
     GenericInt8Engine,
     GenericLoraEngine,
     GenericLoraInt8Engine,
     GenericLoraKbitEngine,
 )
-from .gpt2_engine import GPT2Engine, GPT2Int8Engine, GPT2LoraEngine, GPT2LoraInt8Engine
-from .gptj_engine import GPTJEngine, GPTJInt8Engine, GPTJLoraEngine, GPTJLoraInt8Engine
-from .llama_engine import (
+from xturing.engines.gpt2_engine import (
+    GPT2Engine,
+    GPT2Int8Engine,
+    GPT2LoraEngine,
+    GPT2LoraInt8Engine,
+)
+from xturing.engines.gptj_engine import (
+    GPTJEngine,
+    GPTJInt8Engine,
+    GPTJLoraEngine,
+    GPTJLoraInt8Engine,
+)
+from xturing.engines.llama2_engine import LLama2Engine
+from xturing.engines.llama_engine import (
     LLamaEngine,
     LLamaInt8Engine,
     LlamaLoraEngine,
     LlamaLoraInt8Engine,
     LlamaLoraKbitEngine,
 )
-from .opt_engine import OPTEngine, OPTInt8Engine, OPTLoraEngine, OPTLoraInt8Engine
+from xturing.engines.opt_engine import (
+    OPTEngine,
+    OPTInt8Engine,
+    OPTLoraEngine,
+    OPTLoraInt8Engine,
+)
 
 BaseEngine.add_to_registry(BloomEngine.config_name, BloomEngine)
 BaseEngine.add_to_registry(BloomInt8Engine.config_name, BloomInt8Engine)
 BaseEngine.add_to_registry(BloomLoraEngine.config_name, BloomLoraEngine)
 BaseEngine.add_to_registry(BloomLoraInt8Engine.config_name, BloomLoraInt8Engine)
 BaseEngine.add_to_registry(CerebrasEngine.config_name, CerebrasEngine)
 BaseEngine.add_to_registry(CerebrasInt8Engine.config_name, CerebrasInt8Engine)
@@ -76,11 +92,12 @@
 BaseEngine.add_to_registry(GPT2LoraEngine.config_name, GPT2LoraEngine)
 BaseEngine.add_to_registry(GPT2LoraInt8Engine.config_name, GPT2LoraInt8Engine)
 BaseEngine.add_to_registry(LLamaEngine.config_name, LLamaEngine)
 BaseEngine.add_to_registry(LLamaInt8Engine.config_name, LLamaInt8Engine)
 BaseEngine.add_to_registry(LlamaLoraEngine.config_name, LlamaLoraEngine)
 BaseEngine.add_to_registry(LlamaLoraInt8Engine.config_name, LlamaLoraInt8Engine)
 BaseEngine.add_to_registry(LlamaLoraKbitEngine.config_name, LlamaLoraKbitEngine)
+BaseEngine.add_to_registry(LLama2Engine.config_name, LLama2Engine)
 BaseEngine.add_to_registry(OPTEngine.config_name, OPTEngine)
 BaseEngine.add_to_registry(OPTInt8Engine.config_name, OPTInt8Engine)
 BaseEngine.add_to_registry(OPTLoraEngine.config_name, OPTLoraEngine)
 BaseEngine.add_to_registry(OPTLoraInt8Engine.config_name, OPTLoraInt8Engine)
```

### Comparing `xturing-0.1.6/src/xturing/engines/bloom_engine.py` & `xturing-0.1.7/src/xturing/engines/bloom_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/causal.py` & `xturing-0.1.7/src/xturing/engines/causal.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         model: Optional[Any] = None,
         tokenizer: Optional[Any] = None,
         load_8bit: Optional[bool] = False,
         trust_remote_code: Optional[bool] = False,
         **kwargs,
     ):
         self.model_name = model_name
-
         if weights_path is not None:
             assert Path(
                 weights_path
             ).is_dir(), "The weights path should be a existing directory"
             if load_8bit:
                 device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
                 self.model = AutoModelForCausalLM.from_pretrained(
```

### Comparing `xturing-0.1.6/src/xturing/engines/cerebras_engine.py` & `xturing-0.1.7/src/xturing/engines/cerebras_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/distilgpt2_engine.py` & `xturing-0.1.7/src/xturing/engines/distilgpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/falcon_engine.py` & `xturing-0.1.7/src/xturing/engines/falcon_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/galactica_engine.py` & `xturing-0.1.7/src/xturing/engines/galactica_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/generic_engine.py` & `xturing-0.1.7/src/xturing/engines/generic_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from pathlib import Path
 from typing import List, Optional, Union
 
 from xturing.engines.causal import CausalEngine, CausalLoraEngine, CausalLoraKbitEngine
 
 
 class GenericEngine(CausalEngine):
```

### Comparing `xturing-0.1.6/src/xturing/engines/gpt2_engine.py` & `xturing-0.1.7/src/xturing/engines/gpt2_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/gptj_engine.py` & `xturing-0.1.7/src/xturing/engines/gptj_engine.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/gptj_utils/gptj.py` & `xturing-0.1.7/src/xturing/engines/gptj_utils/gptj.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/llama_utils/llama.py` & `xturing-0.1.7/src/xturing/engines/llama_utils/llama.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import math
 import os
-from pathlib import Path
 from shutil import copyfile
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import sentencepiece as spm
 import torch
 import torch.utils.checkpoint
 from torch import nn
@@ -14,16 +13,14 @@
 from transformers.modeling_outputs import (
     BaseModelOutputWithPast,
     CausalLMOutputWithPast,
 )
 from transformers.modeling_utils import PreTrainedModel
 from transformers.tokenization_utils import PreTrainedTokenizer
 
-from xturing.engines.causal import CausalEngine, CausalLoraEngine
-
 # Tokenizer taken from transformers library: https://github.com/huggingface/transformers
 """Tokenization classes for LLaMA."""
 
 VOCAB_FILES_NAMES = {"vocab_file": "tokenizer.model"}
 
 PRETRAINED_VOCAB_FILES_MAP = {}
```

### Comparing `xturing-0.1.6/src/xturing/engines/lora_engine/lora.py` & `xturing-0.1.7/src/xturing/engines/lora_engine/lora.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/lora_engine/save_and_load.py` & `xturing-0.1.7/src/xturing/engines/lora_engine/save_and_load.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/opt_engine.py` & `xturing-0.1.7/src/xturing/engines/opt_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from pathlib import Path
 from typing import Optional, Union
 
 from xturing.engines.causal import CausalEngine, CausalLoraEngine
 
 
 class OPTEngine(CausalEngine):
```

### Comparing `xturing-0.1.6/src/xturing/engines/quant_utils/cachedistillationoutputs.py` & `xturing-0.1.7/src/xturing/engines/quant_utils/cachedistillationoutputs.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/quant_utils/custom_autotune.py` & `xturing-0.1.7/src/xturing/engines/quant_utils/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/quant_utils/lrec.py` & `xturing-0.1.7/src/xturing/engines/quant_utils/lrec.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/quant_utils/peft_utils.py` & `xturing-0.1.7/src/xturing/engines/quant_utils/peft_utils.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/quant_utils/qerdataloading.py` & `xturing-0.1.7/src/xturing/engines/quant_utils/qerdataloading.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/engines/quant_utils/quant.py` & `xturing-0.1.7/src/xturing/engines/quant_utils/quant.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/model_apis/__init__.py` & `xturing-0.1.7/src/xturing/model_apis/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from .ai21 import AI21TextGenerationAPI
-from .ai21 import J2Grande as AI21J2Grande
-from .base import BaseApi, TextGenerationAPI
-from .cohere import CohereTextGenerationAPI
-from .cohere import Medium as CohereMedium
-from .openai import ChatGPT as OpenAIChatGPT
-from .openai import Davinci as OpenAIDavinci
-from .openai import OpenAITextGenerationAPI
+from xturing.model_apis.ai21 import AI21TextGenerationAPI
+from xturing.model_apis.ai21 import J2Grande as AI21J2Grande
+from xturing.model_apis.base import BaseApi, TextGenerationAPI
+from xturing.model_apis.cohere import CohereTextGenerationAPI
+from xturing.model_apis.cohere import Medium as CohereMedium
+from xturing.model_apis.openai import ChatGPT as OpenAIChatGPT
+from xturing.model_apis.openai import Davinci as OpenAIDavinci
+from xturing.model_apis.openai import OpenAITextGenerationAPI
 
 BaseApi.add_to_registry(OpenAITextGenerationAPI.config_name, OpenAITextGenerationAPI)
 BaseApi.add_to_registry(CohereTextGenerationAPI.config_name, CohereTextGenerationAPI)
 BaseApi.add_to_registry(AI21TextGenerationAPI.config_name, AI21TextGenerationAPI)
 BaseApi.add_to_registry(OpenAIDavinci.config_name, OpenAIDavinci)
 BaseApi.add_to_registry(OpenAIChatGPT.config_name, OpenAIChatGPT)
 BaseApi.add_to_registry(CohereMedium.config_name, CohereMedium)
```

### Comparing `xturing-0.1.6/src/xturing/model_apis/ai21.py` & `xturing-0.1.7/src/xturing/model_apis/ai21.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/model_apis/base.py` & `xturing-0.1.7/src/xturing/model_apis/base.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/model_apis/cohere.py` & `xturing-0.1.7/src/xturing/model_apis/cohere.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/model_apis/openai.py` & `xturing-0.1.7/src/xturing/model_apis/openai.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/models/__init__.py` & `xturing-0.1.7/src/xturing/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,48 @@
-from .base import BaseModel
-from .bloom import Bloom, BloomInt8, BloomLora, BloomLoraInt8
-from .cerebras import Cerebras, CerebrasInt8, CerebrasLora, CerebrasLoraInt8
-from .distilgpt2 import DistilGPT2, DistilGPT2Lora
-from .falcon import Falcon, FalconInt8, FalconLora, FalconLoraInt8, FalconLoraKbit
-from .galactica import Galactica, GalacticaInt8, GalacticaLora, GalacticaLoraInt8
-from .generic import (
+from xturing.models.base import BaseModel
+from xturing.models.bloom import Bloom, BloomInt8, BloomLora, BloomLoraInt8
+from xturing.models.cerebras import (
+    Cerebras,
+    CerebrasInt8,
+    CerebrasLora,
+    CerebrasLoraInt8,
+)
+from xturing.models.distilgpt2 import DistilGPT2, DistilGPT2Lora
+from xturing.models.falcon import (
+    Falcon,
+    FalconInt8,
+    FalconLora,
+    FalconLoraInt8,
+    FalconLoraKbit,
+)
+from xturing.models.galactica import (
+    Galactica,
+    GalacticaInt8,
+    GalacticaLora,
+    GalacticaLoraInt8,
+)
+from xturing.models.generic import (
     GenericInt8Model,
     GenericLoraInt8Model,
     GenericLoraKbitModel,
     GenericLoraModel,
     GenericModel,
 )
-from .gpt2 import GPT2, GPT2Int8, GPT2Lora, GPT2LoraInt8
-from .gptj import GPTJ, GPTJInt8, GPTJLora, GPTJLoraInt8
-from .llama import Llama, LlamaInt8, LlamaLora, LlamaLoraInt8, LlamaLoraKbit
-from .opt import OPT, OPTInt8, OPTLora, OPTLoraInt8
-from .stable_diffusion import StableDiffusion
+from xturing.models.gpt2 import GPT2, GPT2Int8, GPT2Lora, GPT2LoraInt8
+from xturing.models.gptj import GPTJ, GPTJInt8, GPTJLora, GPTJLoraInt8
+from xturing.models.llama import (
+    Llama,
+    LlamaInt8,
+    LlamaLora,
+    LlamaLoraInt8,
+    LlamaLoraKbit,
+)
+from xturing.models.llama2 import Llama2
+from xturing.models.opt import OPT, OPTInt8, OPTLora, OPTLoraInt8
+from xturing.models.stable_diffusion import StableDiffusion
 
 BaseModel.add_to_registry(Bloom.config_name, Bloom)
 BaseModel.add_to_registry(BloomInt8.config_name, BloomInt8)
 BaseModel.add_to_registry(BloomLora.config_name, BloomLora)
 BaseModel.add_to_registry(BloomLoraInt8.config_name, BloomLoraInt8)
 BaseModel.add_to_registry(Cerebras.config_name, Cerebras)
 BaseModel.add_to_registry(CerebrasInt8.config_name, CerebrasInt8)
@@ -50,12 +73,13 @@
 BaseModel.add_to_registry(GPT2Lora.config_name, GPT2Lora)
 BaseModel.add_to_registry(GPT2LoraInt8.config_name, GPT2LoraInt8)
 BaseModel.add_to_registry(Llama.config_name, Llama)
 BaseModel.add_to_registry(LlamaInt8.config_name, LlamaInt8)
 BaseModel.add_to_registry(LlamaLora.config_name, LlamaLora)
 BaseModel.add_to_registry(LlamaLoraInt8.config_name, LlamaLoraInt8)
 BaseModel.add_to_registry(LlamaLoraKbit.config_name, LlamaLoraKbit)
+BaseModel.add_to_registry(Llama2.config_name, Llama2)
 BaseModel.add_to_registry(OPT.config_name, OPT)
 BaseModel.add_to_registry(OPTInt8.config_name, OPTInt8)
 BaseModel.add_to_registry(OPTLora.config_name, OPTLora)
 BaseModel.add_to_registry(OPTLoraInt8.config_name, OPTLoraInt8)
 BaseModel.add_to_registry(StableDiffusion.config_name, StableDiffusion)
```

### Comparing `xturing-0.1.6/src/xturing/models/base.py` & `xturing-0.1.7/src/xturing/models/base.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/models/bloom.py` & `xturing-0.1.7/src/xturing/models/bloom.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/models/cerebras.py` & `xturing-0.1.7/src/xturing/models/cerebras.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/models/distilgpt2.py` & `xturing-0.1.7/src/xturing/models/distilgpt2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Optional
 
 from xturing.engines.distilgpt2_engine import DistilGPT2Engine, DistilGPT2LoraEngine
-
-from .causal import CausalLoraModel, CausalModel
+from xturing.models.causal import CausalLoraModel, CausalModel
 
 
 class DistilGPT2(CausalModel):
     config_name: str = "distilgpt2"
 
     def __init__(self, weights_path: Optional[str] = None):
         super().__init__(DistilGPT2Engine.config_name, weights_path)
```

### Comparing `xturing-0.1.6/src/xturing/models/falcon.py` & `xturing-0.1.7/src/xturing/models/falcon.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/models/galactica.py` & `xturing-0.1.7/src/xturing/models/galactica.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/models/generic.py` & `xturing-0.1.7/src/xturing/models/generic.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/models/gpt2.py` & `xturing-0.1.7/src/xturing/models/gptj.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 from typing import Optional
 
-from xturing.engines.gpt2_engine import (
-    GPT2Engine,
-    GPT2Int8Engine,
-    GPT2LoraEngine,
-    GPT2LoraInt8Engine,
+from xturing.engines.gptj_engine import (
+    GPTJEngine,
+    GPTJInt8Engine,
+    GPTJLoraEngine,
+    GPTJLoraInt8Engine,
+)
+from xturing.models.causal import (
+    CausalInt8Model,
+    CausalLoraInt8Model,
+    CausalLoraModel,
+    CausalModel,
 )
-
-from .causal import CausalInt8Model, CausalLoraInt8Model, CausalLoraModel, CausalModel
 
 
-class GPT2(CausalModel):
-    config_name: str = "gpt2"
+class GPTJ(CausalModel):
+    config_name: str = "gptj"
 
     def __init__(self, weights_path: Optional[str] = None):
-        super().__init__(GPT2Engine.config_name, weights_path)
+        super().__init__(GPTJEngine.config_name, weights_path)
 
 
-class GPT2Lora(CausalLoraModel):
-    config_name: str = "gpt2_lora"
+class GPTJLora(CausalLoraModel):
+    config_name: str = "gptj_lora"
 
     def __init__(self, weights_path: Optional[str] = None):
-        super().__init__(GPT2LoraEngine.config_name, weights_path)
+        super().__init__(GPTJLoraEngine.config_name, weights_path)
 
 
-class GPT2Int8(CausalInt8Model):
-    config_name: str = "gpt2_int8"
+class GPTJInt8(CausalInt8Model):
+    config_name: str = "gptj_int8"
 
     def __init__(self, weights_path: Optional[str] = None):
-        super().__init__(GPT2Int8Engine.config_name, weights_path)
+        super().__init__(GPTJInt8Engine.config_name, weights_path)
 
 
-class GPT2LoraInt8(CausalLoraInt8Model):
-    config_name: str = "gpt2_lora_int8"
+class GPTJLoraInt8(CausalLoraInt8Model):
+    config_name: str = "gptj_lora_int8"
 
     def __init__(self, weights_path: Optional[str] = None):
-        super().__init__(GPT2LoraInt8Engine.config_name, weights_path)
+        super().__init__(GPTJLoraInt8Engine.config_name, weights_path)
```

### Comparing `xturing-0.1.6/src/xturing/models/gptj.py` & `xturing-0.1.7/src/xturing/models/gpt2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from typing import Optional
 
-from xturing.engines.gptj_engine import (
-    GPTJEngine,
-    GPTJInt8Engine,
-    GPTJLoraEngine,
-    GPTJLoraInt8Engine,
+from xturing.engines.gpt2_engine import (
+    GPT2Engine,
+    GPT2Int8Engine,
+    GPT2LoraEngine,
+    GPT2LoraInt8Engine,
 )
 from xturing.models.causal import (
     CausalInt8Model,
     CausalLoraInt8Model,
     CausalLoraModel,
     CausalModel,
 )
 
 
-class GPTJ(CausalModel):
-    config_name: str = "gptj"
+class GPT2(CausalModel):
+    config_name: str = "gpt2"
 
     def __init__(self, weights_path: Optional[str] = None):
-        super().__init__(GPTJEngine.config_name, weights_path)
+        super().__init__(GPT2Engine.config_name, weights_path)
 
 
-class GPTJLora(CausalLoraModel):
-    config_name: str = "gptj_lora"
+class GPT2Lora(CausalLoraModel):
+    config_name: str = "gpt2_lora"
 
     def __init__(self, weights_path: Optional[str] = None):
-        super().__init__(GPTJLoraEngine.config_name, weights_path)
+        super().__init__(GPT2LoraEngine.config_name, weights_path)
 
 
-class GPTJInt8(CausalInt8Model):
-    config_name: str = "gptj_int8"
+class GPT2Int8(CausalInt8Model):
+    config_name: str = "gpt2_int8"
 
     def __init__(self, weights_path: Optional[str] = None):
-        super().__init__(GPTJInt8Engine.config_name, weights_path)
+        super().__init__(GPT2Int8Engine.config_name, weights_path)
 
 
-class GPTJLoraInt8(CausalLoraInt8Model):
-    config_name: str = "gptj_lora_int8"
+class GPT2LoraInt8(CausalLoraInt8Model):
+    config_name: str = "gpt2_lora_int8"
 
     def __init__(self, weights_path: Optional[str] = None):
-        super().__init__(GPTJLoraInt8Engine.config_name, weights_path)
+        super().__init__(GPT2LoraInt8Engine.config_name, weights_path)
```

### Comparing `xturing-0.1.6/src/xturing/models/llama.py` & `xturing-0.1.7/src/xturing/models/llama.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-from typing import Iterable, List, Optional, Union
+from typing import Optional
 
-from pytorch_lightning.loggers import Logger
-
-from xturing.datasets.instruction_dataset import InstructionDataset
-from xturing.datasets.text_dataset import TextDataset
 from xturing.engines.llama_engine import (
     LLamaEngine,
     LLamaInt8Engine,
     LlamaLoraEngine,
     LlamaLoraInt8Engine,
     LlamaLoraKbitEngine,
 )
 from xturing.models.causal import (
     CausalInt8Model,
     CausalLoraInt8Model,
     CausalLoraKbitModel,
     CausalLoraModel,
     CausalModel,
 )
-from xturing.trainers.base import BaseTrainer
-from xturing.trainers.lightning_trainer import LightningTrainer
 
 
 class Llama(CausalModel):
     config_name: str = "llama"
 
     def __init__(self, weights_path: Optional[str] = None):
         super().__init__(LLamaEngine.config_name, weights_path)
```

### Comparing `xturing-0.1.6/src/xturing/models/opt.py` & `xturing-0.1.7/src/xturing/models/opt.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/models/stable_diffusion.py` & `xturing-0.1.7/src/xturing/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/preprocessors/instruction_collator.py` & `xturing-0.1.7/src/xturing/preprocessors/instruction_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/preprocessors/text_collator.py` & `xturing-0.1.7/src/xturing/preprocessors/text_collator.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/registry.py` & `xturing-0.1.7/src/xturing/registry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict
+from typing import Any
 
 
 class BaseParent:
     @classmethod
     def add_to_registry(cls, name: str, obj: Any):
         assert (
             name not in cls.registry
```

### Comparing `xturing-0.1.6/src/xturing/self_instruct/bootstrap_instructions.py` & `xturing-0.1.7/src/xturing/self_instruct/bootstrap_instructions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import os
 import random
 import re
 import string
 from functools import partial
 from multiprocessing import Pool
 from pathlib import Path
```

### Comparing `xturing-0.1.6/src/xturing/self_instruct/generate_instances.py` & `xturing-0.1.7/src/xturing/self_instruct/generate_instances.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import os
 import random
 from collections import OrderedDict
 from pathlib import Path
 
 from tqdm import tqdm
 
 from xturing.model_apis import TextGenerationAPI
```

### Comparing `xturing-0.1.6/src/xturing/self_instruct/identify_if_classification.py` & `xturing-0.1.7/src/xturing/self_instruct/identify_if_classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import os
 import random
 from collections import OrderedDict
 from pathlib import Path
 
 from tqdm import tqdm
 
 from xturing.model_apis import TextGenerationAPI
```

### Comparing `xturing-0.1.6/src/xturing/self_instruct/prepare_for_finetuning.py` & `xturing-0.1.7/src/xturing/self_instruct/prepare_for_finetuning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import os
 import random
 import re
 from pathlib import Path
 from typing import List
 
 from tqdm import tqdm
```

### Comparing `xturing-0.1.6/src/xturing/self_instruct/prepare_seed_tasks.py` & `xturing-0.1.7/src/xturing/self_instruct/prepare_seed_tasks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import ast
 import json
 import os
-from typing import List
 
 from tqdm import tqdm
 
 from xturing.model_apis import TextGenerationAPI
 from xturing.utils.text_splitter import RecursiveCharacterTextSplitter
```

### Comparing `xturing-0.1.6/src/xturing/self_instruct/templates/clf_task_template.py` & `xturing-0.1.7/src/xturing/self_instruct/templates/clf_task_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/self_instruct/templates/instance_gen_template.py` & `xturing-0.1.7/src/xturing/self_instruct/templates/instance_gen_template.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/trainers/lightning_trainer.py` & `xturing-0.1.7/src/xturing/trainers/lightning_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import datetime
-import os
-import tempfile
-import uuid
 from pathlib import Path
-from typing import Iterable, Optional, Union, Type
+from typing import Iterable, Optional, Union
 
 import pytorch_lightning as pl
 import torch
 from deepspeed.ops.adam import DeepSpeedCPUAdam
 from pytorch_lightning import callbacks
-from pytorch_lightning.trainer.trainer import Trainer
 from pytorch_lightning.loggers import Logger
+from pytorch_lightning.trainer.trainer import Trainer
 
 from xturing.config import DEFAULT_DEVICE, IS_INTERACTIVE
 from xturing.datasets.base import BaseDataset
 from xturing.engines.base import BaseEngine
 from xturing.preprocessors.base import BasePreprocessor
```

### Comparing `xturing-0.1.6/src/xturing/ui/playground.py` & `xturing-0.1.7/src/xturing/ui/playground.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/utils/hub.py` & `xturing-0.1.7/src/xturing/utils/hub.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/utils/logging.py` & `xturing-0.1.7/src/xturing/utils/logging.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/utils/loss_fns.py` & `xturing-0.1.7/src/xturing/utils/loss_fns.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/utils/notebooks.py` & `xturing-0.1.7/src/xturing/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `xturing-0.1.6/src/xturing/utils/text_splitter.py` & `xturing-0.1.7/src/xturing/utils/text_splitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,14 @@
 # This code is taken from Langchain https://github.com/hwchase17/langchain
 """Functionality for splitting text."""
 from __future__ import annotations
 
-import copy
 import logging
 from abc import ABC, abstractmethod
-from typing import (
-    AbstractSet,
-    Any,
-    Callable,
-    Collection,
-    Iterable,
-    List,
-    Optional,
-    Union,
-)
+from typing import Any, Callable, Iterable, List, Optional
 
 logger = logging.getLogger()
 
 
 class TextSplitter(ABC):
     """Interface for splitting text into chunks."""
 
@@ -113,16 +103,16 @@
             )
         return cls(length_function=_huggingface_tokenizer_length, **kwargs)
 
     @classmethod
     def from_tiktoken_encoder(
         cls,
         encoding_name: str = "gpt2",
-        allowed_special = set(),
-        disallowed_special = set(),
+        allowed_special=set(),
+        disallowed_special=set(),
         **kwargs: Any,
     ) -> TextSplitter:
         """Text splitter that uses tiktoken encoder to count length."""
         try:
             import tiktoken
         except ImportError:
             raise ValueError(
```

### Comparing `xturing-0.1.6/src/xturing/utils/utils.py` & `xturing-0.1.7/src/xturing/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import contextlib
 import io
+import logging
 import os
 import random
 import string
 import sys
 import tempfile
 from pathlib import Path
+from typing import Any, List
 
 import yaml
 
+SHUFFLE_SEED = 123
+_MAX_SAMPLES = None
+
 
 def read_yamls(config_path):
     conf = {}
 
     with open(config_path) as f:
         conf.update(yaml.safe_load(f))
 
@@ -130,7 +135,18 @@
     to_delete = []
     for key, value in arguments.items():
         if value is None:
             to_delete.append(key)
     for key in to_delete:
         del arguments[key]
     return arguments
+
+
+def _index_samples(samples: List[Any], logger: logging.Logger):
+    """Shuffle `samples` and pair each sample with its index."""
+    indices = list(range(len(samples)))
+    random.Random(SHUFFLE_SEED).shuffle(indices)
+    if _MAX_SAMPLES is not None:
+        indices = indices[:_MAX_SAMPLES]
+    logger.info(f"Evaluating {len(indices)} samples")
+    work_items = [(samples[i], i) for i in indices]
+    return work_items
```

### Comparing `xturing-0.1.6/src/xturing.egg-info/PKG-INFO` & `xturing-0.1.7/src/xturing.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xturing
-Version: 0.1.6
+Version: 0.1.7
 Summary: Fine-tuning, evaluation and data generation for LLMs
 Author-email: Glenn Ko <glenn@stochastic.ai>, Yuji Chai <yuji.chai@stochastic.ai>, Roman Ageev <roman.ageev@stochastic.ai>, Toan Do <toan.do@stochastic.ai>, Marcos R M <marcos.rm@stochastic.ai>, Sarthak Langde <sarthak.langde@stochastic.ai>, Riccardo Romagnoli <riccardo.romagnoli@stochastic.ai>, Subhash G N <subhash.gn@stochastic.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -259,19 +259,79 @@
 - Explore different fine-tuning methods and benchmark them to find the best performing model
 - Evaluate fine-tuned models on well-defined metrics for in-depth analysis
 
 <br>
 
 ## 🌟 What's new?
 We are excited to announce the latest enhancements to our `xTuring` library:
-1. __`Falcon LLM` integration__ - You can use and fine-tune the _`Falcon-7B`_ model in different configurations: _off-the-shelf_, _off-the-shelf with INT8 precision_, _LoRA fine-tuning_, and _LoRA fine-tuning with INT8 precision_.
-2. __`GenericModel` wrapper__ - This new integration allows you to test and fine-tune any new model on `xTuring` without waiting for it to be integrated using class _`GenericModel`_.
+1. __`LLaMA 2` integration__ - You can use and fine-tune the _`LLaMA 2`_ model in different configurations: _off-the-shelf_, _off-the-shelf with INT8 precision_, _LoRA fine-tuning_, _LoRA fine-tuning with INT8 precision_ and _LoRA fine-tuning with INT4 precision_ using the `GenericModel` wrapper and/or you can use the `Llama2` class from `xturing.models` to test and finetune the model.
+```python
+from xturing.models import Llama2
+model = Llama2()
+
+## or
+from xturing.models import BaseModel
+model = BaseModel.create('llama2')
+
+```
+2. __`Evaluation`__ - Now you can evaluate any `Causal Language Model` on any dataset. The metrics currently supported is [`perplexity`](https://towardsdatascience.com/perplexity-in-language-models-87a196019a94).
+```python
+# Make the necessary imports
+from xturing.datasets import InstructionDataset
+from xturing.models import BaseModel
+
+# Load the desired dataset
+dataset = InstructionDataset('../llama/alpaca_data')
+
+# Load the desired model
+model = BaseModel.create('gpt2')
+
+# Run the Evaluation of the model on the dataset
+result = model.evaluate(dataset)
+
+# Print the result
+print(f"Perplexity of the evalution: {result}")
+
+```
+3. __`INT4` Precision__ - You can now use and fine-tune any LLM with `INT4 Precision` using `GenericKbitModel`.
+```python
+# Make the necessary imports
+from xturing.datasets import InstructionDataset
+from xturing.models import GenericKbitModel
+
+# Load the desired dataset
+dataset = InstructionDataset('../llama/alpaca_data')
+
+# Load the desired model for INT4 bit fine-tuning
+model = GenericKbitModel('tiiuae/falcon-7b')
+
+# Run the fine-tuning
+model.finetune(dataset)
+```
+4. __CPU inference__ - Now you can use just your CPU for inference of any LLM. _CAUTION : The inference process may be sluggish because CPUs lack the required computational capacity for efficient inference_.
+5. __Batch integration__ - By tweaking the 'batch_size' in the .generate() and .evaluate() functions, you can expedite results. Using a 'batch_size' greater than 1 typically enhances processing efficiency.
+```python
+# Make the necessary imports
+from xturing.datasets import InstructionDataset
+from xturing.models import GenericKbitModel
+
+# Load the desired dataset
+dataset = InstructionDataset('../llama/alpaca_data')
+
+# Load the desired model for INT4 bit fine-tuning
+model = GenericKbitModel('tiiuae/falcon-7b')
+
+# Generate outputs on desired prompts
+outputs = model.generate(dataset = dataset, batch_size=10)
+
+```
+
+An exploration of the [Llama LoRA INT4 working example](examples/int4_finetuning/LLaMA_lora_int4.ipynb) is recommended for an understanding of its application.
 
-You can check the  [Falcon LoRA INT8 working example](examples/falcon/falcon_lora_int8.py) repository to see how it works.
-Also, you can check the  [GenericModel working example](examples/generic/generic_model.py) repository to see how it works.
+For an extended insight, consider examining the [GenericModel working example](examples/generic/generic_model.py) available in the repository.
 
 <br>
 
 ## ⚙️ Installation
 ```bash
 pip install xturing
 ```
@@ -394,16 +454,16 @@
 - [x] INT8 low-precision fine-tuning support
 - [x] OpenAI, Cohere and AI21 Studio model APIs for dataset generation
 - [x] Added fine-tuned checkpoints for some models to the hub
 - [x] INT4 LLaMA LoRA fine-tuning demo
 - [x] INT4 LLaMA LoRA fine-tuning with INT4 generation
 - [x] Support for a `Generic model` wrapper
 - [x] Support for `Falcon-7B` model
-- [X] INT4 low-precision fine-tuning support
-- [ ] Evaluation of LLM models
+- [x] INT4 low-precision fine-tuning support
+- [x] Evaluation of LLM models
 - [ ] INT3, INT2, INT1 low-precision fine-tuning support
 - [ ] Support for Stable Diffusion
 
 <br>
 
 ## 🤝 Help and Support
 If you have any questions, you can create an issue on this repository.
```

### Comparing `xturing-0.1.6/src/xturing.egg-info/SOURCES.txt` & `xturing-0.1.7/src/xturing.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 src/xturing/engines/cerebras_engine.py
 src/xturing/engines/distilgpt2_engine.py
 src/xturing/engines/falcon_engine.py
 src/xturing/engines/galactica_engine.py
 src/xturing/engines/generic_engine.py
 src/xturing/engines/gpt2_engine.py
 src/xturing/engines/gptj_engine.py
+src/xturing/engines/llama2_engine.py
 src/xturing/engines/llama_engine.py
 src/xturing/engines/opt_engine.py
 src/xturing/engines/gptj_utils/__init__.py
 src/xturing/engines/gptj_utils/gptj.py
 src/xturing/engines/llama_utils/__init__.py
 src/xturing/engines/llama_utils/llama.py
 src/xturing/engines/lora_engine/__init__.py
@@ -66,14 +67,15 @@
 src/xturing/models/distilgpt2.py
 src/xturing/models/falcon.py
 src/xturing/models/galactica.py
 src/xturing/models/generic.py
 src/xturing/models/gpt2.py
 src/xturing/models/gptj.py
 src/xturing/models/llama.py
+src/xturing/models/llama2.py
 src/xturing/models/opt.py
 src/xturing/models/stable_diffusion.py
 src/xturing/preprocessors/__init__.py
 src/xturing/preprocessors/base.py
 src/xturing/preprocessors/instruction_collator.py
 src/xturing/preprocessors/text_collator.py
 src/xturing/self_instruct/__init__.py
@@ -91,10 +93,12 @@
 src/xturing/ui/playground.py
 src/xturing/utils/__init__.py
 src/xturing/utils/external_loggers.py
 src/xturing/utils/hub.py
 src/xturing/utils/interactive.py
 src/xturing/utils/logging.py
 src/xturing/utils/loss_fns.py
+src/xturing/utils/metrics.py
 src/xturing/utils/notebooks.py
+src/xturing/utils/prompt.py
 src/xturing/utils/text_splitter.py
 src/xturing/utils/utils.py
```

