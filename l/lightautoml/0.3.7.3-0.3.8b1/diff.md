# Comparing `tmp/LightAutoML-0.3.7.3.tar.gz` & `tmp/lightautoml-0.3.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LightAutoML-0.3.7.3.tar", max compression
+gzip compressed data, was "lightautoml-0.3.8b1.tar", max compression
```

## Comparing `LightAutoML-0.3.7.3.tar` & `lightautoml-0.3.8b1.tar`

### file list

```diff
@@ -1,148 +1,163 @@
--rw-r--r--   0        0        0    11454 2022-08-17 15:39:28.723055 LightAutoML-0.3.7.3/LICENSE
--rw-r--r--   0        0        0    12401 2022-10-12 17:08:47.626352 LightAutoML-0.3.7.3/README.md
--rw-r--r--   0        0        0      793 2022-10-12 17:08:47.786354 LightAutoML-0.3.7.3/lightautoml/__init__.py
--rw-r--r--   0        0        0      105 2022-10-12 17:08:47.786354 LightAutoML-0.3.7.3/lightautoml/addons/__init__.py
--rw-r--r--   0        0        0    10848 2022-10-12 17:08:47.786354 LightAutoML-0.3.7.3/lightautoml/addons/autots/base.py
--rw-r--r--   0        0        0      124 2022-10-12 17:08:47.786354 LightAutoML-0.3.7.3/lightautoml/addons/interpretation/__init__.py
--rw-r--r--   0        0        0     9909 2022-10-12 17:08:47.786354 LightAutoML-0.3.7.3/lightautoml/addons/interpretation/data_process.py
--rw-r--r--   0        0        0    30205 2022-10-12 17:08:47.786354 LightAutoML-0.3.7.3/lightautoml/addons/interpretation/l2x.py
--rw-r--r--   0        0        0     9455 2022-10-12 17:08:47.786354 LightAutoML-0.3.7.3/lightautoml/addons/interpretation/l2x_model.py
--rw-r--r--   0        0        0    14351 2022-10-12 17:08:47.786354 LightAutoML-0.3.7.3/lightautoml/addons/interpretation/lime.py
--rw-r--r--   0        0        0    12052 2022-10-12 17:08:47.786354 LightAutoML-0.3.7.3/lightautoml/addons/interpretation/utils.py
--rw-r--r--   0        0        0        0 2022-10-12 16:46:07.513702 LightAutoML-0.3.7.3/lightautoml/addons/uplift/__init__.py
--rw-r--r--   0        0        0    64472 2022-11-03 23:12:59.391201 LightAutoML-0.3.7.3/lightautoml/addons/uplift/base.py
--rw-r--r--   0        0        0    35712 2022-11-01 23:09:09.227364 LightAutoML-0.3.7.3/lightautoml/addons/uplift/metalearners.py
--rw-r--r--   0        0        0     8446 2022-11-03 23:12:59.391201 LightAutoML-0.3.7.3/lightautoml/addons/uplift/metrics.py
--rw-r--r--   0        0        0     3184 2022-11-01 23:09:15.519442 LightAutoML-0.3.7.3/lightautoml/addons/uplift/utils.py
--rw-r--r--   0        0        0      121 2022-10-12 17:08:47.786354 LightAutoML-0.3.7.3/lightautoml/addons/utilization/__init__.py
--rw-r--r--   0        0        0    15171 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/addons/utilization/utilization.py
--rw-r--r--   0        0        0      129 2022-10-12 16:46:07.517702 LightAutoML-0.3.7.3/lightautoml/automl/__init__.py
--rw-r--r--   0        0        0    12666 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/base.py
--rw-r--r--   0        0        0    13995 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/blend.py
--rw-r--r--   0        0        0      178 2022-10-12 16:46:07.517702 LightAutoML-0.3.7.3/lightautoml/automl/presets/__init__.py
--rw-r--r--   0        0        0     9292 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/base.py
--rw-r--r--   0        0        0     7032 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/image_config.yml
--rw-r--r--   0        0        0    13110 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/image_presets.py
--rw-r--r--   0        0        0     6868 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/tabular_config.yml
--rw-r--r--   0        0        0     4300 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/tabular_configs/conf_0_sel_type_0.yml
--rw-r--r--   0        0        0     4328 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/tabular_configs/conf_1_sel_type_1.yml
--rw-r--r--   0        0        0     4329 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/tabular_configs/conf_2_select_mode_1_no_typ.yml
--rw-r--r--   0        0        0     4328 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/tabular_configs/conf_3_sel_type_1_no_inter_lgbm.yml
--rw-r--r--   0        0        0     4328 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/tabular_configs/conf_4_sel_type_0_no_int.yml
--rw-r--r--   0        0        0     4329 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/tabular_configs/conf_5_sel_type_1_tuning_full.yml
--rw-r--r--   0        0        0     4328 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/tabular_configs/conf_6_sel_type_1_tuning_full_no_int_lgbm.yml
--rw-r--r--   0        0        0    38928 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/tabular_presets.py
--rw-r--r--   0        0        0    13221 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/text_config.yml
--rw-r--r--   0        0        0    15326 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/text_presets.py
--rw-r--r--   0        0        0     6181 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/utils.py
--rw-r--r--   0        0        0     7653 2022-10-12 16:46:07.521702 LightAutoML-0.3.7.3/lightautoml/automl/presets/whitebox_config.yml
--rw-r--r--   0        0        0     8526 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/automl/presets/whitebox_presets.py
--rw-r--r--   0        0        0      115 2022-10-12 16:46:07.521702 LightAutoML-0.3.7.3/lightautoml/dataset/__init__.py
--rw-r--r--   0        0        0    13965 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/dataset/base.py
--rw-r--r--   0        0        0    20082 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/dataset/np_pd_dataset.py
--rw-r--r--   0        0        0     8430 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/dataset/roles.py
--rw-r--r--   0        0        0    15125 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/dataset/seq_np_pd_dataset.py
--rw-r--r--   0        0        0     4577 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/dataset/utils.py
--rw-r--r--   0        0        0       92 2022-10-12 16:46:07.521702 LightAutoML-0.3.7.3/lightautoml/image/__init__.py
--rw-r--r--   0        0        0     9032 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/image/image.py
--rw-r--r--   0        0        0      298 2022-10-12 16:46:07.521702 LightAutoML-0.3.7.3/lightautoml/image/utils.py
--rw-r--r--   0        0        0      223 2022-10-12 16:46:07.521702 LightAutoML-0.3.7.3/lightautoml/ml_algo/__init__.py
--rwxr-xr-x   0        0        0    10371 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/ml_algo/base.py
--rwxr-xr-x   0        0        0    12096 2022-11-01 23:07:28.446121 LightAutoML-0.3.7.3/lightautoml/ml_algo/boost_cb.py
--rwxr-xr-x   0        0        0     9464 2022-11-01 23:07:28.446121 LightAutoML-0.3.7.3/lightautoml/ml_algo/boost_lgbm.py
--rw-r--r--   0        0        0    12281 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/ml_algo/dl_model.py
--rw-r--r--   0        0        0    10807 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/ml_algo/linear_sklearn.py
--rw-r--r--   0        0        0     7156 2022-11-01 23:07:28.446121 LightAutoML-0.3.7.3/lightautoml/ml_algo/random_forest.py
--rw-r--r--   0        0        0       37 2022-10-12 16:46:07.521702 LightAutoML-0.3.7.3/lightautoml/ml_algo/torch_based/__init__.py
--rw-r--r--   0        0        0    17364 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/ml_algo/torch_based/linear_model.py
--rw-r--r--   0        0        0       81 2022-10-12 16:46:07.525702 LightAutoML-0.3.7.3/lightautoml/ml_algo/tuning/__init__.py
--rw-r--r--   0        0        0     3051 2022-11-01 23:07:28.446121 LightAutoML-0.3.7.3/lightautoml/ml_algo/tuning/base.py
--rw-r--r--   0        0        0       65 2022-11-01 23:07:28.446121 LightAutoML-0.3.7.3/lightautoml/ml_algo/tuning/hyperopt.py
--rw-r--r--   0        0        0     9971 2022-11-01 23:07:28.446121 LightAutoML-0.3.7.3/lightautoml/ml_algo/tuning/optuna.py
--rw-r--r--   0        0        0     2293 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/ml_algo/utils.py
--rw-r--r--   0        0        0    10600 2022-10-12 17:08:47.790355 LightAutoML-0.3.7.3/lightautoml/ml_algo/whitebox.py
--rw-r--r--   0        0        0       98 2022-10-12 16:46:07.525702 LightAutoML-0.3.7.3/lightautoml/pipelines/__init__.py
--rw-r--r--   0        0        0      173 2022-10-12 16:46:07.525702 LightAutoML-0.3.7.3/lightautoml/pipelines/features/__init__.py
--rw-r--r--   0        0        0    17688 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/pipelines/features/base.py
--rw-r--r--   0        0        0     3739 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/pipelines/features/generator_pipeline.py
--rw-r--r--   0        0        0     3719 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/pipelines/features/image_pipeline.py
--rw-r--r--   0        0        0    19753 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/pipelines/features/lgb_pipeline.py
--rw-r--r--   0        0        0     9014 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/pipelines/features/linear_pipeline.py
--rw-r--r--   0        0        0     6803 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/pipelines/features/text_pipeline.py
--rw-r--r--   0        0        0     1218 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/pipelines/features/wb_pipeline.py
--rw-r--r--   0        0        0       85 2022-10-12 16:46:07.525702 LightAutoML-0.3.7.3/lightautoml/pipelines/ml/__init__.py
--rw-r--r--   0        0        0     6230 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/pipelines/ml/base.py
--rw-r--r--   0        0        0     8193 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/pipelines/ml/nested_ml_pipe.py
--rw-r--r--   0        0        0     3524 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/pipelines/ml/whitebox_ml_pipe.py
--rw-r--r--   0        0        0      159 2022-10-12 16:46:07.525702 LightAutoML-0.3.7.3/lightautoml/pipelines/selection/__init__.py
--rw-r--r--   0        0        0     9468 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/pipelines/selection/base.py
--rw-r--r--   0        0        0     2615 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/pipelines/selection/importance_based.py
--rw-r--r--   0        0        0     2813 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/pipelines/selection/linear_selector.py
--rw-r--r--   0        0        0     7495 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/pipelines/selection/permutation_importance_based.py
--rw-r--r--   0        0        0     2254 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/pipelines/utils.py
--rw-r--r--   0        0        0      101 2022-10-12 16:46:07.529702 LightAutoML-0.3.7.3/lightautoml/reader/__init__.py
--rw-r--r--   0        0        0    42646 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/reader/base.py
--rw-r--r--   0        0        0    18564 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/reader/guess_roles.py
--rw-r--r--   0        0        0     4666 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/reader/seq.py
--rw-r--r--   0        0        0    13393 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/reader/tabular_batch_generator.py
--rw-r--r--   0        0        0     1384 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/reader/utils.py
--rw-r--r--   0        0        0      322 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/report/__init__.py
--rw-r--r--   0        0        0     1290 2022-10-12 16:46:07.529702 LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/binary_inference_section.html
--rw-r--r--   0        0        0      422 2022-10-12 16:46:07.529702 LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/feature_importance_section.html
--rw-r--r--   0        0        0      378 2022-10-12 16:46:07.529702 LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/interpretation_section.html
--rw-r--r--   0        0        0      196 2022-10-12 16:46:07.529702 LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/interpretation_subsection.html
--rw-r--r--   0        0        0     2378 2022-10-12 16:46:07.529702 LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/lama_base_template.html
--rw-r--r--   0        0        0      853 2022-10-12 16:46:07.529702 LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/model_section.html
--rw-r--r--   0        0        0      599 2022-10-12 16:46:07.529702 LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/multiclass_inference_section.html
--rw-r--r--   0        0        0      208 2022-10-12 16:46:07.529702 LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/nlp_section.html
--rw-r--r--   0        0        0      238 2022-10-12 16:46:07.529702 LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/nlp_subsection.html
--rw-r--r--   0        0        0      801 2022-10-12 16:46:07.529702 LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/reg_inference_section.html
--rw-r--r--   0        0        0      217 2022-10-12 16:46:07.529702 LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/results_section.html
--rw-r--r--   0        0        0     3005 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/train_set_section.html
--rw-r--r--   0        0        0      214 2022-10-12 16:46:07.529702 LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/uplift_section.html
--rw-r--r--   0        0        0      928 2022-10-12 16:46:07.529702 LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/uplift_subsection.html
--rw-r--r--   0        0        0    12980 2022-10-12 16:46:07.533702 LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/whitebox_section.html
--rw-r--r--   0        0        0    80150 2022-11-03 23:12:59.391201 LightAutoML-0.3.7.3/lightautoml/report/report_deco.py
--rw-r--r--   0        0        0      138 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/tasks/__init__.py
--rw-r--r--   0        0        0    14858 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/tasks/base.py
--rw-r--r--   0        0        0    10624 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/tasks/common_metric.py
--rw-r--r--   0        0        0      386 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/tasks/losses/__init__.py
--rw-r--r--   0        0        0     4239 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/tasks/losses/base.py
--rw-r--r--   0        0        0     6259 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/tasks/losses/cb.py
--rw-r--r--   0        0        0     3949 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/tasks/losses/cb_custom.py
--rw-r--r--   0        0        0     7707 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/tasks/losses/lgb.py
--rw-r--r--   0        0        0     1201 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/tasks/losses/lgb_custom.py
--rw-r--r--   0        0        0     2532 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/tasks/losses/sklearn.py
--rw-r--r--   0        0        0     6902 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/tasks/losses/torch.py
--rw-r--r--   0        0        0     1238 2022-10-12 17:08:47.794355 LightAutoML-0.3.7.3/lightautoml/tasks/utils.py
--rw-r--r--   0        0        0      206 2022-10-12 16:46:07.533702 LightAutoML-0.3.7.3/lightautoml/text/__init__.py
--rw-r--r--   0        0        0    14693 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/text/dl_transformers.py
--rw-r--r--   0        0        0     4608 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/text/dp_utils.py
--rw-r--r--   0        0        0     2600 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/text/embed_dataset.py
--rw-r--r--   0        0        0    10138 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/text/nn_model.py
--rw-r--r--   0        0        0     2143 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/text/sentence_pooling.py
--rw-r--r--   0        0        0    10337 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/text/tokenizer.py
--rw-r--r--   0        0        0    18150 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/text/trainer.py
--rw-r--r--   0        0        0     4659 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/text/utils.py
--rw-r--r--   0        0        0     4491 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/text/weighted_average_transformer.py
--rw-r--r--   0        0        0      113 2022-10-12 16:46:07.537702 LightAutoML-0.3.7.3/lightautoml/transformers/__init__.py
--rw-r--r--   0        0        0    15540 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/transformers/base.py
--rw-r--r--   0        0        0    30748 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/transformers/categorical.py
--rw-r--r--   0        0        0     7530 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/transformers/datetime.py
--rw-r--r--   0        0        0     5851 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/transformers/decomposition.py
--rw-r--r--   0        0        0    13484 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/transformers/generator.py
--rw-r--r--   0        0        0     8553 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/transformers/image.py
--rw-r--r--   0        0        0     9262 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/transformers/numeric.py
--rw-r--r--   0        0        0     7201 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/transformers/seq.py
--rw-r--r--   0        0        0    26966 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/transformers/text.py
--rw-r--r--   0        0        0       46 2022-10-12 16:46:07.537702 LightAutoML-0.3.7.3/lightautoml/utils/__init__.py
--rw-r--r--   0        0        0     1318 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/utils/installation.py
--rwxr-xr-x   0        0        0     5744 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/utils/logging.py
--rw-r--r--   0        0        0     9787 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/utils/timer.py
--rw-r--r--   0        0        0      114 2022-10-12 16:46:07.537702 LightAutoML-0.3.7.3/lightautoml/validation/__init__.py
--rw-r--r--   0        0        0     7571 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/validation/base.py
--rw-r--r--   0        0        0     8952 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/validation/np_iterators.py
--rw-r--r--   0        0        0     1819 2022-10-12 17:08:47.798354 LightAutoML-0.3.7.3/lightautoml/validation/utils.py
--rw-r--r--   0        0        0     4403 2022-11-07 09:07:30.005942 LightAutoML-0.3.7.3/pyproject.toml
--rw-r--r--   0        0        0    15726 2022-11-07 09:08:33.549104 LightAutoML-0.3.7.3/setup.py
--rw-r--r--   0        0        0    15327 2022-11-07 09:08:33.549690 LightAutoML-0.3.7.3/PKG-INFO
+-rw-r--r--   0        0        0    11454 2023-07-25 08:32:37.984981 lightautoml-0.3.8b1/LICENSE
+-rw-r--r--   0        0        0    13285 2023-07-26 10:03:22.588034 lightautoml-0.3.8b1/README.md
+-rw-r--r--   0        0        0      793 2023-07-25 08:32:38.140992 lightautoml-0.3.8b1/lightautoml/__init__.py
+-rw-r--r--   0        0        0      105 2023-07-25 08:32:38.317003 lightautoml-0.3.8b1/lightautoml/addons/__init__.py
+-rw-r--r--   0        0        0     9582 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/addons/autots/base.py
+-rw-r--r--   0        0        0      328 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/addons/hypex/README.md
+-rw-r--r--   0        0        0       53 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/addons/hypex/__init__.py
+-rw-r--r--   0        0        0    29375 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/addons/hypex/algorithms/faiss_matcher.py
+-rw-r--r--   0        0        0    16500 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/addons/hypex/matcher.py
+-rw-r--r--   0        0        0     3717 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/addons/hypex/selectors/lama_feature_selector.py
+-rw-r--r--   0        0        0     3345 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/addons/hypex/selectors/outliers_filter.py
+-rw-r--r--   0        0        0     2504 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/addons/hypex/selectors/spearman_filter.py
+-rw-r--r--   0        0        0     5944 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/addons/hypex/utils/metrics.py
+-rw-r--r--   0        0        0    19272 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/addons/hypex/utils/psi_pandas.py
+-rw-r--r--   0        0        0     2584 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/addons/hypex/utils/validators.py
+-rw-r--r--   0        0        0      124 2023-07-25 08:32:38.613022 lightautoml-0.3.8b1/lightautoml/addons/interpretation/__init__.py
+-rw-r--r--   0        0        0     9909 2023-07-25 08:32:38.617023 lightautoml-0.3.8b1/lightautoml/addons/interpretation/data_process.py
+-rw-r--r--   0        0        0    30205 2023-07-25 08:32:38.617023 lightautoml-0.3.8b1/lightautoml/addons/interpretation/l2x.py
+-rw-r--r--   0        0        0     9455 2023-07-25 08:32:38.625023 lightautoml-0.3.8b1/lightautoml/addons/interpretation/l2x_model.py
+-rw-r--r--   0        0        0    14351 2023-07-25 08:32:38.625023 lightautoml-0.3.8b1/lightautoml/addons/interpretation/lime.py
+-rw-r--r--   0        0        0    12052 2023-07-25 08:32:38.625023 lightautoml-0.3.8b1/lightautoml/addons/interpretation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-25 08:32:38.413009 lightautoml-0.3.8b1/lightautoml/addons/uplift/__init__.py
+-rw-r--r--   0        0        0    64472 2023-07-25 08:32:38.617023 lightautoml-0.3.8b1/lightautoml/addons/uplift/base.py
+-rw-r--r--   0        0        0    35712 2023-07-25 08:32:38.625023 lightautoml-0.3.8b1/lightautoml/addons/uplift/metalearners.py
+-rw-r--r--   0        0        0     8446 2023-07-25 08:32:38.625023 lightautoml-0.3.8b1/lightautoml/addons/uplift/metrics.py
+-rw-r--r--   0        0        0     3184 2023-07-25 08:32:38.633024 lightautoml-0.3.8b1/lightautoml/addons/uplift/utils.py
+-rw-r--r--   0        0        0      121 2023-07-25 08:32:38.613022 lightautoml-0.3.8b1/lightautoml/addons/utilization/__init__.py
+-rw-r--r--   0        0        0    15171 2023-07-25 08:32:38.613022 lightautoml-0.3.8b1/lightautoml/addons/utilization/utilization.py
+-rw-r--r--   0        0        0      129 2023-07-25 08:32:38.317003 lightautoml-0.3.8b1/lightautoml/automl/__init__.py
+-rw-r--r--   0        0        0    12987 2023-07-25 08:32:38.317003 lightautoml-0.3.8b1/lightautoml/automl/base.py
+-rw-r--r--   0        0        0    13995 2023-07-25 08:32:38.317003 lightautoml-0.3.8b1/lightautoml/automl/blend.py
+-rw-r--r--   0        0        0      178 2023-07-25 08:32:38.625023 lightautoml-0.3.8b1/lightautoml/automl/presets/__init__.py
+-rw-r--r--   0        0        0     9348 2023-07-25 08:32:38.633024 lightautoml-0.3.8b1/lightautoml/automl/presets/base.py
+-rwxr-xr-x   0        0        0     8346 2023-07-26 12:39:23.566758 lightautoml-0.3.8b1/lightautoml/automl/presets/image_config.yml
+-rwxr-xr-x   0        0        0    13134 2023-07-26 12:39:23.566758 lightautoml-0.3.8b1/lightautoml/automl/presets/image_presets.py
+-rwxr-xr-x   0        0        0    13158 2023-07-26 12:39:23.566758 lightautoml-0.3.8b1/lightautoml/automl/presets/tabular_config.yml
+-rw-r--r--   0        0        0     9276 2023-07-25 08:32:38.789034 lightautoml-0.3.8b1/lightautoml/automl/presets/tabular_configs/conf_0_sel_type_0.yml
+-rw-r--r--   0        0        0     9304 2023-07-25 08:32:38.797035 lightautoml-0.3.8b1/lightautoml/automl/presets/tabular_configs/conf_1_sel_type_1.yml
+-rw-r--r--   0        0        0     9305 2023-07-25 08:32:38.797035 lightautoml-0.3.8b1/lightautoml/automl/presets/tabular_configs/conf_2_select_mode_1_no_typ.yml
+-rw-r--r--   0        0        0     9304 2023-07-25 08:32:38.797035 lightautoml-0.3.8b1/lightautoml/automl/presets/tabular_configs/conf_3_sel_type_1_no_inter_lgbm.yml
+-rw-r--r--   0        0        0     9304 2023-07-25 08:32:38.797035 lightautoml-0.3.8b1/lightautoml/automl/presets/tabular_configs/conf_4_sel_type_0_no_int.yml
+-rw-r--r--   0        0        0     9305 2023-07-25 08:32:38.801035 lightautoml-0.3.8b1/lightautoml/automl/presets/tabular_configs/conf_5_sel_type_1_tuning_full.yml
+-rw-r--r--   0        0        0     9304 2023-07-25 08:32:38.801035 lightautoml-0.3.8b1/lightautoml/automl/presets/tabular_configs/conf_6_sel_type_1_tuning_full_no_int_lgbm.yml
+-rwxr-xr-x   0        0        0    45760 2023-07-26 12:39:23.566758 lightautoml-0.3.8b1/lightautoml/automl/presets/tabular_presets.py
+-rwxr-xr-x   0        0        0    14558 2023-07-26 12:39:23.566758 lightautoml-0.3.8b1/lightautoml/automl/presets/text_config.yml
+-rwxr-xr-x   0        0        0    17696 2023-07-26 12:39:23.566758 lightautoml-0.3.8b1/lightautoml/automl/presets/text_presets.py
+-rw-r--r--   0        0        0    12895 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/automl/presets/time_series_config.yml
+-rw-r--r--   0        0        0     6181 2023-07-25 08:32:38.645025 lightautoml-0.3.8b1/lightautoml/automl/presets/utils.py
+-rw-r--r--   0        0        0     7653 2023-07-25 08:32:38.645025 lightautoml-0.3.8b1/lightautoml/automl/presets/whitebox_config.yml
+-rw-r--r--   0        0        0     8526 2023-07-25 08:32:38.661026 lightautoml-0.3.8b1/lightautoml/automl/presets/whitebox_presets.py
+-rw-r--r--   0        0        0      115 2023-07-25 08:32:38.333004 lightautoml-0.3.8b1/lightautoml/dataset/__init__.py
+-rw-r--r--   0        0        0    13965 2023-07-25 08:32:38.333004 lightautoml-0.3.8b1/lightautoml/dataset/base.py
+-rw-r--r--   0        0        0    20082 2023-07-25 08:32:38.333004 lightautoml-0.3.8b1/lightautoml/dataset/np_pd_dataset.py
+-rw-r--r--   0        0        0     8430 2023-07-25 08:32:38.333004 lightautoml-0.3.8b1/lightautoml/dataset/roles.py
+-rw-r--r--   0        0        0    15125 2023-07-25 08:32:38.349005 lightautoml-0.3.8b1/lightautoml/dataset/seq_np_pd_dataset.py
+-rw-r--r--   0        0        0     4577 2023-07-25 08:32:38.349005 lightautoml-0.3.8b1/lightautoml/dataset/utils.py
+-rw-r--r--   0        0        0       92 2023-07-25 08:32:38.317003 lightautoml-0.3.8b1/lightautoml/image/__init__.py
+-rw-r--r--   0        0        0     9032 2023-07-25 08:32:38.317003 lightautoml-0.3.8b1/lightautoml/image/image.py
+-rw-r--r--   0        0        0      298 2023-07-25 08:32:38.317003 lightautoml-0.3.8b1/lightautoml/image/utils.py
+-rw-r--r--   0        0        0      242 2023-07-25 08:32:38.317003 lightautoml-0.3.8b1/lightautoml/ml_algo/__init__.py
+-rwxr-xr-x   0        0        0    10371 2023-07-25 08:50:25.191554 lightautoml-0.3.8b1/lightautoml/ml_algo/base.py
+-rwxr-xr-x   0        0        0    12096 2023-07-25 08:50:44.648957 lightautoml-0.3.8b1/lightautoml/ml_algo/boost_cb.py
+-rwxr-xr-x   0        0        0     9464 2023-07-25 08:50:48.241216 lightautoml-0.3.8b1/lightautoml/ml_algo/boost_lgbm.py
+-rw-r--r--   0        0        0    19312 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/ml_algo/dl_model.py
+-rw-r--r--   0        0        0    10807 2023-07-25 08:32:38.325003 lightautoml-0.3.8b1/lightautoml/ml_algo/linear_sklearn.py
+-rw-r--r--   0        0        0     7183 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/ml_algo/random_forest.py
+-rw-r--r--   0        0        0       78 2023-07-25 08:32:38.673026 lightautoml-0.3.8b1/lightautoml/ml_algo/torch_based/__init__.py
+-rw-r--r--   0        0        0    16882 2023-07-25 08:32:38.673026 lightautoml-0.3.8b1/lightautoml/ml_algo/torch_based/linear_model.py
+-rw-r--r--   0        0        0    22944 2023-07-25 08:32:38.673026 lightautoml-0.3.8b1/lightautoml/ml_algo/torch_based/nn_models.py
+-rw-r--r--   0        0        0       81 2023-07-25 08:32:38.705028 lightautoml-0.3.8b1/lightautoml/ml_algo/tuning/__init__.py
+-rw-r--r--   0        0        0     3051 2023-07-25 08:32:38.673026 lightautoml-0.3.8b1/lightautoml/ml_algo/tuning/base.py
+-rw-r--r--   0        0        0       65 2023-07-25 08:32:38.673026 lightautoml-0.3.8b1/lightautoml/ml_algo/tuning/hyperopt.py
+-rw-r--r--   0        0        0    18027 2023-07-25 08:32:38.693028 lightautoml-0.3.8b1/lightautoml/ml_algo/tuning/optuna.py
+-rw-r--r--   0        0        0     2569 2023-07-25 08:32:38.329004 lightautoml-0.3.8b1/lightautoml/ml_algo/utils.py
+-rw-r--r--   0        0        0    10600 2023-07-25 08:32:38.333004 lightautoml-0.3.8b1/lightautoml/ml_algo/whitebox.py
+-rw-r--r--   0        0        0       98 2023-07-25 08:32:38.349005 lightautoml-0.3.8b1/lightautoml/pipelines/__init__.py
+-rw-r--r--   0        0        0      195 2023-07-25 08:32:38.693028 lightautoml-0.3.8b1/lightautoml/pipelines/features/__init__.py
+-rwxr-xr-x   0        0        0    23594 2023-07-26 12:39:23.566758 lightautoml-0.3.8b1/lightautoml/pipelines/features/base.py
+-rw-r--r--   0        0        0     3739 2023-07-25 08:32:38.649025 lightautoml-0.3.8b1/lightautoml/pipelines/features/generator_pipeline.py
+-rw-r--r--   0        0        0     3719 2023-07-25 08:32:38.649025 lightautoml-0.3.8b1/lightautoml/pipelines/features/image_pipeline.py
+-rwxr-xr-x   0        0        0    23101 2023-07-26 12:39:23.566758 lightautoml-0.3.8b1/lightautoml/pipelines/features/lgb_pipeline.py
+-rwxr-xr-x   0        0        0     9808 2023-07-26 12:39:23.566758 lightautoml-0.3.8b1/lightautoml/pipelines/features/linear_pipeline.py
+-rw-r--r--   0        0        0     6803 2023-07-25 08:32:38.661026 lightautoml-0.3.8b1/lightautoml/pipelines/features/text_pipeline.py
+-rw-r--r--   0        0        0     6635 2023-07-25 08:32:38.673026 lightautoml-0.3.8b1/lightautoml/pipelines/features/torch_pipeline.py
+-rw-r--r--   0        0        0     1218 2023-07-25 08:32:38.661026 lightautoml-0.3.8b1/lightautoml/pipelines/features/wb_pipeline.py
+-rw-r--r--   0        0        0       85 2023-07-25 08:32:38.661026 lightautoml-0.3.8b1/lightautoml/pipelines/ml/__init__.py
+-rw-r--r--   0        0        0     6288 2023-07-25 08:32:38.661026 lightautoml-0.3.8b1/lightautoml/pipelines/ml/base.py
+-rw-r--r--   0        0        0     8193 2023-07-25 08:32:38.693028 lightautoml-0.3.8b1/lightautoml/pipelines/ml/nested_ml_pipe.py
+-rw-r--r--   0        0        0     3524 2023-07-25 08:32:38.673026 lightautoml-0.3.8b1/lightautoml/pipelines/ml/whitebox_ml_pipe.py
+-rw-r--r--   0        0        0      159 2023-07-25 08:32:38.701028 lightautoml-0.3.8b1/lightautoml/pipelines/selection/__init__.py
+-rw-r--r--   0        0        0     9400 2023-07-25 08:32:38.701028 lightautoml-0.3.8b1/lightautoml/pipelines/selection/base.py
+-rw-r--r--   0        0        0     2615 2023-07-25 08:32:38.701028 lightautoml-0.3.8b1/lightautoml/pipelines/selection/importance_based.py
+-rw-r--r--   0        0        0     2817 2023-07-25 08:32:38.701028 lightautoml-0.3.8b1/lightautoml/pipelines/selection/linear_selector.py
+-rw-r--r--   0        0        0     7499 2023-07-25 08:32:38.701028 lightautoml-0.3.8b1/lightautoml/pipelines/selection/permutation_importance_based.py
+-rw-r--r--   0        0        0     2254 2023-07-25 08:32:38.349005 lightautoml-0.3.8b1/lightautoml/pipelines/utils.py
+-rw-r--r--   0        0        0      101 2023-07-25 08:32:38.349005 lightautoml-0.3.8b1/lightautoml/reader/__init__.py
+-rw-r--r--   0        0        0    42642 2023-07-25 08:32:38.349005 lightautoml-0.3.8b1/lightautoml/reader/base.py
+-rw-r--r--   0        0        0    18678 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/reader/guess_roles.py
+-rw-r--r--   0        0        0     4666 2023-07-25 08:32:38.353005 lightautoml-0.3.8b1/lightautoml/reader/seq.py
+-rw-r--r--   0        0        0    13393 2023-07-25 08:32:38.353005 lightautoml-0.3.8b1/lightautoml/reader/tabular_batch_generator.py
+-rw-r--r--   0        0        0     1384 2023-07-25 08:32:38.353005 lightautoml-0.3.8b1/lightautoml/reader/utils.py
+-rw-r--r--   0        0        0      322 2023-07-25 08:32:38.353005 lightautoml-0.3.8b1/lightautoml/report/__init__.py
+-rw-r--r--   0        0        0     1290 2023-07-25 08:32:38.673026 lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/binary_inference_section.html
+-rw-r--r--   0        0        0      422 2023-07-25 08:32:38.693028 lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/feature_importance_section.html
+-rw-r--r--   0        0        0      378 2023-07-25 08:32:38.693028 lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/interpretation_section.html
+-rw-r--r--   0        0        0      196 2023-07-25 08:32:38.701028 lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/interpretation_subsection.html
+-rw-r--r--   0        0        0     2378 2023-07-25 08:32:38.693028 lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/lama_base_template.html
+-rw-r--r--   0        0        0      853 2023-07-25 08:32:38.693028 lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/model_section.html
+-rw-r--r--   0        0        0      599 2023-07-25 08:32:38.693028 lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/multiclass_inference_section.html
+-rw-r--r--   0        0        0      208 2023-07-25 08:32:38.705028 lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/nlp_section.html
+-rw-r--r--   0        0        0      238 2023-07-25 08:32:38.693028 lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/nlp_subsection.html
+-rw-r--r--   0        0        0      801 2023-07-25 08:32:38.693028 lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/reg_inference_section.html
+-rw-r--r--   0        0        0      217 2023-07-25 08:32:38.701028 lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/results_section.html
+-rw-r--r--   0        0        0     3005 2023-07-25 08:32:38.701028 lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/train_set_section.html
+-rw-r--r--   0        0        0      214 2023-07-25 08:32:38.701028 lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/uplift_section.html
+-rw-r--r--   0        0        0      928 2023-07-25 08:32:38.701028 lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/uplift_subsection.html
+-rw-r--r--   0        0        0    12980 2023-07-25 08:32:38.705028 lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/whitebox_section.html
+-rw-r--r--   0        0        0    80150 2023-07-25 08:32:38.361006 lightautoml-0.3.8b1/lightautoml/report/report_deco.py
+-rw-r--r--   0        0        0      138 2023-07-25 08:32:38.357006 lightautoml-0.3.8b1/lightautoml/tasks/__init__.py
+-rw-r--r--   0        0        0    14858 2023-07-25 08:32:38.361006 lightautoml-0.3.8b1/lightautoml/tasks/base.py
+-rw-r--r--   0        0        0    10624 2023-07-25 08:32:38.357006 lightautoml-0.3.8b1/lightautoml/tasks/common_metric.py
+-rw-r--r--   0        0        0      386 2023-07-25 08:32:38.717029 lightautoml-0.3.8b1/lightautoml/tasks/losses/__init__.py
+-rw-r--r--   0        0        0     4239 2023-07-25 08:32:38.717029 lightautoml-0.3.8b1/lightautoml/tasks/losses/base.py
+-rw-r--r--   0        0        0     6783 2023-07-25 08:32:38.717029 lightautoml-0.3.8b1/lightautoml/tasks/losses/cb.py
+-rw-r--r--   0        0        0     3949 2023-07-25 08:32:38.717029 lightautoml-0.3.8b1/lightautoml/tasks/losses/cb_custom.py
+-rw-r--r--   0        0        0     7707 2023-07-25 08:32:38.717029 lightautoml-0.3.8b1/lightautoml/tasks/losses/lgb.py
+-rw-r--r--   0        0        0     1201 2023-07-25 08:32:38.717029 lightautoml-0.3.8b1/lightautoml/tasks/losses/lgb_custom.py
+-rw-r--r--   0        0        0     2532 2023-07-25 08:32:38.717029 lightautoml-0.3.8b1/lightautoml/tasks/losses/sklearn.py
+-rw-r--r--   0        0        0     6948 2023-07-25 08:32:38.717029 lightautoml-0.3.8b1/lightautoml/tasks/losses/torch.py
+-rw-r--r--   0        0        0     1238 2023-07-25 08:32:38.361006 lightautoml-0.3.8b1/lightautoml/tasks/utils.py
+-rw-r--r--   0        0        0      206 2023-07-25 08:32:38.381007 lightautoml-0.3.8b1/lightautoml/text/__init__.py
+-rw-r--r--   0        0        0    14763 2023-07-25 08:32:38.361006 lightautoml-0.3.8b1/lightautoml/text/dl_transformers.py
+-rw-r--r--   0        0        0     4608 2023-07-25 08:32:38.401008 lightautoml-0.3.8b1/lightautoml/text/dp_utils.py
+-rw-r--r--   0        0        0     2600 2023-07-25 08:32:38.381007 lightautoml-0.3.8b1/lightautoml/text/embed_dataset.py
+-rw-r--r--   0        0        0    11991 2023-07-25 08:32:38.405009 lightautoml-0.3.8b1/lightautoml/text/nn_model.py
+-rw-r--r--   0        0        0    10337 2023-07-25 08:32:38.381007 lightautoml-0.3.8b1/lightautoml/text/tokenizer.py
+-rw-r--r--   0        0        0    19072 2023-07-25 08:32:38.381007 lightautoml-0.3.8b1/lightautoml/text/trainer.py
+-rw-r--r--   0        0        0     4659 2023-07-25 08:32:38.381007 lightautoml-0.3.8b1/lightautoml/text/utils.py
+-rw-r--r--   0        0        0     4491 2023-07-25 08:32:38.381007 lightautoml-0.3.8b1/lightautoml/text/weighted_average_transformer.py
+-rw-r--r--   0        0        0      135 2023-07-26 12:39:23.566758 lightautoml-0.3.8b1/lightautoml/transformers/__init__.py
+-rw-r--r--   0        0        0    15540 2023-07-25 08:32:38.401008 lightautoml-0.3.8b1/lightautoml/transformers/base.py
+-rw-r--r--   0        0        0    30777 2023-07-25 08:32:38.401008 lightautoml-0.3.8b1/lightautoml/transformers/categorical.py
+-rw-r--r--   0        0        0     6032 2023-07-26 12:39:23.566758 lightautoml-0.3.8b1/lightautoml/transformers/composite.py
+-rw-r--r--   0        0        0     7530 2023-07-25 08:32:38.401008 lightautoml-0.3.8b1/lightautoml/transformers/datetime.py
+-rw-r--r--   0        0        0     5851 2023-07-25 08:32:38.405009 lightautoml-0.3.8b1/lightautoml/transformers/decomposition.py
+-rw-r--r--   0        0        0    13485 2023-07-26 10:03:22.632037 lightautoml-0.3.8b1/lightautoml/transformers/generator.py
+-rw-r--r--   0        0        0     8358 2023-07-26 12:39:23.570758 lightautoml-0.3.8b1/lightautoml/transformers/groupby.py
+-rw-r--r--   0        0        0     8553 2023-07-25 08:32:38.413009 lightautoml-0.3.8b1/lightautoml/transformers/image.py
+-rw-r--r--   0        0        0    13666 2023-07-25 08:32:38.405009 lightautoml-0.3.8b1/lightautoml/transformers/numeric.py
+-rw-r--r--   0        0        0    10306 2023-07-25 08:32:38.405009 lightautoml-0.3.8b1/lightautoml/transformers/seq.py
+-rw-r--r--   0        0        0    26966 2023-07-25 08:32:38.409009 lightautoml-0.3.8b1/lightautoml/transformers/text.py
+-rw-r--r--   0        0        0     7152 2023-07-26 12:39:23.570758 lightautoml-0.3.8b1/lightautoml/transformers/utils.py
+-rw-r--r--   0        0        0       46 2023-07-25 08:32:38.381007 lightautoml-0.3.8b1/lightautoml/utils/__init__.py
+-rw-r--r--   0        0        0     1432 2023-07-25 08:32:38.401008 lightautoml-0.3.8b1/lightautoml/utils/installation.py
+-rwxr-xr-x   0        0        0     5744 2023-07-25 08:53:19.504143 lightautoml-0.3.8b1/lightautoml/utils/logging.py
+-rw-r--r--   0        0        0     9787 2023-07-25 08:32:38.405009 lightautoml-0.3.8b1/lightautoml/utils/timer.py
+-rw-r--r--   0        0        0      114 2023-07-25 08:32:38.409009 lightautoml-0.3.8b1/lightautoml/validation/__init__.py
+-rw-r--r--   0        0        0     7571 2023-07-25 08:32:38.413009 lightautoml-0.3.8b1/lightautoml/validation/base.py
+-rw-r--r--   0        0        0     8952 2023-07-25 08:32:38.413009 lightautoml-0.3.8b1/lightautoml/validation/np_iterators.py
+-rw-r--r--   0        0        0     1819 2023-07-25 08:32:38.413009 lightautoml-0.3.8b1/lightautoml/validation/utils.py
+-rw-r--r--   0        0        0     5744 2023-07-26 13:23:12.656330 lightautoml-0.3.8b1/pyproject.toml
+-rw-r--r--   0        0        0    17112 1970-01-01 00:00:00.000000 lightautoml-0.3.8b1/setup.py
+-rw-r--r--   0        0        0    16705 1970-01-01 00:00:00.000000 lightautoml-0.3.8b1/PKG-INFO
```

### Comparing `LightAutoML-0.3.7.3/LICENSE` & `lightautoml-0.3.8b1/LICENSE`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/README.md` & `lightautoml-0.3.8b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 # LightAutoML - automatic model creation framework
 
 [![Telegram](https://img.shields.io/badge/chat-on%20Telegram-2ba2d9.svg)](https://t.me/lightautoml)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/lightautoml?color=green&label=PyPI%20downloads&logo=pypi&logoColor=orange&style=plastic)
 ![Read the Docs](https://img.shields.io/readthedocs/lightautoml?style=plastic)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![Poetry-Lock](https://img.shields.io/github/workflow/status/sb-ai-lab/LightAutoML/Poetry%20run/master?label=Poetry-Lock)
+
 
 LightAutoML (LAMA) is an AutoML framework which provides automatic model creation for the following tasks:
 - binary classification
 - multiclass  classification
 - regression
 
 Current version of the package handles datasets that have independent samples in each row. I.e. **each row is an object with its specific features and target**.
@@ -117,26 +119,29 @@
 - [Titanic **12-code-lines** competition solution (78% accuracy)](https://www.kaggle.com/alexryzhkov/lightautoml-extreme-short-titanic-solution)
 - [House prices competition solution](https://www.kaggle.com/alexryzhkov/lightautoml-houseprices-love)
 - [Natural Language Processing with Disaster Tweets solution](https://www.kaggle.com/alexryzhkov/lightautoml-starter-nlp)
 - [Tabular Playground Series March 2021 competition solution](https://www.kaggle.com/alexryzhkov/lightautoml-starter-for-tabulardatamarch)
 - [Tabular Playground Series February 2021 competition solution](https://www.kaggle.com/alexryzhkov/lightautoml-tabulardata-love)
 - [Interpretable WhiteBox solution](https://www.kaggle.com/simakov/lama-whitebox-preset-example)
 - [Custom ML pipeline elements inside existing ones](https://www.kaggle.com/simakov/lama-custom-automl-pipeline-example)
+- [Custom ML pipeline elements inside existing ones](https://www.kaggle.com/simakov/lama-custom-automl-pipeline-example)
+- [Tabular Playground Series November 2022 competition solution with Neural Networks](https://www.kaggle.com/code/mikhailkuz/lightautoml-nn-happiness)
 
 ### Google Colab tutorials and [other examples](examples/):
 
 - [`Tutorial_1_basics.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_1_basics.ipynb) - get started with LightAutoML on tabular data.
 - [`Tutorial_2_WhiteBox_AutoWoE.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_2_WhiteBox_AutoWoE.ipynb) - creating interpretable models.
 - [`Tutorial_3_sql_data_source.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_3_sql_data_source.ipynb) - shows how to use LightAutoML presets (both standalone and time utilized variants) for solving ML tasks on tabular data from SQL data base instead of CSV.
 - [`Tutorial_4_NLP_Interpretation.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_4_NLP_Interpretation.ipynb) - example of using TabularNLPAutoML preset, LimeTextExplainer.
 - [`Tutorial_5_uplift.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_5_uplift.ipynb) - shows how to use LightAutoML for a uplift-modeling task.
 - [`Tutorial_6_custom_pipeline.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_6_custom_pipeline.ipynb) - shows how to create your own pipeline from specified blocks: pipelines for feature generation and feature selection, ML algorithms, hyperparameter optimization etc.
 - [`Tutorial_7_ICE_and_PDP_interpretation.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_7_ICE_and_PDP_interpretation.ipynb) - shows how to obtain local and global interpretation of model results using ICE and PDP approaches.
 - [`Tutorial_8_CV_preset.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_8_CV_preset.ipynb) - example of using TabularCVAutoML preset in CV multi-class classification task.
-
+- [`Tutorial_9_neural_networks.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_9_neural_networks.ipynb) - example of using Tabular preset with neural networks.
+- [`Tutorial_10_relational_data_with_star_scheme.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_10_relational_data_with_star_scheme.ipynb) - example of using Tabular preset with neural networks.
 
 **Note 1**: for production you have no need to use profiler (which increase work time and memory consomption), so please do not turn it on - it is in off state by default
 
 **Note 2**: to take a look at this report after the run, please comment last line of demo with report deletion command.
 
 ### Courses, videos and papers
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/__init__.py` & `lightautoml-0.3.8b1/lightautoml/__init__.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/addons/autots/base.py` & `lightautoml-0.3.8b1/lightautoml/addons/autots/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,41 @@
 # Standard python libraries
 import logging
+import os
 
-from copy import deepcopy
+import yaml
 
 
 logging.basicConfig(format="[%(asctime)s] (%(levelname)s): %(message)s", level=logging.INFO)
 
 # Installed libraries
 import numpy as np
 import pandas as pd
 
 from statsmodels.tsa.seasonal import STL
 from statsmodels.tsa.seasonal import seasonal_decompose
 
 # Imports from our package
 from ...automl.base import AutoML
-from ...automl.blend import WeightedBlender
+from ...automl.presets.base import upd_params
+from ...automl.presets.tabular_presets import TabularAutoML
 from ...dataset.roles import DatetimeRole
-from ...ml_algo.boost_cb import BoostCB
 from ...ml_algo.linear_sklearn import LinearLBFGS
-from ...ml_algo.random_forest import RandomForestSklearn
-from ...pipelines.features.lgb_pipeline import LGBSeqSimpleFeatures
 from ...pipelines.features.linear_pipeline import LinearTrendFeatures
 from ...pipelines.ml.base import MLPipeline
 from ...reader.base import DictToPandasSeqReader
 from ...tasks import Task
 
 
 class TrendModel:
 
     _available_trend_types = ["decompose", "decompose_STL", "linear", "rolling"]
-    default_params = {
-        "trend": True,
-        "train_on_trend": True,
-        "trend_type": "decompose",
-        "trend_size": 7,
-        "decompose_period": 30,
-        "detect_step_quantile": 0.01,
-        "detect_step_window": 7,
-        "detect_step_threshold": 0.7,
-        "rolling_size": 7,
-        "verbose": 0,
-    }
 
     def __init__(self, params=None):
-        self.params = deepcopy(self.default_params)
-        if params is not None:
-            self.params.update(params)
+        self.params = params
         assert self.params["trend_type"] in self._available_trend_types
 
     def _detect_step(self, x):
         x_min, x_max = tuple(
             np.quantile(x, [self.params["detect_step_quantile"], 1 - self.params["detect_step_quantile"]])
         )
         x_range = x_max - x_min
@@ -142,45 +127,31 @@
         else:
             trend = self._estimate_trend(data, self.roles)
         pred_trend = self.automl_trend.predict({"plain": future_time, "seq": None}).data[:, 0]
         return trend, pred_trend
 
 
 class AutoTS:
-
-    default_trend_params = {
-        "trend": True,
-        "train_on_trend": True,
-        "trend_type": "decompose",  # 'decompose', 'decompose_STL', 'linear' or 'rolling'
-        "trend_size": 7,
-        "decompose_period": 30,
-        "detect_step_quantile": 0.01,
-        "detect_step_window": 7,
-        "detect_step_threshold": 0.7,
-        "rolling_size": 7,
-        "verbose": 0,
-    }
-
     @property
     def n_target(self):
         """Get length of future prediction.
 
         Returns:
             length
         """
-        return self.seq_params["seq0"]["params"]["n_target"]
+        return self.reader_params["seq_params"]["seq0"]["params"]["n_target"]
 
     @property
     def n_history(self):
         """Get length of history used for feature generation.
 
         Returns:
             length
         """
-        return self.seq_params["seq0"]["params"]["history"]
+        return self.reader_params["seq_params"]["params"]["history"]
 
     @property
     def datetime_key(self):
         """Get name of datetime index column
 
         Returns:
             column name
@@ -188,71 +159,67 @@
         return (
             self.TM.automl_trend.levels[0][0]
             .features_pipeline._pipeline.transformer_list[0]
             .transformer_list[0]
             .keys[0]
         )
 
-    def __init__(self, task, seq_params=None, trend_params=None):
+    def __init__(self, task, time_series_trend_params=None, reader_params=None, **kwargs):
         self.task = task
         self.task_trend = Task("reg", greater_is_better=False, metric="mae", loss="mae")
-        if seq_params is None:
-            self.seq_params = {
-                "seq0": {
-                    "case": "next_values",
-                    "params": {"n_target": 7, "history": 7, "step": 1, "from_last": True, "test_last": True},
-                },
-            }
-        else:
-            self.seq_params = seq_params
-        self.test_last = self.seq_params["seq0"]["params"]["test_last"]
+        self.kwargs = kwargs
+
+        if "config_path" not in kwargs:
+            self.kwargs["config_path"] = (
+                "/".join(os.path.dirname(__file__).split("/")[:-2]) + "/automl/presets/time_series_config.yml"
+            )
+
+        with open(self.kwargs["config_path"]) as f:
+            params = yaml.safe_load(f)
+
+        # TrendModel and reader_params initialization
+        for name, param in zip(
+            ["time_series_trend_params", "reader_params"], [time_series_trend_params, reader_params]
+        ):
+            if param is None:
+                param = {}
+            self.__dict__[name] = upd_params(params[name], param)
 
-        self.trend_params = deepcopy(self.default_trend_params)
-        if trend_params is not None:
-            self.trend_params.update(trend_params)
-        self.TM = TrendModel(params=self.trend_params)
+        self.TM = TrendModel(params=self.time_series_trend_params)
 
     def fit_predict(self, train_data, roles, verbose=0):
         self.roles = roles
         train_trend = self.TM.fit_predict(train_data, roles)
 
         if hasattr(self.TM, "automl_trend"):
             self.datetime_step = (
-                pd.to_datetime(train_data[self.datetime_key])[1] - pd.to_datetime(train_data[self.datetime_key])[0]
+                pd.to_datetime(train_data[self.datetime_key]).iloc[1]
+                - pd.to_datetime(train_data[self.datetime_key]).iloc[0]
             )
         # fit main
         train_detrend = train_data.copy()
         train_detrend.loc[:, roles["target"]] = train_detrend.loc[:, roles["target"]] - train_trend
 
-        reader_seq = DictToPandasSeqReader(task=self.task, cv=2, seq_params=self.seq_params)
-        feats_seq = LGBSeqSimpleFeatures(fill_na=True, scaler=True)
-        model = RandomForestSklearn(default_params={"verbose": 0})
-        # model2 = LinearLBFGS(default_params={'cs': [1]})
-        model2 = LinearLBFGS()
-
-        model3 = BoostCB()
-        pipeline_lvl1 = MLPipeline([model], pre_selection=None, features_pipeline=feats_seq, post_selection=None)
-        pipeline2_lvl1 = MLPipeline([model2], pre_selection=None, features_pipeline=feats_seq, post_selection=None)
-        pipeline3_lvl1 = MLPipeline([model3], pre_selection=None, features_pipeline=feats_seq, post_selection=None)
-        self.automl_seq = AutoML(
-            reader_seq, [[pipeline_lvl1, pipeline2_lvl1, pipeline3_lvl1]], skip_conn=False, blender=WeightedBlender()
+        # Tabular preset
+        self.automl_seq = TabularAutoML(
+            task=self.task, is_time_series=True, reader_params=self.reader_params, **self.kwargs
         )
 
         oof_pred_seq = self.automl_seq.fit_predict({"seq": {"seq0": train_detrend}}, roles=roles, verbose=verbose)
         return oof_pred_seq, train_trend
 
     def predict(self, data, return_raw=False):
         test_idx = None
-        if self.trend_params["trend"] is True:
+        if self.time_series_trend_params["trend"] is True:
             last_datetime = pd.to_datetime(data[self.datetime_key]).values[-1]
             vals = [last_datetime + (i + 1) * self.datetime_step for i in range(self.n_target)]
-            if not self.test_last:
+            if not self.reader_params["seq_params"]["seq0"]["params"]["test_last"]:
                 vals = data[self.datetime_key].tolist() + vals
             test_data = pd.DataFrame(vals, columns=[self.datetime_key])
-            if not self.test_last:
+            if not self.reader_params["seq_params"]["seq0"]["params"]["test_last"]:
                 test_idx = self.automl_seq.reader.ti["seq0"].create_target(test_data, plain_data=None)
             trend, test_pred_trend = self.TM.predict(data, test_data)
         else:
             test_pred_trend = np.zeros(self.n_target)
             trend = np.zeros(len(data))
 
         detrend = data.copy()
@@ -260,11 +227,11 @@
         test_pred_detrend = self.automl_seq.predict({"seq": {"seq0": detrend}})
         if return_raw:
             return test_pred_detrend
 
         if test_pred_detrend.data.shape[0] == 1:
             final_pred = test_pred_trend + test_pred_detrend.data.flatten()
         else:
-            if (test_idx is not None) and (not self.test_last):
+            if (test_idx is not None) and (not self.reader_params["seq_params"]["seq0"]["params"]["test_last"]):
                 test_pred_trend = test_pred_trend[test_idx]
             final_pred = test_pred_trend + test_pred_detrend.data
         return final_pred, test_pred_trend
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/addons/interpretation/data_process.py` & `lightautoml-0.3.8b1/lightautoml/addons/interpretation/data_process.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/addons/interpretation/l2x.py` & `lightautoml-0.3.8b1/lightautoml/addons/interpretation/l2x.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/addons/interpretation/l2x_model.py` & `lightautoml-0.3.8b1/lightautoml/addons/interpretation/l2x_model.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/addons/interpretation/lime.py` & `lightautoml-0.3.8b1/lightautoml/addons/interpretation/lime.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/addons/interpretation/utils.py` & `lightautoml-0.3.8b1/lightautoml/addons/interpretation/utils.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/addons/uplift/base.py` & `lightautoml-0.3.8b1/lightautoml/addons/uplift/base.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/addons/uplift/metalearners.py` & `lightautoml-0.3.8b1/lightautoml/addons/uplift/metalearners.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/addons/uplift/metrics.py` & `lightautoml-0.3.8b1/lightautoml/addons/uplift/metrics.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/addons/uplift/utils.py` & `lightautoml-0.3.8b1/lightautoml/addons/uplift/utils.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/addons/utilization/utilization.py` & `lightautoml-0.3.8b1/lightautoml/addons/utilization/utilization.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/automl/base.py` & `lightautoml-0.3.8b1/lightautoml/automl/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,39 +89,44 @@
         self,
         reader: Reader,
         levels: Sequence[Sequence[MLPipeline]],
         timer: Optional[PipelineTimer] = None,
         blender: Optional[Blender] = None,
         skip_conn: bool = False,
         return_all_predictions: bool = False,
+        debug: bool = False,
     ):
-        self._initialize(reader, levels, timer, blender, skip_conn, return_all_predictions)
+        self._initialize(reader, levels, timer, blender, skip_conn, return_all_predictions, debug)
 
     def _initialize(
         self,
         reader: Reader,
         levels: Sequence[Sequence[MLPipeline]],
         timer: Optional[PipelineTimer] = None,
         blender: Optional[Blender] = None,
         skip_conn: bool = False,
         return_all_predictions: bool = False,
+        debug: bool = False,
     ):
         """Same as __init__. Exists for delayed initialization in presets.
 
         Args:
             reader: Instance of Reader class object that
                 creates :class:`~lightautoml.dataset.base.LAMLDataset` from input data.
             levels: List of list of :class:`~lightautoml.pipelines.ml..base.MLPipelines`.
             timer: Timer instance of :class:`~lightautoml.utils.timer.PipelineTimer`.
                 Default - unlimited timer.
             blender: Instance of Blender. Default - :class:`~lightautoml.automl.blend.BestModelSelector`.
             skip_conn: True if we should pass first level
                 input features to next levels.
             return_all_predictions: True if we should return all predictions from last
                 level models.
+            debug: To catch running model exceptions or not.
+                - ``True`` :  show exceptions during model training.
+                - ``False``:  catch and hide exceptions.
 
         """
         assert len(levels) > 0, "At least 1 level should be defined"
 
         self.timer = timer
         if timer is None:
             self.timer = PipelineTimer()
@@ -137,14 +142,15 @@
         for i, lvl in enumerate(self._levels):
 
             for j, pipe in enumerate(lvl):
                 pipe.upd_model_names("Lvl_{0}_Pipe_{1}".format(i, j))
 
         self.skip_conn = skip_conn
         self.return_all_predictions = return_all_predictions
+        self.debug = debug
 
     def fit_predict(
         self,
         train_data: Any,
         roles: dict,
         train_features: Optional[Sequence[str]] = None,
         cv_iter: Optional[Iterable] = None,
@@ -204,15 +210,15 @@
             flg_last_level = leven_number == len(self._levels)
 
             logger.info(
                 f"Layer \x1b[1m{leven_number}\x1b[0m train process start. Time left {self.timer.time_left:.2f} secs"
             )
 
             for k, ml_pipe in enumerate(level):
-
+                ml_pipe.debug = self.debug
                 pipe_pred = ml_pipe.fit_predict(train_valid)
                 level_predictions.append(pipe_pred)
                 pipes.append(ml_pipe)
 
                 logger.info("Time left {:.2f} secs\n".format(self.timer.time_left))
 
                 if self.timer.time_limit_exceeded():
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/automl/blend.py` & `lightautoml-0.3.8b1/lightautoml/automl/blend.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/automl/presets/base.py` & `lightautoml-0.3.8b1/lightautoml/automl/presets/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,25 +86,27 @@
     def __init__(
         self,
         task: Task,
         timeout: int = 3600,
         memory_limit: int = 16,
         cpu_limit: int = 4,
         gpu_ids: Optional[str] = "all",
+        debug: bool = False,
         timing_params: Optional[dict] = None,
         config_path: Optional[str] = None,
         **kwargs: Any,
     ):
         self._set_config(config_path)
 
         for name, param in zip(["timing_params"], [timing_params]):
             if param is None:
                 param = {}
             self.__dict__[name] = {**self.__dict__[name], **param}
 
+        self.debug = debug
         self.timer = PipelineTimer(timeout, **getattr(self, "timing_params"))
         self.memory_limit = memory_limit
         if cpu_limit == -1:
             cpu_limit = os.cpu_count()
         self.cpu_limit = cpu_limit
         self.gpu_ids = gpu_ids
         if gpu_ids == "all":
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/automl/presets/image_config.yml` & `lightautoml-0.3.8b1/lightautoml/automl/presets/tabular_configs/conf_1_sel_type_1.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,29 @@
 general_params:
   # possible values are list of lists, that describes levels
   # possible values are ['lgb', 'lgb_tuned', 'linear_l2', 'cb', 'cb_tuned']. List will be extended later
   # or 'auto' - configuration will be infered from data
   # ex.[['lgb', 'lgb_tuned', 'linear_l2', 'cb', 'cb_tuned'], ['lgb', 'linear_l2']] is 3 algos on 1 level, 2 algos on 2 level and blender on 3 level
   # to define more than 1 level nested_cv_params.cv should be > 1
   use_algos: 'auto'
-  # nested_cv - True/False. If true, check nested_cv params. Use folds-in-folds cross-validation scheme
-  # May performs better but take much more time to run (train and inference)
+  # nested_cv - True/False. If true, check nested_cv params
   nested_cv: False
   # skip connections
   skip_conn: True
+  return_all_predictions: False
+  weighted_blender_max_nonzero_coef: 0.05
 
 reader_params:
-  # sample of data to perform analisys
   samples: 100000
-  # minimum nan_rate in feature to keep feature
   max_nan_rate: 0.999
-  # maximum frequency of top frequent value to keep feature
   max_constant_rate: 0.999
-  # create validation folds. Folds will be created even if valid samples or custom validation will be passed
-  # it will be used for feature generation
-  cv: 3
-  # random state for folds creation
+  cv: 5
   random_state: 42
-  # default roles params.
-  # Ex if {'numeric': {'force_input': True}} will be passed, all numeric features will pass all selectors,
-  # if another will not be passed in roles argument of .fit_predict
   roles_params:
-  # n_jobs for advanced roles guess and reading csv files (more RAM needed due to multiprocessing)
   n_jobs: 8
-  # If to turn on advanced roles guess. Slower, but shows better quality
-  # If role of feature is not defined, reader will guess role in 2 ways:
-  #   - simple (numbers as numbers, object as categories or dates if dateformat inferred)
-  #   - advanced, based on some statistic calculation
-  # Advanced also searches to best processing type for defined roles, and in most cases is better, but slower
   advanced_roles: True
   # advanced roles parsing params
   # defaults are ok in general case, don't touch it if you don't know it's meanings
   numeric_unique_rate: 0.999
   max_to_3rd_rate: 1.1
   binning_enc_rate: 2
   raw_decr_rate: 1.1
@@ -61,51 +47,44 @@
   inner_tune: False
   # should we refit tuner each inner cv loop or just take first
   refit_tuner: True
 
 selection_params:
   # selection mode 0/1/2
   # 0 for no selection, 1 - cutoff selection, 2 - iterative selection
-  # harder features selection means increasing train time, but much smaller and faster for inference model
-  mode: 0
+  # harder features selection means increasing train time
+  mode: 1
   # importance type permutation/gain
   importance_type: 'gain'
   # pretrain selector on holdout set. True - fast/ False - accurate
   fit_on_holdout: True
-  # cutoff value for permutation or gain (mode 1/2)
   cutoff: 0
-  # group features add size for iterative algo (mode 2)
   feature_group_size: 1
-  # max features count (mode2)
   max_features_cnt_in_result:
   # list of algos to apply selector. Possible values - 'gbm', 'linear_l2'. gbm stands for both catboost and lgb
   select_algos: [ 'gbm' ]
 
 tuning_params:
   # pretrain tuner on holdout set. True - fast/ False - accurate
-  # Ex. if you have 5-fold cv, validate tuner only on 1 fold
   fit_on_holdout: True
   # max tuning iter for lightgbm. Auto - depends on dataset
-  # smaller dataset gets more iters (int or 'auto')
-  max_tuning_iter: 101
-  # max tuning time. Tuning time might be set lower during train by automl's timer, but cannot be higher
+  # smaller dataset gets more iters
+  max_tuning_iter: 101 # 'auto'
+  # max tuning time. Tuning time might be set lower depending on timer, but cannot be higher
   max_tuning_time: 300
 
-# params for BoostLGBM MLAlgo. Note - params are default and may be changed during train if not freeze_defaults
+# params for BoostLGBM MLAlgo
 lgb_params:
-  # Look for lightgbm train params here. (num_threads will be rewrited by global preset's cpu limit)
   default_params:
     num_threads: 100
   freeze_defaults: False
 
-# params for BoostCB MLAlgo. Note - params are default and may be changed during train if not freeze_defaults
+# params for BoostCB MLAlgo
 cb_params:
-  # Look for lightgbm train params here. (thread_count will be rewrited by global preset's cpu limit)
   default_params:
-    # task type - auto based on gpu available
     task_type: 'CPU'
     thread_count: 100
   freeze_defaults: False
 
 # params for RandomForest MLAlgo. Note - params are default and may be changed during train if not freeze_defaults
 rf_params:
   # Look for RF train params here. (thread_count will be rewrited by global preset's cpu limit)
@@ -114,67 +93,175 @@
 
 # params for LinearLBFGS MLAlgo
 # no tuner needed for this algo - regularization params are found during fit
 linear_l2_params:
   default_params: { }
   freeze_defaults: False
 
+# params for NN model
+nn_params:
+  # Look for NN train params here.
+  # str in ['nn', 'mlp', 'dense', 'denselight', 'resnet', 'snn'] or custom torch model
+  model: denselight
+  # use model with custom embeddings
+  model_with_emb: false
+  # tune custom network
+  tuned: false
+  # fewf
+  optimization_search_space: null
+  # str in torch.nn loss functions or nn.Module or func with (y_pred, y_true) args
+  loss: null
+  loss_params: {}
+  # calculate loss on logits or on predictions of model for classification tasks
+  loss_on_logits: true
+  # clip gradient before loss backprop
+  clip_grad: false
+  clip_grad_params: {}
+  drop_rate: 0.1
+  # add fc layer before model with certain dim
+  num_init_features: null
+  # activation function (str in torch.nn activation functions or custom nn.Module)
+  act_fun: ReLU
+  # add noise after dropout layer for more regularization
+  use_noise: false
+  # noise parameter
+  noise_std: 0.05
+  # use BatchNorm
+  use_bn: true
+  # define hidden layer dimensions for models in ['mlp', 'denselight', 'snn']
+  hidden_size: [512, 512, 512]
+  # dim of intermediate fc is increased times this factor in ResnetModel layer
+  hid_factor: [2, 2]
+  # list of number of layers within each DenseModel block
+  block_config: [2, 2]
+  # portion of neuron to drop after DenseBlock
+  compression: 0.5
+  # output dim of every DenseLayer
+  growth_size: 256
+  # dim of intermediate fc is increased times this factor in DenseModel layer
+  bn_factor: 2
+  # early stopping and scheduler use metric
+  stop_by_metric: false
+  random_state: 42
+  # path to save model state
+  # if None: stay in memory (CPU)
+  path_to_save: null
+  # optimizer
+  opt: Adam
+  # params of optimizer
+  opt_params: { 'lr': 0.0003, 'weight_decay': 0 }
+  # scheduler
+  sch: ReduceLROnPlateau
+  # params of ReduceLROnPlateau scheduler
+  scheduler_params: { 'patience': 5, 'factor': 0.5, 'min_lr': 0.00001 }
+  # using snapshot ensembles
+  # https://arxiv.org/abs/1704.00109
+  is_snap: false
+  # params of snapshots:
+  # k - number of best snapshots (in terms of loss)
+  # early_stopping - use early stopping
+  # patience - early_stopping patience
+  # swa - stochastic weight average - averaging of snapshots weights and replace base model
+  # https://pytorch.org/blog/stochastic-weight-averaging-in-pytorch/ for idea details (different implementation)
+  # use swa with disabled is_snap
+  snap_params: { 'k': 3, 'early_stopping': True, 'patience': 10, 'swa': True }
+  # init last linear layer:
+  # zeros for weights, mean value for bias in regression, inverse sigmoid mean for binary, argmax for multiclass
+  init_bias: true
+  # verbose and create snapshots inside one training epoch every k steps
+  verbose_inside: null
+  # verbose every k epochs
+  verbose: 1
+  # show progress bar for each epoch during batchwise training
+  verbose_bar: false
+  n_epochs: 50
+  input_bn: False
+  emb_dropout: 0.1
+  emb_ratio: 3
+  max_emb_size: 256
+  use_cont: true
+  use_cat: true
+  use_text: false
+  #set cudnn backend
+  deterministic: true
+  # use DP for model training
+  # currently, must be set to FALSE value
+  multigpu: false
+  # device
+  device: cuda:0
+  # use defualt dataset config or custom torch dataset
+  dataset: UniversalDataset
+  pin_memory: false
+  # training and inference batch size
+  bs: 512
+  num_workers: 0
+
+  tuning_params:
+    # pretrain tuner on holdout set. True - fast/ False - accurate
+    # Ex. if you have 5-fold cv, validate tuner only on 1 fold
+    fit_on_holdout: True
+    # max tuning iter for lightgbm. Auto - depends on dataset
+    # smaller dataset gets more iters (int or 'auto')
+    max_tuning_iter: 25
+    # max tuning time. Tuning time might be set lower during train by automl's timer, but cannot be higher
+    max_tuning_time: 3600
+  freeze_defaults: False
+
 gbm_pipeline_params:
-  # max number of categories to generate intersections
   top_intersections: 4
-  # max depth of cat intersection
   max_intersection_depth: 3
-  # subsample to calc data statistics
   subsample: 100000
   auto_unique_co: 10
-  # n_classes to use target encoding for multiclass task
   multiclass_te_co: 3
-  # text_features in gbm feature pipeline. embed or simple
-  cv_features: "simple"
+  output_categories: False
 
 linear_pipeline_params:
-  # max number of categories to generate intersections
   top_intersections: 4
+  max_intersection_depth: 3
+  subsample: 100000
+  auto_unique_co: 50
+  multiclass_te_co: 3
+
+nn_pipeline_params:
+  # use quantile transformer for numerical columns
+  use_qnt: false
+  # number of quantiles to be computed
+  n_quantiles: null
+  # maximum number of samples used to estimate the quantiles for computational efficiency
+  subsample: 1000000000
+  # marginal distribution for the transformed data. The choices are 'uniform' or 'normal'
+  output_distribution: normal
+  # add noise with certain std to dataset before quantile transformation to make data more smooth
+  noise: 0.001
+  # if number of quantiles is none then it equals dataset size / factor
+  qnt_factor: 30
+  # use target encoding for categorical columns
+  use_te: false
+  # max number of categories to generate intersections
+  top_intersections: 5
+  max_bin_count: 10
   # max depth of cat intersection
   max_intersection_depth: 3
   # subsample to calc data statistics
-  subsample: 100000
+  te_subsample: null
+  # should we output sparse if ohe encoding was used during cat handling
+  sparse_ohe: auto
+  # switch to target encoding if high cardinality
   auto_unique_co: 50
-  # n_classes to use target encoding for multiclass task
+  # output encoded categories or embed idxs
+  output_categories: true
+  # cutoff if use target encoding in cat handling on multiclass task if number of classes is high
   multiclass_te_co: 3
-  # text_features in linear feature pipeline. embed or simple
-  cv_features: "embed"
 
 timing_params:
   # select timing mode:
   # 0: no limits - use time limits to create algo's settings but if automl run out of time - let it finish
   # 1: soft - approximate time limits - tasks will finished after timeout
   # 2: hard - hard time limits - stop all tasks before timeout to be exactly in time
   # Any time limitation mode will start working after at least single fold of single model will be computed
   mode: 1
   overhead: 0.1
-  # we assume than each algo takes same amount of time to calc (adjusted with some timing score).
-  # So each algo gets TIME/N_ALGOS.
+  # we assume than each algo takes same amount of time to calc. So each algo gets TIME/N_ALGOS.
   # tuning_rate of that time can be given to the params tuner
   # 0 - means no tuning
   # 'auto' - means infer depends on dataset size
   tuning_rate: 0.7
-
-cv_simple_features:
-  # size of image histogram for each channel
-  hist_size: 30
-  is_hsv: True
-  n_jobs: 4
-
-autocv_features:
-  # model name from effnet family
-  embed_model: 'efficientnet-b0'
-  weights_path: null
-  # directory for save / load cache
-  cache_dir: './cache_CV'
-  subs: 10000
-  device: 'cuda:0'
-  n_jobs: 4
-  random_state: 42
-  is_advprop: True
-  batch_size: 128
-  verbose: True
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/automl/presets/image_presets.py` & `lightautoml-0.3.8b1/lightautoml/automl/presets/image_presets.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         self,
         keys: Sequence[str],
         n_level: int = 1,
         pre_selector: Optional[SelectionPipeline] = None,
     ):
         """Get gbm pipeline."""
         cv_gbm_feats = self.get_cv_pipe(self.gbm_pipeline_params["cv_features"])
-        gbm_feats = LGBAdvancedPipeline(output_categories=False, **self.gbm_pipeline_params)
+        gbm_feats = LGBAdvancedPipeline(feats_imp=pre_selector, output_categories=False, **self.gbm_pipeline_params)
         if cv_gbm_feats is not None:
             gbm_feats.append(cv_gbm_feats)
 
         ml_algos = []
         force_calc = []
         for key, force in zip(keys, [True, False, False, False]):
             tuned = "_tuned" in key
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/automl/presets/tabular_config.yml` & `lightautoml-0.3.8b1/lightautoml/automl/presets/tabular_configs/conf_2_select_mode_1_no_typ.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,30 @@
 general_params:
   # possible values are list of lists, that describes levels
   # possible values are ['lgb', 'lgb_tuned', 'linear_l2', 'cb', 'cb_tuned']. List will be extended later
   # or 'auto' - configuration will be infered from data
   # ex.[['lgb', 'lgb_tuned', 'linear_l2', 'cb', 'cb_tuned'], ['lgb', 'linear_l2']] is 3 algos on 1 level, 2 algos on 2 level and blender on 3 level
   # to define more than 1 level nested_cv_params.cv should be > 1
   use_algos: 'auto'
-  # nested_cv - True/False. If true, check nested_cv params. Use folds-in-folds cross-validation scheme
-  # May performs better but take much more time to run (train and inference)
+  # nested_cv - True/False. If true, check nested_cv params
   nested_cv: False
   # skip connections
   skip_conn: True
-  # Return prediction from all last layer algos?
   return_all_predictions: False
-  # The smallest weight in weighted blender (if lower - the algo will be dropped from final model)
   weighted_blender_max_nonzero_coef: 0.05
 
 reader_params:
-  # sample of data to perform analysis
   samples: 100000
-  # minimum nan_rate in feature to keep feature
   max_nan_rate: 0.999
-  # maximum frequency of top frequent value to keep feature
   max_constant_rate: 0.999
-  # create validation folds. Folds will be created even if valid samples or custom validation will be passed
-  # it will be used for feature generation
   cv: 5
-  # random state for folds creation
   random_state: 42
-  # default roles params.
-  # Ex if {'numeric': {'force_input': True}} will be passed, all numeric features will pass all selectors,
-  # if another will not be passed in roles argument of .fit_predict
   roles_params:
-  # n_jobs for advanced roles guess and reading csv files (more RAM needed due to multiprocessing)
   n_jobs: 8
-  # If to turn on advanced roles guess. Slower, but shows better quality
-  # If role of feature is not defined, reader will guess role in 2 ways:
-  #   - simple (numbers as numbers, object as categories or dates if dateformat inferred)
-  #   - advanced, based on some statistic calculation
-  # Advanced also searches to best processing type for defined roles, and in most cases is better, but slower
-  advanced_roles: True
+  advanced_roles: False
   # advanced roles parsing params
   # defaults are ok in general case, don't touch it if you don't know it's meanings
   numeric_unique_rate: 0.999
   max_to_3rd_rate: 1.1
   binning_enc_rate: 2
   raw_decr_rate: 1.1
   max_score_rate: 0.2
@@ -65,52 +47,44 @@
   inner_tune: False
   # should we refit tuner each inner cv loop or just take first
   refit_tuner: True
 
 selection_params:
   # selection mode 0/1/2
   # 0 for no selection, 1 - cutoff selection, 2 - iterative selection
-  # harder features selection means increasing train time, but much smaller and faster for inference model
-  # 1 is good in most cases
+  # harder features selection means increasing train time
   mode: 1
   # importance type permutation/gain
   importance_type: 'gain'
   # pretrain selector on holdout set. True - fast/ False - accurate
   fit_on_holdout: True
-  # cutoff value for permutation or gain (mode 1/2)
   cutoff: 0
-  # group features add size for iterative algo (mode 2)
   feature_group_size: 1
-  # max features count (mode2)
   max_features_cnt_in_result:
-  # list of algos to apply selector. Possible values - 'gbm', 'rf', 'linear_l2'. gbm stands for both catboost and lgb
+  # list of algos to apply selector. Possible values - 'gbm', 'linear_l2'. gbm stands for both catboost and lgb
   select_algos: [ 'gbm' ]
 
 tuning_params:
   # pretrain tuner on holdout set. True - fast/ False - accurate
-  # Ex. if you have 5-fold cv, validate tuner only on 1 fold
   fit_on_holdout: True
   # max tuning iter for lightgbm. Auto - depends on dataset
-  # smaller dataset gets more iters (int or 'auto')
-  max_tuning_iter: 101
-  # max tuning time. Tuning time might be set lower during train by automl's timer, but cannot be higher
+  # smaller dataset gets more iters
+  max_tuning_iter: 101 # 'auto'
+  # max tuning time. Tuning time might be set lower depending on timer, but cannot be higher
   max_tuning_time: 300
 
-# params for BoostLGBM MLAlgo. Note - params are default and may be changed during train if not freeze_defaults
+# params for BoostLGBM MLAlgo
 lgb_params:
-  # Look for lightgbm train params here. (num_threads will be rewrited by global preset's cpu limit)
   default_params:
     num_threads: 100
   freeze_defaults: False
 
-# params for BoostCB MLAlgo. Note - params are default and may be changed during train if not freeze_defaults
+# params for BoostCB MLAlgo
 cb_params:
-  # Look for lightgbm train params here. (thread_count will be rewrited by global preset's cpu limit)
   default_params:
-    # task type - auto based on gpu available
     task_type: 'CPU'
     thread_count: 100
   freeze_defaults: False
 
 # params for RandomForest MLAlgo. Note - params are default and may be changed during train if not freeze_defaults
 rf_params:
   # Look for RF train params here. (thread_count will be rewrited by global preset's cpu limit)
@@ -119,45 +93,175 @@
 
 # params for LinearLBFGS MLAlgo
 # no tuner needed for this algo - regularization params are found during fit
 linear_l2_params:
   default_params: { }
   freeze_defaults: False
 
+# params for NN model
+nn_params:
+  # Look for NN train params here.
+  # str in ['nn', 'mlp', 'dense', 'denselight', 'resnet', 'snn'] or custom torch model
+  model: denselight
+  # use model with custom embeddings
+  model_with_emb: false
+  # tune custom network
+  tuned: false
+  # fewf
+  optimization_search_space: null
+  # str in torch.nn loss functions or nn.Module or func with (y_pred, y_true) args
+  loss: null
+  loss_params: {}
+  # calculate loss on logits or on predictions of model for classification tasks
+  loss_on_logits: true
+  # clip gradient before loss backprop
+  clip_grad: false
+  clip_grad_params: {}
+  drop_rate: 0.1
+  # add fc layer before model with certain dim
+  num_init_features: null
+  # activation function (str in torch.nn activation functions or custom nn.Module)
+  act_fun: ReLU
+  # add noise after dropout layer for more regularization
+  use_noise: false
+  # noise parameter
+  noise_std: 0.05
+  # use BatchNorm
+  use_bn: true
+  # define hidden layer dimensions for models in ['mlp', 'denselight', 'snn']
+  hidden_size: [512, 512, 512]
+  # dim of intermediate fc is increased times this factor in ResnetModel layer
+  hid_factor: [2, 2]
+  # list of number of layers within each DenseModel block
+  block_config: [2, 2]
+  # portion of neuron to drop after DenseBlock
+  compression: 0.5
+  # output dim of every DenseLayer
+  growth_size: 256
+  # dim of intermediate fc is increased times this factor in DenseModel layer
+  bn_factor: 2
+  # early stopping and scheduler use metric
+  stop_by_metric: false
+  random_state: 42
+  # path to save model state
+  # if None: stay in memory (CPU)
+  path_to_save: null
+  # optimizer
+  opt: Adam
+  # params of optimizer
+  opt_params: { 'lr': 0.0003, 'weight_decay': 0 }
+  # scheduler
+  sch: ReduceLROnPlateau
+  # params of ReduceLROnPlateau scheduler
+  scheduler_params: { 'patience': 5, 'factor': 0.5, 'min_lr': 0.00001 }
+  # using snapshot ensembles
+  # https://arxiv.org/abs/1704.00109
+  is_snap: false
+  # params of snapshots:
+  # k - number of best snapshots (in terms of loss)
+  # early_stopping - use early stopping
+  # patience - early_stopping patience
+  # swa - stochastic weight average - averaging of snapshots weights and replace base model
+  # https://pytorch.org/blog/stochastic-weight-averaging-in-pytorch/ for idea details (different implementation)
+  # use swa with disabled is_snap
+  snap_params: { 'k': 3, 'early_stopping': True, 'patience': 10, 'swa': True }
+  # init last linear layer:
+  # zeros for weights, mean value for bias in regression, inverse sigmoid mean for binary, argmax for multiclass
+  init_bias: true
+  # verbose and create snapshots inside one training epoch every k steps
+  verbose_inside: null
+  # verbose every k epochs
+  verbose: 1
+  # show progress bar for each epoch during batchwise training
+  verbose_bar: false
+  n_epochs: 50
+  input_bn: False
+  emb_dropout: 0.1
+  emb_ratio: 3
+  max_emb_size: 256
+  use_cont: true
+  use_cat: true
+  use_text: false
+  #set cudnn backend
+  deterministic: true
+  # use DP for model training
+  # currently, must be set to FALSE value
+  multigpu: false
+  # device
+  device: cuda:0
+  # use defualt dataset config or custom torch dataset
+  dataset: UniversalDataset
+  pin_memory: false
+  # training and inference batch size
+  bs: 512
+  num_workers: 0
+
+  tuning_params:
+    # pretrain tuner on holdout set. True - fast/ False - accurate
+    # Ex. if you have 5-fold cv, validate tuner only on 1 fold
+    fit_on_holdout: True
+    # max tuning iter for lightgbm. Auto - depends on dataset
+    # smaller dataset gets more iters (int or 'auto')
+    max_tuning_iter: 25
+    # max tuning time. Tuning time might be set lower during train by automl's timer, but cannot be higher
+    max_tuning_time: 3600
+  freeze_defaults: False
+
 gbm_pipeline_params:
-  # max number of categories to generate intersections
   top_intersections: 4
-  # max depth of cat intersection
   max_intersection_depth: 3
-  # subsample to calc data statistics
   subsample: 100000
   auto_unique_co: 10
-  # n_classes to use target encoding for multiclass task
   multiclass_te_co: 3
-  # DEV feature: output categorical features as categories (if True, can totally overfit your model - be careful!)
   output_categories: False
 
 linear_pipeline_params:
-  # max number of categories to generate intersections
   top_intersections: 4
+  max_intersection_depth: 3
+  subsample: 100000
+  auto_unique_co: 50
+  multiclass_te_co: 3
+
+nn_pipeline_params:
+  # use quantile transformer for numerical columns
+  use_qnt: false
+  # number of quantiles to be computed
+  n_quantiles: null
+  # maximum number of samples used to estimate the quantiles for computational efficiency
+  subsample: 1000000000
+  # marginal distribution for the transformed data. The choices are 'uniform' or 'normal'
+  output_distribution: normal
+  # add noise with certain std to dataset before quantile transformation to make data more smooth
+  noise: 0.001
+  # if number of quantiles is none then it equals dataset size / factor
+  qnt_factor: 30
+  # use target encoding for categorical columns
+  use_te: false
+  # max number of categories to generate intersections
+  top_intersections: 5
+  max_bin_count: 10
   # max depth of cat intersection
   max_intersection_depth: 3
   # subsample to calc data statistics
-  subsample: 100000
+  te_subsample: null
+  # should we output sparse if ohe encoding was used during cat handling
+  sparse_ohe: auto
+  # switch to target encoding if high cardinality
   auto_unique_co: 50
-  # n_classes to use target encoding for multiclass task
+  # output encoded categories or embed idxs
+  output_categories: true
+  # cutoff if use target encoding in cat handling on multiclass task if number of classes is high
   multiclass_te_co: 3
 
 timing_params:
   # select timing mode:
   # 0: no limits - use time limits to create algo's settings but if automl run out of time - let it finish
   # 1: soft - approximate time limits - tasks will finished after timeout
   # 2: hard - hard time limits - stop all tasks before timeout to be exactly in time
   # Any time limitation mode will start working after at least single fold of single model will be computed
   mode: 1
   overhead: 0.1
-  # we assume than each algo takes same amount of time to calc (adjusted with some timing score).
-  # So each algo gets TIME/N_ALGOS.
+  # we assume than each algo takes same amount of time to calc. So each algo gets TIME/N_ALGOS.
   # tuning_rate of that time can be given to the params tuner
   # 0 - means no tuning
   # 'auto' - means infer depends on dataset size
   tuning_rate: 0.7
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/automl/presets/tabular_presets.py` & `lightautoml-0.3.8b1/lightautoml/automl/presets/tabular_presets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# TODO: проверить что NLP не падает, CV
 """Tabular presets."""
 
 import logging
 import os
 
 from collections import Counter
 from copy import copy
@@ -10,41 +11,47 @@
 from typing import Optional
 from typing import Sequence
 from typing import cast
 
 import numpy as np
 import pandas as pd
 import torch
+import torch.nn as nn
 
 from joblib import Parallel
 from joblib import delayed
 from pandas import DataFrame
 from tqdm import tqdm
 
 from ...addons.utilization import TimeUtilization
 from ...dataset.np_pd_dataset import NumpyDataset
 from ...ml_algo.boost_cb import BoostCB
 from ...ml_algo.boost_lgbm import BoostLGBM
+from ...ml_algo.dl_model import TorchModel
 from ...ml_algo.linear_sklearn import LinearLBFGS
 from ...ml_algo.random_forest import RandomForestSklearn
+from ...ml_algo.tuning.optuna import DLOptunaTuner
 from ...ml_algo.tuning.optuna import OptunaTuner
 from ...pipelines.features.lgb_pipeline import LGBAdvancedPipeline
+from ...pipelines.features.lgb_pipeline import LGBSeqSimpleFeatures
 from ...pipelines.features.lgb_pipeline import LGBSimpleFeatures
 from ...pipelines.features.linear_pipeline import LinearFeatures
+from ...pipelines.features.torch_pipeline import TorchSimpleFeatures
 from ...pipelines.ml.nested_ml_pipe import NestedTabularMLPipeline
 from ...pipelines.selection.base import ComposedSelector
 from ...pipelines.selection.base import SelectionPipeline
 from ...pipelines.selection.importance_based import ImportanceCutoffSelector
 from ...pipelines.selection.importance_based import ModelBasedImportanceEstimator
 from ...pipelines.selection.permutation_importance_based import (
     NpIterativeFeatureSelector,
 )
 from ...pipelines.selection.permutation_importance_based import (
     NpPermutationImportanceEstimator,
 )
+from ...reader.base import DictToPandasSeqReader
 from ...reader.base import PandasToPandasReader
 from ...reader.tabular_batch_generator import ReadableToDf
 from ...reader.tabular_batch_generator import read_batch
 from ...reader.tabular_batch_generator import read_data
 from ...tasks import Task
 from ..blend import MeanBlender
 from ..blend import WeightedBlender
@@ -81,98 +88,134 @@
 
     Args:
         task: Task to solve.
         timeout: Timeout in seconds.
         memory_limit: Memory limit that are passed to each automl.
         cpu_limit: CPU limit that that are passed to each automl.
         gpu_ids: GPU IDs that are passed to each automl.
+        debug: To catch running model exceptions or not.
         timing_params: Timing param dict. Optional.
         config_path: Path to config file.
         general_params: General param dict.
         reader_params: Reader param dict.
         read_csv_params: Params to pass ``pandas.read_csv``
             (case of train/predict from file).
         nested_cv_params: Param dict for nested cross-validation.
         tuning_params: Params of Optuna tuner.
         selection_params: Params of feature selection.
         lgb_params: Params of lightgbm model.
         cb_params: Params of catboost model.
         rf_params: Params of Sklearn Random Forest model.
         linear_l2_params: Params of linear model.
+        nn_params: Params of neural network model.
         gbm_pipeline_params: Params of feature generation
             for boosting models.
         linear_pipeline_params: Params of feature generation
             for linear models.
-
+        nn_pipeline_params: Params of feature generation
+            for neural network models.
     """
 
     _default_config_path = "tabular_config.yml"
 
     # set initial runtime rate guess for first level models
-    _time_scores = {"lgb": 1, "lgb_tuned": 3, "linear_l2": 0.7, "cb": 2, "cb_tuned": 6, "rf": 5, "rf_tuned": 10}
+    _time_scores = {
+        "lgb": 1,
+        "lgb_tuned": 3,
+        "linear_l2": 0.7,
+        "cb": 2,
+        "cb_tuned": 6,
+        "rf": 5,
+        "rf_tuned": 10,
+        "nn": 10,
+        "nn_tuned": 20,
+    }
 
     def __init__(
         self,
         task: Task,
         timeout: int = 3600,
         memory_limit: int = 16,
         cpu_limit: int = 4,
         gpu_ids: Optional[str] = "all",
+        debug: bool = False,
         timing_params: Optional[dict] = None,
         config_path: Optional[str] = None,
         general_params: Optional[dict] = None,
         reader_params: Optional[dict] = None,
         read_csv_params: Optional[dict] = None,
         nested_cv_params: Optional[dict] = None,
         tuning_params: Optional[dict] = None,
         selection_params: Optional[dict] = None,
         lgb_params: Optional[dict] = None,
         cb_params: Optional[dict] = None,
         rf_params: Optional[dict] = None,
         linear_l2_params: Optional[dict] = None,
+        nn_params: Optional[dict] = None,
         gbm_pipeline_params: Optional[dict] = None,
         linear_pipeline_params: Optional[dict] = None,
+        nn_pipeline_params: Optional[dict] = None,
+        time_series_pipeline_params: Optional[dict] = None,
+        is_time_series: bool = False,
     ):
-        super().__init__(task, timeout, memory_limit, cpu_limit, gpu_ids, timing_params, config_path)
+        super().__init__(task, timeout, memory_limit, cpu_limit, gpu_ids, debug, timing_params, config_path)
+        #
+        self.is_time_series = is_time_series
 
         # upd manual params
         for name, param in zip(
             [
                 "general_params",
                 "reader_params",
                 "read_csv_params",
                 "nested_cv_params",
                 "tuning_params",
-                "selection_params",
                 "lgb_params",
                 "cb_params",
                 "rf_params",
                 "linear_l2_params",
+                "nn_params",
                 "gbm_pipeline_params",
                 "linear_pipeline_params",
+                "nn_pipeline_params",
             ],
             [
                 general_params,
                 reader_params,
                 read_csv_params,
                 nested_cv_params,
                 tuning_params,
-                selection_params,
                 lgb_params,
                 cb_params,
                 rf_params,
                 linear_l2_params,
+                nn_params,
                 gbm_pipeline_params,
                 linear_pipeline_params,
+                nn_pipeline_params,
             ],
         ):
             if param is None:
                 param = {}
             self.__dict__[name] = upd_params(self.__dict__[name], param)
 
+        # if not time-series mode --> update selection_params too
+        if not self.is_time_series:
+            for name, param in zip(["selection_params"], [selection_params]):
+                if param is None:
+                    param = {}
+                self.__dict__[name] = upd_params(self.__dict__[name], param)
+
+        # if time-series mode --> update time_series_pipeline_params
+        if self.is_time_series:
+            for name, param in zip(["time_series_pipeline_params"], [time_series_pipeline_params]):
+                if param is None:
+                    param = {}
+                self.__dict__[name] = upd_params(self.__dict__[name], param)
+
     def infer_auto_params(self, train_data: DataFrame, multilevel_avail: bool = False):
 
         length = train_data.shape[0]
 
         # infer optuna tuning iteration based on dataframe len
         if self.tuning_params["max_tuning_iter"] == "auto":
             if length < 10000:
@@ -183,45 +226,76 @@
                 self.tuning_params["max_tuning_iter"] = 10
             else:
                 self.tuning_params["max_tuning_iter"] = 5
 
         if self.general_params["use_algos"] == "auto":
             # TODO: More rules and add cases
             self.general_params["use_algos"] = [["lgb", "lgb_tuned", "linear_l2", "cb", "cb_tuned"]]
-            if self.task.name == "multiclass" and multilevel_avail:
-                self.general_params["use_algos"].append(["linear_l2", "lgb"])
+            if self.task.name == "multi:reg" and self.is_time_series:
+                self.general_params["use_algos"] = [["cb", "linear_l2", "rf"]]
+            else:
+                if self.task.name == "multiclass" and multilevel_avail:
+                    self.general_params["use_algos"].append(["linear_l2", "lgb"])
 
-            if (self.task.name == "multi:reg") or (self.task.name == "multilabel"):
-                self.general_params["use_algos"] = [["linear_l2", "cb", "rf", "rf_tuned", "cb_tuned"]]
+                if (self.task.name == "multi:reg") or (self.task.name == "multilabel"):
+                    self.general_params["use_algos"] = [["linear_l2", "cb", "rf", "rf_tuned", "cb_tuned"]]
 
         if not self.general_params["nested_cv"]:
             self.nested_cv_params["cv"] = 1
 
         # check gpu to use catboost
         gpu_cnt = torch.cuda.device_count()
         gpu_ids = self.gpu_ids
         if gpu_cnt > 0 and gpu_ids:
             if gpu_ids == "all":
                 gpu_ids = ",".join(list(map(str, range(gpu_cnt))))
 
+            self.nn_params["device"] = gpu_ids.split(",")
             self.cb_params["default_params"]["task_type"] = "GPU"
             self.cb_params["default_params"]["devices"] = gpu_ids.replace(",", ":")
 
+        else:
+            self.nn_params["device"] = "cpu"
+
         # check all n_jobs params
         cpu_cnt = min(os.cpu_count(), self.cpu_limit)
         torch.set_num_threads(cpu_cnt)
 
         self.cb_params["default_params"]["thread_count"] = min(
             self.cb_params["default_params"]["thread_count"], cpu_cnt
         )
         self.lgb_params["default_params"]["num_threads"] = min(
             self.lgb_params["default_params"]["num_threads"], cpu_cnt
         )
         self.reader_params["n_jobs"] = min(self.reader_params["n_jobs"], cpu_cnt)
 
+    def get_feature_pipeline(self, model, **kwargs):
+        """Get LGBSeqSimpleFeatures pipeline if task is the time series prediction.
+
+        Args:
+            model: one from ["gbm", "linear_l2",, "rf", "nn"].
+            kwargs: Arbitrary keyword arguments.
+
+        Returns:
+            appropriate features pipeline.
+        """
+        if self.is_time_series and model in ["gbm", "linear_l2", "rf", "nn"]:
+            return LGBSeqSimpleFeatures(fill_na=True, scaler=True, transformers_params=self.time_series_pipeline_params)
+        else:
+            if model == "nn":
+                return TorchSimpleFeatures(**self.nn_pipeline_params)
+            if model == "linear_l2":
+                return LinearFeatures(output_categories=True, **self.linear_pipeline_params)
+            if model == "gbm":
+                return LGBAdvancedPipeline(**self.gbm_pipeline_params, **kwargs)
+            if model == "rf":
+                if "fill_na" in kwargs:
+                    return LGBAdvancedPipeline(**self.gbm_pipeline_params, **kwargs)
+                return LGBAdvancedPipeline(**self.gbm_pipeline_params, fill_na=True, **kwargs)
+
     def get_time_score(self, n_level: int, model_type: str, nested: Optional[bool] = None):
 
         if nested is None:
             nested = self.general_params["nested_cv"]
 
         score = self._time_scores[model_type]
 
@@ -315,21 +389,78 @@
                     max_features_cnt_in_result=selection_params["max_features_cnt_in_result"],
                 )
 
                 pre_selector = ComposedSelector([pre_selector, extra_selector])
 
         return pre_selector
 
+    def get_nn(
+        self, keys: Sequence[str], n_level: int = 1, pre_selector: Optional[SelectionPipeline] = None
+    ) -> NestedTabularMLPipeline:
+        ml_algos = []
+        force_calc = []
+
+        nn_feats = self.get_feature_pipeline(model="nn")
+        general_nn_params = deepcopy(self.nn_params)
+        if "0" in self.nn_params:
+            for i in range(len(keys)):
+                if str(i) in general_nn_params:
+                    del general_nn_params[str(i)]
+
+        for i, key in enumerate(keys):
+            time_score = self.get_time_score(n_level, "nn")
+            nn_timer = self.timer.get_task_timer("reg_nn", time_score)
+            model_params = deepcopy(general_nn_params)
+
+            model_params.update(self.nn_params.get(str(i), general_nn_params))
+            model_name = key
+
+            if isinstance(key, str):
+                tuned = "_tuned" in key
+                if key[:2] == "nn":
+                    model_name = "mlp"
+                _name = "TorchNN_" + model_name + "_" + str(i)
+                model_name = model_name.replace("_tuned", "")
+            else:
+                tuned = model_params.get("tuned")
+                _name = "TorchNN_" + str(i)
+
+            model_params["model"] = model_name
+            nn_model = TorchModel(
+                timer=nn_timer,
+                default_params=model_params,
+                freeze_defaults=model_params["freeze_defaults"],
+                optimization_search_space=model_params.get("optimization_search_space", None),
+            )
+            nn_model._name = _name
+
+            if tuned:
+                nn_model.set_prefix("Tuned")
+                nn_tuner = DLOptunaTuner(
+                    n_trials=model_params["tuning_params"]["max_tuning_iter"],
+                    timeout=model_params["tuning_params"]["max_tuning_time"],
+                    fit_on_holdout=model_params["tuning_params"]["fit_on_holdout"],
+                )
+                nn_model = (nn_model, nn_tuner)
+            ml_algos.append(nn_model)
+            force_calc.append(True if not len(ml_algos) - 1 else False)
+
+        nn_pipe = NestedTabularMLPipeline(
+            ml_algos, force_calc, pre_selection=None, features_pipeline=nn_feats, **self.nested_cv_params
+        )
+
+        return nn_pipe
+
     def get_linear(self, n_level: int = 1, pre_selector: Optional[SelectionPipeline] = None) -> NestedTabularMLPipeline:
 
         # linear model with l2
         time_score = self.get_time_score(n_level, "linear_l2")
         linear_l2_timer = self.timer.get_task_timer("reg_l2", time_score)
         linear_l2_model = LinearLBFGS(timer=linear_l2_timer, **self.linear_l2_params)
-        linear_l2_feats = LinearFeatures(output_categories=True, **self.linear_pipeline_params)
+        linear_l2_feats = self.get_feature_pipeline(model="linear_l2")
 
         linear_l2_pipe = NestedTabularMLPipeline(
             [linear_l2_model],
             force_calc=True,
             pre_selection=pre_selector,
             features_pipeline=linear_l2_feats,
             **self.nested_cv_params
@@ -339,15 +470,15 @@
     def get_gbms(
         self,
         keys: Sequence[str],
         n_level: int = 1,
         pre_selector: Optional[SelectionPipeline] = None,
     ):
 
-        gbm_feats = LGBAdvancedPipeline(**self.gbm_pipeline_params)
+        gbm_feats = self.get_feature_pipeline(model="gbm", feats_imp=pre_selector)
 
         ml_algos = []
         force_calc = []
         for key, force in zip(keys, [True, False, False, False]):
             tuned = "_tuned" in key
             algo_key = key.split("_")[0]
             time_score = self.get_time_score(n_level, key)
@@ -374,16 +505,15 @@
             ml_algos, force_calc, pre_selection=pre_selector, features_pipeline=gbm_feats, **self.nested_cv_params
         )
 
         return gbm_pipe
 
     def get_rfs(self, keys: Sequence[str], n_level: int = 1, pre_selector: Optional[SelectionPipeline] = None):
 
-        rf_feats = LGBAdvancedPipeline(**self.gbm_pipeline_params, fill_na=True)
-
+        rf_feats = self.get_feature_pipeline(model="rf", feats_imp=pre_selector, fill_na=True)
         ml_algos = []
         force_calc = []
         for key, force in zip(keys, [True, False]):
             tuned = "_tuned" in key
             algo_key = key.split("_")[0]
             time_score = self.get_time_score(n_level, key)
             rf_timer = self.timer.get_task_timer(algo_key, time_score)
@@ -413,63 +543,89 @@
         Args:
             **fit_args: Contain all information needed for creating automl.
 
         """
         train_data = fit_args["train_data"]
         multilevel_avail = fit_args["valid_data"] is None and fit_args["cv_iter"] is None
 
-        self.infer_auto_params(train_data, multilevel_avail)
-        reader = PandasToPandasReader(task=self.task, **self.reader_params)
-
-        pre_selector = self.get_selector()
+        if self.is_time_series:
+            self.infer_auto_params(train_data["seq"]["seq0"], multilevel_avail)
+            reader = DictToPandasSeqReader(task=self.task, **self.reader_params)
+            pre_selector = None
+        else:
+            self.infer_auto_params(train_data, multilevel_avail)
+            reader = PandasToPandasReader(task=self.task, **self.reader_params)
+            pre_selector = self.get_selector()
 
         levels = []
 
         for n, names in enumerate(self.general_params["use_algos"]):
             lvl = []
             # regs
             rf_models = [x for x in ["rf", "rf_tuned"] if x in names]
 
             if len(rf_models) > 0:
                 selector = None
-                if "rf" in self.selection_params["select_algos"] and (self.general_params["skip_conn"] or n == 0):
+                if (
+                    self.is_time_series
+                    or "rf" in self.selection_params["select_algos"]
+                    and (self.general_params["skip_conn"] or n == 0)
+                ):
                     selector = pre_selector
                 lvl.append(self.get_rfs(rf_models, n + 1, selector))
 
             if "linear_l2" in names:
                 selector = None
-                if "linear_l2" in self.selection_params["select_algos"] and (
-                    self.general_params["skip_conn"] or n == 0
+                if (
+                    self.is_time_series
+                    or "linear_l2" in self.selection_params["select_algos"]
+                    and (self.general_params["skip_conn"] or n == 0)
                 ):
                     selector = pre_selector
                 lvl.append(self.get_linear(n + 1, selector))
 
             gbm_models = [
                 x for x in ["lgb", "lgb_tuned", "cb", "cb_tuned"] if x in names and x.split("_")[0] in self.task.losses
             ]
 
             if len(gbm_models) > 0:
                 selector = None
-                if "gbm" in self.selection_params["select_algos"] and (self.general_params["skip_conn"] or n == 0):
+                if (
+                    self.is_time_series
+                    or "gbm" in self.selection_params["select_algos"]
+                    and (self.general_params["skip_conn"] or n == 0)
+                ):
                     selector = pre_selector
                 lvl.append(self.get_gbms(gbm_models, n + 1, selector))
 
-            levels.append(lvl)
+            available_nn_models = ["nn", "mlp", "dense", "denselight", "resnet", "snn", "linear_layer", "_linear_layer"]
+            available_nn_models = available_nn_models + [x + "_tuned" for x in available_nn_models]
+            nn_models = [
+                x for x in names if x in available_nn_models or (isinstance(x, type) and issubclass(x, nn.Module))
+            ]
+
+            if len(nn_models) > 0:
+                selector = None
+                lvl.append(self.get_nn(nn_models, n + 1, selector))
+
+            if len(lvl) != 0:
+                levels.append(lvl)
 
         # blend everything
         blender = WeightedBlender(max_nonzero_coef=self.general_params["weighted_blender_max_nonzero_coef"])
 
         # initialize
         self._initialize(
             reader,
             levels,
             skip_conn=self.general_params["skip_conn"],
             blender=blender,
             return_all_predictions=self.general_params["return_all_predictions"],
             timer=self.timer,
+            debug=self.debug,
         )
 
     def _get_read_csv_params(self):
         try:
             cols_to_read = self.reader.used_features
             numeric_dtypes = {
                 x: self.reader.roles[x].dtype for x in self.reader.roles if self.reader.roles[x].name == "Numeric"
@@ -532,24 +688,28 @@
 
         Returns:
             Dataset with predictions. Call ``.data`` to get predictions array.
 
         """
         # roles may be none in case of train data is set {'data': np.ndarray, 'target': np.ndarray ...}
         self.set_logfile(log_file)
-
         if roles is None:
             roles = {}
         read_csv_params = self._get_read_csv_params()
+        if self.is_time_series:
+            train_data = train_data["seq"]["seq0"]
         train, upd_roles = read_data(train_data, train_features, self.cpu_limit, read_csv_params)
         if upd_roles:
             roles = {**roles, **upd_roles}
         if valid_data is not None:
             data, _ = read_data(valid_data, valid_features, self.cpu_limit, self.read_csv_params)
 
+        if self.is_time_series:
+            train = {"seq": {"seq0": train}}
+
         oof_pred = super().fit_predict(train, roles=roles, cv_iter=cv_iter, valid_data=valid_data, verbose=verbose)
 
         return cast(NumpyDataset, oof_pred)
 
     def predict(
         self,
         data: ReadableToDf,
@@ -589,15 +749,19 @@
         Returns:
             Dataset with predictions.
 
         """
         read_csv_params = self._get_read_csv_params()
 
         if batch_size is None and n_jobs == 1:
+            if self.is_time_series:
+                data = data["seq"]["seq0"]
             data, _ = read_data(data, features_names, self.cpu_limit, read_csv_params)
+            if self.is_time_series:
+                data = {"seq": {"seq0": data}}
             pred = super().predict(data, features_names, return_all_predictions)
             return cast(NumpyDataset, pred)
 
         data_generator = read_batch(
             data,
             features_names,
             n_jobs=n_jobs,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/automl/presets/text_config.yml` & `lightautoml-0.3.8b1/lightautoml/automl/presets/text_config.yml`

 * *Files 7% similar despite different names*

```diff
@@ -156,14 +156,15 @@
   n_epochs: 20
   input_bn: False
   emb_dropout: 0.1
   emb_ratio: 3
   max_emb_size: 50
   # null to use default bert for this language
   bert_name: null
+  model: _linear_layer
   # pooling: cls, mean, max, sum
   pooling: 'cls'
   use_cont: True
   use_cat: True
   use_text: True
   lang: null
   #set cudnn backend
@@ -182,27 +183,53 @@
   # max depth of cat intersection
   max_intersection_depth: 3
   # subsample to calc data statistics
   subsample: 100000
   auto_unique_co: 10
   # n_classes to use target encoding for multiclass task
   multiclass_te_co: 3
+  # use groupby features
+  use_groupby: False
+  # groupby types used in feature engeneering
+  groupby_types: [ 'delta_median', 'delta_mean', 'min', 'max', 'std', 'mode', 'is_mode' ]
+  # top features are choosen by cardinality or feature importance
+  groupby_top_based_on: 'cardinality'
+  # top categorical features to use in groupby transformer
+  groupby_top_categorical: 3
+  # top numerical features to use in groupby transformer
+  groupby_top_numerical: 3
+  # list of groupby triplets ("group_col", "feat", "groupby_type") for manual setting
+  # disables groupby_types, groupby_top_based_on and other groupby parameters if defined
+  groupby_triplets: [ ]
   # text_features in gbm feature pipeline. embed or tfidf
   text_features: "embed"
 
 linear_pipeline_params:
   # max number of categories to generate intersections
   top_intersections: 4
   # max depth of cat intersection
   max_intersection_depth: 3
   # subsample to calc data statistics
   subsample: 100000
   auto_unique_co: 50
   # n_classes to use target encoding for multiclass task
   multiclass_te_co: 3
+  # use groupby features
+  use_groupby: False
+  # groupby types used in feature engeneering
+  groupby_types: [ 'delta_median', 'delta_mean', 'min', 'max', 'std', 'mode', 'is_mode' ]
+  # top features are choosen by cardinality or feature importance
+  groupby_top_based_on: 'cardinality'
+  # top categorical features to use in groupby transformer
+  groupby_top_categorical: 3
+  # top numerical features to use in groupby transformer
+  groupby_top_numerical: 3
+  # list of groupby triplets ("group_col", "feat", "groupby_type") for manual setting
+  # disables groupby_types, groupby_top_based_on and other groupby parameters if defined
+  groupby_triplets: [ ]
   # text_features in linear feature pipeline. embed or tfidf
   text_features: "tfidf"
 
 timing_params:
   # select timing mode:
   # 0: no limits - use time limits to create algo's settings but if automl run out of time - let it finish
   # 1: soft - approximate time limits - tasks will finished after timeout
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/automl/presets/text_presets.py` & `lightautoml-0.3.8b1/lightautoml/automl/presets/text_presets.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 
 __validate_extra_deps("nlp", error=True)
 
 
 import logging
 import os
 
+from copy import deepcopy
 from typing import Optional
 from typing import Sequence
 
 import torch
+import torch.nn as nn
 
 from pandas import DataFrame
 
 from ...ml_algo.boost_cb import BoostCB
 from ...ml_algo.boost_lgbm import BoostLGBM
 from ...ml_algo.dl_model import TorchModel
 from ...ml_algo.linear_sklearn import LinearLBFGS
+from ...ml_algo.tuning.optuna import DLOptunaTuner
 from ...ml_algo.tuning.optuna import OptunaTuner
 from ...pipelines.features.base import FeaturesPipeline
 from ...pipelines.features.lgb_pipeline import LGBAdvancedPipeline
 from ...pipelines.features.linear_pipeline import LinearFeatures
 from ...pipelines.features.text_pipeline import NLPTFiDFFeatures
 from ...pipelines.features.text_pipeline import TextAutoFeatures
 from ...pipelines.features.text_pipeline import TextBertFeatures
@@ -39,15 +42,25 @@
 
 
 logger = logging.getLogger(__name__)
 
 
 _base_dir = os.path.dirname(__file__)
 # set initial runtime rate guess for first level models
-_time_scores = {"lgb": 1, "lgb_tuned": 3, "linear_l2": 0.7, "cb": 2, "cb_tuned": 6, "nn": 1, "rf": 5, "rf_tuned": 10}
+_time_scores = {
+    "lgb": 1,
+    "lgb_tuned": 3,
+    "linear_l2": 0.7,
+    "cb": 2,
+    "cb_tuned": 6,
+    "nn": 10,
+    "nn_tuned": 20,
+    "rf": 5,
+    "rf_tuned": 10,
+}
 
 
 # TODO: add text feature selection
 class TabularNLPAutoML(TabularAutoML):
     """Classic preset - work with tabular and text data.
 
     Supported data roles - numbers, dates, categories, text
@@ -68,14 +81,15 @@
 
     Args:
         task: Task to solve.
         timeout: Timeout in seconds.
         memory_limit: Memory limit that are passed to each automl.
         cpu_limit: CPU limit that that are passed to each automl.
         gpu_ids: GPU IDs that are passed to each automl.
+        debug: To catch running model exceptions or not.
         timing_params: Timing param dict.
         config_path: Path to config file.
         general_params: General param dict.
         reader_params: Reader param dict.
         read_csv_params: Params to pass :func:`pandas.read_csv`
             (case of train/predict from file).
         nested_cv_params: Param dict for nested cross-validation.
@@ -113,14 +127,15 @@
     def __init__(
         self,
         task: Task,
         timeout: int = 3600,
         memory_limit: int = 16,
         cpu_limit: int = 4,
         gpu_ids: Optional[str] = "all",
+        debug: bool = False,
         timing_params: Optional[dict] = None,
         config_path: Optional[str] = None,
         general_params: Optional[dict] = None,
         reader_params: Optional[dict] = None,
         read_csv_params: Optional[dict] = None,
         nested_cv_params: Optional[dict] = None,
         tuning_params: Optional[dict] = None,
@@ -139,14 +154,15 @@
     ):
         super().__init__(
             task,
             timeout,
             memory_limit,
             cpu_limit,
             gpu_ids,
+            debug,
             timing_params,
             config_path,
         )
 
         # upd manual params
         for name, param in zip(
             [
@@ -242,29 +258,72 @@
         elif type == "embed":
             return TextAutoFeatures(**self.text_params, **self.autonlp_params)
         elif type == "bert":
             return TextBertFeatures(**self.text_params)
         else:
             return None
 
-    def get_nn(self, n_level: int = 1, pre_selector: Optional[SelectionPipeline] = None) -> NestedTabularMLPipeline:
-
-        # nn model
-        time_score = self.get_time_score(n_level, "nn")
-        nn_timer = self.timer.get_task_timer("reg_nn", time_score)
-        nn_model = TorchModel(timer=nn_timer, default_params=self.nn_params)
+    def get_nn(
+        self, keys: Sequence[str], n_level: int = 1, pre_selector: Optional[SelectionPipeline] = None
+    ) -> NestedTabularMLPipeline:
+        ml_algos = []
+        force_calc = []
 
         text_nn_feats = self.get_nlp_pipe(self.nn_pipeline_params["text_features"])
         nn_feats = LinearFeatures(output_categories=True, **self.linear_pipeline_params)
         if text_nn_feats is not None:
             nn_feats.append(text_nn_feats)
 
+        general_nn_params = deepcopy(self.nn_params)
+        if "0" in self.nn_params:
+            for i in range(len(keys)):
+                if str(i) in general_nn_params:
+                    del general_nn_params[str(i)]
+
+        for i, key in enumerate(keys):
+            time_score = self.get_time_score(n_level, "nn")
+            nn_timer = self.timer.get_task_timer("reg_nn", time_score)
+            model_params = deepcopy(general_nn_params)
+
+            model_params.update(self.nn_params.get(str(i), general_nn_params))
+            model_name = key
+
+            if isinstance(key, str):
+                tuned = "_tuned" in key
+                if key[:2] == "nn":
+                    model_name = "_linear_layer"
+                _name = "TorchNN_" + model_name + "_" + str(i)
+                model_name = model_name.replace("_tuned", "")
+            else:
+                tuned = model_params.get("tuned")
+                _name = "TorchNN_" + str(i)
+
+            model_params["model"] = model_name
+            nn_model = TorchModel(
+                timer=nn_timer,
+                default_params=model_params,
+                optimization_search_space=model_params.get("optimization_search_space", None),
+            )
+            nn_model._name = _name
+
+            if tuned:
+                nn_model.set_prefix("Tuned")
+                nn_tuner = DLOptunaTuner(
+                    n_trials=model_params["tuning_params"]["max_tuning_iter"],
+                    timeout=model_params["tuning_params"]["max_tuning_time"],
+                    fit_on_holdout=model_params["tuning_params"]["fit_on_holdout"],
+                )
+                nn_model = (nn_model, nn_tuner)
+            ml_algos.append(nn_model)
+            force_calc.append(True if not len(ml_algos) - 1 else False)
+
         nn_pipe = NestedTabularMLPipeline(
-            [nn_model], pre_selection=None, features_pipeline=nn_feats, **self.nested_cv_params
+            ml_algos, force_calc, pre_selection=None, features_pipeline=nn_feats, **self.nested_cv_params
         )
+
         return nn_pipe
 
     def get_linear(self, n_level: int = 1, pre_selector: Optional[SelectionPipeline] = None) -> NestedTabularMLPipeline:
 
         # linear model with l2
         time_score = self.get_time_score(n_level, "linear_l2")
         linear_l2_timer = self.timer.get_task_timer("reg_l2", time_score)
@@ -288,15 +347,15 @@
         self,
         keys: Sequence[str],
         n_level: int = 1,
         pre_selector: Optional[SelectionPipeline] = None,
     ):
 
         text_gbm_feats = self.get_nlp_pipe(self.gbm_pipeline_params["text_features"])
-        gbm_feats = LGBAdvancedPipeline(output_categories=False, **self.gbm_pipeline_params)
+        gbm_feats = LGBAdvancedPipeline(feats_imp=pre_selector, output_categories=False, **self.gbm_pipeline_params)
         if text_gbm_feats is not None:
             gbm_feats.append(text_gbm_feats)
 
         ml_algos = []
         force_calc = []
         for key, force in zip(keys, [True, False, False, False]):
             tuned = "_tuned" in key
@@ -358,30 +417,37 @@
 
             if len(gbm_models) > 0:
                 selector = None
                 if "gbm" in self.selection_params["select_algos"] and (self.general_params["skip_conn"] or n == 0):
                     selector = pre_selector
                 lvl.append(self.get_gbms(gbm_models, n + 1, selector))
 
-            if "nn" in names:
+            available_nn_models = ["nn", "mlp", "dense", "denselight", "resnet", "snn", "linear_layer", "_linear_layer"]
+            available_nn_models = available_nn_models + [x + "_tuned" for x in available_nn_models]
+            nn_models = [
+                x for x in names if x in available_nn_models or (isinstance(x, type) and issubclass(x, nn.Module))
+            ]
+
+            if len(nn_models) > 0:
                 selector = None
-                lvl.append(self.get_nn(n + 1, selector))
+                lvl.append(self.get_nn(nn_models, n + 1, selector))
 
             levels.append(lvl)
 
         # blend everything
         blender = WeightedBlender()
 
         # initialize
         self._initialize(
             reader,
             levels,
             skip_conn=self.general_params["skip_conn"],
             blender=blender,
             timer=self.timer,
+            debug=self.debug,
         )
 
     def predict(
         self,
         data: ReadableToDf,
         features_names: Optional[Sequence[str]] = None,
         batch_size: Optional[int] = None,
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/automl/presets/utils.py` & `lightautoml-0.3.8b1/lightautoml/automl/presets/utils.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/automl/presets/whitebox_config.yml` & `lightautoml-0.3.8b1/lightautoml/automl/presets/whitebox_config.yml`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/automl/presets/whitebox_presets.py` & `lightautoml-0.3.8b1/lightautoml/automl/presets/whitebox_presets.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/dataset/base.py` & `lightautoml-0.3.8b1/lightautoml/dataset/base.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/dataset/np_pd_dataset.py` & `lightautoml-0.3.8b1/lightautoml/dataset/np_pd_dataset.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/dataset/roles.py` & `lightautoml-0.3.8b1/lightautoml/dataset/roles.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/dataset/seq_np_pd_dataset.py` & `lightautoml-0.3.8b1/lightautoml/dataset/seq_np_pd_dataset.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/dataset/utils.py` & `lightautoml-0.3.8b1/lightautoml/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/image/image.py` & `lightautoml-0.3.8b1/lightautoml/image/image.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/ml_algo/base.py` & `lightautoml-0.3.8b1/lightautoml/ml_algo/base.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/ml_algo/boost_cb.py` & `lightautoml-0.3.8b1/lightautoml/ml_algo/boost_cb.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/ml_algo/boost_lgbm.py` & `lightautoml-0.3.8b1/lightautoml/ml_algo/boost_lgbm.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/ml_algo/dl_model.py` & `lightautoml-0.3.8b1/lightautoml/ml_algo/dl_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,44 +5,81 @@
 
 __validate_extra_deps("nlp")
 
 
 import gc
 import logging
 import os
+import sys
 import uuid
 
 from copy import copy
+from typing import Dict
 
 import numpy as np
+import optuna
+import pandas as pd
 import torch
+import torch.nn as nn
 
-from torch.optim import lr_scheduler
-from transformers import AutoTokenizer
+from torch.optim.lr_scheduler import ReduceLROnPlateau
+
+from ..dataset.np_pd_dataset import NumpyDataset
+from ..tasks.losses.torch import TorchLossWrapper
+from ..utils.installation import __validate_extra_deps
+from ..validation.base import TrainValidIterator
+
+
+__validate_extra_deps("nlp")
+
+try:
+    from transformers import AutoTokenizer
+
+    from ..pipelines.features.text_pipeline import _model_name_by_lang
+except:
+    import warnings
+
+    warnings.warn("'transformers' - package isn't installed")
 
 from ..ml_algo.base import TabularDataset
 from ..ml_algo.base import TabularMLAlgo
-from ..pipelines.features.text_pipeline import _model_name_by_lang
 from ..pipelines.utils import get_columns_by_role
 from ..text.nn_model import CatEmbedder
 from ..text.nn_model import ContEmbedder
 from ..text.nn_model import TextBert
 from ..text.nn_model import TorchUniversalModel
 from ..text.nn_model import UniversalDataset
 from ..text.trainer import Trainer
 from ..text.utils import collate_dict
 from ..text.utils import inv_sigmoid
 from ..text.utils import inv_softmax
 from ..text.utils import is_shuffle
 from ..text.utils import parse_devices
 from ..text.utils import seed_everything
+from .torch_based.nn_models import MLP
+from .torch_based.nn_models import SNN
+from .torch_based.nn_models import DenseLightModel
+from .torch_based.nn_models import DenseModel
+from .torch_based.nn_models import LinearLayer
+from .torch_based.nn_models import ResNetModel
+from .torch_based.nn_models import _LinearLayer
 
 
 logger = logging.getLogger(__name__)
 
+model_by_name = {
+    "denselight": DenseLightModel,
+    "dense": DenseModel,
+    "resnet": ResNetModel,
+    "mlp": MLP,
+    "linear_layer": LinearLayer,
+    "_linear_layer": _LinearLayer,
+    "snn": SNN,
+}
+
 
 class TorchModel(TabularMLAlgo):
     """Neural net for tabular datasets.
 
     default_params:
 
         - bs: Batch size.
@@ -54,23 +91,34 @@
         - snap_params: Dict with SE parameters.
         - init_bias: Init last linear bias by mean target values.
         - n_epochs: Number of training epochs.
         - input_bn: Use 1d batch norm for input data.
         - emb_dropout: Dropout probability.
         - emb_ratio: Ratio for embedding size = (x + 1) // emb_ratio.
         - max_emb_size: Max embedding size.
-        - bert_name: Name of HuggingFace transformer model.
-        - pooling: Type of pooling strategy for bert model.
         - device: Torch device or str.
         - use_cont: Use numeric data.
         - use_cat: Use category data.
         - use_text: Use text data.
         - lang: Text language.
+        - bert_name: Name of HuggingFace transformer model.
+        - pooling: Type of pooling strategy for bert model.
         - deterministic: CUDNN backend.
         - multigpu: Use Data Parallel.
+        - model_with_emb: Use model with custom embeddings.
+        - loss: Torch loss or str or func with (y_pred, y_true) args.
+        - loss_params: Dict with loss params.
+        - loss_on_logits: Calculate loss on logits or on predictions of model for classification tasks.
+        - clip_grad: Clip gradient before loss backprop.
+        - clip_grad_params: Dict with clip_grad params.
+        - dataset: Class for data retrieval
+        - tuned: Tune custom model
+        - num_init_features: Scale input dimension to another one
+        - use_noise: Use Noise
+        - use_bn: Use BatchNorm
         - path_to_save: Path to save model checkpoints,
           ``None`` - stay in memory.
         - random_state: Random state to take subsample.
         - verbose_inside: Number of steps between
           verbose inside epoch or ``None``.
         - verbose: Verbose every N epochs.
 
@@ -80,72 +128,129 @@
         - ``False``:  params may be changed only manually or with tuning.
 
     timer: :class:`~lightautoml.utils.timer.Timer` instance or ``None``.
 
     """
 
     _name: str = "TorchNN"
+    _params: Dict = None
+
+    _default_models_params = {
+        "n_out": None,
+        "hid_factor": [2, 2],
+        "hidden_size": [512, 512, 512],
+        "block_config": [2, 2],
+        "compression": 0.5,
+        "growth_size": 256,
+        "bn_factor": 2,
+        "drop_rate": 0.1,
+        "noise_std": 0.05,
+        "num_init_features": None,
+        "act_fun": nn.ReLU,
+        "use_noise": False,
+        "use_bn": True,
+    }
 
     _default_params = {
-        "bs": 16,
-        "num_workers": 4,
+        "num_workers": 0,
+        "pin_memory": False,
         "max_length": 256,
-        "opt_params": {
-            "lr": 1e-4,
-        },
-        "scheduler_params": {"patience": 5, "factor": 0.5, "verbose": True},
         "is_snap": False,
-        "snap_params": {"k": 1, "early_stopping": True, "patience": 1, "swa": False},
-        "init_bias": True,
-        "n_epochs": 20,
         "input_bn": False,
-        "emb_dropout": 0.1,
-        "emb_ratio": 3,
-        "max_emb_size": 50,
+        "max_emb_size": 256,
         "bert_name": None,
         "pooling": "cls",
-        "device": [0],
+        "device": torch.device("cuda:0"),
         "use_cont": True,
         "use_cat": True,
         "use_text": True,
         "lang": "en",
         "deterministic": True,
         "multigpu": False,
         "random_state": 42,
+        "model": "dense",
+        "model_with_emb": False,
         "path_to_save": os.path.join("./models/", "model"),
         "verbose_inside": None,
         "verbose": 1,
-        "stop_by_metric": False,
+        "n_epochs": 20,
+        "snap_params": {"k": 3, "early_stopping": True, "patience": 16, "swa": True},
+        "bs": 512,
+        "emb_dropout": 0.1,
+        "emb_ratio": 3,
+        "opt": torch.optim.Adam,
+        "opt_params": {"weight_decay": 0, "lr": 3e-4},
+        "sch": ReduceLROnPlateau,
+        "scheduler_params": {"patience": 10, "factor": 1e-2, "min_lr": 1e-5},
+        "loss": None,
+        "loss_params": {},
+        "loss_on_logits": True,
+        "clip_grad": False,
+        "clip_grad_params": {},
+        "init_bias": True,
+        "dataset": UniversalDataset,
+        "tuned": False,
+        "optimization_search_space": None,
+        "verbose_bar": False,
+        "freeze_defaults": False,
+        **_default_models_params,
     }
 
     def _infer_params(self):
         if self.params["path_to_save"] is not None:
             self.path_to_save = os.path.relpath(self.params["path_to_save"])
             if not os.path.exists(self.path_to_save):
                 os.makedirs(self.path_to_save)
         else:
             self.path_to_save = None
 
         params = copy(self.params)
-        if params["bert_name"] is None:
-            params["bert_name"] = _model_name_by_lang[params["lang"]]
+        loss = params["loss"]
+
+        if isinstance(loss, str):
+            loss = getattr(nn, loss)
+        if loss is not None and issubclass(loss, nn.Module):
+            loss = TorchLossWrapper(loss, **params["loss_params"])
+        if loss is None:
+            loss = self.task.losses["torch"].loss
 
-        params["loss"] = self.task.losses["torch"].loss
+        params["loss"] = loss
         params["metric"] = self.task.losses["torch"].metric_func
 
+        if params["bert_name"] is None and params["use_text"]:
+            params["bert_name"] = _model_name_by_lang[params["lang"]]
+
         is_text = (len(params["text_features"]) > 0) and (params["use_text"]) and (params["device"].type == "cuda")
         is_cat = (len(params["cat_features"]) > 0) and (params["use_cat"])
         is_cont = (len(params["cont_features"]) > 0) and (params["use_cont"])
 
+        torch_model = params["model"]
+
+        if isinstance(torch_model, str):
+            assert torch_model in model_by_name, "Wrong model name. Available models: " + str(model_by_name.keys())
+            if torch_model == "snn":
+                params["init_bias"] = False
+            torch_model = model_by_name[torch_model]
+
+        assert issubclass(torch_model, nn.Module), "Wrong model format, only support torch models"
+
+        # str to nn modules
+        for p_name, module in [
+            ["act_fun", nn],
+            ["dataset", sys.modules[__name__]],
+            ["opt", torch.optim],
+            ["sch", torch.optim.lr_scheduler],
+        ]:
+            if isinstance(params[p_name], str):
+                params[p_name] = getattr(module, params[p_name])
+
         model = Trainer(
-            net=TorchUniversalModel,
+            net=TorchUniversalModel if not params["model_with_emb"] else params["model"],
             net_params={
-                "loss": params["loss"],
                 "task": self.task,
-                "n_out": params["n_out"],
                 "cont_embedder": ContEmbedder if is_cont else None,
                 "cont_params": {
                     "num_dims": params["cont_dim"],
                     "input_bn": params["input_bn"],
                 }
                 if is_cont
                 else None,
@@ -161,46 +266,49 @@
                 "text_embedder": TextBert if is_text else None,
                 "text_params": {
                     "model_name": params["bert_name"],
                     "pooling": params["pooling"],
                 }
                 if is_text
                 else None,
-                "bias": params["bias"],
+                "torch_model": torch_model,
+                **params,
             },
-            opt=torch.optim.Adam,
-            opt_params=params["opt_params"],
-            n_epochs=params["n_epochs"],
-            device=params["device"],
-            device_ids=params["device_ids"],
-            is_snap=params["is_snap"],
-            snap_params=params["snap_params"],
-            sch=lr_scheduler.ReduceLROnPlateau,
-            scheduler_params=params["scheduler_params"],
-            verbose=params["verbose"],
-            verbose_inside=params["verbose_inside"],
-            metric=params["metric"],
-            stop_by_metric=params["stop_by_metric"],
-            apex=False,
+            **{"apex": False, **params},
         )
 
         self.train_params = {
-            "dataset": UniversalDataset,
+            "dataset": params["dataset"],
             "bs": params["bs"],
             "num_workers": params["num_workers"],
+            "pin_memory": params["pin_memory"],
             "tokenizer": AutoTokenizer.from_pretrained(params["bert_name"], use_fast=False) if is_text else None,
             "max_length": params["max_length"],
         }
 
         return model
 
     @staticmethod
-    def get_mean_target(target, task_name):  # noqa: D102
+    def get_mean_target(target, task_name: str):
+        """Get target mean / inverse sigmoid transformation \
+            to init bias in last layer of network.
+
+        Args:
+            target: Target values.
+            task_name: One of the available task names
+
+        Returns:
+            Array with bias values.
+
+        """
+        if isinstance(target, pd.Series) or isinstance(target, pd.DataFrame):
+            target = target.values
+        target = target.reshape(target.shape[0], -1)
         bias = (
-            np.array(target.mean(axis=0)).reshape(1, -1).astype(float)
+            np.nanmean(target, axis=0).astype(float)
             if (task_name != "multiclass")
             else np.unique(target, return_counts=True)[1]
         )
         bias = (
             inv_sigmoid(bias)
             if (task_name == "binary") or (task_name == "multilabel")
             else inv_softmax(bias)
@@ -210,53 +318,106 @@
 
         bias[bias == np.inf] = np.nanmax(bias[bias != np.inf])
         bias[bias == -np.inf] = np.nanmin(bias[bias != -np.inf])
         bias[bias == np.NaN] = np.nanmean(bias[bias != np.NaN])
 
         return bias
 
-    def init_params_on_input(self, train_valid_iterator) -> dict:
-        """Get model parameters depending on dataset parameters.
+    def _init_params_on_input(self, train_valid_iterator) -> dict:
+        """Init params that common for all folds.
 
         Args:
             train_valid_iterator: Classic cv-iterator.
 
         Returns:
-            Parameters of model.
+            Dict with data parameters.
 
         """
-        suggested_params = copy(self.default_params)
-        suggested_params["device"], suggested_params["device_ids"] = parse_devices(
-            suggested_params["device"], suggested_params["multigpu"]
-        )
+        params = self.params
+        new_params = {}
+        new_params["device"], new_params["device_ids"] = parse_devices(params["device"], params["multigpu"])
 
         task_name = train_valid_iterator.train.task.name
         target = train_valid_iterator.train.target
-        suggested_params["n_out"] = 1 if task_name != "multiclass" else np.max(target) + 1
+
+        if params["n_out"] is None:
+            new_params["n_out"] = 1 if task_name != "multiclass" else np.max(target) + 1
+            new_params["n_out"] = target.shape[1] if task_name in ["multi:reg", "multilabel"] else new_params["n_out"]
 
         cat_dims = []
-        suggested_params["cat_features"] = get_columns_by_role(train_valid_iterator.train, "Category")
-        for cat_feature in suggested_params["cat_features"]:
-            num_unique_categories = max(train_valid_iterator.train[:, cat_feature].data) + 1
+        new_params["cat_features"] = get_columns_by_role(train_valid_iterator.train, "Category")
+
+        # Cat_features are needed to be preprocessed with LE, where 0 = not known category
+        valid = train_valid_iterator.get_validation_data()
+        for cat_feature in new_params["cat_features"]:
+            num_unique_categories = (
+                max(
+                    max(train_valid_iterator.train[:, cat_feature].data),
+                    max(valid[:, cat_feature].data),
+                )
+                + 1
+            )
             cat_dims.append(num_unique_categories)
-        suggested_params["cat_dims"] = cat_dims
+        new_params["cat_dims"] = cat_dims
+
+        new_params["cont_features"] = get_columns_by_role(train_valid_iterator.train, "Numeric")
+        new_params["cont_dim"] = len(new_params["cont_features"])
+
+        new_params["text_features"] = get_columns_by_role(train_valid_iterator.train, "Text")
+        new_params["bias"] = self.get_mean_target(target, task_name) if params["init_bias"] else None
 
-        suggested_params["cont_features"] = get_columns_by_role(train_valid_iterator.train, "Numeric")
-        suggested_params["cont_dim"] = len(suggested_params["cont_features"])
+        logger.debug(f'number of text features: {len(new_params["text_features"])} ')
+        logger.debug(f'number of categorical features: {len(new_params["cat_features"])} ')
+        logger.debug(f'number of continuous features: {new_params["cont_dim"]} ')
 
-        suggested_params["text_features"] = get_columns_by_role(train_valid_iterator.train, "Text")
-        suggested_params["bias"] = self.get_mean_target(target, task_name) if suggested_params["init_bias"] else None
+        return new_params
+
+    def init_params_on_input(self, train_valid_iterator) -> dict:
+        """Get model parameters depending on dataset parameters.
 
+        Args:
+            train_valid_iterator: Classic cv-iterator.
+
+        Returns:
+            Parameters of model.
+
+        """
+        suggested_params = copy(self.params)
+        if self.freeze_defaults:
+            # if user change defaults manually - keep it
+            return suggested_params
+
+        rows_num = len(train_valid_iterator.train) + len(train_valid_iterator.get_validation_data())
+        bs = 256
+
+        if rows_num > 50_000:
+            bs = 512
+        if rows_num > 100_000:
+            bs = 1024
+        if rows_num > 1_000_000:
+            bs = 2048
+
+        suggested_params["bs"] = bs
+        suggested_params["snap_params"] = (
+            {"k": 1, "early_stopping": True, "patience": 16, "swa": False}
+            if self.params["model"] == "snn"
+            else self.params["snap_params"]
+        )
         return suggested_params
 
-    def get_dataloaders_from_dicts(self, data_dict):  # noqa: D102
-        logger.debug(f'number of text features: {len(self.params["text_features"])} ')
-        logger.debug(f'number of categorical features: {len(self.params["cat_features"])} ')
-        logger.debug(f'number of continuous features: {self.params["cont_dim"]} ')
+    def get_dataloaders_from_dicts(self, data_dict: Dict):
+        """Construct dataloaders depending on stage.
+
+        Args:
+            data_dict: Dict with (stage_name, data) (key, value).
+
+        Returns:
+            Dataloaders.
 
+        """
         datasets = {}
         for stage, value in data_dict.items():
             data = {
                 name: value.data[cols].values
                 for name, cols in zip(
                     ["text", "cat", "cont"],
                     [
@@ -280,39 +441,63 @@
         dataloaders = {
             stage: torch.utils.data.DataLoader(
                 datasets[stage],
                 batch_size=self.train_params["bs"],
                 shuffle=is_shuffle(stage),
                 num_workers=self.train_params["num_workers"],
                 collate_fn=collate_dict,
-                pin_memory=False,
+                pin_memory=self.train_params["pin_memory"],
             )
             for stage, value in data_dict.items()
         }
         return dataloaders
 
+    def fit_predict(self, train_valid_iterator: TrainValidIterator) -> NumpyDataset:
+        """Fit and then predict accordig the strategy that uses train_valid_iterator.
+
+        If item uses more then one time it will
+        predict mean value of predictions.
+        If the element is not used in training then
+        the prediction will be ``numpy.nan`` for this item
+
+        Args:
+            train_valid_iterator: Classic cv-iterator.
+
+        Returns:
+            Dataset with predicted values.
+
+        """
+        if self._params is None:
+            self.params = self.init_params_on_input(train_valid_iterator)
+        self.params = self._init_params_on_input(train_valid_iterator)
+        return super().fit_predict(train_valid_iterator)
+
     def fit_predict_single_fold(self, train, valid):
         """Implements training and prediction on single fold.
 
         Args:
             train: Train Dataset.
             valid: Validation Dataset.
 
         Returns:
             Tuple (model, predicted_values).
 
         """
         seed_everything(self.params["random_state"], self.params["deterministic"])
+        task_name = train.task.name
+        target = train.target
+        self.params["bias"] = self.get_mean_target(target, task_name) if self.params["init_bias"] else None
+
         model = self._infer_params()
 
         model_path = (
             os.path.join(self.path_to_save, f"{uuid.uuid4()}.pickle") if self.path_to_save is not None else None
         )
         # init datasets
-        dataloaders = self.get_dataloaders_from_dicts({"train": train, "val": valid})
+        dataloaders = self.get_dataloaders_from_dicts({"train": train.to_pandas(), "val": valid.to_pandas()})
 
         val_pred = model.fit(dataloaders)
 
         if model_path is None:
             model_path = model.state_dict(model_path)
         else:
             model.state_dict(model_path)
@@ -331,20 +516,50 @@
             dataset: Test dataset.
 
         Returns:
             Predicted target values.
 
         """
         seed_everything(self.params["random_state"], self.params["deterministic"])
-        dataloaders = self.get_dataloaders_from_dicts({"test": dataset})
+        dataloaders = self.get_dataloaders_from_dicts({"test": dataset.to_pandas()})
 
         if isinstance(model, (str, dict)):
             model = self._infer_params().load_state(model)
 
         pred = model.predict(dataloaders["test"], "test")
 
         model.clean()
         del dataloaders, model
         gc.collect()
         torch.cuda.empty_cache()
 
         return pred
+
+    def _default_sample(self, trial: optuna.trial.Trial, estimated_n_trials: int, suggested_params: Dict) -> Dict:
+        """Implements simple tuning sampling strategy.
+
+        Args:
+            trial: Current optuna Trial.
+            estimated_n_trials: Estimated trials based on time spent on previous ones.
+            suggested_params: Suggested params
+
+        Returns:
+            Dict with Sampled params.
+
+        """
+        # optionally
+        trial_values = copy(suggested_params)
+
+        trial_values["bs"] = trial.suggest_categorical("bs", [2 ** i for i in range(6, 11)])
+
+        weight_decay_bin = trial.suggest_categorical("weight_decay_bin", [0, 1])
+        if weight_decay_bin == 0:
+            weight_decay = 0
+        else:
+            weight_decay = trial.suggest_loguniform("weight_decay", low=1e-6, high=1e-2)
+
+        lr = trial.suggest_loguniform("lr", low=1e-5, high=1e-1)
+        trial_values["opt_params"] = {
+            "lr": lr,
+            "weight_decay": weight_decay,
+        }
+        return trial_values
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/ml_algo/linear_sklearn.py` & `lightautoml-0.3.8b1/lightautoml/ml_algo/linear_sklearn.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/ml_algo/random_forest.py` & `lightautoml-0.3.8b1/lightautoml/ml_algo/random_forest.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import numpy as np
 
 from pandas import Series
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.ensemble import RandomForestRegressor
 
 from ..pipelines.selection.base import ImportanceEstimator
+from ..utils.logging import get_stdout_level
 from ..validation.base import TrainValidIterator
 from .base import TabularDataset
 from .base import TabularMLAlgo
 from .tuning.base import Uniform
 
 
 logger = logging.getLogger(__name__)
@@ -63,20 +64,21 @@
         Returns:
             Tuple (params, verbose).
         """
         params = copy(self.params)
 
         # Logging
         if "verbose" not in params:
-            root_logger = logging.getLogger()
-            level = root_logger.getEffectiveLevel()
-            if level in (logging.CRITICAL, logging.ERROR, logging.WARNING):
+            level = get_stdout_level()
+            if level <= logging.INFO:
                 params["verbose"] = 0
-            else:
+            elif level == logging.DEBUG:
                 params["verbose"] = 2
+            else:
+                params["verbose"] = 1
 
         return params
 
     def init_params_on_input(self, train_valid_iterator: TrainValidIterator) -> dict:
         """Get model parameters depending on dataset parameters.
 
         Args:
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/ml_algo/torch_based/linear_model.py` & `lightautoml-0.3.8b1/lightautoml/ml_algo/torch_based/linear_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,15 @@
             nn.init.zeros_(self.linear.weight)
 
         # add categories if it is defined
         self.cat_params = None
         if len(embed_sizes) > 0:
             self.cat_params = nn.Parameter(torch.zeros(sum(embed_sizes), output_size))
             self.embed_idx = torch.LongTensor(embed_sizes).cumsum(dim=0) - torch.LongTensor(embed_sizes)
+        self.final_act = nn.Identity()
 
     def forward(
         self,
         numbers: Optional[torch.Tensor] = None,
         categories: Optional[torch.Tensor] = None,
     ):
         """Forward-pass.
@@ -92,78 +93,55 @@
             x = x + self.linear(numbers)
 
         if self.cat_params is not None:
             x = x + self.cat_params[categories + self.embed_idx].sum(dim=1)
 
         return x
 
-
-class CatLogisticRegression(CatLinear):
-    """Realisation of torch-based logistic regression."""
-
-    def __init__(self, numeric_size: int, embed_sizes: Sequence[int] = (), output_size: int = 1):
-        super().__init__(numeric_size, embed_sizes=embed_sizes, output_size=output_size)
-        self.sigmoid = nn.Sigmoid()
-
-    def forward(
+    def predict(
         self,
         numbers: Optional[torch.Tensor] = None,
         categories: Optional[torch.Tensor] = None,
     ):
-        """Forward-pass. Sigmoid func at the end of linear layer.
+        """Inference phase.
 
         Args:
-            numbers: Input numeric features.
-            categories: Input categorical features.
+            numbers: Numeric data.
+            categories: Categorical data.
 
         Returns:
-            Probabilitics.
+            Predicted logits/targets for cls/other tasks.
 
         """
-        x = super().forward(numbers, categories)
-        x = torch.clamp(x, -50, 50)
-        x = self.sigmoid(x)
-
+        x = self.forward(numbers, categories)
+        x = self.final_act(x)
         return x
 
 
+class CatLogisticRegression(CatLinear):
+    """Realisation of torch-based logistic regression."""
+
+    def __init__(self, numeric_size: int, embed_sizes: Sequence[int] = (), output_size: int = 1):
+        super().__init__(numeric_size, embed_sizes=embed_sizes, output_size=output_size)
+        self.final_act = nn.Sigmoid()
+
+
 class CatRegression(CatLinear):
     """Realisation of torch-based linear regreession."""
 
     def __init__(self, numeric_size: int, embed_sizes: Sequence[int] = (), output_size: int = 1):
         super().__init__(numeric_size, embed_sizes=embed_sizes, output_size=output_size)
 
 
 class CatMulticlass(CatLinear):
     """Realisation of multi-class linear classifier."""
 
     def __init__(self, numeric_size: int, embed_sizes: Sequence[int] = (), output_size: int = 1):
         super().__init__(numeric_size, embed_sizes=embed_sizes, output_size=output_size)
-        self.softmax = nn.Softmax(dim=1)
-
-    def forward(
-        self,
-        numbers: Optional[torch.Tensor] = None,
-        categories: Optional[torch.Tensor] = None,
-    ):
-        """Forward-pass.
-
-        Args:
-            numbers: Input numeric features.
-            categories: Input categorical features.
-
-        Returns:
-            Linear prediction.
-
-        """
-        x = super().forward(numbers, categories)
-        x = torch.clamp(x, -50, 50)
-        x = self.softmax(x)
-
-        return x
+        self.final_act = nn.Softmax(dim=1)
 
 
 class TorchBasedLinearEstimator:
     """Linear model based on torch L-BFGS solver.
 
     Accepts Numeric + Label Encoded categories or Numeric sparse input.
 
@@ -428,15 +406,15 @@
 
         Returns:
             Predicted target values.
 
         """
         with torch.set_grad_enabled(False):
             self.model.eval()
-            preds = self.model(data, data_cat).numpy()
+            preds = self.model.predict(data, data_cat).numpy()
 
         return preds
 
     def predict(self, data: np.ndarray) -> np.ndarray:
         """Inference phase.
 
         Args:
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/ml_algo/tuning/base.py` & `lightautoml-0.3.8b1/lightautoml/ml_algo/tuning/base.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/ml_algo/tuning/optuna.py` & `lightautoml-0.3.8b1/lightautoml/ml_algo/tuning/optuna.py`

 * *Files 24% similar despite different names*

```diff
@@ -281,7 +281,218 @@
                 raise ValueError(f"Optuna does not support distribution {search_space}")
 
         return trial_values
 
     def plot(self):
         """Plot optimization history of all trials in a study."""
         return optuna.visualization.plot_optimization_history(self.study)
+
+
+class DLOptunaTuner(ParamsTuner):
+    """Wrapper for optuna tuner.
+
+    Args:
+        timeout: Maximum learning time.
+        n_trials: Maximum number of trials.
+        direction: Direction of optimization.
+            Set ``minimize`` for minimization
+            and ``maximize`` for maximization.
+        fit_on_holdout: Will be used holdout cv-iterator.
+        random_state: Seed for optuna sampler.
+
+    """
+
+    _name: str = "OptunaTuner"
+
+    study: optuna.study.Study = None
+    estimated_n_trials: int = None
+    mean_trial_time: Optional[int] = None
+
+    def __init__(
+        # TODO: For now, metric is designed to be greater is better. Change maximize param after metric refactor if needed
+        self,
+        timeout: Optional[int] = 1000,
+        n_trials: Optional[int] = 100,
+        direction: Optional[str] = "maximize",
+        fit_on_holdout: bool = True,
+        random_state: int = 42,
+    ):
+        self.timeout = timeout
+        self.n_trials = n_trials
+        self.estimated_n_trials = n_trials
+        self.direction = direction
+        self._fit_on_holdout = fit_on_holdout
+        self.random_state = random_state
+
+    def _upd_timeout(self, timeout):
+        self.timeout = min(self.timeout, timeout)
+
+    def fit(
+        self,
+        ml_algo: TunableAlgo,
+        train_valid_iterator: Optional[TrainValidIterator] = None,
+    ) -> Tuple[Optional[TunableAlgo], Optional[LAMLDataset]]:
+        """Tune model.
+
+        Args:
+            ml_algo: Algo that is tuned.
+            train_valid_iterator: Classic cv-iterator.
+
+        Returns:
+            Tuple (None, None) if an optuna exception raised
+            or ``fit_on_holdout=True`` and ``train_valid_iterator`` is
+            not :class:`~lightautoml.validation.base.HoldoutIterator`.
+            Tuple (MlALgo, preds_ds) otherwise.
+
+        """
+        assert not ml_algo.is_fitted, "Fitted algo cannot be tuned."
+        self._params_scores = []
+
+        # optuna.logging.set_verbosity(get_stdout_level())
+        # upd timeout according to ml_algo timer
+        estimated_tuning_time = ml_algo.timer.estimate_tuner_time(len(train_valid_iterator))
+        if estimated_tuning_time:
+            # TODO: Check for minimal runtime!
+            estimated_tuning_time = max(estimated_tuning_time, 1)
+            self._upd_timeout(estimated_tuning_time)
+
+        logger.info(
+            f"Start hyperparameters optimization for \x1b[1m{ml_algo._name}\x1b[0m ... Time budget is {self.timeout:.2f} secs"
+        )
+
+        metric_name = train_valid_iterator.train.task.get_dataset_metric().name
+        ml_algo = deepcopy(ml_algo)
+
+        flg_new_iterator = False
+        if self._fit_on_holdout and type(train_valid_iterator) != HoldoutIterator:
+            train_valid_iterator = train_valid_iterator.convert_to_holdout_iterator()
+            flg_new_iterator = True
+
+        # TODO: Check if time estimation will be ok with multiprocessing
+        def update_trial_time(study: optuna.study.Study, trial: optuna.trial.FrozenTrial):
+            """Callback for number of iteration with time cut-off.
+
+            Args:
+                study: Optuna study object.
+                trial: Optuna trial object.
+
+            """
+            ml_algo.mean_trial_time = study.trials_dataframe()["duration"].mean().total_seconds()
+            self.estimated_n_trials = min(self.n_trials, self.timeout // ml_algo.mean_trial_time)
+
+            logger.info3(
+                f"\x1b[1mTrial {len(study.trials)}\x1b[0m with hyperparameters {trial.params} scored {trial.value} in {trial.duration}"
+            )
+
+        try:
+            sampler = optuna.samplers.TPESampler(seed=self.random_state)
+            self.study = optuna.create_study(direction=self.direction, sampler=sampler)
+
+            self.study.optimize(
+                func=self._get_objective(
+                    ml_algo=ml_algo,
+                    estimated_n_trials=self.estimated_n_trials,
+                    train_valid_iterator=train_valid_iterator,
+                ),
+                n_trials=self.n_trials,
+                timeout=self.timeout,
+                callbacks=[update_trial_time],
+                # show_progress_bar=True,
+            )
+
+            # need to update best params here
+            if self.direction == "maximize":
+                self._best_params = max(self._params_scores, key=lambda x: x[1])[0]
+            else:
+                self._best_params = min(self._params_scores, key=lambda x: x[1])[0]
+
+            ml_algo.params = self._best_params
+            del self._params_scores
+
+            logger.info(f"Hyperparameters optimization for \x1b[1m{ml_algo._name}\x1b[0m completed")
+            logger.info2(
+                f"The set of hyperparameters \x1b[1m{self._best_params}\x1b[0m\n achieve {self.study.best_value:.4f} {metric_name}"
+            )
+
+            if flg_new_iterator:
+                # if tuner was fitted on holdout set we dont need to save train results
+                return None, None
+
+            preds_ds = ml_algo.fit_predict(train_valid_iterator)
+
+            return ml_algo, preds_ds
+        except optuna.exceptions.OptunaError:
+            del self._params_scores
+            return None, None
+
+    def _get_objective(
+        self,
+        ml_algo: TunableAlgo,
+        estimated_n_trials: int,
+        train_valid_iterator: TrainValidIterator,
+    ) -> Callable[[optuna.trial.Trial], Union[float, int]]:
+        """Get objective.
+
+        Args:
+            ml_algo: Tunable algorithm.
+            estimated_n_trials: Maximum number of hyperparameter estimations.
+            train_valid_iterator: Used for getting parameters
+                depending on dataset.
+
+        Returns:
+            Callable objective.
+
+        """
+        assert isinstance(ml_algo, MLAlgo)
+
+        def objective(trial: optuna.trial.Trial) -> float:
+            _ml_algo = deepcopy(ml_algo)
+
+            optimization_search_space = _ml_algo.optimization_search_space
+            if not optimization_search_space:
+                optimization_search_space = _ml_algo._default_sample
+
+            if callable(optimization_search_space):
+                sampled_params = optimization_search_space(
+                    trial=trial,
+                    estimated_n_trials=estimated_n_trials,
+                    suggested_params=_ml_algo.init_params_on_input(train_valid_iterator),
+                )
+            else:
+                sampled_params = self._sample(
+                    trial=trial,
+                    optimization_search_space=optimization_search_space,
+                    suggested_params=_ml_algo.init_params_on_input(train_valid_iterator),
+                )
+
+            _ml_algo.params = sampled_params
+            output_dataset = _ml_algo.fit_predict(train_valid_iterator=train_valid_iterator)
+            score = _ml_algo.score(output_dataset)
+            self._params_scores.append((sampled_params, score))
+            return score
+
+        return objective
+
+    def _sample(
+        self,
+        optimization_search_space,
+        trial: optuna.trial.Trial,
+        suggested_params: dict,
+    ) -> dict:
+        # logger.info3(f'Suggested parameters: {suggested_params}')
+        trial_values = copy(suggested_params)
+        for parameter_name, search_space in optimization_search_space.items():
+            not_supported = True
+            for key_class in OPTUNA_DISTRIBUTIONS_MAP:
+                if isinstance(search_space, key_class):
+                    wrapped_search_space = OPTUNA_DISTRIBUTIONS_MAP[key_class](search_space)
+                    trial_values[parameter_name] = wrapped_search_space(
+                        name=parameter_name,
+                        trial=trial,
+                    )
+                    not_supported = False
+            if not_supported:
+                raise ValueError(f"Optuna does not support distribution {search_space}")
+
+    def plot(self):
+        """Plot optimization history of all trials in a study."""
+        return optuna.visualization.plot_optimization_history(self.study)
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/ml_algo/utils.py` & `lightautoml-0.3.8b1/lightautoml/ml_algo/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,32 +41,38 @@
     if not force_calc and (
         (single_fold_time is not None and single_fold_time > timer.time_left) or timer.time_limit_exceeded()
     ):
         return None, None
 
     if params_tuner.best_params is None:
         # this try/except clause was added because catboost died for some unexpected reason
-        try:
-            # TODO: Set some conditions to the tuner
+        if getattr(ml_algo, "debug", False):
             new_algo, preds = params_tuner.fit(ml_algo, train_valid)
-        except Exception as e:
-            logger.info2("Model {0} failed during params_tuner.fit call.\n\n{1}".format(ml_algo.name, e))
-            return None, None
+        else:
+            try:
+                # TODO: Set some conditions to the tuner
+                new_algo, preds = params_tuner.fit(ml_algo, train_valid)
+            except Exception as e:
+                logger.info2("Model {0} failed during params_tuner.fit call.\n\n{1}".format(ml_algo.name, e))
+                return None, None
 
         if preds is not None:
             return new_algo, preds
 
     if not force_calc and (
         (single_fold_time is not None and single_fold_time > timer.time_left) or timer.time_limit_exceeded()
     ):
         return None, None
 
     ml_algo.params = params_tuner.best_params
     # this try/except clause was added because catboost died for some unexpected reason
-    try:
+    if getattr(ml_algo, "debug", False):
         preds = ml_algo.fit_predict(train_valid)
-    except Exception as e:
-        logger.info2("Model {0} failed during ml_algo.fit_predict call.\n\n{1}".format(ml_algo.name, e))
-        logger.info3(traceback.format_exc())
-        return None, None
+    else:
+        try:
+            preds = ml_algo.fit_predict(train_valid)
+        except Exception as e:
+            logger.info2("Model {0} failed during ml_algo.fit_predict call.\n\n{1}".format(ml_algo.name, e))
+            logger.info3(traceback.format_exc())
+            return None, None
 
     return ml_algo, preds
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/ml_algo/whitebox.py` & `lightautoml-0.3.8b1/lightautoml/ml_algo/whitebox.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/pipelines/features/base.py` & `lightautoml-0.3.8b1/lightautoml/pipelines/features/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Basic classes for features generation."""
 
+import logging
+
 from copy import copy
 from copy import deepcopy
 from typing import Any
 from typing import Callable
 from typing import List
 from typing import Optional
 from typing import Tuple
@@ -13,14 +15,15 @@
 
 from pandas import DataFrame
 from pandas import Series
 
 from ...dataset.base import LAMLDataset
 from ...dataset.np_pd_dataset import NumpyDataset
 from ...dataset.np_pd_dataset import PandasDataset
+from ...dataset.roles import CategoryRole
 from ...dataset.roles import ColumnRole
 from ...dataset.roles import NumericRole
 from ...transformers.base import ChangeRoles
 from ...transformers.base import ColumnsSelector
 from ...transformers.base import ConvertDataset
 from ...transformers.base import LAMLTransformer
 from ...transformers.base import SequentialTransformer
@@ -30,21 +33,26 @@
 from ...transformers.categorical import LabelEncoder
 from ...transformers.categorical import MultiClassTargetEncoder
 from ...transformers.categorical import MultioutputTargetEncoder
 from ...transformers.categorical import OrdinalEncoder
 from ...transformers.categorical import TargetEncoder
 from ...transformers.datetime import BaseDiff
 from ...transformers.datetime import DateSeasons
+from ...transformers.groupby import GroupByTransformer
+from ...transformers.numeric import FillInf
+from ...transformers.numeric import FillnaMedian
 from ...transformers.numeric import QuantileBinning
 from ..utils import get_columns_by_role
 from ..utils import map_pipeline_names
 
 
 NumpyOrPandas = Union[PandasDataset, NumpyDataset]
 
+logger = logging.getLogger(__name__)
+
 
 class FeaturesPipeline:
     """Abstract class.
 
     Analyze train dataset and create composite transformer
     based on subset of features.
     Instance can be interpreted like Transformer
@@ -210,14 +218,20 @@
         self.random_state = 42
         self.feats_imp = None
         self.ascending_by_cardinality = False
 
         self.max_bin_count = 10
         self.sparse_ohe = "auto"
 
+        self.groupby_types = ["delta_median", "delta_mean", "min", "max", "std", "mode", "is_mode"]
+        self.groupby_triplets = []
+        self.groupby_top_based_on = "cardinality"
+        self.groupby_top_categorical = 3
+        self.groupby_top_numerical = 3
+
         for k in kwargs:
             self.__dict__[k] = kwargs[k]
 
     @staticmethod
     def get_cols_for_datetime(train: NumpyOrPandas) -> Tuple[List[str], List[str]]:
         """Get datetime columns to calculate features.
 
@@ -478,16 +492,18 @@
 
             categories = get_columns_by_role(train, "Category")
             feats_to_select = categories
 
             if len(categories) <= 1:
                 return
 
+            if self.max_intersection_depth <= 1 or self.top_intersections <= 1:
+                return
             elif len(categories) > self.top_intersections:
-                feats_to_select = self.get_top_categories(train, self.top_intersections)
+                feats_to_select = self.get_top_categories(train, mode="cat_intersections", top_n=self.top_intersections)
 
         elif len(feats_to_select) <= 1:
             return
 
         cat_processing = [
             ColumnsSelector(keys=feats_to_select),
             CatIntersectstions(
@@ -522,48 +538,159 @@
                 )
 
             un = feat.value_counts(dropna=False)
             uns.append(un.shape[0])
 
         return Series(uns, index=feats, dtype="int")
 
-    def get_top_categories(self, train: NumpyOrPandas, top_n: int = 5) -> List[str]:
+    def get_top_categories(self, train: NumpyOrPandas, mode: str, top_n: int = 5) -> List[str]:
         """Get top categories by importance.
 
         If feature importance is not defined,
         or feats has same importance - sort it by unique values counts.
         In second case init param ``ascending_by_cardinality``
         defines how - asc or desc.
 
         Args:
             train: Dataset with train data.
+            mode: What feature generation mode is used. Can be "cat_intersections" or "groupby".
             top_n: Number of top categories.
 
         Returns:
             List.
 
         """
-        if self.max_intersection_depth <= 1 or self.top_intersections <= 1:
-            return []
-
+        assert mode in ["cat_intersections", "groupby"]
         cats = get_columns_by_role(train, "Category")
-        if len(cats) == 0:
+        if len(cats) == 0 or top_n == 0:
             return []
-
+        elif len(cats) <= top_n:
+            return cats
         df = DataFrame({"importance": 0, "cardinality": 0}, index=cats)
         # importance if defined
         if self.feats_imp is not None:
             feats_imp = Series(self.feats_imp.get_features_score()).sort_values(ascending=False)
             df["importance"] = feats_imp[feats_imp.index.isin(cats)]
             df["importance"].fillna(-np.inf)
-
         # check for cardinality
         df["cardinality"] = self.get_uniques_cnt(train, cats)
         # sort
-        df = df.sort_values(
-            by=["importance", "cardinality"],
-            ascending=[False, self.ascending_by_cardinality],
-        )
+        if mode == "groupby" and self.groupby_top_based_on == "cardinality" or self.feats_imp is None:
+            df = df.sort_values(by="cardinality", ascending=self.ascending_by_cardinality)
+        else:
+            df = df.sort_values(by="importance", ascending=False)
         # get top n
         top = list(df.index[:top_n])
+        return top
+
+    def get_top_numeric(self, train: NumpyOrPandas, top_n: int = 5) -> List[str]:
+        """Get top numeric features by importance.
 
+        If feature importance is not defined,
+        or feats has same importance - sort it by unique values counts.
+        In second case init param ``ascending_by_cardinality``
+        defines how - asc or desc.
+
+        Args:
+            train: Dataset with train data.
+            top_n: Number of top numeric features.
+
+        Returns:
+            List.
+        """
+        nums = get_columns_by_role(train, "Numeric")
+        if len(nums) == 0 or top_n == 0:
+            return []
+        elif len(nums) <= top_n:
+            return nums
+        df = DataFrame({"importance": 0, "cardinality": 0}, index=nums)
+        # importance if defined
+        if self.feats_imp is not None:
+            feats_imp = Series(self.feats_imp.get_features_score()).sort_values(ascending=False)
+            df["importance"] = feats_imp[feats_imp.index.isin(nums)]
+            df["importance"].fillna(-np.inf)
+        # check for cardinality
+        df["cardinality"] = -self.get_uniques_cnt(train, nums)
+        # sort
+        if self.groupby_top_based_on == "cardinality" or self.feats_imp is None:
+            df = df.sort_values(by="cardinality", ascending=self.ascending_by_cardinality)
+        else:
+            df = df.sort_values(by="importance", ascending=False)
+        # get top n
+        top = list(df.index[:top_n])
         return top
+
+    def get_groupby(self, train: NumpyOrPandas) -> Optional[LAMLTransformer]:
+        """Get transformer that calculates group by features.
+
+        Amount of features is limited to ``self.top_group_by_categorical`` and ``self.top_group_by_numerical`` fields.
+
+        Args:
+            train: Dataset with train data.
+
+        Returns:
+            Transformer.
+        """
+        categorical_names = get_columns_by_role(train, "Category")
+        numerical_names = get_columns_by_role(train, "Numeric")
+
+        groupby_transformations = []
+        if len(self.groupby_triplets) > 0:
+            for group_col, feat_name, trans in self.groupby_triplets:
+                categorical_cols = [] if feat_name in numerical_names else [feat_name]
+                numeric_cols = [] if feat_name in categorical_names else [feat_name]
+                if len(categorical_cols) + len(numeric_cols) == 0:
+                    logging.info2("Feature is incorrect or dropped by preselector: {}".format(feat_name))
+                    continue
+                if group_col not in categorical_names:
+                    logging.info2("Groupby column is incorrect or dropped by preselector: {}".format(group_col))
+                    continue
+                new_transformation = {
+                    "group_col": group_col,
+                    "categorical_cols": categorical_cols,
+                    "numeric_cols": numeric_cols,
+                    "used_transforms": [trans],
+                }
+                groupby_transformations.append(new_transformation)
+        else:
+            cat_feats_to_select = self.get_top_categories(train, "groupby", self.groupby_top_categorical)
+            num_feats_to_select = self.get_top_numeric(train, self.groupby_top_numerical)
+            # At least two categoricals or one categorical and one numeric
+            if len(cat_feats_to_select) < 1:
+                return
+            if len(cat_feats_to_select) == 1 and len(num_feats_to_select) < 1:
+                return
+            # collect groupby_transformations
+            for i, group_col in enumerate(cat_feats_to_select):
+                new_transformation = {
+                    "group_col": group_col,
+                    "categorical_cols": cat_feats_to_select[:i] + cat_feats_to_select[i + 1 :],
+                    "numeric_cols": num_feats_to_select,
+                    "used_transforms": self.groupby_types,
+                }
+                groupby_transformations.append(new_transformation)
+
+        groupby_processing = [
+            SequentialTransformer(
+                [
+                    UnionTransformer(
+                        [
+                            SequentialTransformer(
+                                [
+                                    ColumnsSelector(keys=[trans["group_col"]] + trans["categorical_cols"]),
+                                    LabelEncoder(subs=None, random_state=42),
+                                    ChangeRoles(CategoryRole(int)),
+                                ]
+                            ),
+                            SequentialTransformer(
+                                [ColumnsSelector(keys=trans["numeric_cols"]), FillInf(), FillnaMedian()]
+                            ),
+                        ]
+                    ),
+                    GroupByTransformer(**trans),
+                ]
+            )
+            for trans in groupby_transformations
+        ]
+        groupby_processing = UnionTransformer(groupby_processing)
+
+        return groupby_processing
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/pipelines/features/generator_pipeline.py` & `lightautoml-0.3.8b1/lightautoml/pipelines/features/generator_pipeline.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/pipelines/features/image_pipeline.py` & `lightautoml-0.3.8b1/lightautoml/pipelines/features/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/pipelines/features/lgb_pipeline.py` & `lightautoml-0.3.8b1/lightautoml/pipelines/features/lgb_pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Pipeline for tree based models."""
 
+from typing import List
 from typing import Optional
 from typing import Union
 
 import numpy as np
 
 from ...dataset.np_pd_dataset import NumpyDataset
 from ...dataset.np_pd_dataset import PandasDataset
@@ -20,18 +21,20 @@
 from ...transformers.categorical import OrdinalEncoder
 from ...transformers.datetime import TimeToNum
 from ...transformers.numeric import FillInf
 from ...transformers.numeric import FillnaMedian
 from ...transformers.numeric import NaNFlags
 from ...transformers.numeric import StandardScaler
 from ...transformers.seq import GetSeqTransformer
+from ...transformers.seq import SeqDiffTransformer
 from ...transformers.seq import SeqLagTransformer
 from ...transformers.seq import SeqNumCountsTransformer
 from ...transformers.seq import SeqStatisticsTransformer
 from ..selection.base import ImportanceEstimator
+from ..selection.base import SelectionPipeline
 from ..utils import get_columns_by_role
 from .base import FeaturesPipeline
 from .base import TabularDataFeatures
 
 
 NumpyOrPandas = Union[PandasDataset, NumpyDataset]
 
@@ -115,14 +118,15 @@
         max_intersection_depth: int = 3,
         subsample: Optional[Union[int, float]] = None,
         multiclass_te_co: int = 3,
         auto_unique_co: int = 10,
         output_categories: bool = False,
         fill_na=False,
         scaler=False,
+        transformers_params=None,
         **kwargs
     ):
         super().__init__(
             multiclass_te_co=multiclass_te_co,
             top_intersections=top_intersections,
             max_intersection_depth=max_intersection_depth,
             subsample=subsample,
@@ -130,75 +134,130 @@
             auto_unique_co=auto_unique_co,
             output_categories=output_categories,
             ascending_by_cardinality=False,
         )
 
         self.fill_na = fill_na
         self.scaler = scaler
+        self.transformers_params = transformers_params
 
     def get_seq_pipeline(self, train):
         """Create pipeline for seq data.
 
         Args:
             train: Dataset with train features.
 
         Returns:
             Composite datetime, categorical, numeric transformer.
 
         """
-        transformers_list = []
-        # process categories
-
         # process datetimes
+        time_transformers_list = []
+
+        # datetimes features generating
+        time_features_transformers_list = []
         datetimes = get_columns_by_role(train, "Datetime")
         if len(datetimes) > 0:
             dt_processing = SequentialTransformer([ColumnsSelector(keys=datetimes), TimeToNum()])
-            transformers_list.append(dt_processing)
-            transformers_list.append(self.get_datetime_diffs(train))
-            transformers_list.append(self.get_datetime_seasons(train, NumericRole(np.float32)))
+            time_features_transformers_list.append(dt_processing)
+            time_features_transformers_list.append(self.get_datetime_diffs(train))
+            time_features_transformers_list.append(self.get_datetime_seasons(train, NumericRole(np.float32)))
+
+        # datetime features preprocessing
+        time_preprocessing_transformers_list = []
+        if self.fill_na:
+            time_preprocessing_transformers_list.append(
+                UnionTransformer([SequentialTransformer([FillInf(), FillnaMedian()]), NaNFlags()])
+            )
+
+            if self.scaler:
+                time_preprocessing_transformers_list.append(StandardScaler())
+
+        time_transformers_list.append(UnionTransformer(time_features_transformers_list))
+        time_transformers_list += time_preprocessing_transformers_list
+
+        time_transforms = SequentialTransformer(time_transformers_list)
+
+        if self.transformers_params["lag_time_features"]:
+            seq = ColumnsSelector(keys=[])  # SequentialTransformer([EmptyTransformer(), ColumnsSelector(keys=[])])
+            time_transforms = SequentialTransformer(
+                [
+                    UnionTransformer([time_transforms, seq]),
+                    SeqLagTransformer(lags=self.transformers_params["lag_time_features"]),
+                ]
+            )
+
+        # process other features
+        other_transformers_list = []
 
+        # process categories
+        other_features_transformers_list = []
         categories = get_columns_by_role(train, "Category")
         if len(categories) > 0:
             cat_processing = SequentialTransformer(
                 [
                     ColumnsSelector(keys=categories),
                     LabelEncoder(subs=None, random_state=42),
                     ChangeRoles(NumericRole(np.float32)),
                 ]
             )
-            transformers_list.append(cat_processing)
+            other_features_transformers_list.append(cat_processing)
 
+        # process numeric
         numerics = get_columns_by_role(train, "Numeric")
         if len(numerics) > 0:
             num_processing = SequentialTransformer(
                 [ColumnsSelector(keys=numerics), ConvertDataset(dataset_type=NumpyDataset)]
             )
-            transformers_list.append(num_processing)
-
-        simple_seq_transforms = UnionTransformer(transformers_list)
+            other_features_transformers_list.append(num_processing)
 
+        # other features preprocessing
+        other_preprocessing_transformers_list = []
         if self.fill_na:
-            filler = UnionTransformer([SequentialTransformer([FillInf(), FillnaMedian()]), NaNFlags()])
+            other_preprocessing_transformers_list.append(
+                UnionTransformer([SequentialTransformer([FillInf(), FillnaMedian()]), NaNFlags()])
+            )
 
             if self.scaler:
-                filler = SequentialTransformer([filler, StandardScaler()])
+                other_preprocessing_transformers_list.append(StandardScaler())
 
-            simple_seq_transforms = SequentialTransformer([simple_seq_transforms, filler])
+        other_transformers_list.append(UnionTransformer(other_features_transformers_list))
+        other_transformers_list += other_preprocessing_transformers_list
 
-        # to seq dataset
-        seq = ColumnsSelector(keys=[])  # SequentialTransformer([EmptyTransformer(), ColumnsSelector(keys=[])])
-        simple_seq_transforms = UnionTransformer([seq, simple_seq_transforms])
+        lags = self.transformers_params["lag_features"]
+        diffs = self.transformers_params["diff_features"]
+
+        other_transforms = SequentialTransformer(other_transformers_list)
+
+        if lags or diffs:
+            seq = ColumnsSelector(keys=[])  # SequentialTransformer([EmptyTransformer(), ColumnsSelector(keys=[])])
+            seq_features = []
+
+            if lags:
+                seq_features.append(SeqLagTransformer(lags=lags))
+
+            if diffs:
+                # if we have lag with number 0, we shouldn't have diff with number 0
+                if lags:
+                    flag_del_0_diff = not (
+                        not isinstance(diffs, int) and 0 not in diffs or not isinstance(lags, int) and 0 not in lags
+                    )
+                else:
+                    flag_del_0_diff = False
+                seq_features.append(SeqDiffTransformer(diffs=diffs, flag_del_0_diff=flag_del_0_diff))
+
+            other_transforms = SequentialTransformer(
+                [UnionTransformer([other_transforms, seq]), UnionTransformer(seq_features)]
+            )
 
-        # get seq features
         all_feats = SequentialTransformer(
             [
                 GetSeqTransformer(name=train.name),
                 SetAttribute("date", datetimes[0]),
-                simple_seq_transforms,  # preprocessing
-                SeqLagTransformer(n_lags=30),  # plain features
+                UnionTransformer([time_transforms, other_transforms]),
             ]
         )
 
         return all_feats
 
     def create_pipeline(self, train: NumpyOrPandas) -> LAMLTransformer:
         """Create tree pipeline.
@@ -427,35 +486,48 @@
             handling on multiclass task if number of classes is high.
         auto_unique_co: Switch to target encoding if high cardinality.
 
     """
 
     def __init__(
         self,
-        feats_imp: Optional[ImportanceEstimator] = None,
+        feats_imp: Optional[Union[ImportanceEstimator, SelectionPipeline]] = None,
         top_intersections: int = 5,
         max_intersection_depth: int = 3,
         subsample: Optional[Union[int, float]] = None,
         multiclass_te_co: int = 3,
         auto_unique_co: int = 10,
         output_categories: bool = False,
-        fill_na=False,
+        fill_na: bool = False,
+        ascending_by_cardinality: bool = False,
+        use_groupby: bool = False,
+        groupby_types: List[str] = ["delta_median", "delta_mean", "min", "max", "std", "mode", "is_mode"],
+        groupby_triplets: list = [],
+        groupby_top_based_on: str = "cardinality",
+        groupby_top_categorical: int = 3,
+        groupby_top_numerical: int = 3,
         **kwargs
     ):
         super().__init__(
             multiclass_te_co=multiclass_te_co,
             top_intersections=top_intersections,
             max_intersection_depth=max_intersection_depth,
             subsample=subsample,
             feats_imp=feats_imp,
             auto_unique_co=auto_unique_co,
             output_categories=output_categories,
-            ascending_by_cardinality=False,
+            ascending_by_cardinality=ascending_by_cardinality,
+            groupby_types=groupby_types,
+            groupby_triplets=groupby_triplets,
+            groupby_top_based_on=groupby_top_based_on,
+            groupby_top_categorical=groupby_top_categorical,
+            groupby_top_numerical=groupby_top_numerical,
         )
         self.fill_na = fill_na
+        self.use_groupby = use_groupby
 
     def create_pipeline(self, train: NumpyOrPandas) -> LAMLTransformer:
         """Create tree pipeline.
 
         Args:
             train: Dataset with train features.
 
@@ -532,13 +604,16 @@
         transformer_list.append(self.get_numeric_data(train))
         transformer_list.append(self.get_ordinal_encoding(train, ordinal))
         # add difference with base date
         transformer_list.append(self.get_datetime_diffs(train))
         # add datetime seasonality
         transformer_list.append(self.get_datetime_seasons(train, NumericRole(np.float32)))
 
+        if self.use_groupby:
+            transformer_list.append(self.get_groupby(train))
+
         # final pipeline
         union_all = UnionTransformer([x for x in transformer_list if x is not None])
         if self.fill_na:
             union_all = SequentialTransformer([union_all, SequentialTransformer([FillInf(), FillnaMedian()])])
 
         return union_all
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/pipelines/features/linear_pipeline.py` & `lightautoml-0.3.8b1/lightautoml/pipelines/features/linear_pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Linear models features."""
 
+from typing import List
 from typing import Optional
 from typing import Union
 
 import numpy as np
 
 from ...dataset.np_pd_dataset import NumpyDataset
 from ...dataset.np_pd_dataset import PandasDataset
@@ -18,14 +19,15 @@
 from ...transformers.datetime import TimeToNum
 from ...transformers.numeric import FillInf
 from ...transformers.numeric import FillnaMedian
 from ...transformers.numeric import LogOdds
 from ...transformers.numeric import NaNFlags
 from ...transformers.numeric import StandardScaler
 from ..selection.base import ImportanceEstimator
+from ..selection.base import SelectionPipeline
 from ..utils import get_columns_by_role
 from .base import FeaturesPipeline
 from .base import TabularDataFeatures
 
 
 NumpyOrPandas = Union[PandasDataset, NumpyDataset]
 
@@ -58,23 +60,29 @@
             on multiclass task if number of classes is high.
 
 
     """
 
     def __init__(
         self,
-        feats_imp: Optional[ImportanceEstimator] = None,
+        feats_imp: Optional[Union[ImportanceEstimator, SelectionPipeline]] = None,
         top_intersections: int = 5,
         max_bin_count: int = 10,
         max_intersection_depth: int = 3,
         subsample: Optional[Union[int, float]] = None,
         sparse_ohe: Union[str, bool] = "auto",
         auto_unique_co: int = 50,
         output_categories: bool = True,
         multiclass_te_co: int = 3,
+        use_groupby: bool = False,
+        groupby_types: List[str] = ["delta_median", "delta_mean", "min", "max", "std", "mode", "is_mode"],
+        groupby_triplets: list = [],
+        groupby_top_based_on: str = "cardinality",
+        groupby_top_categorical: int = 3,
+        groupby_top_numerical: int = 3,
         **kwargs
     ):
         assert max_bin_count is None or max_bin_count > 1, "Max bin count should be >= 2 or None"
 
         super().__init__(
             multiclass_te=False,
             top_intersections=top_intersections,
@@ -83,15 +91,21 @@
             feats_imp=feats_imp,
             auto_unique_co=auto_unique_co,
             output_categories=output_categories,
             ascending_by_cardinality=True,
             max_bin_count=max_bin_count,
             sparse_ohe=sparse_ohe,
             multiclass_te_co=multiclass_te_co,
+            groupby_types=groupby_types,
+            groupby_triplets=groupby_triplets,
+            groupby_top_based_on=groupby_top_based_on,
+            groupby_top_categorical=groupby_top_categorical,
+            groupby_top_numerical=groupby_top_numerical,
         )
+        self.use_groupby = use_groupby
 
     def create_pipeline(self, train: NumpyOrPandas) -> LAMLTransformer:
         """Create linear pipeline.
 
         Args:
             train: Dataset with train features.
 
@@ -163,14 +177,17 @@
         # add ordinal categories
         dense_list.append(self.get_ordinal_encoding(train))
         # add probs
         probs_list.append(self.get_numeric_data(train, prob=True))
         # add difference with base date
         dense_list.append(self.get_datetime_diffs(train))
 
+        if self.use_groupby:
+            dense_list.append(self.get_groupby(train))
+
         # combine it all together
         # handle probs if exists
         probs_list = [x for x in probs_list if x is not None]
         if len(probs_list) > 0:
             probs_pipe = UnionTransformer(probs_list)
             probs_pipe = SequentialTransformer([probs_pipe, LogOdds()])
             dense_list.append(probs_pipe)
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/pipelines/features/text_pipeline.py` & `lightautoml-0.3.8b1/lightautoml/pipelines/features/text_pipeline.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/pipelines/features/wb_pipeline.py` & `lightautoml-0.3.8b1/lightautoml/pipelines/features/wb_pipeline.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/pipelines/ml/base.py` & `lightautoml-0.3.8b1/lightautoml/pipelines/ml/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 
         # train and apply post selection
         train_valid = train_valid.apply_selector(self.post_selection)
 
         predictions = []
 
         for ml_algo, param_tuner, force_calc in zip(self._ml_algos, self.params_tuners, self.force_calc):
+            ml_algo.debug = getattr(self, "debug", False)
             ml_algo, preds = tune_and_fit_predict(ml_algo, param_tuner, train_valid, force_calc)
             if ml_algo is not None:
                 self.ml_algos.append(ml_algo)
 
                 predictions.append(preds)
 
         assert (
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/pipelines/ml/nested_ml_pipe.py` & `lightautoml-0.3.8b1/lightautoml/pipelines/ml/nested_ml_pipe.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/pipelines/ml/whitebox_ml_pipe.py` & `lightautoml-0.3.8b1/lightautoml/pipelines/ml/whitebox_ml_pipe.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/pipelines/selection/base.py` & `lightautoml-0.3.8b1/lightautoml/pipelines/selection/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,23 +195,23 @@
             dataset: Dataset for feature selection.
 
         Returns:
             New dataset with selected features only.
 
         """
         selected_features = copy(self.selected_features)
-        # Add features that forces input
-        sl_set = set(selected_features)
-        roles = dataset.roles
-        for col in (x for x in dataset.features if x not in sl_set):
-            if roles[col].force_input:
-                if col not in sl_set:
-                    selected_features.append(col)
 
-        return dataset[:, self.selected_features]
+        # Add forced features
+        selected_features = selected_features + [
+            feature
+            for feature in dataset.features
+            if dataset.roles[feature].force_input and (feature not in selected_features)
+        ]
+
+        return dataset[:, selected_features]
 
     def map_raw_feature_importances(self, raw_importances: Series):
         """Calculate input feature importances.
 
         Calculated as sum of importances on different levels of pipeline.
 
         Args:
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/pipelines/selection/importance_based.py` & `lightautoml-0.3.8b1/lightautoml/pipelines/selection/importance_based.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/pipelines/selection/linear_selector.py` & `lightautoml-0.3.8b1/lightautoml/pipelines/selection/linear_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
         if self.subsample != 1 and self.subsample < train.shape[0]:
             if self.subsample < 1:
                 subsample = int(train.shape[0] * self.subsample)
             else:
                 subsample = int(self.subsample)
 
-            idx = np.random.RandomState(self.random_state).permutation(train.shape[0])[:subsample]
+            idx = np.random.RandomState(self.random_state + 1).permutation(train.shape[0])[:subsample]
             train, target = train[idx], target[idx]
 
         # correlation or cosine
         if type(train) is np.ndarray:
             corr = np.corrcoef(train, rowvar=False)
 
         else:
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/pipelines/selection/permutation_importance_based.py` & `lightautoml-0.3.8b1/lightautoml/pipelines/selection/permutation_importance_based.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         """
         normal_score = ml_algo.score(preds)
         logger.debug("Normal score = {}".format(normal_score))
 
         valid_data = train_valid.get_validation_data()
         valid_data = valid_data.to_numpy()
 
-        permutation = np.random.RandomState(seed=self.random_state).permutation(valid_data.shape[0])
+        permutation = np.random.RandomState(seed=self.random_state + 1).permutation(valid_data.shape[0])
         permutation_importance = {}
 
         for it, col in enumerate(valid_data.features):
             logger.debug("Start processing ({},{})".format(it, col))
             # Save initial column
             save_col = deepcopy(valid_data[:, col])
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/pipelines/utils.py` & `lightautoml-0.3.8b1/lightautoml/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/reader/base.py` & `lightautoml-0.3.8b1/lightautoml/reader/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,15 @@
         self._n_classes = len(unqiues)
 
         # case - target correctly defined and no mapping
         if (np.arange(srtd.shape[0]) == srtd).all():
             assert srtd.shape[0] > 1, "Less than 2 unique values in target"
             if (self.task.name == "binary") or (self.task.name == "multilabel"):
                 assert srtd.shape[0] == 2, "Binary task and more than 2 values in target"
-                return target, None
+            return target, None
 
         # case - create mapping
         class_mapping = {n: x for (x, n) in enumerate(unqiues)}
         return target.map(class_mapping).astype(np.int32), class_mapping
 
     def _get_default_role_from_str(self, name) -> RoleType:
         """Get default role for string name according to automl's defaults and user settings.
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/reader/guess_roles.py` & `lightautoml-0.3.8b1/lightautoml/reader/guess_roles.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,18 @@
         Metric value.
 
     """
     actual = np.asarray(actual)
     n = len(actual)
     a_s = actual[np.argsort(pred)]
     a_c = a_s.cumsum()
+
+    if a_s.sum() == 0:
+        return 0
+
     gini_sum = a_c.sum() / a_s.sum() - (n + 1) / 2.0
     return gini_sum / n
 
 
 def gini_normalizedc(a: np.ndarray, p: np.ndarray) -> float:
     """Calculated normalized gini.
 
@@ -64,15 +68,20 @@
         a: True values.
         p: Predicted values.
 
     Returns:
         Metric value.
 
     """
-    return ginic(a, p) / ginic(a, a)
+    ginic_aa = ginic(a, a)
+
+    if ginic_aa:
+        return ginic(a, p) / ginic_aa
+
+    return 0
 
 
 def gini_normalized(y_true: np.ndarray, y_pred: np.ndarray, empty_slice: Optional[np.ndarray] = None):
     """Calculate normalized gini index.
 
     Args:
         y_true: True values.
@@ -294,15 +303,15 @@
 
     train = train[:, roles_to_identify].to_numpy()
 
     if train.folds is None:
         train.folds = set_sklearn_folds(train.task, train.target, cv=5, random_state=42, group=train.group)
 
     if subsample is not None:
-        idx = np.random.RandomState(random_state).permutation(train.shape[0])[:subsample]
+        idx = np.random.RandomState(random_state + 1).permutation(train.shape[0])[:subsample]
         train = train[idx]
 
     data, target = train.data, train.target
 
     # check task specific
     target, encoder = get_target_and_encoder(train)
 
@@ -509,15 +518,15 @@
 
     train = train[:, roles_to_identify].to_pandas()
 
     if train.folds is None:
         train.folds = set_sklearn_folds(train.task, train.target.values, cv=5, random_state=42, group=train.group)
 
     if subsample is not None:
-        idx = np.random.RandomState(random_state).permutation(train.shape[0])[:subsample]
+        idx = np.random.RandomState(random_state + 1).permutation(train.shape[0])[:subsample]
         train = train[idx]
 
     # check task specific
     target, encoder = get_target_and_encoder(train)
 
     empty_slice = train.data.isnull().values
 
@@ -622,15 +631,15 @@
         Series.
 
     """
     if feats is not None:
         train = train[:, feats].to_pandas()
 
     if subsample is not None:
-        idx = np.random.RandomState(random_state).permutation(train.shape[0])[:subsample]
+        idx = np.random.RandomState(random_state + 1).permutation(train.shape[0])[:subsample]
         train = train[idx]
 
     # check task specific
     target, _ = get_target_and_encoder(train)
 
     empty_slice = train.data.isnull().values
     notnan = empty_slice.sum(axis=0)
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/reader/seq.py` & `lightautoml-0.3.8b1/lightautoml/reader/seq.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/reader/tabular_batch_generator.py` & `lightautoml-0.3.8b1/lightautoml/reader/tabular_batch_generator.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/reader/utils.py` & `lightautoml-0.3.8b1/lightautoml/reader/utils.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/binary_inference_section.html` & `lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/binary_inference_section.html`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/lama_base_template.html` & `lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/lama_base_template.html`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/model_section.html` & `lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/model_section.html`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/multiclass_inference_section.html` & `lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/multiclass_inference_section.html`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/reg_inference_section.html` & `lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/reg_inference_section.html`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/train_set_section.html` & `lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/train_set_section.html`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/uplift_subsection.html` & `lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/uplift_subsection.html`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/report/lama_report_templates/whitebox_section.html` & `lightautoml-0.3.8b1/lightautoml/report/lama_report_templates/whitebox_section.html`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/report/report_deco.py` & `lightautoml-0.3.8b1/lightautoml/report/report_deco.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/tasks/base.py` & `lightautoml-0.3.8b1/lightautoml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/tasks/common_metric.py` & `lightautoml-0.3.8b1/lightautoml/tasks/common_metric.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/tasks/losses/base.py` & `lightautoml-0.3.8b1/lightautoml/tasks/losses/base.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/tasks/losses/cb.py` & `lightautoml-0.3.8b1/lightautoml/tasks/losses/cb.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,7 +208,18 @@
                 self.metric_name = _metric_dict[metric]
 
         else:
             # TODO: Check it later
             self.metric_name = self.fobj_name
             self.metric_params = self.fobj_params
             self.metric = None
+
+            if task_name == "multi:reg":
+                logger.info2("CatBoost supports only MultiRMSE metric and loss for multi:reg task.")
+                self.fobj = None
+                self.fobj_name = "MultiRMSE"
+                self.metric_name = "MultiRMSE"
+            if task_name == "multilabel":
+                logger.info2("CatBoost uses as obj. MultiCrossEntropy.")
+                self.fobj = None
+                self.fobj_name = "MultiCrossEntropy"
+                self.metric_name = "MultiCrossEntropy"
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/tasks/losses/cb_custom.py` & `lightautoml-0.3.8b1/lightautoml/tasks/losses/cb_custom.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/tasks/losses/lgb.py` & `lightautoml-0.3.8b1/lightautoml/tasks/losses/lgb.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/tasks/losses/lgb_custom.py` & `lightautoml-0.3.8b1/lightautoml/tasks/losses/lgb_custom.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/tasks/losses/sklearn.py` & `lightautoml-0.3.8b1/lightautoml/tasks/losses/sklearn.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/tasks/losses/torch.py` & `lightautoml-0.3.8b1/lightautoml/tasks/losses/torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,15 @@
         y_pred: predicted target values.
         sample_weight: specify weighted mean.
 
     Returns:
         metric value.
 
     """
+    y_pred = torch.sigmoid(y_pred)
     y_true = y_true[:, 0].type(torch.int64)
     y_true_ohe = torch.zeros_like(y_pred)
 
     y_true_ohe[range(y_true.shape[0]), y_true] = 1
     tp = y_true_ohe * y_pred
     if sample_weight is not None:
         sample_weight = sample_weight.unsqueeze(-1)
@@ -251,16 +252,16 @@
 
     return err.mean()
 
 
 _torch_loss_dict = {
     "mse": (nn.MSELoss, False, False),
     "mae": (nn.L1Loss, False, False),
-    "logloss": (nn.BCELoss, False, False),
-    "crossentropy": (nn.CrossEntropyLoss, True, True),
+    "logloss": (nn.BCEWithLogitsLoss, False, False),
+    "crossentropy": (nn.CrossEntropyLoss, True, False),
     "rmsle": (torch_rmsle, False, False),
     "mape": (torch_mape, False, False),
     "quantile": (torch_quantile, False, False),
     "fair": (torch_fair, False, False),
     "huber": (torch_huber, False, False),
     "f1": (torch_f1, False, False),
 }
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/tasks/utils.py` & `lightautoml-0.3.8b1/lightautoml/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/text/dl_transformers.py` & `lightautoml-0.3.8b1/lightautoml/text/dl_transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 try:
     from transformers import AutoModel
 except:
     import warnings
 
     warnings.warn("'transformers' - package isn't installed")
 
+from ..ml_algo.torch_based.nn_models import SequenceAvgPooler
+from ..ml_algo.torch_based.nn_models import SequenceClsPooler
+from ..ml_algo.torch_based.nn_models import SequenceIndentityPooler
+from ..ml_algo.torch_based.nn_models import SequenceMaxPooler
+from ..ml_algo.torch_based.nn_models import SequenceSumPooler
 from .dp_utils import CustomDataParallel
-from .sentence_pooling import SequenceAvgPooler
-from .sentence_pooling import SequenceClsPooler
-from .sentence_pooling import SequenceIndentityPooler
-from .sentence_pooling import SequenceMaxPooler
-from .sentence_pooling import SequenceSumPooler
 from .utils import _dtypes_mapping
 from .utils import collate_dict
 from .utils import parse_devices
 from .utils import seed_everything
 from .utils import single_text_hash
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/text/dp_utils.py` & `lightautoml-0.3.8b1/lightautoml/text/dp_utils.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/text/embed_dataset.py` & `lightautoml-0.3.8b1/lightautoml/text/embed_dataset.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/text/nn_model.py` & `lightautoml-0.3.8b1/lightautoml/text/nn_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Neural Net modules for differen data types."""
 
+import logging
 
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Optional
 from typing import Sequence
+from typing import Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 
 
 try:
@@ -19,14 +21,17 @@
 
     warnings.warn("'transformers' - package isn't installed")
 
 from ..tasks.base import Task
 from .dl_transformers import pooling_by_name
 
 
+logger = logging.getLogger(__name__)
+
+
 class UniversalDataset:
     """Dataset class for mixed data.
 
     Args:
         data: Dict with data.
         y: Array of target variable.
         w: Optional array of observation weight.
@@ -178,15 +183,15 @@
     ):
         super(CatEmbedder, self).__init__()
         emb_dims = [(int(x), int(min(max_emb_size, max(1, (x + 1) // emb_ratio)))) for x in cat_dims]
         self.no_of_embs = sum([y for x, y in emb_dims])
         assert self.no_of_embs != 0, "The input is empty."
         # Embedding layers
         self.emb_layers = nn.ModuleList([nn.Embedding(x, y) for x, y in emb_dims])
-        self.emb_dropout_layer = nn.Dropout(emb_dropout)
+        self.emb_dropout_layer = nn.Dropout(emb_dropout) if emb_dropout else nn.Identity()
 
     def get_out_shape(self) -> int:
         """Output shape.
 
         Returns:
             Int with module output shape.
 
@@ -213,15 +218,15 @@
         input_bn: Use 1d batch norm for input data.
 
     """
 
     def __init__(self, num_dims: int, input_bn: bool = True):
         super(ContEmbedder, self).__init__()
         self.n_out = num_dims
-        self.bn = None
+        self.bn = nn.Identity()
         if input_bn:
             self.bn = nn.BatchNorm1d(num_dims)
         assert num_dims != 0, "The input is empty."
 
     def get_out_shape(self) -> int:
         """Output shape.
 
@@ -230,55 +235,60 @@
 
         """
         return self.n_out
 
     def forward(self, inp: Dict[str, torch.Tensor]) -> torch.Tensor:
         """Forward-pass."""
         output = inp["cont"]
-        if self.bn is not None:
-            output = self.bn(output)
+        output = self.bn(output)
         return output
 
 
 class TorchUniversalModel(nn.Module):
     """Mixed data model.
 
     Class for preparing input for DL model with mixed data.
 
     Args:
         loss: Callable torch loss with order of arguments (y_true, y_pred).
         task: Task object.
+        torch_model: Torch model.
         n_out: Number of output dimensions.
         cont_embedder: Torch module for numeric data.
         cont_params: Dict with numeric model params.
         cat_embedder: Torch module for category data.
         cat_params: Dict with category model params.
         text_embedder: Torch module for text data.
         text_params: Dict with text model params.
+        loss_on_logits: Calculate loss on logits or on predictions of model for classification tasks.
         bias: Array with last hidden linear layer bias.
 
     """
 
     def __init__(
         self,
         loss: Callable,
         task: Task,
+        torch_model: nn.Module,
         n_out: int = 1,
         cont_embedder: Optional[Any] = None,
         cont_params: Optional[Dict] = None,
         cat_embedder: Optional[Any] = None,
         cat_params: Optional[Dict] = None,
         text_embedder: Optional[Any] = None,
         text_params: Optional[Dict] = None,
-        bias: Optional[Sequence] = None,
+        loss_on_logits: bool = True,
+        bias: Union[np.array, torch.Tensor] = None,
+        **kwargs,
     ):
         super(TorchUniversalModel, self).__init__()
         self.n_out = n_out
         self.loss = loss
         self.task = task
+        self.loss_on_logits = loss_on_logits
 
         self.cont_embedder = None
         self.cat_embedder = None
         self.text_embedder = None
 
         n_in = 0
         if cont_embedder is not None:
@@ -287,44 +297,87 @@
         if cat_embedder is not None:
             self.cat_embedder = cat_embedder(**cat_params)
             n_in += self.cat_embedder.get_out_shape()
         if text_embedder is not None:
             self.text_embedder = text_embedder(**text_params)
             n_in += self.text_embedder.get_out_shape()
 
-        self.bn = nn.BatchNorm1d(n_in)
-        self.fc = torch.nn.Linear(n_in, self.n_out)
+        self.torch_model = (
+            torch_model(
+                **{
+                    **kwargs,
+                    **{"n_in": n_in, "n_out": n_out, "loss": loss, "task": task},
+                }
+            )
+            if torch_model is not None
+            else nn.Sequential(nn.Linear(n_in, n_out))
+        )
 
         if bias is not None:
-            bias = torch.Tensor(bias)
-            self.fc.bias.data = nn.Parameter(bias)
-            self.fc.weight.data = nn.Parameter(torch.zeros(self.n_out, n_in))
-
-        if (self.task.name == "binary") or (self.task.name == "multilabel"):
-            self.fc = nn.Sequential(self.fc, Clump(), nn.Sigmoid())
-        elif self.task.name == "multiclass":
-            self.fc = nn.Sequential(self.fc, Clump(), nn.Softmax(dim=1))
-
-    def forward(self, inp: Dict[str, torch.Tensor]) -> torch.Tensor:
-        """Forward-pass."""
-        x = self.predict(inp)
-        loss = self.loss(inp["label"].view(inp["label"].shape[0], -1), x, inp.get("weight", None))
-        return loss
+            try:
+                last_layer = list(
+                    filter(
+                        lambda x: isinstance(x, nn.Linear) or isinstance(x, nn.Sequential),
+                        list(self.torch_model.children()),
+                    )
+                )[-1]
+                while isinstance(last_layer, nn.Sequential):
+                    last_layer = list(
+                        filter(lambda x: isinstance(x, nn.Linear) or isinstance(x, nn.Sequential), last_layer)
+                    )[-1]
+                bias = torch.Tensor(bias)
+                last_layer.bias.data = bias
+                shape = last_layer.weight.data.shape
+                last_layer.weight.data = torch.zeros(shape[0], shape[1], requires_grad=True)
+            except:
+                logger.info3("Last linear layer not founded, so init_bias=False")
+
+        self.сlump = Clump()
+        self.sig = nn.Sigmoid()
+        self.softmax = nn.Softmax(dim=1)
 
-    def predict(self, inp: Dict[str, torch.Tensor]) -> torch.Tensor:
-        """Prediction."""
+    def get_logits(self, inp: Dict[str, torch.Tensor]) -> torch.Tensor:
+        """Forward-pass of model with embeddings."""
         outputs = []
         if self.cont_embedder is not None:
             outputs.append(self.cont_embedder(inp))
 
         if self.cat_embedder is not None:
             outputs.append(self.cat_embedder(inp))
 
         if self.text_embedder is not None:
             outputs.append(self.text_embedder(inp))
 
         if len(outputs) > 1:
             output = torch.cat(outputs, dim=1)
         else:
             output = outputs[0]
-        logits = self.fc(output)
-        return logits.view(logits.shape[0], -1)
+
+        logits = self.torch_model(output)
+        return logits
+
+    def get_preds_from_logits(self, logits: torch.Tensor) -> torch.Tensor:
+        """Prediction from logits."""
+        if self.task.name in ["binary", "multilabel"]:
+            out = self.sig(self.сlump(logits))
+        elif self.task.name == "multiclass":
+            # cant find self.clump when predicting
+            out = self.softmax(torch.clamp(logits, -50, 50))
+        else:
+            out = logits
+
+        return out
+
+    def forward(self, inp: Dict[str, torch.Tensor]) -> torch.Tensor:
+        """Forward-pass with output loss."""
+        x = self.get_logits(inp)
+        if not self.loss_on_logits:
+            x = self.get_preds_from_logits(x)
+
+        loss = self.loss(inp["label"].view(inp["label"].shape[0], -1), x, inp.get("weight", None))
+        return loss
+
+    def predict(self, inp: Dict[str, torch.Tensor]) -> torch.Tensor:
+        """Prediction."""
+        x = self.get_logits(inp)
+        x = self.get_preds_from_logits(x)
+        return x
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/text/tokenizer.py` & `lightautoml-0.3.8b1/lightautoml/text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/text/trainer.py` & `lightautoml-0.3.8b1/lightautoml/text/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import numpy as np
 import torch
 import torch.nn as nn
 
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
+from ..utils.logging import get_stdout_level
 from .dp_utils import CustomDataParallel
 
 
 try:
     from apex import amp
 except:
     amp = None
@@ -255,14 +256,16 @@
         snap_params: Dict with SE parameters.
         is_snap: Use snapshots.
         sch: Uninitialized torch scheduler.
         scheduler_params: Dict with scheduler params.
         verbose: Verbose every N epochs.
         verbose_inside: Number of steps between verbose
             inside epoch or None.
+        verbose_bar: Show progress bar for each epoch
+            during batchwise training.
         apex: Use apex (lead to GPU memory leak among folds).
         pretrained_path: Path to the pretrained model weights.
         stop_by_metric: es and scheduler will stop by metric.
 
     """
 
     def __init__(
@@ -277,35 +280,42 @@
         metric: Callable,
         snap_params: Dict,
         is_snap: bool = False,
         sch: Optional[Any] = None,
         scheduler_params: Optional[Dict] = None,
         verbose: int = 1,
         verbose_inside: Optional[int] = None,
+        verbose_bar: bool = False,
         apex: bool = False,
         pretrained_path: Optional[str] = None,
         stop_by_metric: bool = False,
+        clip_grad: bool = False,
+        clip_grad_params: Optional[Dict] = None,
+        **kwargs
     ):
         self.net = net
         self.net_params = net_params
         self.opt = opt
         self.opt_params = opt_params
         self.n_epochs = n_epochs
         self.device = device
         self.device_ids = device_ids
         self.is_snap = is_snap
         self.snap_params = snap_params
         self.sch = sch
-        self.scheduler_params = scheduler_params
+        self.scheduler_params = scheduler_params if scheduler_params is not None else {}
         self.verbose = verbose
         self.metric = metric
         self.verbose_inside = verbose_inside
+        self.verbose_bar = verbose_bar
         self.apex = apex
         self.pretrained_path = pretrained_path
         self.stop_by_metric = stop_by_metric
+        self.clip_grad = clip_grad
+        self.clip_grad_params = clip_grad_params if clip_grad_params is not None else {}
 
         self.dataloader = None
         self.model = None
         self.optimizer = None
         self.scheduler = None
         self.se = None
         self.amp = None
@@ -422,48 +432,50 @@
         train_log = []
         for epoch in range(self.n_epochs):
             self.epoch = epoch
             # train
             train_loss = self.train(dataloaders=dataloaders)
             train_log.extend(train_loss)
             # test
-            val_loss, val_data = self.test(dataloader=dataloaders["val"])
+            val_loss, val_data, weights = self.test(dataloader=dataloaders["val"])
             if self.stop_by_metric:
-                cond = -1 * self.metric(*val_data)
+                cond = -1 * self.metric(*val_data, weights)
             else:
                 cond = np.mean(val_loss)
             self.se.update(self.model, cond)
 
             if self.sch is not None:
                 self.scheduler.step(cond)
 
             if (self.verbose is not None) and ((epoch + 1) % self.verbose == 0):
                 logger.info3(
                     "Epoch: {e}, train loss: {tl}, val loss: {vl}, val metric: {me}".format(
-                        me=self.metric(*val_data),
+                        me=self.metric(*val_data, weights),
                         e=self.epoch,
                         tl=np.mean(train_loss),
                         vl=np.mean(val_loss),
                     )
                 )
             if self.se.early_stop:
                 break
 
         self.se.set_best_params(self.model)
 
         if self.is_snap:
-            val_loss, val_data = self.test(dataloader=dataloaders["val"], snap=True, stage="val")
+            val_loss, val_data, weights = self.test(dataloader=dataloaders["val"], snap=True, stage="val")
             logger.info3(
-                "Result SE, val loss: {vl}, val metric: {me}".format(me=self.metric(*val_data), vl=np.mean(val_loss))
+                "Result SE, val loss: {vl}, val metric: {me}".format(
+                    me=self.metric(*val_data, weights), vl=np.mean(val_loss)
+                )
             )
-        elif self.se.early_stop:
-            val_loss, val_data = self.test(dataloader=dataloaders["val"])
+        elif self.se.swa:
+            val_loss, val_data, weights = self.test(dataloader=dataloaders["val"])
             logger.info3(
                 "Early stopping: val loss: {vl}, val metric: {me}".format(
-                    me=self.metric(*val_data), vl=np.mean(val_loss)
+                    me=self.metric(*val_data, weights), vl=np.mean(val_loss)
                 )
             )
 
         self.is_fitted = True
 
         return val_data[1]
 
@@ -477,16 +489,17 @@
             Loss.
 
         """
         loss_log = []
         self.model.train()
         running_loss = 0
         c = 0
-        logging_level = logger.getEffectiveLevel()
-        if logging_level <= logging.INFO and self.verbose:
+
+        logging_level = get_stdout_level()
+        if logging_level < logging.INFO and self.verbose and self.verbose_bar:
             loader = tqdm(dataloaders["train"], desc="train", disable=False)
         else:
             loader = dataloaders["train"]
 
         for sample in loader:
             data = {
                 i: (sample[i].long().to(self.device) if _dtypes_mapping[i] == "long" else sample[i].to(self.device))
@@ -495,39 +508,42 @@
 
             loss = self.model(data).mean()
             if self.apex:
                 with self.amp.scale_loss(loss, self.optimizer) as scaled_loss:
                     scaled_loss.backward()
             else:
                 loss.backward()
+
+            if self.clip_grad:
+                torch.nn.utils.clip_grad_norm_(self.model.parameters(), **self.clip_grad_params)
             self.optimizer.step()
             self.optimizer.zero_grad()
+
             loss = loss.data.cpu().numpy()
             loss_log.append(loss)
             running_loss += loss
 
             c += 1
-            if self.verbose_inside and logging_level <= logging.INFO:
-                if c % self.verbose_inside == 0:
-                    val_loss, val_data = self.test(dataloader=dataloaders["val"])
+            if self.verbose and self.verbose_bar and logging_level < logging.INFO:
+                if self.verbose_inside and c % self.verbose_inside == 0:
+                    val_loss, val_data, weights = self.test(dataloader=dataloaders["val"])
                     if self.stop_by_metric:
-                        cond = -1 * self.metric(*val_data)
+                        cond = -1 * self.metric(*val_data, weights)
                     else:
                         cond = np.mean(val_loss)
                     self.se.update(self.model, cond)
-                    if self.verbose is not None:
-                        logger.info3(
-                            "Epoch: {e}, iter: {c}, val loss: {vl}, val metric: {me}".format(
-                                me=self.metric(*val_data),
-                                e=self.epoch,
-                                c=c,
-                                vl=np.mean(val_loss),
-                            )
+
+                    logger.info3(
+                        "Epoch: {e}, iter: {c}, val loss: {vl}, val metric: {me}".format(
+                            me=self.metric(*val_data, weights),
+                            e=self.epoch,
+                            c=c,
+                            vl=np.mean(val_loss),
                         )
-            if logging_level <= logging.INFO and self.verbose:
+                    )
                 loader.set_description("train (loss=%g)" % (running_loss / c))
 
         return loss_log
 
     def test(
         self, dataloader: DataLoader, stage: str = "val", snap: bool = False
     ) -> Tuple[List[float], Tuple[np.ndarray, np.ndarray]]:
@@ -539,61 +555,70 @@
             snap: Use snapshots.
 
         Returns:
             Loss, (Target, OOF).
 
         """
         loss_log = []
+        weights_log = []
         self.model.eval()
         pred = []
         target = []
-        logging_level = logger.getEffectiveLevel()
-        if logging_level <= logging.INFO and self.verbose:
+        logging_level = get_stdout_level()
+        if logging_level < logging.INFO and self.verbose and self.verbose_bar:
             loader = tqdm(dataloader, desc=stage, disable=False)
         else:
             loader = dataloader
 
         with torch.no_grad():
             for sample in loader:
                 data = {
                     i: (sample[i].long().to(self.device) if _dtypes_mapping[i] == "long" else sample[i].to(self.device))
                     for i in sample.keys()
                 }
 
                 if snap:
                     output = self.se.predict(data)
-                    loss = self.se.forward(data)
+                    loss = self.se.forward(data) if stage != "test" else None
                 else:
                     output = self.model.predict(data)
-                    loss = self.model(data)
+                    loss = self.model(data) if stage != "test" else None
+
+                if stage != "test":
+                    loss = loss.mean().data.cpu().numpy()
 
-                loss = loss.mean().data.cpu().numpy()
                 loss_log.append(loss)
 
-                if self.model.n_out == 1:
-                    output = output.view(-1).data.cpu().numpy()
-                else:
-                    output = output.view(-1, self.model.n_out).data.cpu().numpy()
+                output = output.data.cpu().numpy()
+                target_data = data["label"].data.cpu().numpy()
+                weights = data.get("weight", None)
+                if weights is not None:
+                    weights = weights.data.cpu().numpy()
 
                 pred.append(output)
-                target.append(data["label"].view(-1).data.cpu().numpy())
+                target.append(target_data)
+                weights_log.extend(weights)
 
         self.model.train()
 
-        return loss_log, (
-            np.vstack(target) if len(target[0].shape) == 2 else np.hstack(target),
-            np.vstack(pred) if len(pred[0].shape) == 2 else np.hstack(pred),
+        return (
+            loss_log,
+            (
+                np.vstack(target) if len(target[0].shape) == 2 else np.hstack(target),
+                np.vstack(pred) if len(pred[0].shape) == 2 else np.hstack(pred),
+            ),
+            np.array(weights_log),
         )
 
     def predict(self, dataloader: DataLoader, stage: str) -> np.ndarray:
         """Predict model.
 
         Args:
             dataloader: Torch dataloader.
             stage: Train, val or test.
 
         Returns:
             Prediction.
 
         """
-        loss, (target, pred) = self.test(stage=stage, snap=self.is_snap, dataloader=dataloader)
+        loss, (target, pred), _ = self.test(stage=stage, snap=self.is_snap, dataloader=dataloader)
         return pred
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/text/utils.py` & `lightautoml-0.3.8b1/lightautoml/text/utils.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/text/weighted_average_transformer.py` & `lightautoml-0.3.8b1/lightautoml/text/weighted_average_transformer.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/transformers/base.py` & `lightautoml-0.3.8b1/lightautoml/transformers/base.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/transformers/categorical.py` & `lightautoml-0.3.8b1/lightautoml/transformers/categorical.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Union
 from typing import cast
 
 import numpy as np
 
 from pandas import DataFrame
 from pandas import Series
+from pandas import concat
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.utils.murmurhash import murmurhash3_32
 
 from ..dataset.base import LAMLDataset
 from ..dataset.np_pd_dataset import CSRSparseDataset
 from ..dataset.np_pd_dataset import NumpyDataset
 from ..dataset.np_pd_dataset import PandasDataset
@@ -1022,11 +1023,11 @@
                 flg_number = False
 
             if not flg_number:
                 co = role.unknown
                 cnts = subs[i].value_counts(dropna=True)
                 cnts = cnts[cnts > co].reset_index()
                 cnts = Series(cnts["index"].astype(str).rank().values, index=cnts["index"].values)
-                cnts = cnts.append(Series([cnts.shape[0] + 1], index=[np.nan]))
+                cnts = concat([cnts, Series([cnts.shape[0] + 1], index=[np.nan])])
                 self.dicts[i] = cnts
 
         return self
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/transformers/datetime.py` & `lightautoml-0.3.8b1/lightautoml/transformers/datetime.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/transformers/decomposition.py` & `lightautoml-0.3.8b1/lightautoml/transformers/decomposition.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/transformers/generator.py` & `lightautoml-0.3.8b1/lightautoml/transformers/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                         index=plain_id,
                     )
 
         # Define new tables' names
         # If in the main table contains two keys, there will be two additional tables with the keys and key to connect with major table.
         plain_i_id = dict()
         for unique_id in plain_unique_ids:
-            plain_i_id[unique_id] = f"plain_{plain_id}"
+            plain_i_id[unique_id] = f"plain_{unique_id}"
         # TODO: check unused variable 'plain_i_id_inv'
         # plain_i_id_inv = dict((v, k) for k, v in plain_i_id.items())
 
         # Update defined params for scheme
         for seq_table_name in self.seq_table_names:
             if self.seq_params[seq_table_name]["scheme"]["to"] == "plain":
                 self.seq_params[seq_table_name]["scheme"]["to"] = plain_i_id[
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/transformers/image.py` & `lightautoml-0.3.8b1/lightautoml/transformers/image.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/transformers/numeric.py` & `lightautoml-0.3.8b1/lightautoml/transformers/numeric.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Numeric features transformers."""
 
+from typing import Optional
 from typing import Union
 
 import numpy as np
 
+from sklearn.preprocessing import QuantileTransformer as SklQntTr
+
 from ..dataset.base import LAMLDataset
 from ..dataset.np_pd_dataset import NumpyDataset
 from ..dataset.np_pd_dataset import PandasDataset
 from ..dataset.roles import CategoryRole
 from ..dataset.roles import NumericRole
 from .base import LAMLTransformer
 
@@ -149,14 +152,69 @@
         # create resulted
         output = dataset.empty().to_numpy()
         output.set_data(data, self.features, NumericRole(np.float32))
 
         return output
 
 
+class FillnaMean(LAMLTransformer):
+    """Fillna with mean."""
+
+    _fit_checks = (numeric_check,)
+    _transform_checks = ()
+    _fname_prefix = "fillnamean"
+
+    def fit(self, dataset: NumpyTransformable):
+        """Estimate means.
+
+        Args:
+            dataset: Pandas or Numpy dataset of features.
+
+        Returns:
+            self.
+
+        """
+        # set transformer names and add checks
+        super().fit(dataset)
+        # set transformer features
+
+        # convert to accepted dtype and get attributes
+        dataset = dataset.to_numpy()
+        data = dataset.data
+
+        self.means = np.nanmean(data, axis=0)
+        self.means[np.isnan(self.means)] = 0
+
+        return self
+
+    def transform(self, dataset: NumpyTransformable) -> NumpyDataset:
+        """Transform - fillna with means.
+
+        Args:
+            dataset: Pandas or Numpy dataset of features.
+
+        Returns:
+            Numpy dataset with encoded labels.
+
+        """
+        # checks here
+        super().transform(dataset)
+        # convert to accepted dtype and get attributes
+        dataset = dataset.to_numpy()
+        data = dataset.data
+        # transform
+        data = np.where(np.isnan(data), self.means, data)
+
+        # create resulted
+        output = dataset.empty().to_numpy()
+        output.set_data(data, self.features, NumericRole(np.float32))
+
+        return output
+
+
 class FillInf(LAMLTransformer):
     """Fill inf with nan to handle as nan value."""
 
     _fit_checks = (numeric_check,)
     _transform_checks = ()
     _fname_prefix = "fillinf"
 
@@ -350,7 +408,96 @@
         new_data = np.where(sl, 0, new_data)
 
         # create resulted
         output = dataset.empty().to_numpy()
         output.set_data(new_data, self.features, CategoryRole(np.int32, label_encoded=True))
 
         return output
+
+
+class QuantileTransformer(LAMLTransformer):
+    """Transform features using quantiles information."""
+
+    _fit_checks = (numeric_check,)
+    _transform_checks = ()
+    _fname_prefix = "qntl_tr"
+    # TODO: Make normal docs
+
+    def __init__(
+        self,
+        n_quantiles: Optional[int] = None,
+        subsample: int = 1e9,
+        output_distribution: str = "normal",
+        noise: float = 1e-3,
+        qnt_factor: int = 30,
+    ):
+        """QuantileTransformer.
+
+        Args:
+            n_quantiles: Number of quantiles to be computed.
+            subsample: Maximum number of samples used to estimate the quantiles for computational efficiency.
+            output_distribution: Marginal distribution for the transformed data. The choices are 'uniform' or 'normal'.
+            noise: Add noise with certain std to dataset before quantile transformation to make data more smooth.
+            qnt_factor: If number of quantiles is none then it equals dataset size / factor
+        """
+        self.params = {
+            "n_quantiles": n_quantiles,
+            "subsample": subsample,
+            "copy": False,
+            "output_distribution": output_distribution,
+            "noise": noise,
+        }
+        self.qnt_factor = qnt_factor
+        self.transformer = None
+
+    def fit(self, dataset: NumpyTransformable):
+        """Fit Sklearn QuantileTransformer.
+
+        Args:
+            dataset: Pandas or Numpy dataset of numeric features.
+
+        Returns:
+            self.
+
+        """
+        for check_func in self._fit_checks:
+            check_func(dataset)
+
+        np_dataset = dataset.to_numpy().data
+        if self.params["noise"] is not None:
+            stds = np.std(np_dataset, axis=0, keepdims=True)
+            noise_std = self.params["noise"] / np.maximum(stds, self.params["noise"])
+            np_dataset += noise_std * np.random.randn(*np_dataset.shape)
+
+        if self.params["n_quantiles"] is None:
+            self.params["n_quantiles"] = max(min(np_dataset.shape[0] // self.qnt_factor, 1000), 10)
+
+        skl_params = self.params
+        del skl_params["noise"]
+        self.transformer = SklQntTr(**skl_params)
+        self.transformer.fit(np_dataset)
+        self._features = dataset.features
+        return self
+
+    def transform(self, dataset: NumpyTransformable) -> NumpyDataset:
+        """Apply transformer.
+
+        Args:
+            dataset: Pandas or Numpy dataset of numeric features.
+
+        Returns:
+            Numpy dataset with encoded labels.
+
+        """
+        # checks here
+        super().transform(dataset)
+        # convert to accepted dtype and get attributes
+        dataset = dataset.to_numpy()
+
+        # transform
+        new_arr = self.transformer.transform(dataset.data)
+
+        # create resulted
+        output = dataset.empty().to_numpy()
+        output.set_data(new_arr, self.features, NumericRole(np.float32))
+
+        return output
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/transformers/text.py` & `lightautoml-0.3.8b1/lightautoml/transformers/text.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/utils/installation.py` & `lightautoml-0.3.8b1/lightautoml/utils/installation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Tools for partial installation."""
 
+import os
+
+
 try:
     from importlib.metadata import PackageNotFoundError
     from importlib.metadata import distribution
 except ModuleNotFoundError:
     from importlib_metadata import PackageNotFoundError, distribution
 
 import logging
@@ -16,14 +19,16 @@
     """Check if extra dependecies is installed.
 
     Args:
         extra_section: Name of extra dependecies
         error: How to process error
 
     """
+    ignore_deps = os.environ.get("DOCUMENTATION_ENV", False)
+
     md = distribution("lightautoml").metadata
     extra_pattern = 'extra == "{}"'.format(extra_section)
     reqs_info = []
     for k, v in md.items():
         if k == "Requires-Dist" and extra_pattern in v:
             req = v.split(";")[0].split()[0]
             reqs_info.append(req)
@@ -37,9 +42,10 @@
             logger.warning(
                 "'%s' extra dependecy package '%s' isn't installed. "
                 "Look at README.md in repo 'LightAutoML' for installation instructions.",
                 extra_section,
                 lib_name,
             )
 
-            if error:
-                raise e
+            if not ignore_deps:
+                if error:
+                    raise e
```

### Comparing `LightAutoML-0.3.7.3/lightautoml/utils/logging.py` & `lightautoml-0.3.8b1/lightautoml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/utils/timer.py` & `lightautoml-0.3.8b1/lightautoml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/validation/base.py` & `lightautoml-0.3.8b1/lightautoml/validation/base.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/validation/np_iterators.py` & `lightautoml-0.3.8b1/lightautoml/validation/np_iterators.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/lightautoml/validation/utils.py` & `lightautoml-0.3.8b1/lightautoml/validation/utils.py`

 * *Files identical despite different names*

### Comparing `LightAutoML-0.3.7.3/pyproject.toml` & `lightautoml-0.3.8b1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LightAutoML"
-version = "0.3.7.3"
+version = "0.3.8-b1"
 description = "Fast and customizable framework for automatic ML model creation (AutoML)"
 authors = [
     "Alexander Ryzhkov <alexmryzhkov@gmail.com>",
     "Anton Vakhrushev <btbpanda@gmail.com>",
     "Dmitrii Simakov <dmitryevsimakov@gmail.com>",
     "Rinchin Damdinov <damdinovr@gmail.com>",
     "Alexander Kirilin <adkirilin@gmail.com>",
@@ -15,52 +15,56 @@
 homepage = "https://lightautoml.readthedocs.io/en/latest/"
 repository = "https://github.com/AILab-MLTools/LightAutoML"
 classifiers = [
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Natural Language :: English",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Typing :: Typed"
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.6.1, <3.10"
+python = ">=3.6.1, <3.11"
 
-poetry-core = "^1.0.0"
+poetry-core = [
+    {version = ">=1.0.0", python = "<3.7"},
+    {version = "^1.0.0", python = "^3.7"}
+]
 pandas = [
   {version = "<=1.1.5", python = ">=3.6.1, <3.7.1"},
   {version = "<=1.3.5", python = ">=3.7.1, <3.8"},
   {version = "<=1.4.3", python = ">=3.8"}
 ]
+numpy = "<1.24.0"
 scikit-learn = ">=0.22"
 lightgbm = ">=2.3, <=3.2.1"
 catboost = ">=0.26.1"
 optuna = "*"
 torch = [
     {platform = "win32", python = "3.6.1", version = "1.7.0"},
-    {platform = "*", version = "<1.9"}
+    {version = ">=1.0.0"}
 ]
 dataclasses = {version = "0.6", python = "<3.7"}
 holidays = "*"
+statsmodels = "<=0.14.0"
 networkx = "*"
 cmaes = "*"
 pyyaml = "*"
 tqdm = "*"
-joblib = "*"
-importlib-metadata = {version = "^1.0", python = "<3.8"}
-
+joblib = "<1.3.0"
+importlib-metadata = {version = ">=1.0", python = "<3.8"}
 autowoe = ">=1.2"
-
 jinja2 = "*"
 json2html = "*"
 seaborn = "*"
 
 # NLP
 gensim = {version = ">=4", optional = true}
 nltk = {version = "*", optional = true}
@@ -80,41 +84,14 @@
 featuretools = {version = ">=1.11.1", python = ">=3.7", optional = true}
 
 # Report (pdf)
 weasyprint = {version = "52.5", optional = true}
 cffi = {version = "1.14.5", optional = true}
 
 
-[tool.poetry.dev-dependencies]
-pytest = "6.2.5"
-sphinx = "4.3.2"
-sphinx-autodoc-typehints = "1.12.0"
-sphinx-rtd-theme = "1.0.0"
-ipython = [
-    {version = "<7.0.0", python = "<3.8"},
-    {version = "8.5.0", python = ">=3.8"}
-]
-ipywidgets = "7.7.1"
-nbsphinx = "0.8.8"
-nbsphinx-link = "1.3.0"
-pandoc = "2.0.1"
-pre-commit = "2.15.0"
-notebook = "6.4.7"
-mypy = "0.910"
-tox = "3.24.4"
-darglint = "1.8.1"
-black = "20.8b1"
-flake8-docstrings = "1.6.0"
-isort = "5.7.0"
-jupyter-contrib-nbextensions = "0.5.1"
-flake8 = "4.0.1"
-doc8 = "0.10.1"
-rstcheck = "3.3.1"
-
-
 [tool.poetry.extras]
 cv = [
     "albumentations",
     "efficientnet-pytorch",
     "opencv-python",
     "PyWavelets",
     "scikit-image",
@@ -169,43 +146,107 @@
   | buck-out
   | build
   | dist
   | tests/.*/setup.py
 )/
 '''
 
-
 [tool.isort]
 profile = "black"
 force_single_line = true
 atomic = true
 include_trailing_comma = true
 lines_after_imports = 2
 lines_between_types = 1
 use_parentheses = true
 filter_files = true
 
 
 [tool.tox]
 legacy_tox_ini = """
-[tox]
-isolated_build = True
-envlist = py{36, 37, 38, 39}
-
-[gh-actions]
-python =
-    3.6: py36
-    3.7: py37
-    3.8: py38
-    3.9: py39
-
-[gh-actions:env]
-PLATFORM =
-    ubuntu-latest: linux
-    macos-latest: macos
-    windows-latest: windows
-
-[testenv]
-whitelist_externals = poetry
-commands =
-    poetry run pytest tests -v
+    [tox]
+    min_version = 4.0
+    isolated_build = True
+    envlist =
+        py{36, 37, 38, 39, 310},
+        lint,
+        docs,
+        typing,
+        jupyter,
+        experiment_tracking,
+        build
+
+    [tox:.package]
+    # note tox will use the same python version as under what tox is installed to package
+    # so unless this is python 3 you can require a given python version for the packaging
+    # environment via the basepython key
+    basepython = python3
+
+    [gh-actions]
+    python =
+        3.6: py36
+        3.7: py37
+        3.8: py38
+        3.9: py39
+        3.10: py310
+
+    [gh-actions:env]
+    PLATFORM =
+        ubuntu-latest: linux
+        macos-latest: macos
+        windows-latest: windows
+
+    [testenv]
+    package = wheel
+    deps =
+        .[all]
+        pytest >= 6.2.5
+    commands = pytest {posargs} -v --basetemp="{envtmpdir}"
+
+    [testenv:lint]
+    deps =
+        pre-commit == 2.15.0
+    commands = pre-commit run --all-files
+
+    [testenv:docs]
+    requires = python >= 3.8
+    changedir = docs
+    deps =
+        poetry >= 1.1.7
+        sphinx == 5.3.0 # extras = ["autdoc", "autosummary", "intersphinx", "napoleon", "viewcode"]
+        sphinx-autodoc-typehints >=1.19.5
+        sphinx-rtd-theme >=1.1.1
+        nbsphinx == 0.8.10
+        nbsphinx-link == 1.3.0
+        doc8 == 0.10.1
+        rstcheck == 3.3.1
+        pandoc == 2.0.1
+    commands =
+        poetry run make clean html
+        poetry run python ../check_docs.py
+
+    [testenv:typing]
+    description = run type checks
+    deps =
+        mypy >= 0.991
+    commands =
+        mypy {posargs:src tests}
+
+    [testenv:experiment_tracking]
+    deps = clearml
+    commands = sh experiments/run_bench_release.sh {posargs}
+
+    [testenv:jupyter]
+    requires = python >= 3.8
+    deps =
+        ipython >=3.8
+        ipywidgets == 7.7.1
+        notebook == 6.4.10
+        jupyter-contrib-nbextensions == 0.5.1
+
+    [testenv:build]
+    deps =
+        poetry >= 1.1.7
+    commands =
+        poetry run python scripts/poetry_fix.py -f
+        poetry build
 """
```

### Comparing `LightAutoML-0.3.7.3/setup.py` & `lightautoml-0.3.8b1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['lightautoml',
  'lightautoml.addons',
  'lightautoml.addons.autots',
+ 'lightautoml.addons.hypex',
+ 'lightautoml.addons.hypex.algorithms',
+ 'lightautoml.addons.hypex.selectors',
+ 'lightautoml.addons.hypex.utils',
  'lightautoml.addons.interpretation',
  'lightautoml.addons.uplift',
  'lightautoml.addons.utilization',
  'lightautoml.automl',
  'lightautoml.automl.presets',
  'lightautoml.dataset',
  'lightautoml.image',
@@ -35,67 +39,73 @@
 
 install_requires = \
 ['autowoe>=1.2',
  'catboost>=0.26.1',
  'cmaes',
  'holidays',
  'jinja2',
- 'joblib',
+ 'joblib<1.3.0',
  'json2html',
  'lightgbm>=2.3,<=3.2.1',
  'networkx',
+ 'numpy<1.24.0',
  'optuna',
- 'poetry-core>=1.0.0,<2.0.0',
  'pyyaml',
  'scikit-learn>=0.22',
  'seaborn',
- 'torch<1.9',
+ 'statsmodels<=0.14.0',
+ 'torch>=1.0.0',
  'tqdm']
 
 extras_require = \
 {':python_full_version == "3.6.1" and sys_platform == "win32"': ['torch==1.7.0'],
  ':python_full_version >= "3.6.1" and python_full_version < "3.7.1"': ['pandas<=1.1.5'],
  ':python_full_version >= "3.7.1" and python_version < "3.8"': ['pandas<=1.3.5'],
- ':python_version < "3.7"': ['dataclasses==0.6'],
- ':python_version < "3.8"': ['importlib-metadata>=1.0,<2.0'],
+ ':python_version < "3.7"': ['poetry-core>=1.0.0', 'dataclasses==0.6'],
+ ':python_version < "3.8"': ['importlib-metadata>=1.0'],
+ ':python_version >= "3.7" and python_version < "4.0"': ['poetry-core>=1.0.0,<2.0.0'],
  ':python_version >= "3.8"': ['pandas<=1.4.3'],
  'afg:python_version >= "3.7"': ['featuretools>=1.11.1'],
  'all': ['gensim>=4',
          'nltk',
          'transformers>=4',
          'albumentations<=1.0.3',
          'efficientnet-pytorch',
          'opencv-python<=4.5.2.52',
          'PyWavelets',
          'torchvision',
+         'torchvision',
          'weasyprint==52.5',
          'cffi==1.14.5'],
- 'all:python_full_version == "3.6.1" and sys_platform == "win32"': ['torchvision==0.8.0'],
+ 'all:python_full_version == "3.6.1" and sys_platform == "win32"': ['torchvision==0.8.0',
+                                                                    'torchvision==0.8.0'],
  'all:python_version >= "3.7"': ['featuretools>=1.11.1'],
  'cv': ['albumentations<=1.0.3',
         'efficientnet-pytorch',
         'opencv-python<=4.5.2.52',
         'PyWavelets',
+        'torchvision',
         'torchvision'],
- 'cv:python_full_version == "3.6.1" and sys_platform == "win32"': ['torchvision==0.8.0'],
+ 'cv:python_full_version == "3.6.1" and sys_platform == "win32"': ['torchvision==0.8.0',
+                                                                   'torchvision==0.8.0'],
  'nlp': ['gensim>=4', 'nltk', 'transformers>=4'],
  'report': ['weasyprint==52.5', 'cffi==1.14.5']}
 
 setup_kwargs = {
     'name': 'lightautoml',
-    'version': '0.3.7.3',
+    'version': '0.3.8b1',
     'description': 'Fast and customizable framework for automatic ML model creation (AutoML)',
-    'long_description': '<img src=https://github.com/AILab-MLTools/LightAutoML/raw/master/imgs/LightAutoML_logo_big.png />\n\n# LightAutoML - automatic model creation framework\n\n[![Telegram](https://img.shields.io/badge/chat-on%20Telegram-2ba2d9.svg)](https://t.me/lightautoml)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/lightautoml?color=green&label=PyPI%20downloads&logo=pypi&logoColor=orange&style=plastic)\n![Read the Docs](https://img.shields.io/readthedocs/lightautoml?style=plastic)\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nLightAutoML (LAMA) is an AutoML framework which provides automatic model creation for the following tasks:\n- binary classification\n- multiclass  classification\n- regression\n\nCurrent version of the package handles datasets that have independent samples in each row. I.e. **each row is an object with its specific features and target**.\nMultitable datasets and sequences are a work in progress :)\n\n**Note**: we use [`AutoWoE`](https://pypi.org/project/autowoe) library to automatically create interpretable models.\n\n**Authors**: [Alexander Ryzhkov](https://kaggle.com/alexryzhkov), [Anton Vakhrushev](https://kaggle.com/btbpanda), [Dmitry Simakov](https://kaggle.com/simakov), Vasilii Bunakov, Rinchin Damdinov, Alexander Kirilin, Pavel Shvets.\n\n**Documentation** of LightAutoML is available [here](https://lightautoml.readthedocs.io/), you can also [generate](https://github.com/AILab-MLTools/LightAutoML/blob/master/.github/CONTRIBUTING.md#building-documentation) it.\n\n# (New features) GPU and Spark pipelines\nFull GPU and Spark pipelines for LightAutoML currently available for developers testing (still in progress). The code and tutorials for:\n- GPU pipeline is [available here](https://github.com/Rishat-skoltech/LightAutoML_GPU)\n- Spark pipeline is [available here](https://github.com/sb-ai-lab/SLAMA)\n\n<a name="toc"></a>\n# Table of Contents\n\n* [Installation LightAutoML from PyPI](#installation)\n* [Quick tour](#quicktour)\n* [Resources](#examples)\n* [Contributing to LightAutoML](#contributing)\n* [License](#apache)\n* [For developers](#developers)\n* [Support and feature requests](#support)\n\n<a name="installation"></a>\n# Installation\nTo install LAMA framework on your machine from PyPI, execute following commands:\n```bash\n\n# Install base functionality:\n\npip install -U lightautoml\n\n# For partial installation use corresponding option.\n# Extra dependecies: [nlp, cv, report]\n# Or you can use \'all\' to install everything\n\npip install -U lightautoml[nlp]\n\n```\n\nAdditionaly, run following commands to enable pdf report generation:\n\n```bash\n# MacOS\nbrew install cairo pango gdk-pixbuf libffi\n\n# Debian / Ubuntu\nsudo apt-get install build-essential libcairo2 libpango-1.0-0 libpangocairo-1.0-0 libgdk-pixbuf2.0-0 libffi-dev shared-mime-info\n\n# Fedora\nsudo yum install redhat-rpm-config libffi-devel cairo pango gdk-pixbuf2\n\n# Windows\n# follow this tutorial https://weasyprint.readthedocs.io/en/stable/install.html#windows\n```\n[Back to top](#toc)\n\n<a name="quicktour"></a>\n# Quick tour\n\nLet\'s solve the popular Kaggle Titanic competition below. There are two main ways to solve machine learning problems using LightAutoML:\n* Use ready preset for tabular data:\n```python\nimport pandas as pd\nfrom sklearn.metrics import f1_score\n\nfrom lightautoml.automl.presets.tabular_presets import TabularAutoML\nfrom lightautoml.tasks import Task\n\ndf_train = pd.read_csv(\'../input/titanic/train.csv\')\ndf_test = pd.read_csv(\'../input/titanic/test.csv\')\n\nautoml = TabularAutoML(\n    task = Task(\n        name = \'binary\',\n        metric = lambda y_true, y_pred: f1_score(y_true, (y_pred > 0.5)*1))\n)\noof_pred = automl.fit_predict(\n    df_train,\n    roles = {\'target\': \'Survived\', \'drop\': [\'PassengerId\']}\n)\ntest_pred = automl.predict(df_test)\n\npd.DataFrame({\n    \'PassengerId\':df_test.PassengerId,\n    \'Survived\': (test_pred.data[:, 0] > 0.5)*1\n}).to_csv(\'submit.csv\', index = False)\n```\n\nLighAutoML framework has a lot of ready-to-use parts and extensive customization options, to learn more check out the [resources](#Resources) section.\n\n[Back to top](#toc)\n\n<a name="examples"></a>\n# Resources\n\n### Kaggle kernel examples of LightAutoML usage:\n\n- [Tabular Playground Series April 2021 competition solution](https://www.kaggle.com/alexryzhkov/n3-tps-april-21-lightautoml-starter)\n- [Titanic competition solution (80% accuracy)](https://www.kaggle.com/alexryzhkov/lightautoml-titanic-love)\n- [Titanic **12-code-lines** competition solution (78% accuracy)](https://www.kaggle.com/alexryzhkov/lightautoml-extreme-short-titanic-solution)\n- [House prices competition solution](https://www.kaggle.com/alexryzhkov/lightautoml-houseprices-love)\n- [Natural Language Processing with Disaster Tweets solution](https://www.kaggle.com/alexryzhkov/lightautoml-starter-nlp)\n- [Tabular Playground Series March 2021 competition solution](https://www.kaggle.com/alexryzhkov/lightautoml-starter-for-tabulardatamarch)\n- [Tabular Playground Series February 2021 competition solution](https://www.kaggle.com/alexryzhkov/lightautoml-tabulardata-love)\n- [Interpretable WhiteBox solution](https://www.kaggle.com/simakov/lama-whitebox-preset-example)\n- [Custom ML pipeline elements inside existing ones](https://www.kaggle.com/simakov/lama-custom-automl-pipeline-example)\n\n### Google Colab tutorials and [other examples](examples/):\n\n- [`Tutorial_1_basics.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_1_basics.ipynb) - get started with LightAutoML on tabular data.\n- [`Tutorial_2_WhiteBox_AutoWoE.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_2_WhiteBox_AutoWoE.ipynb) - creating interpretable models.\n- [`Tutorial_3_sql_data_source.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_3_sql_data_source.ipynb) - shows how to use LightAutoML presets (both standalone and time utilized variants) for solving ML tasks on tabular data from SQL data base instead of CSV.\n- [`Tutorial_4_NLP_Interpretation.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_4_NLP_Interpretation.ipynb) - example of using TabularNLPAutoML preset, LimeTextExplainer.\n- [`Tutorial_5_uplift.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_5_uplift.ipynb) - shows how to use LightAutoML for a uplift-modeling task.\n- [`Tutorial_6_custom_pipeline.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_6_custom_pipeline.ipynb) - shows how to create your own pipeline from specified blocks: pipelines for feature generation and feature selection, ML algorithms, hyperparameter optimization etc.\n- [`Tutorial_7_ICE_and_PDP_interpretation.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_7_ICE_and_PDP_interpretation.ipynb) - shows how to obtain local and global interpretation of model results using ICE and PDP approaches.\n- [`Tutorial_8_CV_preset.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_8_CV_preset.ipynb) - example of using TabularCVAutoML preset in CV multi-class classification task.\n\n\n**Note 1**: for production you have no need to use profiler (which increase work time and memory consomption), so please do not turn it on - it is in off state by default\n\n**Note 2**: to take a look at this report after the run, please comment last line of demo with report deletion command.\n\n### Courses, videos and papers\n\n* **LightAutoML crash courses**:\n    - (Russian) [AutoML course for OpenDataScience community](https://ods.ai/tracks/automl-course-part1)\n\n* **Video guides**:\n    - (Russian) [LightAutoML webinar for Sberloga community](https://www.youtube.com/watch?v=ci8uqgWFJGg) ([Alexander Ryzhkov](https://kaggle.com/alexryzhkov), [Dmitry Simakov](https://kaggle.com/simakov))\n    - (Russian) [LightAutoML hands-on tutorial in Kaggle Kernels](https://www.youtube.com/watch?v=TYu1UG-E9e8) ([Alexander Ryzhkov](https://kaggle.com/alexryzhkov))\n    - (English) [Automated Machine Learning with LightAutoML: theory and practice](https://www.youtube.com/watch?v=4pbO673B9Oo) ([Alexander Ryzhkov](https://kaggle.com/alexryzhkov))\n    - (English) [LightAutoML framework general overview, benchmarks and advantages for business](https://vimeo.com/485383651) ([Alexander Ryzhkov](https://kaggle.com/alexryzhkov))\n    - (English) [LightAutoML practical guide - ML pipeline presets overview](https://vimeo.com/487166940) ([Dmitry Simakov](https://kaggle.com/simakov))\n\n* **Papers**:\n    - Anton Vakhrushev, Alexander Ryzhkov, Dmitry Simakov, Rinchin Damdinov, Maxim Savchenko, Alexander Tuzhilin ["LightAutoML: AutoML Solution for a Large Financial Services Ecosystem"](https://arxiv.org/pdf/2109.01528.pdf). arXiv:2109.01528, 2021.\n\n* **Articles about LightAutoML**:\n    - (English) [LightAutoML vs Titanic: 80% accuracy in several lines of code (Medium)](https://alexmryzhkov.medium.com/lightautoml-preset-usage-tutorial-2cce7da6f936)\n    - (English) [Hands-On Python Guide to LightAutoML – An Automatic ML Model Creation Framework (Analytic Indian Mag)](https://analyticsindiamag.com/hands-on-python-guide-to-lama-an-automatic-ml-model-creation-framework/?fbclid=IwAR0f0cVgQWaLI60m1IHMD6VZfmKce0ZXxw-O8VRTdRALsKtty8a-ouJex7g)\n\n[Back to top](#toc)\n\n<a name="contributing"></a>\n# Contributing to LightAutoML\nIf you are interested in contributing to LightAutoML, please read the [Contributing Guide](.github/CONTRIBUTING.md) to get started.\n\n[Back to top](#toc)\n\n<a name="apache"></a>\n# License\nThis project is licensed under the Apache License, Version 2.0. See [LICENSE](https://github.com/AILab-MLTools/LightAutoML/blob/master/LICENSE) file for more details.\n\n[Back to top](#toc)\n\n<a name="developers"></a>\n# For developers\n\n## Build your own custom pipeline:\n\n```python\nimport pandas as pd\nfrom sklearn.metrics import f1_score\n\nfrom lightautoml.automl.presets.tabular_presets import TabularAutoML\nfrom lightautoml.tasks import Task\n\ndf_train = pd.read_csv(\'../input/titanic/train.csv\')\ndf_test = pd.read_csv(\'../input/titanic/test.csv\')\n\n# define that machine learning problem is binary classification\ntask = Task("binary")\n\nreader = PandasToPandasReader(task, cv=N_FOLDS, random_state=RANDOM_STATE)\n\n# create a feature selector\nmodel0 = BoostLGBM(\n    default_params={\'learning_rate\': 0.05, \'num_leaves\': 64,\n    \'seed\': 42, \'num_threads\': N_THREADS}\n)\npipe0 = LGBSimpleFeatures()\nmbie = ModelBasedImportanceEstimator()\nselector = ImportanceCutoffSelector(pipe0, model0, mbie, cutoff=0)\n\n# build first level pipeline for AutoML\npipe = LGBSimpleFeatures()\n# stop after 20 iterations or after 30 seconds\nparams_tuner1 = OptunaTuner(n_trials=20, timeout=30)\nmodel1 = BoostLGBM(\n    default_params={\'learning_rate\': 0.05, \'num_leaves\': 128,\n    \'seed\': 1, \'num_threads\': N_THREADS}\n)\nmodel2 = BoostLGBM(\n    default_params={\'learning_rate\': 0.025, \'num_leaves\': 64,\n    \'seed\': 2, \'num_threads\': N_THREADS}\n)\npipeline_lvl1 = MLPipeline([\n    (model1, params_tuner1),\n    model2\n], pre_selection=selector, features_pipeline=pipe, post_selection=None)\n\n# build second level pipeline for AutoML\npipe1 = LGBSimpleFeatures()\nmodel = BoostLGBM(\n    default_params={\'learning_rate\': 0.05, \'num_leaves\': 64,\n    \'max_bin\': 1024, \'seed\': 3, \'num_threads\': N_THREADS},\n    freeze_defaults=True\n)\npipeline_lvl2 = MLPipeline([model], pre_selection=None, features_pipeline=pipe1,\n post_selection=None)\n\n# build AutoML pipeline\nautoml = AutoML(reader, [\n    [pipeline_lvl1],\n    [pipeline_lvl2],\n], skip_conn=False)\n\n# train AutoML and get predictions\noof_pred = automl.fit_predict(df_train, roles = {\'target\': \'Survived\', \'drop\': [\'PassengerId\']})\ntest_pred = automl.predict(df_test)\n\npd.DataFrame({\n    \'PassengerId\':df_test.PassengerId,\n    \'Survived\': (test_pred.data[:, 0] > 0.5)*1\n}).to_csv(\'submit.csv\', index = False)\n```\n\n[Back to top](#toc)\n\n<a name="support"></a>\n# Support and feature requests\nSeek prompt advice at [Telegram group](https://t.me/lightautoml).\n\nOpen bug reports and feature requests on GitHub [issues](https://github.com/AILab-MLTools/LightAutoML/issues).\n',
+    'long_description': '<img src=https://github.com/AILab-MLTools/LightAutoML/raw/master/imgs/LightAutoML_logo_big.png />\n\n# LightAutoML - automatic model creation framework\n\n[![Telegram](https://img.shields.io/badge/chat-on%20Telegram-2ba2d9.svg)](https://t.me/lightautoml)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/lightautoml?color=green&label=PyPI%20downloads&logo=pypi&logoColor=orange&style=plastic)\n![Read the Docs](https://img.shields.io/readthedocs/lightautoml?style=plastic)\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![Poetry-Lock](https://img.shields.io/github/workflow/status/sb-ai-lab/LightAutoML/Poetry%20run/master?label=Poetry-Lock)\n\n\nLightAutoML (LAMA) is an AutoML framework which provides automatic model creation for the following tasks:\n- binary classification\n- multiclass  classification\n- regression\n\nCurrent version of the package handles datasets that have independent samples in each row. I.e. **each row is an object with its specific features and target**.\nMultitable datasets and sequences are a work in progress :)\n\n**Note**: we use [`AutoWoE`](https://pypi.org/project/autowoe) library to automatically create interpretable models.\n\n**Authors**: [Alexander Ryzhkov](https://kaggle.com/alexryzhkov), [Anton Vakhrushev](https://kaggle.com/btbpanda), [Dmitry Simakov](https://kaggle.com/simakov), Vasilii Bunakov, Rinchin Damdinov, Alexander Kirilin, Pavel Shvets.\n\n**Documentation** of LightAutoML is available [here](https://lightautoml.readthedocs.io/), you can also [generate](https://github.com/AILab-MLTools/LightAutoML/blob/master/.github/CONTRIBUTING.md#building-documentation) it.\n\n# (New features) GPU and Spark pipelines\nFull GPU and Spark pipelines for LightAutoML currently available for developers testing (still in progress). The code and tutorials for:\n- GPU pipeline is [available here](https://github.com/Rishat-skoltech/LightAutoML_GPU)\n- Spark pipeline is [available here](https://github.com/sb-ai-lab/SLAMA)\n\n<a name="toc"></a>\n# Table of Contents\n\n* [Installation LightAutoML from PyPI](#installation)\n* [Quick tour](#quicktour)\n* [Resources](#examples)\n* [Contributing to LightAutoML](#contributing)\n* [License](#apache)\n* [For developers](#developers)\n* [Support and feature requests](#support)\n\n<a name="installation"></a>\n# Installation\nTo install LAMA framework on your machine from PyPI, execute following commands:\n```bash\n\n# Install base functionality:\n\npip install -U lightautoml\n\n# For partial installation use corresponding option.\n# Extra dependecies: [nlp, cv, report]\n# Or you can use \'all\' to install everything\n\npip install -U lightautoml[nlp]\n\n```\n\nAdditionaly, run following commands to enable pdf report generation:\n\n```bash\n# MacOS\nbrew install cairo pango gdk-pixbuf libffi\n\n# Debian / Ubuntu\nsudo apt-get install build-essential libcairo2 libpango-1.0-0 libpangocairo-1.0-0 libgdk-pixbuf2.0-0 libffi-dev shared-mime-info\n\n# Fedora\nsudo yum install redhat-rpm-config libffi-devel cairo pango gdk-pixbuf2\n\n# Windows\n# follow this tutorial https://weasyprint.readthedocs.io/en/stable/install.html#windows\n```\n[Back to top](#toc)\n\n<a name="quicktour"></a>\n# Quick tour\n\nLet\'s solve the popular Kaggle Titanic competition below. There are two main ways to solve machine learning problems using LightAutoML:\n* Use ready preset for tabular data:\n```python\nimport pandas as pd\nfrom sklearn.metrics import f1_score\n\nfrom lightautoml.automl.presets.tabular_presets import TabularAutoML\nfrom lightautoml.tasks import Task\n\ndf_train = pd.read_csv(\'../input/titanic/train.csv\')\ndf_test = pd.read_csv(\'../input/titanic/test.csv\')\n\nautoml = TabularAutoML(\n    task = Task(\n        name = \'binary\',\n        metric = lambda y_true, y_pred: f1_score(y_true, (y_pred > 0.5)*1))\n)\noof_pred = automl.fit_predict(\n    df_train,\n    roles = {\'target\': \'Survived\', \'drop\': [\'PassengerId\']}\n)\ntest_pred = automl.predict(df_test)\n\npd.DataFrame({\n    \'PassengerId\':df_test.PassengerId,\n    \'Survived\': (test_pred.data[:, 0] > 0.5)*1\n}).to_csv(\'submit.csv\', index = False)\n```\n\nLighAutoML framework has a lot of ready-to-use parts and extensive customization options, to learn more check out the [resources](#Resources) section.\n\n[Back to top](#toc)\n\n<a name="examples"></a>\n# Resources\n\n### Kaggle kernel examples of LightAutoML usage:\n\n- [Tabular Playground Series April 2021 competition solution](https://www.kaggle.com/alexryzhkov/n3-tps-april-21-lightautoml-starter)\n- [Titanic competition solution (80% accuracy)](https://www.kaggle.com/alexryzhkov/lightautoml-titanic-love)\n- [Titanic **12-code-lines** competition solution (78% accuracy)](https://www.kaggle.com/alexryzhkov/lightautoml-extreme-short-titanic-solution)\n- [House prices competition solution](https://www.kaggle.com/alexryzhkov/lightautoml-houseprices-love)\n- [Natural Language Processing with Disaster Tweets solution](https://www.kaggle.com/alexryzhkov/lightautoml-starter-nlp)\n- [Tabular Playground Series March 2021 competition solution](https://www.kaggle.com/alexryzhkov/lightautoml-starter-for-tabulardatamarch)\n- [Tabular Playground Series February 2021 competition solution](https://www.kaggle.com/alexryzhkov/lightautoml-tabulardata-love)\n- [Interpretable WhiteBox solution](https://www.kaggle.com/simakov/lama-whitebox-preset-example)\n- [Custom ML pipeline elements inside existing ones](https://www.kaggle.com/simakov/lama-custom-automl-pipeline-example)\n- [Custom ML pipeline elements inside existing ones](https://www.kaggle.com/simakov/lama-custom-automl-pipeline-example)\n- [Tabular Playground Series November 2022 competition solution with Neural Networks](https://www.kaggle.com/code/mikhailkuz/lightautoml-nn-happiness)\n\n### Google Colab tutorials and [other examples](examples/):\n\n- [`Tutorial_1_basics.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_1_basics.ipynb) - get started with LightAutoML on tabular data.\n- [`Tutorial_2_WhiteBox_AutoWoE.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_2_WhiteBox_AutoWoE.ipynb) - creating interpretable models.\n- [`Tutorial_3_sql_data_source.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_3_sql_data_source.ipynb) - shows how to use LightAutoML presets (both standalone and time utilized variants) for solving ML tasks on tabular data from SQL data base instead of CSV.\n- [`Tutorial_4_NLP_Interpretation.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_4_NLP_Interpretation.ipynb) - example of using TabularNLPAutoML preset, LimeTextExplainer.\n- [`Tutorial_5_uplift.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_5_uplift.ipynb) - shows how to use LightAutoML for a uplift-modeling task.\n- [`Tutorial_6_custom_pipeline.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_6_custom_pipeline.ipynb) - shows how to create your own pipeline from specified blocks: pipelines for feature generation and feature selection, ML algorithms, hyperparameter optimization etc.\n- [`Tutorial_7_ICE_and_PDP_interpretation.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_7_ICE_and_PDP_interpretation.ipynb) - shows how to obtain local and global interpretation of model results using ICE and PDP approaches.\n- [`Tutorial_8_CV_preset.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_8_CV_preset.ipynb) - example of using TabularCVAutoML preset in CV multi-class classification task.\n- [`Tutorial_9_neural_networks.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_9_neural_networks.ipynb) - example of using Tabular preset with neural networks.\n- [`Tutorial_10_relational_data_with_star_scheme.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_10_relational_data_with_star_scheme.ipynb) - example of using Tabular preset with neural networks.\n\n**Note 1**: for production you have no need to use profiler (which increase work time and memory consomption), so please do not turn it on - it is in off state by default\n\n**Note 2**: to take a look at this report after the run, please comment last line of demo with report deletion command.\n\n### Courses, videos and papers\n\n* **LightAutoML crash courses**:\n    - (Russian) [AutoML course for OpenDataScience community](https://ods.ai/tracks/automl-course-part1)\n\n* **Video guides**:\n    - (Russian) [LightAutoML webinar for Sberloga community](https://www.youtube.com/watch?v=ci8uqgWFJGg) ([Alexander Ryzhkov](https://kaggle.com/alexryzhkov), [Dmitry Simakov](https://kaggle.com/simakov))\n    - (Russian) [LightAutoML hands-on tutorial in Kaggle Kernels](https://www.youtube.com/watch?v=TYu1UG-E9e8) ([Alexander Ryzhkov](https://kaggle.com/alexryzhkov))\n    - (English) [Automated Machine Learning with LightAutoML: theory and practice](https://www.youtube.com/watch?v=4pbO673B9Oo) ([Alexander Ryzhkov](https://kaggle.com/alexryzhkov))\n    - (English) [LightAutoML framework general overview, benchmarks and advantages for business](https://vimeo.com/485383651) ([Alexander Ryzhkov](https://kaggle.com/alexryzhkov))\n    - (English) [LightAutoML practical guide - ML pipeline presets overview](https://vimeo.com/487166940) ([Dmitry Simakov](https://kaggle.com/simakov))\n\n* **Papers**:\n    - Anton Vakhrushev, Alexander Ryzhkov, Dmitry Simakov, Rinchin Damdinov, Maxim Savchenko, Alexander Tuzhilin ["LightAutoML: AutoML Solution for a Large Financial Services Ecosystem"](https://arxiv.org/pdf/2109.01528.pdf). arXiv:2109.01528, 2021.\n\n* **Articles about LightAutoML**:\n    - (English) [LightAutoML vs Titanic: 80% accuracy in several lines of code (Medium)](https://alexmryzhkov.medium.com/lightautoml-preset-usage-tutorial-2cce7da6f936)\n    - (English) [Hands-On Python Guide to LightAutoML – An Automatic ML Model Creation Framework (Analytic Indian Mag)](https://analyticsindiamag.com/hands-on-python-guide-to-lama-an-automatic-ml-model-creation-framework/?fbclid=IwAR0f0cVgQWaLI60m1IHMD6VZfmKce0ZXxw-O8VRTdRALsKtty8a-ouJex7g)\n\n[Back to top](#toc)\n\n<a name="contributing"></a>\n# Contributing to LightAutoML\nIf you are interested in contributing to LightAutoML, please read the [Contributing Guide](.github/CONTRIBUTING.md) to get started.\n\n[Back to top](#toc)\n\n<a name="apache"></a>\n# License\nThis project is licensed under the Apache License, Version 2.0. See [LICENSE](https://github.com/AILab-MLTools/LightAutoML/blob/master/LICENSE) file for more details.\n\n[Back to top](#toc)\n\n<a name="developers"></a>\n# For developers\n\n## Build your own custom pipeline:\n\n```python\nimport pandas as pd\nfrom sklearn.metrics import f1_score\n\nfrom lightautoml.automl.presets.tabular_presets import TabularAutoML\nfrom lightautoml.tasks import Task\n\ndf_train = pd.read_csv(\'../input/titanic/train.csv\')\ndf_test = pd.read_csv(\'../input/titanic/test.csv\')\n\n# define that machine learning problem is binary classification\ntask = Task("binary")\n\nreader = PandasToPandasReader(task, cv=N_FOLDS, random_state=RANDOM_STATE)\n\n# create a feature selector\nmodel0 = BoostLGBM(\n    default_params={\'learning_rate\': 0.05, \'num_leaves\': 64,\n    \'seed\': 42, \'num_threads\': N_THREADS}\n)\npipe0 = LGBSimpleFeatures()\nmbie = ModelBasedImportanceEstimator()\nselector = ImportanceCutoffSelector(pipe0, model0, mbie, cutoff=0)\n\n# build first level pipeline for AutoML\npipe = LGBSimpleFeatures()\n# stop after 20 iterations or after 30 seconds\nparams_tuner1 = OptunaTuner(n_trials=20, timeout=30)\nmodel1 = BoostLGBM(\n    default_params={\'learning_rate\': 0.05, \'num_leaves\': 128,\n    \'seed\': 1, \'num_threads\': N_THREADS}\n)\nmodel2 = BoostLGBM(\n    default_params={\'learning_rate\': 0.025, \'num_leaves\': 64,\n    \'seed\': 2, \'num_threads\': N_THREADS}\n)\npipeline_lvl1 = MLPipeline([\n    (model1, params_tuner1),\n    model2\n], pre_selection=selector, features_pipeline=pipe, post_selection=None)\n\n# build second level pipeline for AutoML\npipe1 = LGBSimpleFeatures()\nmodel = BoostLGBM(\n    default_params={\'learning_rate\': 0.05, \'num_leaves\': 64,\n    \'max_bin\': 1024, \'seed\': 3, \'num_threads\': N_THREADS},\n    freeze_defaults=True\n)\npipeline_lvl2 = MLPipeline([model], pre_selection=None, features_pipeline=pipe1,\n post_selection=None)\n\n# build AutoML pipeline\nautoml = AutoML(reader, [\n    [pipeline_lvl1],\n    [pipeline_lvl2],\n], skip_conn=False)\n\n# train AutoML and get predictions\noof_pred = automl.fit_predict(df_train, roles = {\'target\': \'Survived\', \'drop\': [\'PassengerId\']})\ntest_pred = automl.predict(df_test)\n\npd.DataFrame({\n    \'PassengerId\':df_test.PassengerId,\n    \'Survived\': (test_pred.data[:, 0] > 0.5)*1\n}).to_csv(\'submit.csv\', index = False)\n```\n\n[Back to top](#toc)\n\n<a name="support"></a>\n# Support and feature requests\nSeek prompt advice at [Telegram group](https://t.me/lightautoml).\n\nOpen bug reports and feature requests on GitHub [issues](https://github.com/AILab-MLTools/LightAutoML/issues).\n',
     'author': 'Alexander Ryzhkov',
     'author_email': 'alexmryzhkov@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://lightautoml.readthedocs.io/en/latest/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.6.1,<3.10',
+    'python_requires': '>=3.6.1,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `LightAutoML-0.3.7.3/PKG-INFO` & `lightautoml-0.3.8b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,79 +1,89 @@
 Metadata-Version: 2.1
 Name: lightautoml
-Version: 0.3.7.3
+Version: 0.3.8b1
 Summary: Fast and customizable framework for automatic ML model creation (AutoML)
 Home-page: https://lightautoml.readthedocs.io/en/latest/
 License: Apache-2.0
 Author: Alexander Ryzhkov
 Author-email: alexmryzhkov@gmail.com
-Requires-Python: >=3.6.1,<3.10
+Requires-Python: >=3.6.1,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Typing :: Typed
 Provides-Extra: afg
 Provides-Extra: all
 Provides-Extra: cv
 Provides-Extra: nlp
 Provides-Extra: report
-Requires-Dist: PyWavelets; extra == "cv" or extra == "all"
-Requires-Dist: albumentations (<=1.0.3); extra == "cv" or extra == "all"
+Requires-Dist: PyWavelets ; extra == "cv" or extra == "all"
+Requires-Dist: albumentations (<=1.0.3) ; extra == "cv" or extra == "all"
 Requires-Dist: autowoe (>=1.2)
 Requires-Dist: catboost (>=0.26.1)
-Requires-Dist: cffi (==1.14.5); extra == "report" or extra == "all"
+Requires-Dist: cffi (==1.14.5) ; extra == "report" or extra == "all"
 Requires-Dist: cmaes
-Requires-Dist: dataclasses (==0.6); python_version < "3.7"
-Requires-Dist: efficientnet-pytorch; extra == "cv" or extra == "all"
-Requires-Dist: featuretools (>=1.11.1); (python_version >= "3.7") and (extra == "afg" or extra == "all")
-Requires-Dist: gensim (>=4); extra == "nlp" or extra == "all"
+Requires-Dist: dataclasses (==0.6) ; python_version < "3.7"
+Requires-Dist: efficientnet-pytorch ; extra == "cv" or extra == "all"
+Requires-Dist: featuretools (>=1.11.1) ; (python_version >= "3.7") and (extra == "afg" or extra == "all")
+Requires-Dist: gensim (>=4) ; extra == "nlp" or extra == "all"
 Requires-Dist: holidays
-Requires-Dist: importlib-metadata (>=1.0,<2.0); python_version < "3.8"
+Requires-Dist: importlib-metadata (>=1.0) ; python_version < "3.8"
 Requires-Dist: jinja2
-Requires-Dist: joblib
+Requires-Dist: joblib (<1.3.0)
 Requires-Dist: json2html
 Requires-Dist: lightgbm (>=2.3,<=3.2.1)
 Requires-Dist: networkx
-Requires-Dist: nltk; extra == "nlp" or extra == "all"
-Requires-Dist: opencv-python (<=4.5.2.52); extra == "cv" or extra == "all"
+Requires-Dist: nltk ; extra == "nlp" or extra == "all"
+Requires-Dist: numpy (<1.24.0)
+Requires-Dist: opencv-python (<=4.5.2.52) ; extra == "cv" or extra == "all"
 Requires-Dist: optuna
-Requires-Dist: pandas (<=1.1.5); python_full_version >= "3.6.1" and python_full_version < "3.7.1"
-Requires-Dist: pandas (<=1.3.5); python_full_version >= "3.7.1" and python_version < "3.8"
-Requires-Dist: pandas (<=1.4.3); python_version >= "3.8"
-Requires-Dist: poetry-core (>=1.0.0,<2.0.0)
+Requires-Dist: pandas (<=1.1.5) ; python_full_version >= "3.6.1" and python_full_version < "3.7.1"
+Requires-Dist: pandas (<=1.3.5) ; python_full_version >= "3.7.1" and python_version < "3.8"
+Requires-Dist: pandas (<=1.4.3) ; python_version >= "3.8"
+Requires-Dist: poetry-core (>=1.0.0) ; python_version < "3.7"
+Requires-Dist: poetry-core (>=1.0.0,<2.0.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: pyyaml
 Requires-Dist: scikit-learn (>=0.22)
 Requires-Dist: seaborn
-Requires-Dist: torch (<1.9)
-Requires-Dist: torch (==1.7.0); python_full_version == "3.6.1" and sys_platform == "win32"
-Requires-Dist: torchvision
-Requires-Dist: torchvision (==0.8.0); (python_full_version == "3.6.1" and sys_platform == "win32") and (extra == "cv" or extra == "all")
+Requires-Dist: statsmodels (<=0.14.0)
+Requires-Dist: torch (==1.7.0) ; python_full_version == "3.6.1" and sys_platform == "win32"
+Requires-Dist: torch (>=1.0.0)
+Requires-Dist: torchvision (==0.8.0) ; (python_full_version == "3.6.1" and sys_platform == "win32") and (extra == "cv" or extra == "all")
+Requires-Dist: torchvision ; extra == "cv" or extra == "all"
 Requires-Dist: tqdm
-Requires-Dist: transformers (>=4); extra == "nlp" or extra == "all"
-Requires-Dist: weasyprint (==52.5); extra == "report" or extra == "all"
+Requires-Dist: transformers (>=4) ; extra == "nlp" or extra == "all"
+Requires-Dist: weasyprint (==52.5) ; extra == "report" or extra == "all"
 Project-URL: Repository, https://github.com/AILab-MLTools/LightAutoML
 Description-Content-Type: text/markdown
 
 <img src=https://github.com/AILab-MLTools/LightAutoML/raw/master/imgs/LightAutoML_logo_big.png />
 
 # LightAutoML - automatic model creation framework
 
 [![Telegram](https://img.shields.io/badge/chat-on%20Telegram-2ba2d9.svg)](https://t.me/lightautoml)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/lightautoml?color=green&label=PyPI%20downloads&logo=pypi&logoColor=orange&style=plastic)
 ![Read the Docs](https://img.shields.io/readthedocs/lightautoml?style=plastic)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![Poetry-Lock](https://img.shields.io/github/workflow/status/sb-ai-lab/LightAutoML/Poetry%20run/master?label=Poetry-Lock)
+
 
 LightAutoML (LAMA) is an AutoML framework which provides automatic model creation for the following tasks:
 - binary classification
 - multiclass  classification
 - regression
 
 Current version of the package handles datasets that have independent samples in each row. I.e. **each row is an object with its specific features and target**.
@@ -181,26 +191,29 @@
 - [Titanic **12-code-lines** competition solution (78% accuracy)](https://www.kaggle.com/alexryzhkov/lightautoml-extreme-short-titanic-solution)
 - [House prices competition solution](https://www.kaggle.com/alexryzhkov/lightautoml-houseprices-love)
 - [Natural Language Processing with Disaster Tweets solution](https://www.kaggle.com/alexryzhkov/lightautoml-starter-nlp)
 - [Tabular Playground Series March 2021 competition solution](https://www.kaggle.com/alexryzhkov/lightautoml-starter-for-tabulardatamarch)
 - [Tabular Playground Series February 2021 competition solution](https://www.kaggle.com/alexryzhkov/lightautoml-tabulardata-love)
 - [Interpretable WhiteBox solution](https://www.kaggle.com/simakov/lama-whitebox-preset-example)
 - [Custom ML pipeline elements inside existing ones](https://www.kaggle.com/simakov/lama-custom-automl-pipeline-example)
+- [Custom ML pipeline elements inside existing ones](https://www.kaggle.com/simakov/lama-custom-automl-pipeline-example)
+- [Tabular Playground Series November 2022 competition solution with Neural Networks](https://www.kaggle.com/code/mikhailkuz/lightautoml-nn-happiness)
 
 ### Google Colab tutorials and [other examples](examples/):
 
 - [`Tutorial_1_basics.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_1_basics.ipynb) - get started with LightAutoML on tabular data.
 - [`Tutorial_2_WhiteBox_AutoWoE.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_2_WhiteBox_AutoWoE.ipynb) - creating interpretable models.
 - [`Tutorial_3_sql_data_source.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_3_sql_data_source.ipynb) - shows how to use LightAutoML presets (both standalone and time utilized variants) for solving ML tasks on tabular data from SQL data base instead of CSV.
 - [`Tutorial_4_NLP_Interpretation.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_4_NLP_Interpretation.ipynb) - example of using TabularNLPAutoML preset, LimeTextExplainer.
 - [`Tutorial_5_uplift.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_5_uplift.ipynb) - shows how to use LightAutoML for a uplift-modeling task.
 - [`Tutorial_6_custom_pipeline.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_6_custom_pipeline.ipynb) - shows how to create your own pipeline from specified blocks: pipelines for feature generation and feature selection, ML algorithms, hyperparameter optimization etc.
 - [`Tutorial_7_ICE_and_PDP_interpretation.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_7_ICE_and_PDP_interpretation.ipynb) - shows how to obtain local and global interpretation of model results using ICE and PDP approaches.
 - [`Tutorial_8_CV_preset.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_8_CV_preset.ipynb) - example of using TabularCVAutoML preset in CV multi-class classification task.
-
+- [`Tutorial_9_neural_networks.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_9_neural_networks.ipynb) - example of using Tabular preset with neural networks.
+- [`Tutorial_10_relational_data_with_star_scheme.ipynb`](https://colab.research.google.com/github/AILab-MLTools/LightAutoML/blob/master/examples/tutorials/Tutorial_10_relational_data_with_star_scheme.ipynb) - example of using Tabular preset with neural networks.
 
 **Note 1**: for production you have no need to use profiler (which increase work time and memory consomption), so please do not turn it on - it is in off state by default
 
 **Note 2**: to take a look at this report after the run, please comment last line of demo with report deletion command.
 
 ### Courses, videos and papers
```

