# Comparing `tmp/truss-0.5.0.tar.gz` & `tmp/truss-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.5.0.tar", max compression
+gzip compressed data, was "truss-0.5.1.tar", max compression
```

## Comparing `truss-0.5.0.tar` & `truss-0.5.1.tar`

### file list

```diff
@@ -1,210 +1,217 @@
--rw-r--r--   0        0        0     5483 2023-07-20 04:33:21.801140 truss-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2418 2023-07-20 04:33:21.801140 truss-0.5.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2023-07-20 04:33:21.801140 truss-0.5.0/LICENSE
--rw-r--r--   0        0        0     3415 2023-07-20 04:33:21.801140 truss-0.5.0/README.md
--rw-r--r--   0        0        0      933 2023-07-20 04:33:21.801140 truss-0.5.0/context_builder.Dockerfile
--rw-r--r--   0        0        0     2502 2023-07-20 04:33:21.905146 truss-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      330 2023-07-20 04:33:21.905146 truss-0.5.0/truss/__init__.py
--rw-r--r--   0        0        0      252 2023-07-20 04:33:21.905146 truss-0.5.0/truss/blob/blob_backend.py
--rw-r--r--   0        0        0      733 2023-07-20 04:33:21.905146 truss-0.5.0/truss/blob/blob_backend_registry.py
--rw-r--r--   0        0        0      648 2023-07-20 04:33:21.905146 truss-0.5.0/truss/blob/http_public_blob_backend.py
--rw-r--r--   0        0        0    13068 2023-07-20 04:33:21.905146 truss-0.5.0/truss/build.py
--rw-r--r--   0        0        0    12963 2023-07-20 04:33:21.905146 truss-0.5.0/truss/cli.py
--rw-r--r--   0        0        0     2873 2023-07-20 04:33:21.905146 truss-0.5.0/truss/constants.py
--rw-r--r--   0        0        0      338 2023-07-20 04:33:21.905146 truss-0.5.0/truss/contexts/image_builder/cache_warmer.py
--rw-r--r--   0        0        0     1294 2023-07-20 04:33:21.905146 truss-0.5.0/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0     7028 2023-07-20 04:33:21.905146 truss-0.5.0/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     4684 2023-07-20 04:33:21.905146 truss-0.5.0/truss/contexts/image_builder/training_image_builder.py
--rw-r--r--   0        0        0     1893 2023-07-20 04:33:21.905146 truss-0.5.0/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     2120 2023-07-20 04:33:21.905146 truss-0.5.0/truss/contexts/local_loader/docker_build_emulator.py
--rw-r--r--   0        0        0     1823 2023-07-20 04:33:21.905146 truss-0.5.0/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     2239 2023-07-20 04:33:21.905146 truss-0.5.0/truss/contexts/local_loader/train_local.py
--rw-r--r--   0        0        0      974 2023-07-20 04:33:21.905146 truss-0.5.0/truss/contexts/local_loader/truss_file_syncer.py
--rw-r--r--   0        0        0     5801 2023-07-20 04:33:21.905146 truss-0.5.0/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2023-07-20 04:33:21.905146 truss-0.5.0/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2023-07-20 04:33:21.905146 truss-0.5.0/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2023-07-20 04:33:21.905146 truss-0.5.0/truss/decorators.py
--rw-r--r--   0        0        0     3641 2023-07-20 04:33:21.905146 truss-0.5.0/truss/docker.py
--rw-r--r--   0        0        0     3759 2023-07-20 04:33:21.905146 truss-0.5.0/truss/environment_inference/requirements_inference.py
--rw-r--r--   0        0        0      643 2023-07-20 04:33:21.905146 truss-0.5.0/truss/errors.py
--rw-r--r--   0        0        0      824 2023-07-20 04:33:21.905146 truss-0.5.0/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2023-07-20 04:33:21.905146 truss-0.5.0/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     2713 2023-07-20 04:33:21.905146 truss-0.5.0/truss/model_framework.py
--rw-r--r--   0        0        0     1687 2023-07-20 04:33:21.905146 truss-0.5.0/truss/model_frameworks/__init__.py
--rw-r--r--   0        0        0     1895 2023-07-20 04:33:21.905146 truss-0.5.0/truss/model_frameworks/huggingface_transformer.py
--rw-r--r--   0        0        0      918 2023-07-20 04:33:21.905146 truss-0.5.0/truss/model_frameworks/keras.py
--rw-r--r--   0        0        0     1230 2023-07-20 04:33:21.905146 truss-0.5.0/truss/model_frameworks/lightgbm.py
--rw-r--r--   0        0        0     2403 2023-07-20 04:33:21.905146 truss-0.5.0/truss/model_frameworks/mlflow.py
--rw-r--r--   0        0        0     2441 2023-07-20 04:33:21.905146 truss-0.5.0/truss/model_frameworks/pytorch.py
--rw-r--r--   0        0        0     1225 2023-07-20 04:33:21.905146 truss-0.5.0/truss/model_frameworks/sklearn.py
--rw-r--r--   0        0        0     1027 2023-07-20 04:33:21.905146 truss-0.5.0/truss/model_frameworks/xgboost.py
--rw-r--r--   0        0        0     5425 2023-07-20 04:33:21.905146 truss-0.5.0/truss/model_inference.py
--rw-r--r--   0        0        0      510 2023-07-20 04:33:21.905146 truss-0.5.0/truss/notebook.py
--rw-r--r--   0        0        0    14800 2023-07-20 04:33:21.905146 truss-0.5.0/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      139 2023-07-20 04:33:21.905146 truss-0.5.0/truss/patch/constants.py
--rw-r--r--   0        0        0      774 2023-07-20 04:33:21.905146 truss-0.5.0/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2378 2023-07-20 04:33:21.905146 truss-0.5.0/truss/patch/hash.py
--rw-r--r--   0        0        0     2930 2023-07-20 04:33:21.905146 truss-0.5.0/truss/patch/local_truss_patch_applier.py
--rw-r--r--   0        0        0      468 2023-07-20 04:33:21.905146 truss-0.5.0/truss/patch/signature.py
--rw-r--r--   0        0        0     3075 2023-07-20 04:33:21.905146 truss-0.5.0/truss/patch/truss_dir_patch_applier.py
--rw-r--r--   0        0        0      937 2023-07-20 04:33:21.905146 truss-0.5.0/truss/patch/types.py
--rw-r--r--   0        0        0      237 2023-07-20 04:33:21.905146 truss-0.5.0/truss/pytest.ini
--rw-r--r--   0        0        0      705 2023-07-20 04:33:21.905146 truss-0.5.0/truss/readme_generator.py
--rw-r--r--   0        0        0      176 2023-07-20 04:33:21.909146 truss-0.5.0/truss/remote/baseten/__init__.py
--rw-r--r--   0        0        0     4650 2023-07-20 04:33:21.909146 truss-0.5.0/truss/remote/baseten/api.py
--rw-r--r--   0        0        0      752 2023-07-20 04:33:21.909146 truss-0.5.0/truss/remote/baseten/auth.py
--rw-r--r--   0        0        0     3549 2023-07-20 04:33:21.909146 truss-0.5.0/truss/remote/baseten/core.py
--rw-r--r--   0        0        0      943 2023-07-20 04:33:21.909146 truss-0.5.0/truss/remote/baseten/error.py
--rw-r--r--   0        0        0     4841 2023-07-20 04:33:21.909146 truss-0.5.0/truss/remote/baseten/remote.py
--rw-r--r--   0        0        0     1156 2023-07-20 04:33:21.909146 truss-0.5.0/truss/remote/baseten/service.py
--rw-r--r--   0        0        0     2001 2023-07-20 04:33:21.909146 truss-0.5.0/truss/remote/baseten/utils/tar.py
--rw-r--r--   0        0        0      985 2023-07-20 04:33:21.909146 truss-0.5.0/truss/remote/baseten/utils/transfer.py
--rw-r--r--   0        0        0     3330 2023-07-20 04:33:21.909146 truss-0.5.0/truss/remote/remote_factory.py
--rw-r--r--   0        0        0     5781 2023-07-20 04:33:21.909146 truss-0.5.0/truss/remote/truss_remote.py
--rw-r--r--   0        0        0     2482 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/__init__.py
--rw-r--r--   0        0        0     1967 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     3819 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     5103 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      955 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     6317 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     4026 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2652 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0      998 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/control/control/helpers/truss_patch/__init__.py
--rw-r--r--   0        0        0     1842 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
--rw-r--r--   0        0        0     7386 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
--rw-r--r--   0        0        0      551 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
--rw-r--r--   0        0        0      208 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/control/control/helpers/truss_patch/system_packages.py
--rw-r--r--   0        0        0     5930 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     2319 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/control/control/server.py
--rw-r--r--   0        0        0      144 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       48 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0      534 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0      460 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/custom/train/train.py
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/huggingface_transformer/model/__init__.py
--rw-r--r--   0        0        0     1827 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/huggingface_transformer/model/model.py
--rw-r--r--   0        0        0       47 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/huggingface_transformer/requirements.txt
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/keras/model/__init__.py
--rw-r--r--   0        0        0      728 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/keras/model/model.py
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/lightgbm/model/__init__.py
--rw-r--r--   0        0        0     1251 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/lightgbm/model/model.py
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/mlflow/model/__init__.py
--rw-r--r--   0        0        0      751 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/mlflow/model/model.py
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/pipeline/model/__init__.py
--rw-r--r--   0        0        0      430 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/pipeline/model/model.py
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/pytorch/model/__init__.py
--rw-r--r--   0        0        0     1263 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/pytorch/model/model.py
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0     2433 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     2382 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/server/common/patches/whisper/patch.py
--rw-r--r--   0        0        0     1450 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/server/common/patches.py
--rw-r--r--   0        0        0      593 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/server/common/retry.py
--rw-r--r--   0        0        0     2340 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/server/common/termination_handler_middleware.py
--rw-r--r--   0        0        0    12330 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0      727 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0     8344 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      274 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0     3279 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/shared/logging.py
--rw-r--r--   0        0        0     1430 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0     3318 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/shared/serialization.py
--rw-r--r--   0        0        0     1863 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/shared/util.py
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/sklearn/model/__init__.py
--rw-r--r--   0        0        0     1221 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/sklearn/model/model.py
--rw-r--r--   0        0        0     3400 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/training/job.py
--rw-r--r--   0        0        0       12 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/training/requirements.txt
--rw-r--r--   0        0        0      491 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/training.Dockerfile.jinja
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/xgboost/model/__init__.py
--rw-r--r--   0        0        0     1453 2023-07-20 04:33:21.909146 truss-0.5.0/truss/templates/xgboost/model/model.py
--rw-r--r--   0        0        0    30286 2023-07-20 04:33:21.909146 truss-0.5.0/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0       93 2023-07-20 04:33:21.909146 truss-0.5.0/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2023-07-20 04:33:21.909146 truss-0.5.0/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0     1394 2023-07-20 04:33:21.909146 truss-0.5.0/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0      739 2023-07-20 04:33:21.909146 truss-0.5.0/truss/test_data/model_load_failure_test/config.yaml
--rw-r--r--   0        0        0      552 2023-07-20 04:33:21.909146 truss-0.5.0/truss/test_data/model_load_failure_test/model/model.py
--rw-r--r--   0        0        0     1267 2023-07-20 04:33:21.909146 truss-0.5.0/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0     1550 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/server.Dockerfile
--rw-r--r--   0        0        0      669 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/server_conformance_test_truss/config.yaml
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/server_conformance_test_truss/model/__init__.py
--rw-r--r--   0        0        0      597 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/server_conformance_test_truss/model/model.py
--rw-r--r--   0        0        0      739 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/test_streaming_truss/config.yaml
--rw-r--r--   0        0        0      568 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/test_streaming_truss/model/model.py
--rw-r--r--   0        0        0      669 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0      534 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        6 2023-07-20 04:33:21.913146 truss-0.5.0/truss/test_data/test_truss/packages/test_package/test.py
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/__init__.py
--rw-r--r--   0        0        0    22226 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/conftest.py
--rw-r--r--   0        0        0     1255 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/contexts/image_builder/test_serving_image_builder.py
--rw-r--r--   0        0        0      783 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      968 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/environments_inference/test_requirements_inference.py
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0        0 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/model_frameworks/__init__.py
--rw-r--r--   0        0        0     3293 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
--rw-r--r--   0        0        0     2789 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/model_frameworks/test_keras_framework.py
--rw-r--r--   0        0        0     2409 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/model_frameworks/test_lightgbm_framework.py
--rw-r--r--   0        0        0     1479 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/model_frameworks/test_pytorch_framework.py
--rw-r--r--   0        0        0     2427 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/model_frameworks/test_sklearn_framework.py
--rw-r--r--   0        0        0     2437 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/model_frameworks/test_xgboost_framework.py
--rw-r--r--   0        0        0    18726 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0      487 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      394 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0     1929 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/patch/test_truss_dir_patch_applier.py
--rw-r--r--   0        0        0      273 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0     2073 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/remote/baseten/test_api.py
--rw-r--r--   0        0        0      580 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/remote/baseten/test_auth.py
--rw-r--r--   0        0        0      835 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/remote/baseten/test_core.py
--rw-r--r--   0        0        0     4110 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/remote/test_remote_factory.py
--rw-r--r--   0        0        0     2394 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/remote/test_truss_remote.py
--rw-r--r--   0        0        0    10415 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/samples.py
--rw-r--r--   0        0        0      283 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     6081 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
--rw-r--r--   0        0        0      964 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
--rw-r--r--   0        0        0     7513 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0     8326 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/templates/control/control/test_server_integration.py
--rw-r--r--   0        0        0     1560 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/templates/core/server/common/test_truss_server.py
--rw-r--r--   0        0        0      821 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     2038 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/templates/server/common/test_retry.py
--rw-r--r--   0        0        0     2605 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/templates/server/common/test_termination_handler_middleware.py
--rw-r--r--   0        0        0     2252 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/templates/server/test_model_wrapper.py
--rw-r--r--   0        0        0     1910 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/test_backward.py
--rw-r--r--   0        0        0     8260 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/test_build.py
--rw-r--r--   0        0        0     7759 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0    14982 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/test_control_truss_patching.py
--rw-r--r--   0        0        0      517 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/test_docker.py
--rw-r--r--   0        0        0     8584 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0      656 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/test_notebooks.py
--rw-r--r--   0        0        0     1483 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    30057 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0     1865 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/test_validation.py
--rw-r--r--   0        0        0     4974 2023-07-20 04:33:21.913146 truss-0.5.0/truss/tests/util/test_path.py
--rw-r--r--   0        0        0    14790 2023-07-20 04:33:21.913146 truss-0.5.0/truss/truss_config.py
--rw-r--r--   0        0        0     2698 2023-07-20 04:33:21.913146 truss-0.5.0/truss/truss_gatherer.py
--rw-r--r--   0        0        0    41143 2023-07-20 04:33:21.913146 truss-0.5.0/truss/truss_handle.py
--rw-r--r--   0        0        0     5671 2023-07-20 04:33:21.913146 truss-0.5.0/truss/truss_spec.py
--rw-r--r--   0        0        0     2782 2023-07-20 04:33:21.913146 truss-0.5.0/truss/types.py
--rw-r--r--   0        0        0     3121 2023-07-20 04:33:21.917147 truss-0.5.0/truss/util/.truss_ignore
--rw-r--r--   0        0        0      379 2023-07-20 04:33:21.917147 truss-0.5.0/truss/util/data_structures.py
--rw-r--r--   0        0        0     2552 2023-07-20 04:33:21.917147 truss-0.5.0/truss/util/download.py
--rw-r--r--   0        0        0      553 2023-07-20 04:33:21.917147 truss-0.5.0/truss/util/gpu.py
--rw-r--r--   0        0        0      333 2023-07-20 04:33:21.917147 truss-0.5.0/truss/util/jinja.py
--rw-r--r--   0        0        0     6040 2023-07-20 04:33:21.917147 truss-0.5.0/truss/util/path.py
--rw-r--r--   0        0        0     2736 2023-07-20 04:33:21.917147 truss-0.5.0/truss/validation.py
--rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 truss-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     5483 2023-07-26 21:14:15.359366 truss-0.5.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2418 2023-07-26 21:14:15.363366 truss-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2023-07-26 21:14:15.363366 truss-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3415 2023-07-26 21:14:15.363366 truss-0.5.1/README.md
+-rw-r--r--   0        0        0      933 2023-07-26 21:14:15.363366 truss-0.5.1/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2546 2023-07-26 21:14:15.435366 truss-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-07-26 21:14:15.435366 truss-0.5.1/truss/__init__.py
+-rw-r--r--   0        0        0      252 2023-07-26 21:14:15.435366 truss-0.5.1/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2023-07-26 21:14:15.435366 truss-0.5.1/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2023-07-26 21:14:15.435366 truss-0.5.1/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0    13068 2023-07-26 21:14:15.439365 truss-0.5.1/truss/build.py
+-rw-r--r--   0        0        0    11021 2023-07-26 21:14:15.439365 truss-0.5.1/truss/cli.py
+-rw-r--r--   0        0        0     2873 2023-07-26 21:14:15.439365 truss-0.5.1/truss/constants.py
+-rw-r--r--   0        0        0      338 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/image_builder/cache_warmer.py
+-rw-r--r--   0        0        0     1294 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0     7028 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     4684 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/image_builder/training_image_builder.py
+-rw-r--r--   0        0        0     1893 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     2120 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/local_loader/docker_build_emulator.py
+-rw-r--r--   0        0        0     1823 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     2239 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/local_loader/train_local.py
+-rw-r--r--   0        0        0     1072 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/local_loader/truss_file_syncer.py
+-rw-r--r--   0        0        0     5801 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2023-07-26 21:14:15.439365 truss-0.5.1/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2023-07-26 21:14:15.439365 truss-0.5.1/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2023-07-26 21:14:15.439365 truss-0.5.1/truss/docker.py
+-rw-r--r--   0        0        0     3759 2023-07-26 21:14:15.439365 truss-0.5.1/truss/environment_inference/requirements_inference.py
+-rw-r--r--   0        0        0      643 2023-07-26 21:14:15.439365 truss-0.5.1/truss/errors.py
+-rw-r--r--   0        0        0      824 2023-07-26 21:14:15.439365 truss-0.5.1/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2023-07-26 21:14:15.439365 truss-0.5.1/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     2713 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_framework.py
+-rw-r--r--   0        0        0     1687 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     1895 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/huggingface_transformer.py
+-rw-r--r--   0        0        0      918 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/keras.py
+-rw-r--r--   0        0        0     1230 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/lightgbm.py
+-rw-r--r--   0        0        0     2403 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/mlflow.py
+-rw-r--r--   0        0        0     2441 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/pytorch.py
+-rw-r--r--   0        0        0     1225 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/sklearn.py
+-rw-r--r--   0        0        0     1027 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_frameworks/xgboost.py
+-rw-r--r--   0        0        0     5425 2023-07-26 21:14:15.439365 truss-0.5.1/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2023-07-26 21:14:15.439365 truss-0.5.1/truss/notebook.py
+-rw-r--r--   0        0        0    15420 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      139 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/constants.py
+-rw-r--r--   0        0        0      774 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2378 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/hash.py
+-rw-r--r--   0        0        0     2930 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/local_truss_patch_applier.py
+-rw-r--r--   0        0        0      468 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/signature.py
+-rw-r--r--   0        0        0     3075 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      937 2023-07-26 21:14:15.439365 truss-0.5.1/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2023-07-26 21:14:15.439365 truss-0.5.1/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2023-07-26 21:14:15.439365 truss-0.5.1/truss/readme_generator.py
+-rw-r--r--   0        0        0      176 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/__init__.py
+-rw-r--r--   0        0        0     4919 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/api.py
+-rw-r--r--   0        0        0      752 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/auth.py
+-rw-r--r--   0        0        0     3616 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/core.py
+-rw-r--r--   0        0        0      943 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/error.py
+-rw-r--r--   0        0        0     4639 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/remote.py
+-rw-r--r--   0        0        0     1156 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/service.py
+-rw-r--r--   0        0        0     2001 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/utils/tar.py
+-rw-r--r--   0        0        0      985 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/baseten/utils/transfer.py
+-rw-r--r--   0        0        0     1407 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/remote_cli.py
+-rw-r--r--   0        0        0     4219 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/remote_factory.py
+-rw-r--r--   0        0        0     5970 2023-07-26 21:14:15.439365 truss-0.5.1/truss/remote/truss_remote.py
+-rw-r--r--   0        0        0     2482 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/__init__.py
+-rw-r--r--   0        0        0     1967 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     3819 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     5103 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      955 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     6317 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     4026 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2652 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0      998 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/truss_patch/__init__.py
+-rw-r--r--   0        0        0     1842 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
+-rw-r--r--   0        0        0     7386 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
+-rw-r--r--   0        0        0      551 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
+-rw-r--r--   0        0        0      208 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/truss_patch/system_packages.py
+-rw-r--r--   0        0        0     5930 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     2319 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0      144 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       48 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0      534 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0      460 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/custom/train/train.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/huggingface_transformer/model/__init__.py
+-rw-r--r--   0        0        0     1827 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/huggingface_transformer/model/model.py
+-rw-r--r--   0        0        0       47 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/huggingface_transformer/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/keras/model/__init__.py
+-rw-r--r--   0        0        0      728 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/keras/model/model.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/lightgbm/model/__init__.py
+-rw-r--r--   0        0        0     1251 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/lightgbm/model/model.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/mlflow/model/__init__.py
+-rw-r--r--   0        0        0      751 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/mlflow/model/model.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/pipeline/model/__init__.py
+-rw-r--r--   0        0        0      430 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/pipeline/model/model.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/pytorch/model/__init__.py
+-rw-r--r--   0        0        0     1263 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/pytorch/model/model.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0     2433 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     2382 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server/common/patches/whisper/patch.py
+-rw-r--r--   0        0        0     1450 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server/common/patches.py
+-rw-r--r--   0        0        0      593 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server/common/retry.py
+-rw-r--r--   0        0        0     2340 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server/common/termination_handler_middleware.py
+-rw-r--r--   0        0        0    12328 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0      727 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0    11624 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      274 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     3279 2023-07-26 21:14:15.439365 truss-0.5.1/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/shared/logging.py
+-rw-r--r--   0        0        0     1430 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0     3318 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/shared/serialization.py
+-rw-r--r--   0        0        0     1863 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/shared/util.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/sklearn/model/__init__.py
+-rw-r--r--   0        0        0     1221 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/sklearn/model/model.py
+-rw-r--r--   0        0        0     3400 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/training/job.py
+-rw-r--r--   0        0        0       12 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/training/requirements.txt
+-rw-r--r--   0        0        0      491 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/training.Dockerfile.jinja
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/xgboost/model/__init__.py
+-rw-r--r--   0        0        0     1453 2023-07-26 21:14:15.443366 truss-0.5.1/truss/templates/xgboost/model/model.py
+-rw-r--r--   0        0        0    30286 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0       93 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0     1394 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0      739 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/model_load_failure_test/config.yaml
+-rw-r--r--   0        0        0      552 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/model_load_failure_test/model/model.py
+-rw-r--r--   0        0        0     1267 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0     1550 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/server.Dockerfile
+-rw-r--r--   0        0        0      669 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/server_conformance_test_truss/config.yaml
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/server_conformance_test_truss/model/__init__.py
+-rw-r--r--   0        0        0      597 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/server_conformance_test_truss/model/model.py
+-rw-r--r--   0        0        0      739 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_async_truss/config.yaml
+-rw-r--r--   0        0        0      646 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_async_truss/model/model.py
+-rw-r--r--   0        0        0       34 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_concurrency_truss/config.yaml
+-rw-r--r--   0        0        0      547 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_concurrency_truss/model/model.py
+-rw-r--r--   0        0        0      739 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_streaming_async_generator_truss/config.yaml
+-rw-r--r--   0        0        0      521 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_streaming_async_generator_truss/model/model.py
+-rw-r--r--   0        0        0      773 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_streaming_truss/config.yaml
+-rw-r--r--   0        0        0      568 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_streaming_truss/model/model.py
+-rw-r--r--   0        0        0      669 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0      534 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        6 2023-07-26 21:14:15.443366 truss-0.5.1/truss/test_data/test_truss/packages/test_package/test.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/__init__.py
+-rw-r--r--   0        0        0    22226 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/conftest.py
+-rw-r--r--   0        0        0     1255 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/contexts/image_builder/test_serving_image_builder.py
+-rw-r--r--   0        0        0      783 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      968 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/environments_inference/test_requirements_inference.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     3293 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
+-rw-r--r--   0        0        0     2789 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/model_frameworks/test_keras_framework.py
+-rw-r--r--   0        0        0     2409 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/model_frameworks/test_lightgbm_framework.py
+-rw-r--r--   0        0        0     1479 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/model_frameworks/test_pytorch_framework.py
+-rw-r--r--   0        0        0     2427 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/model_frameworks/test_sklearn_framework.py
+-rw-r--r--   0        0        0     2437 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/model_frameworks/test_xgboost_framework.py
+-rw-r--r--   0        0        0    18726 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0      487 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      394 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0     1929 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/patch/test_truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      273 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0     2073 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/remote/baseten/test_api.py
+-rw-r--r--   0        0        0      580 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/remote/baseten/test_auth.py
+-rw-r--r--   0        0        0      835 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/remote/baseten/test_core.py
+-rw-r--r--   0        0        0     4316 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/remote/test_remote_factory.py
+-rw-r--r--   0        0        0     2394 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/remote/test_truss_remote.py
+-rw-r--r--   0        0        0    10415 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/samples.py
+-rw-r--r--   0        0        0      283 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     6081 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
+-rw-r--r--   0        0        0      964 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
+-rw-r--r--   0        0        0     7513 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0     8326 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/control/control/test_server_integration.py
+-rw-r--r--   0        0        0     1560 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/core/server/common/test_truss_server.py
+-rw-r--r--   0        0        0      821 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2038 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/server/common/test_retry.py
+-rw-r--r--   0        0        0     2605 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/server/common/test_termination_handler_middleware.py
+-rw-r--r--   0        0        0     2252 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/templates/server/test_model_wrapper.py
+-rw-r--r--   0        0        0     1910 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/test_backward.py
+-rw-r--r--   0        0        0     8260 2023-07-26 21:14:15.443366 truss-0.5.1/truss/tests/test_build.py
+-rw-r--r--   0        0        0     8657 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0    14982 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_control_truss_patching.py
+-rw-r--r--   0        0        0      517 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_docker.py
+-rw-r--r--   0        0        0    12242 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0      656 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1483 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    30057 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0     1865 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/test_validation.py
+-rw-r--r--   0        0        0     4974 2023-07-26 21:14:15.447366 truss-0.5.1/truss/tests/util/test_path.py
+-rw-r--r--   0        0        0    15256 2023-07-26 21:14:15.447366 truss-0.5.1/truss/truss_config.py
+-rw-r--r--   0        0        0     2698 2023-07-26 21:14:15.447366 truss-0.5.1/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    41143 2023-07-26 21:14:15.447366 truss-0.5.1/truss/truss_handle.py
+-rw-r--r--   0        0        0     5671 2023-07-26 21:14:15.447366 truss-0.5.1/truss/truss_spec.py
+-rw-r--r--   0        0        0     2782 2023-07-26 21:14:15.447366 truss-0.5.1/truss/types.py
+-rw-r--r--   0        0        0     3121 2023-07-26 21:14:15.447366 truss-0.5.1/truss/util/.truss_ignore
+-rw-r--r--   0        0        0      379 2023-07-26 21:14:15.447366 truss-0.5.1/truss/util/data_structures.py
+-rw-r--r--   0        0        0     2552 2023-07-26 21:14:15.447366 truss-0.5.1/truss/util/download.py
+-rw-r--r--   0        0        0      553 2023-07-26 21:14:15.447366 truss-0.5.1/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2023-07-26 21:14:15.447366 truss-0.5.1/truss/util/jinja.py
+-rw-r--r--   0        0        0     6040 2023-07-26 21:14:15.447366 truss-0.5.1/truss/util/path.py
+-rw-r--r--   0        0        0     2736 2023-07-26 21:14:15.447366 truss-0.5.1/truss/validation.py
+-rw-r--r--   0        0        0     5343 1970-01-01 00:00:00.000000 truss-0.5.1/PKG-INFO
```

### Comparing `truss-0.5.0/CODE_OF_CONDUCT.md` & `truss-0.5.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/CONTRIBUTING.md` & `truss-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/LICENSE` & `truss-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/README.md` & `truss-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/context_builder.Dockerfile` & `truss-0.5.1/context_builder.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/pyproject.toml` & `truss-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.5.0"
+version = "0.5.1"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = ["MLOps", "AI", "Model Serving", "Model Deployment", "Machine Learning"]
@@ -35,14 +35,16 @@
 psutil = "^5.9.4"
 joblib = "^1.2.0"
 pydantic = "^1.10.9"
 boto3 = "^1.26.157"
 rich = "^13.4.2"
 watchfiles = "^0.19.0"
 huggingface_hub = "^0.16.4"
+rich-click = "^1.6.1"
+inquirerpy = "^0.3.4"
 
 [tool.poetry.group.builder.dependencies]
 python = ">=3.8,<3.12"
 packaging = ">=20.9"
 python-json-logger = ">=2.0.2"
 PyYAML = "^6.0"
 Jinja2 = "^3.1.2"
@@ -78,15 +80,15 @@
 transformers = "^4.20.1"
 black = "^22.6.0"
 nbconvert = "^7.2.1"
 ipykernel = "^6.16.0"
 dockerfile = "^3.2.0"
 
 [tool.poetry.scripts]
-truss = 'truss.cli:cli_group'
+truss = 'truss.cli:truss_cli'
 
 [tool.poetry.group.dev.dependencies]
 mlflow = "^1.29.0"
 mypy = "^1.0.0"
 pytest-split = "^0.8.1"
 httpx = {extras = ["cli"], version = "^0.24.1"}
```

### Comparing `truss-0.5.0/truss/blob/blob_backend_registry.py` & `truss-0.5.1/truss/blob/blob_backend_registry.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/blob/http_public_blob_backend.py` & `truss-0.5.1/truss/blob/http_public_blob_backend.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/build.py` & `truss-0.5.1/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/cli.py` & `truss-0.5.1/truss/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,44 @@
 import json
 import logging
 import os
+import sys
 from functools import wraps
 from pathlib import Path
-from typing import Callable, List, Optional, Union
+from typing import Callable, Optional, Union
 
-import click
+import rich
+import rich_click as click
 import truss
-import yaml
+from truss.remote.remote_cli import inquire_model_name, inquire_remote_name
 from truss.remote.remote_factory import RemoteFactory
 
 logging.basicConfig(level=logging.INFO)
 
 
+click.rich_click.COMMAND_GROUPS = {
+    "truss": [
+        {
+            "name": "Main usage",
+            "commands": ["init", "push", "watch", "predict"],
+            "table_styles": {  # type: ignore
+                "row_styles": ["green"],
+            },
+        },
+        {
+            "name": "Advanced Usage",
+            "commands": ["image", "container", "cleanup"],
+            "table_styles": {  # type: ignore
+                "row_styles": ["yellow"],
+            },
+        },
+    ]
+}
+
+
 def echo_output(f: Callable[..., object]):
     @wraps(f)
     def wrapper(*args, **kwargs):
         click.echo(f(*args, **kwargs))
 
     return wrapper
 
@@ -35,31 +57,34 @@
 def print_help() -> None:
     ctx = click.get_current_context()
     click.echo(ctx.get_help())
 
 
 @click.group(name="truss", invoke_without_command=True)  # type: ignore
 @click.pass_context
-@click.option(
-    "-v",
-    "--version",
-    is_flag=True,
-    show_default=False,
-    default=False,
-    help="Show Truss package version.",
-)
-def cli_group(ctx, version) -> None:
+@click.version_option(truss.version())
+def truss_cli(ctx) -> None:
+    """truss: The simplest way to serve models in production"""
     if not ctx.invoked_subcommand:
-        if version:
-            click.echo(truss.version())
-        else:
-            click.echo(ctx.get_help())
+        click.echo(ctx.get_help())
+
 
+@click.group()
+def container():
+    """Subcommands for truss container"""
+    pass
 
-@cli_group.command()
+
+@click.group()
+def image():
+    """Subcommands for truss image"""
+    pass
+
+
+@truss_cli.command()
 @click.argument("target_directory", required=True)
 @click.option(
     "-s",
     "--skip-confirm",
     is_flag=True,
     show_default=True,
     default=False,
@@ -71,25 +96,25 @@
     is_flag=True,
     show_default=True,
     default=False,
     help="Create a trainable truss.",
 )
 @error_handling
 def init(target_directory, skip_confirm, trainable) -> None:
-    """Initializes an empty Truss directory.
+    """Create a new truss.
 
     TARGET_DIRECTORY: A Truss is created in this directory
     """
     tr_path = Path(target_directory)
     if skip_confirm or click.confirm(f"A Truss will be created at {tr_path}"):
         truss.init(target_directory=target_directory, trainable=trainable)
         click.echo(f"Truss was created in {tr_path}")
 
 
-@cli_group.command()
+@image.command()  # type: ignore
 @click.argument("build_dir")
 @click.argument("target_directory", required=False)
 @error_handling
 def build_context(build_dir, target_directory: str) -> None:
     """
     Create a docker build context for a Truss.
 
@@ -97,43 +122,43 @@
 
     TARGET_DIRECTORY: A Truss directory. If none, use current directory.
     """
     tr = _get_truss_from_directory(target_directory=target_directory)
     tr.docker_build_setup(build_dir=Path(build_dir))
 
 
-@cli_group.command()  # type: ignore
+@image.command()  # type: ignore
 @click.argument("target_directory", required=False)
 @click.argument("build_dir", required=False)
 @error_handling
 @click.option("--tag", help="Docker image tag")
-def build_image(target_directory: str, build_dir: Path, tag) -> None:
+def build(target_directory: str, build_dir: Path, tag) -> None:
     """
     Builds the docker image for a Truss.
 
     TARGET_DIRECTORY: A Truss directory. If none, use current directory.
 
     BUILD_DIR: Image context. If none, a temp directory is created.
     """
     tr = _get_truss_from_directory(target_directory=target_directory)
     if build_dir:
         build_dir = Path(build_dir)
     tr.build_serving_docker_image(build_dir=build_dir, tag=tag)
 
 
-@cli_group.command()
+@image.command()  # type: ignore
 @click.argument("target_directory", required=False)
 @click.argument("build_dir", required=False)
 @click.option("--tag", help="Docker build image tag")
 @click.option("--port", type=int, default=8080, help="Local port used to run image")
 @click.option(
     "--attach", is_flag=True, default=False, help="Flag for attaching the process"
 )
 @error_handling
-def run_image(target_directory: str, build_dir: Path, tag, port, attach) -> None:
+def run(target_directory: str, build_dir: Path, tag, port, attach) -> None:
     """
     Runs the docker image for a Truss.
 
     TARGET_DIRECTORY: A Truss directory. If none, use current directory.
 
     BUILD_DIR: Image context. If none, a temp directory is created.
     """
@@ -144,46 +169,53 @@
     if urls:
         click.confirm(
             f"Container already exists at {urls}. Are you sure you want to continue?"
         )
     tr.docker_run(build_dir=build_dir, tag=tag, local_port=port, detach=not attach)
 
 
-@cli_group.command()
+@truss_cli.command()
 @click.argument("target_directory", required=False, default=os.getcwd())
 @click.option(
     "--remote",
     type=str,
-    required=True,
+    required=False,
     help="Name of the remote in .trussrc to patch changes to",
 )
 @error_handling
 def watch(
     target_directory: str,
     remote: str,
 ) -> None:
     """
-    Watches local truss directory for changes and sends patch requests to remote development truss
+    Seamless remote development with truss
 
     TARGET_DIRECTORY: A Truss directory. If none, use current directory.
     """
 
     # TODO: ensure that provider support draft
+    if not remote:
+        remote = inquire_remote_name(RemoteFactory.get_available_config_names())
+
     remote_provider = RemoteFactory.create(remote=remote)
 
     tr = _get_truss_from_directory(target_directory=target_directory)
     model_name = tr.spec.config.model_name
     if not model_name:
-        raise ValueError("'NoneType' model_name value provided in config.yaml")
+        rich.print(
+            "🧐 NoneType model_name provided in config.yaml. "
+            "Please check that you have the correct model name in your config file."
+        )
+        sys.exit(1)
 
-    click.echo(f"Watching for changes to truss at: {target_directory} ...")
+    rich.print(f"👀 Watching for changes to truss at '{target_directory}' ...")
     remote_provider.sync_truss_to_dev_version_by_name(model_name, target_directory)  # type: ignore
 
 
-@cli_group.command()
+@truss_cli.command()
 @click.option("--target_directory", required=False, help="Directory of truss")
 @click.option(
     "--request",
     type=str,
     required=False,
     help="String formatted as json that represents request",
 )
@@ -214,15 +246,15 @@
     build_dir,
     tag,
     port,
     no_docker,
     request_file,
 ):
     """
-    Invokes the packaged model, either locally or in a Docker container.
+    Invokes the packaged model
 
     TARGET_DIRECTORY: A Truss directory. If none, use current directory.
 
     REQUEST: String formatted as json that represents request
 
     BUILD_DIR: Directory where context is built. If none, a temp directory is created.
 
@@ -247,62 +279,20 @@
         return tr.server_predict(request_data)
     else:
         return tr.docker_predict(
             request_data, build_dir=build_dir, tag=tag, local_port=port, detach=True
         )
 
 
-@cli_group.command()
-@click.option("--target_directory", required=False, help="Directory of truss")
-@click.option(
-    "--build-dir",
-    type=click.Path(exists=True),
-    required=False,
-    help="Directory where context is built",
-)
-@click.option("--tag", help="Docker build image tag")
-@click.option(
-    "--var",
-    multiple=True,
-    help="""Training variables in key=value form where value is string.
-    For more complex values use vars_yaml_file""",
-)
-@click.option(
-    "--vars_yaml_file",
-    required=False,
-    help="Training variables from a yaml file",
-)
-@click.option(
-    "--local",
-    is_flag=True,
-    default=False,
-    help="Flag to run training locally (not on docker)",
-)
-@error_handling
-@echo_output
-def train(target_directory: str, build_dir, tag, var: List[str], vars_yaml_file, local):
-    """Runs prediction for a Truss in a docker image or locally"""
-    tr = _get_truss_from_directory(target_directory=target_directory)
-    if vars_yaml_file is not None:
-        with Path(vars_yaml_file).open() as vars_file:
-            variables = yaml.safe_load(vars_file)
-    else:
-        variables = _variables_dict_from_option(var)
-    if local:
-        return tr.local_train(variables=variables)
-
-    return tr.docker_train(build_dir=build_dir, tag=tag, variables=variables)
-
-
-@cli_group.command()
+@truss_cli.command()
 @click.argument("target_directory", required=False, default=os.getcwd())
 @click.option(
     "--remote",
     type=str,
-    required=True,
+    required=False,
     help="Name of the remote in .trussrc to push to",
 )
 @click.option("--model-name", type=str, required=False, help="Name of the model")
 @click.option(
     "--publish",
     type=bool,
     is_flag=True,
@@ -319,101 +309,71 @@
 ) -> None:
     """
     Pushes a truss to a TrussRemote.
 
     TARGET_DIRECTORY: A Truss directory. If none, use current directory.
 
     """
+    if not remote:
+        remote = inquire_remote_name(RemoteFactory.get_available_config_names())
+
     remote_provider = RemoteFactory.create(remote=remote)
 
     tr = _get_truss_from_directory(target_directory=target_directory)
 
     # Push
     model_name = model_name or tr.spec.config.model_name
-    if model_name is None:
-        raise ValueError(
-            "Model name must be provided either as a flag or in the Truss config"
-        )
+    if not model_name:
+        model_name = inquire_model_name()
 
     # Write model name to config if it's not already there
     if model_name != tr.spec.config.model_name:
         tr.spec.config.model_name = model_name
         tr.spec.config.write_to_yaml_file(tr.spec.config_path, verbose=False)
 
     # TODO(Abu): This needs to be refactored to be more generic
     _ = remote_provider.push(tr, model_name, publish=publish)  # type: ignore
 
     click.echo(f"Model {model_name} was successfully pushed.")
 
 
-@cli_group.command()
+@container.command()  # type: ignore
 @click.argument("target_directory", required=False)
-@click.option("--name", type=str, required=False, help="Name of example to run")
-@click.option(
-    "--local", is_flag=True, default=False, help="Flag to run prediction locally"
-)
 @error_handling
-@echo_output
-def run_example(target_directory: str, name, local):
-    """
-    Runs examples specified in the Truss, over docker.
-
-    TARGET_DIRECTORY: A Truss directory. If none, use current directory.
-    """
-    tr = _get_truss_from_directory(target_directory=target_directory)
-    predict_fn = tr.docker_predict
-    if local:
-        predict_fn = tr.server_predict
-
-    if name is not None:
-        example = tr.example(name)
-        click.echo(f"Running example: {name}")
-        return predict_fn(example.input)
-    else:
-        example_outputs = []
-        for example in tr.examples():
-            click.echo(f"Running example: {example.name}")
-            example_outputs.append(predict_fn(example.input))
-        return example_outputs
-
-
-@cli_group.command()
-@click.argument("target_directory", required=False)
-@error_handling
-def get_container_logs(target_directory) -> None:
+def logs(target_directory) -> None:
     """
     Get logs in a container is running for a truss
 
     TARGET_DIRECTORY: A Truss directory. If none, use current directory.
     """
     for log in _get_truss_from_directory(
         target_directory=target_directory
     ).serving_container_logs():
         click.echo(log)
 
 
-@cli_group.command()  # type: ignore
+@container.command()  # type: ignore
 @click.argument("target_directory", required=False)
 def kill(target_directory: str) -> None:
     """
     Kills containers related to truss.
 
     TARGET_DIRECTORY: A Truss directory. If none, use current directory.
     """
     tr = _get_truss_from_directory(target_directory=target_directory)
     tr.kill_container()
 
 
-@cli_group.command()
+@container.command()  # type: ignore
 def kill_all() -> None:
     "Kills all truss containers that are not manually persisted"
     truss.kill_all()
 
 
-@cli_group.command()
+@truss_cli.command()
 @error_handling
 def cleanup() -> None:
     """
     Clean up truss data.
 
     Truss creates temporary directories for various operations
     such as for building docker images. This command clears
@@ -425,23 +385,12 @@
 def _get_truss_from_directory(target_directory: Optional[str] = None):
     """Gets Truss from directory. If none, use the current directory"""
     if target_directory is None:
         target_directory = os.getcwd()
     return truss.load(target_directory)
 
 
-def _variables_dict_from_option(variables_list: List[str]) -> dict:
-    vars_dict = {}
-    for var in variables_list:
-        first_equals_pos = var.find("=")
-        if first_equals_pos == -1:
-            raise ValueError(
-                f"Training variable expected in `key=value` from but found `{var}`",
-            )
-        var_name = var[:first_equals_pos]
-        var_value = var[first_equals_pos + 1 :]
-        vars_dict[var_name] = var_value
-    return vars_dict
-
+truss_cli.add_command(container)
+truss_cli.add_command(image)
 
 if __name__ == "__main__":
-    cli_group()
+    truss_cli()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `truss-0.5.0/truss/constants.py` & `truss-0.5.1/truss/constants.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/contexts/image_builder/image_builder.py` & `truss-0.5.1/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.5.1/truss/contexts/image_builder/serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/contexts/image_builder/training_image_builder.py` & `truss-0.5.1/truss/contexts/image_builder/training_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/contexts/image_builder/util.py` & `truss-0.5.1/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/contexts/local_loader/docker_build_emulator.py` & `truss-0.5.1/truss/contexts/local_loader/docker_build_emulator.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/contexts/local_loader/load_model_local.py` & `truss-0.5.1/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/contexts/local_loader/train_local.py` & `truss-0.5.1/truss/contexts/local_loader/train_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/contexts/local_loader/truss_file_syncer.py` & `truss-0.5.1/truss/contexts/local_loader/truss_file_syncer.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,11 +22,14 @@
             load_trussignore_patterns(),
         )
 
     def run(self) -> None:
         """Watch for files in background and apply appropriate patches."""
         from watchfiles import watch
 
+        # disable watchfiles logger
+        logging.getLogger("watchfiles.main").disabled = True
+
         for _ in watch(
             self.watch_path, watch_filter=self.watch_filter, raise_interrupt=False
         ):
             self.remote.patch(self.watch_path, self._logger)
```

### Comparing `truss-0.5.0/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.5.1/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/contexts/local_loader/utils.py` & `truss-0.5.1/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/docker.py` & `truss-0.5.1/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/environment_inference/requirements_inference.py` & `truss-0.5.1/truss/environment_inference/requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/errors.py` & `truss-0.5.1/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/local/local_config.py` & `truss-0.5.1/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/local/local_config_handler.py` & `truss-0.5.1/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/model_framework.py` & `truss-0.5.1/truss/model_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/model_frameworks/__init__.py` & `truss-0.5.1/truss/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/model_frameworks/huggingface_transformer.py` & `truss-0.5.1/truss/model_frameworks/huggingface_transformer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/model_frameworks/keras.py` & `truss-0.5.1/truss/model_frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/model_frameworks/lightgbm.py` & `truss-0.5.1/truss/model_frameworks/lightgbm.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/model_frameworks/mlflow.py` & `truss-0.5.1/truss/model_frameworks/mlflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/model_frameworks/pytorch.py` & `truss-0.5.1/truss/model_frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/model_frameworks/sklearn.py` & `truss-0.5.1/truss/model_frameworks/sklearn.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/model_frameworks/xgboost.py` & `truss-0.5.1/truss/model_frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/model_inference.py` & `truss-0.5.1/truss/model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/patch/calc_patch.py` & `truss-0.5.1/truss/patch/calc_patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,28 +83,30 @@
         of view.
         """
         return _strictly_under(path, [data_dir_path])
 
     patches = []
     for path in changed_paths["removed"]:
         if _strictly_under(path, [model_module_path]):
+            logger.info(f"Created patch to remove model code file: {path}")
             patches.append(
                 Patch(
                     type=PatchType.MODEL_CODE,
                     body=ModelCodePatch(
                         action=Action.REMOVE,
                         path=_relative_to(path, model_module_path),
                     ),
                 )
             )
         elif path == CONFIG_FILE:
             # Don't support removal of config file
             logger.info(f"Patching not supported for removing {path}")
             return None
         elif _strictly_under(path, [bundled_packages_path]):
+            logger.info(f"Created patch to remove package file: {path}")
             patches.append(
                 Patch(
                     type=PatchType.PACKAGE,
                     body=PackagePatch(
                         action=Action.REMOVE,
                         path=_relative_to(path, bundled_packages_path),
                     ),
@@ -118,14 +120,17 @@
         action = Action.ADD if path in changed_paths["added"] else Action.UPDATE
         if _strictly_under(path, [model_module_path]):
             full_path = truss_dir / path
 
             # TODO(pankaj) Add support for empty directories, skip them for now.
             if not full_path.is_file():
                 continue
+            logger.info(
+                f"Created patch to {action.value.lower()} model code file: {path}"
+            )
             patches.append(
                 Patch(
                     type=PatchType.MODEL_CODE,
                     body=ModelCodePatch(
                         action=action,
                         path=_relative_to(path, model_module_path),
                         content=full_path.read_text(),
@@ -134,20 +139,22 @@
             )
         elif path == CONFIG_FILE:
             new_config = TrussConfig.from_yaml(truss_dir / CONFIG_FILE)
             prev_config = TrussConfig.from_dict(
                 yaml.safe_load(previous_truss_signature.config)
             )
             config_patches = calc_config_patches(prev_config, new_config)
+            if config_patches:
+                logger.info(f"Created patch to {action.value.lower()} config")
             patches.extend(config_patches)
         elif _strictly_under(path, [bundled_packages_path]):
             full_path = truss_dir / path
             if not full_path.is_file():
                 continue
-
+            logger.info(f"Created patch to {action.value.lower()} package file: {path}")
             patches.append(
                 Patch(
                     type=PatchType.PACKAGE,
                     body=PackagePatch(
                         action=action,
                         path=_relative_to(path, bundled_packages_path),
                         content=full_path.read_text(),
@@ -219,21 +226,24 @@
     prev_config: TrussConfig, new_config: TrussConfig
 ) -> List[Patch]:
     """Calculate patch based on changes to config.
 
     Returns None if patch cannot be calculated. Empty list means no relevant
     differences found.
     """
-
-    config_patches = _calc_general_config_patches(prev_config, new_config)
-    python_requirement_patches = _calc_python_requirements_patches(
-        prev_config, new_config
-    )
-    system_package_patches = _calc_system_packages_patches(prev_config, new_config)
-    return [*config_patches, *python_requirement_patches, *system_package_patches]
+    try:
+        config_patches = _calc_general_config_patches(prev_config, new_config)
+        python_requirement_patches = _calc_python_requirements_patches(
+            prev_config, new_config
+        )
+        system_package_patches = _calc_system_packages_patches(prev_config, new_config)
+        return [*config_patches, *python_requirement_patches, *system_package_patches]
+    except Exception as e:
+        logger.error(f"Failed to calculate config patch with exception: {e}")
+        raise
 
 
 def _calc_general_config_patches(
     prev_config: TrussConfig, new_config: TrussConfig
 ) -> List[Patch]:
     """Calculate patch based on changes to config.yaml
     If a change has been made to the config, at least one ConfigPatch is created
```

### Comparing `truss-0.5.0/truss/patch/dir_signature.py` & `truss-0.5.1/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/patch/hash.py` & `truss-0.5.1/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/patch/local_truss_patch_applier.py` & `truss-0.5.1/truss/patch/local_truss_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/patch/truss_dir_patch_applier.py` & `truss-0.5.1/truss/patch/truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/patch/types.py` & `truss-0.5.1/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/readme_generator.py` & `truss-0.5.1/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/remote/baseten/api.py` & `truss-0.5.1/truss/remote/baseten/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from typing import Optional
 
 import requests
 from truss.remote.baseten.auth import AuthService
 from truss.remote.baseten.error import ApiError
 from truss.remote.baseten.utils.transfer import base64_encoded_json_str
 
 logger = logging.getLogger(__name__)
@@ -60,32 +61,40 @@
         self,
         model_name,
         s3_key,
         config,
         semver_bump,
         client_version,
         is_trusted=False,
+        model_id: Optional[str] = None,
     ):
+        if model_id:
+            mutation = "create_model_version_from_truss"
+            first_arg = f'model_id: "{model_id}"'
+        else:
+            mutation = "create_model_from_truss"
+            first_arg = f'name: "{model_name}"'
+
         query_string = f"""
         mutation {{
-        create_model_from_truss(name: "{model_name}",
+        {mutation}({first_arg},
                     s3_key: "{s3_key}",
                     config: "{config}",
                     semver_bump: "{semver_bump}",
                     client_version: "{client_version}",
                     is_trusted: {'true' if is_trusted else 'false'}
     ) {{
             id,
             name,
             version_id
         }}
         }}
         """
         resp = self._post_graphql_query(query_string)
-        return resp["data"]["create_model_from_truss"]
+        return resp["data"][mutation]
 
     def create_development_model_from_truss(
         self,
         model_name,
         s3_key,
         config,
         client_version,
```

### Comparing `truss-0.5.0/truss/remote/baseten/auth.py` & `truss-0.5.1/truss/remote/baseten/auth.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/remote/baseten/core.py` & `truss-0.5.1/truss/remote/baseten/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 from truss.remote.baseten.utils.tar import create_tar_with_progress_bar
 from truss.remote.baseten.utils.transfer import multipart_upload_boto3
 from truss.truss_handle import TrussHandle
 
 logger = logging.getLogger(__name__)
 
 
-def exists_model(api: BasetenApi, model_name: str) -> bool:
+def exists_model(api: BasetenApi, model_name: str) -> Optional[str]:
     """
     Check if a model with the given name exists in the Baseten remote.
 
     Args:
         api: BasetenApi instance
         model_name: Name of the model to check for existence
 
     Returns:
-        True if the model exists, False otherwise
+        model_id if present, otherwise None
     """
     models = api.models()
     for model in models["models"]:
         if model["name"] == model_name:
-            return True
-    return False
+            return model["id"]
+    return None
 
 
 def get_dev_version_info(api: BasetenApi, model_name: str) -> dict:
     model = api.get_model(model_name)
     versions = model["model_version"]["oracle"]["versions"]
     for version in versions:
         if version["is_draft"] is True:
@@ -81,14 +81,15 @@
     api: BasetenApi,
     model_name: str,
     s3_key: str,
     config: str,
     semver_bump: Optional[str] = "MINOR",
     is_trusted: Optional[bool] = False,
     is_draft: Optional[bool] = False,
+    model_id: Optional[str] = None,
 ) -> Tuple[str, str]:
     """
     Create a model in the Baseten remote.
 
     Args:
         api: BasetenApi instance
         model_name: Name of the model to create
@@ -112,10 +113,11 @@
         model_version_json = api.create_model_from_truss(
             model_name,
             s3_key,
             config,
             semver_bump,
             f"truss=={truss.version()}",
             is_trusted,
+            model_id,
         )
 
     return (model_version_json["id"], model_version_json["version_id"])
```

### Comparing `truss-0.5.0/truss/remote/baseten/error.py` & `truss-0.5.1/truss/remote/baseten/error.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/remote/baseten/remote.py` & `truss-0.5.1/truss/remote/baseten/remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 from pathlib import Path
 
 import yaml
 from truss.contexts.local_loader.truss_file_syncer import TrussFilesSyncer
 from truss.local.local_config_handler import LocalConfigHandler
-from truss.patch.constants import PATCHABLE_STATUSES
 from truss.remote.baseten.api import BasetenApi
 from truss.remote.baseten.auth import AuthService
 from truss.remote.baseten.core import (
     archive_truss,
     create_truss_service,
     exists_model,
     get_dev_version_info,
@@ -29,42 +28,47 @@
     def authenticate(self):
         return self._auth_service.validate()
 
     def push(self, truss_handle: TrussHandle, model_name: str, publish: bool = True):  # type: ignore
         if model_name.isspace():
             raise ValueError("Model name cannot be empty")
 
-        if exists_model(self._api, model_name):
-            raise ValueError(f"Model with name {model_name} already exists")
+        model_id = exists_model(self._api, model_name)
 
         gathered_truss = TrussHandle(truss_handle.gather())
         encoded_config_str = base64_encoded_json_str(
             gathered_truss._spec._config.to_dict()
         )
 
         temp_file = archive_truss(gathered_truss)
         s3_key = upload_truss(self._api, temp_file)
+
         model_id, model_version_id = create_truss_service(
             api=self._api,
             model_name=model_name,
             s3_key=s3_key,
             config=encoded_config_str,
             is_draft=not publish,
+            model_id=model_id,
         )
 
         return BasetenService(
             model_id=model_id,
             model_version_id=model_version_id,
             is_draft=not publish,
             api_key=self._auth_service.authenticate().value,
             service_url=f"{self._remote_url}/model_versions/{model_version_id}",
             truss_handle=truss_handle,
         )
 
-    def sync_truss_to_dev_version_by_name(self, model_name: str, target_directory: str):
+    def sync_truss_to_dev_version_by_name(
+        self,
+        model_name: str,
+        target_directory: str,
+    ):
         # verify that development deployment exists for given model name
         _ = get_dev_version_info(
             self._api, model_name  # pylint: disable=protected-access
         )
         TrussFilesSyncer(
             Path(target_directory),
             self,
@@ -72,37 +76,40 @@
 
         # Since the `TrussFilesSyncer` runs a daemon thread, we run this infinite loop on the main
         # thread to keep it alive. When this loop is interrupted by the user, then the whole process
         # can shutdown gracefully.
         while True:
             pass
 
-    def patch(self, watch_path: Path, logger: logging.Logger):
+    def patch(
+        self,
+        watch_path: Path,
+        logger: logging.Logger,
+    ):
         try:
             truss_handle = TrussHandle(watch_path)
         except yaml.parser.ParserError:
-            logger.error("Unable to parse config file.")
+            logger.error("Unable to parse config file")
             return
         model_name = truss_handle.spec.config.model_name
         dev_version = get_dev_version_info(self._api, model_name)  # type: ignore
         truss_hash = dev_version.get("truss_hash", None)
         truss_signature = dev_version.get("truss_signature", None)
         LocalConfigHandler.add_signature(truss_hash, truss_signature)
-        patch_request = truss_handle.calc_patch(truss_hash)
+        try:
+            patch_request = truss_handle.calc_patch(truss_hash)
+        except Exception:
+            logger.error("Failed to calculate patch")
+            return
         if patch_request:
             if (
                 patch_request.prev_hash == patch_request.next_hash
                 or len(patch_request.patch_ops) == 0
             ):
                 logger.info("No changes observed, skipping deployment")
-            model_deployment_status = dev_version.get(
-                "current_model_deployment_status", None
-            ).get("status", None)
-            if model_deployment_status not in PATCHABLE_STATUSES:
-                logger.info(f"Model {model_name} is not ready for patching")
             resp = self._api.patch_draft_truss(model_name, patch_request)
             if not resp["succeeded"]:
                 needs_full_deploy = resp.get("needs_full_deploy", None)
                 if needs_full_deploy:
                     logger.info(
                         f"Model {model_name} is not able to be patched, use `truss push` to deploy"
                     )
```

### Comparing `truss-0.5.0/truss/remote/baseten/service.py` & `truss-0.5.1/truss/remote/baseten/service.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/remote/baseten/utils/tar.py` & `truss-0.5.1/truss/remote/baseten/utils/tar.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/remote/baseten/utils/transfer.py` & `truss-0.5.1/truss/remote/baseten/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/remote/remote_factory.py` & `truss-0.5.1/truss/remote/remote_factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,69 @@
-import configparser
 import inspect
+from configparser import DEFAULTSECT, SafeConfigParser
+from functools import partial
+from operator import is_not
 from pathlib import Path
-from typing import Dict, Type
+from typing import Dict, List, Type
 
 from truss.remote.baseten import BasetenRemote
-from truss.remote.truss_remote import TrussRemote
+from truss.remote.truss_remote import RemoteConfig, TrussRemote
+
+USER_TRUSSRC_PATH = Path("~/.trussrc").expanduser()
+
+
+def load_config() -> SafeConfigParser:
+    config = SafeConfigParser()
+    config.read(USER_TRUSSRC_PATH)
+    return config
+
+
+def update_config(config: SafeConfigParser):
+    with open(USER_TRUSSRC_PATH, "w") as configfile:
+        config.write(configfile)
 
 
 class RemoteFactory:
     """
     A factory for instantiating a TrussRemote from a .trussrc file and a user-specified remote config name
     """
 
     REGISTRY: Dict[str, Type[TrussRemote]] = {"baseten": BasetenRemote}
 
     @staticmethod
-    def load_remote_config(remote_name: str) -> Dict:
+    def get_available_config_names() -> List[str]:
+        if not USER_TRUSSRC_PATH.exists():
+            return []
+
+        config = load_config()
+        return list(filter(partial(is_not, DEFAULTSECT), config.keys()))
+
+    @staticmethod
+    def load_remote_config(remote_name: str) -> RemoteConfig:
         """
         Load and validate a remote config from the .trussrc file
         """
-        config_path = Path("~/.trussrc").expanduser()
-
-        if not config_path.exists():
-            raise FileNotFoundError(f"No .trussrc file found at {config_path}")
+        if not USER_TRUSSRC_PATH.exists():
+            raise FileNotFoundError("No ~/.trussrc file found.")
 
-        config = configparser.ConfigParser()
-        config.read(config_path)
+        config = load_config()
 
         if remote_name not in config:
-            raise ValueError(f"Service provider {remote_name} not found in .trussrc")
+            raise ValueError(f"Service provider {remote_name} not found in ~/.trussrc")
 
-        return dict(config[remote_name])
+        return RemoteConfig(name=remote_name, configs=dict(config[remote_name]))
+
+    @staticmethod
+    def update_remote_config(remote_config: RemoteConfig):
+        """
+        Load and validate a remote config from the .trussrc file
+        """
+        config = load_config()
+        config[remote_config.name] = remote_config.configs
+        update_config(config)
 
     @staticmethod
     def validate_remote_config(remote_config: Dict, remote_name: str):
         """
         Validates remote config by checking
             1. the 'remote' field exists
             2. all required parameters for the 'remote' class are provided
@@ -72,21 +101,21 @@
             and name not in {"self", "args", "kwargs"}
         }
         return required_params
 
     @classmethod
     def create(cls, remote: str) -> TrussRemote:
         remote_config = cls.load_remote_config(remote)
-        cls.validate_remote_config(remote_config, remote)
+        configs = remote_config.configs
+        cls.validate_remote_config(configs, remote)
 
-        remote_class = cls.REGISTRY[remote_config.pop("remote_provider")]
+        remote_class = cls.REGISTRY[configs.pop("remote_provider")]
         remote_params = {
-            param: remote_config.get(param)
-            for param in cls.required_params(remote_class)
+            param: configs.get(param) for param in cls.required_params(remote_class)
         }
 
         # Add any additional params provided by the user in their .trussrc
-        additional_params = set(remote_config.keys()) - set(remote_params.keys())
+        additional_params = set(configs.keys()) - set(remote_params.keys())
         for param in additional_params:
-            remote_params[param] = remote_config.get(param)
+            remote_params[param] = configs.get(param)
 
         return remote_class(**remote_params)  # type: ignore
```

### Comparing `truss-0.5.0/truss/remote/truss_remote.py` & `truss-0.5.1/truss/remote/truss_remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+from dataclasses import dataclass, field
 from typing import Dict, Optional
 
 import requests
 from truss.truss_handle import TrussHandle
 
 
 class TrussService(ABC):
@@ -182,7 +183,15 @@
         the user has valid authentication credentials to push to the remote service.
         If not, it should raise an exception.
 
         Args:
             **kwargs: Additional keyword arguments for the authentication operation.
         """
         pass
+
+
+@dataclass
+class RemoteConfig:
+    """Class to hold configs for various remotes"""
+
+    name: str
+    configs: Dict = field(default_factory=dict)
```

### Comparing `truss-0.5.0/truss/templates/README.md.jinja` & `truss-0.5.1/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/base.Dockerfile.jinja` & `truss-0.5.1/truss/templates/base.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/control/control/application.py` & `truss-0.5.1/truss/templates/control/control/application.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/control/control/endpoints.py` & `truss-0.5.1/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/control/control/helpers/errors.py` & `truss-0.5.1/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.5.1/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.5.1/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.5.1/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/control/control/helpers/truss_patch/__init__.py` & `truss-0.5.1/truss/templates/control/control/helpers/truss_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py` & `truss-0.5.1/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py` & `truss-0.5.1/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py` & `truss-0.5.1/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/control/control/helpers/types.py` & `truss-0.5.1/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/control/control/server.py` & `truss-0.5.1/truss/templates/control/control/server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/custom/model/model.py` & `truss-0.5.1/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/huggingface_transformer/model/model.py` & `truss-0.5.1/truss/templates/huggingface_transformer/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/keras/model/model.py` & `truss-0.5.1/truss/templates/keras/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/lightgbm/model/model.py` & `truss-0.5.1/truss/templates/lightgbm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/mlflow/model/model.py` & `truss-0.5.1/truss/templates/mlflow/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/pytorch/model/model.py` & `truss-0.5.1/truss/templates/pytorch/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/server/common/errors.py` & `truss-0.5.1/truss/templates/server/common/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/server/common/patches/whisper/patch.py` & `truss-0.5.1/truss/templates/server/common/patches/whisper/patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/server/common/patches.py` & `truss-0.5.1/truss/templates/server/common/patches.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/server/common/retry.py` & `truss-0.5.1/truss/templates/server/common/retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/server/common/termination_handler_middleware.py` & `truss-0.5.1/truss/templates/server/common/termination_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/server/common/truss_server.py` & `truss-0.5.1/truss/templates/server/common/truss_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import signal
 import socket
 import sys
 import time
 from collections.abc import Generator
 from pathlib import Path
-from typing import Dict, List, Optional, Union
+from typing import AsyncGenerator, Dict, List, Optional, Union
 
 import common.errors as errors
 import shared.util as utils
 import uvicorn
 from common.termination_handler_middleware import TerminationHandlerMiddleware
 from fastapi import Depends, FastAPI, Request
 from fastapi.responses import ORJSONResponse, StreamingResponse
@@ -103,23 +103,23 @@
         """
         if self._model is None:
             raise errors.ModelMissingError("model")
         self.check_healthy(self._model)
 
         return {}
 
-    def invocations(
+    async def invocations(
         self, request: Request, body_raw: bytes = Depends(parse_body)
     ) -> Response:
         """
         This method provides compatibility with Sagemaker hosting for the 'invocations' endpoint.
         """
-        return self.predict(self._model.name, request, body_raw)
+        return await self.predict(self._model.name, request, body_raw)
 
-    def predict(
+    async def predict(
         self, model_name: str, request: Request, body_raw: bytes = Depends(parse_body)
     ) -> Response:
         """
         This method is called by FastAPI, which introspects that it's not async, and schedules it on a thread
         """
         model: ModelWrapper = self._safe_lookup_model(model_name)
 
@@ -128,24 +128,22 @@
         body: Dict
         if self.is_binary(request):
             body = truss_msgpack_deserialize(body_raw)
         else:
             body = json.loads(body_raw)
 
         # calls ModelWrapper.__call__, which runs validate, preprocess, predict, and postprocess
-        response: Union[Dict, Generator] = asyncio.run(
-            model(
-                body,
-                headers=utils.transform_keys(request.headers, lambda key: key.lower()),
-            )
+        response: Union[Dict, Generator] = await model(
+            body,
+            headers=utils.transform_keys(request.headers, lambda key: key.lower()),
         )
 
         # In the case that the model returns a Generator object, return a
         # StreamingResponse instead.
-        if isinstance(response, Generator):
+        if isinstance(response, AsyncGenerator):
             # media_type in StreamingResponse sets the Content-Type header
             return StreamingResponse(response, media_type="application/octet-stream")
 
         response_headers = {}
         if self.is_binary(request):
             response_headers["Content-Type"] = "application/octet-stream"
             return Response(
```

### Comparing `truss-0.5.0/truss/templates/server/inference_server.py` & `truss-0.5.1/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/server/model_wrapper.py` & `truss-0.5.1/truss/templates/server/model_wrapper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+import asyncio
 import importlib
 import inspect
 import logging
 import os
 import sys
 import time
 import traceback
 from collections.abc import Generator
 from enum import Enum
 from pathlib import Path
-from queue import Queue
 from threading import Lock, Thread
-from typing import Any, Dict, Optional, Union
+from typing import Any, AsyncGenerator, Dict, Optional, Set, Union
 
-from anyio import to_thread
+from anyio import Semaphore, to_thread
 from common.patches import apply_patches
 from common.retry import retry
 from shared.secrets_resolver import SecretsResolver
 
 MODEL_BASENAME = "model"
 
 NUM_LOAD_RETRIES = int(os.environ.get("NUM_LOAD_RETRIES_TRUSS", "3"))
 STREAMING_RESPONSE_QUEUE_READ_TIMEOUT_SECS = 60
+DEFAULT_PREDICT_CONCURRENCY = 1
 
 
 class ModelWrapper:
     class Status(Enum):
         NOT_READY = 0
         LOADING = 1
         READY = 2
@@ -32,16 +33,21 @@
 
     def __init__(self, config: Dict):
         self._config = config
         self._logger = logging.getLogger()
         self.name = MODEL_BASENAME
         self.ready = False
         self._load_lock = Lock()
-        self._predict_lock = Lock()
         self._status = ModelWrapper.Status.NOT_READY
+        self._predict_semaphore = Semaphore(
+            self._config.get("runtime", {}).get(
+                "predict_concurrency", DEFAULT_PREDICT_CONCURRENCY
+            )
+        )
+        self._background_tasks: Set[asyncio.Task] = set()
 
     def load(self) -> bool:
         if self.ready:
             return self.ready
 
         # if we are already loading, just pass; our container will return 503 while we're loading
         if not self._load_lock.acquire(blocking=False):
@@ -119,42 +125,95 @@
                 self._model.load,
                 NUM_LOAD_RETRIES,
                 self._logger.warn,
                 "Failed to load model.",
                 gap_seconds=1.0,
             )
 
-    def preprocess(
+    async def preprocess(
         self,
         payload: Any,
         headers: Optional[Dict[str, str]] = None,
     ) -> Any:
         if not hasattr(self._model, "preprocess"):
             return payload
-        return self._model.preprocess(payload)  # type: ignore
 
-    def postprocess(
+        if inspect.iscoroutinefunction(self._model.preprocess):
+            return await self._model.preprocess(payload)
+        else:
+            return await to_thread.run_sync(self._model.preprocess, payload)
+
+    def _predict_sync_with_error_handling(self, payload):
+        try:
+            return self._model.predict(payload)
+        except Exception:
+            logging.exception("Exception while running predict")
+            return {"error": {"traceback": traceback.format_exc()}}
+
+    async def _predict_async_with_error_handling(self, payload):
+        try:
+            return await self._model.predict(payload)
+        except Exception:
+            logging.exception("Exception while running predict")
+            return {"error": {"traceback": traceback.format_exc()}}
+
+    async def predict(
         self,
-        response: Any,
+        payload: Any,
         headers: Optional[Dict[str, str]] = None,
     ) -> Any:
-        if not hasattr(self._model, "postprocess"):
-            return response
-        return self._model.postprocess(response)  # type: ignore
+        # It's possible for the user's predict function to be a:
+        #   1. Generator function (function that returns a generator)
+        #   2. Async generator (function that returns async generator)
+        # In these cases, just return the generator or async generator,
+        # as we will be propagating these up. No need for await at this point.
+        #   3. Coroutine -- in this case, await the predict function as it is async
+        #   4. Normal function -- in this case, offload to a separate thread to prevent
+        #      blocking the main event loop
+        if inspect.isasyncgenfunction(
+            self._model.predict
+        ) or inspect.isgeneratorfunction(self._model.predict):
+            return self._model.predict(payload)
+
+        if inspect.iscoroutinefunction(self._model.predict):
+            return await self._predict_async_with_error_handling(payload)
 
-    def predict(
+        return await to_thread.run_sync(self._predict_sync_with_error_handling, payload)
+
+    async def postprocess(
         self,
-        payload: Any,
+        response: Any,
         headers: Optional[Dict[str, str]] = None,
     ) -> Any:
-        try:
-            return self._model.predict(payload)  # type: ignore
-        except Exception:
-            logging.exception("Exception while running predict")
-            return {"error": {"traceback": traceback.format_exc()}}
+        # Similar to the predict function, it is possible for postprocess
+        # to return either a generator or async generator, in which case
+        # just return the generator.
+        #
+        # It can also return a coroutine or just be a function, in which
+        # case either await, or offload to a thread respectively.
+        if not hasattr(self._model, "postprocess"):
+            return response
+
+        if inspect.isasyncgenfunction(
+            self._model.postprocess
+        ) or inspect.isgeneratorfunction(self._model.postprocess):
+            return self._model.postprocess(response, headers)
+
+        if inspect.iscoroutinefunction(self._model.postprocess):
+            return await self._model.postprocess(response)
+
+        return await to_thread.run_sync(self._model.postprocess, response)
+
+    async def write_response_to_queue(
+        self, queue: asyncio.Queue, generator: AsyncGenerator
+    ):
+        async for chunk in generator:
+            await queue.put(ResponseChunk(chunk))
+
+        await queue.put(None)
 
     async def __call__(
         self, body: Any, headers: Optional[Dict[str, str]] = None
     ) -> Union[Dict, Generator]:
         """Method to call predictor or explainer with the given input.
 
         Args:
@@ -162,87 +221,92 @@
             headers (Dict): Request headers.
 
         Returns:
             Dict: Response output from preprocess -> predictor -> postprocess
             Generator: In case of streaming response
         """
 
-        payload = (
-            await self.preprocess(body, headers)
-            if inspect.iscoroutinefunction(self.preprocess)
-            else self.preprocess(body, headers)
-        )
+        payload = await self.preprocess(body, headers)
 
-        return await to_thread.run_sync(self._predict_and_post, payload, headers)
+        async with self._predict_semaphore:
+            response = await self.predict(payload, headers)
 
-    def _predict_and_post(
-        self,
-        payload: Any,
-        headers: Optional[Dict[str, str]] = None,
-    ) -> Any:
-        self._predict_lock.acquire()
-        defer_lock_release = False
-        try:
-            response = self.predict(payload, headers)
-            response = self.postprocess(response, headers)
-            if not isinstance(response, Generator):
-                return response
-
-            # Generator response
-            if headers and headers.get("accept") == "application/json":
-                return _convert_streamed_response_to_string(response)
+            processed_response = await self.postprocess(response)
 
-            # Reaching here means streaming response, and need to defer releasing lock
-            defer_lock_release = True
-        finally:
-            if not defer_lock_release:
-                self._predict_lock.release()
+            # Streaming cases
+            if inspect.isgenerator(response) or inspect.isasyncgen(response):
+                async_generator = _force_async_generator(response)
+
+                if headers and headers.get("accept") == "application/json":
+                    # In the case of a streaming response, consume stream
+                    # if the http accept header is set, and json is requested.
+                    return await _convert_streamed_response_to_string(async_generator)
+
+                # To ensure that a partial read from a client does not cause the semaphore
+                # to stay claimed, we immediately write all of the data from the stream to a
+                # queue. We then return a new generator that reads from the queue, and then
+                # exit the semaphore block.
+                response_queue: asyncio.Queue = asyncio.Queue()
+
+                # This task will be triggered and run in the background.
+                task = asyncio.create_task(
+                    self.write_response_to_queue(response_queue, async_generator)
+                )
+                self._background_tasks.add(task)
+
+                task.add_done_callback(self._background_tasks.discard)
+
+                async def _response_generator():
+                    while True:
+                        chunk = await asyncio.wait_for(
+                            response_queue.get(),
+                            timeout=STREAMING_RESPONSE_QUEUE_READ_TIMEOUT_SECS,
+                        )
+                        if chunk is None:
+                            return
+                        yield chunk.value
 
-        # Streaming response
-        response_queue: Queue = Queue()
+                return _response_generator()
 
-        def queue_response_chunks():
-            # In a background thread, write the response chunks to a queue.
-            # In the main thread, read data from the queue until a "None"
-            # is written. This allows to us to use the predict lock only
-            # around the actual predict, and does not create a dependency
-            # on the client reading the entire response before releasing
-            # the lock.
-            try:
-                for chunk in response:
-                    response_queue.put(ResponseChunk(chunk))
-                response_queue.put(None)
-            finally:
-                self._predict_lock.release()
-
-        response_generate_thread = Thread(target=queue_response_chunks)
-        response_generate_thread.start()
-        return _response_generator(response_queue)
+            return processed_response
 
 
 class ResponseChunk:
     def __init__(self, value):
         self.value = value
 
 
-def _response_generator(queue: Queue):
+async def _convert_streamed_response_to_string(response: AsyncGenerator):
+    return "".join([str(chunk) async for chunk in response])
+
+
+def _force_async_generator(gen: Union[Generator, AsyncGenerator]) -> AsyncGenerator:
     """
-    When returning the stream result, simply read from the response queue until a `None`
-    is reached.
+    Takes a generator, and converts it into an async generator if it is not already.
     """
-    while True:
-        chunk = queue.get(timeout=STREAMING_RESPONSE_QUEUE_READ_TIMEOUT_SECS)
-        if chunk is None:
-            return
-        else:
-            yield chunk.value
+    if inspect.isasyncgen(gen):
+        return gen
 
+    async def _convert_generator_to_async():
+        """
+        Runs each iteration of the generator in an offloaded thread, to ensure
+        the main loop is not blocked, and yield to create an async generator.
+        """
+        FINAL_GENERATOR_VALUE = object()
+        while True:
+            # Note that this is the equivalent of running:
+            # next(gen, FINAL_GENERATOR_VALUE) on a separate thread,
+            # ensuring that if there is anything blocking in the generator,
+            # it does not block the main loop.
+            chunk = await to_thread.run_sync(next, gen, FINAL_GENERATOR_VALUE)
+            if chunk == FINAL_GENERATOR_VALUE:
+                break
+            yield chunk
 
-def _convert_streamed_response_to_string(response: Any):
-    return "".join([str(chunk) for chunk in list(response)])
+    return _convert_generator_to_async()
 
 
 def _signature_accepts_keyword_arg(signature: inspect.Signature, kwarg: str) -> bool:
     return kwarg in signature.parameters or _signature_accepts_kwargs(signature)
 
 
 def _signature_accepts_kwargs(signature: inspect.Signature) -> bool:
```

### Comparing `truss-0.5.0/truss/templates/server.Dockerfile.jinja` & `truss-0.5.1/truss/templates/server.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/shared/logging.py` & `truss-0.5.1/truss/templates/shared/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/shared/secrets_resolver.py` & `truss-0.5.1/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/shared/serialization.py` & `truss-0.5.1/truss/templates/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/shared/util.py` & `truss-0.5.1/truss/templates/shared/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/sklearn/model/model.py` & `truss-0.5.1/truss/templates/sklearn/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/training/job.py` & `truss-0.5.1/truss/templates/training/job.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/templates/xgboost/model/model.py` & `truss-0.5.1/truss/templates/xgboost/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/auto-mpg.data` & `truss-0.5.1/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/happy.ipynb` & `truss-0.5.1/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/model_load_failure_test/config.yaml` & `truss-0.5.1/truss/test_data/model_load_failure_test/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/model_load_failure_test/model/model.py` & `truss-0.5.1/truss/test_data/model_load_failure_test/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/patch_ping_test_server/app.py` & `truss-0.5.1/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/pima-indians-diabetes.csv` & `truss-0.5.1/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/readme_int_example.md` & `truss-0.5.1/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/readme_no_example.md` & `truss-0.5.1/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/readme_str_example.md` & `truss-0.5.1/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/server.Dockerfile` & `truss-0.5.1/truss/test_data/server.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/server_conformance_test_truss/config.yaml` & `truss-0.5.1/truss/test_data/server_conformance_test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/server_conformance_test_truss/model/model.py` & `truss-0.5.1/truss/test_data/server_conformance_test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/test_streaming_truss/config.yaml` & `truss-0.5.1/truss/test_data/test_async_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/test_streaming_truss/model/model.py` & `truss-0.5.1/truss/test_data/test_streaming_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/test_truss/config.yaml` & `truss-0.5.1/truss/test_data/test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/test_data/test_truss/model/model.py` & `truss-0.5.1/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/conftest.py` & `truss-0.5.1/truss/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/contexts/image_builder/test_serving_image_builder.py` & `truss-0.5.1/truss/tests/contexts/image_builder/test_serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.5.1/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.5.1/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/environments_inference/test_requirements_inference.py` & `truss-0.5.1/truss/tests/environments_inference/test_requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/local/test_local_config_handler.py` & `truss-0.5.1/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/model_frameworks/test_huggingface_transformer_framework.py` & `truss-0.5.1/truss/tests/model_frameworks/test_huggingface_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/model_frameworks/test_keras_framework.py` & `truss-0.5.1/truss/tests/model_frameworks/test_keras_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/model_frameworks/test_lightgbm_framework.py` & `truss-0.5.1/truss/tests/model_frameworks/test_lightgbm_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/model_frameworks/test_pytorch_framework.py` & `truss-0.5.1/truss/tests/model_frameworks/test_pytorch_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/model_frameworks/test_sklearn_framework.py` & `truss-0.5.1/truss/tests/model_frameworks/test_sklearn_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/model_frameworks/test_xgboost_framework.py` & `truss-0.5.1/truss/tests/model_frameworks/test_xgboost_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/patch/test_calc_patch.py` & `truss-0.5.1/truss/tests/patch/test_calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/patch/test_hash.py` & `truss-0.5.1/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/patch/test_truss_dir_patch_applier.py` & `truss-0.5.1/truss/tests/patch/test_truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/remote/baseten/test_api.py` & `truss-0.5.1/truss/tests/remote/baseten/test_api.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/remote/baseten/test_auth.py` & `truss-0.5.1/truss/tests/remote/baseten/test_auth.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/remote/baseten/test_core.py` & `truss-0.5.1/truss/tests/remote/baseten/test_core.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/remote/test_remote_factory.py` & `truss-0.5.1/truss/tests/remote/test_remote_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest import mock
 
 import pytest
 from truss.remote.remote_factory import RemoteFactory
-from truss.remote.truss_remote import TrussRemote
+from truss.remote.truss_remote import RemoteConfig, TrussRemote
 
 SAMPLE_CONFIG = {"api_key": "test_key", "remote_url": "http://test.com"}
 
 SAMPLE_TRUSSRC = """
 [test]
 remote_provider=test_remote
 api_key=test_key
@@ -34,19 +34,25 @@
         return {"Authorization": self.api_key}
 
     def push(self):
         return {"status": "success"}
 
 
 def mock_service_config():
-    return {"remote_provider": "test_remote", **SAMPLE_CONFIG}
+    return RemoteConfig(
+        name="mock-service",
+        configs={"remote_provider": "test_remote", **SAMPLE_CONFIG},
+    )
 
 
 def mock_incorrect_service_config():
-    return {"remote_provider": "nonexistent_remote", **SAMPLE_CONFIG}
+    return RemoteConfig(
+        name="mock-incorrect-service",
+        configs={"remote_provider": "nonexistent_remote", **SAMPLE_CONFIG},
+    )
 
 
 @mock.patch.dict(RemoteFactory.REGISTRY, {"test_remote": TestRemote}, clear=True)
 @mock.patch(
     "truss.remote.remote_factory.RemoteFactory.load_remote_config",
     return_value=mock_service_config(),
 )
@@ -69,15 +75,16 @@
 
 
 @mock.patch.dict(RemoteFactory.REGISTRY, {"test_remote": TestRemote}, clear=True)
 @mock.patch("builtins.open", new_callable=mock.mock_open, read_data=SAMPLE_TRUSSRC)
 @mock.patch("pathlib.Path.exists", return_value=True)
 def test_load_remote_config(mock_exists, mock_open):
     service = RemoteFactory.load_remote_config("test")
-    assert service == {"remote_provider": "test_remote", **SAMPLE_CONFIG}
+    assert service.name == "test"
+    assert service.configs == {"remote_provider": "test_remote", **SAMPLE_CONFIG}
 
 
 @mock.patch.dict(RemoteFactory.REGISTRY, {"test_remote": TestRemote}, clear=True)
 @mock.patch("builtins.open", new_callable=mock.mock_open, read_data=SAMPLE_TRUSSRC)
 @mock.patch("pathlib.Path.exists", return_value=False)
 def test_load_remote_config_no_file(mock_exists, mock_open):
     with pytest.raises(FileNotFoundError):
@@ -100,21 +107,21 @@
 
 @mock.patch.dict(RemoteFactory.REGISTRY, {"test_remote": TestRemote}, clear=True)
 @mock.patch(
     "builtins.open", new_callable=mock.mock_open, read_data=SAMPLE_TRUSSRC_NO_REMOTE
 )
 @mock.patch("pathlib.Path.exists", return_value=True)
 def test_validate_remote_config_no_remote(mock_exists, mock_open):
+    service = RemoteFactory.load_remote_config("test")
     with pytest.raises(ValueError):
-        service = RemoteFactory.load_remote_config("test")
-        RemoteFactory.validate_remote_config(service, "test")
+        RemoteFactory.validate_remote_config(service.configs, "test")
 
 
 @mock.patch.dict(RemoteFactory.REGISTRY, {"test_remote": TestRemote}, clear=True)
 @mock.patch(
     "builtins.open", new_callable=mock.mock_open, read_data=SAMPLE_TRUSSRC_NO_PARAMS
 )
 @mock.patch("pathlib.Path.exists", return_value=True)
 def test_load_remote_config_no_params(mock_exists, mock_open):
+    service = RemoteFactory.load_remote_config("test")
     with pytest.raises(ValueError):
-        service = RemoteFactory.load_remote_config("test")
-        RemoteFactory.validate_remote_config(service, "test")
+        RemoteFactory.validate_remote_config(service.configs, "test")
```

### Comparing `truss-0.5.0/truss/tests/remote/test_truss_remote.py` & `truss-0.5.1/truss/tests/remote/test_truss_remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/samples.py` & `truss-0.5.1/truss/tests/samples.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py` & `truss-0.5.1/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py` & `truss-0.5.1/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/templates/control/control/test_server.py` & `truss-0.5.1/truss/tests/templates/control/control/test_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/templates/control/control/test_server_integration.py` & `truss-0.5.1/truss/tests/templates/control/control/test_server_integration.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/templates/core/server/common/test_truss_server.py` & `truss-0.5.1/truss/tests/templates/core/server/common/test_truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/templates/core/server/common/test_util.py` & `truss-0.5.1/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.5.1/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/templates/server/common/test_retry.py` & `truss-0.5.1/truss/tests/templates/server/common/test_retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/templates/server/common/test_termination_handler_middleware.py` & `truss-0.5.1/truss/tests/templates/server/common/test_termination_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/templates/server/test_model_wrapper.py` & `truss-0.5.1/truss/tests/templates/server/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/test_backward.py` & `truss-0.5.1/truss/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/test_build.py` & `truss-0.5.1/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/test_config.py` & `truss-0.5.1/truss/tests/test_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 import pytest
 import yaml
 from truss.truss_config import (
     DEFAULT_CPU,
     DEFAULT_MEMORY,
     DEFAULT_USE_GPU,
     Accelerator,
@@ -275,7 +277,43 @@
         },
         {"repo_id": "test/model2", "revision": "not-main2"},
     ]
 
     assert new_config == config.to_dict(verbose=False)
     assert config.to_dict(verbose=True)["hf_cache"][0].get("revision") is None
     assert config.to_dict(verbose=True)["hf_cache"][1].get("revision") == "not-main2"
+
+
+def test_empty_config():
+    config = TrussConfig()
+    new_config = generate_default_config()
+
+    assert new_config == config.to_dict(verbose=False)
+
+
+def test_from_yaml():
+    yaml_path = Path("test.yaml")
+    data = {"description": "this is a test"}
+    with yaml_path.open("w") as yaml_file:
+        yaml.safe_dump(data, yaml_file)
+
+    result = TrussConfig.from_yaml(yaml_path)
+
+    assert result.description == "this is a test"
+
+    yaml_path.unlink()
+
+
+def test_from_yaml_empty():
+    yaml_path = Path("test.yaml")
+    data = {}
+    with yaml_path.open("w") as yaml_file:
+        yaml.safe_dump(data, yaml_file)
+
+    result = TrussConfig.from_yaml(yaml_path)
+
+    # test some attributes (should be default)
+    assert result.description is None
+    assert result.spec_version == "2.0"
+    assert result.bundled_packages_dir == "packages"
+
+    yaml_path.unlink()
```

### Comparing `truss-0.5.0/truss/tests/test_context_builder_image.py` & `truss-0.5.1/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/test_control_truss_patching.py` & `truss-0.5.1/truss/tests/test_control_truss_patching.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/test_docker.py` & `truss-0.5.1/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/test_model_inference.py` & `truss-0.5.1/truss/tests/test_model_inference.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,34 @@
 )
 from truss.tests.test_testing_utilities_for_other_tests import ensure_kill_all
 from truss.truss_handle import TrussHandle
 
 logger = logging.getLogger(__name__)
 
 
+class PropagatingThread(Thread):
+    """
+    PropagatingThread allows us to run threads and keep track of exceptions
+    thrown.
+    """
+
+    def run(self):
+        self.exc = None
+        try:
+            self.ret = self._target(*self._args, **self._kwargs)
+        except BaseException as e:
+            self.exc = e
+
+    def join(self, timeout=None):
+        super(PropagatingThread, self).join(timeout)
+        if self.exc:
+            raise self.exc
+        return self.ret
+
+
 def test_pytorch_init_arg_validation(
     pytorch_model_with_init_args, pytorch_model_init_args
 ):
     pytorch_model_with_init_args, _ = pytorch_model_with_init_args
     # Validates with args and kwargs
     validate_provided_parameters_with_model(
         pytorch_model_with_init_args.__class__, pytorch_model_init_args
@@ -134,14 +154,101 @@
         assert not _test_readiness_probe(expected_code=200)
         assert not _test_liveness_probe(expected_code=200)
         assert not _test_ping(expected_code=200)
         assert not _test_invocations(expected_code=200)
 
 
 @pytest.mark.integration
+def test_concurrency_truss():
+    # Tests that concurrency limits work correctly
+    with ensure_kill_all():
+        truss_root = Path(__file__).parent.parent.parent.resolve() / "truss"
+
+        truss_dir = truss_root / "test_data" / "test_concurrency_truss"
+
+        tr = TrussHandle(truss_dir)
+
+        _ = tr.docker_run(local_port=8090, detach=True, wait_for_server_ready=True)
+
+        truss_server_addr = "http://localhost:8090"
+        full_url = f"{truss_server_addr}/v1/models/model:predict"
+
+        # Each request takes 2 seconds, for this thread, we allow
+        # a concurrency of 2. This means the first two requests will
+        # succeed within the 2 seconds, and the third will fail, since
+        # it cannot start until the first two have completed.
+        def make_request():
+            requests.post(full_url, json={}, timeout=3)
+
+        successful_thread_1 = PropagatingThread(target=make_request)
+        successful_thread_2 = PropagatingThread(target=make_request)
+        failed_thread = PropagatingThread(target=make_request)
+
+        successful_thread_1.start()
+        successful_thread_2.start()
+        # Ensure that the thread to fail starts a little after the others
+        time.sleep(0.2)
+        failed_thread.start()
+
+        successful_thread_1.join()
+        successful_thread_2.join()
+        with pytest.raises(requests.exceptions.ReadTimeout):
+            failed_thread.join()
+
+
+@pytest.mark.integration
+def test_async_truss():
+    with ensure_kill_all():
+        truss_root = Path(__file__).parent.parent.parent.resolve() / "truss"
+
+        truss_dir = truss_root / "test_data" / "test_async_truss"
+
+        tr = TrussHandle(truss_dir)
+
+        _ = tr.docker_run(local_port=8090, detach=True, wait_for_server_ready=True)
+        truss_server_addr = "http://localhost:8090"
+        full_url = f"{truss_server_addr}/v1/models/model:predict"
+
+        response = requests.post(full_url, json={})
+        assert response.json() == {
+            "preprocess_value": "value",
+            "postprocess_value": "value",
+        }
+
+
+@pytest.mark.integration
+def test_async_streaming():
+    with ensure_kill_all():
+        truss_root = Path(__file__).parent.parent.parent.resolve() / "truss"
+
+        truss_dir = truss_root / "test_data" / "test_streaming_async_generator_truss"
+
+        tr = TrussHandle(truss_dir)
+
+        _ = tr.docker_run(local_port=8090, detach=True, wait_for_server_ready=True)
+        truss_server_addr = "http://localhost:8090"
+        full_url = f"{truss_server_addr}/v1/models/model:predict"
+
+        response = requests.post(full_url, json={}, stream=True)
+        assert response.headers.get("transfer-encoding") == "chunked"
+        assert [
+            byte_string.decode() for byte_string in list(response.iter_content())
+        ] == ["0", "1", "2", "3", "4"]
+
+        predict_non_stream_response = requests.post(
+            full_url,
+            json={},
+            stream=True,
+            headers={"accept": "application/json"},
+        )
+        assert "transfer-encoding" not in predict_non_stream_response.headers
+        assert predict_non_stream_response.json() == "01234"
+
+
+@pytest.mark.integration
 def test_streaming_truss():
     with ensure_kill_all():
         truss_root = Path(__file__).parent.parent.parent.resolve() / "truss"
         truss_dir = truss_root / "test_data" / "test_streaming_truss"
         tr = TrussHandle(truss_dir)
 
         _ = tr.docker_run(local_port=8090, detach=True, wait_for_server_ready=True)
```

### Comparing `truss-0.5.0/truss/tests/test_notebooks.py` & `truss-0.5.1/truss/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.5.1/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/test_truss_gatherer.py` & `truss-0.5.1/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/test_truss_handle.py` & `truss-0.5.1/truss/tests/test_truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/test_validation.py` & `truss-0.5.1/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/tests/util/test_path.py` & `truss-0.5.1/truss/tests/util/test_path.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/truss_config.py` & `truss-0.5.1/truss/truss_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 DEFAULT_MODEL_CLASS_NAME = "Model"
 DEFAULT_TRUSS_STRUCTURE_VERSION = "2.0"
 DEFAULT_MODEL_INPUT_TYPE = "Any"
 DEFAULT_PYTHON_VERSION = "py39"
 DEFAULT_DATA_DIRECTORY = "data"
 DEFAULT_EXAMPLES_FILENAME = "examples.yaml"
 DEFAULT_SPEC_VERSION = "2.0"
+DEFAULT_PREDICT_CONCURRENCY = 1
 
 DEFAULT_CPU = "500m"
 DEFAULT_MEMORY = "512Mi"
 DEFAULT_USE_GPU = False
 
 DEFAULT_TRAINING_CLASS_FILENAME = "train.py"
 DEFAULT_TRAINING_CLASS_NAME = "Train"
@@ -104,14 +105,32 @@
         return HuggingFaceCache([HuggingFaceModel.from_dict(item) for item in items])
 
     def to_list(self, verbose=False) -> List[Dict[str, str]]:
         return [model.to_dict(verbose=verbose) for model in self.models]
 
 
 @dataclass
+class Runtime:
+    predict_concurrency: int = DEFAULT_PREDICT_CONCURRENCY
+
+    @staticmethod
+    def from_dict(d):
+        predict_concurrency = d.get("predict_concurrency", DEFAULT_PREDICT_CONCURRENCY)
+
+        return Runtime(
+            predict_concurrency=predict_concurrency,
+        )
+
+    def to_dict(self):
+        return {
+            "predict_concurrency": self.predict_concurrency,
+        }
+
+
+@dataclass
 class Resources:
     cpu: str = DEFAULT_CPU
     memory: str = DEFAULT_MEMORY
     use_gpu: bool = DEFAULT_USE_GPU
     accelerator: AcceleratorSpec = field(default_factory=AcceleratorSpec)
 
     @staticmethod
@@ -278,14 +297,15 @@
     # Python types for what the model expects as input
     input_type: str = DEFAULT_MODEL_INPUT_TYPE
     model_metadata: Dict[str, Any] = field(default_factory=dict)
     requirements: List[str] = field(default_factory=list)
     system_packages: List[str] = field(default_factory=list)
     environment_variables: Dict[str, str] = field(default_factory=dict)
     resources: Resources = field(default_factory=Resources)
+    runtime: Runtime = field(default_factory=Runtime)
     python_version: str = DEFAULT_PYTHON_VERSION
     examples_filename: str = DEFAULT_EXAMPLES_FILENAME
     secrets: Dict[str, str] = field(default_factory=dict)
     description: Optional[str] = None
     bundled_packages_dir: str = DEFAULT_BUNDLED_PACKAGES_DIR
     external_package_dirs: List[str] = field(default_factory=list)
     live_reload: bool = False
@@ -304,17 +324,14 @@
             "py38": "3.8",
             "py37": "3.7",
         }[self.python_version]
 
     @staticmethod
     def from_dict(d):
         config = TrussConfig(
-            # Users that are calling `load` on an existing Truss
-            # should default to 1.0 whereas users creating a new Truss
-            # should default to 2.0.
             spec_version=d.get("spec_version", DEFAULT_SPEC_VERSION),
             model_type=d.get("model_type", DEFAULT_MODEL_TYPE),
             model_framework=ModelFrameworkType(
                 d.get("model_framework", DEFAULT_MODEL_FRAMEWORK_TYPE.value)
             ),
             model_module_dir=d.get("model_module_dir", DEFAULT_MODEL_MODULE_DIR),
             model_class_filename=d.get(
@@ -324,14 +341,15 @@
             data_dir=d.get("data_dir", DEFAULT_DATA_DIRECTORY),
             input_type=d.get("input_type", DEFAULT_MODEL_INPUT_TYPE),
             model_metadata=d.get("model_metadata", {}),
             requirements=d.get("requirements", []),
             system_packages=d.get("system_packages", []),
             environment_variables=d.get("environment_variables", {}),
             resources=Resources.from_dict(d.get("resources", {})),
+            runtime=Runtime.from_dict(d.get("runtime", {})),
             python_version=d.get("python_version", DEFAULT_PYTHON_VERSION),
             model_name=d.get("model_name", None),
             examples_filename=d.get("examples_filename", DEFAULT_EXAMPLES_FILENAME),
             secrets=d.get("secrets", {}),
             description=d.get("description", None),
             bundled_packages_dir=d.get(
                 "bundled_packages_dir", DEFAULT_BUNDLED_PACKAGES_DIR
@@ -348,15 +366,16 @@
         )
         config.validate()
         return config
 
     @staticmethod
     def from_yaml(yaml_path: Path):
         with yaml_path.open() as yaml_file:
-            return TrussConfig.from_dict(yaml.safe_load(yaml_file))
+            raw_data = yaml.safe_load(yaml_file) or {}
+            return TrussConfig.from_dict(raw_data)
 
     def write_to_yaml_file(self, path: Path, verbose: bool = True):
         with path.open("w") as config_file:
             yaml.dump(self.to_dict(verbose=verbose), config_file)
 
     def to_dict(self, verbose: bool = True):
         return obj_to_dict(self, verbose=verbose)
@@ -368,14 +387,15 @@
         for secret_name in self.secrets:
             validate_secret_name(secret_name)
 
 
 DATACLASS_TO_REQ_KEYS_MAP = {
     Train: {"variables"},
     Resources: {"accelerator", "cpu", "memory", "use_gpu"},
+    Runtime: {"predict_concurrency"},
     TrussConfig: {
         "environment_variables",
         "external_package_dirs",
         "model_metadata",
         "model_name",
         "python_version",
         "requirements",
```

### Comparing `truss-0.5.0/truss/truss_gatherer.py` & `truss-0.5.1/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/truss_handle.py` & `truss-0.5.1/truss/truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/truss_spec.py` & `truss-0.5.1/truss/truss_spec.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/types.py` & `truss-0.5.1/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/util/.truss_ignore` & `truss-0.5.1/truss/util/.truss_ignore`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/util/download.py` & `truss-0.5.1/truss/util/download.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/util/gpu.py` & `truss-0.5.1/truss/util/gpu.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/util/path.py` & `truss-0.5.1/truss/util/path.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/truss/validation.py` & `truss-0.5.1/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.5.0/PKG-INFO` & `truss-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.5.0
+Version: 0.5.1
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.12
@@ -18,24 +18,26 @@
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: blake3 (>=0.3.3,<0.4.0)
 Requires-Dist: boto3 (>=1.26.157,<2.0.0)
 Requires-Dist: cloudpickle (>=2.2.0,<3.0.0)
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: huggingface_hub (>=0.16.4,<0.17.0)
+Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: msgpack (>=1.0.2)
 Requires-Dist: msgpack-numpy (>=0.4.7.1)
 Requires-Dist: numpy (==1.23.5)
 Requires-Dist: packaging (>=20.9)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: python-json-logger (>=2.0.2)
 Requires-Dist: python-on-whales (>=0.46.0,<0.47.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Requires-Dist: single-source (>=0.3.0,<0.4.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
 Requires-Dist: watchfiles (>=0.19.0,<0.20.0)
 Project-URL: Bug Reports, https://github.com/basetenlabs/truss/issues
 Project-URL: Baseten, https://baseten.co
 Project-URL: Documentation, https://truss.baseten.co
```

