# Comparing `tmp/adbench-0.1.7.tar.gz` & `tmp/adbench-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\adbench-0.1.7.tar", last modified: Fri Jul 21 08:19:18 2023, max compression
+gzip compressed data, was "dist\adbench-0.1.8.tar", last modified: Wed Jul 26 14:39:52 2023, max compression
```

## Comparing `adbench-0.1.7.tar` & `adbench-0.1.8.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/
--rw-rw-rw-   0        0        0     1349 2023-07-08 02:17:37.000000 adbench-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       79 2023-07-17 08:18:24.000000 adbench-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      950 2023-07-21 08:19:18.000000 adbench-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    22703 2023-07-20 08:54:10.000000 adbench-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/
--rw-rw-rw-   0        0        0       79 2023-07-17 11:51:08.000000 adbench-0.1.7/adbench/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/Customized/
--rw-rw-rw-   0        0        0        0 2023-07-20 03:36:50.000000 adbench-0.1.7/adbench/baseline/Customized/__init__.py
--rw-rw-rw-   0        0        0       84 2023-07-17 15:06:50.000000 adbench-0.1.7/adbench/baseline/Customized/fit.py
--rw-rw-rw-   0        0        0      169 2023-07-17 15:06:50.000000 adbench-0.1.7/adbench/baseline/Customized/model.py
--rw-rw-rw-   0        0        0      843 2023-07-17 15:06:50.000000 adbench-0.1.7/adbench/baseline/Customized/run.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/DAGMM/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.7/adbench/baseline/DAGMM/__init__.py
--rw-rw-rw-   0        0        0     3287 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DAGMM/forward_step.py
--rw-rw-rw-   0        0        0     1941 2023-07-17 12:11:45.000000 adbench-0.1.7/adbench/baseline/DAGMM/main.py
--rw-rw-rw-   0        0        0     1775 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DAGMM/model.py
--rw-rw-rw-   0        0        0     2003 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DAGMM/preprocess.py
--rw-rw-rw-   0        0        0     4209 2023-07-17 12:11:45.000000 adbench-0.1.7/adbench/baseline/DAGMM/run.py
--rw-rw-rw-   0        0        0     5384 2023-07-12 01:46:26.000000 adbench-0.1.7/adbench/baseline/DAGMM/test.py
--rw-rw-rw-   0        0        0     1915 2023-07-17 12:11:45.000000 adbench-0.1.7/adbench/baseline/DAGMM/train.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/DAGMM/utils/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.7/adbench/baseline/DAGMM/utils/__init__.py
--rw-rw-rw-   0        0        0      528 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DAGMM/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/DeepSAD/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.7/adbench/baseline/DeepSAD/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/base/
--rw-rw-rw-   0        0        0      148 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/base/__init__.py
--rw-rw-rw-   0        0        0     1032 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/base/base_dataset.py
--rw-rw-rw-   0        0        0      823 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/base/base_net.py
--rw-rw-rw-   0        0        0     1166 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/base/base_trainer.py
--rw-rw-rw-   0        0        0     1682 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/base/odds_dataset.py
--rw-rw-rw-   0        0        0      846 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/base/torchvision_dataset.py
--rw-rw-rw-   0        0        0    13565 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/baseline_SemiDGM.py
--rw-rw-rw-   0        0        0     9937 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/baseline_isoforest.py
--rw-rw-rw-   0        0        0     9478 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/baseline_kde.py
--rw-rw-rw-   0        0        0     9062 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/baseline_ocsvm.py
--rw-rw-rw-   0        0        0     9157 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/baseline_ssad.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/
--rw-rw-rw-   0        0        0     5610 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/SemiDGM.py
--rw-rw-rw-   0        0        0      202 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/__init__.py
--rw-rw-rw-   0        0        0     5879 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/isoforest.py
--rw-rw-rw-   0        0        0     6702 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/kde.py
--rw-rw-rw-   0        0        0     9033 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/ocsvm.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/shallow_ssad/
--rw-rw-rw-   0        0        0       37 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/shallow_ssad/__init__.py
--rw-rw-rw-   0        0        0     8022 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/shallow_ssad/ssad_convex.py
--rw-rw-rw-   0        0        0    10201 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/ssad.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/datasets/
--rw-rw-rw-   0        0        0      215 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/datasets/__init__.py
--rw-rw-rw-   0        0        0     3609 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/datasets/cifar10.py
--rw-rw-rw-   0        0        0     3663 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/datasets/fmnist.py
--rw-rw-rw-   0        0        0      325 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/datasets/main.py
--rw-rw-rw-   0        0        0     3606 2023-07-12 01:46:27.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/datasets/mnist.py
--rw-rw-rw-   0        0        0     1389 2023-07-12 01:46:27.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/datasets/odds.py
--rw-rw-rw-   0        0        0     3629 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/datasets/preprocessing.py
--rw-rw-rw-   0        0        0     7054 2023-07-12 01:46:27.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/deepsad.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/
--rw-rw-rw-   0        0        0      706 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/__init__.py
--rw-rw-rw-   0        0        0     3085 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/cifar10_LeNet.py
--rw-rw-rw-   0        0        0     4405 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/dgm.py
--rw-rw-rw-   0        0        0     2584 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/fmnist_LeNet.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/inference/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/inference/__init__.py
--rw-rw-rw-   0        0        0     1256 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/inference/distributions.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/layers/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/layers/__init__.py
--rw-rw-rw-   0        0        0     1705 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/layers/standard.py
--rw-rw-rw-   0        0        0     1511 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/layers/stochastic.py
--rw-rw-rw-   0        0        0     1501 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/main.py
--rw-rw-rw-   0        0        0     2327 2023-07-12 01:46:26.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/mlp.py
--rw-rw-rw-   0        0        0     2222 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/mnist_LeNet.py
--rw-rw-rw-   0        0        0     4826 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/vae.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/optim/
--rw-rw-rw-   0        0        0     7050 2023-07-12 01:46:27.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/optim/DeepSAD_trainer.py
--rw-rw-rw-   0        0        0     7565 2023-07-17 12:35:57.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/optim/SemiDGM_trainer.py
--rw-rw-rw-   0        0        0      228 2023-07-17 12:35:19.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/optim/__init__.py
--rw-rw-rw-   0        0        0     5381 2023-07-12 01:46:27.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/optim/ae_trainer.py
--rw-rw-rw-   0        0        0     5252 2023-07-12 01:46:27.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/optim/vae_trainer.py
--rw-rw-rw-   0        0        0     2832 2023-07-12 01:46:27.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/optim/variational.py
--rw-rw-rw-   0        0        0     4957 2023-07-11 01:16:07.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/run.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/utils/
--rw-rw-rw-   0        0        0      163 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/utils/__init__.py
--rw-rw-rw-   0        0        0      682 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/utils/config.py
--rw-rw-rw-   0        0        0     1468 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/utils/misc.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/utils/visualization/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/utils/visualization/__init__.py
--rw-rw-rw-   0        0        0      803 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DeepSAD/src/utils/visualization/plot_images_grid.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/DevNet/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.7/adbench/baseline/DevNet/__init__.py
--rw-rw-rw-   0        0        0    10603 2023-07-17 12:37:39.000000 adbench-0.1.7/adbench/baseline/DevNet/run.py
--rw-rw-rw-   0        0        0     2367 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/DevNet/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/FEAWAD/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.7/adbench/baseline/FEAWAD/__init__.py
--rw-rw-rw-   0        0        0    18613 2023-07-12 00:41:49.000000 adbench-0.1.7/adbench/baseline/FEAWAD/run.py
--rw-rw-rw-   0        0        0     1533 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/FEAWAD/toolsdev.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/FTTransformer/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.7/adbench/baseline/FTTransformer/__init__.py
--rw-rw-rw-   0        0        0     6098 2023-07-11 01:16:07.000000 adbench-0.1.7/adbench/baseline/FTTransformer/run.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/GANomaly/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.7/adbench/baseline/GANomaly/__init__.py
--rw-rw-rw-   0        0        0     2878 2023-07-12 01:46:27.000000 adbench-0.1.7/adbench/baseline/GANomaly/fit.py
--rw-rw-rw-   0        0        0     1260 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/GANomaly/model.py
--rw-rw-rw-   0        0        0     2998 2023-07-17 12:11:45.000000 adbench-0.1.7/adbench/baseline/GANomaly/run.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/PReNet/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.7/adbench/baseline/PReNet/__init__.py
--rw-rw-rw-   0        0        0     1227 2023-07-17 12:38:15.000000 adbench-0.1.7/adbench/baseline/PReNet/fit.py
--rw-rw-rw-   0        0        0      703 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/PReNet/model.py
--rw-rw-rw-   0        0        0     2952 2023-07-12 01:46:27.000000 adbench-0.1.7/adbench/baseline/PReNet/run.py
--rw-rw-rw-   0        0        0     2931 2023-07-11 01:16:07.000000 adbench-0.1.7/adbench/baseline/PReNet/utils.py
--rw-rw-rw-   0        0        0    13241 2023-07-11 01:16:07.000000 adbench-0.1.7/adbench/baseline/PyOD.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/baseline/REPEN/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.7/adbench/baseline/REPEN/__init__.py
--rw-rw-rw-   0        0        0    12481 2023-07-12 00:46:22.000000 adbench-0.1.7/adbench/baseline/REPEN/model.py
--rw-rw-rw-   0        0        0     1928 2023-07-17 12:37:11.000000 adbench-0.1.7/adbench/baseline/REPEN/run.py
--rw-rw-rw-   0        0        0     2011 2023-07-08 02:17:37.000000 adbench-0.1.7/adbench/baseline/REPEN/utils.py
--rw-rw-rw-   0        0        0     1491 2023-07-11 01:16:07.000000 adbench-0.1.7/adbench/baseline/Supervised.py
--rw-rw-rw-   0        0        0       79 2023-07-17 11:47:13.000000 adbench-0.1.7/adbench/baseline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/datasets/
--rw-rw-rw-   0        0        0       79 2023-07-17 11:51:08.000000 adbench-0.1.7/adbench/datasets/__init__.py
--rw-rw-rw-   0        0        0    17216 2023-07-17 13:23:37.000000 adbench-0.1.7/adbench/datasets/data_generator.py
--rw-rw-rw-   0        0        0    14376 2023-07-21 08:18:56.000000 adbench-0.1.7/adbench/myutils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/other_utils/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:49:49.000000 adbench-0.1.7/adbench/other_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench/other_utils/gmm/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:49:49.000000 adbench-0.1.7/adbench/other_utils/gmm/__init__.py
--rw-rw-rw-   0        0        0     2111 2023-07-08 02:17:46.000000 adbench-0.1.7/adbench/other_utils/gmm/example.py
--rw-rw-rw-   0        0        0    19823 2023-07-12 01:49:59.000000 adbench-0.1.7/adbench/other_utils/gmm/gmm.py
--rw-rw-rw-   0        0        0     6856 2023-07-08 02:17:46.000000 adbench-0.1.7/adbench/other_utils/gmm/test.py
--rw-rw-rw-   0        0        0     1129 2023-07-08 02:17:46.000000 adbench-0.1.7/adbench/other_utils/gmm/utils.py
--rw-rw-rw-   0        0        0    14138 2023-07-08 02:17:46.000000 adbench-0.1.7/adbench/other_utils/utils.py
--rw-rw-rw-   0        0        0    17380 2023-07-19 15:57:03.000000 adbench-0.1.7/adbench/run.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench.egg-info/
--rw-rw-rw-   0        0        0      950 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4566 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-21 08:19:18.000000 adbench-0.1.7/adbench.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      131 2023-07-20 01:30:38.000000 adbench-0.1.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 08:19:18.000000 adbench-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1393 2023-07-21 08:18:56.000000 adbench-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/
+-rw-rw-rw-   0        0        0     1349 2023-07-08 02:17:37.000000 adbench-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       79 2023-07-17 08:18:24.000000 adbench-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      950 2023-07-26 14:39:52.000000 adbench-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    23234 2023-07-26 14:39:11.000000 adbench-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:51.000000 adbench-0.1.8/adbench/
+-rw-rw-rw-   0        0        0       79 2023-07-17 11:51:08.000000 adbench-0.1.8/adbench/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:51.000000 adbench-0.1.8/adbench/baseline/
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:51.000000 adbench-0.1.8/adbench/baseline/Customized/
+-rw-rw-rw-   0        0        0        0 2023-07-20 03:36:50.000000 adbench-0.1.8/adbench/baseline/Customized/__init__.py
+-rw-rw-rw-   0        0        0       84 2023-07-17 15:06:50.000000 adbench-0.1.8/adbench/baseline/Customized/fit.py
+-rw-rw-rw-   0        0        0      169 2023-07-17 15:06:50.000000 adbench-0.1.8/adbench/baseline/Customized/model.py
+-rw-rw-rw-   0        0        0      843 2023-07-17 15:06:50.000000 adbench-0.1.8/adbench/baseline/Customized/run.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:51.000000 adbench-0.1.8/adbench/baseline/DAGMM/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.8/adbench/baseline/DAGMM/__init__.py
+-rw-rw-rw-   0        0        0     3287 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DAGMM/forward_step.py
+-rw-rw-rw-   0        0        0     1941 2023-07-17 12:11:45.000000 adbench-0.1.8/adbench/baseline/DAGMM/main.py
+-rw-rw-rw-   0        0        0     1775 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DAGMM/model.py
+-rw-rw-rw-   0        0        0     2003 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DAGMM/preprocess.py
+-rw-rw-rw-   0        0        0     4209 2023-07-17 12:11:45.000000 adbench-0.1.8/adbench/baseline/DAGMM/run.py
+-rw-rw-rw-   0        0        0     5384 2023-07-12 01:46:26.000000 adbench-0.1.8/adbench/baseline/DAGMM/test.py
+-rw-rw-rw-   0        0        0     1915 2023-07-17 12:11:45.000000 adbench-0.1.8/adbench/baseline/DAGMM/train.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:51.000000 adbench-0.1.8/adbench/baseline/DAGMM/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.8/adbench/baseline/DAGMM/utils/__init__.py
+-rw-rw-rw-   0        0        0      528 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DAGMM/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:51.000000 adbench-0.1.8/adbench/baseline/DeepSAD/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.8/adbench/baseline/DeepSAD/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:51.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:51.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/base/
+-rw-rw-rw-   0        0        0      148 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/base/__init__.py
+-rw-rw-rw-   0        0        0     1032 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/base/base_dataset.py
+-rw-rw-rw-   0        0        0      823 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/base/base_net.py
+-rw-rw-rw-   0        0        0     1166 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/base/base_trainer.py
+-rw-rw-rw-   0        0        0     1682 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/base/odds_dataset.py
+-rw-rw-rw-   0        0        0      846 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/base/torchvision_dataset.py
+-rw-rw-rw-   0        0        0    13565 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/baseline_SemiDGM.py
+-rw-rw-rw-   0        0        0     9937 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/baseline_isoforest.py
+-rw-rw-rw-   0        0        0     9478 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/baseline_kde.py
+-rw-rw-rw-   0        0        0     9062 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/baseline_ocsvm.py
+-rw-rw-rw-   0        0        0     9157 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/baseline_ssad.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:51.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/
+-rw-rw-rw-   0        0        0     5610 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/SemiDGM.py
+-rw-rw-rw-   0        0        0      202 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/__init__.py
+-rw-rw-rw-   0        0        0     5879 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/isoforest.py
+-rw-rw-rw-   0        0        0     6702 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/kde.py
+-rw-rw-rw-   0        0        0     9033 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/ocsvm.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/shallow_ssad/
+-rw-rw-rw-   0        0        0       37 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/shallow_ssad/__init__.py
+-rw-rw-rw-   0        0        0     8022 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/shallow_ssad/ssad_convex.py
+-rw-rw-rw-   0        0        0    10201 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/ssad.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/datasets/
+-rw-rw-rw-   0        0        0      215 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/datasets/__init__.py
+-rw-rw-rw-   0        0        0     3609 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/datasets/cifar10.py
+-rw-rw-rw-   0        0        0     3663 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/datasets/fmnist.py
+-rw-rw-rw-   0        0        0      325 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/datasets/main.py
+-rw-rw-rw-   0        0        0     3606 2023-07-12 01:46:27.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/datasets/mnist.py
+-rw-rw-rw-   0        0        0     1389 2023-07-12 01:46:27.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/datasets/odds.py
+-rw-rw-rw-   0        0        0     3629 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/datasets/preprocessing.py
+-rw-rw-rw-   0        0        0     7054 2023-07-12 01:46:27.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/deepsad.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/
+-rw-rw-rw-   0        0        0      706 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/__init__.py
+-rw-rw-rw-   0        0        0     3085 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/cifar10_LeNet.py
+-rw-rw-rw-   0        0        0     4405 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/dgm.py
+-rw-rw-rw-   0        0        0     2584 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/fmnist_LeNet.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/inference/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/inference/__init__.py
+-rw-rw-rw-   0        0        0     1256 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/inference/distributions.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/layers/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/layers/__init__.py
+-rw-rw-rw-   0        0        0     1705 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/layers/standard.py
+-rw-rw-rw-   0        0        0     1511 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/layers/stochastic.py
+-rw-rw-rw-   0        0        0     1501 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/main.py
+-rw-rw-rw-   0        0        0     2327 2023-07-12 01:46:26.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/mlp.py
+-rw-rw-rw-   0        0        0     2222 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/mnist_LeNet.py
+-rw-rw-rw-   0        0        0     4826 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/vae.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/optim/
+-rw-rw-rw-   0        0        0     7050 2023-07-12 01:46:27.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/optim/DeepSAD_trainer.py
+-rw-rw-rw-   0        0        0     7565 2023-07-17 12:35:57.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/optim/SemiDGM_trainer.py
+-rw-rw-rw-   0        0        0      228 2023-07-17 12:35:19.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/optim/__init__.py
+-rw-rw-rw-   0        0        0     5381 2023-07-12 01:46:27.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/optim/ae_trainer.py
+-rw-rw-rw-   0        0        0     5252 2023-07-12 01:46:27.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/optim/vae_trainer.py
+-rw-rw-rw-   0        0        0     2832 2023-07-12 01:46:27.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/optim/variational.py
+-rw-rw-rw-   0        0        0     4957 2023-07-11 01:16:07.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/run.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/utils/
+-rw-rw-rw-   0        0        0      163 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      682 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/utils/config.py
+-rw-rw-rw-   0        0        0     1468 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/utils/misc.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/utils/visualization/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/utils/visualization/__init__.py
+-rw-rw-rw-   0        0        0      803 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DeepSAD/src/utils/visualization/plot_images_grid.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/baseline/DevNet/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.8/adbench/baseline/DevNet/__init__.py
+-rw-rw-rw-   0        0        0    10603 2023-07-17 12:37:39.000000 adbench-0.1.8/adbench/baseline/DevNet/run.py
+-rw-rw-rw-   0        0        0     2367 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/DevNet/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/baseline/FEAWAD/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.8/adbench/baseline/FEAWAD/__init__.py
+-rw-rw-rw-   0        0        0    18613 2023-07-12 00:41:49.000000 adbench-0.1.8/adbench/baseline/FEAWAD/run.py
+-rw-rw-rw-   0        0        0     1533 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/FEAWAD/toolsdev.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/baseline/FTTransformer/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.8/adbench/baseline/FTTransformer/__init__.py
+-rw-rw-rw-   0        0        0     6098 2023-07-11 01:16:07.000000 adbench-0.1.8/adbench/baseline/FTTransformer/run.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/baseline/GANomaly/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.8/adbench/baseline/GANomaly/__init__.py
+-rw-rw-rw-   0        0        0     2878 2023-07-12 01:46:27.000000 adbench-0.1.8/adbench/baseline/GANomaly/fit.py
+-rw-rw-rw-   0        0        0     1260 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/GANomaly/model.py
+-rw-rw-rw-   0        0        0     2998 2023-07-17 12:11:45.000000 adbench-0.1.8/adbench/baseline/GANomaly/run.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/baseline/PReNet/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.8/adbench/baseline/PReNet/__init__.py
+-rw-rw-rw-   0        0        0     1227 2023-07-17 12:38:15.000000 adbench-0.1.8/adbench/baseline/PReNet/fit.py
+-rw-rw-rw-   0        0        0      703 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/PReNet/model.py
+-rw-rw-rw-   0        0        0     2952 2023-07-12 01:46:27.000000 adbench-0.1.8/adbench/baseline/PReNet/run.py
+-rw-rw-rw-   0        0        0     2931 2023-07-11 01:16:07.000000 adbench-0.1.8/adbench/baseline/PReNet/utils.py
+-rw-rw-rw-   0        0        0    13241 2023-07-11 01:16:07.000000 adbench-0.1.8/adbench/baseline/PyOD.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/baseline/REPEN/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:40:30.000000 adbench-0.1.8/adbench/baseline/REPEN/__init__.py
+-rw-rw-rw-   0        0        0    12481 2023-07-12 00:46:22.000000 adbench-0.1.8/adbench/baseline/REPEN/model.py
+-rw-rw-rw-   0        0        0     1928 2023-07-17 12:37:11.000000 adbench-0.1.8/adbench/baseline/REPEN/run.py
+-rw-rw-rw-   0        0        0     2011 2023-07-08 02:17:37.000000 adbench-0.1.8/adbench/baseline/REPEN/utils.py
+-rw-rw-rw-   0        0        0     1491 2023-07-11 01:16:07.000000 adbench-0.1.8/adbench/baseline/Supervised.py
+-rw-rw-rw-   0        0        0       79 2023-07-17 11:47:13.000000 adbench-0.1.8/adbench/baseline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/datasets/
+-rw-rw-rw-   0        0        0       79 2023-07-17 11:51:08.000000 adbench-0.1.8/adbench/datasets/__init__.py
+-rw-rw-rw-   0        0        0    17216 2023-07-17 13:23:37.000000 adbench-0.1.8/adbench/datasets/data_generator.py
+-rw-rw-rw-   0        0        0    16773 2023-07-26 14:37:06.000000 adbench-0.1.8/adbench/myutils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/other_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:49:49.000000 adbench-0.1.8/adbench/other_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:52.000000 adbench-0.1.8/adbench/other_utils/gmm/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:49:49.000000 adbench-0.1.8/adbench/other_utils/gmm/__init__.py
+-rw-rw-rw-   0        0        0     2111 2023-07-08 02:17:46.000000 adbench-0.1.8/adbench/other_utils/gmm/example.py
+-rw-rw-rw-   0        0        0    19823 2023-07-12 01:49:59.000000 adbench-0.1.8/adbench/other_utils/gmm/gmm.py
+-rw-rw-rw-   0        0        0     6856 2023-07-08 02:17:46.000000 adbench-0.1.8/adbench/other_utils/gmm/test.py
+-rw-rw-rw-   0        0        0     1129 2023-07-08 02:17:46.000000 adbench-0.1.8/adbench/other_utils/gmm/utils.py
+-rw-rw-rw-   0        0        0    14138 2023-07-08 02:17:46.000000 adbench-0.1.8/adbench/other_utils/utils.py
+-rw-rw-rw-   0        0        0    17380 2023-07-19 15:57:03.000000 adbench-0.1.8/adbench/run.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:39:51.000000 adbench-0.1.8/adbench.egg-info/
+-rw-rw-rw-   0        0        0      950 2023-07-26 14:39:51.000000 adbench-0.1.8/adbench.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4566 2023-07-26 14:39:51.000000 adbench-0.1.8/adbench.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 14:39:51.000000 adbench-0.1.8/adbench.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-07-26 14:39:51.000000 adbench-0.1.8/adbench.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 14:39:51.000000 adbench-0.1.8/adbench.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      131 2023-07-20 01:30:38.000000 adbench-0.1.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 14:39:52.000000 adbench-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1393 2023-07-26 14:39:23.000000 adbench-0.1.8/setup.py
```

### Comparing `adbench-0.1.7/LICENSE` & `adbench-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/PKG-INFO` & `adbench-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbench
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python package of ADBench
 Home-page: https://github.com/Minqi824/ADBench
 Author: Minqi Jiang
 Author-email: <jiangmq95@163.com>
 Keywords: anomaly detection,outlier detection,tabular data,benchmark
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `adbench-0.1.7/README.md` & `adbench-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -100,16 +100,16 @@
 ```
 
 _Prerequisite: Downloading datasets in ADBench from the github repo_
 ```python
 from adbench.myutils import Utils
 utils = Utils() # utility function
 # download datasets from the remote github repo
-# we recommend gitee for China mainland user and github otherwise
-utils.download_datasets(repo='gitee')
+# we recommend tianchi for China mainland user and github otherwise
+utils.download_datasets(repo='tianchi')
 ```
 
 ### Quickly implement ADBench for benchmarking AD algorithms.
 We present the following example for quickly implementing ADBench in _three different Angles_ illustrated
 in the paper. Currently, [57 datasets](#datasets) can be used for evaluating [30 algorithms](#algorithms) in ADBench,
 and we encourage to test your customized datasets/algorithms in our ADBench testbed.
 
@@ -132,27 +132,33 @@
 noise type: evaluating algorithms on 'duplicated_anomalies', 'irrelevant_features' and 'label_contamination',
 corresponding to the Angle III: Model Robustness with Noisy and Corrupted Data.
 '''
 
 # return the results including [params, model_name, metrics, time_fit, time_inference]
 # besides, results will be automatically saved in the dataframe and ouputted as csv file in adbench/result folder
 pipeline = RunPipeline(suffix='ADBench', parallel='semi-supervise', realistic_synthetic_mode=None, noise_type=None)
-pipeline.run()
+results = pipeline.run()
 
 pipeline = RunPipeline(suffix='ADBench', parallel='unsupervise', realistic_synthetic_mode='cluster', noise_type=None)
 results = pipeline.run()
 
 pipeline = RunPipeline(suffix='ADBench', parallel='supervise', realistic_synthetic_mode=None, noise_type='irrelevant_features')
 results = pipeline.run()
 ```
 
 **_Run Your Customized Algorithms on either ADBench Datasets or Your Customized Dataset_**
 ```python
 # customized model on ADBench's datasets
+from adbench.run import RunPipeline
 from adbench.baseline.Customized.run import Customized
+
+# notice that you should specify the corresponding category of your customized AD algorithm
+# for example, here we use Logistic Regression as customized clf, which belongs to the supervised algorithm
+# for your own algorithm, you can realize the same usage as other baselines by modifying the fit.py, model.py, and run.py files in the adbench/baseline/Customized
+pipeline = RunPipeline(suffix='ADBench', parallel='supervise', realistic_synthetic_mode=None, noise_type=None)
 results = pipeline.run(clf=Customized)
 
 # customized model on customized dataset
 import numpy as np
 dataset = {}
 dataset['X'] = np.random.randn(1000, 20)
 dataset['y'] = np.random.choice([0, 1], 1000)
```

#### html2text {}

```diff
@@ -57,18 +57,18 @@
 [comment]: <> (- keras) [comment]: <> (- tensorflow) [comment]: <> (- delu)
 [comment]: <> (- lightgbm) [comment]: <> (- xgboost) [comment]: <> (- catboost
 ) [comment]: <> (- copulas) [comment]: <> (- combo) [comment]: <> (- barbar) We
 provide full guidance of ADBench in the [notebook](guidance.ipynb). ###
 Installation ```python pip install adbench pip install --upgrade adbench ```
 _Prerequisite: Downloading datasets in ADBench from the github repo_ ```python
 from adbench.myutils import Utils utils = Utils() # utility function # download
-datasets from the remote github repo # we recommend gitee for China mainland
-user and github otherwise utils.download_datasets(repo='gitee') ``` ### Quickly
-implement ADBench for benchmarking AD algorithms. We present the following
-example for quickly implementing ADBench in _three different Angles_
+datasets from the remote github repo # we recommend tianchi for China mainland
+user and github otherwise utils.download_datasets(repo='tianchi') ``` ###
+Quickly implement ADBench for benchmarking AD algorithms. We present the
+following example for quickly implementing ADBench in _three different Angles_
 illustrated in the paper. Currently, [57 datasets](#datasets) can be used for
 evaluating [30 algorithms](#algorithms) in ADBench, and we encourage to test
 your customized datasets/algorithms in our ADBench testbed. **_Run Entire
 Experiments of ADBench_** ```python from adbench.run import RunPipeline '''
 Params: suffix: file name suffix; parallel: running either 'unsupervise',
 'semi-supervise', or 'supervise' (AD) algorithms, corresponding to the Angle I:
 Availability of Ground Truth Labels (Supervision); realistic_synthetic_mode:
@@ -76,22 +76,29 @@
 corresponding to the Angle II: Types of Anomalies; noise type: evaluating
 algorithms on 'duplicated_anomalies', 'irrelevant_features' and
 'label_contamination', corresponding to the Angle III: Model Robustness with
 Noisy and Corrupted Data. ''' # return the results including [params,
 model_name, metrics, time_fit, time_inference] # besides, results will be
 automatically saved in the dataframe and ouputted as csv file in adbench/result
 folder pipeline = RunPipeline(suffix='ADBench', parallel='semi-supervise',
-realistic_synthetic_mode=None, noise_type=None) pipeline.run() pipeline =
-RunPipeline(suffix='ADBench', parallel='unsupervise',
+realistic_synthetic_mode=None, noise_type=None) results = pipeline.run()
+pipeline = RunPipeline(suffix='ADBench', parallel='unsupervise',
 realistic_synthetic_mode='cluster', noise_type=None) results = pipeline.run()
 pipeline = RunPipeline(suffix='ADBench', parallel='supervise',
 realistic_synthetic_mode=None, noise_type='irrelevant_features') results =
 pipeline.run() ``` **_Run Your Customized Algorithms on either ADBench Datasets
 or Your Customized Dataset_** ```python # customized model on ADBench's
-datasets from adbench.baseline.Customized.run import Customized results =
+datasets from adbench.run import RunPipeline from
+adbench.baseline.Customized.run import Customized # notice that you should
+specify the corresponding category of your customized AD algorithm # for
+example, here we use Logistic Regression as customized clf, which belongs to
+the supervised algorithm # for your own algorithm, you can realize the same
+usage as other baselines by modifying the fit.py, model.py, and run.py files in
+the adbench/baseline/Customized pipeline = RunPipeline(suffix='ADBench',
+parallel='supervise', realistic_synthetic_mode=None, noise_type=None) results =
 pipeline.run(clf=Customized) # customized model on customized dataset import
 numpy as np dataset = {} dataset['X'] = np.random.randn(1000, 20) dataset['y']
 = np.random.choice([0, 1], 1000) results = pipeline.run(dataset=dataset,
 clf=Customized) ``` See detailed guidance of ADBench in the [notebook]
 (guidance.ipynb). ### Datasets ADBench includes [57 datasets](https://
 github.com/Minqi824/ADBench/tree/main/datasets), as shown in the following
 Table. - Among them, **47 widely-used real-world datasets** are gathered for
```

### Comparing `adbench-0.1.7/adbench/baseline/Customized/run.py` & `adbench-0.1.8/adbench/baseline/Customized/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DAGMM/forward_step.py` & `adbench-0.1.8/adbench/baseline/DAGMM/forward_step.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DAGMM/main.py` & `adbench-0.1.8/adbench/baseline/DAGMM/main.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DAGMM/model.py` & `adbench-0.1.8/adbench/baseline/DAGMM/model.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DAGMM/preprocess.py` & `adbench-0.1.8/adbench/baseline/DAGMM/preprocess.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DAGMM/run.py` & `adbench-0.1.8/adbench/baseline/DAGMM/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DAGMM/test.py` & `adbench-0.1.8/adbench/baseline/DAGMM/test.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DAGMM/train.py` & `adbench-0.1.8/adbench/baseline/DAGMM/train.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DAGMM/utils/utils.py` & `adbench-0.1.8/adbench/baseline/DAGMM/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/base/base_dataset.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/base/base_dataset.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/base/base_net.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/base/base_net.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/base/base_trainer.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/base/base_trainer.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/base/odds_dataset.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/base/odds_dataset.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/base/torchvision_dataset.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/base/torchvision_dataset.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/baseline_SemiDGM.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/baseline_SemiDGM.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/baseline_isoforest.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/baseline_isoforest.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/baseline_kde.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/baseline_kde.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/baseline_ocsvm.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/baseline_ocsvm.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/baseline_ssad.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/baseline_ssad.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/SemiDGM.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/SemiDGM.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/isoforest.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/isoforest.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/kde.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/kde.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/ocsvm.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/ocsvm.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/shallow_ssad/ssad_convex.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/shallow_ssad/ssad_convex.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/baselines/ssad.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/baselines/ssad.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/datasets/cifar10.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/datasets/fmnist.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/datasets/fmnist.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/datasets/mnist.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/datasets/odds.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/datasets/odds.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/datasets/preprocessing.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/datasets/preprocessing.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/deepsad.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/deepsad.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/__init__.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/cifar10_LeNet.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/cifar10_LeNet.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/dgm.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/dgm.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/fmnist_LeNet.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/fmnist_LeNet.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/inference/distributions.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/inference/distributions.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/layers/standard.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/layers/standard.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/layers/stochastic.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/layers/stochastic.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/main.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/main.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/mlp.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/mlp.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/mnist_LeNet.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/mnist_LeNet.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/networks/vae.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/networks/vae.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/optim/DeepSAD_trainer.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/optim/DeepSAD_trainer.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/optim/SemiDGM_trainer.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/optim/SemiDGM_trainer.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/optim/ae_trainer.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/optim/ae_trainer.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/optim/vae_trainer.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/optim/vae_trainer.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/optim/variational.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/optim/variational.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/run.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/utils/config.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/utils/config.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/utils/misc.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/utils/misc.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DeepSAD/src/utils/visualization/plot_images_grid.py` & `adbench-0.1.8/adbench/baseline/DeepSAD/src/utils/visualization/plot_images_grid.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DevNet/run.py` & `adbench-0.1.8/adbench/baseline/DevNet/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/DevNet/utils.py` & `adbench-0.1.8/adbench/baseline/DevNet/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/FEAWAD/run.py` & `adbench-0.1.8/adbench/baseline/FEAWAD/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/FEAWAD/toolsdev.py` & `adbench-0.1.8/adbench/baseline/FEAWAD/toolsdev.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/FTTransformer/run.py` & `adbench-0.1.8/adbench/baseline/FTTransformer/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/GANomaly/fit.py` & `adbench-0.1.8/adbench/baseline/GANomaly/fit.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/GANomaly/model.py` & `adbench-0.1.8/adbench/baseline/GANomaly/model.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/GANomaly/run.py` & `adbench-0.1.8/adbench/baseline/GANomaly/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/PReNet/fit.py` & `adbench-0.1.8/adbench/baseline/PReNet/fit.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/PReNet/model.py` & `adbench-0.1.8/adbench/baseline/PReNet/model.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/PReNet/run.py` & `adbench-0.1.8/adbench/baseline/PReNet/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/PReNet/utils.py` & `adbench-0.1.8/adbench/baseline/PReNet/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/PyOD.py` & `adbench-0.1.8/adbench/baseline/PyOD.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/REPEN/model.py` & `adbench-0.1.8/adbench/baseline/REPEN/model.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/REPEN/run.py` & `adbench-0.1.8/adbench/baseline/REPEN/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/REPEN/utils.py` & `adbench-0.1.8/adbench/baseline/REPEN/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/baseline/Supervised.py` & `adbench-0.1.8/adbench/baseline/Supervised.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/datasets/data_generator.py` & `adbench-0.1.8/adbench/datasets/data_generator.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/myutils.py` & `adbench-0.1.8/adbench/myutils.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 import random
 import torch
 import tensorflow as tf
 import fsspec
 from tqdm import tqdm
 import requests
 import json
+import time
+import wget
+import zipfile
 # metric
 from sklearn.metrics import roc_auc_score, average_precision_score
 
 # plot
 import matplotlib.pyplot as plt
 
 # statistical analysis
@@ -60,15 +63,15 @@
 
     # generate unique value
     def unique(self, a, b):
         u = 0.5 * (a + b) * (a + b + 1) + b
         return int(u)
 
     # download datasets from the remote git repo
-    def download_datasets(self, repo='gitee'):
+    def download_datasets(self, repo='tianchi'):
         # folder_list = ['CV_by_ResNet18', 'CV_by_ViT', 'NLP_by_BERT', 'NLP_by_RoBERTa', 'Classical']
         folder_list = ['CV_by_ResNet18', 'NLP_by_BERT', 'Classical']
         
         if repo == 'github':
             fs = fsspec.filesystem("github", org="Minqi824", repo="ADBench")
             print(f'Downloading datasets from the remote github repo...')
             for folder in tqdm(folder_list):
@@ -77,14 +80,40 @@
                 if os.path.exists(save_path):
                     print(f'{folder} already exists. Skipping download...')
                     continue
 
                 os.makedirs(save_path, exist_ok=True)
                 fs.get(fs.ls("adbench/datasets/" + folder), save_path, recursive=True)
         
+        elif repo == 'tianchi':
+            print(f'Downloading datasets from aliyun tianchi datasets...')
+            dic_datasetsName2url = {
+                'Classical':'https://tianchi-jupyter-sh.oss-cn-shanghai.aliyuncs.com/file/opensearch/documents/159210/Classical.zip?Expires=1690154932&OSSAccessKeyId=LTAI4GGBCQcb7KD7NwKinA3D&Signature=cBQiIMTuxI12Drz7rSux479RrFM%3D',
+                'CV_by_ResNet18':'https://tianchi-jupyter-sh.oss-cn-shanghai.aliyuncs.com/file/opensearch/documents/159210/CV_by_ResNet18.zip?Expires=1690155534&OSSAccessKeyId=LTAI4GGBCQcb7KD7NwKinA3D&Signature=lG3iXH%2B1PlOCKIdSUt4%2Bb%2FZ4yiA%3D',
+                'NLP_by_BERT':'https://tianchi-jupyter-sh.oss-cn-shanghai.aliyuncs.com/file/opensearch/documents/159210/NLP_by_BERT.zip?Expires=1690155579&OSSAccessKeyId=LTAI4GGBCQcb7KD7NwKinA3D&Signature=EvzKTodvUXNQEZS%2FD2bajY3gpzY%3D',
+                'NLP_by_RoBERTa':'https://tianchi-jupyter-sh.oss-cn-shanghai.aliyuncs.com/file/opensearch/documents/159210/NLP_by_RoBERTa.zip?Expires=1690155694&OSSAccessKeyId=LTAI4GGBCQcb7KD7NwKinA3D&Signature=2%2FtIBZs%2FAkAI79W1Y9qr%2F12Q2I8%3D',
+                'CV_by_Vit':'https://tianchi-jupyter-sh.oss-cn-shanghai.aliyuncs.com/file/opensearch/documents/159210/CV_by_ViT.zip?Expires=1690155712&OSSAccessKeyId=LTAI4GGBCQcb7KD7NwKinA3D&Signature=4EsYCySYZOC0m8xz4GGd8ZEa5hA%3D'
+            } # the link won't work after Friday, December 12, 2023 17:22:12 (in GMT)
+            for folder in tqdm(folder_list):
+                save_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'datasets')
+                print(f'Current saving path: {save_path}')
+                if os.path.exists(os.path.join(save_path, folder)):
+                    print(f'{folder} already exists. Skipping download...')
+                    continue
+                    
+                dataset_url = dic_datasetsName2url[folder]
+                wget.download(dataset_url,out = folder+'.zip') # download the datasets zip
+                zip_file = zipfile.ZipFile(folder+'.zip') # save to the current fold temporarily
+                zip_file.extractall(save_path)
+                
+                zip_file.close()
+                del zip_file
+                time.sleep(1)
+                os.remove(folder+'.zip') # delete the temporary zip file
+                
         elif repo == 'gitee':
             url_repo = 'https://gitee.com/hou-chaochuan/adbench_datasets/raw/master'
             print(f'Downloading datasets from the remote gitee repo...')
             
             # load the datasets path
             # url_dictionary = os.path.join(url_repo,'datasets_files_name.json') # only for linux
             url_dictionary = url_repo + '/datasets_files_name.json'
@@ -350,8 +379,8 @@
         for _ in result_show.index:
             if _ in ['Ave.rank', 'p-value']:
                 result_show.loc[_, :] = [format(round(_, 2), '.2f') for _ in result_show.loc[_, :].values]
 
         # result_show = result_show.astype('float')
         # result_show = result_show.round(2)
 
-        return result_show
+        return result_show
```

### Comparing `adbench-0.1.7/adbench/other_utils/gmm/example.py` & `adbench-0.1.8/adbench/other_utils/gmm/example.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/other_utils/gmm/gmm.py` & `adbench-0.1.8/adbench/other_utils/gmm/gmm.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/other_utils/gmm/test.py` & `adbench-0.1.8/adbench/other_utils/gmm/test.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/other_utils/gmm/utils.py` & `adbench-0.1.8/adbench/other_utils/gmm/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/other_utils/utils.py` & `adbench-0.1.8/adbench/other_utils/utils.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench/run.py` & `adbench-0.1.8/adbench/run.py`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/adbench.egg-info/PKG-INFO` & `adbench-0.1.8/adbench.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbench
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python package of ADBench
 Home-page: https://github.com/Minqi824/ADBench
 Author: Minqi Jiang
 Author-email: <jiangmq95@163.com>
 Keywords: anomaly detection,outlier detection,tabular data,benchmark
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `adbench-0.1.7/adbench.egg-info/SOURCES.txt` & `adbench-0.1.8/adbench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adbench-0.1.7/setup.py` & `adbench-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # read the contents of requirements.txt
 with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'requirements.txt'), encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 # 配置
 setup(
     name="adbench",
-    version='0.1.7',
+    version='0.1.8',
     author="Minqi Jiang",
     author_email="<jiangmq95@163.com>",
     url='https://github.com/Minqi824/ADBench',
     description='Python package of ADBench',
     long_description='Python package of ADBench: Anomaly detection benchmark. Fast implementation of the large '
                      'experiments in ADBench and your customized AD algorithm.',
     packages=find_packages(),
```

