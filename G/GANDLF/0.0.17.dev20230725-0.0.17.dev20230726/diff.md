# Comparing `tmp/GANDLF-0.0.17.dev20230725.tar.gz` & `tmp/GANDLF-0.0.17.dev20230726.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GANDLF-0.0.17.dev20230725.tar", last modified: Tue Jul 25 03:13:04 2023, max compression
+gzip compressed data, was "GANDLF-0.0.17.dev20230726.tar", last modified: Wed Jul 26 03:12:35 2023, max compression
```

## Comparing `GANDLF-0.0.17.dev20230725.tar` & `GANDLF-0.0.17.dev20230726.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.972634 GANDLF-0.0.17.dev20230725/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/Dockerfile-CPU
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/Dockerfile-CUDA11.6
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/Dockerfile-ROCm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.924633 GANDLF-0.0.17.dev20230725/GANDLF/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.924633 GANDLF-0.0.17.dev20230725/GANDLF/anonymize/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/anonymize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/anonymize/convert_to_nifti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.928633 GANDLF-0.0.17.dev20230725/GANDLF/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/cli/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/cli/generate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/cli/main_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/cli/patch_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/cli/post_training_model_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/cli/preprocess_and_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/cli/recover_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.932633 GANDLF-0.0.17.dev20230725/GANDLF/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23147 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/compute/forward_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/compute/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/compute/inference_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/compute/loss_and_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/compute/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    21289 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/compute/training_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.932633 GANDLF-0.0.17.dev20230725/GANDLF/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/ImagesFromDataFrame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.936633 GANDLF-0.0.17.dev20230725/GANDLF/data/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/augmentation/blur_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/augmentation/hed_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/augmentation/noise_enhanced.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/augmentation/rgb_augs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/augmentation/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/augmentation/wrap_torchio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/inference_dataloader_histopath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.936633 GANDLF-0.0.17.dev20230725/GANDLF/data/patch_miner/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/patch_miner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.936633 GANDLF-0.0.17.dev20230725/GANDLF/data/patch_miner/opm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/patch_miner/opm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/patch_miner/opm/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/patch_miner/opm/patch_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17090 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/patch_miner/opm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.940633 GANDLF-0.0.17.dev20230725/GANDLF/data/post_process/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/post_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/post_process/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/post_process/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.940633 GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/crop_zero_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/non_zero_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/normalize_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/resample_minimum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/rgb_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.944633 GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/template_matching/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/template_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/template_matching/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/template_matching/histogram_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/template_matching/stain_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/template_matching/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/threshold_and_clip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.944633 GANDLF-0.0.17.dev20230725/GANDLF/grad_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/grad_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/grad_clipping/adaptive_gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/grad_clipping/clip_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/grad_clipping/grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/inference_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.948633 GANDLF-0.0.17.dev20230725/GANDLF/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/losses/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/losses/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/losses/segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.948633 GANDLF-0.0.17.dev20230725/GANDLF/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/metrics/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/metrics/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/metrics/synthesis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.964634 GANDLF-0.0.17.dev20230725/GANDLF/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/MSDNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/brain_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/deep_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/imagenet_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/imagenet_vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/light_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/light_unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/modelBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/sdnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.968634 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/DecodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/DownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/EncodingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/FCNUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/IncConv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/IncDownsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/IncDropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/IncUpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/InceptionModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/InitialConv.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/Interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/ResNetModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/UpsamplingModule.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/add_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/add_downsample_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/average_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/out_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/transunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/uinc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/unet_multilayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/models/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.968634 GANDLF-0.0.17.dev20230725/GANDLF/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/optimizers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    31386 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/parseConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.968634 GANDLF-0.0.17.dev20230725/GANDLF/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/schedulers/wrap_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/training_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.972634 GANDLF-0.0.17.dev20230725/GANDLF/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/utils/handle_collisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/utils/imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/utils/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/utils/modelio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/utils/parameter_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/GANDLF/utils/write_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-25 03:12:58.000000 GANDLF-0.0.17.dev20230725/GANDLF/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:13:04.924633 GANDLF-0.0.17.dev20230725/GANDLF.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-07-25 03:13:04.000000 GANDLF-0.0.17.dev20230725/GANDLF.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-25 03:13:04.000000 GANDLF-0.0.17.dev20230725/GANDLF.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 03:13:04.000000 GANDLF-0.0.17.dev20230725/GANDLF.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 03:10:48.000000 GANDLF-0.0.17.dev20230725/GANDLF.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-25 03:13:04.000000 GANDLF-0.0.17.dev20230725/GANDLF.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 03:13:04.000000 GANDLF-0.0.17.dev20230725/GANDLF.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-07-25 03:13:04.972634 GANDLF-0.0.17.dev20230725/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/gandlf_anonymizer
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/gandlf_collectStats
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/gandlf_configGenerator
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/gandlf_constructCSV
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/gandlf_deploy
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/gandlf_generateMetrics
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/gandlf_optimizeModel
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/gandlf_patchMiner
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/gandlf_preprocess
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/gandlf_recoverConfig
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/gandlf_run
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/gandlf_verifyInstall
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 03:13:04.976634 GANDLF-0.0.17.dev20230725/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-25 03:10:28.000000 GANDLF-0.0.17.dev20230725/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.071314 GANDLF-0.0.17.dev20230726/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/Dockerfile-CPU
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/Dockerfile-CUDA11.6
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/Dockerfile-ROCm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.035313 GANDLF-0.0.17.dev20230726/GANDLF/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.035313 GANDLF-0.0.17.dev20230726/GANDLF/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/anonymize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/anonymize/convert_to_nifti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.039313 GANDLF-0.0.17.dev20230726/GANDLF/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/cli/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/cli/generate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/cli/main_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/cli/patch_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/cli/post_training_model_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/cli/preprocess_and_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/cli/recover_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.043314 GANDLF-0.0.17.dev20230726/GANDLF/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23147 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/compute/forward_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/compute/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/compute/inference_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/compute/loss_and_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/compute/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21289 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/compute/training_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.043314 GANDLF-0.0.17.dev20230726/GANDLF/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12615 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/ImagesFromDataFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.043314 GANDLF-0.0.17.dev20230726/GANDLF/data/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/augmentation/blur_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/augmentation/hed_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/augmentation/noise_enhanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/augmentation/rgb_augs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/augmentation/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/augmentation/wrap_torchio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/inference_dataloader_histopath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.043314 GANDLF-0.0.17.dev20230726/GANDLF/data/patch_miner/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/patch_miner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.047314 GANDLF-0.0.17.dev20230726/GANDLF/data/patch_miner/opm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/patch_miner/opm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/patch_miner/opm/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/patch_miner/opm/patch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17090 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/patch_miner/opm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.047314 GANDLF-0.0.17.dev20230726/GANDLF/data/post_process/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/post_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/post_process/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/post_process/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.047314 GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/crop_zero_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/non_zero_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/normalize_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/resample_minimum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/rgb_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.051313 GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/template_matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/template_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/template_matching/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/template_matching/histogram_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/template_matching/stain_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/template_matching/stain_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/template_matching/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/threshold_and_clip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.051313 GANDLF-0.0.17.dev20230726/GANDLF/grad_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/grad_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/grad_clipping/adaptive_gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/grad_clipping/clip_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/grad_clipping/grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/inference_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.051313 GANDLF-0.0.17.dev20230726/GANDLF/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/losses/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/losses/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/losses/segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.055314 GANDLF-0.0.17.dev20230726/GANDLF/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/metrics/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/metrics/synthesis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.063314 GANDLF-0.0.17.dev20230726/GANDLF/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/MSDNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/brain_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/deep_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12081 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/imagenet_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/imagenet_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/light_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/light_unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/modelBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17514 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14834 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/sdnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.067314 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/DecodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/DownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/EncodingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/FCNUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/IncConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/IncDownsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/IncDropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/IncUpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/InceptionModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/InitialConv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/Interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/ResNetModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/UpsamplingModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/add_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/add_downsample_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/average_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/out_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/transunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/uinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/unet_multilayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24719 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/models/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.067314 GANDLF-0.0.17.dev20230726/GANDLF/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/optimizers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31631 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/parseConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.067314 GANDLF-0.0.17.dev20230726/GANDLF/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/schedulers/wrap_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/training_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.071314 GANDLF-0.0.17.dev20230726/GANDLF/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/utils/handle_collisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9007 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/utils/imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/utils/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/utils/modelio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/utils/parameter_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/GANDLF/utils/write_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-26 03:12:28.000000 GANDLF-0.0.17.dev20230726/GANDLF/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:12:35.035313 GANDLF-0.0.17.dev20230726/GANDLF.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-07-26 03:12:35.000000 GANDLF-0.0.17.dev20230726/GANDLF.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-26 03:12:35.000000 GANDLF-0.0.17.dev20230726/GANDLF.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 03:12:35.000000 GANDLF-0.0.17.dev20230726/GANDLF.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 03:10:23.000000 GANDLF-0.0.17.dev20230726/GANDLF.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-26 03:12:35.000000 GANDLF-0.0.17.dev20230726/GANDLF.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 03:12:35.000000 GANDLF-0.0.17.dev20230726/GANDLF.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-07-26 03:12:35.071314 GANDLF-0.0.17.dev20230726/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/gandlf_anonymizer
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/gandlf_collectStats
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/gandlf_configGenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/gandlf_constructCSV
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/gandlf_deploy
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/gandlf_generateMetrics
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/gandlf_optimizeModel
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/gandlf_patchMiner
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/gandlf_preprocess
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/gandlf_recoverConfig
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/gandlf_run
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/gandlf_verifyInstall
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 03:12:35.071314 GANDLF-0.0.17.dev20230726/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-26 03:10:08.000000 GANDLF-0.0.17.dev20230726/setup.py
```

### Comparing `GANDLF-0.0.17.dev20230725/CODE_OF_CONDUCT.md` & `GANDLF-0.0.17.dev20230726/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/CONTRIBUTING.md` & `GANDLF-0.0.17.dev20230726/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/Dockerfile-CPU` & `GANDLF-0.0.17.dev20230726/Dockerfile-CPU`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/Dockerfile-CUDA11.6` & `GANDLF-0.0.17.dev20230726/Dockerfile-CUDA11.6`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/Dockerfile-ROCm` & `GANDLF-0.0.17.dev20230726/Dockerfile-ROCm`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/anonymize/__init__.py` & `GANDLF-0.0.17.dev20230726/GANDLF/anonymize/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/anonymize/convert_to_nifti.py` & `GANDLF-0.0.17.dev20230726/GANDLF/anonymize/convert_to_nifti.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/cli/__init__.py` & `GANDLF-0.0.17.dev20230726/GANDLF/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/cli/config_generator.py` & `GANDLF-0.0.17.dev20230726/GANDLF/cli/config_generator.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/cli/deploy.py` & `GANDLF-0.0.17.dev20230726/GANDLF/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/cli/generate_metrics.py` & `GANDLF-0.0.17.dev20230726/GANDLF/cli/generate_metrics.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/cli/main_run.py` & `GANDLF-0.0.17.dev20230726/GANDLF/cli/main_run.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/cli/patch_extraction.py` & `GANDLF-0.0.17.dev20230726/GANDLF/cli/patch_extraction.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/cli/post_training_model_optimization.py` & `GANDLF-0.0.17.dev20230726/GANDLF/cli/post_training_model_optimization.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/cli/preprocess_and_save.py` & `GANDLF-0.0.17.dev20230726/GANDLF/cli/preprocess_and_save.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/cli/recover_config.py` & `GANDLF-0.0.17.dev20230726/GANDLF/cli/recover_config.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/compute/forward_pass.py` & `GANDLF-0.0.17.dev20230726/GANDLF/compute/forward_pass.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/compute/generic.py` & `GANDLF-0.0.17.dev20230726/GANDLF/compute/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/compute/inference_loop.py` & `GANDLF-0.0.17.dev20230726/GANDLF/compute/inference_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/compute/loss_and_metric.py` & `GANDLF-0.0.17.dev20230726/GANDLF/compute/loss_and_metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,34 +21,30 @@
             return temp
         else:
             return metric_output.item()
 
 
 def get_loss_and_metrics(image, ground_truth, predicted, params):
     """
-    image: torch.Tensor
-        The input image stack according to requirements
-    ground_truth : torch.Tensor
-        The input ground truth for the corresponding image label
-    predicted : torch.Tensor
-        The input predicted label for the corresponding image label
-    params : dict
-        The parameters passed by the user yaml
+    This function computes the loss and metrics for a given image, ground truth and predicted output.
 
-    Returns
-    -------
-    loss : torch.Tensor
-        The computed loss from the label and the output
-    metric_output : torch.Tensor
-        The computed metric from the label and the output
+    Args:
+        image (torch.Tensor): The input image stack according to requirements.
+        ground_truth (torch.Tensor): The input ground truth for the corresponding image label.
+        predicted (torch.Tensor): The input predicted label for the corresponding image label.
+        params (dict): The parameters passed by the user yaml.
+
+    Returns:
+        torch.Tensor: The computed loss from the label and the prediction.
+        dict: The computed metric from the label and the prediction.
     """
     # this is currently only happening for mse_torch
     if isinstance(params["loss_function"], dict):
         # check for mse_torch
-        loss_function = global_losses_dict["mse"]
+        loss_function = global_losses_dict[list(params["loss_function"].keys())[0]]
     else:
         loss_str_lower = params["loss_function"].lower()
         if loss_str_lower in global_losses_dict:
             loss_function = global_losses_dict[loss_str_lower]
         else:
             sys.exit(
                 "WARNING: Could not find the requested loss function '"
```

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/compute/step.py` & `GANDLF-0.0.17.dev20230726/GANDLF/compute/step.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/compute/training_loop.py` & `GANDLF-0.0.17.dev20230726/GANDLF/compute/training_loop.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/ImagesFromDataFrame.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/ImagesFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/__init__.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/augmentation/__init__.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/augmentation/blur_enhanced.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/augmentation/blur_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/augmentation/hed_augs.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/augmentation/hed_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/augmentation/noise_enhanced.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/augmentation/noise_enhanced.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/augmentation/rgb_augs.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/augmentation/rgb_augs.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/augmentation/rotations.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/augmentation/rotations.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/augmentation/wrap_torchio.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/augmentation/wrap_torchio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/inference_dataloader_histopath.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/inference_dataloader_histopath.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/patch_miner/opm/patch.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/patch_miner/opm/patch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/patch_miner/opm/patch_manager.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/patch_miner/opm/patch_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/patch_miner/opm/utils.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/patch_miner/opm/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/post_process/morphology.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/post_process/morphology.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/post_process/tensor.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/post_process/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/__init__.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/crop_zero_planes.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/crop_zero_planes.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/non_zero_normalize.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/non_zero_normalize.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/normalize_rgb.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/normalize_rgb.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/resample_minimum.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/resample_minimum.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/rgb_conversion.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/rgb_conversion.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/template_matching/base.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/template_matching/base.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/template_matching/histogram_matching.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/template_matching/histogram_matching.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/template_matching/stain_extractors.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/template_matching/stain_extractors.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/template_matching/stain_normalizer.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/template_matching/stain_normalizer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/template_matching/utils.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/template_matching/utils.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/data/preprocessing/threshold_and_clip.py` & `GANDLF-0.0.17.dev20230726/GANDLF/data/preprocessing/threshold_and_clip.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/grad_clipping/adaptive_gradient_clipping.py` & `GANDLF-0.0.17.dev20230726/GANDLF/grad_clipping/adaptive_gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/grad_clipping/clip_gradients.py` & `GANDLF-0.0.17.dev20230726/GANDLF/grad_clipping/clip_gradients.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/grad_clipping/grad_scaler.py` & `GANDLF-0.0.17.dev20230726/GANDLF/grad_clipping/grad_scaler.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/inference_manager.py` & `GANDLF-0.0.17.dev20230726/GANDLF/inference_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/logger.py` & `GANDLF-0.0.17.dev20230726/GANDLF/logger.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/losses/__init__.py` & `GANDLF-0.0.17.dev20230726/GANDLF/losses/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 """
 All the losses are to be called from here
 """
-from .segmentation import MCD_loss, MCD_log_loss, MCT_loss, KullbackLeiblerDivergence
+from .segmentation import (
+    MCD_loss,
+    MCD_log_loss,
+    MCT_loss,
+    KullbackLeiblerDivergence,
+    FocalLoss,
+)
 from .regression import CE, CEL, MSE_loss, L1_loss
-from .hybrid import DCCE, DCCE_Logits
+from .hybrid import DCCE, DCCE_Logits, DC_Focal
 
 
 # global defines for the losses
 global_losses_dict = {
     "dc": MCD_loss,
     "dice": MCD_loss,
     "dc_log": MCD_log_loss,
@@ -16,8 +22,10 @@
     "dcce_logits": DCCE_Logits,
     "ce": CE,
     "mse": MSE_loss,
     "cel": CEL,
     "tversky": MCT_loss,
     "kld": KullbackLeiblerDivergence,
     "l1": L1_loss,
+    "focal": FocalLoss,
+    "dc_focal": DC_Focal,
 }
```

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/losses/hybrid.py` & `GANDLF-0.0.17.dev20230726/GANDLF/losses/hybrid.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,57 @@
-from .segmentation import MCD_loss
+import torch
+
+from .segmentation import MCD_loss, FocalLoss
 from .regression import CCE_Generic, CE, CE_Logits
 
 
-def DCCE(predicted_mask, ground_truth, params):
+def DCCE(predicted_mask, ground_truth, params) -> torch.Tensor:
     """
     Calculates the Dice-Cross-Entropy loss.
 
-    Parameters
-    ----------
-    predicted_mask : torch.Tensor
-        Predicted mask
-    ground_truth : torch.Tensor
-        Ground truth mask
-    params : dict
-        Dictionary of parameters
-
-    Returns
-    -------
-    torch.Tensor
-        Calculated loss
+    Args:
+        predicted_mask (torch.Tensor): The predicted mask.
+        ground_truth (torch.Tensor): The ground truth mask.
+        params (dict): The parameters.
+
+    Returns:
+        torch.Tensor: The calculated loss.
     """
     dcce_loss = MCD_loss(predicted_mask, ground_truth, params) + CCE_Generic(
         predicted_mask, ground_truth, params, CE
     )
     return dcce_loss
 
 
 def DCCE_Logits(predicted_mask, ground_truth, params):
     """
     Calculates the Dice-Cross-Entropy loss using logits.
 
-    Parameters
-    ----------
-    predicted_mask : torch.Tensor
-        Predicted mask logits
-    ground_truth : torch.Tensor
-        Ground truth mask
-    params : dict
-        Dictionary of parameters
-
-    Returns
-    -------
-    torch.Tensor
-        Calculated loss
+    Args:
+        predicted_mask (torch.Tensor): The predicted mask.
+        ground_truth (torch.Tensor): The ground truth mask.
+        params (dict): The parameters.
+
+    Returns:
+        torch.Tensor: The calculated loss.
     """
     dcce_loss = MCD_loss(predicted_mask, ground_truth, params) + CCE_Generic(
         predicted_mask, ground_truth, params, CE_Logits
     )
     return dcce_loss
+
+
+def DC_Focal(predicted_mask, ground_truth, params):
+    """
+    Calculates the Dice-Focal loss.
+
+    Args:
+        predicted_mask (torch.Tensor): The predicted mask.
+        ground_truth (torch.Tensor): The ground truth mask.
+        params (dict): The parameters.
+
+    Returns:
+        torch.Tensor: The calculated loss.
+    """
+    return MCD_loss(predicted_mask, ground_truth, params) + FocalLoss(
+        predicted_mask, ground_truth, params
+    )
```

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/losses/regression.py` & `GANDLF-0.0.17.dev20230726/GANDLF/losses/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/losses/segmentation.py` & `GANDLF-0.0.17.dev20230726/GANDLF/losses/segmentation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 import sys
 import torch
 
 
 # Dice scores and dice losses
-def dice(predicted, target):
+def dice(predicted, target) -> torch.Tensor:
     """
-    This function computes a dice score between two tensors
+    This function computes a dice score between two tensors.
 
-    Parameters
-    ----------
-    predicted : Tensor
-        predicted value by the network
-    target : Tensor
-        Required target label to match the predicted with
-
-    Returns
-    -------
-    Tensor
-        Computed Dice Score
+    Args:
+        predicted (_type_): Predicted value by the network.
+        target (_type_): Required target label to match the predicted with
 
+    Returns:
+        torch.Tensor: The computed dice score.
     """
     predicted_flat = predicted.flatten()
     label_flat = target.flatten()
     intersection = (predicted_flat * label_flat).sum()
 
     dice_score = (2.0 * intersection + sys.float_info.min) / (
         predicted_flat.sum() + label_flat.sum() + sys.float_info.min
@@ -32,15 +26,15 @@
 
 
 def MCD(predicted, target, num_class, weights=None, ignore_class=None, loss_type=0):
     """
     This function computes the mean class dice score between two tensors
 
     Args:
-        predicted (torch.Tensor): predicted generally by the network
+        predicted (torch.Tensor): Predicted generally by the network
         target (torch.Tensor): Required target label to match the predicted with
         num_class (int): Number of classes (including the background class)
         weights (list, optional): Dice weights for each class (excluding the background class), defaults to None
         ignore_class (int, optional): Class to ignore, defaults to None
         loss_type (int, optional): Type of loss to compute, defaults to 0
             0: no loss, normal dice calculation
             1: dice loss, (1-dice)
@@ -101,15 +95,15 @@
 
 
 def tversky_loss(predicted, target, alpha=0.5, beta=0.5):
     """
     This function calculates the Tversky loss between two tensors.
 
     Args:
-        predicted (torch.Tensor): predicted generally by the network
+        predicted (torch.Tensor): Predicted generally by the network
         target (torch.Tensor): Required target label to match the predicted with
         alpha (float, optional): Weight of false positives. Defaults to 0.5.
         beta (float, optional): Weight of false negatives. Defaults to 0.5.
 
     Returns:
         torch.Tensor: Computed Tversky Loss
     """
@@ -134,15 +128,15 @@
 
 
 def MCT_loss(predicted, target, params=None):
     """
     This function calculates the Multi-Class Tversky loss between two tensors.
 
     Args:
-        predicted (torch.Tensor): predicted generally by the network
+        predicted (torch.Tensor): Predicted generally by the network
         target (torch.Tensor): Required target label to match the predicted with
         params (dict, optional): Additional parameters for computing loss function, including weights for each class
 
     Returns:
         torch.Tensor: Computed Multi-Class Tversky Loss
     """
 
@@ -171,7 +165,61 @@
         params (dict, optional): A dictionary of optional parameters
 
     Returns:
         torch.Tensor: The computed Kullback-Leibler divergence
     """
     loss = -0.5 * torch.sum(1 + logvar - mu.pow(2) - logvar.exp(), dim=-1)
     return loss.mean()
+
+
+def FocalLoss(predicted, target, params=None):
+    """
+    This function calculates the Focal loss between two tensors.
+
+    Args:
+        predicted (torch.Tensor): Predicted generally by the network
+        target (torch.Tensor): Required target label to match the predicted with
+        params (dict, optional): Additional parameters for computing loss function, including weights for each class
+
+    Returns:
+        torch.Tensor: Computed Focal Loss
+    """
+    gamma = 2.0
+    size_average = True
+    if isinstance(params["loss_function"], dict):
+        gamma = params["loss_function"].get("gamma", 2.0)
+        size_average = params["loss_function"].get("size_average", True)
+
+    def _focal_loss(preds, target, gamma, size_average=True):
+        """
+        Internal helper function to calcualte focal loss for a single class.
+
+        Args:
+            preds (torch.Tensor): predicted generally by the network
+            target (torch.Tensor): Required target label to match the predicted with
+            gamma (float): The gamma value for focal loss
+            size_average (bool, optional): Whether to average the loss across the batch. Defaults to True.
+
+        Returns:
+            torch.Tensor: Computed focal loss for a single class.
+        """
+        ce_loss = torch.nn.CrossEntropyLoss(reduce=False)
+        logpt = ce_loss(preds, target)
+        pt = torch.exp(-logpt)
+        loss = ((1 - pt) ** gamma) * logpt
+        return_loss = loss.sum()
+        if size_average:
+            return_loss = loss.mean()
+        return return_loss
+
+    acc_focal_loss = 0
+    num_classes = predicted.shape[1]
+
+    for i in range(num_classes):
+        curr_loss = _focal_loss(
+            predicted[:, i, ...], target[:, i, ...], gamma, size_average
+        )
+        if params is not None and params.get("weights") is not None:
+            curr_loss = curr_loss * params["weights"][i]
+        acc_focal_loss += curr_loss
+
+    return acc_focal_loss
```

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/metrics/__init__.py` & `GANDLF-0.0.17.dev20230726/GANDLF/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/metrics/classification.py` & `GANDLF-0.0.17.dev20230726/GANDLF/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/metrics/generic.py` & `GANDLF-0.0.17.dev20230726/GANDLF/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/metrics/regression.py` & `GANDLF-0.0.17.dev20230726/GANDLF/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/metrics/segmentation.py` & `GANDLF-0.0.17.dev20230726/GANDLF/metrics/segmentation.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/metrics/synthesis.py` & `GANDLF-0.0.17.dev20230726/GANDLF/metrics/synthesis.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/MSDNet.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/MSDNet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/__init__.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/brain_age.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/brain_age.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/deep_unet.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/deep_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/densenet.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/densenet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/efficientnet.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/fcn.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/fcn.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/imagenet_unet.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/imagenet_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/imagenet_vgg.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/imagenet_vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/light_unet.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/light_unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/light_unet_multilayer.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/light_unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/modelBase.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/modelBase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/resnet.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/resnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/sdnet.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/sdnet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/DecodingModule.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/DecodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/DownsamplingModule.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/DownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/EncodingModule.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/EncodingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/FCNUpsamplingModule.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/FCNUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/IncConv.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/IncConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/IncDownsamplingModule.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/IncDownsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/IncDropout.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/IncDropout.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/IncUpsamplingModule.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/IncUpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/InceptionModule.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/InceptionModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/InitialConv.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/InitialConv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/Interpolate.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/Interpolate.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/ResNetModule.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/ResNetModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/UpsamplingModule.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/UpsamplingModule.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/add_conv_block.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/add_conv_block.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/average_pool.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/average_pool.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/seg_modules/out_conv.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/seg_modules/out_conv.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/transunet.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/transunet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/uinc.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/uinc.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/unet.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/unet.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/unet_multilayer.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/unet_multilayer.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/unetr.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/unetr.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/models/vgg.py` & `GANDLF-0.0.17.dev20230726/GANDLF/models/vgg.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/optimizers/__init__.py` & `GANDLF-0.0.17.dev20230726/GANDLF/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/optimizers/wrap_torch.py` & `GANDLF-0.0.17.dev20230726/GANDLF/optimizers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/parseConfig.py` & `GANDLF-0.0.17.dev20230726/GANDLF/parseConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 }
 
 ## dictionary to define string defaults for appropriate options
 parameter_defaults_string = {
     "optimizer": "adam",  # the optimizer
     "patch_sampler": "uniform",  # type of sampling strategy
     "scheduler": "triangle_modified",  # the default scheduler
-    "loss_function": "dc",  # default loss
     "clip_mode": None,  # default clip mode
 }
 
 
 def initialize_parameter(params, parameter_to_initialize, value=None, evaluate=True):
     """
     Initializes the specified parameter with supplied value
@@ -182,14 +181,19 @@
                         params["loss_function"] = key
         else:
             # check if user has passed a single string
             if params["loss_function"] == "mse":
                 params["loss_function"] = {}
                 params["loss_function"]["mse"] = {}
                 params["loss_function"]["mse"]["reduction"] = "mean"
+            elif params["loss_function"] == "focal":
+                params["loss_function"] = {}
+                params["loss_function"]["focal"] = {}
+                params["loss_function"]["focal"]["gamma"] = 2.0
+                params["loss_function"]["focal"]["size_average"] = True
 
     assert "metrics" in params, "'metrics' needs to be defined in the config file"
     if "metrics" in params:
         if not isinstance(params["metrics"], dict):
             temp_dict = {}
         else:
             temp_dict = params["metrics"]
```

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/schedulers/__init__.py` & `GANDLF-0.0.17.dev20230726/GANDLF/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/schedulers/wrap_torch.py` & `GANDLF-0.0.17.dev20230726/GANDLF/schedulers/wrap_torch.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/training_manager.py` & `GANDLF-0.0.17.dev20230726/GANDLF/training_manager.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/utils/__init__.py` & `GANDLF-0.0.17.dev20230726/GANDLF/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/utils/generic.py` & `GANDLF-0.0.17.dev20230726/GANDLF/utils/generic.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/utils/handle_collisions.py` & `GANDLF-0.0.17.dev20230726/GANDLF/utils/handle_collisions.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/utils/imaging.py` & `GANDLF-0.0.17.dev20230726/GANDLF/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/utils/modelbase.py` & `GANDLF-0.0.17.dev20230726/GANDLF/utils/modelbase.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/utils/modelio.py` & `GANDLF-0.0.17.dev20230726/GANDLF/utils/modelio.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/utils/parameter_processing.py` & `GANDLF-0.0.17.dev20230726/GANDLF/utils/parameter_processing.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/utils/tensor.py` & `GANDLF-0.0.17.dev20230726/GANDLF/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF/utils/write_parse.py` & `GANDLF-0.0.17.dev20230726/GANDLF/utils/write_parse.py`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF.egg-info/PKG-INFO` & `GANDLF-0.0.17.dev20230726/GANDLF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230725
+Version: 0.0.17.dev20230726
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230725 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230726 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230725/GANDLF.egg-info/SOURCES.txt` & `GANDLF-0.0.17.dev20230726/GANDLF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/LICENSE` & `GANDLF-0.0.17.dev20230726/LICENSE`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/PKG-INFO` & `GANDLF-0.0.17.dev20230726/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GANDLF
-Version: 0.0.17.dev20230725
+Version: 0.0.17.dev20230726
 Summary: PyTorch-based framework that handles segmentation/regression/classification using various DL architectures for medical imaging.
 Author: MLCommons
 Author-email: gandlf@mlcommons.org
 License: Apache-2.0
 Keywords: semantic,segmentation,regression,classification,data-augmentation,medical-imaging,clinical-workflows,deep-learning,pytorch
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230725 Summary:
+Metadata-Version: 2.1 Name: GANDLF Version: 0.0.17.dev20230726 Summary:
 PyTorch-based framework that handles segmentation/regression/classification
 using various DL architectures for medical imaging. Author: MLCommons Author-
 email: gandlf@mlcommons.org License: Apache-2.0 Keywords:
 semantic,segmentation,regression,classification,data-augmentation,medical-
 imaging,clinical-workflows,deep-learning,pytorch Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
```

### Comparing `GANDLF-0.0.17.dev20230725/README.md` & `GANDLF-0.0.17.dev20230726/README.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/SECURITY.md` & `GANDLF-0.0.17.dev20230726/SECURITY.md`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/gandlf_anonymizer` & `GANDLF-0.0.17.dev20230726/gandlf_anonymizer`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/gandlf_collectStats` & `GANDLF-0.0.17.dev20230726/gandlf_collectStats`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/gandlf_configGenerator` & `GANDLF-0.0.17.dev20230726/gandlf_configGenerator`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/gandlf_constructCSV` & `GANDLF-0.0.17.dev20230726/gandlf_constructCSV`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/gandlf_deploy` & `GANDLF-0.0.17.dev20230726/gandlf_deploy`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/gandlf_generateMetrics` & `GANDLF-0.0.17.dev20230726/gandlf_generateMetrics`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/gandlf_optimizeModel` & `GANDLF-0.0.17.dev20230726/gandlf_optimizeModel`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/gandlf_patchMiner` & `GANDLF-0.0.17.dev20230726/gandlf_patchMiner`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/gandlf_preprocess` & `GANDLF-0.0.17.dev20230726/gandlf_preprocess`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/gandlf_recoverConfig` & `GANDLF-0.0.17.dev20230726/gandlf_recoverConfig`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/gandlf_run` & `GANDLF-0.0.17.dev20230726/gandlf_run`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/gandlf_verifyInstall` & `GANDLF-0.0.17.dev20230726/gandlf_verifyInstall`

 * *Files identical despite different names*

### Comparing `GANDLF-0.0.17.dev20230725/setup.py` & `GANDLF-0.0.17.dev20230726/setup.py`

 * *Files identical despite different names*

